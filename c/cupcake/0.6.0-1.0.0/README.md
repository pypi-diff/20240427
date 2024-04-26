# Comparing `tmp/cupcake-0.6.0.tar.gz` & `tmp/cupcake-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-0.6.0.tar", max compression
+gzip compressed data, was "cupcake-1.0.0.tar", max compression
```

## Comparing `cupcake-0.6.0.tar` & `cupcake-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.6.0/LICENSE
--rw-r--r--   0        0        0      594 2024-02-28 19:10:25.539369 cupcake-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.6.0/src/cupcake/__init__.py
--rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-0.6.0/src/cupcake/cascade.py
--rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-0.6.0/src/cupcake/confee.py
--rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-0.6.0/src/cupcake/data/cmake_names.py
--rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.6.0/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0      989 2024-02-01 04:09:54.265674 cupcake-0.6.0/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     2083 2024-02-28 00:21:08.869413 cupcake-0.6.0/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      259 2023-09-22 12:15:54.010771 cupcake-0.6.0/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0      111 2023-09-22 12:16:43.153172 cupcake-0.6.0/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      235 2024-02-01 17:15:10.547104 cupcake-0.6.0/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-0.6.0/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      203 2024-02-01 17:12:54.853037 cupcake-0.6.0/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.6.0/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-0.6.0/src/cupcake/expression.py
--rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-0.6.0/src/cupcake/functional.py
--rw-r--r--   0        0        0    47316 2024-02-28 16:34:37.901335 cupcake-0.6.0/src/cupcake/main.py
--rw-r--r--   0        0        0     3493 2024-02-28 04:15:50.749636 cupcake-0.6.0/src/cupcake/transformations.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 cupcake-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-1.0.0/LICENSE
+-rw-r--r--   0        0        0      576 2024-04-26 23:12:40.394996 cupcake-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-1.0.0/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     3965 2024-02-28 04:41:46.514999 cupcake-1.0.0/src/cupcake/cascade.py
+-rw-r--r--   0        0        0    10078 2024-02-22 06:16:05.800878 cupcake-1.0.0/src/cupcake/confee.py
+-rw-r--r--   0        0        0     1027 2024-01-11 04:42:54.793235 cupcake-1.0.0/src/cupcake/data/cmake_names.py
+-rw-r--r--   0        0        0       58 2024-03-30 22:14:37.710534 cupcake-1.0.0/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0     1031 2024-04-26 22:06:39.942764 cupcake-1.0.0/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     2409 2024-04-26 22:06:34.282479 cupcake-1.0.0/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      438 2024-03-19 14:45:33.698677 cupcake-1.0.0/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0      103 2024-03-19 14:16:34.798335 cupcake-1.0.0/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      227 2024-03-19 14:16:51.427197 cupcake-1.0.0/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      470 2024-02-01 17:18:45.120789 cupcake-1.0.0/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      203 2024-03-19 13:09:50.402090 cupcake-1.0.0/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-1.0.0/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0     1758 2024-02-06 16:16:50.206575 cupcake-1.0.0/src/cupcake/expression.py
+-rw-r--r--   0        0        0      227 2024-02-04 01:50:29.311228 cupcake-1.0.0/src/cupcake/functional.py
+-rw-r--r--   0        0        0    52971 2024-04-26 22:32:20.677109 cupcake-1.0.0/src/cupcake/main.py
+-rw-r--r--   0        0        0     1053 2024-04-26 23:12:40.126982 cupcake-1.0.0/src/cupcake/transformations.py
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 cupcake-1.0.0/PKG-INFO
```

### Comparing `cupcake-0.6.0/LICENSE` & `cupcake-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-0.6.0/pyproject.toml` & `cupcake-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "cupcake"
-version = "0.6.0"
+version = "1.0.0"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.0.4"
 click-option-group = "^0.5.3"
 tomlkit = "^0.10.1"
 jinja2 = "^3.1.1"
