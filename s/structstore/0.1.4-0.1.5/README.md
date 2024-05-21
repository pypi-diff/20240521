# Comparing `tmp/structstore-0.1.4.tar.gz` & `tmp/structstore-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structstore-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "structstore-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `structstore-0.1.4.tar` & `structstore-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4654 2024-05-14 11:26:54.360922 structstore-0.1.4/CMakeLists.txt
--rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.4/LICENSE
--rw-r--r--   0        0        0     3879 2024-05-13 22:03:39.240898 structstore-0.1.4/README.md
--rw-r--r--   0        0        0      709 2024-05-14 08:27:19.167743 structstore-0.1.4/cmake/NanobindStubgen.cmake
--rw-r--r--   0        0        0      462 2024-05-13 21:53:42.800696 structstore-0.1.4/cmake/StructStoreConfig.cmake.in
--rw-r--r--   0        0        0      378 2024-05-13 21:20:28.538842 structstore-0.1.4/cmake/StructStoreConfigVersion.cmake.in
--rw-r--r--   0        0        0      385 2024-05-13 21:43:45.044481 structstore-0.1.4/include/structstore/structstore.hpp
--rw-r--r--   0        0        0    13883 2024-05-13 21:43:45.034481 structstore-0.1.4/include/structstore/stst_alloc.hpp
--rw-r--r--   0        0        0     4778 2024-05-14 09:32:31.984724 structstore-0.1.4/include/structstore/stst_containers.hpp
--rw-r--r--   0        0        0     4721 2024-05-13 21:43:45.094481 structstore-0.1.4/include/structstore/stst_field.hpp
--rw-r--r--   0        0        0     1178 2024-05-13 21:07:08.207963 structstore-0.1.4/include/structstore/stst_hashstring.hpp
--rw-r--r--   0        0        0     1578 2024-05-14 10:53:18.590588 structstore-0.1.4/include/structstore/stst_lock.hpp
--rw-r--r--   0        0        0     1255 2024-05-13 21:43:45.071147 structstore-0.1.4/include/structstore/stst_serialization.hpp
--rw-r--r--   0        0        0     4230 2024-05-13 21:43:45.084481 structstore-0.1.4/include/structstore/stst_shared.hpp
--rw-r--r--   0        0        0     5402 2024-05-13 21:43:45.104481 structstore-0.1.4/include/structstore/stst_structstore.hpp
--rw-r--r--   0        0        0     1422 2024-05-14 07:45:17.149944 structstore-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.4/src/main.bak.cpp
--rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.4/src/main.cpp
--rw-r--r--   0        0        0     1024 2024-05-13 21:43:45.054481 structstore-0.1.4/src/structstore.cpp
--rw-r--r--   0        0        0      246 2024-05-14 11:26:54.340922 structstore-0.1.4/src/structstore/__init__.py
--rw-r--r--   0        0        0    17005 2024-05-14 11:23:13.947177 structstore-0.1.4/src/structstore_bindings.cpp
--rw-r--r--   0        0        0      975 2024-05-13 21:43:44.997814 structstore-0.1.4/src/structstore_containers.cpp
--rw-r--r--   0        0        0      336 2024-05-13 21:43:45.064481 structstore-0.1.4/src/structstore_field.cpp
--rw-r--r--   0        0        0     2644 2024-05-13 21:43:45.017814 structstore-0.1.4/src/structstore_serialization.cpp
--rw-r--r--   0        0        0     8919 2024-05-13 21:43:45.027814 structstore-0.1.4/src/structstore_shared.cpp
--rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4654 2024-05-21 07:26:59.509136 structstore-0.1.5/CMakeLists.txt
+-rw-r--r--   0        0        0     1489 2022-11-06 13:29:39.097613 structstore-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3879 2024-05-21 06:58:01.634087 structstore-0.1.5/README.md
+-rw-r--r--   0        0        0      709 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/NanobindStubgen.cmake
+-rw-r--r--   0        0        0      462 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/StructStoreConfig.cmake.in
+-rw-r--r--   0        0        0      378 2024-05-14 11:34:33.427123 structstore-0.1.5/cmake/StructStoreConfigVersion.cmake.in
+-rw-r--r--   0        0        0      385 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/structstore.hpp
+-rw-r--r--   0        0        0    13883 2024-05-16 12:14:20.969152 structstore-0.1.5/include/structstore/stst_alloc.hpp
+-rw-r--r--   0        0        0     5117 2024-05-21 07:26:43.262447 structstore-0.1.5/include/structstore/stst_containers.hpp
+-rw-r--r--   0        0        0     4712 2024-05-21 07:26:43.262447 structstore-0.1.5/include/structstore/stst_field.hpp
+-rw-r--r--   0        0        0     1178 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_hashstring.hpp
+-rw-r--r--   0        0        0     1578 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_lock.hpp
+-rw-r--r--   0        0        0     1255 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/stst_serialization.hpp
+-rw-r--r--   0        0        0     4230 2024-05-21 06:57:50.027421 structstore-0.1.5/include/structstore/stst_shared.hpp
+-rw-r--r--   0        0        0     5402 2024-05-21 06:58:01.634087 structstore-0.1.5/include/structstore/stst_structstore.hpp
+-rw-r--r--   0        0        0     1422 2024-05-14 11:34:33.427123 structstore-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1250 2022-11-18 12:53:02.673000 structstore-0.1.5/src/main.bak.cpp
+-rw-r--r--   0        0        0     1355 2022-11-20 10:32:04.499910 structstore-0.1.5/src/main.cpp
+-rw-r--r--   0        0        0     1024 2024-05-21 06:58:01.634087 structstore-0.1.5/src/structstore.cpp
+-rw-r--r--   0        0        0      246 2024-05-21 07:26:59.519136 structstore-0.1.5/src/structstore/__init__.py
+-rw-r--r--   0        0        0    16485 2024-05-21 07:26:43.262447 structstore-0.1.5/src/structstore_bindings.cpp
+-rw-r--r--   0        0        0     1069 2024-05-21 07:26:43.262447 structstore-0.1.5/src/structstore_containers.cpp
+-rw-r--r--   0        0        0      336 2024-05-21 06:58:01.634087 structstore-0.1.5/src/structstore_field.cpp
+-rw-r--r--   0        0        0     2644 2024-05-21 06:58:01.637420 structstore-0.1.5/src/structstore_serialization.cpp
+-rw-r--r--   0        0        0     8919 2024-05-21 06:58:01.637420 structstore-0.1.5/src/structstore_shared.cpp
+-rw-r--r--   0        0        0     4220 1970-01-01 00:00:00.000000 structstore-0.1.5/PKG-INFO
```

### Comparing `structstore-0.1.4/CMakeLists.txt` & `structstore-0.1.5/CMakeLists.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.10)
-project(structstore VERSION 0.1.4)
+project(structstore VERSION 0.1.5)
 
 set(PY_VERSION_SUFFIX "")
 set(PY_FULL_VERSION ${PROJECT_VERSION}${PY_VERSION_SUFFIX})
 
 # make sure that the Python and CMake versions match
 if (DEFINED PY_BUILD_CMAKE_PACKAGE_VERSION)
     if (NOT "${PY_BUILD_CMAKE_PACKAGE_VERSION}" MATCHES "^${PY_FULL_VERSION}$")
