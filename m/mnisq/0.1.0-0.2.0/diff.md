# Comparing `tmp/mnisq-0.1.0.tar.gz` & `tmp/mnisq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnisq-0.1.0.tar", max compression
+gzip compressed data, was "mnisq-0.2.0.tar", max compression
```

## Comparing `mnisq-0.1.0.tar` & `mnisq-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    20139 2023-06-06 23:15:19.098044 mnisq-0.1.0/LICENSE
--rw-r--r--   0        0        0      656 2023-06-12 01:33:39.285052 mnisq-0.1.0/README.md
--rw-r--r--   0        0        0       95 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/__init__.py
--rw-r--r--   0        0        0       76 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/config/__init__.py
--rw-r--r--   0        0        0      301 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/fashion_mnist/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/fashion_mnist/loader.py
--rw-r--r--   0        0        0        0 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/__init__.py
--rw-r--r--   0        0        0      141 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/dataset/__init__.py
--rw-r--r--   0        0        0     4927 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/dataset/dataset.py
--rw-r--r--   0        0        0        0 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/__init__.py
--rw-r--r--   0        0        0    12506 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE.cpp
--rw-r--r--   0        0        0     1196 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE_from_program.py
--rw-r--r--   0        0        0     4572 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE_from_python.py
--rw-r--r--   0        0        0       86 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/aqce/__init__.py
--rw-r--r--   0        0        0        0 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/cifar_10/__init__.py
--rw-r--r--   0        0        0     2021 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/cifar_10/downloader.py
--rw-r--r--   0        0        0      564 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/cifar_10/gray_scale.py
--rw-r--r--   0        0        0     3095 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/generator/cifar_10/main.py
--rw-r--r--   0        0        0     3585 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/generator/mnist_like/Source.py
--rw-r--r--   0        0        0        0 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/mnist_like/__init__.py
--rw-r--r--   0        0        0       43 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/mnist_like/downloader/__init__.py
--rw-r--r--   0        0        0     4171 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/generator/mnist_like/downloader/mnist.py
--rw-r--r--   0        0        0    12896 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/generator/mnist_like/qasm_converter.py
--rw-r--r--   0        0        0        0 2023-06-06 23:15:19.128044 mnisq-0.1.0/mnisq/internal/loader/__init__.py
--rw-r--r--   0        0        0       83 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/loader/mnist_like/__init__.py
--rw-r--r--   0        0        0     1353 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/internal/loader/mnist_like/load.py
--rw-r--r--   0        0        0      321 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/kuzushiji_mnist/__init__.py
--rw-r--r--   0        0        0     1305 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/kuzushiji_mnist/loader.py
--rw-r--r--   0        0        0      275 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/mnist/__init__.py
--rw-r--r--   0        0        0     1215 2023-06-12 01:33:39.285052 mnisq-0.1.0/mnisq/mnist/loader.py
--rw-r--r--   0        0        0     1118 2023-06-12 01:34:25.125044 mnisq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1669 1970-01-01 00:00:00.000000 mnisq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    20139 2023-06-21 11:28:43.737989 mnisq-0.2.0/LICENSE
+-rw-r--r--   0        0        0      947 2023-06-24 00:12:47.316543 mnisq-0.2.0/README.md
+-rw-r--r--   0        0        0       95 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/config/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/fashion_mnist/__init__.py
+-rw-r--r--   0        0        0     1269 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/fashion_mnist/loader.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/__init__.py
+-rw-r--r--   0        0        0      141 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/dataset/__init__.py
+-rw-r--r--   0        0        0     4927 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/dataset/dataset.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/__init__.py
+-rw-r--r--   0        0        0    12506 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE.cpp
+-rw-r--r--   0        0        0     1196 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE_from_program.py
+-rw-r--r--   0        0        0     4572 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE_from_python.py
+-rw-r--r--   0        0        0       86 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/aqce/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/cifar_10/__init__.py
+-rw-r--r--   0        0        0     2021 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/cifar_10/downloader.py
+-rw-r--r--   0        0        0      564 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/cifar_10/gray_scale.py
+-rw-r--r--   0        0        0     3095 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/cifar_10/main.py
+-rw-r--r--   0        0        0     3585 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/mnist_like/Source.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/mnist_like/__init__.py
+-rw-r--r--   0        0        0       43 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/mnist_like/downloader/__init__.py
+-rw-r--r--   0        0        0     4171 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/generator/mnist_like/downloader/mnist.py
+-rw-r--r--   0        0        0    13558 2023-06-25 04:35:25.520583 mnisq-0.2.0/mnisq/internal/generator/mnist_like/qasm_converter.py
+-rw-r--r--   0        0        0        0 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/loader/__init__.py
+-rw-r--r--   0        0        0       83 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/internal/loader/mnist_like/__init__.py
+-rw-r--r--   0        0        0     1504 2023-06-25 08:15:19.972636 mnisq-0.2.0/mnisq/internal/loader/mnist_like/load.py
+-rw-r--r--   0        0        0      321 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/kuzushiji_mnist/__init__.py
+-rw-r--r--   0        0        0     1305 2023-06-21 11:28:43.757989 mnisq-0.2.0/mnisq/kuzushiji_mnist/loader.py
+-rw-r--r--   0        0        0      305 2023-06-24 00:10:08.780107 mnisq-0.2.0/mnisq/mnist/__init__.py
+-rw-r--r--   0        0        0     1339 2023-06-24 00:17:21.882698 mnisq-0.2.0/mnisq/mnist/loader.py
+-rw-r--r--   0        0        0     1118 2023-06-24 07:27:07.324305 mnisq-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 mnisq-0.2.0/PKG-INFO
```

### Comparing `mnisq-0.1.0/LICENSE` & `mnisq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/fashion_mnist/loader.py` & `mnisq-0.2.0/mnisq/fashion_mnist/loader.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/dataset/dataset.py` & `mnisq-0.2.0/mnisq/internal/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE.cpp` & `mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE.cpp`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE_from_program.py` & `mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE_from_program.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/aqce/AQCE_from_python.py` & `mnisq-0.2.0/mnisq/internal/generator/aqce/AQCE_from_python.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/cifar_10/downloader.py` & `mnisq-0.2.0/mnisq/internal/generator/cifar_10/downloader.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/cifar_10/gray_scale.py` & `mnisq-0.2.0/mnisq/internal/generator/cifar_10/gray_scale.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/cifar_10/main.py` & `mnisq-0.2.0/mnisq/internal/generator/cifar_10/main.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/mnist_like/Source.py` & `mnisq-0.2.0/mnisq/internal/generator/mnist_like/Source.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/mnist_like/downloader/mnist.py` & `mnisq-0.2.0/mnisq/internal/generator/mnist_like/downloader/mnist.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/internal/generator/mnist_like/qasm_converter.py` & `mnisq-0.2.0/mnisq/internal/generator/mnist_like/qasm_converter.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,26 +2,35 @@
 import typing
 from cmath import phase
 from logging import NullHandler, getLogger
 from typing import List
 
 import numpy as np
 import qulacs_core
+
 from qulacs import QuantumCircuit
 from qulacs.gate import DenseMatrix, Identity
 
 logger = getLogger(__name__)
 logger.addHandler(NullHandler())
 
+FIXED_POINT_PATTERN = r"[+-]?\d+(?:\.\d*)?|\.\d+"
+FLOATING_POINT_PATTERN = r"[eE][-+]?\d+"
+GENERAL_NUMBER_PATTERN = (
+    rf"(?:{FIXED_POINT_PATTERN})(?:{FLOATING_POINT_PATTERN})?"  # noqa
+)
+
 
 def convert_qulacs_circuit_to_QASM(cir: QuantumCircuit) -> typing.List[str]:
     # convert qulacs Quantum Circuit to QASM List[str].
     # This method uses extended QASM for serializing Density Matrix.
     # This serializes almost all gate type defined in qelib1.inc,
     # except for sqrtY gate.
+    # CAVEAT: this function currently does not accept leading zero notation like
+    # .5, .832 etc.
 
     out_strs = [
         "OPENQASM 2.0;",
         'include "qelib1.inc";',
         f"qreg q[{cir.get_qubit_count()}];",
     ]
 
@@ -32,14 +41,16 @@
 
         if it.get_name() == "CNOT":
             out_strs.append(f"cx q[{clis[0]}],q[{tlis[0]}];")
         elif it.get_name() == "CZ":
             out_strs.append(f"cz q[{clis[0]}],q[{tlis[0]}];")
         elif it.get_name() == "SWAP":
             out_strs.append(f"swap q[{tlis[0]}],q[{tlis[1]}];")
+        elif it.get_name() == "FusedSWAP":
+            print("# FusedSWAP is not supported yet")
         elif it.get_name() == "Identity" or it.get_name() == "I":
             out_strs.append(f"id q[{tlis[0]}];")
         elif it.get_name() == "X":
             out_strs.append(f"x q[{tlis[0]}];")
         elif it.get_name() == "Y":
             out_strs.append(f"y q[{tlis[0]}];")
         elif it.get_name() == "Z":
@@ -109,176 +120,182 @@
 def convert_QASM_to_qulacs_circuit(
     input_strs: typing.List[str], *, remap_remove: bool = False
 ) -> QuantumCircuit:
     # convert QASM List[str] to qulacs QuantumCircuit.
     # constraints: qreg must be named q, and creg cannot be used.
 
     mapping: List[int] = []
+
     for instr_moto in input_strs:
         # process input string for parsing instruction.
         instr = instr_moto.lower().strip().replace(" ", "").replace("\t", "")
         if instr == "":
             continue
         if instr[0:4] == "qreg":
-            matchobj = re.match(r"qregq\[(\d+)\]", instr)
+            matchobj = re.match(r"qregq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir = QuantumCircuit(int(ary[0]))
             if len(mapping) == 0:
                 mapping = list(range(int(ary[0])))
         elif instr[0:2] == "cx":
-            matchobj = re.match(r"cxq\[(\d+)\],q\[(\d+)\]", instr)
+            matchobj = re.match(r"cxq\[(\d+)\],q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_CNOT_gate(mapping[int(ary[0])], mapping[int(ary[1])])
         elif instr[0:2] == "cz":
-            matchobj = re.match(r"czq\[(\d+)\],q\[(\d+)\]", instr)
+            matchobj = re.match(r"czq\[(\d+)\],q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_CZ_gate(mapping[int(ary[0])], mapping[int(ary[1])])
         elif instr[0:4] == "swap":
-            matchobj = re.match(r"swapq\[(\d+)\],q\[(\d+)\]", instr)
+            matchobj = re.match(r"swapq\[(\d+)\],q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_SWAP_gate(mapping[int(ary[0])], mapping[int(ary[1])])
         elif instr[0:2] == "id":
-            matchobj = re.match(r"idq\[(\d+)\]", instr)
+            matchobj = re.match(r"idq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_gate(Identity(mapping[int(ary[0])]))
         elif instr[0:2] == "xq":
-            matchobj = re.match(r"xq\[(\d+)\]", instr)
+            matchobj = re.match(r"xq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_X_gate(mapping[int(ary[0])])
         elif instr[0:2] == "yq":
-            matchobj = re.match(r"yq\[(\d+)\]", instr)
+            matchobj = re.match(r"yq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_Y_gate(mapping[int(ary[0])])
         elif instr[0:2] == "zq":
-            matchobj = re.match(r"zq\[(\d+)\]", instr)
+            matchobj = re.match(r"zq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_Z_gate(mapping[int(ary[0])])
         elif instr[0:2] == "hq":
-            matchobj = re.match(r"hq\[(\d+)\]", instr)
+            matchobj = re.match(r"hq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_H_gate(mapping[int(ary[0])])
         elif instr[0:2] == "sq":
-            matchobj = re.match(r"sq\[(\d+)\]", instr)
+            matchobj = re.match(r"sq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_S_gate(mapping[int(ary[0])])
         elif instr[0:4] == "sdgq":
-            matchobj = re.match(r"sdgq\[(\d+)\]", instr)
+            matchobj = re.match(r"sdgq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_Sdag_gate(mapping[int(ary[0])])
         elif instr[0:2] == "tq":
-            matchobj = re.match(r"tq\[(\d+)\]", instr)
+            matchobj = re.match(r"tq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_T_gate(mapping[int(ary[0])])
         elif instr[0:4] == "tdgq":
-            matchobj = re.match(r"tdgq\[(\d+)\]", instr)
+            matchobj = re.match(r"tdgq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_Tdag_gate(mapping[int(ary[0])])
         elif instr[0:2] == "rx":
             matchobj = re.match(
-                r"rx\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]", instr
-            )
+                rf"rx\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RX_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:2] == "ry":
             matchobj = re.match(
-                r"ry\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]", instr
-            )
+                rf"ry\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RY_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:2] == "rz":
             matchobj = re.match(
-                r"rz\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]", instr
-            )
+                rf"rz\(({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_RZ_gate(mapping[int(ary[1])], -float(ary[0]))
         elif instr[0:1] == "p":
             matchobj = re.match(
-                r"p\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]", instr
-            )
+                rf"p\({GENERAL_NUMBER_PATTERN}\)q\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U1_gate(mapping[int(ary[1])], float(ary[0]))
         elif instr[0:2] == "u1":
             matchobj = re.match(
-                r"u1\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+\)?)q[(\d+)]", instr
-            )
+                rf"u1\(({GENERAL_NUMBER_PATTERN})\)q[(\d+)];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U1_gate(mapping[int(ary[1])], float(ary[0]))
         elif instr[0:2] == "u2":
             matchobj = re.match(
-                r"u2\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]",
+                rf"u2\(({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];",
                 instr,
             )
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U2_gate(mapping[int(ary[2])], float(ary[0]), float(ary[1]))
         elif instr[0:2] == "u3":
             matchobj = re.match(
-                r"u3\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]",
+                rf"u3\(({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];",
                 instr,
             )
+            #print("u3:", instr)
+            if matchobj is None:
+                print("matchobj is None:", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U3_gate(
-                mapping[int(ary[3])], float(ary[0]), float(ary[1]), float(ary[2])
+                mapping[int(ary[3])], float(
+                    ary[0]), float(ary[1]), float(ary[2])
             )
         elif instr[0:1] == "u":
             matchobj = re.match(
-                r"u\((\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?,"
-                + r"(\d+(\.\d*)?|\.\d+)([eE][-+]?\d+)?\)q\[(\d+)\]",
+                rf"u\(({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN}),"
+                + rf"({GENERAL_NUMBER_PATTERN})\)q\[(\d+)\];",
                 instr,
             )
+            #print("u:", instr)
+            if matchobj is None:
+                print("matchobj is None:", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_U3_gate(
-                mapping[int(ary[3])], float(ary[0]), float(ary[1]), float(ary[2])
+                mapping[int(ary[3])], float(
+                    ary[0]), float(ary[1]), float(ary[2])
             )
         elif instr[0:3] == "sxq":
-            matchobj = re.match(r"sxq\[(\d+)\]", instr)
+            matchobj = re.match(r"sxq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_sqrtX_gate(mapping[int(ary[0])])
         elif instr[0:5] == "sxdgq":
-            matchobj = re.match(r"sxdgq\[(\d+)\]", instr)
+            matchobj = re.match(r"sxdgq\[(\d+)\];", instr)
             assert matchobj is not None
             ary = matchobj.groups()
             cir.add_sqrtXdag_gate(mapping[int(ary[0])])
         elif instr[0:11] == "densematrix":
+            # Matches all matrix elements and qubit indexes
             deary = re.findall(r"[+-]?\d+(?:\.\d+)?(?:[eE][+-]?\d+)?", instr)
             target_qubit_count = int(deary[0])
             control_qubit_count = int(deary[1])
 
             gate_mat = np.zeros(
                 (2**target_qubit_count, 2**target_qubit_count), dtype="complex"
             )
             bas = 2
             for i in range(2**target_qubit_count):
                 for j in range(2**target_qubit_count):
-                    gate_mat[i][j] = float(deary[bas]) + float(deary[bas + 1]) * 1.0j
+                    gate_mat[i][j] = float(deary[bas]) + \
+                        float(deary[bas + 1]) * 1.0j
                     bas += 2
             control_values = []
             for i in range(control_qubit_count):
                 control_values.append(mapping[int(deary[bas])])
                 bas += 1
             terget_indexes = []
             for i in range(target_qubit_count):
@@ -302,9 +319,10 @@
             assert matchobj is not None
             ary = matchobj.groups()
             mapping = list(range(int(ary[0])))
         elif instr == "openqasm2.0;" or instr == 'include"qelib1.inc";':
             # related to file format, not for read.
             pass
         else:
-            raise RuntimeError(f"unknown line: {instr}")
+            # raise RuntimeError(f"unknown line: {instr}")
+            print(f"unknown line: {instr}")
     return cir
```

