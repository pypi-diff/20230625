# Comparing `tmp/anonpi-0.1.0.tar.gz` & `tmp/anonpi-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonpi-0.1.0.tar", last modified: Sun Jun 25 08:08:04 2023, max compression
+gzip compressed data, was "anonpi-0.1.5.tar", last modified: Sun Jun 25 08:25:07 2023, max compression
```

## Comparing `anonpi-0.1.0.tar` & `anonpi-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-25 08:08:04.973553 anonpi-0.1.0/
--rw-rw-rw-   0        0        0     2143 2023-06-25 08:08:04.972553 anonpi-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-25 08:08:04.922584 anonpi-0.1.0/anonpi/
--rw-rw-rw-   0        0        0       85 2023-06-25 08:07:17.000000 anonpi-0.1.0/anonpi/__init__.py
--rw-rw-rw-   0        0        0       41 2023-06-25 08:06:08.000000 anonpi-0.1.0/anonpi/call.py
-drwxrwxrwx   0        0        0        0 2023-06-25 08:08:04.970555 anonpi-0.1.0/anonpi.egg-info/
--rw-rw-rw-   0        0        0     2143 2023-06-25 08:08:04.000000 anonpi-0.1.0/anonpi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      191 2023-06-25 08:08:04.000000 anonpi-0.1.0/anonpi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-25 08:08:04.000000 anonpi-0.1.0/anonpi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-25 08:08:04.000000 anonpi-0.1.0/anonpi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-25 08:08:04.000000 anonpi-0.1.0/anonpi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-25 08:08:04.974552 anonpi-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      790 2023-06-25 08:04:48.000000 anonpi-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:25:07.238248 anonpi-0.1.5/
+-rw-rw-rw-   0        0        0     2143 2023-06-25 08:25:07.236249 anonpi-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-25 08:25:07.202263 anonpi-0.1.5/anonpi/
+-rw-rw-rw-   0        0        0     2066 2023-06-25 08:24:54.000000 anonpi-0.1.5/anonpi/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-06-25 08:24:26.000000 anonpi-0.1.5/anonpi/call.py
+drwxrwxrwx   0        0        0        0 2023-06-25 08:25:07.234252 anonpi-0.1.5/anonpi.egg-info/
+-rw-rw-rw-   0        0        0     2143 2023-06-25 08:25:06.000000 anonpi-0.1.5/anonpi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-06-25 08:25:07.000000 anonpi-0.1.5/anonpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 08:25:06.000000 anonpi-0.1.5/anonpi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-25 08:25:06.000000 anonpi-0.1.5/anonpi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-25 08:25:06.000000 anonpi-0.1.5/anonpi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 08:25:07.239247 anonpi-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      790 2023-06-25 08:24:14.000000 anonpi-0.1.5/setup.py
```

### Comparing `anonpi-0.1.0/PKG-INFO` & `anonpi-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonpi
-Version: 0.1.0
+Version: 0.1.5
 Summary: The "anonpi" module is a powerful Python package that provides a convenient interface for interacting with calling systems. It simplifies the development of applications that require functionalities such as machine detection, IVR (Interactive Voice Response), DTMF (Dual-Tone Multi-Frequency) handling, recording, playback, and more
 Author: Adistar
 Author-email: adityasamalllll6@gmail.com
 Description-Content-Type: text/markdown
 
 # anonpi: Python Module for Calling Systems
```

### Comparing `anonpi-0.1.0/anonpi.egg-info/PKG-INFO` & `anonpi-0.1.5/anonpi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonpi
-Version: 0.1.0
+Version: 0.1.5
 Summary: The "anonpi" module is a powerful Python package that provides a convenient interface for interacting with calling systems. It simplifies the development of applications that require functionalities such as machine detection, IVR (Interactive Voice Response), DTMF (Dual-Tone Multi-Frequency) handling, recording, playback, and more
 Author: Adistar
 Author-email: adityasamalllll6@gmail.com
 Description-Content-Type: text/markdown
 
 # anonpi: Python Module for Calling Systems
```

### Comparing `anonpi-0.1.0/setup.py` & `anonpi-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 
 
 setup(
     name='anonpi',
-    version='0.1.0',
+    version='0.1.5',
     author='Adistar',
     author_email='adityasamalllll6@gmail.com',
     description='The "anonpi" module is a powerful Python package that provides a convenient interface for interacting with calling systems. It simplifies the development of applications that require functionalities such as machine detection, IVR (Interactive Voice Response), DTMF (Dual-Tone Multi-Frequency) handling, recording, playback, and more',
     packages=['anonpi'],
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['requests','flask','colorama']
```

