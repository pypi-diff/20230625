# Comparing `tmp/graphix-0.2.2.tar.gz` & `tmp/graphix-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphix-0.2.2.tar", last modified: Thu May 25 00:15:50 2023, max compression
+gzip compressed data, was "graphix-0.2.3.tar", last modified: Sun Jun 25 12:44:31 2023, max compression
```

## Comparing `graphix-0.2.2.tar` & `graphix-0.2.3.tar`

### file list

```diff
@@ -1,41 +1,37 @@
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.736813 graphix-0.2.2/
--rw-r--r--   0 ss         (501) staff       (20)    10761 2023-04-29 07:04:06.000000 graphix-0.2.2/LICENSE
--rw-r--r--   0 ss         (501) staff       (20)       94 2022-12-15 06:51:32.000000 graphix-0.2.2/MANIFEST.in
--rw-r--r--   0 ss         (501) staff       (20)     5510 2023-05-25 00:15:50.736242 graphix-0.2.2/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)     4576 2023-04-25 07:20:26.000000 graphix-0.2.2/README.md
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.669115 graphix-0.2.2/docs/
--rw-r--r--   0 ss         (501) staff       (20)      638 2022-12-02 15:18:40.000000 graphix-0.2.2/docs/Makefile
--rw-r--r--   0 ss         (501) staff       (20)      804 2022-12-02 15:18:40.000000 graphix-0.2.2/docs/make.bat
--rw-r--r--   0 ss         (501) staff       (20)     1294 2023-01-09 01:14:11.000000 graphix-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.709185 graphix-0.2.2/graphix/
--rw-r--r--   0 ss         (501) staff       (20)      247 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/__init__.py
--rw-r--r--   0 ss         (501) staff       (20)     7451 2023-01-14 13:01:46.000000 graphix-0.2.2/graphix/clifford.py
--rw-r--r--   0 ss         (501) staff       (20)     4173 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/generator.py
--rw-r--r--   0 ss         (501) staff       (20)    13035 2023-04-07 01:21:59.000000 graphix-0.2.2/graphix/gflow.py
--rw-r--r--   0 ss         (501) staff       (20)    13678 2023-01-14 13:01:46.000000 graphix-0.2.2/graphix/graphsim.py
--rw-r--r--   0 ss         (501) staff       (20)     2463 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/ops.py
--rw-r--r--   0 ss         (501) staff       (20)    64919 2023-05-25 00:12:26.000000 graphix-0.2.2/graphix/pattern.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.715511 graphix-0.2.2/graphix/sim/
--rw-r--r--   0 ss         (501) staff       (20)        0 2022-12-12 11:17:35.000000 graphix-0.2.2/graphix/sim/__init__.py
--rw-r--r--   0 ss         (501) staff       (20)    11313 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/sim/statevec.py
--rw-r--r--   0 ss         (501) staff       (20)    26198 2023-05-25 00:12:26.000000 graphix-0.2.2/graphix/sim/tensornet.py
--rw-r--r--   0 ss         (501) staff       (20)     2269 2023-03-01 11:13:38.000000 graphix-0.2.2/graphix/simulator.py
--rw-r--r--   0 ss         (501) staff       (20)    37241 2023-03-16 06:55:32.000000 graphix-0.2.2/graphix/transpiler.py
--rw-r--r--   0 ss         (501) staff       (20)       22 2023-05-25 00:12:43.000000 graphix-0.2.2/graphix/version.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.712842 graphix-0.2.2/graphix.egg-info/
--rw-r--r--   0 ss         (501) staff       (20)     5510 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/PKG-INFO
--rw-r--r--   0 ss         (501) staff       (20)      681 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/SOURCES.txt
--rw-r--r--   0 ss         (501) staff       (20)        1 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/dependency_links.txt
--rw-r--r--   0 ss         (501) staff       (20)       85 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/requires.txt
--rw-r--r--   0 ss         (501) staff       (20)        8 2023-05-25 00:15:50.000000 graphix-0.2.2/graphix.egg-info/top_level.txt
--rw-r--r--   0 ss         (501) staff       (20)       81 2022-12-15 06:51:32.000000 graphix-0.2.2/pyproject.toml
--rw-r--r--   0 ss         (501) staff       (20)       38 2023-05-25 00:15:50.737027 graphix-0.2.2/setup.cfg
--rw-r--r--   0 ss         (501) staff       (20)     1488 2023-05-16 06:15:33.000000 graphix-0.2.2/setup.py
-drwxr-xr-x   0 ss         (501) staff       (20)        0 2023-05-25 00:15:50.734735 graphix-0.2.2/tests/
--rw-r--r--   0 ss         (501) staff       (20)     2904 2023-01-14 13:01:46.000000 graphix-0.2.2/tests/test_clifford.py
--rw-r--r--   0 ss         (501) staff       (20)     2986 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_generator.py
--rw-r--r--   0 ss         (501) staff       (20)     2479 2023-04-07 01:21:59.000000 graphix-0.2.2/tests/test_gflow.py
--rw-r--r--   0 ss         (501) staff       (20)     3974 2022-12-15 11:43:28.000000 graphix-0.2.2/tests/test_graphsim.py
--rw-r--r--   0 ss         (501) staff       (20)    15790 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_pattern.py
--rw-r--r--   0 ss         (501) staff       (20)    15778 2023-05-15 04:40:18.000000 graphix-0.2.2/tests/test_tnsim.py
--rw-r--r--   0 ss         (501) staff       (20)     5102 2023-01-14 13:01:46.000000 graphix-0.2.2/tests/test_transpiler.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.013814 graphix-0.2.3/
+-rw-r--r--   0 sunami     (501) staff       (20)    10761 2023-06-25 12:12:17.000000 graphix-0.2.3/LICENSE
+-rw-r--r--   0 sunami     (501) staff       (20)       94 2023-06-25 12:12:17.000000 graphix-0.2.3/MANIFEST.in
+-rw-r--r--   0 sunami     (501) staff       (20)     5510 2023-06-25 12:44:31.013613 graphix-0.2.3/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)     4576 2023-06-25 12:12:17.000000 graphix-0.2.3/README.md
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.009542 graphix-0.2.3/graphix/
+-rw-r--r--   0 sunami     (501) staff       (20)      247 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)     7451 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     4173 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    13035 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)    14059 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2463 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/ops.py
+-rw-r--r--   0 sunami     (501) staff       (20)    68268 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/pattern.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.010939 graphix-0.2.3/graphix/sim/
+-rw-r--r--   0 sunami     (501) staff       (20)        0 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/sim/__init__.py
+-rw-r--r--   0 sunami     (501) staff       (20)    11396 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/sim/statevec.py
+-rw-r--r--   0 sunami     (501) staff       (20)    26314 2023-06-25 12:16:17.000000 graphix-0.2.3/graphix/sim/tensornet.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2269 2023-06-25 12:41:22.000000 graphix-0.2.3/graphix/simulator.py
+-rw-r--r--   0 sunami     (501) staff       (20)    37241 2023-06-25 12:12:17.000000 graphix-0.2.3/graphix/transpiler.py
+-rw-r--r--   0 sunami     (501) staff       (20)       22 2023-06-25 12:41:33.000000 graphix-0.2.3/graphix/version.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.010354 graphix-0.2.3/graphix.egg-info/
+-rw-r--r--   0 sunami     (501) staff       (20)     5510 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/PKG-INFO
+-rw-r--r--   0 sunami     (501) staff       (20)      631 2023-06-25 12:44:31.000000 graphix-0.2.3/graphix.egg-info/SOURCES.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        1 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/dependency_links.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       85 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/requires.txt
+-rw-r--r--   0 sunami     (501) staff       (20)        8 2023-06-25 12:44:30.000000 graphix-0.2.3/graphix.egg-info/top_level.txt
+-rw-r--r--   0 sunami     (501) staff       (20)       81 2023-06-25 12:12:17.000000 graphix-0.2.3/pyproject.toml
+-rw-r--r--   0 sunami     (501) staff       (20)       38 2023-06-25 12:44:31.013918 graphix-0.2.3/setup.cfg
+-rw-r--r--   0 sunami     (501) staff       (20)     1488 2023-06-25 12:12:17.000000 graphix-0.2.3/setup.py
+drwxr-xr-x   0 sunami     (501) staff       (20)        0 2023-06-25 12:44:31.013250 graphix-0.2.3/tests/
+-rw-r--r--   0 sunami     (501) staff       (20)     2904 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_clifford.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2986 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_generator.py
+-rw-r--r--   0 sunami     (501) staff       (20)     2479 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_gflow.py
+-rw-r--r--   0 sunami     (501) staff       (20)     3974 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_graphsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)    15447 2023-06-25 12:16:17.000000 graphix-0.2.3/tests/test_pattern.py
+-rw-r--r--   0 sunami     (501) staff       (20)    15771 2023-06-25 12:16:17.000000 graphix-0.2.3/tests/test_tnsim.py
+-rw-r--r--   0 sunami     (501) staff       (20)     5102 2023-06-25 12:12:17.000000 graphix-0.2.3/tests/test_transpiler.py
```

### Comparing `graphix-0.2.2/LICENSE` & `graphix-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/PKG-INFO` & `graphix-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.2
+Version: 0.2.3
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
```

### Comparing `graphix-0.2.2/README.md` & `graphix-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/clifford.py` & `graphix-0.2.3/graphix/clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/generator.py` & `graphix-0.2.3/graphix/generator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/gflow.py` & `graphix-0.2.3/graphix/gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/graphsim.py` & `graphix-0.2.3/graphix/graphsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         ----------
         node : int
             graph node to apply S gate
         """
         if self.nodes[node]["hollow"]:
             if self.nodes[node]["loop"]:
                 self.flip_fill(node)
-                self.nodes["loop"] = False
+                self.nodes[node]["loop"] = False
                 self.local_complement(node)
                 for i in self.neighbors(node):
                     self.advance(i)
             else:
                 self.local_complement(node)
                 for i in self.neighbors(node):
                     self.advance(i)
@@ -234,31 +234,32 @@
         Parameters
         ----------
         node1, node2 : int
             connected graph nodes to apply rule E2
         """
         assert (node1, node2) in list(self.edges) or (node2, node1) in list(self.edges)
         assert not self.nodes[node1]["loop"] and not self.nodes[node2]["loop"]
