# Comparing `tmp/lanablas-0.0.6.tar.gz` & `tmp/lanablas-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.6.tar", last modified: Sat Jun 24 15:01:34 2023, max compression
+gzip compressed data, was "lanablas-0.0.7.tar", last modified: Sun Jun 25 09:32:20 2023, max compression
```

## Comparing `lanablas-0.0.6.tar` & `lanablas-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.597684 lanablas-0.0.6/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.6/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-24 15:01:34.597449 lanablas-0.0.6/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1547 2023-06-24 14:55:58.000000 lanablas-0.0.6/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.594761 lanablas-0.0.6/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-24 14:56:09.000000 lanablas-0.0.6/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    11138 2023-06-24 14:57:13.000000 lanablas-0.0.6/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-24 15:01:34.597010 lanablas-0.0.6/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-24 15:01:33.000000 lanablas-0.0.6/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-24 15:01:34.000000 lanablas-0.0.6/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-24 15:01:33.000000 lanablas-0.0.6/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-24 15:01:34.000000 lanablas-0.0.6/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-24 15:01:34.597766 lanablas-0.0.6/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-24 14:56:02.000000 lanablas-0.0.6/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.522398 lanablas-0.0.7/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.7/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-25 09:32:20.522155 lanablas-0.0.7/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1547 2023-06-25 09:11:41.000000 lanablas-0.0.7/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.520703 lanablas-0.0.7/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1113 2023-06-25 09:18:54.000000 lanablas-0.0.7/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    13273 2023-06-25 09:32:14.000000 lanablas-0.0.7/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-25 09:32:20.521792 lanablas-0.0.7/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1959 2023-06-25 09:32:19.000000 lanablas-0.0.7/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-25 09:32:20.000000 lanablas-0.0.7/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-25 09:32:19.000000 lanablas-0.0.7/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-25 09:32:20.000000 lanablas-0.0.7/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-25 09:32:20.522481 lanablas-0.0.7/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-25 09:11:36.000000 lanablas-0.0.7/setup.py
```

### Comparing `lanablas-0.0.6/LICENSE` & `lanablas-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lanablas-0.0.6/PKG-INFO` & `lanablas-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.6
+pip install lanablas==0.0.7
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.6/README.md` & `lanablas-0.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.6
+pip install lanablas==0.0.7
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.6/lanablas/__init__.py` & `lanablas-0.0.7/lanablas/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Union, List
 from matrix import Matrix
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 def inject(data: Union[float, int, List, List[List]]) -> List[List[float]]:
     """
     Injects the input data into a matrix.
 
     Args:
```

### Comparing `lanablas-0.0.6/lanablas/matrix.c` & `lanablas-0.0.7/lanablas/matrix.c`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+//TODO - Matrix_negative
+//TODO - Matrix_pow
+//TODO - Matrix_matmul
+//TODO - Matrix_truediv
 #include <Python.h>
 #include <cblas.h>
 
 
 typedef struct {
     PyObject_HEAD
     int rows;
@@ -288,22 +292,81 @@
     }
 
     return (PyObject*)result;
 
 }
 
 
+PyObject * Matrix_mul(PyObject *self, PyObject *other) {
+    // Cast the input objects to MatrixObject
+    MatrixObject* selfMatrix = (MatrixObject*)self;
+    MatrixObject* otherMatrix = (MatrixObject*)other;
+
+    // Check if the dimensions of the matrices are compatible for addition
+    if (selfMatrix->rows != otherMatrix->rows || selfMatrix->cols != otherMatrix->cols) {
+        PyErr_SetString(PyExc_ValueError, "Matrix dimensions are not compatible for addition");
+        return NULL;
+    }
+
+    // Create a new MatrixObject for the result
+    MatrixObject* result = (MatrixObject*)MatrixType.tp_alloc(&MatrixType, 0);
+    if (result == NULL) {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate memory for result matrix");
+        return NULL;
+    }
+
+    result->rows = selfMatrix->rows;
+    result->cols = selfMatrix->cols;
+    result->data = malloc(result->rows * sizeof(double*));
+    for (int i = 0; i < result->rows; i++) {
+        result->data[i] = malloc(result->cols * sizeof(double));
+        for (int j = 0; j < result->cols; j++) {
+            result->data[i][j] = selfMatrix->data[i][j] * otherMatrix->data[i][j];
+        }
+    }
+
+    return (PyObject*)result;
+
+}
+
+
+PyObject * Matrix_negative(PyObject *self) {
+    // Cast the input objects to MatrixObject
+    MatrixObject* selfMatrix = (MatrixObject*)self;
+
+    // Create a new MatrixObject for the result
+    MatrixObject* result = (MatrixObject*)MatrixType.tp_alloc(&MatrixType, 0);
+    if (result == NULL) {
+        PyErr_SetString(PyExc_MemoryError, "Failed to allocate memory for result matrix");
+        return NULL;
+    }
+
+    result->rows = selfMatrix->rows;
+    result->cols = selfMatrix->cols;
+    result->data = malloc(result->rows * sizeof(double*));
+    for (int i = 0; i < result->rows; i++) {
+        result->data[i] = malloc(result->cols * sizeof(double));
+        for (int j = 0; j < result->cols; j++) {
+            result->data[i][j] = selfMatrix->data[i][j] * -1;
+        }
+    }
+
+    return (PyObject*)result;
+
+}
+
+
 PyNumberMethods Matrix_as_number = {
     Matrix_add,
     Matrix_subtract,
+    Matrix_mul,
     0,
     0,
     0,
-    0,
-    0,
+    Matrix_negative,
     0,
     0,
     0,
     0,
     0,
     0,
     0,
```

### Comparing `lanablas-0.0.6/lanablas.egg-info/PKG-INFO` & `lanablas-0.0.7/lanablas.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanablas
-Version: 0.0.6
+Version: 0.0.7
 Summary: Extension module for matrix multiplication
 Author: Marco Salvalaggio
 Author-email: mar.salvalaggio@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -24,15 +24,15 @@
 
 
 ## Install 
 
 Actually, the package is currently only available for macOS x86. Wheels for ARM and Linux platforms will be added to the PyPI registry as soon as possible.
 
 ```console
-pip install lanablas==0.0.6
+pip install lanablas==0.0.7
 ```
 
 ## Example 
 
 ```python
 from lanablas import Matrix
```

### Comparing `lanablas-0.0.6/setup.py` & `lanablas-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.6',
+    version='0.0.7',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
```