-libcst = "^0.4.9"
 
 [tool.poetry.group.dev.dependencies]
 shush = "^0.3.2"
 pytest = "^7.0.1"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.2.1"
```

### Comparing `cupcake-0.6.0/src/cupcake/cascade.py` & `cupcake-1.0.0/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.6.0/src/cupcake/confee.py` & `cupcake-1.0.0/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.6.0/src/cupcake/data/cmake_names.py` & `cupcake-1.0.0/src/cupcake/data/cmake_names.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.6.0/src/cupcake/data/new/CMakeLists.txt` & `cupcake-1.0.0/src/cupcake/data/new/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,22 @@
   VERSION 0.1.0
   {% if github %}
   HOMEPAGE_URL https://github.com/{{ github }}/{{ name }}
   {% endif %}
   LANGUAGES CXX
 )
 
-find_package(cupcake REQUIRED)
+find_package(cupcake.cmake REQUIRED)
 
 cupcake_project()
 
 {% if special %}
 cupcake_find_packages(main)
 cupcake_link_libraries(${PROJECT_NAME}.imports.main INTERFACE main)
+cupcake_find_packages(tool PRIVATE)
 {% endif %}
 
 {% if with_library %}
 {% if special %}
 cupcake_add_libraries()
 {% else %}
 cupcake_add_library({{ name }})
```

### Comparing `cupcake-0.6.0/src/cupcake/data/new/conanfile.py` & `cupcake-1.0.0/src/cupcake/data/new/conanfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from conan import ConanFile
+import conan
 from conan.tools.cmake import CMake, cmake_layout
 
-class {{ NameTitle }}(ConanFile):
+class {{ name | pascal }}(conan.ConanFile):
     name = '{{ name }}'
     version = '0.1.0'
     {% if github %}
     user = 'github'
     channel = '{{ github }}'
     {% endif %}
 
