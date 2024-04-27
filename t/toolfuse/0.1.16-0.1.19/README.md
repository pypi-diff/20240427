# Comparing `tmp/toolfuse-0.1.16.tar.gz` & `tmp/toolfuse-0.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolfuse-0.1.16.tar", max compression
+gzip compressed data, was "toolfuse-0.1.19.tar", max compression
```

## Comparing `toolfuse-0.1.16.tar` & `toolfuse-0.1.19.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.16/LICENSE
--rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.16/README.md
--rw-r--r--   0        0        0      803 2024-04-15 00:39:00.528715 toolfuse-0.1.16/pyproject.toml
--rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.16/toolfuse/__init__.py
--rw-r--r--   0        0        0    19575 2024-04-15 00:38:34.973759 toolfuse-0.1.16/toolfuse/base.py
--rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.16/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:50:27.204544 toolfuse-0.1.19/LICENSE
+-rw-r--r--   0        0        0     3333 2024-04-08 16:29:21.395807 toolfuse-0.1.19/README.md
+-rw-r--r--   0        0        0      803 2024-04-27 21:02:12.438459 toolfuse-0.1.19/pyproject.toml
+-rw-r--r--   0        0        0      341 2024-04-08 15:50:27.209682 toolfuse-0.1.19/toolfuse/__init__.py
+-rw-r--r--   0        0        0    24639 2024-04-27 21:02:27.158378 toolfuse-0.1.19/toolfuse/base.py
+-rw-r--r--   0        0        0      197 2024-04-27 21:02:03.126589 toolfuse-0.1.19/toolfuse/models.py
+-rw-r--r--   0        0        0     3978 1970-01-01 00:00:00.000000 toolfuse-0.1.19/PKG-INFO
```

### Comparing `toolfuse-0.1.16/LICENSE` & `toolfuse-0.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.16/README.md` & `toolfuse-0.1.19/README.md`

 * *Files identical despite different names*

### Comparing `toolfuse-0.1.16/pyproject.toml` & `toolfuse-0.1.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "toolfuse"
-version = "0.1.16"
+version = "0.1.19"
 description = "Tools for AI agents"
 authors = ["Patrick Barker <patrickbarkerco@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "toolfuse"}]
 
 [tool.poetry.dependencies]
```

### Comparing `toolfuse-0.1.16/toolfuse/base.py` & `toolfuse-0.1.19/toolfuse/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from abc import ABC
 from typing import List, Callable, Any, Dict, Optional, TypeVar, Type, Union
-from inspect import getdoc
+from inspect import getdoc, getmodule
 import inspect
 import re
+from importlib.metadata import version as pkgversion
 
 from toolcore import FunctionWrapper
+from .models import V1ToolRef
 
 
 class Action:
     """
     Represents an action that an agent can perform in an environment.
 
     This class is used to encapsulate information about an action, including its
@@ -331,39 +333,84 @@
         """Tool name
 
         Returns:
             str: Tool name
         """
         return cls.__name__
 
+    def ref(self) -> V1ToolRef:
+        """Tool reference"""
+        module = getmodule(self)
+        if not module:
+            raise ValueError("Tool not associated with a module")
+        version = pkgversion(module.__name__)
+        return V1ToolRef(module=module.__name__, name=self.name(), version=version)
+
 
 def tool_from_cls(cls: Type[T]) -> Type[Tool]:
     """
     Dynamically creates a subclass of `Tool` that integrates methods from a given class `cls` as actions.
 
     Args:
         cls (Type[T]): The class from which to create a Tool, integrating its methods as actions.
 
     Returns:
         Type[Tool]: A new subclass of Tool that includes actions derived from `cls` methods.
     """
 
     class Combined(Tool, cls):
+        """
+        A combined class that inherits from both Tool and a user-defined class (cls).
+
+        This class is dynamically created to combine the functionality of a user-defined class
+        with the Tool class, allowing methods from the user-defined class to be registered as actions
+        within the Tool framework. It initializes both parent classes and registers the user-defined
+        class's methods as actions.
+
+        Attributes:
+            Inherits all attributes from the Tool class and the user-defined class (cls).
+
+        Methods:
+            __init__(*args, **kwargs): Initializes the Combined class, the Tool part of the class,
+                                       and registers methods from the user-defined class as actions.
+            name(): Returns the name of the class.
+            _register_methods_from_cls(): Registers public methods from the user-defined class as actions.
+        """
+
         def __init__(self, *args, **kwargs):
-            cls.__init__(self, *args, **kwargs)  # type: ignore
+            """
+            Initializes the Combined class by initializing both the user-defined class part and the Tool class part.
+            It also registers the methods from the user-defined class (cls) as actions within the Tool framework.
+
+            Args:
+                *args: Variable length argument list passed to the user-defined class initializer.
+                **kwargs: Arbitrary keyword arguments passed to the user-defined class initializer.
+            """
+            cls.__init__(
+                self, *args, **kwargs  # type: ignore
+            )  # Initialize the user-defined part of the combined class
             Tool.__init__(self)  # Initialize the Tool part of the combined class
-            self._register_methods_from_cls()
+            self._register_methods_from_cls()  # Register methods from cls as actions
 
         @classmethod
         def name(cls) -> str:
+            """
+            Returns the name of the class.
+
+            Returns:
+                str: The name of the class.
+            """
             return cls.__name__
 
         def _register_methods_from_cls(self):
             """
-            Registers all public methods of `cls` as actions for the Tool.
+            Registers all public methods from the user-defined class (cls) as actions.
+
+            This method iterates over all public methods of cls and registers them as actions,
+            allowing them to be utilized within the Tool framework.
             """
             for name, method in inspect.getmembers(self, predicate=inspect.ismethod):
                 # Skip private and protected methods, skip methods from Tool or object class
                 if (
                     name.startswith("_")
                     or inspect.getmodule(method) == inspect.getmodule(Tool)
                     or inspect.getmodule(method) == inspect.getmodule(object)
@@ -397,22 +444,45 @@
         function (Callable): The function to be encapsulated as an action in the Tool.
 
     Returns:
         Type[Tool]: A new subclass of Tool that includes the given function as an action.
     """
 
     class FunctionTool(Tool):
+        """
+        A subclass of `Tool` designed to encapsulate a single function as an actionable method within the Tool framework.
+
+        This class takes a function upon initialization and registers it as an action, making it callable within the context of the Tool's environment. The primary purpose of this class is to allow standalone functions to be seamlessly integrated into the Tool framework, providing a straightforward way to extend functionality with custom actions.
+
+        Attributes:
+            function (Callable): The function that is encapsulated as an action within the Tool.
+
+        Methods:
+            __init__(self, function: Callable): Initializes a new instance of the FunctionTool class, registering the provided function as an action.
+            _register_function_as_action(self, function: Callable): Registers the provided function as an action for the Tool.
+        """
+
         def __init__(self):
+            """
+            Initializes a new instance of the FunctionTool class.
+
+            This constructor method takes a function as an argument and calls the internal method to register it as an action within the Tool.
+
+            Args:
+                function (Callable): The function to be encapsulated as an action in the Tool.
+            """
             super().__init__()
             self._register_function_as_action(function)
 
         def _register_function_as_action(self, function: Callable):
             """
             Registers the provided function as an action for the Tool.
 
+            This method wraps the given function to extract its schema and documentation, creating an Action instance that encapsulates the function. This allows the function to be called as an action within the Tool's environment.
+
             Args:
                 function (Callable): The function to be registered as an action.
             """
             # Wrap the function to get its schema
             wrapper = FunctionWrapper(function)
 
             # Generate a description from the function's docstring
@@ -442,22 +512,45 @@
         obj (Any): The object instance whose methods are to be encapsulated as actions in the Tool.
 
     Returns:
         Tool: A new subclass of Tool that includes the object's methods as actions.
     """
 
     class ObjectTool(Tool):
+        """
+        A subclass of `Tool` that encapsulates the methods of a given object instance as actions.
+
+        This class dynamically creates actions based on the public methods of the provided object instance. Each method is wrapped as an `Action` object, allowing it to be invoked within the Tool's environment.
+
+        Attributes:
+            obj_instance (Any): The object instance whose methods are to be encapsulated as actions.
+
+        Methods:
+            __init__(self, obj_instance: Any): Initializes a new instance of `ObjectTool` with the given object.
+            _register_methods_from_object(self): Registers all public methods of `obj_instance` as actions.
+        """
+
         def __init__(self, obj_instance: Any):
+            """
+            Initializes a new instance of `ObjectTool`.
+
+            This constructor method takes an object instance as an argument and calls the internal method to register its public methods as actions within the Tool.
+
+            Args:
+                obj_instance (Any): The object instance whose methods are to be encapsulated as actions.
+            """
             super().__init__()
             self.obj_instance = obj_instance
             self._register_methods_from_object()
 
         def _register_methods_from_object(self):
             """
             Registers all public methods of the object instance as actions for the Tool.
+
+            This method iterates over all public methods of the provided object instance, excluding private, protected, and dunder methods. Each method is wrapped as an `Action` object and added to the tool's actions list.
             """
             for name, method in inspect.getmembers(
                 self.obj_instance, predicate=inspect.ismethod
             ):
                 # Skip private and protected methods, and skip dunder methods
                 if name.startswith("_"):
                     continue
```

### Comparing `toolfuse-0.1.16/PKG-INFO` & `toolfuse-0.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolfuse
-Version: 0.1.16
+Version: 0.1.19
 Summary: Tools for AI agents
 License: MIT
 Author: Patrick Barker
 Author-email: patrickbarkerco@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

