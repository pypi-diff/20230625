# Comparing `tmp/kubescaler-0.0.11.tar.gz` & `tmp/kubescaler-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubescaler-0.0.11.tar", last modified: Wed Jun 21 21:22:39 2023, max compression
+gzip compressed data, was "kubescaler-0.0.12.tar", last modified: Sun Jun 25 05:02:22 2023, max compression
```

## Comparing `kubescaler-0.0.11.tar` & `kubescaler-0.0.12.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.11/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.11/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.11/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.11/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3372 2023-06-21 21:22:39.094038 kubescaler-0.0.11/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.11/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/decorators.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6105 2023-05-24 04:39:20.000000 kubescaler-0.0.11/kubescaler/logger.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler/scaler/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       59 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/kubescaler/scaler/aws/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/ami.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22082 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/scaler/aws/template.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.11/kubescaler/scaler/google.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.094038 kubescaler-0.0.11/kubescaler/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.11/kubescaler/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.11/kubescaler/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-21 21:22:35.000000 kubescaler-0.0.11/kubescaler/version.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-21 21:22:39.090038 kubescaler-0.0.11/kubescaler.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3372 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      716 2023-06-21 21:22:39.000000 kubescaler-0.0.11/kubescaler.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.11/kubescaler.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      228 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-06-21 21:22:38.000000 kubescaler-0.0.11/kubescaler.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.11/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-06-21 21:22:39.094038 kubescaler-0.0.11/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3582 2023-05-24 04:57:06.000000 kubescaler-0.0.11/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-05-24 04:09:38.000000 kubescaler-0.0.12/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-05-24 04:09:38.000000 kubescaler-0.0.12/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      317 2023-05-24 04:15:45.000000 kubescaler-0.0.12/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-05-24 04:09:38.000000 kubescaler-0.0.12/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-06-25 05:02:22.354797 kubescaler-0.0.12/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2512 2023-05-25 18:09:11.000000 kubescaler-0.0.12/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2370 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1755 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/decorators.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      604 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6105 2023-05-24 04:39:20.000000 kubescaler-0.0.12/kubescaler/logger.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler/scaler/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:18.000000 kubescaler-0.0.12/kubescaler/scaler/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/kubescaler/scaler/aws/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       32 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1103 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/ami.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    22082 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/scaler/aws/template.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    11961 2023-06-21 21:22:35.000000 kubescaler-0.0.12/kubescaler/scaler/google.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.354797 kubescaler-0.0.12/kubescaler/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      399 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5085 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-05-24 04:38:11.000000 kubescaler-0.0.12/kubescaler/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      912 2023-05-25 18:09:11.000000 kubescaler-0.0.12/kubescaler/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1414 2023-06-25 05:02:18.000000 kubescaler-0.0.12/kubescaler/version.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-06-25 05:02:22.350798 kubescaler-0.0.12/kubescaler.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3374 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      716 2023-06-25 05:02:22.000000 kubescaler-0.0.12/kubescaler.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-24 05:01:47.000000 kubescaler-0.0.12/kubescaler.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      230 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       11 2023-06-25 05:02:21.000000 kubescaler-0.0.12/kubescaler.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-05-24 04:09:39.000000 kubescaler-0.0.12/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      294 2023-06-25 05:02:22.354797 kubescaler-0.0.12/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3584 2023-06-25 05:02:18.000000 kubescaler-0.0.12/setup.py
```

### Comparing `kubescaler-0.0.11/LICENSE` & `kubescaler-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/NOTICE` & `kubescaler-0.0.12/NOTICE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/PKG-INFO` & `kubescaler-0.0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.11
+Version: 0.0.12
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: basic
 Provides-Extra: google
 Provides-Extra: aws
 License-File: LICENSE
 License-File: NOTICE
 
 # KubeScaler
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.11 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.12 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
-Type: text/markdown Provides-Extra: all Provides-Extra: google Provides-Extra:
-aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
+Type: text/markdown Provides-Extra: basic Provides-Extra: google Provides-
+Extra: aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
 Kubernetes cluster YUGE! Or Smol. :)  [![All Contributors](https://
 img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
 (#contributors-)  [![PyPI](https://img.shields.io/pypi/v/kubescaler)](https://
 pypi.org/project/kubescaler/) [KubeScaler_Logo] This is a set of helper Python
 classes that make it easy to add elasticity, or scaling up and down, of your
 Kubernetes clusters in Python. We currently have support for the clouds we use,
 namely: - Google (GKE) - Amazon (EKS) ð§ï¸ **under development** ð§ï¸
```

### Comparing `kubescaler-0.0.11/README.md` & `kubescaler-0.0.12/README.md`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/cluster.py` & `kubescaler-0.0.12/kubescaler/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/decorators.py` & `kubescaler-0.0.12/kubescaler/decorators.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/defaults.py` & `kubescaler-0.0.12/kubescaler/defaults.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/logger.py` & `kubescaler-0.0.12/kubescaler/logger.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/scaler/aws/ami.py` & `kubescaler-0.0.12/kubescaler/scaler/aws/ami.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/scaler/aws/cluster.py` & `kubescaler-0.0.12/kubescaler/scaler/aws/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/scaler/aws/template.py` & `kubescaler-0.0.12/kubescaler/scaler/aws/template.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/scaler/google.py` & `kubescaler-0.0.12/kubescaler/scaler/google.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/utils/fileio.py` & `kubescaler-0.0.12/kubescaler/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/utils/misc.py` & `kubescaler-0.0.12/kubescaler/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/utils/terminal.py` & `kubescaler-0.0.12/kubescaler/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/kubescaler/version.py` & `kubescaler-0.0.12/kubescaler/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.11"
+__version__ = "0.0.12"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "kubescaler"
 PACKAGE_URL = "https://github.com/converged-computing/kubescaler"
 KEYWORDS = "Kubernetes, elasticity, scaling, EKS, GKE"
 DESCRIPTION = "Helper classes for scaling Kubernetes clusters"
 LICENSE = "LICENSE"
```

### Comparing `kubescaler-0.0.11/kubescaler.egg-info/PKG-INFO` & `kubescaler-0.0.12/kubescaler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.11
+Version: 0.0.12
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: basic
 Provides-Extra: google
 Provides-Extra: aws
 License-File: LICENSE
 License-File: NOTICE
 
 # KubeScaler
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.11 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.12 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3.8 Description-Content-
-Type: text/markdown Provides-Extra: all Provides-Extra: google Provides-Extra:
-aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
+Type: text/markdown Provides-Extra: basic Provides-Extra: google Provides-
+Extra: aws License-File: LICENSE License-File: NOTICE # KubeScaler > Make your
 Kubernetes cluster YUGE! Or Smol. :)  [![All Contributors](https://
 img.shields.io/badge/all_contributors-1-orange.svg?style=flat-square)]
 (#contributors-)  [![PyPI](https://img.shields.io/pypi/v/kubescaler)](https://
 pypi.org/project/kubescaler/) [KubeScaler_Logo] This is a set of helper Python
 classes that make it easy to add elasticity, or scaling up and down, of your
 Kubernetes clusters in Python. We currently have support for the clouds we use,
 namely: - Google (GKE) - Amazon (EKS) ð§ï¸ **under development** ð§ï¸
```

### Comparing `kubescaler-0.0.11/kubescaler.egg-info/SOURCES.txt` & `kubescaler-0.0.12/kubescaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.11/setup.py` & `kubescaler-0.0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,18 @@
         url=PACKAGE_URL,
         license=LICENSE,
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         long_description_content_type="text/markdown",
         keywords=KEYWORDS,
         setup_requires=["pytest-runner"],
-        install_requires=INSTALL_REQUIRES,
+        install_requires=INSTALL_REQUIRES_ALL,
         tests_require=TESTS_REQUIRES,
         extras_require={
-            "all": [INSTALL_REQUIRES_ALL],
+            "basic": [INSTALL_REQUIRES],
             "google": INSTALL_REQUIRES_GOOGLE,
             "aws": INSTALL_REQUIRES_AWS,
         },
         classifiers=[
             "Intended Audience :: Science/Research",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: MIT License",
```

