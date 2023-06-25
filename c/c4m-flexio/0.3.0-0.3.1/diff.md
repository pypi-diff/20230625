# Comparing `tmp/c4m_flexio-0.3.0.tar.gz` & `tmp/c4m_flexio-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexio-0.3.0.tar", last modified: Wed Mar  8 16:12:25 2023, max compression
+gzip compressed data, was "c4m_flexio-0.3.1.tar", last modified: Sun Jun 25 19:23:13 2023, max compression
```

## Comparing `c4m_flexio-0.3.0.tar` & `c4m_flexio-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:12:25.355614 c4m_flexio-0.3.0/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       95 2022-07-11 14:44:35.000000 c4m_flexio-0.3.0/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1354 2022-11-01 15:22:07.000000 c4m_flexio-0.3.0/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      482 2020-07-06 12:57:05.000000 c4m_flexio-0.3.0/COPYRIGHT.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      336 2020-07-06 12:49:55.000000 c4m_flexio-0.3.0/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:12:25.351614 c4m_flexio-0.3.0/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2020-07-06 12:49:55.000000 c4m_flexio-0.3.0/LICENSES/GPL-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 12:49:55.000000 c4m_flexio-0.3.0/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1455 2023-03-08 16:12:25.355614 c4m_flexio-0.3.0/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1000 2023-03-08 14:44:33.000000 c4m_flexio-0.3.0/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:12:25.351614 c4m_flexio-0.3.0/c4m/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       65 2020-10-07 17:43:33.000000 c4m_flexio-0.3.0/c4m/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:12:25.351614 c4m_flexio-0.3.0/c4m/flexio/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      107 2022-06-15 15:12:47.000000 c4m_flexio-0.3.0/c4m/flexio/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20860 2023-02-21 17:10:10.000000 c4m_flexio-0.3.0/c4m/flexio/_helpers.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   239603 2023-03-03 15:19:08.000000 c4m_flexio-0.3.0/c4m/flexio/factory.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-03-08 16:12:25.355614 c4m_flexio-0.3.0/c4m_flexio.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1455 2023-03-08 16:12:25.000000 c4m_flexio-0.3.0/c4m_flexio.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      418 2023-03-08 16:12:25.000000 c4m_flexio-0.3.0/c4m_flexio.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-03-08 16:12:25.000000 c4m_flexio-0.3.0/c4m_flexio.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       48 2023-03-08 16:12:25.000000 c4m_flexio-0.3.0/c4m_flexio.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-03-08 16:12:25.000000 c4m_flexio-0.3.0/c4m_flexio.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:22:23.000000 c4m_flexio-0.3.0/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-04-30 15:10:26.000000 c4m_flexio-0.3.0/dev-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1820 2022-04-30 14:32:24.000000 c4m_flexio-0.3.0/dodo.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-03-08 16:12:25.355614 c4m_flexio-0.3.0/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1380 2023-03-08 14:44:51.000000 c4m_flexio-0.3.0/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       95 2022-07-11 14:44:35.000000 c4m_flexio-0.3.1/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1354 2022-11-01 15:22:07.000000 c4m_flexio-0.3.1/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      482 2020-07-06 12:57:05.000000 c4m_flexio-0.3.1/COPYRIGHT.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      336 2020-07-06 12:49:55.000000 c4m_flexio-0.3.1/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2020-07-06 12:49:55.000000 c4m_flexio-0.3.1/LICENSES/GPL-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 12:49:55.000000 c4m_flexio-0.3.1/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1542 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1087 2023-06-25 19:21:43.000000 c4m_flexio-0.3.1/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/c4m/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       65 2020-10-07 17:43:33.000000 c4m_flexio-0.3.1/c4m/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/c4m/flexio/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      107 2022-06-15 15:12:47.000000 c4m_flexio-0.3.1/c4m/flexio/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    20860 2023-02-21 17:10:10.000000 c4m_flexio-0.3.1/c4m/flexio/_helpers.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   239603 2023-03-03 15:19:08.000000 c4m_flexio-0.3.1/c4m/flexio/factory.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/c4m_flexio.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1542 2023-06-25 19:23:13.000000 c4m_flexio-0.3.1/c4m_flexio.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      418 2023-06-25 19:23:13.000000 c4m_flexio-0.3.1/c4m_flexio.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-25 19:23:13.000000 c4m_flexio-0.3.1/c4m_flexio.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       55 2023-06-25 19:23:13.000000 c4m_flexio-0.3.1/c4m_flexio.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-06-25 19:23:13.000000 c4m_flexio-0.3.1/c4m_flexio.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:22:23.000000 c4m_flexio-0.3.1/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-04-30 15:10:26.000000 c4m_flexio-0.3.1/dev-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1976 2023-06-25 13:29:07.000000 c4m_flexio-0.3.1/dodo.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-25 19:23:13.631669 c4m_flexio-0.3.1/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1387 2023-06-25 13:28:34.000000 c4m_flexio-0.3.1/setup.py
```

### Comparing `c4m_flexio-0.3.0/.gitlab-ci.yml` & `c4m_flexio-0.3.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.3.0/LICENSES/GPL-2.0.txt` & `c4m_flexio-0.3.1/LICENSES/GPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.3.0/LICENSES/cern_ohl_s_v2.txt` & `c4m_flexio-0.3.1/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.3.0/PKG-INFO` & `c4m_flexio-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_flexio
-Version: 0.3.0
+Version: 0.3.1
 Summary: PDKMaster based scalable IO library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexio
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexio/issues
 Requires-Python: ~=3.6
