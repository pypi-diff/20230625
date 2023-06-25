# Comparing `tmp/viterbi-0.0.3.tar.gz` & `tmp/viterbi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viterbi-0.0.3.tar", last modified: Sat Jun 24 09:22:07 2023, max compression
+gzip compressed data, was "viterbi-0.0.4.tar", last modified: Sun Jun 25 06:03:17 2023, max compression
```

## Comparing `viterbi-0.0.3.tar` & `viterbi-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:22:07.248939 viterbi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-24 09:21:57.000000 viterbi-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-24 09:21:57.000000 viterbi-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-24 09:22:07.248939 viterbi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-24 09:21:57.000000 viterbi-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-24 09:21:57.000000 viterbi-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 09:22:07.248939 viterbi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-24 09:21:57.000000 viterbi-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 09:22:07.244939 viterbi-0.0.3/viterbi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-24 09:22:07.000000 viterbi-0.0.3/viterbi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.h
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-24 09:21:57.000000 viterbi-0.0.3/viterbi_python.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:03:17.759557 viterbi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-25 06:03:08.000000 viterbi-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-25 06:03:08.000000 viterbi-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-25 06:03:17.759557 viterbi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-25 06:03:08.000000 viterbi-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-25 06:03:08.000000 viterbi-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 06:03:17.763557 viterbi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-25 06:03:08.000000 viterbi-0.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-25 06:03:08.000000 viterbi-0.0.4/viterbi.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 06:03:17.759557 viterbi-0.0.4/viterbi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-25 06:03:17.000000 viterbi-0.0.4/viterbi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 06:03:17.000000 viterbi-0.0.4/viterbi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 06:03:17.000000 viterbi-0.0.4/viterbi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-25 06:03:17.000000 viterbi-0.0.4/viterbi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-25 06:03:08.000000 viterbi-0.0.4/viterbi.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-25 06:03:08.000000 viterbi-0.0.4/viterbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-25 06:03:08.000000 viterbi-0.0.4/viterbi_python.cpp
```

### Comparing `viterbi-0.0.3/LICENSE` & `viterbi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `viterbi-0.0.3/PKG-INFO` & `viterbi-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viterbi
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Convolutional Encoder and Viterbi Decoder in Python/C++.
 Author-email: Yachen Mao <maoyachen55@gmail.com>, Min Xu <xukmin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,34 +201,49 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Project-URL: Source, https://github.com/clysto/viterbi
 Keywords: viterbi
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Convolutional Encoder and Viterbi Decoder
 
+![License](https://img.shields.io/github/license/clysto/viterbi)
+![Version](https://img.shields.io/github/tag/clysto/viterbi)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/viterbi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/viterbi)
+
 > This project is a fork of <https://github.com/xukmin/viterbi> that introduces Python support, enabling effortless utilization of the Viterbi module within the Python environment.
 
 ## Install
 
 ```sh
 pip install viterbi
 ```
 
 ## Usage
 
 The following is a convolutional encoder with a constraint length of 7. The diagram indicates the binary values and polynomial form, indicating the left-most bit is the most-significant-bit (MSB). The generating polynomials are 1011011 and 1111001 can be alternatively expressed in octal as 133 and 171, respectively.
 
-![convolutional encoder](docs/convolutional%20encoder.svg)
+![convolutional encoder](https://raw.githubusercontent.com/clysto/viterbi/master/docs/convolutional%20encoder.svg)
 
 Expressed in code as:
 
 ```python
 from viterbi import Viterbi
 dot11a_codec = Viterbi(7, [0o133, 0o171])
 ```
@@ -242,10 +257,21 @@
 bits = [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 output = dot11a_codec.encode(bits)
 # [0, 0, 1, 1, 0, 1, 0, 0, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0, 1]
 dot11a_codec.decode(output)
 # [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 ```
 
+## Puncturing
+
+This library also allows you to puncture the original encoded data by specifying a puncture pattern or decode data that has already been punctured.
+
+```python
+from viterbi import Viterbi
+
+# Puncture Pattern: [1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1]
+dot11a_codec = Viterbi(7, [0o133, 0o171], [1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1])
+```
+
 ## Using in C++
 
 You can find the way to use the Viterbi decoder in C++ in the [README](https://github.com/xukmin/viterbi) of the original project.
```

### Comparing `viterbi-0.0.3/viterbi.cpp` & `viterbi-0.0.4/viterbi.cpp`

 * *Files identical despite different names*

### Comparing `viterbi-0.0.3/viterbi.egg-info/PKG-INFO` & `viterbi-0.0.4/viterbi.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viterbi
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Convolutional Encoder and Viterbi Decoder in Python/C++.
 Author-email: Yachen Mao <maoyachen55@gmail.com>, Min Xu <xukmin@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -201,34 +201,49 @@
         
            Unless required by applicable law or agreed to in writing, software
            distributed under the License is distributed on an "AS IS" BASIS,
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
+Project-URL: Source, https://github.com/clysto/viterbi
 Keywords: viterbi
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Convolutional Encoder and Viterbi Decoder
 
+![License](https://img.shields.io/github/license/clysto/viterbi)
+![Version](https://img.shields.io/github/tag/clysto/viterbi)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/viterbi)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/viterbi)
+
 > This project is a fork of <https://github.com/xukmin/viterbi> that introduces Python support, enabling effortless utilization of the Viterbi module within the Python environment.
 
 ## Install
 
 ```sh
 pip install viterbi
 ```
 
 ## Usage
 
 The following is a convolutional encoder with a constraint length of 7. The diagram indicates the binary values and polynomial form, indicating the left-most bit is the most-significant-bit (MSB). The generating polynomials are 1011011 and 1111001 can be alternatively expressed in octal as 133 and 171, respectively.
 
-![convolutional encoder](docs/convolutional%20encoder.svg)
+![convolutional encoder](https://raw.githubusercontent.com/clysto/viterbi/master/docs/convolutional%20encoder.svg)
 
 Expressed in code as:
 
 ```python
 from viterbi import Viterbi
 dot11a_codec = Viterbi(7, [0o133, 0o171])
 ```
@@ -242,10 +257,21 @@
 bits = [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 output = dot11a_codec.encode(bits)
 # [0, 0, 1, 1, 0, 1, 0, 0, 1, 0, 1, 1, 0, 1, 1, 1, 0, 1, 0, 1, 0, 1, 0, 1]
 dot11a_codec.decode(output)
 # [0, 1, 0, 1, 0, 0, 0, 0, 1, 1, 1, 0]
 ```
 
+## Puncturing
+
+This library also allows you to puncture the original encoded data by specifying a puncture pattern or decode data that has already been punctured.
+
+```python
+from viterbi import Viterbi
+
+# Puncture Pattern: [1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1]
+dot11a_codec = Viterbi(7, [0o133, 0o171], [1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1, 1, 1, 1, 0, 0, 1])
+```
+
 ## Using in C++
 
 You can find the way to use the Viterbi decoder in C++ in the [README](https://github.com/xukmin/viterbi) of the original project.
```

### Comparing `viterbi-0.0.3/viterbi.h` & `viterbi-0.0.4/viterbi.h`

 * *Files identical despite different names*

### Comparing `viterbi-0.0.3/viterbi.py` & `viterbi-0.0.4/viterbi.py`

 * *Files identical despite different names*