```

### Comparing `structstore-0.1.4/LICENSE` & `structstore-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/README.md` & `structstore-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/cmake/NanobindStubgen.cmake` & `structstore-0.1.5/cmake/NanobindStubgen.cmake`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_alloc.hpp` & `structstore-0.1.5/include/structstore/stst_alloc.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_containers.hpp` & `structstore-0.1.5/include/structstore/stst_containers.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -111,28 +111,32 @@
     }
 };
 
 template<>
 void List::push_back<const char*>(const char* const& value);
 
 class Matrix {
+public:
+    static constexpr int MAX_DIMS = 4;
+
+protected:
     MiniMalloc& mm_alloc;
-    size_t _rows, _cols;
+    size_t _ndim;
+    size_t _shape[MAX_DIMS] = {};
     double* _data;
-    bool _is_vector = false;
 
 public:
     Matrix(MiniMalloc& mm_alloc) : Matrix(0, 0, mm_alloc) {}
 
-    Matrix(size_t rows, size_t cols, MiniMalloc& mm_alloc, bool is_vector = false)
-            : mm_alloc(mm_alloc), _rows(rows), _cols(cols), _is_vector(is_vector) {
-        if (rows == 0 || cols == 0) {
+    Matrix(size_t ndim, const size_t* shape, MiniMalloc& mm_alloc)
+            : mm_alloc(mm_alloc), _ndim(ndim) {
+        if (ndim == 0) {
             _data = nullptr;
         } else {
-            _data = (double*) mm_alloc.allocate(sizeof(double) * rows * cols);
+            from(ndim, shape, nullptr);
         }
     }
 
     ~Matrix() {
         if (_data != nullptr) {
             mm_alloc.deallocate(_data);
         }
@@ -142,54 +146,66 @@
 
     Matrix(const Matrix& other) : Matrix(0, 0, other.mm_alloc) {
         *this = other;
     }
 
     Matrix& operator=(Matrix&& other) {
         if (&mm_alloc == &other.mm_alloc) {
-            _data = other._data;
+            std::swap(_ndim, other._ndim);
+            std::swap(_shape, other._shape);
+            std::swap(_data, other._data);
         } else {
             const Matrix& other_ = other;
             *this = other_;
         }
-        other._data = nullptr;
         return *this;
     }
 
     Matrix& operator=(const Matrix& other) {
-        from(other._rows, other._cols, other._data, other._is_vector);
+        from(other._ndim, other._shape, other._data);
         return *this;
     }
 
-    double* data() { return _data; }
-
-    size_t rows() const { return _rows; }
+    size_t ndim() const { return _ndim; }
 
-    size_t cols() const { return _cols; }
+    const size_t* shape() const { return _shape; }
 
-    bool is_vector() const { return _is_vector; }
+    double* data() { return _data; }
 
-    void from(size_t rows, size_t cols, const double* data, bool is_vector) {
+    void from(size_t ndim, const size_t* shape, const double* data) {
         if (data == _data) {
-            if (rows != _rows || cols != _cols) {
+            if (ndim != _ndim) {
                 throw std::runtime_error("setting matrix data to same pointer but different size");
             }
-            _is_vector = is_vector;
+            for (size_t i = 0; i < ndim; ++i) {
+                if (shape[i] != _shape[i]) {
+                    throw std::runtime_error("setting matrix data to same pointer but different size");
+                }
+            }
             return;
         }
-        if (_data == nullptr || rows != _rows || cols != _cols) {
-            if (_data != nullptr) {
-                mm_alloc.deallocate(_data);
+        if (_data != nullptr) {
+            mm_alloc.deallocate(_data);
+            _data = nullptr;
+        }
+        _ndim = ndim;
+        size_t size = sizeof(double);
+        for (size_t i = 0; i < ndim; ++i) {
+            if ((ssize_t) shape[i] < 0) {
+                throw std::runtime_error("initializing matrix with invalid shape");
+            }
+            _shape[i] = shape[i];
+            size *= shape[i];
+        }
+        if (size > 0) {
+            _data = (double*) mm_alloc.allocate(size);
+            if (data != nullptr) {
+                std::memcpy(_data, data, size);
             }
-            _rows = rows;
-            _cols = cols;
-            _is_vector = is_vector;
-            _data = (double*) mm_alloc.allocate(sizeof(double) * _rows * _cols);
         }
-        std::memcpy(_data, data, sizeof(double) * _rows * _cols);
     }
 
     friend std::ostream& operator<<(std::ostream& os, const Matrix& self);
 };
 
 }
```

