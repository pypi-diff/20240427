# Comparing `tmp/pycxpress-0.0.5.tar.gz` & `tmp/pycxpress-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycxpress-0.0.5.tar", max compression
+gzip compressed data, was "pycxpress-0.0.6.tar", max compression
```

## Comparing `pycxpress-0.0.5.tar` & `pycxpress-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1066 2024-04-25 17:09:19.066959 pycxpress-0.0.5/LICENSE
--rw-r--r--   0        0        0     2324 2024-04-25 17:09:19.066959 pycxpress-0.0.5/README.md
--rw-r--r--   0        0        0     4030 2024-04-25 17:09:19.070959 pycxpress-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1036 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/__init__.py
--rw-r--r--   0        0        0      947 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/__main__.py
--rw-r--r--   0        0        0     5428 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/core.py
--rw-r--r--   0        0        0     1501 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/debugger.py
--rw-r--r--   0        0        0      999 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/Makefile
--rw-r--r--   0        0        0     1730 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/main.cpp
--rw-r--r--   0        0        0     2633 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/example/model.py
--rw-r--r--   0        0        0     9174 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/core.hpp
--rw-r--r--   0        0        0      849 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/utils.hpp
--rw-r--r--   0        0        0     1033 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/interface.py
--rw-r--r--   0        0        0      714 2024-04-25 17:09:19.070959 pycxpress-0.0.5/src/PyCXpress/utils.py
--rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 pycxpress-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-27 06:43:40.521206 pycxpress-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2324 2024-04-27 06:43:40.521206 pycxpress-0.0.6/README.md
+-rw-r--r--   0        0        0     4030 2024-04-27 06:43:40.521206 pycxpress-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1036 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/__main__.py
+-rw-r--r--   0        0        0     5428 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/core.py
+-rw-r--r--   0        0        0     1501 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/debugger.py
+-rw-r--r--   0        0        0      999 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/Makefile
+-rw-r--r--   0        0        0     2320 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/main.cpp
+-rw-r--r--   0        0        0     2635 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/example/model.py
+-rw-r--r--   0        0        0    10312 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/core.hpp
+-rw-r--r--   0        0        0      849 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/utils.hpp
+-rw-r--r--   0        0        0     1033 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/interface.py
+-rw-r--r--   0        0        0      714 2024-04-27 06:43:40.521206 pycxpress-0.0.6/src/PyCXpress/utils.py
+-rw-r--r--   0        0        0     3669 1970-01-01 00:00:00.000000 pycxpress-0.0.6/PKG-INFO
```

### Comparing `pycxpress-0.0.5/LICENSE` & `pycxpress-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/README.md` & `pycxpress-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/pyproject.toml` & `pycxpress-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "PyCXpress"
-version = "0.0.5"
+version = "0.0.6"
 description = "PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing."
 readme = "README.md"
 authors = ["chaoqing <chaoqingwang.nick@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/chaoqing/PyCXpress"
 homepage = "https://github.com/chaoqing/PyCXpress"
 packages = [
```

### Comparing `pycxpress-0.0.5/src/PyCXpress/__init__.py` & `pycxpress-0.0.6/src/PyCXpress/__init__.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/__main__.py` & `pycxpress-0.0.6/src/PyCXpress/__main__.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/core.py` & `pycxpress-0.0.6/src/PyCXpress/core.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/debugger.py` & `pycxpress-0.0.6/src/PyCXpress/debugger.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/example/Makefile` & `pycxpress-0.0.6/src/PyCXpress/example/Makefile`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/example/main.cpp` & `pycxpress-0.0.6/src/PyCXpress/example/main.cpp`

 * *Files 19% similar despite different names*

```diff
@@ -4,43 +4,57 @@
 #define PYBIND11_DETAILED_ERROR_MESSAGES
 
 #include <PyCXpress/core.hpp>
 #include <PyCXpress/utils.hpp>
 
 namespace pcx = PyCXpress;
 
-void show_test(pcx::Model &python) {
+void show_test(pcx::Model &model) {
     std::vector<double> data(12);
     for (size_t i = 0; i < 12; i++) {
         data[i] = i;
     }
 
-    std::vector<uint8_t> shape = {3, 4};
-    memcpy(python.set_buffer("data_to_be_reshaped", {12}), data.data(),
-           data.size() * sizeof(double));
-    memcpy(python.set_buffer("new_2d_shape", {2}), shape.data(),
+    std::vector<uint8_t> shape   = {3, 4};
+    void                *pBuffer = nullptr;
+    size_t               nBytes  = 0;
+    std::tie(pBuffer, nBytes) = model.set_buffer("data_to_be_reshaped", {12});
+    assert(data.size() * sizeof(double) == nBytes);
+
+    memcpy(pBuffer, data.data(), nBytes);
+    memcpy(model.set_buffer("new_2d_shape", {2}).first, shape.data(),
            shape.size() * sizeof(uint8_t));
 
-    python.run();
+    model.run();
 
+    // test retrieve output tensor
     void               *p = nullptr;
     std::vector<size_t> new_shape;
-    std::tie(p, new_shape) = python.get_buffer("output_a");
+    pcx::BufferPtr      buf;
+    std::tie(buf, new_shape) = model.get_buffer("output_a");
+    std::tie(p, nBytes)      = buf;
 
     std::cout << "output shape: ";
     std::copy(new_shape.begin(), new_shape.end(),
               std::ostream_iterator<size_t>(std::cout, ", "));
     std::cout << std::endl;
 
     size_t size = std::accumulate(new_shape.begin(), new_shape.end(), 1,
                                   std::multiplies<int>());
+    assert(nBytes == sizeof(double) * size);
     std::cout << "output data: ";
     std::copy((double *)p, (double *)p + size,
               std::ostream_iterator<double>(std::cout, ", "));
     std::cout << std::endl;
+
+    // test retrieve input tensor
+    std::tie(buf, new_shape) = model.get_buffer("new_2d_shape");
+    assert(new_shape.size() == 1 && new_shape.front() == shape.size());
+    assert(buf.second == shape.size() * sizeof(uint8_t));
+    assert(0 == std::memcmp(buf.first, shape.data(), buf.second));
 }
 
 int main(int argc, char *argv[]) {
     auto &python     = utils::Singleton<pcx::PythonInterpreter>::Instance();
     auto &model0     = python.create_model("model.Model");
     auto &model1     = python.create_model("model.Model", "odd");
     int   loop_times = 3;
```

### Comparing `pycxpress-0.0.5/src/PyCXpress/example/model.py` & `pycxpress-0.0.6/src/PyCXpress/example/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.model(self.input, self.output)
 
     @staticmethod
     def model(input: InputDataSet, output: OutputDataSet):
         with nullcontext():
             # print(input.data_to_be_reshaped)
             # print(input.new_2d_shape)
-            output.output_a = input.data_to_be_reshaped.reshape(input.new_2d_shape)
+            output.output_a = input.data_to_be_reshaped.reshape(input.new_2d_shape).T
             # print(output.output_a)
 
 
 def main():
 
     model = Model()
     input_data, output_data, spec = model.initialize()
```

### Comparing `pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/core.hpp` & `pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/core.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -20,109 +20,114 @@
 #endif
 #endif
 
 namespace PyCXpress {
 namespace py = pybind11;
 using namespace utils;
 
-class PYCXPRESS_EXPORT Buffer {
+typedef std::pair<void *, size_t> BufferPtr;
+class PYCXPRESS_EXPORT            Buffer {
     typedef unsigned char Bytes;
 
     template <typename T>
     static py::array __to_array(const std::vector<size_t> &shape, void *data,
-                                size_t max_size) {
-        std::vector<size_t> stride(shape.size());
-        *stride.rbegin() = sizeof(T);
-        auto ps          = shape.rbegin();
-        for (auto pt = stride.rbegin() + 1; pt != stride.rend(); pt++, ps++) {
-            *pt = *(pt - 1) * (*ps);
-        }
-        if (max_size < stride.front() * shape.front()) {
-            throw std::runtime_error("Buffer size is too small");
-        }
-        return py::array_t<T>{shape, std::move(stride), (T *)(data),
-                              py::none()};
+                                           size_t &max_size) {
+                   std::vector<size_t> stride(shape.size());
+                   *stride.rbegin() = sizeof(T);
+                   auto ps          = shape.rbegin();
+                   for (auto pt = stride.rbegin() + 1; pt != stride.rend(); pt++, ps++) {
+                       *pt = *(pt - 1) * (*ps);
+        }
+                   auto real_size = stride.front() * shape.front();
+                   if (max_size < real_size) {
+                       throw std::runtime_error("Buffer size is too small");
+        }
+                   max_size = real_size;
+                   return py::array_t<T>{shape, std::move(stride), (T *)(data),
+                                         py::none()};
     }
 
 public:
     Buffer() : m_size(0), m_data(nullptr), m_converter(nullptr) {}
     Buffer(size_t size, const std::string &data_type) : m_size(size) {
-        m_data   = new Bytes[m_size];
-        m_length = size;
+                   m_data = new Bytes[m_size];
 
-        if (data_type == "bool") {
-            m_converter = __to_array<bool>;
-            m_length /= sizeof(bool);
+                   if (data_type == "bool") {
+                       m_converter = __to_array<bool>;
+                       m_itemsize  = sizeof(bool);
         } else if (data_type == "int8_t") {
-            m_converter = __to_array<int8_t>;
-            m_length /= sizeof(int8_t);
+                       m_converter = __to_array<int8_t>;
+                       m_itemsize  = sizeof(int8_t);
         } else if (data_type == "int16_t") {
-            m_converter = __to_array<int16_t>;
-            m_length /= sizeof(int16_t);
+                       m_converter = __to_array<int16_t>;
+                       m_itemsize  = sizeof(int16_t);
         } else if (data_type == "int32_t") {
-            m_converter = __to_array<int32_t>;
-            m_length /= sizeof(int32_t);
+                       m_converter = __to_array<int32_t>;
+                       m_itemsize  = sizeof(int32_t);
         } else if (data_type == "int64_t") {
-            m_converter = __to_array<int64_t>;
-            m_length /= sizeof(int64_t);
+                       m_converter = __to_array<int64_t>;
+                       m_itemsize  = sizeof(int64_t);
         } else if (data_type == "uint8_t") {
-            m_converter = __to_array<uint8_t>;
-            m_length /= sizeof(uint8_t);
+                       m_converter = __to_array<uint8_t>;
+                       m_itemsize  = sizeof(uint8_t);
         } else if (data_type == "uint16_t") {
-            m_converter = __to_array<uint16_t>;
-            m_length /= sizeof(uint16_t);
+                       m_converter = __to_array<uint16_t>;
+                       m_itemsize  = sizeof(uint16_t);
         } else if (data_type == "uint32_t") {
-            m_converter = __to_array<uint32_t>;
-            m_length /= sizeof(uint32_t);
+                       m_converter = __to_array<uint32_t>;
+                       m_itemsize  = sizeof(uint32_t);
         } else if (data_type == "uint64_t") {
-            m_converter = __to_array<uint64_t>;
-            m_length /= sizeof(uint64_t);
+                       m_converter = __to_array<uint64_t>;
+                       m_itemsize  = sizeof(uint64_t);
         } else if (data_type == "float") {
-            m_converter = __to_array<float>;
-            m_length /= sizeof(float);
+                       m_converter = __to_array<float>;
+                       m_itemsize  = sizeof(float);
         } else if (data_type == "double") {
-            m_converter = __to_array<double>;
-            m_length /= sizeof(double);
+                       m_converter = __to_array<double>;
+                       m_itemsize  = sizeof(double);
         } else if (data_type == "char") {
-            m_converter = __to_array<char>;
-            m_length /= sizeof(char);
+                       m_converter = __to_array<char>;
+                       m_itemsize  = sizeof(char);
         } else {
-            throw NotImplementedError(data_type);
+                       throw NotImplementedError(data_type);
         }
     }
     Buffer(Buffer &&ohs)
         : m_size(ohs.m_size),
-          m_length(ohs.m_length),
+          m_itemsize(ohs.m_itemsize),
           m_data(ohs.m_data),
           m_converter(ohs.m_converter) {
-        ohs.m_data = nullptr;
+                   ohs.m_data = nullptr;
     }
 
     ~Buffer() {
-        delete[] m_data;
-        m_data = nullptr;
+                   delete[] m_data;
+                   m_data = nullptr;
     }
 
-    void *set(const std::vector<size_t> &shape) {
-        m_array = m_converter(shape, m_data, m_size);
-        return m_data;
+    BufferPtr set(const std::vector<size_t> &shape) {
+                   auto real_size = m_size;
+                   m_array        = m_converter(shape, m_data, real_size);
+                   return std::make_pair(m_data, real_size);
     }
 
-    inline size_t itemsize() const { return m_size / m_length; }
+    inline size_t itemsize() const { return m_itemsize; }
 
     py::array &array() { return m_array; }
 
-    void reset() { m_array = m_converter({m_length}, m_data, m_size); }
+    void reset() {
+                   m_array = m_converter({m_size / m_itemsize}, m_data, m_size);
+    }
 
 private:
     size_t    m_size;
-    size_t    m_length;
+    size_t    m_itemsize;
     Bytes    *m_data;
     py::array m_array;
-    py::array (*m_converter)(const std::vector<size_t> &, void *, size_t);
+    py::array (*m_converter)(const std::vector<size_t> &, void *, size_t &);
 };
 
 class PYCXPRESS_EXPORT Model {
 public:
     explicit Model(const std::string &path) {
         std::vector<char> module_name(path.data(), path.data() + path.length());
         if (module_name.empty() || module_name.back() == '.') {
@@ -151,33 +156,43 @@
         m_output_buffer_sizes.clear();
         m_model  = py::none();
         m_input  = py::none();
         m_output = py::none();
     }
 
 
-    void *set_buffer(const std::string         &name,
-                     const std::vector<size_t> &shape) {
-        auto &buf = m_buffers[name];
-        void *p   = buf.set(shape);
+    BufferPtr set_buffer(const std::string         &name,
+                         const std::vector<size_t> &shape) {
+        auto &buf  = m_buffers[name];
+        auto  pBuf = buf.set(shape);
         m_input.attr("set_buffer_value")(name, buf.array());
-        return p;
+        return pBuf;
     }
 
-    std::pair<void *, std::vector<size_t>> get_buffer(const std::string &name) {
-        auto &array  = m_buffers[name].array();
-        auto  pShape = m_output_buffer_sizes.find(name);
-        if (pShape == m_output_buffer_sizes.end()) {
-            return std::make_pair(
-                array.request().ptr,
-                std::vector<size_t>(array.shape(),
-                                    array.shape() + array.ndim()));
-        } else {
-            return std::make_pair(array.request().ptr, pShape->second);
-        }
+    std::pair<BufferPtr, std::vector<size_t>> get_buffer(
+        const std::string &name) {
+        auto &buf   = m_buffers[name];
+        auto &array = buf.array();
+
+        auto                iter = m_output_buffer_sizes.find(name);
+        std::vector<size_t> shape;
+        if (iter != m_output_buffer_sizes.end()) {
+            shape = iter->second;
+        } else {  // must be an input tensor, we do not suggest retrieve the
+                  // data from this interface
+            auto p = array.shape();
+            shape.resize(array.ndim());
+            std::copy_n(p, shape.size(), shape.begin());
+        }
+
+        auto nBytes = buf.itemsize() *
+                      std::accumulate(shape.begin(), shape.end(), size_t(1),
+                                      std::multiplies<size_t>());
+        return std::make_pair(std::make_pair(array.request().ptr, nBytes),
+                              std::move(shape));
     }
 
     void run() {
         m_model.attr("run")();
 
         auto get_buffer_shape = m_output.attr("get_buffer_shape");
```

### Comparing `pycxpress-0.0.5/src/PyCXpress/include/PyCXpress/utils.hpp` & `pycxpress-0.0.6/src/PyCXpress/include/PyCXpress/utils.hpp`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/interface.py` & `pycxpress-0.0.6/src/PyCXpress/interface.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/src/PyCXpress/utils.py` & `pycxpress-0.0.6/src/PyCXpress/utils.py`

 * *Files identical despite different names*

### Comparing `pycxpress-0.0.5/PKG-INFO` & `pycxpress-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCXpress
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyCXpress is a high-performance hybrid framework that seamlessly integrates Python and C++ to harness the flexibility of Python and the speed of C++ for efficient and expressive computation, particularly in the realm of deep learning and numerical computing.
 Home-page: https://github.com/chaoqing/PyCXpress
 License: MIT
 Keywords: CPP,Embdedding
 Author: chaoqing
 Author-email: chaoqingwang.nick@gmail.com
 Requires-Python: >=3.8,<4.0
```