+        sg1 = self.nodes[node1]["sign"]
+        sg2 = self.nodes[node2]["sign"]
         self.flip_fill(node1)
         self.flip_fill(node2)
         # local complement along edge between node1, node2
         self.local_complement(node1)
         self.local_complement(node2)
         self.local_complement(node1)
         for i in iter(set(self.neighbors(node1)) & set(self.neighbors(node2))):
             self.flip_sign(i)
-        if self.nodes[node1]["sign"] != self.nodes[node2]["sign"]:
-            if self.nodes[node1]["sign"]:
-                self.flip_sign(node1)
-                for i in self.neighbors(node1):
-                    self.flip_sign(i)
-            elif self.nodes[node2]["sign"]:
-                self.flip_sign(node2)
-                for i in self.neighbors(node2):
-                    self.flip_sign(i)
+        if sg1:
+            self.flip_sign(node1)
+            for i in self.neighbors(node1):
+                self.flip_sign(i)
+        if sg2:
+            self.flip_sign(node2)
+            for i in self.neighbors(node2):
+                self.flip_sign(i)
 
     def local_complement(self, node):
         """Perform local complementation of a graph
 
         Parameters
         ----------
         node : int
@@ -316,16 +317,27 @@
         Parameters
         ----------
         node : int
             qubit index to be measured
         choice : int, 0 or 1
             choice of measurement outcome. observe (-1)^choice
         """
-        self.h(node)
-        return self.measure_z(node, choice=choice)
+        # check if isolated
+        if len(list(self.neighbors(node))) == 0:
+            if self.nodes[node]["hollow"] or self.nodes[node]["loop"]:
+                choice_ = choice
+            elif self.nodes[node]["sign"]:  # isolated and state is |->
+                choice_ = 1
+            else:  # isolated and state is |+>
+                choice_ = 0
+            self.remove_node(node)
+            return choice_
+        else:
+            self.h(node)
+            return self.measure_z(node, choice=choice)
 
     def measure_y(self, node, choice=0):
         """perform measurement in Y basis
         According to original paper, we realise Y measurement by
         applying S,Z and H gate to the measured node before Z measurement.
 
         Parameters
```

### Comparing `graphix-0.2.2/graphix/ops.py` & `graphix-0.2.3/graphix/ops.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/pattern.py` & `graphix-0.2.3/graphix/pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,15 @@
 ref: V. Danos, E. Kashefi and P. Panangaden. J. ACM 54.2 8 (2007)
 """
 import numpy as np
 import networkx as nx
 from graphix.simulator import PatternSimulator
 from graphix.graphsim import GraphState
 from graphix.gflow import flow, gflow, get_layers