### Comparing `mnisq-0.1.0/mnisq/kuzushiji_mnist/loader.py` & `mnisq-0.2.0/mnisq/kuzushiji_mnist/loader.py`

 * *Files identical despite different names*

### Comparing `mnisq-0.1.0/mnisq/mnist/loader.py` & `mnisq-0.2.0/mnisq/mnist/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,7 +34,10 @@
 
 def load_mnist_train_f90() -> Dict[str, Any]:
     return load_mnist_like_dataset(URL + "/train_mnist_784_f90.zip")
 
 
 def load_mnist_train_f95() -> Dict[str, Any]:
     return load_mnist_like_dataset(URL + "/train_mnist_784_f95.zip")
+
+def load_mnist_base_test_f80() -> Dict[str, Any]:
+    return load_mnist_like_dataset(URL + "/base_test_mnist_784_f80.zip")
```

### Comparing `mnisq-0.1.0/pyproject.toml` & `mnisq-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mnisq"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["MNISQ <mnisq.osaka@gmail.com>"]
 license = "MIT"
 readme = "./README.md"
 repository = "https://github.com/FujiiLabCollaboration/MNISQ-quantum-circuit-dataset"
 homepage = "https://github.com/FujiiLabCollaboration/MNISQ-quantum-circuit-dataset"
 