@@ -15,14 +15,15 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* v0.3.1: no code change; mark IO cell code compatible with dev v0.4.0 of c4m-flexcell
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of tape-outs.  
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
```

### Comparing `c4m_flexio-0.3.0/c4m/flexio/_helpers.py` & `c4m_flexio-0.3.1/c4m/flexio/_helpers.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.3.0/c4m/flexio/factory.py` & `c4m_flexio-0.3.1/c4m/flexio/factory.py`

 * *Files identical despite different names*

### Comparing `c4m_flexio-0.3.0/c4m_flexio.egg-info/PKG-INFO` & `c4m_flexio-0.3.1/c4m_flexio.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexio
-Version: 0.3.0
+Version: 0.3.1
 Summary: PDKMaster based scalable IO library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexio
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexio/issues
 Requires-Python: ~=3.6
@@ -15,14 +15,15 @@
 
 A IO library is a collection of cells that allows to do the input and output from on-chip signals to outside the chip. Typically these libraries with a fixed set of cells with a fixed layout and functionality and provided by the foundry or a third party.
 
 Purpose of c4m-flexio library is to have a library that is easily scalable between different technologies using the [PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster) framework. It will also be configurable to adapt the cells to one's needs.
 
 ## Release history
 
+* v0.3.1: no code change; mark IO cell code compatible with dev v0.4.0 of c4m-flexcell
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md)
 * no notes for older releases
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever. The library now progresses at the need of tape-outs.  
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
```

### Comparing `c4m_flexio-0.3.0/dodo.py` & `c4m_flexio-0.3.1/dodo.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,17 +69,22 @@
         "actions": (f"{python} -m build",)
     }
 
 
 #
 # install
 def task_install():
-    """Install the python module"""
+    """Install the python module
+
+    It will not install dependencies to avoid overwriting locally installed versions
+    with release versions.
+    """
 
     return {
         "title": lambda _: "Installing python module",
         "file_dep": c4m_py_files,
         "targets": (flexio_inst_dir,),
         "actions": (
-            f"{pip} install {top_dir}",
+            f"{pip} install --no-deps {top_dir}",
+            f"{pip} check",
         ),
     }
```

### Comparing `c4m_flexio-0.3.0/setup.py` & `c4m_flexio-0.3.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     author_email="staf@fibraservi.eu",
     description="PDKMaster based scalable IO library",
     long_description=long_description,
     long_description_content_type="text/markdown",
    license="GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+",
     python_requires="~=3.6",
     setup_requires=["setuptools_scm"],
-    install_requires=["setuptools", "PDKMaster==0.9.*", "c4m-flexcell==0.3.*"],
+    install_requires=["setuptools", "PDKMaster==0.9.*", "c4m-flexcell>=0.3.3,<0.5.0"],
     include_package_data=True,
     packages=_packages,
     project_urls={
         #"Documentation": "???",
         "Source Code": "https://gitlab.com/Chips4Makers/c4m-flexio",
         "Bug Tracker": "https://gitlab.com/Chips4Makers/c4m-flexio/issues",
     },
```

