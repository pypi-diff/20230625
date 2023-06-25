# Comparing `tmp/bpmn-tools-0.1.0.tar.gz` & `tmp/bpmn-tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpmn-tools-0.1.0.tar", last modified: Wed May 31 09:45:30 2023, max compression
+gzip compressed data, was "bpmn-tools-0.1.1.tar", last modified: Sun Jun 25 08:14:28 2023, max compression
```

## Comparing `bpmn-tools-0.1.0.tar` & `bpmn-tools-0.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.308263 bpmn-tools-0.1.0/
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.305083 bpmn-tools-0.1.0/.github/
--rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.0/.github/README.md
--rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/LICENSE.txt
--rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/MANIFEST.in
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-31 09:45:30.308155 bpmn-tools-0.1.0/PKG-INFO
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306073 bpmn-tools-0.1.0/bpmn_tools/
--rw-r--r--   0 xtof       (501) staff       (20)       91 2023-05-31 09:44:39.000000 bpmn-tools-0.1.0/bpmn_tools/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-05-30 17:10:54.000000 bpmn-tools-0.1.0/bpmn_tools/collaboration.py
--rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.0/bpmn_tools/colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-05-31 09:17:36.000000 bpmn-tools-0.1.0/bpmn_tools/diagrams.py
--rw-r--r--   0 xtof       (501) staff       (20)     6648 2023-05-31 08:29:20.000000 bpmn-tools-0.1.0/bpmn_tools/flow.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306925 bpmn-tools-0.1.0/bpmn_tools/layout/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.0/bpmn_tools/layout/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     4430 2023-05-31 09:03:53.000000 bpmn-tools-0.1.0/bpmn_tools/layout/simple.py
--rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-05-31 08:57:15.000000 bpmn-tools-0.1.0/bpmn_tools/notation.py
--rw-r--r--   0 xtof       (501) staff       (20)      744 2023-05-31 09:05:57.000000 bpmn-tools-0.1.0/bpmn_tools/util.py
--rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.0/bpmn_tools/visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-05-31 07:52:16.000000 bpmn-tools-0.1.0/bpmn_tools/xml.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.306728 bpmn-tools-0.1.0/bpmn_tools.egg-info/
--rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/PKG-INFO
--rw-r--r--   0 xtof       (501) staff       (20)      703 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/SOURCES.txt
--rw-r--r--   0 xtof       (501) staff       (20)        1 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/dependency_links.txt
--rw-r--r--   0 xtof       (501) staff       (20)       48 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/entry_points.txt
--rw-r--r--   0 xtof       (501) staff       (20)       24 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/requires.txt
--rw-r--r--   0 xtof       (501) staff       (20)       22 2023-05-31 09:45:30.000000 bpmn-tools-0.1.0/bpmn_tools.egg-info/top_level.txt
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.307114 bpmn-tools-0.1.0/docs/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/docs/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/docs/conf.py
--rw-r--r--   0 xtof       (501) staff       (20)       38 2023-05-31 09:45:30.308301 bpmn-tools-0.1.0/setup.cfg
--rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.0/setup.py
-drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-05-31 09:45:30.307966 bpmn-tools-0.1.0/tests/
--rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.0/tests/__init__.py
--rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.0/tests/test_colors.py
--rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.0/tests/test_flows.py
--rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.0/tests/test_hello.py
--rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.0/tests/test_lanes.py
--rw-r--r--   0 xtof       (501) staff       (20)     1133 2023-05-31 08:58:08.000000 bpmn-tools-0.1.0/tests/test_roundtrip.py
--rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.0/tests/test_visitor.py
--rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.0/tests/test_xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.510932 bpmn-tools-0.1.1/
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.506826 bpmn-tools-0.1.1/.github/
+-rw-r--r--   0 xtof       (501) staff       (20)     2335 2023-05-29 16:17:25.000000 bpmn-tools-0.1.1/.github/README.md
+-rw-r--r--   0 xtof       (501) staff       (20)     1062 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/LICENSE.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       77 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/MANIFEST.in
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-06-25 08:14:28.510821 bpmn-tools-0.1.1/PKG-INFO
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.507771 bpmn-tools-0.1.1/bpmn_tools/
+-rw-r--r--   0 xtof       (501) staff       (20)       91 2023-06-25 08:13:25.000000 bpmn-tools-0.1.1/bpmn_tools/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1002 2023-06-25 07:47:11.000000 bpmn-tools-0.1.1/bpmn_tools/collaboration.py
+-rw-r--r--   0 xtof       (501) staff       (20)      957 2023-05-31 08:54:54.000000 bpmn-tools-0.1.1/bpmn_tools/colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     6325 2023-05-31 09:17:36.000000 bpmn-tools-0.1.1/bpmn_tools/diagrams.py
+-rw-r--r--   0 xtof       (501) staff       (20)     7094 2023-06-25 08:11:42.000000 bpmn-tools-0.1.1/bpmn_tools/flow.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508583 bpmn-tools-0.1.1/bpmn_tools/layout/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-05-29 12:19:35.000000 bpmn-tools-0.1.1/bpmn_tools/layout/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4430 2023-05-31 09:03:53.000000 bpmn-tools-0.1.1/bpmn_tools/layout/simple.py
+-rw-r--r--   0 xtof       (501) staff       (20)     3228 2023-06-25 08:13:52.000000 bpmn-tools-0.1.1/bpmn_tools/notation.py
+-rw-r--r--   0 xtof       (501) staff       (20)      744 2023-05-31 09:05:57.000000 bpmn-tools-0.1.1/bpmn_tools/util.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1203 2023-05-29 13:34:37.000000 bpmn-tools-0.1.1/bpmn_tools/visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4665 2023-05-31 07:52:16.000000 bpmn-tools-0.1.1/bpmn_tools/xml.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508408 bpmn-tools-0.1.1/bpmn_tools.egg-info/
+-rw-r--r--   0 xtof       (501) staff       (20)     3333 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/PKG-INFO
+-rw-r--r--   0 xtof       (501) staff       (20)      703 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 xtof       (501) staff       (20)        1 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       48 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/entry_points.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       24 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/requires.txt
+-rw-r--r--   0 xtof       (501) staff       (20)       22 2023-06-25 08:14:28.000000 bpmn-tools-0.1.1/bpmn_tools.egg-info/top_level.txt
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.508763 bpmn-tools-0.1.1/docs/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/docs/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     5481 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/docs/conf.py
+-rw-r--r--   0 xtof       (501) staff       (20)       38 2023-06-25 08:14:28.510970 bpmn-tools-0.1.1/setup.cfg
+-rw-r--r--   0 xtof       (501) staff       (20)     1472 2023-05-29 16:12:47.000000 bpmn-tools-0.1.1/setup.py
+drwxr-xr-x   0 xtof       (501) staff       (20)        0 2023-06-25 08:14:28.510525 bpmn-tools-0.1.1/tests/
+-rw-r--r--   0 xtof       (501) staff       (20)        0 2023-04-16 17:05:11.000000 bpmn-tools-0.1.1/tests/__init__.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1326 2023-05-30 20:03:04.000000 bpmn-tools-0.1.1/tests/test_colors.py
+-rw-r--r--   0 xtof       (501) staff       (20)     2208 2023-05-31 08:38:49.000000 bpmn-tools-0.1.1/tests/test_flows.py
+-rw-r--r--   0 xtof       (501) staff       (20)    10458 2023-05-30 19:47:37.000000 bpmn-tools-0.1.1/tests/test_hello.py
+-rw-r--r--   0 xtof       (501) staff       (20)     4076 2023-05-31 08:39:36.000000 bpmn-tools-0.1.1/tests/test_lanes.py
+-rw-r--r--   0 xtof       (501) staff       (20)     1133 2023-05-31 08:58:08.000000 bpmn-tools-0.1.1/tests/test_roundtrip.py
+-rw-r--r--   0 xtof       (501) staff       (20)      887 2023-05-29 15:17:30.000000 bpmn-tools-0.1.1/tests/test_visitor.py
+-rw-r--r--   0 xtof       (501) staff       (20)      370 2023-05-29 15:17:39.000000 bpmn-tools-0.1.1/tests/test_xml.py
```

### Comparing `bpmn-tools-0.1.0/.github/README.md` & `bpmn-tools-0.1.1/.github/README.md`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/LICENSE.txt` & `bpmn-tools-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/PKG-INFO` & `bpmn-tools-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.0/bpmn_tools/collaboration.py` & `bpmn-tools-0.1.1/bpmn_tools/collaboration.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/colors.py` & `bpmn-tools-0.1.1/bpmn_tools/colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/diagrams.py` & `bpmn-tools-0.1.1/bpmn_tools/diagrams.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/flow.py` & `bpmn-tools-0.1.1/bpmn_tools/flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,14 +125,26 @@
 class Task(Element):
   __tag__     = "bpmn:task"
 
   def __init__(self, name="", **kwargs):
     super().__init__(**kwargs)
     self["name"] = name
 
+  @property
+  def process(self):
+    return self._parent
+
+  @property
+  def lane(self):
+    for lane in self.process.laneset.lanes:
+      for ref in lane.refs:
+        if ref.ref == self:
+          return lane
+    return None
+
 class UserTask(Task):
   __tag__ = "bpmn:userTask"
 
 class ScriptTask(Task):
   __tag__ = "bpmn:scriptTask"
 
 class ServiceTask(Task):
@@ -143,15 +155,15 @@
 
   def __init__(self, ref=None, **kwargs):
     super().__init__(**kwargs)
     self._ref = ref
 
   @property
   def process(self):
-    return self._parent.process()
+    return self._parent.process
 
   @property
   def ref(self):
     if self._ref:
       return self._ref
     try:
       return self.process.element(super().text)
@@ -245,14 +257,22 @@
   def element(self, id):
     for element in self._elements:
       if element["id"] == id:
         return element
     return None
   
   @property
+  def participant(self):
+    for collaboration in self._parent.collaborations:
+      participant = collaboration.find("processRef", self.id)
+      if participant:
+        return participant
+    return None
+  
+  @property
   def elements(self):
     elems = self._elements  # direct elements
     # add elements that are "hidden" in lanes
     if len(self.laneset) > 0:
       for lane in self.laneset.lanes:
         for element in lane.elements:
           if not element in elems:
```