@@ -13,15 +13,15 @@
 numpy = "^1.0.0"
 matplotlib = "^3.6.2"
 requests = "^2.28.1"
 types-requests = "^2.28.11.5"
 tqdm = "^4.64.1"
 typer = {extras = ["all"], version = "^0.7.0"}
 scikit-learn = "^1.2.0"
-qulacs = "^0.6.0"
+qulacs = "^0.5.4"
 opencv-python = "^4.7.0.72"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.0"
 black = "^22.3.0"
 flake8 = "^4.0.1"
 mypy = "^0.942"
```

### Comparing `mnisq-0.1.0/PKG-INFO` & `mnisq-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mnisq
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Home-page: https://github.com/FujiiLabCollaboration/MNISQ-quantum-circuit-dataset
 License: MIT
 Author: MNISQ
 Author-email: mnisq.osaka@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.0.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
-Requires-Dist: qulacs (>=0.6.0,<0.7.0)
+Requires-Dist: qulacs (>=0.5.4,<0.6.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
 Requires-Dist: types-requests (>=2.28.11.5,<3.0.0.0)
 Project-URL: Repository, https://github.com/FujiiLabCollaboration/MNISQ-quantum-circuit-dataset
 Description-Content-Type: text/markdown
@@ -33,16 +33,33 @@
 
 # MNISQ-quantum-circuit-dataset
 
 This library provides machine learning datasets as a Qulacs's QuantumCircuit instance.
 
 ## How To Install
 
+### pypi
+```
+pip install mnisq
+```
+
+### source install
 ```
 pip install git+https://github.com/FujiiLabCollaboration/MNISQ-quantum-circuit-dataset.git
 ```
 
 ## Directory structure
 - `doc/source/notebooks` provides sample usage of this library.
 - `mnisq` and `tests` contains python code.
 - `generator_scripts` contains scripts used to generate datasets.
 
+# Contributor
+This project was developed by:
+- Koki Aoyama(@kotamanegi)
+- Hayata Morisaki
+- Kouki Kawamura(@KowerKoint)
+- Toshio Mori(@forest1040)
+- Leonardo Placidi(@Gruntrexpewrus)
+- Ryuichiro Hataya
+- Kosuke Mitarai
+- Keisuke Fujii
+
```