@@ -18,15 +18,15 @@
     {% endif %}
 
     settings = 'os', 'compiler', 'build_type', 'arch'
     options = {'shared': [True, False], 'fPIC': [True, False]}
     default_options = {'shared': False, 'fPIC': True}
 
     requires = [
-        'cupcake/{{ version }}@github/thejohnfreeman',
+        'cupcake.cmake/{{ version }}@github/thejohnfreeman',
         {% if with_tests and not special %}
         'doctest/2.4.8',
         {% endif %}
     ]
     generators = ['CMakeDeps', 'CMakeToolchain']
 
     exports_sources = [
@@ -50,16 +50,23 @@
     {% if special %}
     def requirements(self):
         import json
         import pathlib
         path = pathlib.Path(self.recipe_folder) / 'cupcake.json'
         with path.open('r') as file:
             metadata = json.load(file)
+        methods = {
+            'tool': 'tool_requires',
+            'test': 'test_requires',
+        } if conan.conan_version.major.value == 2 else {}
         for requirement in metadata.get('imports', []):
-            self.requires(requirement['reference'])
+            groups = requirement.get('groups', [])
+            group = groups[0] if len(groups) == 1 else 'main'
+            method = methods.get(group, 'requires')
+            getattr(self, method)(requirement['reference'])
 
     {% endif %}
     def config_options(self):
         if self.settings.os == 'Windows':
             del self.options.fPIC
 
     def build(self):
```

### Comparing `cupcake-0.6.0/src/cupcake/expression.py` & `cupcake-1.0.0/src/cupcake/expression.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.6.0/src/cupcake/main.py` & `cupcake-1.0.0/src/cupcake/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,16 +57,24 @@
     return function
 
 # Build flavor is selected at build time.
 # Configuration commands take a set of possible flavors.
 
 # Map from friendly Cupcake name to Conan/CMake name.
 FLAVORS = {
-    'release': 'Release',
+    'd': 'Debug',
     'debug': 'Debug',
+    'minsizerel': 'MinSizeRel',
+    'msr': 'MinSizeRel',
+    'r': 'Release',
+    'rd': 'RelWithDebInfo',
+    'release': 'Release',
+    'relwithdebinfo': 'RelWithDebInfo',
+    'rwdi': 'RelWithDebInfo',
+    'size': 'MinSizeRel',
 }
 
 PATTERN_INDEX_FILENAME = re.compile(r'^index-.*\.json$')
 
 def const(value):
     def f(*args, **kwargs):
         return value
@@ -133,28 +141,38 @@
             return diff
     return 0
 
 key = functools.cmp_to_key(
     lambda a, b: compare_version(a, b)
 )
 
+def assert_legal_name(name):
+    if not re.match(r'^[a-z][a-z0-9-]*$', name):
+        raise SystemExit(f'name must contain only lowercase letters, numbers, and dashes: {name}')
+
 def parse_options(options: t.Iterable[str], default):
     """Parse "name[=value]" strings into a {name: value, ...} dictionary."""
     adds = {}
     for option in options:
         match = re.match(r'^([^=]+)(?:=(.+))?$', option)
         if not match:
             raise SystemExit(f'bad option: `{option}`')
         name = match.group(1)
         value = match.group(2)
         if value is None:
             value = default
         adds[name] = value
     return adds
 
+def snake(string):
+    return string.replace('-', '_')
+
+def pascal(string):
+    return string.title().replace('-', '')
+
 PATTERN_GITHUB_PATH = r'/([^/]+)/([^/]+)(?:/tree/[^/]+(.+))?'
 
 @contextmanager
 def pack_directory(path):
     yield path
 
 @contextmanager
@@ -178,14 +196,21 @@
         del requirements[i:i+1]
     after = f(before)
     if after is not None:
         requirements.append(after)
     requirements.sort(key=lambda item: item['name'])
     metadata.imports = requirements
 
+def expand(reference):
+    if reference.startswith('lib'):
+        return ('libraries', reference[len('lib'):])
+    if reference.startswith('test.'):
+        return ('tests', reference[len('test.'):])
+    return ('executables', reference)
+
 class SearchResult:
     """Representation for a Conan package search result."""
 
     key = functools.cmp_to_key(
         lambda a, b: compare_version(a.version, b.version)
     )
 
@@ -338,25 +363,35 @@
         SearchResult(remote, reference)
         for remote in results
         for reference in results[remote]
         if reference != 'error'
     ]
 
 
+_SINGLES = ('Unix Makefiles', 'Ninja')
+_MULTIS = ('Ninja Multi-Config', 'Xcode')
+
 class CMake:
     def __init__(self, CMAKE):
         self.CMAKE = CMAKE
 
     def is_multi_config(self, generator):
         """
         Configure a tiny project
         using the CMake file API
         in a temporary directory
         to find out whether the generator is multi-config.
         """
+        if type(generator) == str:
+            if generator in _SINGLES:
+                return False
+            if generator in _MULTIS:
+                return True
+            if generator.startswith('Visual Studio '):
+                return True
         with tempfile.TemporaryDirectory() as cmake_dir:
             cmake_dir = pathlib.Path(cmake_dir)
             api_dir = cmake_dir / '.cmake/api/v1'
             query_dir = api_dir / 'query'
             query_dir.mkdir(parents=True)
             (query_dir / 'cmakeFiles-v1').touch()
             source_dir = resources.as_file(
@@ -372,37 +407,31 @@
                 f for f in reply_dir.iterdir()
                 if PATTERN_INDEX_FILENAME.match(f.name)
             )
             index = json.loads(index_file.read_text())
             multiConfig = index['cmake']['generator']['multiConfig']
             return multiConfig
 
-    def configure(self, build_dir, source_dir, generator, variables={}):
+    def configure(self, build_dir, source_dir, generator, variables={}, env={}):
         """
         source_dir : path-like
             If relative, must be relative to build_dir.
         """
         variables = dict(variables)
         args = [f'-D{name}={value}' for name, value in variables.items()]
-        args = [*args, source_dir]
         if generator is not None:
             args = ['-G', generator, *args]
