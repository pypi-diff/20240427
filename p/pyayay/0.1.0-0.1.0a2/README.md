# Comparing `tmp/pyayay-0.1.0.tar.gz` & `tmp/pyayay-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyayay-0.1.0.tar", last modified: Fri Apr 26 16:13:57 2024, max compression
+gzip compressed data, was "pyayay-0.1.0a2.tar", last modified: Sat Apr 27 17:23:11 2024, max compression
```

## Comparing `pyayay-0.1.0.tar` & `pyayay-0.1.0a2.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxr-xr-x   0 ruguevara (871050518) 593637566        0 2024-04-26 16:13:57.731049 pyayay-0.1.0/
--rw-r--r--   0 ruguevara (871050518) 593637566     1091 2024-04-26 15:20:51.000000 pyayay-0.1.0/LICENSE
--rw-r--r--   0 ruguevara (871050518) 593637566     3502 2024-04-26 16:13:57.730713 pyayay-0.1.0/PKG-INFO
--rw-r--r--   0 ruguevara (871050518) 593637566     2900 2024-04-26 15:53:28.000000 pyayay-0.1.0/README.md
--rw-r--r--   0 ruguevara (871050518) 593637566      689 2024-04-26 15:20:51.000000 pyayay-0.1.0/pyproject.toml
--rw-r--r--   0 ruguevara (871050518) 593637566       38 2024-04-26 16:13:57.731104 pyayay-0.1.0/setup.cfg
--rw-r--r--   0 ruguevara (871050518) 593637566      649 2024-04-26 15:20:51.000000 pyayay-0.1.0/setup.py
-drwxr-xr-x   0 ruguevara (871050518) 593637566        0 2024-04-26 16:13:57.727675 pyayay-0.1.0/src/
--rw-r--r--   0 ruguevara (871050518) 593637566     4074 2024-04-26 15:20:51.000000 pyayay-0.1.0/src/aychip.cpp
-drwxr-xr-x   0 ruguevara (871050518) 593637566        0 2024-04-26 16:13:57.730358 pyayay-0.1.0/src/pyayay.egg-info/
--rw-r--r--   0 ruguevara (871050518) 593637566     3502 2024-04-26 16:13:57.000000 pyayay-0.1.0/src/pyayay.egg-info/PKG-INFO
--rw-r--r--   0 ruguevara (871050518) 593637566      274 2024-04-26 16:13:57.000000 pyayay-0.1.0/src/pyayay.egg-info/SOURCES.txt
--rw-r--r--   0 ruguevara (871050518) 593637566        1 2024-04-26 16:13:57.000000 pyayay-0.1.0/src/pyayay.egg-info/dependency_links.txt
--rw-r--r--   0 ruguevara (871050518) 593637566        1 2024-04-26 13:03:54.000000 pyayay-0.1.0/src/pyayay.egg-info/not-zip-safe
--rw-r--r--   0 ruguevara (871050518) 593637566       25 2024-04-26 16:13:57.000000 pyayay-0.1.0/src/pyayay.egg-info/top_level.txt
--rw-r--r--   0 ruguevara (871050518) 593637566        0 2024-04-26 15:20:51.000000 pyayay-0.1.0/src/setup.py
--rw-r--r--   0 ruguevara (871050518) 593637566    14129 2024-04-26 15:20:51.000000 pyayay-0.1.0/src/wrapper.cpp
-drwxr-xr-x   0 ruguevara (871050518) 593637566        0 2024-04-26 16:13:57.729817 pyayay-0.1.0/tests/
--rw-r--r--   0 ruguevara (871050518) 593637566    10912 2024-04-26 15:20:51.000000 pyayay-0.1.0/tests/test_ayumi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.207512 pyayay-0.1.0a2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.203512 pyayay-0.1.0a2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.203512 pyayay-0.1.0a2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/.github/workflows/cibuildwheel.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-27 17:23:11.207512 pyayay-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-27 17:23:11.207512 pyayay-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.203512 pyayay-0.1.0a2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/aychip.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11180 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/aychip.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.203512 pyayay-0.1.0a2/src/ayumi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/ayumi/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/ayumi/ayumi.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/ayumi/ayumi.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.207512 pyayay-0.1.0a2/src/pyayay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-27 17:23:11.000000 pyayay-0.1.0a2/src/pyayay.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.203512 pyayay-0.1.0a2/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/utils/tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14239 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/src/wrapper.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:11.207512 pyayay-0.1.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-27 17:23:06.000000 pyayay-0.1.0a2/tests/test_ayumi.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-27 17:23:10.000000 pyayay-0.1.0a2/version.txt
```

### Comparing `pyayay-0.1.0/LICENSE` & `pyayay-0.1.0a2/src/ayumi/LICENSE`

 * *Files identical despite different names*

### Comparing `pyayay-0.1.0/PKG-INFO` & `pyayay-0.1.0a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pyayay
-Version: 0.1.0
+Version: 0.1.0a2
 Summary: PyAYay is a Python extension wrapper for AY-3-8910 sound chip emulator
 Author: Ruslan Grohovecki