-from graphix.clifford import (
-    CLIFFORD_CONJ,
-    CLIFFORD_TO_QASM3,
-    CLIFFORD_MUL,
-    CLIFFORD_MEASURE,
-)
+from graphix.clifford import CLIFFORD_CONJ, CLIFFORD_TO_QASM3, CLIFFORD_MEASURE
 from copy import deepcopy
 
 
 class Pattern:
     """
     MBQC pattern class
 
@@ -53,14 +48,15 @@
         """
         # number of input qubits
         self.width = width
         self.seq = [["N", i] for i in range(width)]  # where command sequence is stored
         self.results = {}  # measurement results from the graph state simulator
         self.output_nodes = output_nodes  # output nodes
         self.Nnode = width  # total number of nodes in the graph state
+        self._pauli_preprocessed = False  # flag for `measure_pauli` preprocessing completion
 
     def add(self, cmd):
         """add command to the end of the pattern.
         an MBQC command is specified by a list of [type, node, attr], where
 
             type : 'N', 'M', 'E', 'X', 'Z', 'S' or 'C'
             nodes : int for 'N', 'M', 'X', 'Z', 'S', 'C' commands
@@ -1048,15 +1044,17 @@
         """Optimize the pattern to minimize the max_space property of
         the pattern i.e. the optimized pattern has significantly
         reduced space requirement (memory space for classical simulation,
         and maximum simultaneously prepared qubits for quantum hardwares).
         """
         if not self.is_standard():
             self.standardize()
-        meas_order = self.get_measurement_order_from_flow()
+        meas_order = None
+        if not self._pauli_preprocessed:
+            meas_order = self.get_measurement_order_from_flow()
         if meas_order is None:
             meas_order = self._measurement_order_space()
         self._reorder_pattern(self.sort_measurement_commands(meas_order))
 
     def _reorder_pattern(self, meas_commands):
         """internal method to reorder the command sequence
 
@@ -1083,14 +1081,19 @@
             measured.append(node)
 
         # add isolated nodes
         for cmd in self.seq:
             if cmd[0] == "N":
                 if not cmd[1] in prepared:
                     new.append(["N", cmd[1]])
+        for cmd in self.seq:
+            if cmd[0] == "E":
+                if cmd[1][0] in self.output_nodes:
+                    if cmd[1][1] in self.output_nodes:
+                        new.append(cmd)
 
         # add Clifford nodes
         for cmd in self.seq:
             if cmd[0] == "C":
                 new.append(cmd)
 
         # add corrections
@@ -1542,15 +1545,15 @@
 
         Returns
         -------
         pattern : Pattern
             standardized global pattern
         """
         assert self.is_standard()
-        pattern = Pattern(output_nodes=self.output_nodes)
+        pattern = Pattern(output_nodes=self.output_nodes, width=len(self.output_nodes))
         Nseq = [["N", i] for i in self.nodes.keys()]
         Eseq = []
         Mseq = []
         Xseq = []
         Zseq = []
         Cseq = []
         for node_index in self.morder + self.output_nodes:
@@ -1622,84 +1625,98 @@
 
 
     .. seealso:: :class:`graphix.graphsim.GraphState`
     """
     if not pattern.is_standard():
         pattern.standardize()
     nodes, edges = pattern.get_graph()
-    vop_init = pattern.get_vops(conj=True)
-    graph_state = GraphState(nodes=nodes, edges=edges)
+    vop_init = pattern.get_vops(conj=False)
+    graph_state = GraphState(nodes=nodes, edges=edges, vops=vop_init)
     results = {}
     to_measure, non_pauli_meas = pauli_nodes(pattern)
     for cmd in to_measure:
-        # extract signals for adaptive angle. Assumes XY plane measurements
-        if np.mod(cmd[3], 2) in [0, 1]:  # \pm X Pauli measurement
+        # extract signals for adaptive angle.
+        if cmd[1] in ["+X", "-X"]:
             s_signal = 0  # X meaurement is not affected by s_signal
-            t_signal = np.sum([results[j] for j in cmd[5]])
-        elif np.mod(cmd[3], 2) in [0.5, 1.5]:  # \pm Y Pauli measurement
-            s_signal = np.sum([results[j] for j in cmd[4]])
-            t_signal = np.sum([results[j] for j in cmd[5]])
-        angle = cmd[3] * (-1) ** s_signal + t_signal
-        if np.mod(angle, 2) == 0:  # +x measurement
-            results[cmd[1]] = graph_state.measure_x(cmd[1], choice=0)
-        elif np.mod(angle, 2) == 1:  # -x measurement
-            results[cmd[1]] = 1 - graph_state.measure_x(cmd[1], choice=1)
-        elif np.mod(angle, 2) == 0.5:  # +y measurement
-            results[cmd[1]] = graph_state.measure_y(cmd[1], choice=0)
-        elif np.mod(angle, 2) == 1.5:  # -y measurement
-            results[cmd[1]] = 1 - graph_state.measure_y(cmd[1], choice=1)
+            t_signal = np.sum([results[j] for j in cmd[0][5]])
+        elif cmd[1] in ["+Y", "-Y"]:
+            s_signal = np.sum([results[j] for j in cmd[0][4]])
+            t_signal = np.sum([results[j] for j in cmd[0][5]])
+        elif cmd[1] in ["+Z", "-Z"]:
+            s_signal = np.sum([results[j] for j in cmd[0][4]])
+            t_signal = 0  # Z meaurement is not affected by t_signal
+        else:
+            raise ValueError("unknown Pauli measurement basis", cmd[1])
+
+        if int(s_signal % 2) == 1:  # equivalent to X byproduct
+            graph_state.h(cmd[0][1])
+            graph_state.z(cmd[0][1])
+            graph_state.h(cmd[0][1])
+        if int(t_signal % 2) == 1:  # equivalent to Z byproduct
+            graph_state.z(cmd[0][1])
+
+        if cmd[1] == "+X":
+            results[cmd[0][1]] = graph_state.measure_x(cmd[0][1], choice=0)
+        elif cmd[1] == "-X":
+            results[cmd[0][1]] = 1 - graph_state.measure_x(cmd[0][1], choice=1)
+        elif cmd[1] == "+Y":
+            results[cmd[0][1]] = graph_state.measure_y(cmd[0][1], choice=0)
+        elif cmd[1] == "-Y":
+            results[cmd[0][1]] = 1 - graph_state.measure_y(cmd[0][1], choice=1)
+        elif cmd[1] == "+Z":
+            results[cmd[0][1]] = graph_state.measure_z(cmd[0][1], choice=0)
+        elif cmd[1] == "-Z":
+            results[cmd[0][1]] = 1 - graph_state.measure_z(cmd[0][1], choice=1)
 
     # measure (remove) isolated nodes. if they aren't Pauli measurements,
     # measuring one of the results with probability of 1 should not occur as was possible above for Pauli measurements,
     # which means we can just choose s=0. We should not remove output nodes even if isolated.
     isolates = list(nx.isolates(graph_state))