-            # CMake will warn when this variable is unused by the generator.
-            # https://cmake.org/cmake/help/latest/variable/CMAKE_EXPORT_COMPILE_COMMANDS.html
-            # TODO: Let `cupcake_project()` set a different default for this
-            # variable, and Cupcake can just link it in the build directory if
-            # it is found after the `cmake` step.
-            if re.search('Makefiles|Ninja', generator):
-                variables['CMAKE_EXPORT_COMPILE_COMMANDS'] = 'ON'
-        run([self.CMAKE, *args], cwd=build_dir)
+        args = [*args, source_dir]
+        env = { **os.environ, **env }
+        run([self.CMAKE, *args], cwd=build_dir, env=env)
 
 TEST_TEMPLATE_ = """
-'{{ cmake }}' --build '{{ cmakeDir }}'
-{% if multiConfig %} --config {{ flavor }} {% endif %}
---target {% if multiConfig %} RUN_TESTS {% else %} test {% endif %}
+'{{ ctest }}' --test-dir '{{ cmakeDir }}'
+{% if multiConfig %} --build-config {{ flavor }} {% endif %}
+{% if regex %} --tests-regex {{ regex }} {% endif %}
 """
 
 # We want commands to call dependencies,
 # and want them to be able to pass options.
 # That means dependent command must accept all the options of all its
 # dependencies.
 
@@ -440,14 +469,18 @@
         return Conan.construct(command)
 
     @cascade.value()
     def CMAKE(self, config_):
         return confee.resolve(None, config_.CMAKE, 'cmake')
 
     @cascade.value()