-Author-email: Ruslan Grohovecki <ruslan.gr@gmail.com>, Peter Sovietov <peter@sovietov.com>
+Author-email: Ruslan Grokhovetskiy <ruslan.gr@gmail.com>, Peter Sovietov <peter@sovietov.com>
 Project-URL: Homepage, https://github.com/ruguevara/pyayay
 Project-URL: Issues, https://github.com/ruguevara/pyayay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
-# PyAyAy
+# PyAYay
 
-PyAyAy is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
+PyAYay is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
 
 ## Installation
 
 The package is not yet available on PyPi, so you need to install it from the source.
 
 ```bash
 git clone https://github.com/ruguevara/pyayay.git
```

### Comparing `pyayay-0.1.0/README.md` & `pyayay-0.1.0a2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# PyAyAy
+# PyAYay
 
-PyAyAy is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
+PyAYay is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
 
 ## Installation
 
 The package is not yet available on PyPi, so you need to install it from the source.
 
 ```bash
 git clone https://github.com/ruguevara/pyayay.git
```

### Comparing `pyayay-0.1.0/setup.py` & `pyayay-0.1.0a2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
         ],
         include_dirs = ["src"],
     ),
 ]
 
 setup(
     name="pyayay",
-    version="0.1.0",
     author="Ruslan Grohovecki",
     author_email="ruslan.gr@gmail.com",
     description="PyAYay is a Python extension wrapper for AY-3-8910 sound chip emulator",
     long_description="",
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
     python_requires=">=3.8",
+    setup_requires=["setuptools_scm"],
 )
```

### Comparing `pyayay-0.1.0/src/aychip.cpp` & `pyayay-0.1.0a2/src/aychip.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -150,13 +150,13 @@
 
 auto AyumiEmulator::processBlock(float* outLeft, float* outRight, size_t numSamples, bool removeDC, size_t stride) -> void {
     for (size_t i = 0; i < numSamples; ++i, outLeft+=stride, outRight+=stride) {
         ayumi_process(&Ayumi_);
         if (removeDC) {
             ayumi_remove_dc(&Ayumi_);
         }
-        *outLeft = Ayumi_.left * MasterVolume_;
-        *outRight = Ayumi_.right * MasterVolume_;
+        *outLeft = static_cast<float>(Ayumi_.left) * MasterVolume_;
+        *outRight = static_cast<float>(Ayumi_.right) * MasterVolume_;
     }
 }
 
 }
```

### Comparing `pyayay-0.1.0/src/pyayay.egg-info/PKG-INFO` & `pyayay-0.1.0a2/src/pyayay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: pyayay
-Version: 0.1.0
+Version: 0.1.0a2
 Summary: PyAYay is a Python extension wrapper for AY-3-8910 sound chip emulator
 Author: Ruslan Grohovecki
-Author-email: Ruslan Grohovecki <ruslan.gr@gmail.com>, Peter Sovietov <peter@sovietov.com>
+Author-email: Ruslan Grokhovetskiy <ruslan.gr@gmail.com>, Peter Sovietov <peter@sovietov.com>
 Project-URL: Homepage, https://github.com/ruguevara/pyayay
 Project-URL: Issues, https://github.com/ruguevara/pyayay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
 
-# PyAyAy
+# PyAYay
 
-PyAyAy is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
+PyAYay is a Python wrapper for the AY/YM sound chip emulator. Currently it supports only the Ayumi emulator by Peter Sovietov.
 
 ## Installation
 
 The package is not yet available on PyPi, so you need to install it from the source.
 
 ```bash
 git clone https://github.com/ruguevara/pyayay.git
```

