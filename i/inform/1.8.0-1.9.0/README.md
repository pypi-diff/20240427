# Comparing `tmp/inform-1.8.0.tar.gz` & `tmp/inform-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/inform-1.8.0.tar", last modified: Fri Mar 31 20:53:08 2017, max compression
+gzip compressed data, was "dist/inform-1.9.0.tar", last modified: Sun Apr  2 16:33:39 2017, max compression
```

## Comparing `inform-1.8.0.tar` & `inform-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-03-31 20:53:08.000000 inform-1.8.0/
--rw-r--r--   0 ken       (1000) officers   (501)    32224 2017-03-31 20:22:17.000000 inform-1.8.0/README.rst
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-03-31 20:53:08.000000 inform-1.8.0/inform/
--rw-r--r--   0 ken       (1000) officers   (501)    31654 2017-03-27 00:41:22.000000 inform-1.8.0/inform/inform.py
--rw-r--r--   0 ken       (1000) officers   (501)      520 2017-03-31 20:22:17.000000 inform-1.8.0/inform/__init__.py
--rw-r--r--   0 ken       (1000) officers   (501)    41008 2017-03-31 20:53:08.000000 inform-1.8.0/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)     1420 2017-03-31 20:51:23.000000 inform-1.8.0/setup.py
--rw-r--r--   0 ken       (1000) officers   (501)       59 2017-03-31 20:53:08.000000 inform-1.8.0/setup.cfg
-drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/
--rw-r--r--   0 ken       (1000) officers   (501)       17 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/requires.txt
--rw-r--r--   0 ken       (1000) officers   (501)      229 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/SOURCES.txt
--rw-r--r--   0 ken       (1000) officers   (501)        1 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/dependency_links.txt
--rw-r--r--   0 ken       (1000) officers   (501)    41008 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/PKG-INFO
--rw-r--r--   0 ken       (1000) officers   (501)        7 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/top_level.txt
--rw-r--r--   0 ken       (1000) officers   (501)        1 2017-03-31 20:53:08.000000 inform-1.8.0/inform.egg-info/zip-safe
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-04-02 16:33:39.000000 inform-1.9.0/
+-rw-r--r--   0 ken       (1000) officers   (501)    32395 2017-04-02 16:32:46.000000 inform-1.9.0/README.rst
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-04-02 16:33:39.000000 inform-1.9.0/inform/
+-rw-r--r--   0 ken       (1000) officers   (501)    31624 2017-04-02 15:00:03.000000 inform-1.9.0/inform/inform.py
+-rw-r--r--   0 ken       (1000) officers   (501)      518 2017-04-02 16:23:52.000000 inform-1.9.0/inform/__init__.py
+-rw-r--r--   0 ken       (1000) officers   (501)    41355 2017-04-02 16:33:39.000000 inform-1.9.0/PKG-INFO
+-rw-r--r--   0 ken       (1000) officers   (501)     1420 2017-04-02 16:23:52.000000 inform-1.9.0/setup.py
+-rw-r--r--   0 ken       (1000) officers   (501)       59 2017-04-02 16:33:39.000000 inform-1.9.0/setup.cfg
+drwxr-xr-x   0 ken       (1000) officers   (501)        0 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/
+-rw-r--r--   0 ken       (1000) officers   (501)       17 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/requires.txt
+-rw-r--r--   0 ken       (1000) officers   (501)      229 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/SOURCES.txt
+-rw-r--r--   0 ken       (1000) officers   (501)        1 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/dependency_links.txt
+-rw-r--r--   0 ken       (1000) officers   (501)    41355 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/PKG-INFO
+-rw-r--r--   0 ken       (1000) officers   (501)        7 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/top_level.txt
+-rw-r--r--   0 ken       (1000) officers   (501)        1 2017-04-02 16:33:39.000000 inform-1.9.0/inform.egg-info/zip-safe
```

### Comparing `inform-1.8.0/README.rst` & `inform-1.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -12,81 +12,69 @@
 
 .. image:: https://img.shields.io/pypi/pyversions/inform.svg
     :target: https://pypi.python.org/pypi/inform/
 
 .. image:: https://img.shields.io/pypi/dd/inform.svg
     :target: https://pypi.python.org/pypi/inform/
 
-| Version: 1.8.0
-| Released: 2017-03-31
+| Version: 1.9.0
+| Released: 2017-04-02
 |
 
 A light-weight package with few dependencies that provides various print-like 
-functions to communicate to the user. It allows you to easily print attractive, 
-informative, and consistent error messages.  For example:
+functions that are uses when communicating with the user. It allows you to 
+easily print attractive, informative, and consistent error messages.  For 
+example:
 
 .. code-block:: python
 
     >> from inform import display, warn, error
-    >> display('Display is like print, except that it support logging and can be disabled.')
-    Display is like print, except that it support logging and can be disabled.
+    >> display(
+    ..     'Display is like print'
+    ..     'except that it supports logging and can be disabled.'
+    ..     sep=', ')
+    Display is like print, except that it supports logging and can be disabled.
 
     >> warn('warnings get a header that is printed in yellow.')
     warning: warnings get a header that is printed in yellow.
 
-    >> error('erros get a header that is printed in red.')
-    error: warnings get a header that is printed in red.
+    >> error('errors get a header that is printed in red.')
+    error: errors get a header that is printed in red.
 
-Inform also supports normal best practices such as providing logging and output 
-control and adding the program name to error messages.
+Inform also provides logging and output control.
 
 Install with::
 
     pip install inform
 
 Supported in Python2.7, Python3.3, Python3.4, Python3.5, and Python3.6.
 
+
+Introduction
+------------
+
 This package defines a collection of 'print' functions that have different 
 roles.  These functions are referred to as 'informants' and are described below 
-in the the Informants section. They include include *log*, *comment*, *codicil*, 
+in the Informants section. They include include *log*, *comment*, *codicil*, 
 *narrate*, *display*, *output*, *notify*, *debug*, *warn*, *error*, *fatal* and 
-*panic*.  Each of these functions takes arguments like the standard print 
-function: unnamed arguments are converted to strings and joined together to 
-produce the output, the named arguments act to control the process.  The 
-available controls (named arguments) are:
-
-sep = ' ':
-   Specifies the string used to join the unnamed arguments.
-end = '\\n':
-   Specifies a string to append to the message.
-file = stdout:
-   The destination stream (a file pointer).
-flush = *False*:
-   Whether the message should flush the destination stream (not available in 
-   python2).
-culprit = *None*:
-   A string that is added to the beginning of the message that identifies the 
-   culprit (the object for which the problem being reported was found). May also 
-   be a collection of strings, in which case they are joined with '.'.
-hanging = *True*:
-   Indicates hanging indentation should be used when outputting multi-line 
-   message with headers or culprits.
+*panic*.
 
 With the simplest use of the program, you simply import the informants you need 