### Comparing `bpmn-tools-0.1.0/bpmn_tools/layout/simple.py` & `bpmn-tools-0.1.1/bpmn_tools/layout/simple.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/notation.py` & `bpmn-tools-0.1.1/bpmn_tools/notation.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/util.py` & `bpmn-tools-0.1.1/bpmn_tools/util.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/visitor.py` & `bpmn-tools-0.1.1/bpmn_tools/visitor.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools/xml.py` & `bpmn-tools-0.1.1/bpmn_tools/xml.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/bpmn_tools.egg-info/PKG-INFO` & `bpmn-tools-0.1.1/bpmn_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpmn-tools
-Version: 0.1.0
+Version: 0.1.1
 Summary: a collection of tools to work with BPMN
 Home-page: https://github.com/christophevg/bpmn-tools
 Author: Christophe VG
 License: MIT
 Description: # BPMN Tools
         
         > a collection of tools to work with BPMN
```

### Comparing `bpmn-tools-0.1.0/bpmn_tools.egg-info/SOURCES.txt` & `bpmn-tools-0.1.1/bpmn_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/docs/conf.py` & `bpmn-tools-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/setup.py` & `bpmn-tools-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_colors.py` & `bpmn-tools-0.1.1/tests/test_colors.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_flows.py` & `bpmn-tools-0.1.1/tests/test_flows.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_hello.py` & `bpmn-tools-0.1.1/tests/test_hello.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_lanes.py` & `bpmn-tools-0.1.1/tests/test_lanes.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_roundtrip.py` & `bpmn-tools-0.1.1/tests/test_roundtrip.py`

 * *Files identical despite different names*

### Comparing `bpmn-tools-0.1.0/tests/test_visitor.py` & `bpmn-tools-0.1.1/tests/test_visitor.py`

 * *Files identical despite different names*

