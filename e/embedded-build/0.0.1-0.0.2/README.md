# Comparing `tmp/embedded_build-0.0.1.tar.gz` & `tmp/embedded_build-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedded_build-0.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "embedded_build-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `embedded_build-0.0.1.tar` & `embedded_build-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     3078 2024-04-26 05:03:50.620059 embedded_build-0.0.1/.gitignore
--rw-r--r--   0        0        0     1082 2024-04-26 04:35:26.293359 embedded_build-0.0.1/LICENSE
--rw-r--r--   0        0        0      250 2024-04-26 05:05:39.480062 embedded_build-0.0.1/embedded/__init__.py
--rw-r--r--   0        0        0     1266 2024-04-26 04:40:48.860032 embedded_build-0.0.1/embedded/cli.py
--rw-r--r--   0        0        0      425 2024-04-26 04:21:52.410010 embedded_build-0.0.1/embedded/compiler.py
--rw-r--r--   0        0        0      545 2024-04-26 04:26:46.776682 embedded_build-0.0.1/embedded/cpu/__init__.py
--rw-r--r--   0        0        0     2797 2024-04-26 04:57:38.176719 embedded_build-0.0.1/embedded/cpu/arm.py
--rw-r--r--   0        0        0      676 2024-04-26 04:43:56.533369 embedded_build-0.0.1/embedded/cpu/riscv.py
--rw-r--r--   0        0        0     1109 2024-04-26 04:55:06.176716 embedded_build-0.0.1/embedded/microcontroller/__init__.py
--rw-r--r--   0        0        0      398 2024-04-26 05:20:49.353413 embedded_build-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 embedded_build-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3094 2024-04-27 00:25:03.170023 embedded_build-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1082 2024-04-26 04:35:26.293359 embedded_build-0.0.2/LICENSE
+-rw-r--r--   0        0        0      250 2024-04-27 06:00:38.326796 embedded_build-0.0.2/embedded/__init__.py
+-rw-r--r--   0        0        0     1400 2024-04-27 05:37:22.113436 embedded_build-0.0.2/embedded/build/__init__.py
+-rw-r--r--   0        0        0     1645 2024-04-27 05:15:26.660076 embedded_build-0.0.2/embedded/build/meson.py
+-rw-r--r--   0        0        0      503 2024-04-27 04:13:47.420004 embedded_build-0.0.2/embedded/build/ninja.py
+-rw-r--r--   0        0        0     2552 2024-04-27 05:24:48.973421 embedded_build-0.0.2/embedded/cli.py
+-rw-r--r--   0        0        0      425 2024-04-26 04:21:52.410010 embedded_build-0.0.2/embedded/compiler.py
+-rw-r--r--   0        0        0      545 2024-04-26 04:26:46.776682 embedded_build-0.0.2/embedded/cpu/__init__.py
+-rw-r--r--   0        0        0     2727 2024-04-27 05:55:54.090124 embedded_build-0.0.2/embedded/cpu/arm.py
+-rw-r--r--   0        0        0      676 2024-04-26 04:43:56.533369 embedded_build-0.0.2/embedded/cpu/riscv.py
+-rw-r--r--   0        0        0     1052 2024-04-27 04:53:46.450051 embedded_build-0.0.2/embedded/microcontroller/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-26 05:20:49.353413 embedded_build-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 embedded_build-0.0.2/PKG-INFO
```

### Comparing `embedded_build-0.0.1/.gitignore` & `embedded_build-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
+!embedded/build
 develop-eggs/
 dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
```

### Comparing `embedded_build-0.0.1/LICENSE` & `embedded_build-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `embedded_build-0.0.1/embedded/cpu/__init__.py` & `embedded_build-0.0.2/embedded/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `embedded_build-0.0.1/embedded/cpu/arm.py` & `embedded_build-0.0.2/embedded/cpu/arm.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from typing import Optional
 
 class ARM(embedded.CPU):
     def __init__(self, mcpu: str, floating_point: bool = False, floating_point_unit: str = None):
         self.mcpu = mcpu
         self.floating_point = floating_point
         self.floating_point_unit = floating_point_unit
-        self.unique_id = mcpu + "f" if floating_point else ""
+        self.unique_id = mcpu + ("f" if floating_point else "")
 
     def get_arch_cflags(self, compiler: embedded.Compiler) -> list[str]:
         flags = ["-mthumb"]
         floating_point_unit = self.floating_point_unit
-        print(compiler)
         assert(compiler is not None)
         if isinstance(compiler, embedded.compiler.Clang):
             flags.append("--target=arm-none-eabi")
             flags.append(f"-mcpu={self.mcpu}")
             flags.append(f"-mfpu={floating_point_unit}")
         else:
             flags.append(f"-mcpu={self.mcpu}")
@@ -29,17 +28,15 @@
             flags.extend(("-mfloat-abi=hard",))
         return flags
 
     @staticmethod
     def from_pdsc(description: dict) -> Optional[embedded.CPU]:
         if "core" in description:
             core = description["core"]
-            print(core)
             if core == "CortexM0Plus":
-                print("cm0")
                 return CortexM0Plus()
             elif core == "CortexM4":
                 return CortexM4(description["fpu"])
             elif core == "CortexM7":
                 return CortexM7(description["fpu"])
             elif core == "CortexM33":
                 return CortexM33(description["fpu"])
@@ -55,15 +52,15 @@
 
 class CortexM4(ARM):
     def __init__(self, floating_point: bool):
         if floating_point:
             fp = ""
         else:
             fp = "+nofp"
-        super().__init__("cortex-m4" + fp, floating_point=floating_point, floating_point_unit="vfp4sp")
+        super().__init__("cortex-m4" + fp, floating_point=floating_point, floating_point_unit="fpv4-sp-d16")
 
 class CortexM7(ARM):
     def __init__(self, floating_point: str):
         if floating_point:
             fp = ""
         else:
             fp = "+nofp"
```

### Comparing `embedded_build-0.0.1/embedded/cpu/riscv.py` & `embedded_build-0.0.2/embedded/cpu/riscv.py`

 * *Files identical despite different names*