-    for cmd in non_pauli_meas:
-        if (cmd[1] in isolates) and (cmd[1] not in pattern.output_nodes):
-            graph_state.remove_node(cmd[1])
-            results[cmd[1]] = 0
+    for node in non_pauli_meas:
+        if (node in isolates) and (node not in pattern.output_nodes):
+            graph_state.remove_node(node)
+            results[node] = 0
 
     # update command sequence
     vops = graph_state.get_vops()
     new_seq = []
     for index in iter(graph_state.nodes):
         new_seq.append(["N", index])
     for edge in iter(graph_state.edges):
         new_seq.append(["E", edge])
     for cmd in pattern.seq:
         if cmd[0] == "M":
             if cmd[1] in list(graph_state.nodes):
                 cmd_new = deepcopy(cmd)
-                new_clifford_ = CLIFFORD_CONJ[vops[cmd[1]]]
-                if cmd[1] in vop_init.keys():
-                    new_clifford_ = CLIFFORD_MUL[vop_init[cmd[1]], new_clifford_]
+                new_clifford_ = vops[cmd[1]]
                 if len(cmd_new) == 7:
                     cmd_new[6] = new_clifford_
                 else:
                     cmd_new.append(new_clifford_)
                 new_seq.append(cmd_new)
     for index in pattern.output_nodes:
         new_clifford_ = vops[index]
-        if index in vop_init.keys():
-            new_clifford_ = CLIFFORD_MUL[vop_init[index], new_clifford_]
         if new_clifford_ != 0:
             new_seq.append(["C", index, new_clifford_])
     for cmd in pattern.seq:
         if cmd[0] == "X" or cmd[0] == "Z":
             new_seq.append(cmd)
 
     if copy:
         pat = deepcopy(pattern)
         pat.seq = new_seq
         pat.Nnode = len(graph_state.nodes)
         pat.results = results
+        pat._pauli_preprocessed = True
         return pat
     else:
         pattern.seq = new_seq
         pattern.Nnode = len(graph_state.nodes)
         pattern.results = results
+        pattern._pauli_preprocessed = True
 
 
 def pauli_nodes(pattern):
     """returns the list of measurement commands that are in Pauli bases
     and that are not dependent on any non-Pauli measurements
 
     Parameters
@@ -1714,37 +1731,117 @@
     if not pattern.is_standard():
         pattern.standardize()
     m_commands = pattern.get_measurement_commands()
     pauli_node = []
     # Nodes that are non-Pauli measured, or pauli measured but depends on pauli measurement
     non_pauli_node = []
     for cmd in m_commands:
-        if cmd[2] == "XY":
-            if cmd[3] in [-1, 0, 1]:  # Not affected by t dependency
-                t_cond = np.any(np.isin(cmd[5], np.array(non_pauli_node, dtype=object)))
+        pm = is_pauli_measurement(cmd, ignore_vop=True)
+        if pm is not None:  # Pauli measurement
+            if pm in ["+X", "-X"]:
+                t_cond = np.any(np.isin(cmd[5], np.array(non_pauli_node)))
                 if t_cond:  # cmd depend on non-Pauli measurement
-                    non_pauli_node.append(cmd)
-                else:  # cmd do not depend on non-Pauli measurements
-                    # note: s_signal is irrelevant for X measurements
-                    # because change of sign will do nothing
-                    pauli_node.append(cmd)
-            elif cmd[3] in [-0.5, 0.5]:  # Affected by t dependency
-                s_cond = np.any(np.isin(cmd[4], np.array(non_pauli_node, dtype=object)))
-                t_cond = np.any(np.isin(cmd[5], np.array(non_pauli_node, dtype=object)))
-                if s_cond or t_cond:  # cmd depend on non-pauli measurement
-                    non_pauli_node.append(cmd)
+                    non_pauli_node.append(cmd[1])
                 else:
-                    pauli_node.append(cmd)
+                    pauli_node.append((cmd, pm))
+            elif pm in ["+Y", "-Y"]:
+                s_cond = np.any(np.isin(cmd[4], np.array(non_pauli_node)))
+                t_cond = np.any(np.isin(cmd[5], np.array(non_pauli_node)))
+                if t_cond or s_cond:  # cmd depend on non-Pauli measurement
+                    non_pauli_node.append(cmd[1])
+                else:
+                    pauli_node.append((cmd, pm))
+            elif pm in ["+Z", "-Z"]:
+                s_cond = np.any(np.isin(cmd[4], np.array(non_pauli_node)))
+                if s_cond:  # cmd depend on non-Pauli measurement
+                    non_pauli_node.append(cmd[1])
+                else:
+                    pauli_node.append((cmd, pm))
             else:
-                non_pauli_node.append(cmd)
+                raise ValueError("Unknown Pauli measurement basis")
         else:
-            raise NotImplementedError("YZ and XZ plane measurements not considered for pauli_node")
+            non_pauli_node.append(cmd[1])
     return pauli_node, non_pauli_node
 
 
+def is_pauli_measurement(cmd, ignore_vop=True):
+    """Determines whether or not the measurement command is a Pauli measurement,
+    and if so returns the measurement basis.
+
+    Parameters
+    ----------
+    cmd : list
+        measurement command. list containing the information of the measurement,
+        "M", node index, measurement plane, angle (in unit of pi), s-signal, t-signal, clifford index.
+
+        e.g. `['M', 2, 'XY', 0.25, [], [], 6]`
+        for measurement of node 2, in 4/pi angle in XY plane, with local Clifford index 6 (Hadamard).
+    ignore_vop : bool
+        whether or not to ignore local Clifford to detemrine the measurement basis.
+
+    Returns
+    -------
+        str, one of '+X', '-X', '+Y', '-Y', '+Z', '-Z'
+        if the measurement is not in Pauli basis, returns None.
+    """
+    assert cmd[0] == "M"
+    basis_str = [("+X", "-X"), ("+Y", "-Y"), ("+Z", "-Z")]
+    if len(cmd) == 7:
+        vop = cmd[6]
+    else:
+        vop = 0
+    # first item: 0, 1 or 2. correspond to choice of X, Y and Z
+    # second item: 0 or 1. correspond to sign (+, -)
+    basis_index = (0, 0)
+    if np.mod(cmd[3], 2) == 0:
+        if cmd[2] == "XY":
+            basis_index = (0, 0)
+        elif cmd[2] == "YZ":
+            basis_index = (1, 0)
+        elif cmd[2] == "XZ":
+            basis_index = (0, 0)
+        else:
+            raise ValueError("Unknown measurement plane")
+    elif np.mod(cmd[3], 2) == 1:
+        if cmd[2] == "XY":
+            basis_index = (0, 1)
+        elif cmd[2] == "YZ":
+            basis_index = (1, 1)
+        elif cmd[2] == "XZ":
+            basis_index = (0, 1)
+        else:
+            raise ValueError("Unknown measurement plane")
+    elif np.mod(cmd[3], 2) == 0.5:
+        if cmd[2] == "XY":
+            basis_index = (1, 0)
+        elif cmd[2] == "YZ":
+            basis_index = (2, 0)
+        elif cmd[2] == "XZ":
+            basis_index = (2, 0)
+        else:
+            raise ValueError("Unknown measurement plane")
+    elif np.mod(cmd[3], 2) == 1.5:
+        if cmd[2] == "XY":
+            basis_index = (1, 1)
+        elif cmd[2] == "YZ":
+            basis_index = (2, 1)
+        elif cmd[2] == "XZ":
+            basis_index = (2, 1)
+        else:
+            raise ValueError("Unknown measurement plane")
+    else:
+        return None
+    if not ignore_vop:
+        basis_index = (
+            CLIFFORD_MEASURE[vop][basis_index[0]][0],
+            int(np.abs(basis_index[1] - CLIFFORD_MEASURE[vop][basis_index[0]][1])),
+        )
+    return basis_str[basis_index[0]][basis_index[1]]
+
+
 def cmd_to_qasm3(cmd):
     """Converts a command in the pattern into OpenQASM 3.0 statement.
 
     Parameter
     ---------
     cmd : list
         command [type:str, node:int, attr]