-and call them (they take the same arguments as does the *print* function built 
-into Python:
+and call them (they take the same arguments as Python's built-in *print* 
+function):
 
 .. code-block:: python
 
     >>> from inform import display
     >>> display('ice', 9)
     ice 9
 
-More typical is to import and instantiate the Inform class yourself along with 
-the desired informants.  This gives you the ability to specify options:
+For more control of the informants, you can import and instantiate the Inform 
+class yourself along with the desired informants.  This gives you the ability to 
+specify options:
 
 .. code-block:: python
 
     >>> from inform import Inform, display, error
     >>> Inform(logfile=False, prog_name=False)
     <...>
     >>> display('hello')
@@ -154,18 +142,18 @@
     >>> str(logfile_text[:10]), str(logfile_text[-13:])
     ('Invoked as', 'running test\n')
 
 You can create your own informants:
 
 .. code-block:: python
 
-    >>> from inform import Inform, InformantGenerator
+    >>> from inform import Inform, InformantFactory
 
-    >>> verbose1 = InformantGenerator(output=lambda m: m.verbosity >= 1)
-    >>> verbose2 = InformantGenerator(output=lambda m: m.verbosity >= 2)
+    >>> verbose1 = InformantFactory(output=lambda m: m.verbosity >= 1)
+    >>> verbose2 = InformantFactory(output=lambda m: m.verbosity >= 2)
     >>> with Inform(verbosity=0):
     ...     verbose1('First level of verbosity.')
     ...     verbose2('Second level of verbosity.')
 
     >>> with Inform(verbosity=1):
     ...     verbose1('First level of verbosity.')
     ...     verbose2('Second level of verbosity.')
@@ -176,15 +164,15 @@
     ...     verbose2('Second level of verbosity.')
     First level of verbosity.
     Second level of verbosity.
 
 The argument *verbosity* is not an explicitly supported argument to Inform.  In 
 this case Inform simply saves the value and makes it available as an attribute, 
 and it is this attribute that is queried by the lambda function passed to the 
-InformantGenerator when creating the informants.
+InformantFactory when creating the informants.
 
 
 Exception
 ---------
 An exception, *Error*, is provided that takes the same arguments as an 
 informant.  This allows you to catch the exception and handle it if you like.  
 The exception provides the *report* and *terminate* methods that processes the 
@@ -327,17 +315,17 @@
 functionality even if you do not have local access to the informer. They are:
 
 | done()
 | terminate()
 | terminate_if_errors()
 | errors_accrued()
 
-InformantGenerator Class
-------------------------
-The InformantGenerator class takes the following arguments:
+InformantFactory Class
+----------------------
+The InformantFactory class takes the following arguments:
 
 severity = *None*:
    Messages with severities get headers. The header consists of the severity, 
    the program name (if desired), and the culprit (if provided). If the message 
    text does not contain a newline it is appended to the header.  Otherwise the 
    message text is indented and placed on the next line.
 is_error = *False*:
@@ -363,23 +351,23 @@
    message is indented.
 message_color = *None*:
    Color used to display the message. Choose from *black*, *red*, *green*, 
    *yellow*, *blue*, *magenta*, *cyan*, *white*.
 header_color = *None*:
    Color used to display the header, if one is produced.
 
-An object of InformantGenerator is referred to as an informant. It is generally 
+An object of InformantFactory is referred to as an informant. It is generally 
 treated as a function that is called to produce the desired output.
 
 .. code-block:: python
 
-    >>> from inform import InformantGenerator
+    >>> from inform import InformantFactory
 
-    >>> succeed = InformantGenerator(message_color='green')
-    >>> fail = InformantGenerator(message_color='red')
+    >>> succeed = InformantFactory(message_color='green')
+    >>> fail = InformantFactory(message_color='red')
 
     >>> succeed('This message would be green.')
     This message would be green.
 
     >>> fail('This message would be red.')
     This message would be red.
 
@@ -391,28 +379,28 @@
 debug do not produce any output if *mute* is set.
 
 log
 """
 
 .. code-block:: python
 
-   log = InformantGenerator(
+   log = InformantFactory(
        output=False,
        log=True,
    )
 
 Saves a message to the log file without displaying it.
 
 
 comment
 """""""
 
 .. code-block:: python
 
-   comment = InformantGenerator(
+   comment = InformantFactory(
        output=lambda informer: informer.verbose and not informer.mute,
        log=True,
        message_color='cyan',
    )
 
 Displays a message only if *verbose* is set. Logs the message. The message is 
 displayed in cyan.
@@ -421,15 +409,15 @@
 the user's attention.
 
 codicil
 """""""
 
 .. code-block:: python
 
-   codicil = InformantGenerator(is_continuation=True)
+   codicil = InformantFactory(is_continuation=True)
 
 Continues a previous message. Continued messages inherit the properties (output, 
 log, message color, etc) of the previous message.  If the previous message had 
 a header, that header is not output and instead the message is indented.
 
 .. code-block:: python
 
@@ -443,15 +431,15 @@
 
 
 narrate
 """""""
 
 .. code-block:: python
 
-   narrate = InformantGenerator(
+   narrate = InformantFactory(
        output=lambda informer: informer.narrate and not informer.mute,
        log=True,
        message_color='blue',
    )
 
 Displays a message only if *narrate* is set. Logs the message. The message is 
 displayed in blue.
@@ -463,15 +451,15 @@
 
 
 display
 """""""
 
 .. code-block:: python
 
-   display = InformantGenerator(
+   display = InformantFactory(
        output=lambda informer: not informer.quiet and not informer.mute,
        log=True,
    )
 
 Displays a message if *quiet* is not set. Logs the message.
 
 .. code-block:: python
@@ -482,15 +470,15 @@
 
 
 output
 """"""
 
 .. code-block:: python
 
-   output = InformantGenerator(
+   output = InformantFactory(
        output=lambda informer: not informer.mute,
        log=True,
    )
 
 Displays and logs a message. This is used for messages that are not errors that 
 are noteworthy enough that they need to get through even though the user has 
 asked for quiet.
@@ -503,15 +491,15 @@
 
 
 notify
 """"""
 
 .. code-block:: python
 
-   notify = InformantGenerator(
+   notify = InformantFactory(
        notify=True,
        log=True,
    )
 
 Temporarily display the message in a bubble at the top of the screen.  Also 
 prints the message on the standard output and sends it to the log file.  This is 
 used for messages that the user is otherwise unlikely to see because they have 
@@ -525,15 +513,15 @@
 
 
 debug
 """""
 
 .. code-block:: python
 
-   debug = InformantGenerator(
+   debug = InformantFactory(
        severity='DEBUG',
        output=True,
        log=True,
        header_color='magenta',
    )
 
 Displays and logs a debugging message. A header with the label *DEBUG* is added 
@@ -551,15 +539,15 @@
 
 
 warn
 """"
 
 .. code-block:: python
 
-   warn = InformantGenerator(
+   warn = InformantFactory(
        severity='warning',
        header_color='yellow',
        output=lambda informer: not informer.quiet and not informer.mute,
        log=True,
    )
 
 Displays and logs a warning message. A header with the label *warning* is added 
@@ -574,15 +562,15 @@
 
 
 error
 """""
 
 .. code-block:: python
 
-   error = InformantGenerator(
+   error = InformantFactory(
        severity='error',
        is_error=True,
        header_color='red',
        output=lambda informer: not informer.mute,
        log=True,
    )
 
@@ -597,15 +585,15 @@
     myprog error: count: invalid value specified, expected number.
 
 fatal
 """""
 
 .. code-block:: python
 
-   fatal = InformantGenerator(
+   fatal = InformantFactory(
        severity='error',
        is_error=True,
        terminate=1,
        header_color='red',
        output=lambda informer: not informer.mute,
        log=True,
    )
@@ -616,28 +604,54 @@
 
 
 panic
 """""
 
 .. code-block:: python
 
-   panic = InformantGenerator(
+   panic = InformantFactory(
        severity='internal error (please report)',
        is_error=True,
        terminate=3,
        header_color='red',
        output=True,
        log=True,
    )
 
 Displays and logs a panic message. A header with the label *internal error* is 
 added to the message and the header is colored red. The program is terminated 
 with an exit status of 3.
 
 
+Informant Control
+-----------------
+
+The exeception (Error) and all informants take arguments very much like the 
+standard print function: unnamed arguments are converted to strings and joined 
+together to produce the output, the named arguments act to control the process.  
+The available controls (named arguments) are:
+
+sep = ' ':
+   Specifies the string used to join the unnamed arguments.
+end = '\\n':
+   Specifies a string to append to the message.
+file = stdout:
+   The destination stream (a file pointer).
+flush = *False*:
+   Whether the message should flush the destination stream (not available in 
+   python2).
+culprit = *None*:
+   A string that is added to the beginning of the message that identifies the 
+   culprit (the object for which the problem being reported was found). May also 
+   be a collection of strings, in which case they are joined with '.'.
+hanging = *True*:
+   Indicates hanging indentation should be used when outputting multi-line 
+   message with headers or culprits.
+
+
 Utilities
 ---------
 
 Several utility functions are provided for your convenience. They are often 
 helpful when creating messages.
 
 indent(text, leader='    ',  first=0, stops=1, sep='\\n'):
@@ -645,16 +659,24 @@
     lines to indent.  *first* is the number of indentations used for the first 
     line relative to the others (may be negative but (first + stops) should not 
     be. *stops* is the default number of indentations to use. *sep* is the 
     string used to separate the lines.
 
 conjoin(iterable, conj=' and ', sep=', '):
     Like ''.join(), but allows you to specify a conjunction that is placed 
-    between the last two elements, ex: conjoin(['a', 'b', 'c'], conj=' or ') 
-    generates 'a, b or c'.
+    between the last two elements, ex:
+
+    .. code-block:: python
+
+        >>> from inform import conjoin
+        >>> conjoin(['a', 'b', 'c'])
+        'a, b and c'
+
+        >>> conjoin(['a', 'b', 'c'], conj=' or ')
+        'a, b or c'
 
 cull(collection, [remove]):
     Strips items from a list that have a particular value. By default, it strips 
     a list of values that if casted to a boolean would have a value of False (0, 
     False, None, '', (), [], etc.).  A particular value may be specified using 
     the 'remove' as a keyword argument.  The value of remove may be a function, 
     in which case it takes a single item as an argument and returns *True* if 
@@ -804,39 +826,39 @@
 
         >>> from inform import ppp, ddd, vvv
         >>> a = 1
         >>> b = 'this is a test'
         >>> c = (2, 3)
         >>> d = {'a': a, 'b': b, 'c': c}
         >>> ppp(a, b, c)
-        DEBUG: <doctest README.rst[75]>:1, __main__:
+        DEBUG: <doctest README.rst[78]>:1, __main__:
             1 this is a test (2, 3)
 
 ddd(\*args, \*\*kwyargs):
     This function is pretty prints all of both the unnamed and named arguments.
 
     .. code:: python
 
         >>> ddd(a, b, c, d)
-        DEBUG: <doctest README.rst[76]>:1, __main__:
+        DEBUG: <doctest README.rst[79]>:1, __main__:
             1
             'this is a test'
             (2, 3)
             {
                 'a': 1,
                 'b': 'this is a test',
                 'c': (2, 3),
             }
 
     If you give named arguments, the name is prepended to its value:
 
     .. code:: python
 
         >>> ddd(a=a, b=b, c=c, d=d, s='hey now!')
-        DEBUG: <doctest README.rst[77]>:1, __main__:
+        DEBUG: <doctest README.rst[80]>:1, __main__:
             a = 1
             b = 'this is a test'
             c = (2, 3)
             d = {
                 'a': 1,
                 'b': 'this is a test',
                 'c': (2, 3),
@@ -850,29 +872,29 @@
 
         >>> class Info:
         ...     def __init__(self, **kwargs):
         ...         self.__dict__.update(kwargs)
         ...         ddd(self=self)
 
         >>> contact = Info(email='ted@ledbelly.com', name='Ted Ledbelly')
-        DEBUG: <doctest README.rst[78]>:4, __main__.Info.__init__():
+        DEBUG: <doctest README.rst[81]>:4, __main__.Info.__init__():
             self = {
                 'email': 'ted@ledbelly.com',
                 'name': 'Ted Ledbelly',
             }
 
 vvv(\*args):
     This function prints variables from the calling scope. If no arguments are 
     given, then all the variables are printed. You can optionally give specific 
     variables on the argument list and only those variables are printed.
 
     .. code:: python
 
         >>> vvv(b, d)
-        DEBUG: <doctest README.rst[80]>:1, __main__:
+        DEBUG: <doctest README.rst[83]>:1, __main__:
             b = 'this is a test'
             d = {
                 'a': 1,
                 'b': 'this is a test',
                 'c': (2, 3),
             }
 
@@ -880,15 +902,15 @@
     so if several variables share the value of one requested, they are all 
     shown.
 
     .. code:: python
 
         >>> aa = 1
         >>> vvv(a)
-        DEBUG: <doctest README.rst[82]>:1, __main__:
+        DEBUG: <doctest README.rst[85]>:1, __main__:
             a = 1
             aa = 1
 
 
 Color Class
 """""""""""
```

### Comparing `inform-1.8.0/inform/inform.py` & `inform-1.9.0/inform/inform.py`

 * *Files 3% similar despite different names*

```diff
@@ -409,19 +409,19 @@
         if not k.startswith('_')
         if not isinstance(v, (FunctionType, type, ModuleType))
         if not args or v in args
     ]
     _debug(frame_depth, args, kwargs={'sep':'\n'})
 
 
-# InformantGenerator class {{{1
+# InformantFactory class {{{1
 # A bit of terminology. The active Inform object is called the informer, 
-# whereas the print functions returned from InformantGenerator are referred to 
+# whereas the print functions returned from InformantFactory are referred to 
 # as informants.
-class InformantGenerator:
+class InformantFactory:
     def __init__(
         self,
         severity=None,
         is_error=False,
         log=True,
         output=True,
         notify=False,
@@ -508,72 +508,72 @@
         try:
             return self.notify(informer)
         except TypeError:
             return self.notify
 
 
 # Informants {{{1
-log = InformantGenerator(
+log = InformantFactory(
     output=False,
     log=True,
 )
-comment = InformantGenerator(
+comment = InformantFactory(
     output=lambda inform: inform.verbose and not inform.mute,
     log=True,
     message_color='cyan',
 )
-codicil = InformantGenerator(
+codicil = InformantFactory(
     is_continuation=True,
 )
-narrate = InformantGenerator(
+narrate = InformantFactory(
     output=lambda inform: inform.narrate and not inform.mute,
     log=True,
     message_color='blue',
 )
-display = InformantGenerator(
+display = InformantFactory(
     output=lambda inform: not inform.quiet and not inform.mute,
     log=True,
 )
-output = InformantGenerator(
+output = InformantFactory(
     output=lambda inform: not inform.mute,
     log=True,
 )
-notify = InformantGenerator(
+notify = InformantFactory(
     output=lambda inform: not inform.quiet and not inform.mute,
     notify=True,
     log=True,
 )
-debug = InformantGenerator(
+debug = InformantFactory(
     severity='DEBUG',
     output=True,
     log=True,
     header_color='magenta',
 )
-warn = InformantGenerator(
+warn = InformantFactory(
     severity='warning',
     header_color='yellow',
     output=lambda inform: not inform.quiet and not inform.mute,
     log=True,
 )
-error = InformantGenerator(
+error = InformantFactory(
     severity='error',
     is_error=True,
     header_color='red',
     output=lambda inform: not inform.mute,
     log=True,
 )
-fatal = InformantGenerator(
+fatal = InformantFactory(
     severity='error',
     is_error=True,
     terminate=1,
     header_color='red',
     output=lambda inform: not inform.mute,
     log=True,
 )
-panic = InformantGenerator(
+panic = InformantFactory(
     severity='internal error (please report)',
     is_error=True,
     terminate=3,
     header_color='red',
     output=True,
     log=True,
 )
```

### Comparing `inform-1.8.0/inform/__init__.py` & `inform-1.9.0/inform/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-__version__ = '1.8.0'
-__released__ = '2017-03-31'
+__version__ = '1.9.0'
+__released__ = '2017-04-02'
 
 from .inform import (
     # inform utilities
     indent, cull, is_str, is_iterable, is_collection,
 
     # user utilities
     Color, fmt, render, os_error, conjoin, plural, full_stop, ppp, ddd, vvv,
 
     # inform classes
-    InformantGenerator, Inform, Error,
+    InformantFactory, Inform, Error,
 
     # inform functions
     done, terminate, terminate_if_errors, errors_accrued,
 
     # built-in informants
     log, comment, codicil, narrate, display, output,
     notify, debug, warn, error, fatal, panic,
```

### Comparing `inform-1.8.0/PKG-INFO` & `inform-1.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inform
-Version: 1.8.0
+Version: 1.9.0
 Summary: print & logging utilities for communicating with user
 Home-page: http://nurdletech.com/linux-utilities/inform
 Author: Ken Kundert
 Author-email: inform@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/inform/tarball/master
 Description: Inform - Print & Logging Utilities
@@ -21,81 +21,69 @@
         
         .. image:: https://img.shields.io/pypi/pyversions/inform.svg
             :target: https://pypi.python.org/pypi/inform/
         
         .. image:: https://img.shields.io/pypi/dd/inform.svg
             :target: https://pypi.python.org/pypi/inform/
         
-        | Version: 1.8.0
-        | Released: 2017-03-31
+        | Version: 1.9.0
+        | Released: 2017-04-02
         |
         
         A light-weight package with few dependencies that provides various print-like 
-        functions to communicate to the user. It allows you to easily print attractive, 
-        informative, and consistent error messages.  For example:
+        functions that are uses when communicating with the user. It allows you to 
+        easily print attractive, informative, and consistent error messages.  For 
+        example:
         
         .. code-block:: python
         
             >> from inform import display, warn, error
-            >> display('Display is like print, except that it support logging and can be disabled.')
-            Display is like print, except that it support logging and can be disabled.
+            >> display(
+            ..     'Display is like print'
+            ..     'except that it supports logging and can be disabled.'
+            ..     sep=', ')
+            Display is like print, except that it supports logging and can be disabled.
         
             >> warn('warnings get a header that is printed in yellow.')
             warning: warnings get a header that is printed in yellow.
         
-            >> error('erros get a header that is printed in red.')
-            error: warnings get a header that is printed in red.
+            >> error('errors get a header that is printed in red.')
+            error: errors get a header that is printed in red.
         
-        Inform also supports normal best practices such as providing logging and output 
-        control and adding the program name to error messages.
+        Inform also provides logging and output control.
         
         Install with::
         
             pip install inform
         
         Supported in Python2.7, Python3.3, Python3.4, Python3.5, and Python3.6.
         
+        
+        Introduction
+        ------------
+        
         This package defines a collection of 'print' functions that have different 
         roles.  These functions are referred to as 'informants' and are described below 
-        in the the Informants section. They include include *log*, *comment*, *codicil*, 
+        in the Informants section. They include include *log*, *comment*, *codicil*, 
         *narrate*, *display*, *output*, *notify*, *debug*, *warn*, *error*, *fatal* and 
-        *panic*.  Each of these functions takes arguments like the standard print 
-        function: unnamed arguments are converted to strings and joined together to 
-        produce the output, the named arguments act to control the process.  The 
-        available controls (named arguments) are:
-        
-        sep = ' ':
-           Specifies the string used to join the unnamed arguments.
-        end = '\\n':
-           Specifies a string to append to the message.
-        file = stdout:
-           The destination stream (a file pointer).
-        flush = *False*:
-           Whether the message should flush the destination stream (not available in 
-           python2).
-        culprit = *None*:
-           A string that is added to the beginning of the message that identifies the 
-           culprit (the object for which the problem being reported was found). May also 
-           be a collection of strings, in which case they are joined with '.'.
-        hanging = *True*:
-           Indicates hanging indentation should be used when outputting multi-line 
-           message with headers or culprits.
+        *panic*.
         
         With the simplest use of the program, you simply import the informants you need 
-        and call them (they take the same arguments as does the *print* function built 
-        into Python:
+        and call them (they take the same arguments as Python's built-in *print* 
+        function):
         
         .. code-block:: python
         
             >>> from inform import display
             >>> display('ice', 9)
             ice 9
         
-        More typical is to import and instantiate the Inform class yourself along with 
-        the desired informants.  This gives you the ability to specify options:
+        For more control of the informants, you can import and instantiate the Inform 
+        class yourself along with the desired informants.  This gives you the ability to 
+        specify options:
         
         .. code-block:: python
         
             >>> from inform import Inform, display, error
             >>> Inform(logfile=False, prog_name=False)
             <...>
             >>> display('hello')
@@ -163,18 +151,18 @@
             >>> str(logfile_text[:10]), str(logfile_text[-13:])
             ('Invoked as', 'running test\n')
         
         You can create your own informants:
         
         .. code-block:: python
         
-            >>> from inform import Inform, InformantGenerator
+            >>> from inform import Inform, InformantFactory
         
-            >>> verbose1 = InformantGenerator(output=lambda m: m.verbosity >= 1)
-            >>> verbose2 = InformantGenerator(output=lambda m: m.verbosity >= 2)
+            >>> verbose1 = InformantFactory(output=lambda m: m.verbosity >= 1)
+            >>> verbose2 = InformantFactory(output=lambda m: m.verbosity >= 2)
             >>> with Inform(verbosity=0):
             ...     verbose1('First level of verbosity.')
             ...     verbose2('Second level of verbosity.')
         
             >>> with Inform(verbosity=1):
             ...     verbose1('First level of verbosity.')
             ...     verbose2('Second level of verbosity.')
@@ -185,15 +173,15 @@
             ...     verbose2('Second level of verbosity.')
             First level of verbosity.
             Second level of verbosity.
         
         The argument *verbosity* is not an explicitly supported argument to Inform.  In 
         this case Inform simply saves the value and makes it available as an attribute, 
         and it is this attribute that is queried by the lambda function passed to the 
-        InformantGenerator when creating the informants.
+        InformantFactory when creating the informants.
         
         
         Exception
         ---------
         An exception, *Error*, is provided that takes the same arguments as an 
         informant.  This allows you to catch the exception and handle it if you like.  
         The exception provides the *report* and *terminate* methods that processes the 
@@ -336,17 +324,17 @@
         functionality even if you do not have local access to the informer. They are:
         
         | done()
         | terminate()
         | terminate_if_errors()
         | errors_accrued()
         
-        InformantGenerator Class
-        ------------------------
-        The InformantGenerator class takes the following arguments:
+        InformantFactory Class
+        ----------------------
+        The InformantFactory class takes the following arguments:
         
         severity = *None*:
            Messages with severities get headers. The header consists of the severity, 
            the program name (if desired), and the culprit (if provided). If the message 
            text does not contain a newline it is appended to the header.  Otherwise the 
            message text is indented and placed on the next line.
         is_error = *False*:
@@ -372,23 +360,23 @@
            message is indented.
         message_color = *None*:
            Color used to display the message. Choose from *black*, *red*, *green*, 
            *yellow*, *blue*, *magenta*, *cyan*, *white*.
         header_color = *None*:
            Color used to display the header, if one is produced.
         
-        An object of InformantGenerator is referred to as an informant. It is generally 
+        An object of InformantFactory is referred to as an informant. It is generally 
         treated as a function that is called to produce the desired output.
         
         .. code-block:: python
         
-            >>> from inform import InformantGenerator
+            >>> from inform import InformantFactory
         
-            >>> succeed = InformantGenerator(message_color='green')
-            >>> fail = InformantGenerator(message_color='red')
+            >>> succeed = InformantFactory(message_color='green')
+            >>> fail = InformantFactory(message_color='red')
         
             >>> succeed('This message would be green.')
             This message would be green.
         
             >>> fail('This message would be red.')
             This message would be red.
         
@@ -400,28 +388,28 @@
         debug do not produce any output if *mute* is set.
         
         log
         """
         
         .. code-block:: python
         
-           log = InformantGenerator(
+           log = InformantFactory(
                output=False,
                log=True,
            )
         
         Saves a message to the log file without displaying it.
         
         
         comment
         """""""
         
         .. code-block:: python
         
-           comment = InformantGenerator(
+           comment = InformantFactory(
                output=lambda informer: informer.verbose and not informer.mute,
                log=True,
                message_color='cyan',
            )
         
         Displays a message only if *verbose* is set. Logs the message. The message is 
         displayed in cyan.
@@ -430,15 +418,15 @@
         the user's attention.
         
         codicil
         """""""
         
         .. code-block:: python
         
-           codicil = InformantGenerator(is_continuation=True)
+           codicil = InformantFactory(is_continuation=True)
         
         Continues a previous message. Continued messages inherit the properties (output, 
         log, message color, etc) of the previous message.  If the previous message had 
         a header, that header is not output and instead the message is indented.
         
         .. code-block:: python
         
@@ -452,15 +440,15 @@
         
         
         narrate
         """""""
         
         .. code-block:: python
         
-           narrate = InformantGenerator(
+           narrate = InformantFactory(
                output=lambda informer: informer.narrate and not informer.mute,
                log=True,
                message_color='blue',
            )
         
         Displays a message only if *narrate* is set. Logs the message. The message is 
         displayed in blue.
@@ -472,15 +460,15 @@
         
         
         display
         """""""
         
         .. code-block:: python
         
-           display = InformantGenerator(
+           display = InformantFactory(
                output=lambda informer: not informer.quiet and not informer.mute,
                log=True,
            )
         
         Displays a message if *quiet* is not set. Logs the message.
         
         .. code-block:: python
@@ -491,15 +479,15 @@
         
         
         output
         """"""
         
         .. code-block:: python
         
-           output = InformantGenerator(
+           output = InformantFactory(
                output=lambda informer: not informer.mute,
                log=True,
            )
         
         Displays and logs a message. This is used for messages that are not errors that 
         are noteworthy enough that they need to get through even though the user has 
         asked for quiet.
@@ -512,15 +500,15 @@
         
         
         notify
         """"""
         
         .. code-block:: python
         
-           notify = InformantGenerator(
+           notify = InformantFactory(
                notify=True,
                log=True,
            )
         
         Temporarily display the message in a bubble at the top of the screen.  Also 
         prints the message on the standard output and sends it to the log file.  This is 
         used for messages that the user is otherwise unlikely to see because they have 
@@ -534,15 +522,15 @@
         
         
         debug
         """""
         
         .. code-block:: python
         
-           debug = InformantGenerator(
+           debug = InformantFactory(
                severity='DEBUG',
                output=True,
                log=True,
                header_color='magenta',
            )
         
         Displays and logs a debugging message. A header with the label *DEBUG* is added 
@@ -560,15 +548,15 @@
         
         
         warn
         """"
         
         .. code-block:: python
         
-           warn = InformantGenerator(
+           warn = InformantFactory(
                severity='warning',
                header_color='yellow',
                output=lambda informer: not informer.quiet and not informer.mute,
                log=True,
            )
         
         Displays and logs a warning message. A header with the label *warning* is added 
@@ -583,15 +571,15 @@
         
         
         error
         """""
         
         .. code-block:: python
         
-           error = InformantGenerator(
+           error = InformantFactory(
                severity='error',
                is_error=True,
                header_color='red',
                output=lambda informer: not informer.mute,
                log=True,
            )
         
@@ -606,15 +594,15 @@
             myprog error: count: invalid value specified, expected number.
         
         fatal
         """""
         
         .. code-block:: python
         
-           fatal = InformantGenerator(
+           fatal = InformantFactory(
                severity='error',
                is_error=True,
                terminate=1,
                header_color='red',
                output=lambda informer: not informer.mute,
                log=True,
            )
@@ -625,28 +613,54 @@
         
         
         panic
         """""
         
         .. code-block:: python
         
-           panic = InformantGenerator(
+           panic = InformantFactory(
                severity='internal error (please report)',
                is_error=True,
                terminate=3,
                header_color='red',
                output=True,
                log=True,
            )
         
         Displays and logs a panic message. A header with the label *internal error* is 
         added to the message and the header is colored red. The program is terminated 
         with an exit status of 3.
         
         
+        Informant Control
+        -----------------
+        
+        The exeception (Error) and all informants take arguments very much like the 
+        standard print function: unnamed arguments are converted to strings and joined 
+        together to produce the output, the named arguments act to control the process.  
+        The available controls (named arguments) are:
+        
+        sep = ' ':
+           Specifies the string used to join the unnamed arguments.
+        end = '\\n':
+           Specifies a string to append to the message.
+        file = stdout:
+           The destination stream (a file pointer).
+        flush = *False*:
+           Whether the message should flush the destination stream (not available in 
+           python2).
+        culprit = *None*:
+           A string that is added to the beginning of the message that identifies the 
+           culprit (the object for which the problem being reported was found). May also 
+           be a collection of strings, in which case they are joined with '.'.
+        hanging = *True*:
+           Indicates hanging indentation should be used when outputting multi-line 
+           message with headers or culprits.
+        
+        
         Utilities
         ---------
         
         Several utility functions are provided for your convenience. They are often 
         helpful when creating messages.
         
         indent(text, leader='    ',  first=0, stops=1, sep='\\n'):
@@ -654,16 +668,24 @@
             lines to indent.  *first* is the number of indentations used for the first 
             line relative to the others (may be negative but (first + stops) should not 
             be. *stops* is the default number of indentations to use. *sep* is the 
             string used to separate the lines.
         
         conjoin(iterable, conj=' and ', sep=', '):
             Like ''.join(), but allows you to specify a conjunction that is placed 
-            between the last two elements, ex: conjoin(['a', 'b', 'c'], conj=' or ') 
-            generates 'a, b or c'.
+            between the last two elements, ex:
+        
+            .. code-block:: python
+        
+                >>> from inform import conjoin
+                >>> conjoin(['a', 'b', 'c'])
+                'a, b and c'
+        
+                >>> conjoin(['a', 'b', 'c'], conj=' or ')
+                'a, b or c'
         
         cull(collection, [remove]):
             Strips items from a list that have a particular value. By default, it strips 
             a list of values that if casted to a boolean would have a value of False (0, 
             False, None, '', (), [], etc.).  A particular value may be specified using 
             the 'remove' as a keyword argument.  The value of remove may be a function, 
             in which case it takes a single item as an argument and returns *True* if 
@@ -813,39 +835,39 @@
         
                 >>> from inform import ppp, ddd, vvv
                 >>> a = 1
                 >>> b = 'this is a test'
                 >>> c = (2, 3)
                 >>> d = {'a': a, 'b': b, 'c': c}
                 >>> ppp(a, b, c)
-                DEBUG: <doctest README.rst[75]>:1, __main__:
+                DEBUG: <doctest README.rst[78]>:1, __main__:
                     1 this is a test (2, 3)
         
         ddd(\*args, \*\*kwyargs):
             This function is pretty prints all of both the unnamed and named arguments.
         
             .. code:: python
         
                 >>> ddd(a, b, c, d)
-                DEBUG: <doctest README.rst[76]>:1, __main__:
+                DEBUG: <doctest README.rst[79]>:1, __main__:
                     1
                     'this is a test'
                     (2, 3)
                     {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
                     }
         
             If you give named arguments, the name is prepended to its value:
         
             .. code:: python
         
                 >>> ddd(a=a, b=b, c=c, d=d, s='hey now!')
-                DEBUG: <doctest README.rst[77]>:1, __main__:
+                DEBUG: <doctest README.rst[80]>:1, __main__:
                     a = 1
                     b = 'this is a test'
                     c = (2, 3)
                     d = {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
@@ -859,29 +881,29 @@
         
                 >>> class Info:
                 ...     def __init__(self, **kwargs):
                 ...         self.__dict__.update(kwargs)
                 ...         ddd(self=self)
         
                 >>> contact = Info(email='ted@ledbelly.com', name='Ted Ledbelly')
-                DEBUG: <doctest README.rst[78]>:4, __main__.Info.__init__():
+                DEBUG: <doctest README.rst[81]>:4, __main__.Info.__init__():
                     self = {
                         'email': 'ted@ledbelly.com',
                         'name': 'Ted Ledbelly',
                     }
         
         vvv(\*args):
             This function prints variables from the calling scope. If no arguments are 
             given, then all the variables are printed. You can optionally give specific 
             variables on the argument list and only those variables are printed.
         
             .. code:: python
         
                 >>> vvv(b, d)
-                DEBUG: <doctest README.rst[80]>:1, __main__:
+                DEBUG: <doctest README.rst[83]>:1, __main__:
                     b = 'this is a test'
                     d = {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
                     }
         
@@ -889,15 +911,15 @@
             so if several variables share the value of one requested, they are all 
             shown.
         
             .. code:: python
         
                 >>> aa = 1
                 >>> vvv(a)
-                DEBUG: <doctest README.rst[82]>:1, __main__:
+                DEBUG: <doctest README.rst[85]>:1, __main__:
                     a = 1
                     aa = 1
         
         
         Color Class
         """""""""""
```

### Comparing `inform-1.8.0/setup.py` & `inform-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 if sys.version_info < (3,4):
     dependencies='arrow six pathlib'
 else:
     dependencies='arrow six'
 
 setup(
     name='inform',
-    version='1.8.0',
+    version='1.9.0',
     description='print & logging utilities for communicating with user',
     long_description=readme,
     author="Ken Kundert",
     author_email='inform@nurdletech.com',
     url='http://nurdletech.com/linux-utilities/inform',
     download_url='https://github.com/kenkundert/inform/tarball/master',
     license='GPLv3+',
```

### Comparing `inform-1.8.0/inform.egg-info/PKG-INFO` & `inform-1.9.0/inform.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: inform
-Version: 1.8.0
+Version: 1.9.0
 Summary: print & logging utilities for communicating with user
 Home-page: http://nurdletech.com/linux-utilities/inform
 Author: Ken Kundert
 Author-email: inform@nurdletech.com
 License: GPLv3+
 Download-URL: https://github.com/kenkundert/inform/tarball/master
 Description: Inform - Print & Logging Utilities
@@ -21,81 +21,69 @@
         
         .. image:: https://img.shields.io/pypi/pyversions/inform.svg
             :target: https://pypi.python.org/pypi/inform/
         
         .. image:: https://img.shields.io/pypi/dd/inform.svg
             :target: https://pypi.python.org/pypi/inform/
         
-        | Version: 1.8.0
-        | Released: 2017-03-31
+        | Version: 1.9.0
+        | Released: 2017-04-02
         |
         
         A light-weight package with few dependencies that provides various print-like 
-        functions to communicate to the user. It allows you to easily print attractive, 
-        informative, and consistent error messages.  For example:
+        functions that are uses when communicating with the user. It allows you to 
+        easily print attractive, informative, and consistent error messages.  For 
+        example:
         
         .. code-block:: python
         
             >> from inform import display, warn, error
-            >> display('Display is like print, except that it support logging and can be disabled.')
-            Display is like print, except that it support logging and can be disabled.
+            >> display(
+            ..     'Display is like print'
+            ..     'except that it supports logging and can be disabled.'
+            ..     sep=', ')
+            Display is like print, except that it supports logging and can be disabled.
         
             >> warn('warnings get a header that is printed in yellow.')
             warning: warnings get a header that is printed in yellow.
         
-            >> error('erros get a header that is printed in red.')
-            error: warnings get a header that is printed in red.
+            >> error('errors get a header that is printed in red.')
+            error: errors get a header that is printed in red.
         
-        Inform also supports normal best practices such as providing logging and output 
-        control and adding the program name to error messages.
+        Inform also provides logging and output control.
         
         Install with::
         
             pip install inform
         
         Supported in Python2.7, Python3.3, Python3.4, Python3.5, and Python3.6.
         
+        
+        Introduction
+        ------------
+        
         This package defines a collection of 'print' functions that have different 
         roles.  These functions are referred to as 'informants' and are described below 
-        in the the Informants section. They include include *log*, *comment*, *codicil*, 
+        in the Informants section. They include include *log*, *comment*, *codicil*, 
         *narrate*, *display*, *output*, *notify*, *debug*, *warn*, *error*, *fatal* and 
-        *panic*.  Each of these functions takes arguments like the standard print 
-        function: unnamed arguments are converted to strings and joined together to 
-        produce the output, the named arguments act to control the process.  The 
-        available controls (named arguments) are:
-        
-        sep = ' ':
-           Specifies the string used to join the unnamed arguments.
-        end = '\\n':
-           Specifies a string to append to the message.
-        file = stdout:
-           The destination stream (a file pointer).
-        flush = *False*:
-           Whether the message should flush the destination stream (not available in 
-           python2).
-        culprit = *None*:
-           A string that is added to the beginning of the message that identifies the 
-           culprit (the object for which the problem being reported was found). May also 
-           be a collection of strings, in which case they are joined with '.'.
-        hanging = *True*:
-           Indicates hanging indentation should be used when outputting multi-line 
-           message with headers or culprits.
+        *panic*.
         
         With the simplest use of the program, you simply import the informants you need 
-        and call them (they take the same arguments as does the *print* function built 
-        into Python:
+        and call them (they take the same arguments as Python's built-in *print* 
+        function):
         
         .. code-block:: python
         
             >>> from inform import display
             >>> display('ice', 9)
             ice 9
         
-        More typical is to import and instantiate the Inform class yourself along with 
-        the desired informants.  This gives you the ability to specify options:
+        For more control of the informants, you can import and instantiate the Inform 
+        class yourself along with the desired informants.  This gives you the ability to 
+        specify options:
         
         .. code-block:: python
         
             >>> from inform import Inform, display, error
             >>> Inform(logfile=False, prog_name=False)
             <...>
             >>> display('hello')
@@ -163,18 +151,18 @@
             >>> str(logfile_text[:10]), str(logfile_text[-13:])
             ('Invoked as', 'running test\n')
         
         You can create your own informants:
         
         .. code-block:: python
         
-            >>> from inform import Inform, InformantGenerator
+            >>> from inform import Inform, InformantFactory
         
-            >>> verbose1 = InformantGenerator(output=lambda m: m.verbosity >= 1)
-            >>> verbose2 = InformantGenerator(output=lambda m: m.verbosity >= 2)
+            >>> verbose1 = InformantFactory(output=lambda m: m.verbosity >= 1)
+            >>> verbose2 = InformantFactory(output=lambda m: m.verbosity >= 2)
             >>> with Inform(verbosity=0):
             ...     verbose1('First level of verbosity.')
             ...     verbose2('Second level of verbosity.')
         
             >>> with Inform(verbosity=1):
             ...     verbose1('First level of verbosity.')
             ...     verbose2('Second level of verbosity.')
@@ -185,15 +173,15 @@
             ...     verbose2('Second level of verbosity.')
             First level of verbosity.
             Second level of verbosity.
         
         The argument *verbosity* is not an explicitly supported argument to Inform.  In 
         this case Inform simply saves the value and makes it available as an attribute, 
         and it is this attribute that is queried by the lambda function passed to the 
-        InformantGenerator when creating the informants.
+        InformantFactory when creating the informants.
         
         
         Exception
         ---------
         An exception, *Error*, is provided that takes the same arguments as an 
         informant.  This allows you to catch the exception and handle it if you like.  
         The exception provides the *report* and *terminate* methods that processes the 
@@ -336,17 +324,17 @@
         functionality even if you do not have local access to the informer. They are:
         
         | done()
         | terminate()
         | terminate_if_errors()
         | errors_accrued()
         
-        InformantGenerator Class
-        ------------------------
-        The InformantGenerator class takes the following arguments:
+        InformantFactory Class
+        ----------------------
+        The InformantFactory class takes the following arguments:
         
         severity = *None*:
            Messages with severities get headers. The header consists of the severity, 
            the program name (if desired), and the culprit (if provided). If the message 
            text does not contain a newline it is appended to the header.  Otherwise the 
            message text is indented and placed on the next line.
         is_error = *False*:
@@ -372,23 +360,23 @@
            message is indented.
         message_color = *None*:
            Color used to display the message. Choose from *black*, *red*, *green*, 
            *yellow*, *blue*, *magenta*, *cyan*, *white*.
         header_color = *None*:
            Color used to display the header, if one is produced.
         
-        An object of InformantGenerator is referred to as an informant. It is generally 
+        An object of InformantFactory is referred to as an informant. It is generally 
         treated as a function that is called to produce the desired output.
         
         .. code-block:: python
         
-            >>> from inform import InformantGenerator
+            >>> from inform import InformantFactory
         
-            >>> succeed = InformantGenerator(message_color='green')
-            >>> fail = InformantGenerator(message_color='red')
+            >>> succeed = InformantFactory(message_color='green')
+            >>> fail = InformantFactory(message_color='red')
         
             >>> succeed('This message would be green.')
             This message would be green.
         
             >>> fail('This message would be red.')
             This message would be red.
         
@@ -400,28 +388,28 @@
         debug do not produce any output if *mute* is set.
         
         log
         """
         
         .. code-block:: python
         
-           log = InformantGenerator(
+           log = InformantFactory(
                output=False,
                log=True,
            )
         
         Saves a message to the log file without displaying it.
         
         
         comment
         """""""
         
         .. code-block:: python
         
-           comment = InformantGenerator(
+           comment = InformantFactory(
                output=lambda informer: informer.verbose and not informer.mute,
                log=True,
                message_color='cyan',
            )
         
         Displays a message only if *verbose* is set. Logs the message. The message is 
         displayed in cyan.
@@ -430,15 +418,15 @@
         the user's attention.
         
         codicil
         """""""
         
         .. code-block:: python
         
-           codicil = InformantGenerator(is_continuation=True)
+           codicil = InformantFactory(is_continuation=True)
         
         Continues a previous message. Continued messages inherit the properties (output, 
         log, message color, etc) of the previous message.  If the previous message had 
         a header, that header is not output and instead the message is indented.
         
         .. code-block:: python
         
@@ -452,15 +440,15 @@
         
         
         narrate
         """""""
         
         .. code-block:: python
         
-           narrate = InformantGenerator(
+           narrate = InformantFactory(
                output=lambda informer: informer.narrate and not informer.mute,
                log=True,
                message_color='blue',
            )
         
         Displays a message only if *narrate* is set. Logs the message. The message is 
         displayed in blue.
@@ -472,15 +460,15 @@
         
         
         display
         """""""
         
         .. code-block:: python
         
-           display = InformantGenerator(
+           display = InformantFactory(
                output=lambda informer: not informer.quiet and not informer.mute,
                log=True,
            )
         
         Displays a message if *quiet* is not set. Logs the message.
         
         .. code-block:: python
@@ -491,15 +479,15 @@
         
         
         output
         """"""
         
         .. code-block:: python
         
-           output = InformantGenerator(
+           output = InformantFactory(
                output=lambda informer: not informer.mute,
                log=True,
            )
         
         Displays and logs a message. This is used for messages that are not errors that 
         are noteworthy enough that they need to get through even though the user has 
         asked for quiet.
@@ -512,15 +500,15 @@
         
         
         notify
         """"""
         
         .. code-block:: python
         
-           notify = InformantGenerator(
+           notify = InformantFactory(
                notify=True,
                log=True,
            )
         
         Temporarily display the message in a bubble at the top of the screen.  Also 
         prints the message on the standard output and sends it to the log file.  This is 
         used for messages that the user is otherwise unlikely to see because they have 
@@ -534,15 +522,15 @@
         
         
         debug
         """""
         
         .. code-block:: python
         
-           debug = InformantGenerator(
+           debug = InformantFactory(
                severity='DEBUG',
                output=True,
                log=True,
                header_color='magenta',
            )
         
         Displays and logs a debugging message. A header with the label *DEBUG* is added 
@@ -560,15 +548,15 @@
         
         
         warn
         """"
         
         .. code-block:: python
         
-           warn = InformantGenerator(
+           warn = InformantFactory(
                severity='warning',
                header_color='yellow',
                output=lambda informer: not informer.quiet and not informer.mute,
                log=True,
            )
         
         Displays and logs a warning message. A header with the label *warning* is added 
@@ -583,15 +571,15 @@
         
         
         error
         """""
         
         .. code-block:: python
         
-           error = InformantGenerator(
+           error = InformantFactory(
                severity='error',
                is_error=True,
                header_color='red',
                output=lambda informer: not informer.mute,
                log=True,
            )
         
@@ -606,15 +594,15 @@
             myprog error: count: invalid value specified, expected number.
         
         fatal
         """""
         
         .. code-block:: python
         
-           fatal = InformantGenerator(
+           fatal = InformantFactory(
                severity='error',
                is_error=True,
                terminate=1,
                header_color='red',
                output=lambda informer: not informer.mute,
                log=True,
            )
@@ -625,28 +613,54 @@
         
         
         panic
         """""
         
         .. code-block:: python
         
-           panic = InformantGenerator(
+           panic = InformantFactory(
                severity='internal error (please report)',
                is_error=True,
                terminate=3,
                header_color='red',
                output=True,
                log=True,
            )
         
         Displays and logs a panic message. A header with the label *internal error* is 
         added to the message and the header is colored red. The program is terminated 
         with an exit status of 3.
         
         
+        Informant Control
+        -----------------
+        
+        The exeception (Error) and all informants take arguments very much like the 
+        standard print function: unnamed arguments are converted to strings and joined 
+        together to produce the output, the named arguments act to control the process.  
+        The available controls (named arguments) are:
+        
+        sep = ' ':
+           Specifies the string used to join the unnamed arguments.
+        end = '\\n':
+           Specifies a string to append to the message.
+        file = stdout:
+           The destination stream (a file pointer).
+        flush = *False*:
+           Whether the message should flush the destination stream (not available in 
+           python2).
+        culprit = *None*:
+           A string that is added to the beginning of the message that identifies the 
+           culprit (the object for which the problem being reported was found). May also 
+           be a collection of strings, in which case they are joined with '.'.
+        hanging = *True*:
+           Indicates hanging indentation should be used when outputting multi-line 
+           message with headers or culprits.
+        
+        
         Utilities
         ---------
         
         Several utility functions are provided for your convenience. They are often 
         helpful when creating messages.
         
         indent(text, leader='    ',  first=0, stops=1, sep='\\n'):
@@ -654,16 +668,24 @@
             lines to indent.  *first* is the number of indentations used for the first 
             line relative to the others (may be negative but (first + stops) should not 
             be. *stops* is the default number of indentations to use. *sep* is the 
             string used to separate the lines.
         
         conjoin(iterable, conj=' and ', sep=', '):
             Like ''.join(), but allows you to specify a conjunction that is placed 
-            between the last two elements, ex: conjoin(['a', 'b', 'c'], conj=' or ') 
-            generates 'a, b or c'.
+            between the last two elements, ex:
+        
+            .. code-block:: python
+        
+                >>> from inform import conjoin
+                >>> conjoin(['a', 'b', 'c'])
+                'a, b and c'
+        
+                >>> conjoin(['a', 'b', 'c'], conj=' or ')
+                'a, b or c'
         
         cull(collection, [remove]):
             Strips items from a list that have a particular value. By default, it strips 
             a list of values that if casted to a boolean would have a value of False (0, 
             False, None, '', (), [], etc.).  A particular value may be specified using 
             the 'remove' as a keyword argument.  The value of remove may be a function, 
             in which case it takes a single item as an argument and returns *True* if 
@@ -813,39 +835,39 @@
         
                 >>> from inform import ppp, ddd, vvv
                 >>> a = 1
                 >>> b = 'this is a test'
                 >>> c = (2, 3)
                 >>> d = {'a': a, 'b': b, 'c': c}
                 >>> ppp(a, b, c)
-                DEBUG: <doctest README.rst[75]>:1, __main__:
+                DEBUG: <doctest README.rst[78]>:1, __main__:
                     1 this is a test (2, 3)
         
         ddd(\*args, \*\*kwyargs):
             This function is pretty prints all of both the unnamed and named arguments.
         
             .. code:: python
         
                 >>> ddd(a, b, c, d)
-                DEBUG: <doctest README.rst[76]>:1, __main__:
+                DEBUG: <doctest README.rst[79]>:1, __main__:
                     1
                     'this is a test'
                     (2, 3)
                     {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
                     }
         
             If you give named arguments, the name is prepended to its value:
         
             .. code:: python
         
                 >>> ddd(a=a, b=b, c=c, d=d, s='hey now!')
-                DEBUG: <doctest README.rst[77]>:1, __main__:
+                DEBUG: <doctest README.rst[80]>:1, __main__:
                     a = 1
                     b = 'this is a test'
                     c = (2, 3)
                     d = {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
@@ -859,29 +881,29 @@
         
                 >>> class Info:
                 ...     def __init__(self, **kwargs):
                 ...         self.__dict__.update(kwargs)
                 ...         ddd(self=self)
         
                 >>> contact = Info(email='ted@ledbelly.com', name='Ted Ledbelly')
-                DEBUG: <doctest README.rst[78]>:4, __main__.Info.__init__():
+                DEBUG: <doctest README.rst[81]>:4, __main__.Info.__init__():
                     self = {
                         'email': 'ted@ledbelly.com',
                         'name': 'Ted Ledbelly',
                     }
         
         vvv(\*args):
             This function prints variables from the calling scope. If no arguments are 
             given, then all the variables are printed. You can optionally give specific 
             variables on the argument list and only those variables are printed.
         
             .. code:: python
         
                 >>> vvv(b, d)
-                DEBUG: <doctest README.rst[80]>:1, __main__:
+                DEBUG: <doctest README.rst[83]>:1, __main__:
                     b = 'this is a test'
                     d = {
                         'a': 1,
                         'b': 'this is a test',
                         'c': (2, 3),
                     }
         
@@ -889,15 +911,15 @@
             so if several variables share the value of one requested, they are all 
             shown.
         
             .. code:: python
         
                 >>> aa = 1
                 >>> vvv(a)
-                DEBUG: <doctest README.rst[82]>:1, __main__:
+                DEBUG: <doctest README.rst[85]>:1, __main__:
                     a = 1
                     aa = 1
         
         
         Color Class
         """""""""""
```