### Comparing `structstore-0.1.4/include/structstore/stst_field.hpp` & `structstore-0.1.5/include/structstore/stst_field.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         if (FieldType<T>::value != type) {
             throw std::runtime_error("field accessed with wrong type");
         }
         return *(T*) data;
     }
 
     template<typename T>
-    explicit operator T&() {
+    operator T&() {
         return get<T>();
     }
 
     template<typename T>
     StructStoreField& operator=(const T& value) {
         get<T>() = value;
         return *this;
```

### Comparing `structstore-0.1.4/include/structstore/stst_hashstring.hpp` & `structstore-0.1.5/include/structstore/stst_hashstring.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_lock.hpp` & `structstore-0.1.5/include/structstore/stst_lock.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_serialization.hpp` & `structstore-0.1.5/include/structstore/stst_serialization.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_shared.hpp` & `structstore-0.1.5/include/structstore/stst_shared.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/include/structstore/stst_structstore.hpp` & `structstore-0.1.5/include/structstore/stst_structstore.hpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/pyproject.toml` & `structstore-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/src/main.bak.cpp` & `structstore-0.1.5/src/main.bak.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/src/main.cpp` & `structstore-0.1.5/src/main.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/src/structstore.cpp` & `structstore-0.1.5/src/structstore.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/src/structstore_bindings.cpp` & `structstore-0.1.5/src/structstore_bindings.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -38,27 +38,15 @@
             }
         case FieldTypeValue::MATRIX: {
             Matrix& m = field.get<Matrix>();
             // todo: in the recursive case use empty capsule to avoid copy?
             // then memory lifetime is managed by structstore field
             // auto parent = recursive ? nb::handle() : nb::capsule([]() {}).release();
             auto parent = nb::handle();
-
-            int ndim;
-            size_t shape[2];
-            if (m.is_vector()) {
-                ndim = 1;
-                shape[0] = m.rows() * m.cols();
-            } else {
-                ndim = 2;
-                shape[0] = m.rows();
-                shape[1] = m.cols();
-            }
-
-            return nb::cast(nb::ndarray<double, nb::c_contig, nb::numpy>(m.data(), ndim, shape, parent));
+            return nb::cast(nb::ndarray<double, nb::c_contig, nb::numpy>(m.data(), m.ndim(), m.shape(), parent));
         }
         case FieldTypeValue::EMPTY:
             return nb::none();
         default:
             throw std::runtime_error("this type cannot be stored in a StructStore");
     }
 }
