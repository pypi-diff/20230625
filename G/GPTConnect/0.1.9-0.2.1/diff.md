# Comparing `tmp/GPTConnect-0.1.9.tar.gz` & `tmp/GPTConnect-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPTConnect-0.1.9.tar", last modified: Sat Jun 24 09:36:49 2023, max compression
+gzip compressed data, was "GPTConnect-0.2.1.tar", last modified: Sun Jun 25 05:47:30 2023, max compression
```

## Comparing `GPTConnect-0.1.9.tar` & `GPTConnect-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.137951 GPTConnect-0.1.9/
-drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.126908 GPTConnect-0.1.9/GPTConnect.egg-info/
--rw-rw-rw-   0        0        0     1061 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-24 09:36:49.000000 GPTConnect-0.1.9/GPTConnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-24 09:36:48.000000 GPTConnect-0.1.9/GPTConnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-24 09:36:49.000000 GPTConnect-0.1.9/GPTConnect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1061 2023-06-24 09:36:49.136950 GPTConnect-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0      875 2023-06-24 07:57:09.000000 GPTConnect-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 09:36:49.134945 GPTConnect-0.1.9/gptconnect/
--rw-rw-rw-   0        0        0       90 2023-06-24 09:26:23.000000 GPTConnect-0.1.9/gptconnect/__init__.py
--rw-rw-rw-   0        0        0     2830 2023-06-24 09:31:52.000000 GPTConnect-0.1.9/gptconnect/gptconnect.py
--rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.1.9/gptconnect/gptfunction.py
--rw-rw-rw-   0        0        0      453 2023-06-24 09:33:05.000000 GPTConnect-0.1.9/gptconnect/gptfunctionhandler.py
--rw-rw-rw-   0        0        0       42 2023-06-24 09:36:49.137951 GPTConnect-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      364 2023-06-24 09:34:31.000000 GPTConnect-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:47:30.758866 GPTConnect-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-25 05:47:30.747853 GPTConnect-0.2.1/GPTConnect.egg-info/
+-rw-rw-rw-   0        0        0     1222 2023-06-25 05:47:30.000000 GPTConnect-0.2.1/GPTConnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-25 05:47:30.000000 GPTConnect-0.2.1/GPTConnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 05:47:30.000000 GPTConnect-0.2.1/GPTConnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-25 05:47:30.000000 GPTConnect-0.2.1/GPTConnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-25 05:47:30.000000 GPTConnect-0.2.1/GPTConnect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2023-06-25 05:39:53.000000 GPTConnect-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1222 2023-06-25 05:47:30.758866 GPTConnect-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      992 2023-06-25 05:44:14.000000 GPTConnect-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 05:47:30.756865 GPTConnect-0.2.1/gptconnect/
+-rw-rw-rw-   0        0        0       90 2023-06-24 09:26:23.000000 GPTConnect-0.2.1/gptconnect/__init__.py
+-rw-rw-rw-   0        0        0     2830 2023-06-24 09:31:52.000000 GPTConnect-0.2.1/gptconnect/gptconnect.py
+-rw-rw-rw-   0        0        0      807 2023-06-24 07:31:10.000000 GPTConnect-0.2.1/gptconnect/gptfunction.py
+-rw-rw-rw-   0        0        0      453 2023-06-24 09:33:05.000000 GPTConnect-0.2.1/gptconnect/gptfunctionhandler.py
+-rw-rw-rw-   0        0        0       42 2023-06-25 05:47:30.759865 GPTConnect-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      391 2023-06-25 05:47:28.000000 GPTConnect-0.2.1/setup.py
```

### Comparing `GPTConnect-0.1.9/GPTConnect.egg-info/PKG-INFO` & `GPTConnect-0.2.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-Metadata-Version: 2.1
-Name: GPTConnect
-Version: 0.1.9
-Summary: A python package to make GPT functions easy
-Home-page: https://github.com/SleepyStew/gptconnect
-Author: SleepyStew
-
 # GPTConnect
 
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
-## Features
+## 🔧 Features
 
 - 🎉 Simplified and intuitive decorator based system to define GPT functions.
-- 🔤 Function groups system that allow easy integration of multiple commands at a time
+- 🔤 Function groups system that allows for easy integration of multiple commands.
 - 🕐 More features coming soon! This package is only in early stages of development.
 
-## Install
+## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
-[example.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
+[example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+[example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.1.9/PKG-INFO` & `GPTConnect-0.2.1/GPTConnect.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: GPTConnect
-Version: 0.1.9
+Version: 0.2.1
 Summary: A python package to make GPT functions easy
 Home-page: https://github.com/SleepyStew/gptconnect
 Author: SleepyStew
+License: Apache 2.0
+License-File: LICENSE
 
 # GPTConnect
 
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
-## Features
+## 🔧 Features
 
 - 🎉 Simplified and intuitive decorator based system to define GPT functions.
-- 🔤 Function groups system that allow easy integration of multiple commands at a time
+- 🔤 Function groups system that allows for easy integration of multiple commands.
 - 🕐 More features coming soon! This package is only in early stages of development.
 
-## Install
+## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
-[example.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
+[example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+[example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.1.9/README.md` & `GPTConnect-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,29 @@
+Metadata-Version: 2.1
+Name: GPTConnect
+Version: 0.2.1
+Summary: A python package to make GPT functions easy
+Home-page: https://github.com/SleepyStew/gptconnect
+Author: SleepyStew
+License: Apache 2.0
+License-File: LICENSE
+
 # GPTConnect
 
 GPTConnect is a Python 🐍 package that simplifies the use of the new functions feature of ChatGPT by OpenAI. It provides an easy-to-use framework for creating and interacting with GPT functions, making your development process smoother and more efficient.
 
 Make sure to star this project if you find it useful! ✨
 
 If you have any ideas, bug reports or suggestions feel free to open an issue or contact me on discord at @**sleepystew**
 
-## Features
+## 🔧 Features
 
 - 🎉 Simplified and intuitive decorator based system to define GPT functions.
-- 🔤 Function groups system that allow easy integration of multiple commands at a time
+- 🔤 Function groups system that allows for easy integration of multiple commands.
 - 🕐 More features coming soon! This package is only in early stages of development.
 
-## Install
+## 🚀 Install
 `pip install GPTConnect`
 
 ## Example Usage
-[example.py](https://github.com/SleepyStew/gptconnect/blob/master/example.py)
+[example-simple.py](https://github.com/SleepyStew/gptconnect/blob/master/example-simple.py)
+[example-advanced.py](https://github.com/SleepyStew/gptconnect/blob/master/example-advanced.py)
```

### Comparing `GPTConnect-0.1.9/gptconnect/gptconnect.py` & `GPTConnect-0.2.1/gptconnect/gptconnect.py`

 * *Files identical despite different names*

### Comparing `GPTConnect-0.1.9/gptconnect/gptfunction.py` & `GPTConnect-0.2.1/gptconnect/gptfunction.py`

 * *Files identical despite different names*