+    def CTEST(self, config_):
+        return confee.resolve(None, config_.CTEST, 'ctest')
+
+    @cascade.value()
     @cascade.option(
         '--build-dir', '-B',
         help='Path to build directory. Absolute, or relative to source directory.',
         metavar='PATH',
     )
     def build_dir_path_(self, source_dir_, config_, build_dir) -> pathlib.Path:
         """
@@ -638,14 +671,19 @@
     )
     @cascade.option(
         '-U', 'unvariables',
         help='Unset a CMake variable. Repeatable.',
         metavar='NAME',
         multiple=True,
     )
+    @cascade.option(
+        '--keep',
+        help='Do not delete the CMake directory.',
+        is_flag=True,
+    )
     def cmake(
         self,
         source_dir_,
         config_,
         CMAKE,
         build_dir_,
         state_,
@@ -654,14 +692,15 @@
         conan,
         generator,
         shared,
         tests,
         prefixes,
         variables,
         unvariables,
+        keep,
     ):
         """Configure CMake for at least the selected flavor."""
         # Variables are a little unique.
         # We must start with `config.cmake.variables` (default `{}`),
         # override with `variables`,
         # remove `unvariables`,
         # and then write the result to `config.cmake.variables`.
@@ -724,18 +763,23 @@
         else:
             sflavors = [flavor_]
 
         cmake_dir = build_dir_ / 'cmake'
         if not multiConfig:
             cmake_dir /= flavor_
 
-        shutil.rmtree(cmake_dir, ignore_errors=True)
-        # This directory should not yet exist, but its parent might.
-        cmake_dir.mkdir(parents=True)
+        if not keep:
+            shutil.rmtree(cmake_dir, ignore_errors=True)
+        cmake_dir.mkdir(parents=True, exist_ok=True)
+        # CMake complains if any of these variables are unused,
+        # but it is impossible to predict which will be unused.
+        # Don't sweat it.
         cmake_args = {}
+        cmake_args['CMAKE_EXPORT_COMPILE_COMMANDS'] = 'ON'
+        cmake_args['CMAKE_POLICY_DEFAULT_CMP0091'] = 'NEW'
         cmake_args['BUILD_SHARED_LIBS'] = 'ON' if shared else 'OFF'
         cmake_args['CMAKE_INSTALL_PREFIX'] = prefix_
         if conan is not None:
             cmake_args['CMAKE_TOOLCHAIN_FILE:FILEPATH'] = conan.toolchain()
         if tests is not None:
             cmake_args['BUILD_TESTING'] = 'ON' if tests else 'OFF'
         if prefixes:
@@ -745,15 +789,16 @@
             cmake_args['CMAKE_CONFIGURATION_TYPES'] = ';'.join(flavors)
         else:
             cmake_args['CMAKE_BUILD_TYPE'] = FLAVORS[flavor_]
         # Add these last to let callers override anything.
         for name, value in cvars.items():
             cmake_args[name] = value
         CMake(CMAKE).configure(
-            cmake_dir, source_dir_, generator, cmake_args
+            cmake_dir, source_dir_, generator, cmake_args,
+            env={'CMAKE_OUTPUT_DIR': build_dir_ / 'output'},
         )
 
         state_.cmake.id = id
         state_.cmake.generator = generator
         state_.cmake.multiConfig = multiConfig
         state_.cmake.flavors = sflavors
         confee.write(config_)
@@ -765,25 +810,27 @@
         build_dir_ /= 'cmake'
         if not cmake.multiConfig():
             build_dir_ /= flavor_
         return build_dir_
 
     @cascade.command()
     @cascade.option(
-        '--jobs', '-j', help='Maximum number of simultaneous jobs.'
+        '--jobs', '-j', type=int, help='Maximum number of simultaneous jobs.',
     )
     @cascade.argument('target', required=False)
-    def build(self, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs, target):
+    def build(self, config_, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs, target):
         """Build the selected flavor."""
+        jobs = confee.resolve(jobs, config_.jobs, None)
+        confee.write(config_)
         command = [CMAKE, '--build', cmake_dir_, '--verbose']
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
         command.append('--parallel')
         if jobs is not None:
-            command.append(jobs)
+            command.append(str(jobs))
         if target is not None:
             command.extend(['--target', target])
         with (log_dir_ / 'build').open('wb') as stream:
             tee(command, stream=stream)
         return cmake
 
     @cascade.command()
@@ -812,34 +859,48 @@
             '--config',
             FLAVORS[flavor_],
             '--prefix',
             prefix_,
         ])
 
     @cascade.command()
-    def test(self, config_, CMAKE, log_dir_, cmake_dir_, flavor_, cmake):
+    @cascade.argument('regex', required=False)
+    def test(self, config_, CTEST, log_dir_, cmake_dir_, flavor_, cmake, regex):
         """Test the selected flavor."""
         template = confee.resolve(None, config_.scripts.test, TEST_TEMPLATE_)
         template = jinja2.Template(template)
         context = {
-            'cmake': CMAKE,
+            'ctest': CTEST,
             'cmakeDir': cmake_dir_,
             'multiConfig': cmake.multiConfig(),
             'flavor': FLAVORS[flavor_],
+            'regex': regex,
         }
         command = shlex.split(template.render(**context))
         env = os.environ.copy()
         env['CTEST_OUTPUT_ON_FAILURE'] = 'ON'
         with (log_dir_ / 'test').open('wb') as stream:
             tee(command, stream=stream, env=env)
 
+    def jenv_(self, directory):
+        loader = jinja2.PackageLoader('cupcake', directory)
+        jenv = jinja2.Environment(
+            loader=loader,
+            keep_trailing_newline=True,
+            trim_blocks=True,
+            lstrip_blocks=True,
+        )
+        jenv.filters['pascal'] = pascal
+        jenv.filters['snake'] = snake
+        return jenv
+
     @cascade.command()
     @cascade.argument('path', required=False, default='.')
     @cascade.option(
-        '--version', help='Version of requirement cupcake@github/thejohnfreeman.', default='0.7.0',
+        '--version', help='Version of requirement cupcake.cmake@github/thejohnfreeman.', default='1.0.0',
     )
     @cascade.option(
         '--special/--general', help='Whether to enable special commands.', default=True,
     )
     @cascade.option(
         '--library/--no-library', help='Whether to export a library.', default=True,
     )
@@ -884,21 +945,15 @@
         name,
         license,
         author,
         github,
         force,
     ):
         """Create a new project."""
-        loader = jinja2.PackageLoader('cupcake', 'data/new')
-        jenv = jinja2.Environment(
-            loader=loader,
-            keep_trailing_newline=True,
-            trim_blocks=True,
-            lstrip_blocks=True,
-        )
+        jenv = self.jenv_('data/new')
 
         if author is None:
             username = subprocess.run(
                 ['git', 'config', 'user.name'], capture_output=True
             ).stdout.decode().strip()
             email = subprocess.run(
                 ['git', 'config', 'user.email'], capture_output=True
@@ -962,27 +1017,20 @@
                     links.append(f'{name}.lib{name}')
                 test = {'name': name, 'links': links }
                 metadata.tests = [test]
             confee.write(metadata)
 
 
     def generate_(self, jenv, prefix, tnames, name, context):
-        if not re.match(r'[a-z][a-z0-9-]*', name):
-            raise SystemExit(f'name must contain only lowercase letters, numbers, and dashes: {name}')
-
-        NameTitle = name.title().replace('-', '')
-        name_snake_lower = name.replace('-', '_')
-        NAME_SNAKE_UPPER = name_snake_lower.upper()
+        assert_legal_name(name)
 
         context = {
             **context,
             'name': name,
-            'NameTitle': NameTitle,
-            'name_snake_lower': name_snake_lower,
-            'NAME_SNAKE_UPPER': NAME_SNAKE_UPPER,
+            'namespaces': [name],
         }
 
         for tname in tnames:
             suffix = jenv.from_string(tname).render(**context)
             path = pathlib.Path(prefix, suffix)
             path.parent.mkdir(parents=True, exist_ok=True)
             template = jenv.get_template(tname)
@@ -1076,52 +1124,139 @@
             raise SystemExit(f'requirement not found: {name}')
         assert(len(imports) == 1)
         update_requirement(metadata, name, const(None))
         confee.write(metadata)
 
     @cascade.command()
     def list(self, source_dir_):
-        """List targets."""
+        """List targets and their links."""
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        prefixes = {
-            'libraries': 'lib',
-            'executables': '',
-            'tests': 'test.'
-        }
-        targets = [
-            f'{prefixes[kind]}{name()}'
-            for kind in ['libraries', 'executables', 'tests']
-            for name in metadata[kind][:].name
+        kinds = [
+            ('libraries', 'lib'),
+            ('executables', ''),
+            ('tests', 'test.'),
         ]
-        for target in targets:
-            print(target)
+        for kind, prefix in kinds:
+            for item in metadata[kind][:]:
+                line = f'{prefix}{item.name()}'
+                links = item.links([])
+                if links:
+                    line += ' -> ' + ', '.join(links)
+                print(line)
+
+    @cascade.command()
+    @cascade.argument('downstream', required=True)
+    @cascade.argument('upstreams', required=True, nargs=-1)
+    def link(self, source_dir_, downstream, upstreams):
+        """Link downstream artifact to upstream libraries."""
+        metadata = confee.read(source_dir_ / 'cupcake.json')
+        pname = metadata.project.name()
+
+        def unprefix(reference):
+            for prefix in (pname + '.', '${PROJECT_NAME}.'):
+                if reference.startswith(prefix):
+                    return reference[len(prefix):]
+            return reference
+
+        def find(reference):
+            kind, name = expand(reference)
+            items = confee.filter(metadata[kind][:], subject['name'] == name)
+            items = list(items)
+            if len(items) > 1:
+                raise SystemExit(f'ambiguous reference: {reference}')
+            if len(items) < 1:
+                raise SystemExit(f'unknown reference: {reference}')
+            return items[0]
+
+        downstream = unprefix(downstream)
+        dproxy = find(downstream)
+
+        for upstream in upstreams:
+            upstream = unprefix(upstream)
+            if upstream.startswith('lib'):
+                uproxy = find(upstream)
+                if uproxy == dproxy:
+                    raise SystemExit(f'cannot link to self')
+            elif not re.match(f'^imports.\\w+$', upstream):
+                raise SystemExit(f'upstream is not a library: {upstream}')
+
+            link1 = '${PROJECT_NAME}.' + upstream
+            link2 = pname + '.' + upstream
+
+            existing = confee.filter(dproxy.links[:], (
+                (subject == link1) | (subject == link2) |
+                (subject['target'] == link1) | (subject['target'] == link2)
+            ))
+            existing = list(existing)
+            if len(existing) > 0:
+                raise SystemExit('already linked')
+            confee.add(dproxy.links, link1)
+
+        confee.write(metadata)
+
+    @cascade.command()
+    @cascade.argument('downstream', required=True)
+    @cascade.argument('upstreams', required=True, nargs=-1)
+    def unlink(self, source_dir_, downstream, upstreams):
+        """Unlink downstream artifact from upstream libraries."""
+        metadata = confee.read(source_dir_ / 'cupcake.json')
+        pname = metadata.project.name()
+
+        def unprefix(reference):
+            for prefix in (pname + '.', '${PROJECT_NAME}.'):
+                if reference.startswith(prefix):
+                    return reference[len(prefix):]
+            return reference
+
+        def find(reference):
+            kind, name = expand(reference)
+            items = confee.filter(metadata[kind][:], subject['name'] == name)
+            items = list(items)
+            if len(items) > 1:
+                raise SystemExit(f'ambiguous reference: {reference}')
+            if len(items) < 1:
+                raise SystemExit(f'unknown reference: {reference}')
+            return items[0]
+
+        downstream = unprefix(downstream)
+        dproxy = find(downstream)
+
+        for upstream in upstreams:
+            upstream = unprefix(upstream)
+            # We don't need to check that upstream is a library.
+            # All we care is whether it appears in the links.
+
+            link1 = '${PROJECT_NAME}.' + upstream
+            link2 = pname + '.' + upstream
+
+            confee.remove_if(dproxy.links[:], (
+                (subject == link1) | (subject == link2) |
+                (subject['target'] == link1) | (subject['target'] == link2)
+            ))
+
+        confee.write(metadata)
 
     @cascade.command('add:lib')
+    @cascade.option('--public/--private', is_flag=True, default=True, help='Whether to export the library.')
     @cascade.option('--header-only', is_flag=True, help='Whether to create a source file.')
     @cascade.argument('name', required=True)
-    def add_lib(self, source_dir_, header_only, name):
+    def add_lib(self, source_dir_, public, header_only, name):
         """Add a library."""
-        loader = jinja2.PackageLoader('cupcake', 'data/new')
-        jenv = jinja2.Environment(
-            loader=loader,
-            keep_trailing_newline=True,
-            trim_blocks=True,
-            lstrip_blocks=True,
-        )
+        jenv = self.jenv_('data/new')
 
         tnames = ['include/{{name}}/{{name}}.hpp']
         if not header_only:
             tnames.append('src/lib{{name}}.cpp')
         self.generate_(jenv, source_dir_, tnames, name, context={})
 
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        confee.add(
-            metadata.libraries,
-            {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] },
-        )
+        library = {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
+        if not public:
+            library['private'] = True
+        confee.add(metadata.libraries, library)
         confee.write(metadata)
 
     @cascade.command('remove:lib')
     @cascade.argument('name', required=True)
     def remove_lib(self, source_dir_, name):
         """Remove a library."""
         # Find the library in the metadata.
@@ -1184,33 +1319,28 @@
                         for file in files:
                             print(parent / file)
                             transformations.remove_includes(parent / file, name)
 
         confee.write(metadata)
 
     @cascade.command('add:exe')
+    @cascade.option('--public/--private', is_flag=True, default=True, help='Whether to export the executable.')
     @cascade.argument('name', required=True)
-    def add_exe(self, source_dir_, name):
+    def add_exe(self, source_dir_, public, name):
         """Add an executable."""
-        loader = jinja2.PackageLoader('cupcake', 'data/new')
-        jenv = jinja2.Environment(
-            loader=loader,
-            keep_trailing_newline=True,
-            trim_blocks=True,
-            lstrip_blocks=True,
-        )
+        jenv = self.jenv_('data/new')
 
         tnames = ['src/{{name}}.cpp']
         self.generate_(jenv, source_dir_, tnames, name, context={})
 
         metadata = confee.read(source_dir_ / 'cupcake.json')
-        confee.add(
-            metadata.executables,
-            {'name': name, 'links': ['${PROJECT_NAME}.imports.main'] },
-        )
+        executable = { 'name': name, 'links': ['${PROJECT_NAME}.imports.main'] }
+        if not public:
+            executable['private'] = True
+        confee.add(metadata.executables, executable)
         confee.write(metadata)
 
     @cascade.command('remove:exe')
     @cascade.argument('name', required=True)
     def remove_exe(self, source_dir_, name):
         """Remove an executable."""
         # Find the executable in the metadata.
@@ -1234,21 +1364,15 @@
 
         confee.write(metadata)
 
     @cascade.command('add:test')
     @cascade.argument('name', required=True)
     def add_test(self, source_dir_, name):
         """Add a test."""
-        loader = jinja2.PackageLoader('cupcake', 'data/new')
-        jenv = jinja2.Environment(
-            loader=loader,
-            keep_trailing_newline=True,
-            trim_blocks=True,
-            lstrip_blocks=True,
-        )
+        jenv = self.jenv_('data/new')
 
         tnames = ['tests/{{name}}.cpp']
         self.generate_(jenv, source_dir_, tnames, name, context={})
 
         metadata = confee.read(source_dir_ / 'cupcake.json')
         confee.add(
             metadata.tests,
@@ -1277,14 +1401,43 @@
         try:
             shutil.rmtree(source_dir_ / 'tests' / f'{name}')
         except FileNotFoundError:
             pass
 
         confee.write(metadata)
 
+    @cascade.command('add:header')
+    @cascade.argument('qname', required=True)
+    def add_header(self, source_dir_, qname):
+        """
+        Add a new header to an existing library.
+
+        The argument should be a qualified name,
+        e.g. "foo.bar.baz" for include/foo/bar/baz.hpp.
+        """
+        namespaces = qname.split('.')
+        for name in namespaces:
+            assert_legal_name(name)
+        path = source_dir_.joinpath('include', *namespaces).with_suffix('.hpp')
+        if path.exists():
+            raise SystemExit(f'file already exists: {path}')
+        name = namespaces.pop()
+
+        metadata = confee.read(source_dir_ / 'cupcake.json')
+        if not any(l.name() == namespaces[0] for l in metadata.libraries[:]):
+            raise SystemExit(f'missing library: {namespaces[0]}')
+
+        path.parent.mkdir(parents=True, exist_ok=True)
+        jenv = self.jenv_('data/new')
+        template = jenv.get_template('include/{{name}}/{{name}}.hpp')
+        path.write_text(template.render({
+            'namespaces': namespaces,
+            'name': name,
+        }))
+
     @cascade.command()
     @cascade.argument('url', default='.')
     def export(self, CONAN, url):
         """
         Copy a Conan package to your local cache.
 
         For this command, it is important to understand the idea of a "Conan
```

### Comparing `cupcake-0.6.0/PKG-INFO` & `cupcake-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 0.6.0
+Version: 1.0.0
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.0.4,<9.0.0)
 Requires-Dist: click-option-group (>=0.5.3,<0.6.0)
 Requires-Dist: jinja2 (>=3.1.1,<4.0.0)
-Requires-Dist: libcst (>=0.4.9,<0.5.0)
 Requires-Dist: tomlkit (>=0.10.1,<0.11.0)
```