@@ -93,27 +81,18 @@
         access.get<double>() = nb::cast<double>(value);
     } else if (nb::isinstance<nb::str>(value)) {
         access.set_type<structstore::string>();
         access.get<structstore::string>() = nb::cast<std::string>(value);
     } else if (nb::ndarray_check(value)) {
         access.set_type<Matrix>();
         auto array = nb::cast<nb::ndarray<const double, nb::c_contig>>(value);
-        size_t rows, cols;
-        bool is_vector = false;
-        if (array.ndim() == 1) {
-            rows = array.shape(0);
-            cols = 1;
-            is_vector = true;
-        } else if (array.ndim() == 2) {
-            rows = array.shape(0);
-            cols = array.shape(1);
-        } else {
+        if (array.ndim() > Matrix::MAX_DIMS) {
             throw std::runtime_error("Incompatible buffer dimension!");
         }
-        access.get<Matrix>().from(rows, cols, array.data(), is_vector);
+        access.get<Matrix>().from(array.ndim(), (const size_t*) array.shape_ptr(), array.data());
     } else if (nb::hasattr(value, "__dict__")) {
         access.set_type<StructStore>();
         auto dict = nb::dict(value.attr("__dict__"));
         StructStore& store = access.get<StructStore>();
         store.clear();
         for (const auto& [key, val]: dict) {
             std::string key_str = nb::cast<std::string>(key);
```

### Comparing `structstore-0.1.4/src/structstore_containers.cpp` & `structstore-0.1.5/src/structstore_containers.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -19,18 +19,22 @@
     auto node = YAML::Node(YAML::NodeType::Sequence);
     for (const StructStoreField& field: list) {
         node.push_back(to_yaml(field));
     }
     return node;
 }
 
-std::ostream& structstore::operator<<(std::ostream& os, const Matrix& self) {
+std::ostream& structstore::operator<<(std::ostream& os, const Matrix& matrix) {
+    size_t size = 1;
+    for (size_t i = 0; i < matrix._ndim; ++i) {
+        size *= matrix._shape[i];
+    }
     os << "[";
-    for (size_t i = 0; i < self._rows * self._cols; ++i) {
-        os << self._data[i] << ",";
+    for (size_t i = 0; i < size; ++i) {
+        os << matrix._data[i] << ",";
     }
     return os << "]";
 }
 
 void structstore::destruct(List& list) {
     list.~List();
 }
```

### Comparing `structstore-0.1.4/src/structstore_serialization.cpp` & `structstore-0.1.5/src/structstore_serialization.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/src/structstore_shared.cpp` & `structstore-0.1.5/src/structstore_shared.cpp`

 * *Files identical despite different names*

### Comparing `structstore-0.1.4/PKG-INFO` & `structstore-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: structstore
-Version: 0.1.4
+Version: 0.1.5
 Summary: Structured object storage, dynamically typed, to be shared between processes
 Author-email: Max Mertens <max.mail@dameweb.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: nanobind
 Project-URL: Homepage, https://github.com/mertemba/structstore
```