### Comparing `pyayay-0.1.0/src/wrapper.cpp` & `pyayay-0.1.0a2/src/wrapper.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     AyumiEmulator& AY_;
 };
 
 
 PYBIND11_MODULE(pyayay, m) {
     m.doc() = "Python bindings for Ayumi sound chip emulator";
 
-    py::enum_<AYInterface::Enum>(m, "ChipType")
-        .value("AY", AYInterface::AY, "AY-3-8910")
-        .value("YM", AYInterface::YM, "YM2149")
+    py::enum_<AYInterface::TypeEnum::Enum>(m, "ChipType")
+        .value("AY", AYInterface::TypeEnum::AY, "AY-3-8910")
+        .value("YM", AYInterface::TypeEnum::YM, "YM2149")
         .export_values();
 
     py::enum_<AYInterface::EnvShapeEnum::Enum>(m, "EnvShape")
         .value("DOWN_HOLD_BOTTOM_0", AYInterface::EnvShapeEnum::DOWN_HOLD_BOTTOM_0, "\\___" )
         .value("DOWN_HOLD_BOTTOM_1", AYInterface::EnvShapeEnum::DOWN_HOLD_BOTTOM_1, "\\___" )
         .value("DOWN_HOLD_BOTTOM_2", AYInterface::EnvShapeEnum::DOWN_HOLD_BOTTOM_2, "\\___" )
         .value("DOWN_HOLD_BOTTOM_3", AYInterface::EnvShapeEnum::DOWN_HOLD_BOTTOM_3, "\\___" )
@@ -54,21 +54,21 @@
 
     py::class_<RegisterWrapper>(m, "Register")
         .def(py::init<AyumiEmulator&>())
         .def("__setitem__", &RegisterWrapper::setR)
         ;
 
     py::class_<AyumiEmulator>(m, "Ayumi")
-        .def_property_readonly_static("AY", [](py::object) { return AYInterface::AY; })
-        .def_property_readonly_static("YM", [](py::object) { return AYInterface::YM; })
+        .def_property_readonly_static("AY", [](py::object) { return AYInterface::TypeEnum::AY; })
+        .def_property_readonly_static("YM", [](py::object) { return AYInterface::TypeEnum::YM; })
 
-        .def(py::init<int, double, AYInterface::Enum>(),
+        .def(py::init<int, double, AYInterface::TypeEnum::Enum>(),
              py::arg("sample_rate") = 44100,
              py::arg("clock") = 1773400,
-             py::arg("type") = AYInterface::AY
+             py::arg("type") = AYInterface::TypeEnum::AY
         )
         .def_property_readonly("R", [](AyumiEmulator& AY) { return RegisterWrapper(AY); },
               py::return_value_policy::reference_internal)
 
         .def("set_registers", [](AyumiEmulator& AY, const std::vector<uint8_t>& regs, const std::vector<uint8_t>& values) {
             if (regs.size() != values.size()) {
                 throw std::invalid_argument("Buffer sizes must match");
@@ -201,32 +201,32 @@
             }
             float* outLeftPtr = static_cast<float*>(outLeftInfo.ptr);
             float* outRightPtr = static_cast<float*>(outRightInfo.ptr);
             const int stride = 1;
             AY.processBlock(outLeftPtr, outRightPtr, samples, stride, remove_dc);
         }, py::arg("out_left"), py::arg("out_right"), py::arg("samples"), py::arg("remove_dc") = true)
 
-        .def("reset", [](AyumiEmulator& AY, int sampleRate, double clock, AYInterface::Enum type) {
+        .def("reset", [](AyumiEmulator& AY, int sampleRate, double clock, AYInterface::TypeEnum::Enum type) {
             AY.Reset(sampleRate, clock, type);
             },
             py::arg("sample_rate") = 44100,
             py::arg("clock") = 1773400.0,
-            py::arg("type") = AYInterface::AY
+            py::arg("type") = AYInterface::TypeEnum::AY
         )
         .def("can_change_clock", &AyumiEmulator::canChangeClock)
         .def("can_change_clock_continously", &AyumiEmulator::canChangeClockContinously)
         .def("get_clock_values", &AyumiEmulator::getClockValues)
         .def("set_sample_rate", &AyumiEmulator::setSampleRate, py::arg("sampleRate"))
         .def("get_sample_rate", &AyumiEmulator::getSampleRate)
 
-        .def("set_type", [](AyumiEmulator& AY, AYInterface::Enum type) {
+        .def("set_type", [](AyumiEmulator& AY, AYInterface::TypeEnum::Enum type) {
             AY.setType(type);
         }, py::arg("type"))
         .def("get_type", [](AyumiEmulator& AY) {
-            return static_cast<AYInterface::Enum>(AY.getType()); })
+            return static_cast<AYInterface::TypeEnum::Enum>(AY.getType()); })
 
         .def("get_clock", &AyumiEmulator::getClock)
         .def("set_clock", &AyumiEmulator::setClock, py::arg("rate"))
 
         .def("set_pan", &AyumiEmulator::setPan,
             py::arg("index"), py::arg("value"), py::arg("is_eqp") = false)
         .def("get_pan", &AyumiEmulator::getPan, py::arg("index"))
```

### Comparing `pyayay-0.1.0/tests/test_ayumi.py` & `pyayay-0.1.0a2/tests/test_ayumi.py`

 * *Files identical despite different names*