```

### Comparing `graphix-0.2.2/graphix/sim/statevec.py` & `graphix-0.2.3/graphix/sim/statevec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 from graphix.ops import Ops
-from graphix.clifford import CLIFFORD_MEASURE, CLIFFORD
+from graphix.clifford import CLIFFORD_CONJ, CLIFFORD, CLIFFORD_MUL
 from copy import deepcopy
 from scipy.linalg import norm
 
 
 class StatevectorBackend:
     """MBQC simulator with statevector method."""
 
@@ -82,19 +82,24 @@
         # choose the measurement result randomly
         result = np.random.choice([0, 1])
         self.results[cmd[1]] = result
 
         # extract signals for adaptive angle
         s_signal = np.sum([self.results[j] for j in cmd[4]])
         t_signal = np.sum([self.results[j] for j in cmd[5]])
-        angle = cmd[3] * np.pi * (-1) ** s_signal + np.pi * t_signal
+        angle = cmd[3] * np.pi
         if len(cmd) == 7:
-            m_op = meas_op(angle, vop=cmd[6], plane=cmd[2], choice=result)
+            vop = cmd[6]
         else:
-            m_op = meas_op(angle, plane=cmd[2], choice=result)
+            vop = 0
+        if int(s_signal % 2) == 1:
+            vop = CLIFFORD_MUL[1, vop]
+        if int(t_signal % 2) == 1:
+            vop = CLIFFORD_MUL[3, vop]
+        m_op = meas_op(angle, vop=vop, plane=cmd[2], choice=result)
         loc = self.node_index.index(cmd[1])
         self.state.evolve_single(m_op, loc)
 
         self.to_trace.append(cmd[1])
         self.to_trace_loc.append(loc)
 
     def correct_byproduct(self, cmd):
@@ -174,17 +179,16 @@
         vec = (np.cos(angle), np.sin(angle), 0)
     elif plane == "YZ":
         vec = (0, np.cos(angle), np.sin(angle))
     elif plane == "XZ":
         vec = (np.cos(angle), 0, np.sin(angle))
     op_mat = np.eye(2, dtype=np.complex128) / 2
     for i in range(3):
-        op_mat += (
-            (-1) ** (choice + CLIFFORD_MEASURE[vop][i][1]) * vec[CLIFFORD_MEASURE[vop][i][0]] * CLIFFORD[i + 1] / 2
-        )
+        op_mat += (-1) ** (choice) * vec[i] * CLIFFORD[i + 1] / 2
+    op_mat = CLIFFORD[CLIFFORD_CONJ[vop]] @ op_mat @ CLIFFORD[vop]
     return op_mat
 
 
 CZ_TENSOR = np.array(
     [[[[1, 0], [0, 0]], [[0, 1], [0, 0]]], [[[0, 0], [1, 0]], [[0, 0], [0, -1]]]],
     dtype=np.complex128,
 )
```

### Comparing `graphix-0.2.2/graphix/sim/tensornet.py` & `graphix-0.2.3/graphix/sim/tensornet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import quimb.tensor as qtn
 from quimb.tensor import Tensor, TensorNetwork
-from graphix.clifford import CLIFFORD
+from graphix.clifford import CLIFFORD, CLIFFORD_MUL, CLIFFORD_CONJ
 from graphix.ops import States, Ops
 import string
 from copy import deepcopy
 
 
 class TensorNetworkBackend:
     """Tensor Network Simulator for MBQC
@@ -135,19 +135,24 @@
             result = np.random.choice([0, 1])
             self.results[cmd[1]] = result
             buffer = 2**0.5
 
         # extract signals for adaptive angle
         s_signal = np.sum([self.results[j] for j in cmd[4]])
         t_signal = np.sum([self.results[j] for j in cmd[5]])
-        angle = cmd[3] * np.pi * (-1) ** s_signal + np.pi * t_signal
+        angle = cmd[3] * np.pi
         if len(cmd) == 7:
-            proj_vec = proj_basis(angle, vop=cmd[6], plane=cmd[2], choice=result)
+            vop = cmd[6]
         else:
-            proj_vec = proj_basis(angle, vop=0, plane=cmd[2], choice=result)
+            vop = 0
+        if int(s_signal % 2) == 1:
+            vop = CLIFFORD_MUL[1, vop]
+        if int(t_signal % 2) == 1:
+            vop = CLIFFORD_MUL[3, vop]
+        proj_vec = proj_basis(angle, vop=vop, plane=cmd[2], choice=result)
 
         # buffer is necessary for maintaing the norm invariant
         proj_vec = proj_vec * buffer
         self.state.measure_single(cmd[1], basis=proj_vec)
 
     def correct_byproduct(self, cmd):
         """Perform byproduct correction.
@@ -702,18 +707,18 @@
     if plane == "XY":
         vec = States.vec[0 + choice]
         rotU = Ops.Rz(angle)
     elif plane == "YZ":
         vec = States.vec[4 + choice]
         rotU = Ops.Rx(angle)
     elif plane == "XZ":
-        vec = States.vec[2 + choice]
-        rotU = Ops.Ry(angle)
+        vec = States.vec[0 + choice]
+        rotU = Ops.Ry(-angle)
     vec = np.matmul(rotU, vec)
-    vec = np.matmul(CLIFFORD[vop], vec)
+    vec = np.matmul(CLIFFORD[CLIFFORD_CONJ[vop]], vec)
     return vec
 
 
 def outer_product(vectors):
     """outer product of the given vectors
 
     Parameters
```

### Comparing `graphix-0.2.2/graphix/simulator.py` & `graphix-0.2.3/graphix/simulator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix/transpiler.py` & `graphix-0.2.3/graphix/transpiler.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/graphix.egg-info/PKG-INFO` & `graphix-0.2.3/graphix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphix
-Version: 0.2.2
+Version: 0.2.3
 Summary: Optimize and simulate measurement-based quantum computation
 Home-page: https://graphix.readthedocs.io
 Author: Shinichi Sunami
 Author-email: shinichi.sunami@gmail.com
 Maintainer: Shinichi Sunami
 Maintainer-email: shinichi.sunami@gmail.com
 License: Apache License 2.0
```

### Comparing `graphix-0.2.2/graphix.egg-info/SOURCES.txt` & `graphix-0.2.3/graphix.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-docs/Makefile
-docs/make.bat
-docs/requirements.txt
 graphix/__init__.py
 graphix/clifford.py
 graphix/generator.py
 graphix/gflow.py
 graphix/graphsim.py
 graphix/ops.py
 graphix/pattern.py
```

### Comparing `graphix-0.2.2/setup.py` & `graphix-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/tests/test_clifford.py` & `graphix-0.2.3/tests/test_clifford.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/tests/test_generator.py` & `graphix-0.2.3/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/tests/test_gflow.py` & `graphix-0.2.3/tests/test_gflow.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/tests/test_graphsim.py` & `graphix-0.2.3/tests/test_graphsim.py`

 * *Files identical despite different names*

### Comparing `graphix-0.2.2/tests/test_pattern.py` & `graphix-0.2.3/tests/test_pattern.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from graphix.pattern import Pattern, CommandNode
 
 
 class TestPattern(unittest.TestCase):
     def test_standardize(self):
         nqubits = 2
         depth = 1
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
+        circuit = rc.get_rand_circuit(nqubits, depth)
         pattern = circuit.transpile()
         pattern.standardize(method="global")
         np.testing.assert_equal(pattern.is_standard(), True)
         state = circuit.simulate_statevector()
         state_mbqc = pattern.simulate_pattern()
         np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_minimize_space(self):
         nqubits = 5
         depth = 5
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
+        circuit = rc.get_rand_circuit(nqubits, depth)
         pattern = circuit.transpile()
         pattern.standardize(method="global")
         pattern.minimize_space()
         state = circuit.simulate_statevector()
         state_mbqc = pattern.simulate_pattern()
         np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
@@ -54,89 +52,88 @@
             pattern.standardize(method="global")
             pattern.minimize_space()
             np.testing.assert_equal(pattern.max_space(), nqubits + 1)
 
     def test_parallelize_pattern(self):
         nqubits = 2
         depth = 1
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
+        circuit = rc.get_rand_circuit(nqubits, depth)
         pattern = circuit.transpile()
         pattern.standardize(method="global")
         pattern.parallelize_pattern()
         state = circuit.simulate_statevector()
         state_mbqc = pattern.simulate_pattern()
         np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_shift_signals(self):
         nqubits = 2
         depth = 1
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize(method="global")
-        pattern.shift_signals(method="global")
-        np.testing.assert_equal(pattern.is_standard(), True)
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize(method="global")
+            pattern.shift_signals(method="global")
+            np.testing.assert_equal(pattern.is_standard(), True)
+            state = circuit.simulate_statevector()
+            state_mbqc = pattern.simulate_pattern()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_pauli_measurment(self):
         nqubits = 3
         depth = 3
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize(method="global")
-        pattern.shift_signals(method="global")
-        pattern.perform_pauli_measurements()
-        pattern.minimize_space()
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize(method="global")
+            pattern.shift_signals(method="global")
+            pattern.perform_pauli_measurements()
+            pattern.minimize_space()
+            state = circuit.simulate_statevector()
+            state_mbqc = pattern.simulate_pattern()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_pauli_measurment_opt_gate(self):
         nqubits = 3
         depth = 3
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs, use_rzz=True)
-        pattern = circuit.transpile(opt=True)
-        pattern.standardize(method="global")
-        pattern.shift_signals(method="global")
-        pattern.perform_pauli_measurements()
-        pattern.minimize_space()
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth, use_rzz=True)
+            pattern = circuit.transpile(opt=True)
+            pattern.standardize(method="global")
+            pattern.shift_signals(method="global")
+            pattern.perform_pauli_measurements()
+            pattern.minimize_space()
+            state = circuit.simulate_statevector()
+            state_mbqc = pattern.simulate_pattern()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_pauli_measurment_opt_gate_transpiler(self):
         nqubits = 3
         depth = 3
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs, use_rzz=True)
-        pattern = circuit.standardize_and_transpile(opt=True)
-        pattern.standardize(method="global")
-        pattern.shift_signals(method="global")
-        pattern.perform_pauli_measurements()
-        pattern.minimize_space()
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth, use_rzz=True)
+            pattern = circuit.standardize_and_transpile(opt=True)
+            pattern.standardize(method="global")
+            pattern.shift_signals(method="global")
+            pattern.perform_pauli_measurements()
+            pattern.minimize_space()
+            state = circuit.simulate_statevector()
+            state_mbqc = pattern.simulate_pattern()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_pauli_measurment_opt_gate_transpiler_without_signalshift(self):
         nqubits = 3
         depth = 3
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs, use_rzz=True)
-        pattern = circuit.standardize_and_transpile(opt=True)
-        pattern.perform_pauli_measurements()
-        pattern.minimize_space()
-        state = circuit.simulate_statevector()
-        state_mbqc = pattern.simulate_pattern()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth, use_rzz=True)
+            pattern = circuit.standardize_and_transpile(opt=True)
+            pattern.perform_pauli_measurements()
+            pattern.minimize_space()
+            state = circuit.simulate_statevector()
+            state_mbqc = pattern.simulate_pattern()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_mbqc.flatten().conjugate(), state.flatten())), 1)
 
     def test_pauli_measurement(self):
         # test pattern is obtained from 3-qubit QFT with pauli measurement
         circuit = Circuit(3)
         for i in range(3):
             circuit.h(i)
         circuit.x(1)
@@ -260,109 +257,109 @@
                 edges_check2 = False
         np.testing.assert_equal(edges_check1, True)
         np.testing.assert_equal(edges_check2, True)
 
     def test_standardize(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        localpattern = pattern.get_local_pattern()
-        localpattern.standardize()
-        pattern = localpattern.get_pattern()
-        np.testing.assert_equal(pattern.is_standard(), True)
-        pattern.minimize_space()
-        state_p = pattern.simulate_pattern()
-        state_ref = circuit.simulate_statevector()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            localpattern = pattern.get_local_pattern()
+            localpattern.standardize()
+            pattern = localpattern.get_pattern()
+            np.testing.assert_equal(pattern.is_standard(), True)
+            pattern.minimize_space()
+            state_p = pattern.simulate_pattern()
+            state_ref = circuit.simulate_statevector()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_shift_signals(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        localpattern = pattern.get_local_pattern()
-        localpattern.standardize()
-        localpattern.shift_signals()
-        pattern = localpattern.get_pattern()
-        np.testing.assert_equal(pattern.is_standard(), True)
-        pattern.minimize_space()
-        state_p = pattern.simulate_pattern()
-        state_ref = circuit.simulate_statevector()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            localpattern = pattern.get_local_pattern()
+            localpattern.standardize()
+            localpattern.shift_signals()
+            pattern = localpattern.get_pattern()
+            np.testing.assert_equal(pattern.is_standard(), True)
+            pattern.minimize_space()
+            state_p = pattern.simulate_pattern()
+            state_ref = circuit.simulate_statevector()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_standardize_and_shift_signals(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize_and_shift_signals()
-        np.testing.assert_equal(pattern.is_standard(), True)
-        pattern.minimize_space()
-        state_p = pattern.simulate_pattern()
-        state_ref = circuit.simulate_statevector()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize_and_shift_signals()
+            np.testing.assert_equal(pattern.is_standard(), True)
+            pattern.minimize_space()
+            state_p = pattern.simulate_pattern()
+            state_ref = circuit.simulate_statevector()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_mixed_pattern_operations(self):
         processes = [
             [["standardize", "global"], ["standardize", "local"]],
             [["standardize", "local"], ["signal", "global"], ["signal", "local"]],
             [
                 ["standardize", "local"],
                 ["signal", "global"],
                 ["standardize", "global"],
                 ["signal", "local"],
             ],
         ]
         nqubits = 3
         depth = 2
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        state_ref = circuit.simulate_statevector()
-        for process in processes:
-            pattern = circuit.transpile()
-            for operation in process:
-                if operation[0] == "standardize":
-                    pattern.standardize(method=operation[1])
-                elif operation[0] == "signal":
-                    pattern.shift_signals(method=operation[1])
-            np.testing.assert_equal(pattern.is_standard(), True)
-            pattern.minimize_space()
-            state_p = pattern.simulate_pattern()
-            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(3):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            state_ref = circuit.simulate_statevector()
+            for process in processes:
+                pattern = circuit.transpile()
+                for operation in process:
+                    if operation[0] == "standardize":
+                        pattern.standardize(method=operation[1])
+                    elif operation[0] == "signal":
+                        pattern.shift_signals(method=operation[1])
+                np.testing.assert_equal(pattern.is_standard(), True)
+                pattern.minimize_space()
+                state_p = pattern.simulate_pattern()
+                np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_opt_transpile_standardize(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile(opt=True)
-        pattern.standardize(method="local")
-        np.testing.assert_equal(pattern.is_standard(), True)
-        pattern.minimize_space()
-        state_p = pattern.simulate_pattern()
-        state_ref = circuit.simulate_statevector()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile(opt=True)
+            pattern.standardize(method="local")
+            np.testing.assert_equal(pattern.is_standard(), True)
+            pattern.minimize_space()
+            state_p = pattern.simulate_pattern()
+            state_ref = circuit.simulate_statevector()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_opt_transpile_shift_signals(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile(opt=True)
-        pattern.standardize(method="local")
-        pattern.shift_signals(method="local")
-        np.testing.assert_equal(pattern.is_standard(), True)
-        pattern.minimize_space()
-        state_p = pattern.simulate_pattern()
-        state_ref = circuit.simulate_statevector()
-        np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile(opt=True)
+            pattern.standardize(method="local")
+            pattern.shift_signals(method="local")
+            np.testing.assert_equal(pattern.is_standard(), True)
+            pattern.minimize_space()
+            state_p = pattern.simulate_pattern()
+            state_ref = circuit.simulate_statevector()
+            np.testing.assert_almost_equal(np.abs(np.dot(state_p.flatten().conjugate(), state_ref.flatten())), 1)
 
     def test_node_is_standardized(self):
         ref_sequence = [
             [[1, 2, 3, -1], True],
             [[1, 2, 3, -2, -3, -2, -4], True],
             [[1, -4, 2, -3, -1, 3], False],
             [[1, 2, 3, -1, -4, 2], False],
@@ -371,22 +368,22 @@
             node = CommandNode(0, seq, [], [], False, [], [])
             result = node.is_standard()
             np.testing.assert_equal(result, ref)
 
     def test_localpattern_is_standard(self):
         nqubits = 5
         depth = 4
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        localpattern = circuit.transpile().get_local_pattern()
-        result1 = localpattern.is_standard()
-        localpattern.standardize()
-        result2 = localpattern.is_standard()
-        np.testing.assert_equal(result1, False)
-        np.testing.assert_equal(result2, True)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            localpattern = circuit.transpile().get_local_pattern()
+            result1 = localpattern.is_standard()
+            localpattern.standardize()
+            result2 = localpattern.is_standard()
+            np.testing.assert_equal(result1, False)
+            np.testing.assert_equal(result2, True)
 
 
 def assert_equal_edge(edge, ref):
     if (edge[0] == ref[0]) and (edge[1] == ref[1]):
         return True
     elif (edge[0] == ref[1]) and (edge[1] == ref[0]):
         return True
```

### Comparing `graphix-0.2.2/tests/test_tnsim.py` & `graphix-0.2.3/tests/test_tnsim.py`

 * *Files 4% similar despite different names*

```diff
@@ -294,100 +294,100 @@
         tn_mbqc = pattern.simulate_pattern(backend="tensornetwork")
         random_op2 = random_op(2)
         value1 = state.expectation_value(random_op2, [0, 1])
         value2 = tn_mbqc.expectation_value(random_op2, [0, 1])
         np.testing.assert_almost_equal(value1, value2)
 
     def test_with_graphtrans(self):
-        nqubits = 3
+        nqubits = 4
         depth = 6
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize()
-        pattern.shift_signals()
-        pattern.perform_pauli_measurements()
-        state = circuit.simulate_statevector()
-        tn_mbqc = pattern.simulate_pattern(backend="tensornetwork")
-        random_op3 = random_op(3)
-        input = [0, 1, 2]
-        for qargs in itertools.permutations(input):
-            value1 = state.expectation_value(random_op3, list(qargs))
-            value2 = tn_mbqc.expectation_value(random_op3, list(qargs))
-            np.testing.assert_almost_equal(value1, value2)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize()
+            pattern.shift_signals()
+            pattern.perform_pauli_measurements()
+            state = circuit.simulate_statevector()
+            tn_mbqc = pattern.simulate_pattern(backend="tensornetwork")
+            random_op3 = random_op(3)
+            input = [0, 1, 2]
+            for qargs in itertools.permutations(input):
+                value1 = state.expectation_value(random_op3, list(qargs))
+                value2 = tn_mbqc.expectation_value(random_op3, list(qargs))
+                np.testing.assert_almost_equal(value1, value2)
 
     def test_with_graphtrans_sequential(self):
-        nqubits = 3
+        nqubits = 4
         depth = 6
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize()
-        pattern.shift_signals()
-        pattern.perform_pauli_measurements()
-        state = circuit.simulate_statevector()
-        tn_mbqc = pattern.simulate_pattern(backend="tensornetwork", graph_prep="sequential")
-        random_op3 = random_op(3)
-        input = [0, 1, 2]
-        for qargs in itertools.permutations(input):
-            value1 = state.expectation_value(random_op3, list(qargs))
-            value2 = tn_mbqc.expectation_value(random_op3, list(qargs))
-            np.testing.assert_almost_equal(value1, value2)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize()
+            pattern.shift_signals()
+            pattern.perform_pauli_measurements()
+            state = circuit.simulate_statevector()
+            tn_mbqc = pattern.simulate_pattern(backend="tensornetwork", graph_prep="sequential")
+            random_op3 = random_op(3)
+            input = [0, 1, 2]
+            for qargs in itertools.permutations(input):
+                value1 = state.expectation_value(random_op3, list(qargs))
+                value2 = tn_mbqc.expectation_value(random_op3, list(qargs))
+                np.testing.assert_almost_equal(value1, value2)
 
     def test_coef_state(self):
         nqubits = 4
         depth = 2
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.standardize_and_transpile()
-
-        statevec_ref = circuit.simulate_statevector()
-
-        tn = pattern.simulate_pattern("tensornetwork")
-        for number in range(len(statevec_ref.flatten())):
-            self.subTest(number=number)
-            coef_tn = tn.get_basis_coefficient(number)
-            coef_sv = statevec_ref.flatten()[number]
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.standardize_and_transpile()
 
-            np.testing.assert_almost_equal(abs(coef_tn), abs(coef_sv))
+            statevec_ref = circuit.simulate_statevector()
+
+            tn = pattern.simulate_pattern("tensornetwork")
+            for number in range(len(statevec_ref.flatten())):
+                self.subTest(number=number)
+                coef_tn = tn.get_basis_coefficient(number)
+                coef_sv = statevec_ref.flatten()[number]
+
+                np.testing.assert_almost_equal(abs(coef_tn), abs(coef_sv))
 
     def test_to_statevector(self):
         nqubits_set = [i for i in range(2, 6)]
         depth = 3
         for nqubits in nqubits_set:
             self.subTest(nqubit=nqubits)
-            pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-            circuit = rc.generate_gate(nqubits, depth, pairs)
-            pattern = circuit.standardize_and_transpile()
-            statevec_ref = circuit.simulate_statevector()
+            for i in range(5):
+                circuit = rc.get_rand_circuit(nqubits, depth)
+                pattern = circuit.standardize_and_transpile()
+                statevec_ref = circuit.simulate_statevector()
 
-            tn = pattern.simulate_pattern("tensornetwork")
-            statevec_tn = tn.to_statevector()
+                tn = pattern.simulate_pattern("tensornetwork")
+                statevec_tn = tn.to_statevector()
 
-            inner_product = np.inner(statevec_tn, statevec_ref.flatten().conjugate())
-            np.testing.assert_almost_equal(abs(inner_product), 1)
+                inner_product = np.inner(statevec_tn, statevec_ref.flatten().conjugate())
+                np.testing.assert_almost_equal(abs(inner_product), 1)
 
     def test_evolve(self):
-        nqubits = 3
+        nqubits = 4
         depth = 6
-        pairs = [(i, np.mod(i + 1, nqubits)) for i in range(nqubits)]
-        circuit = rc.generate_gate(nqubits, depth, pairs)
-        pattern = circuit.transpile()
-        pattern.standardize()
-        pattern.shift_signals()
-        pattern.perform_pauli_measurements()
-        state = circuit.simulate_statevector()
-        tn_mbqc = pattern.simulate_pattern(backend="tensornetwork")
-        random_op3 = random_op(3)
-        random_op3_exp = random_op(3)
+        for i in range(10):
+            circuit = rc.get_rand_circuit(nqubits, depth)
+            pattern = circuit.transpile()
+            pattern.standardize()
+            pattern.shift_signals()
+            pattern.perform_pauli_measurements()
+            state = circuit.simulate_statevector()
+            tn_mbqc = pattern.simulate_pattern(backend="tensornetwork")
+            random_op3 = random_op(3)
+            random_op3_exp = random_op(3)
 
-        state.evolve(random_op3, [0, 1, 2])
-        tn_mbqc.evolve(random_op3, [0, 1, 2], decompose=False)
+            state.evolve(random_op3, [0, 1, 2])
+            tn_mbqc.evolve(random_op3, [0, 1, 2], decompose=False)
 
-        expval_tn = tn_mbqc.expectation_value(random_op3_exp, [0, 1, 2])
-        expval_ref = state.expectation_value(random_op3_exp, [0, 1, 2])
+            expval_tn = tn_mbqc.expectation_value(random_op3_exp, [0, 1, 2])
+            expval_ref = state.expectation_value(random_op3_exp, [0, 1, 2])
 
-        np.testing.assert_almost_equal(expval_tn, expval_ref)
+            np.testing.assert_almost_equal(expval_tn, expval_ref)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `graphix-0.2.2/tests/test_transpiler.py` & `graphix-0.2.3/tests/test_transpiler.py`

 * *Files identical despite different names*

