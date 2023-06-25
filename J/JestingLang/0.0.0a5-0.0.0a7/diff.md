# Comparing `tmp/JestingLang-0.0.0a5.tar.gz` & `tmp/JestingLang-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JestingLang-0.0.0a5.tar", last modified: Thu Jun  8 13:53:00 2023, max compression
+gzip compressed data, was "JestingLang-0.0.0a7.tar", last modified: Sun Jun 25 11:52:14 2023, max compression
```

## Comparing `JestingLang-0.0.0a5.tar` & `JestingLang-0.0.0a7.tar`

### file list

```diff
@@ -1,40 +1,57 @@
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:53:00.159461 JestingLang-0.0.0a5/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a5/LICENSE
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-08 13:53:00.166579 JestingLang-0.0.0a5/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2096 2023-06-08 13:25:42.000000 JestingLang-0.0.0a5/README.md
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-08 13:53:00.176799 JestingLang-0.0.0a5/setup.cfg
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1274 2023-06-08 13:26:44.000000 JestingLang-0.0.0a5/setup.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.136732 JestingLang-0.0.0a5/src/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.440333 JestingLang-0.0.0a5/src/JestingLang/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.000300 JestingLang-0.0.0a5/src/JestingLang/JParsing/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4326 2023-06-08 13:15:01.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/JestingAST.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5221 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     9898 2023-05-15 07:17:19.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser_cachedParseTable.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a5/src/JestingLang/JParsing/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.356833 JestingLang-0.0.0a5/src/JestingLang/JVisitors/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      816 2023-05-28 16:16:17.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/AbstractJestingVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1371 2023-06-08 12:33:56.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2998 2023-06-08 13:07:54.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2588 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/PrettyPrintingVisitors.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a5/src/JestingLang/JVisitors/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.426563 JestingLang-0.0.0a5/src/JestingLang/Misc/
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.759865 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      243 2023-06-08 08:56:27.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/AbstractContext.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1291 2023-05-28 16:06:05.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MapContext.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1403 2023-06-08 12:42:00.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MemoryContext.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:59.836713 JestingLang-0.0.0a5/src/JestingLang/Misc/JExample/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JExample/__init__.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:53:00.086793 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1430 2023-06-08 11:18:42.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/LogicFunctions.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2629 2023-06-08 13:12:55.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/OperationMapping.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a5/src/JestingLang/Misc/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a5/src/JestingLang/__init__.py
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2702 2023-05-27 13:58:43.000000 JestingLang-0.0.0a5/src/JestingLang/main.py
-drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-08 13:52:58.716675 JestingLang-0.0.0a5/src/JestingLang.egg-info/
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/PKG-INFO
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1107 2023-06-08 13:52:58.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/SOURCES.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/dependency_links.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/requires.txt
--rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-08 13:52:57.000000 JestingLang-0.0.0a5/src/JestingLang.egg-info/top_level.txt
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.430865 JestingLang-0.0.0a7/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1085 2023-05-09 15:44:29.000000 JestingLang-0.0.0a7/LICENSE
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-25 11:52:14.430865 JestingLang-0.0.0a7/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     5048 2023-06-24 06:31:03.000000 JestingLang-0.0.0a7/README.md
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      103 2023-06-25 11:52:14.446556 JestingLang-0.0.0a7/setup.cfg
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1564 2023-06-25 11:51:20.000000 JestingLang-0.0.0a7/setup.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.391610 JestingLang-0.0.0a7/src/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.731538 JestingLang-0.0.0a7/src/JestingLang/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.951585 JestingLang-0.0.0a7/src/JestingLang/Core/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.219187 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      338 2023-06-17 12:27:43.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/AbstractDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1962 2023-06-23 14:00:27.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedCellDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1097 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/CachedDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1311 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.329064 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4766 2023-06-22 15:16:12.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/JestingAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.596683 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1458 2023-06-11 13:16:25.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/AbstractJestingVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1528 2023-06-19 14:48:18.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3014 2023-06-24 03:02:41.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2593 2023-06-17 13:10:33.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 12:31:05.000000 JestingLang-0.0.0a7/src/JestingLang/Core/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.643602 JestingLang-0.0.0a7/src/JestingLang/JestingScript/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.801075 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      660 2023-06-21 14:08:54.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/AbstractScriptDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     4913 2023-06-23 14:12:13.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/ScriptDereferencer.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:20:09.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JDereferencer/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:13.910500 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2150 2023-06-21 14:08:54.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/JestingScriptAST.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-25 16:59:49.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JParsing/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.021545 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3340 2023-06-21 14:23:12.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/ScriptInterpreterVisitor.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 07:17:36.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/JVisitors/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-17 13:09:13.000000 JestingLang-0.0.0a7/src/JestingLang/JestingScript/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    13162 2023-06-23 13:58:27.000000 JestingLang-0.0.0a7/src/JestingLang/LexerParser.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)    11414 2023-06-23 14:12:21.000000 JestingLang-0.0.0a7/src/JestingLang/LexerParser_cachedParseTable.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.068786 JestingLang-0.0.0a7/src/JestingLang/Misc/
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.226034 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2082 2023-06-23 13:58:27.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/LogicFunctions.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     2919 2023-06-22 15:28:50.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/OperationMapping.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:01:19.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/__init__.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:14.396830 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      688 2023-06-17 13:17:53.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/DereferencerHelper.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      349 2023-06-18 00:00:43.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/LexerParserHelpers.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 14:14:47.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/JTesting/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-22 12:31:24.000000 JestingLang-0.0.0a7/src/JestingLang/Misc/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-05-15 06:05:46.000000 JestingLang-0.0.0a7/src/JestingLang/__init__.py
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     3037 2023-06-17 13:52:56.000000 JestingLang-0.0.0a7/src/JestingLang/main.py
+drwxrwxrwx   0 nacho     (1000) nacho     (1000)        0 2023-06-25 11:52:12.904662 JestingLang-0.0.0a7/src/JestingLang.egg-info/
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)      937 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/PKG-INFO
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)     1830 2023-06-25 11:52:12.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/SOURCES.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        1 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/dependency_links.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)        4 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/requires.txt
+-rwxrwxrwx   0 nacho     (1000) nacho     (1000)       12 2023-06-25 11:52:11.000000 JestingLang-0.0.0a7/src/JestingLang.egg-info/top_level.txt
```

### Comparing `JestingLang-0.0.0a5/LICENSE` & `JestingLang-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `JestingLang-0.0.0a5/PKG-INFO` & `JestingLang-0.0.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a5
+Version: 0.0.0a7
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `JestingLang-0.0.0a5/setup.py` & `JestingLang-0.0.0a7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from setuptools import setup
 
 setup(
     name='JestingLang',
-    version='0.0.0a5',
+    version='0.0.0a7',
     author='itrufat',
     description='A compiler for the minimalist spreadsheet language Jesting',
     long_description='A compiler + a few node navigators (including an interpreter) for a minimalist language intended to copy the most basic functionalities found in spreadsheet-applications called JestingLang. It was created to be used with Jesting, a spreadsheet terminal tool.',
     long_description_content_type='text/markdown',
     url='https://github.com/itruffat/JestingLang',
-    packages=['JestingLang', 'JestingLang.JParsing', 'JestingLang.JVisitors', 'JestingLang.Misc',
-              'JestingLang.Misc.JLogic', 'JestingLang.Misc.JContext', 'JestingLang.Misc.JExample'],
+    packages=['JestingLang',
+              'JestingLang.Core',
+                  'JestingLang.Core.JParsing', 'JestingLang.Core.JVisitors', 'JestingLang.Core.JDereferencer',
+              'JestingLang.JestingScript',
+                  'JestingLang.JestingScript.JParsing', 'JestingLang.JestingScript.JVisitors',
+                  'JestingLang.JestingScript.JDereferencer',
+              'JestingLang.Misc',
+                  'JestingLang.Misc.JLogic', 'JestingLang.Misc.JTesting'],
     package_dir={'': 'src'},
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/JParsing/JestingAST.py` & `JestingLang-0.0.0a7/src/JestingLang/Core/JParsing/JestingAST.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from abc import ABC, abstractmethod
 
-operations = {"+","-","*","/","&","=",'>','NOT','AND','OR', "u-"}
+operations = {"+","-","*","/","&","=",'>','NOT','AND','OR', "u-", 'MOD'}
 
 class Node(ABC):
     def __init__(self):
         self.children = {}
 
     @abstractmethod
     def accept(self, visitor):
         pass
 
     @abstractmethod
     def volatile(self):
         pass
 
-
 class SimpleValueNode(Node, ABC):
     def __init__(self, value):
         super().__init__()
+        self.name = ""
         self.value = value
 
     def accept(self, visitor):
         return visitor.visitSimple(self)
 
+    #def __str__(self):
+        #return f"{self.name}:{str(self.value)}"
+
 
 class EmptyValueNode(SimpleValueNode):
     def __init__(self):
+        self.name = "empty"
         super().__init__(None)
 
     def accept(self, visitor):
         child = visitor.visitEmpty(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
@@ -53,67 +57,73 @@
     def isNA(self):
         return True
 
 
 class InvalidValueNode(SimpleValueNode):
 
     def __init__(self, value):
+        self.name = "INVALID"
         super().__init__(NAError() if value == "#NA" else InnerError(value))
 
     def accept(self, visitor):
         child = visitor.visitInvalid(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return not self.value.isNA()
 
 
 class StrValueNode(SimpleValueNode):
 
     def accept(self, visitor):
+        self.name = "str"
         child = visitor.visitStr(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return False
 
 
 class IntValueNode(SimpleValueNode):
 
     def accept(self, visitor):
+        self.name = "Integer"
         child = visitor.visitInt(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return False
 
 
 class BoolValueNode(SimpleValueNode):
 
     def accept(self, visitor):
+        self.name = "Boolean"
         child = visitor.visitBool(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return False
 
 
 class DateValueNode(SimpleValueNode):
 
     def accept(self, visitor):
+        self.name = "Date"
         child = visitor.visitDate(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return False
 
 
 class ReferenceValueNode(SimpleValueNode):
 
     def accept(self, visitor):
+        self.name = "Ref"
         child = visitor.visitRef(self)
         return super().accept(visitor) if child is None else child
 
     def volatile(self):
         return True
 
 class OperationNode(Node):
@@ -125,14 +135,17 @@
 
     def accept(self, visitor):
         return visitor.visitOperation(self)
 
     def volatile(self):
         return any(map(lambda c: c.volatile(), self.children.values()))
 
+    #def __str__(self):
+        #return f"Operation({str(self.operation)}):{','.join(map(lambda x:str(x), self.children))}"
+
 
 class IfNode(Node):
     def __init__(self, _if, _then, _else):
         super().__init__()
         self.children = {0: _if, 1: _then, 2: _else}
 
     def accept(self, visitor):
@@ -171,8 +184,8 @@
         self.value = value
         self.error_msg = error_msg
 
     def volatile(self):
         return False
 
     def accept(self, visitor):
-        return visitor.visitToleratedError(self)
+        return visitor.visitToleratedError(self)
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/JParsing/LexerParser_cachedParseTable.py` & `JestingLang-0.0.0a7/src/JestingLang/LexerParser_cachedParseTable.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,55 +2,58 @@
 # LexerParser_cachedParseTable.py
 # This file is automatically generated. Do not edit.
 # pylint: disable=W,C,R
 _tabversion = '3.10'
 
 _lr_method = 'LALR'
 
-_lr_signature = 'nonassocEQUALSleftPLUSMINUSAMPERSANDleftTIMESDIVIDErightUMINUSAMPERSAND AND BIGGER BOOLEAN CELL_ADDRESS COMMA DIVIDE EQUALS IF INDIRECT LPAREN MINUS NOT NUMBER OR PLUS RPAREN SMALLER STRING TEXT TIMESstatement    : parameter\n                    | callable_operation\n                    | fixed_operation\n    callable_operation   : IF LPAREN statement COMMA  statement COMMA statement RPAREN\n                            | NOT LPAREN statement RPAREN\n                            | AND LPAREN statement COMMA statement RPAREN\n                            | OR LPAREN statement COMMA statement RPAREN\n                            | INDIRECT LPAREN statement RPAREN statement    :  LPAREN statement RPAREN fixed_operation  : statement EQUALS statement\n                        | statement AMPERSAND statement\n                        | statement PLUS statement\n                        | statement MINUS statement\n                        | statement TIMES statement\n                        | statement DIVIDE statement\n                        | statement SMALLER BIGGER statement\n                        | statement BIGGER statement\n                        | statement SMALLER statement\n                        | statement BIGGER EQUALS statement\n                        | statement SMALLER EQUALS statement\n                        | MINUS statement %prec UMINUS parameter    : NUMBERparameter    : STRINGparameter    : CELL_ADDRESSparameter    : BOOLEANparameter     : TEXT'
+_lr_signature = 'nonassocEQUALSleftPLUSMINUSAMPERSANDleftTIMESDIVIDErightUMINUSAMPERSAND AND BIGGER BOOLEAN CELL_ADDRESS COMMA DIVIDE EQUALS IF INDIRECT LPAREN MINUS MOD NOT NUMBER OR PLUS RPAREN SMALLER STRING TEXT TIMESstatement    : parameter\n                            | callable_operation\n                            | fixed_operation\n            callable_operation   : IF LPAREN statement COMMA  statement COMMA statement RPAREN\n                                    | NOT LPAREN statement RPAREN\n                                    | AND LPAREN statement COMMA statement RPAREN\n                                    | OR LPAREN statement COMMA statement RPAREN\n                                    | INDIRECT LPAREN statement RPAREN\n                                    | TEXT LPAREN statement RPAREN\n                                    | TEXT LPAREN statement COMMA statement RPAREN\n                                    | TEXT LPAREN statement COMMA statement COMMA statement RPAREN statement    :  LPAREN statement RPAREN fixed_operation  : statement EQUALS statement\n                                | statement AMPERSAND statement\n                                | statement PLUS statement\n                                | statement MINUS statement\n                                | statement TIMES statement\n                                | statement DIVIDE statement\n                                | statement SMALLER BIGGER statement\n                                | statement BIGGER statement\n                                | statement SMALLER statement\n                                | statement BIGGER EQUALS statement\n                                | statement SMALLER EQUALS statement\n                                | MINUS statement %prec UMINUS parameter    : NUMBERparameter    : STRINGparameter    : CELL_ADDRESSparameter    : BOOLEANstatement     : TEXT'
     
-_lr_action_items = {'LPAREN':([0,5,11,12,13,14,15,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[5,5,26,27,28,29,30,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,]),'NUMBER':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,]),'STRING':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,]),'CELL_ADDRESS':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,]),'BOOLEAN':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,]),'TEXT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,]),'IF':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,]),'NOT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,]),'AND':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,]),'OR':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,]),'INDIRECT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,]),'MINUS':([0,1,2,3,4,5,6,7,8,9,10,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,],[16,20,-1,-2,-3,16,-22,-23,-24,-25,-26,16,16,16,16,16,16,16,16,16,20,16,16,16,16,16,-21,20,-11,-12,-13,-14,-15,20,16,16,20,16,-9,20,20,20,20,20,20,20,20,16,-5,16,16,-8,20,20,20,16,-6,-7,20,-4,]),'$end':([1,2,3,4,6,7,8,9,10,31,32,33,34,35,36,37,38,41,43,49,50,51,53,56,61,62,64,],[0,-1,-2,-3,-22,-23,-24,-25,-26,-21,-10,-11,-12,-13,-14,-15,-18,-17,-9,-16,-20,-19,-5,-8,-6,-7,-4,]),'EQUALS':([1,2,3,4,6,7,8,9,10,23,24,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[17,-1,-2,-3,-22,-23,-24,-25,-26,40,42,17,-21,None,-11,-12,-13,-14,-15,17,17,-9,17,17,17,17,17,17,None,None,-5,-8,17,17,17,-6,-7,17,-4,]),'AMPERSAND':([1,2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[18,-1,-2,-3,-22,-23,-24,-25,-26,18,-21,18,-11,-12,-13,-14,-15,18,18,-9,18,18,18,18,18,18,18,18,-5,-8,18,18,18,-6,-7,18,-4,]),'PLUS':([1,2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[19,-1,-2,-3,-22,-23,-24,-25,-26,19,-21,19,-11,-12,-13,-14,-15,19,19,-9,19,19,19,19,19,19,19,19,-5,-8,19,19,19,-6,-7,19,-4,]),'TIMES':([1,2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[21,-1,-2,-3,-22,-23,-24,-25,-26,21,-21,21,21,21,21,-14,-15,21,21,-9,21,21,21,21,21,21,21,21,-5,-8,21,21,21,-6,-7,21,-4,]),'DIVIDE':([1,2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[22,-1,-2,-3,-22,-23,-24,-25,-26,22,-21,22,22,22,22,-14,-15,22,22,-9,22,22,22,22,22,22,22,22,-5,-8,22,22,22,-6,-7,22,-4,]),'SMALLER':([1,2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[23,-1,-2,-3,-22,-23,-24,-25,-26,23,-21,-10,-11,-12,-13,-14,-15,23,23,-9,23,23,23,23,23,23,-20,-19,-5,-8,23,23,23,-6,-7,23,-4,]),'BIGGER':([1,2,3,4,6,7,8,9,10,23,25,31,32,33,34,35,36,37,38,41,43,44,45,46,47,48,49,50,51,53,56,57,58,59,61,62,63,64,],[24,-1,-2,-3,-22,-23,-24,-25,-26,39,24,-21,-10,-11,-12,-13,-14,-15,24,24,-9,24,24,24,24,24,24,-20,-19,-5,-8,24,24,24,-6,-7,24,-4,]),'RPAREN':([2,3,4,6,7,8,9,10,25,31,32,33,34,35,36,37,38,41,43,45,48,49,50,51,53,56,58,59,61,62,63,64,],[-1,-2,-3,-22,-23,-24,-25,-26,43,-21,-10,-11,-12,-13,-14,-15,-18,-17,-9,53,56,-16,-20,-19,-5,-8,61,62,-6,-7,64,-4,]),'COMMA':([2,3,4,6,7,8,9,10,31,32,33,34,35,36,37,38,41,43,44,46,47,49,50,51,53,56,57,61,62,64,],[-1,-2,-3,-22,-23,-24,-25,-26,-21,-10,-11,-12,-13,-14,-15,-18,-17,-9,52,54,55,-16,-20,-19,-5,-8,60,-6,-7,-4,]),}
+_lr_action_items = {'LPAREN':([0,5,6,11,12,13,14,15,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[5,5,26,27,28,29,30,31,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,5,]),'TEXT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,6,]),'NUMBER':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,7,]),'STRING':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,8,]),'CELL_ADDRESS':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,9,]),'BOOLEAN':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,10,]),'IF':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,11,]),'NOT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,12,]),'AND':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,13,]),'OR':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,14,]),'INDIRECT':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,15,]),'MINUS':([0,1,2,3,4,5,6,7,8,9,10,16,17,18,19,20,21,22,23,24,25,26,27,28,29,30,31,32,33,34,35,36,37,38,39,40,41,42,43,44,45,46,47,48,49,50,51,52,53,54,55,56,57,58,59,60,61,62,63,64,65,66,67,68,69,70,71,72,73,],[16,20,-1,-2,-3,16,-29,-25,-26,-27,-28,16,16,16,16,16,16,16,16,16,20,16,16,16,16,16,16,-24,20,-14,-15,-16,-17,-18,20,16,16,20,16,-12,20,20,20,20,20,20,20,20,20,-9,16,16,-5,16,16,-8,20,20,20,20,16,-10,16,-6,-7,20,20,-11,-4,]),'$end':([1,2,3,4,6,7,8,9,10,32,33,34,35,36,37,38,39,42,44,51,52,53,54,57,60,66,68,69,72,73,],[0,-1,-2,-3,-29,-25,-26,-27,-28,-24,-13,-14,-15,-16,-17,-18,-21,-20,-12,-19,-23,-22,-9,-5,-8,-10,-6,-7,-11,-4,]),'EQUALS':([1,2,3,4,6,7,8,9,10,23,24,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[17,-1,-2,-3,-29,-25,-26,-27,-28,41,43,17,-24,None,-14,-15,-16,-17,-18,17,17,-12,17,17,17,17,17,17,17,None,None,-9,-5,-8,17,17,17,17,-10,-6,-7,17,17,-11,-4,]),'AMPERSAND':([1,2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[18,-1,-2,-3,-29,-25,-26,-27,-28,18,-24,18,-14,-15,-16,-17,-18,18,18,-12,18,18,18,18,18,18,18,18,18,-9,-5,-8,18,18,18,18,-10,-6,-7,18,18,-11,-4,]),'PLUS':([1,2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[19,-1,-2,-3,-29,-25,-26,-27,-28,19,-24,19,-14,-15,-16,-17,-18,19,19,-12,19,19,19,19,19,19,19,19,19,-9,-5,-8,19,19,19,19,-10,-6,-7,19,19,-11,-4,]),'TIMES':([1,2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[21,-1,-2,-3,-29,-25,-26,-27,-28,21,-24,21,21,21,21,-17,-18,21,21,-12,21,21,21,21,21,21,21,21,21,-9,-5,-8,21,21,21,21,-10,-6,-7,21,21,-11,-4,]),'DIVIDE':([1,2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[22,-1,-2,-3,-29,-25,-26,-27,-28,22,-24,22,22,22,22,-17,-18,22,22,-12,22,22,22,22,22,22,22,22,22,-9,-5,-8,22,22,22,22,-10,-6,-7,22,22,-11,-4,]),'SMALLER':([1,2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[23,-1,-2,-3,-29,-25,-26,-27,-28,23,-24,-13,-14,-15,-16,-17,-18,23,23,-12,23,23,23,23,23,23,23,-23,-22,-9,-5,-8,23,23,23,23,-10,-6,-7,23,23,-11,-4,]),'BIGGER':([1,2,3,4,6,7,8,9,10,23,25,32,33,34,35,36,37,38,39,42,44,45,46,47,48,49,50,51,52,53,54,57,60,61,62,63,64,66,68,69,70,71,72,73,],[24,-1,-2,-3,-29,-25,-26,-27,-28,40,24,-24,-13,-14,-15,-16,-17,-18,24,24,-12,24,24,24,24,24,24,24,-23,-22,-9,-5,-8,24,24,24,24,-10,-6,-7,24,24,-11,-4,]),'RPAREN':([2,3,4,6,7,8,9,10,25,32,33,34,35,36,37,38,39,42,44,45,47,50,51,52,53,54,57,60,61,63,64,66,68,69,70,71,72,73,],[-1,-2,-3,-29,-25,-26,-27,-28,44,-24,-13,-14,-15,-16,-17,-18,-21,-20,-12,54,57,60,-19,-23,-22,-9,-5,-8,66,68,69,-10,-6,-7,72,73,-11,-4,]),'COMMA':([2,3,4,6,7,8,9,10,32,33,34,35,36,37,38,39,42,44,45,46,48,49,51,52,53,54,57,60,61,62,66,68,69,72,73,],[-1,-2,-3,-29,-25,-26,-27,-28,-24,-13,-14,-15,-16,-17,-18,-21,-20,-12,55,56,58,59,-19,-23,-22,-9,-5,-8,65,67,-10,-6,-7,-11,-4,]),}
 
 _lr_action = {}
 for _k, _v in _lr_action_items.items():
    for _x,_y in zip(_v[0],_v[1]):
       if not _x in _lr_action:  _lr_action[_x] = {}
       _lr_action[_x][_k] = _y
 del _lr_action_items
 
-_lr_goto_items = {'statement':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[1,25,31,32,33,34,35,36,37,38,41,44,45,46,47,48,49,50,51,57,58,59,63,]),'parameter':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,]),'callable_operation':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,]),'fixed_operation':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,39,40,42,52,54,55,60,],[4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,]),}
+_lr_goto_items = {'statement':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[1,25,32,33,34,35,36,37,38,39,42,45,46,47,48,49,50,51,52,53,61,62,63,64,70,71,]),'parameter':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,2,]),'callable_operation':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,3,]),'fixed_operation':([0,5,16,17,18,19,20,21,22,23,24,26,27,28,29,30,31,40,41,43,55,56,58,59,65,67,],[4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,4,]),}
 
 _lr_goto = {}
 for _k, _v in _lr_goto_items.items():
    for _x, _y in zip(_v[0], _v[1]):
        if not _x in _lr_goto: _lr_goto[_x] = {}
        _lr_goto[_x][_k] = _y
 del _lr_goto_items
 _lr_productions = [
   ("S' -> statement","S'",1,None,None,None),
-  ('statement -> parameter','statement',1,'p_statement','LexerParser.py',85),
-  ('statement -> callable_operation','statement',1,'p_statement','LexerParser.py',86),
-  ('statement -> fixed_operation','statement',1,'p_statement','LexerParser.py',87),
-  ('callable_operation -> IF LPAREN statement COMMA statement COMMA statement RPAREN','callable_operation',8,'p_callable_opereation','LexerParser.py',93),
-  ('callable_operation -> NOT LPAREN statement RPAREN','callable_operation',4,'p_callable_opereation','LexerParser.py',94),
-  ('callable_operation -> AND LPAREN statement COMMA statement RPAREN','callable_operation',6,'p_callable_opereation','LexerParser.py',95),
-  ('callable_operation -> OR LPAREN statement COMMA statement RPAREN','callable_operation',6,'p_callable_opereation','LexerParser.py',96),
-  ('callable_operation -> INDIRECT LPAREN statement RPAREN','callable_operation',4,'p_callable_opereation','LexerParser.py',97),
-  ('statement -> LPAREN statement RPAREN','statement',3,'p_statement_paren','LexerParser.py',111),
-  ('fixed_operation -> statement EQUALS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',117),
-  ('fixed_operation -> statement AMPERSAND statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',118),
-  ('fixed_operation -> statement PLUS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',119),
-  ('fixed_operation -> statement MINUS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',120),
-  ('fixed_operation -> statement TIMES statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',121),
-  ('fixed_operation -> statement DIVIDE statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',122),
-  ('fixed_operation -> statement SMALLER BIGGER statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',123),
-  ('fixed_operation -> statement BIGGER statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',124),
-  ('fixed_operation -> statement SMALLER statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',125),
-  ('fixed_operation -> statement BIGGER EQUALS statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',126),
-  ('fixed_operation -> statement SMALLER EQUALS statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',127),
-  ('fixed_operation -> MINUS statement','fixed_operation',2,'p_fixed_operation','LexerParser.py',128),
-  ('parameter -> NUMBER','parameter',1,'p_parameter_int','LexerParser.py',153),
-  ('parameter -> STRING','parameter',1,'p_parameter_STR','LexerParser.py',159),
-  ('parameter -> CELL_ADDRESS','parameter',1,'p_parameter_ADDRESS','LexerParser.py',165),
-  ('parameter -> BOOLEAN','parameter',1,'p_parameter_BOOL','LexerParser.py',171),
-  ('parameter -> TEXT','parameter',1,'p_parameter_text','LexerParser.py',177),
+  ('statement -> parameter','statement',1,'p_statement','LexerParser.py',244),
+  ('statement -> callable_operation','statement',1,'p_statement','LexerParser.py',245),
+  ('statement -> fixed_operation','statement',1,'p_statement','LexerParser.py',246),
+  ('callable_operation -> IF LPAREN statement COMMA statement COMMA statement RPAREN','callable_operation',8,'p_callable_opereation','LexerParser.py',252),
+  ('callable_operation -> NOT LPAREN statement RPAREN','callable_operation',4,'p_callable_opereation','LexerParser.py',253),
+  ('callable_operation -> AND LPAREN statement COMMA statement RPAREN','callable_operation',6,'p_callable_opereation','LexerParser.py',254),
+  ('callable_operation -> OR LPAREN statement COMMA statement RPAREN','callable_operation',6,'p_callable_opereation','LexerParser.py',255),
+  ('callable_operation -> INDIRECT LPAREN statement RPAREN','callable_operation',4,'p_callable_opereation','LexerParser.py',256),
+  ('callable_operation -> TEXT LPAREN statement RPAREN','callable_operation',4,'p_callable_opereation','LexerParser.py',257),
+  ('callable_operation -> TEXT LPAREN statement COMMA statement RPAREN','callable_operation',6,'p_callable_opereation','LexerParser.py',258),
+  ('callable_operation -> TEXT LPAREN statement COMMA statement COMMA statement RPAREN','callable_operation',8,'p_callable_opereation','LexerParser.py',259),
+  ('statement -> LPAREN statement RPAREN','statement',3,'p_statement_paren','LexerParser.py',287),
+  ('fixed_operation -> statement EQUALS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',293),
+  ('fixed_operation -> statement AMPERSAND statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',294),
+  ('fixed_operation -> statement PLUS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',295),
+  ('fixed_operation -> statement MINUS statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',296),
+  ('fixed_operation -> statement TIMES statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',297),
+  ('fixed_operation -> statement DIVIDE statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',298),
+  ('fixed_operation -> statement SMALLER BIGGER statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',299),
+  ('fixed_operation -> statement BIGGER statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',300),
+  ('fixed_operation -> statement SMALLER statement','fixed_operation',3,'p_fixed_operation','LexerParser.py',301),
+  ('fixed_operation -> statement BIGGER EQUALS statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',302),
+  ('fixed_operation -> statement SMALLER EQUALS statement','fixed_operation',4,'p_fixed_operation','LexerParser.py',303),
+  ('fixed_operation -> MINUS statement','fixed_operation',2,'p_fixed_operation','LexerParser.py',304),
+  ('parameter -> NUMBER','parameter',1,'p_parameter_int','LexerParser.py',329),
+  ('parameter -> STRING','parameter',1,'p_parameter_STR','LexerParser.py',335),
+  ('parameter -> CELL_ADDRESS','parameter',1,'p_parameter_ADDRESS','LexerParser.py',341),
+  ('parameter -> BOOLEAN','parameter',1,'p_parameter_BOOL','LexerParser.py',347),
+  ('statement -> TEXT','statement',1,'p_text_parameter_text','LexerParser.py',353),
 ]
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextBoundInterpreterVisitor.py` & `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextBoundInterpreterVisitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
-from JestingLang.JParsing.JestingAST import InvalidValueNode, ReferenceValueNode, IndirectNode
+from JestingLang.Core.JParsing.JestingAST import InvalidValueNode, ReferenceValueNode, IndirectNode
 from JestingLang.Misc.JLogic.LogicFunctions import ref
-from JestingLang.JVisitors.ContextfreeInterpreterVisitor import ContextfreeInterpreterVisitor
+from JestingLang.Core.JDereferencer.AbstractDereferencer import AbstractDereferencer
+from JestingLang.Core.JVisitors.ContextfreeInterpreterVisitor import ContextfreeInterpreterVisitor
 
 
 class ContextBoundInterpreterVisitor(ContextfreeInterpreterVisitor):
 
     """The complete syntax resolver, it requires a reference resolver to get the references when visiting stuff"""
-    def __init__(self, context, resolveVolatile):
+    def __init__(self, dereferencer : AbstractDereferencer, resolveVolatile):
         super().__init__(resolveVolatile)
-        self.contextResolver = context
+        self.dereferencer = dereferencer
 
     def visitRef(self, node):
         if node.volatile and (not self.resolveVolatile):
             return node
-        referencedNode = self.contextResolver.resolve(node.value)
-        return InvalidValueNode("Broken reference") if referencedNode is None else referencedNode.accept(self)
+        referencedNode = self.dereferencer.resolveReference(node.value)
+        answer = InvalidValueNode("Broken reference") if referencedNode is None else referencedNode.accept(self)
+        return answer
 
     def visitIndirect(self, node):
         children_visited = node.children[0].accept(self)
         if (not self.resolveVolatile) and children_visited.volatile():
             return IndirectNode(children_visited)
         reference = ref(children_visited.value)
         if reference is None:
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/JVisitors/ContextfreeInterpreterVisitor.py` & `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/ContextfreeInterpreterVisitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from JestingLang.JParsing.JestingAST import IntValueNode, StrValueNode, ReferenceValueNode, BoolValueNode, \
+from JestingLang.Core.JParsing.JestingAST import IntValueNode, StrValueNode, ReferenceValueNode, BoolValueNode, \
                                               OperationNode, IfNode, InvalidValueNode, \
                                               ToleratedErrorNode
 from JestingLang.Misc.JLogic.LogicFunctions import boolean
-from JestingLang.JVisitors.AbstractJestingVisitor import AbstractJestingVisitor
+from JestingLang.Core.JVisitors.AbstractJestingVisitor import AbstractJestingVisitor
 from JestingLang.Misc.JLogic.OperationMapping import operations
 
 def renodify(value, label):
     if label == "INT":
         return IntValueNode(int(value))
     if label == "STR":
         return StrValueNode(str(value))
@@ -16,15 +16,15 @@
         return BoolValueNode(bool(value))
 
 
 class ContextfreeInterpreterVisitor(AbstractJestingVisitor):
 
     """The basic resolver for the syntax, does not depend on anything besides itself but can't resolve references"""
 
-    def __init__(self, resolveVolatile):
+    def __init__(self, resolveVolatile: bool):
         super().__init__()
         self.resolveVolatile = resolveVolatile
 
     def visit(self, node):
         return node.accept(self)
 
     def visitSimple(self, node):
@@ -47,15 +47,15 @@
         _if = node.children[0].accept(self)
 
         if not self.resolveVolatile and _if.volatile():
             _then = node.children[1].accept(self)
             _else = node.children[2].accept(self)
             answer = IfNode(_if, _then, _else)
         else:
-            # This behaviour is not real since spreedsheets don't use short-circuit (for whatever reason)
+            # This behaviour is not real since spreadsheets don't use short-circuit (for whatever reason)
             if boolean(_if.value):
                 # if boolean(_if.value) and (self.resolveVolatile or not _then.volatile()):
                 _then = node.children[1].accept(self)
                 answer = _then
             else:
                 # elif not boolean(_if.value) and (self.resolveVolatile or not _else.volatile()):
                 _else = node.children[2].accept(self)
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/JVisitors/PrettyPrintingVisitors.py` & `JestingLang-0.0.0a7/src/JestingLang/Core/JVisitors/PrettyPrintingVisitors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from JestingLang.JVisitors.AbstractJestingVisitor import AbstractJestingVisitor
+from JestingLang.Core.JVisitors.AbstractJestingVisitor import AbstractJestingVisitor
 
 
 class PrintingVisitor(AbstractJestingVisitor):
 
     def visit(self, node):
         print(node.accept(self))
         return None
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/Misc/JContext/MemoryContext.py` & `JestingLang-0.0.0a7/src/JestingLang/Core/JDereferencer/KeyValueDereferencer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from JestingLang.JParsing.JestingAST import SimpleValueNode, Node, StrValueNode, IntValueNode, EmptyValueNode
-from JestingLang.Misc.JContext.MapContext import MapContext
+from JestingLang.Core.JDereferencer.AbstractDereferencer import AbstractDereferencer
+from JestingLang.Core.JParsing.JestingAST import SimpleValueNode, Node
 
-class MemoryContext(MapContext):
-    """Example of a context, more similar to how a real spreadsheet would work.
-    Here an undefined reference returns empty value (which will later translate into '' ) and
-    iteration looks at memory instead of looking at the formula.
+
+class KeyValueDereferencer(AbstractDereferencer):
+    """Example of a deferencer, in this case by using a map for formulas respectively. (as simple as it gets)
+
+    This deferencer does not support circular recursion and will freeze when trying to solve it.
+    It also returns an error value if an unknown name is given.
     """
 
-    def __init__(self):
+    def __init__(self, memory=None):
         super().__init__()
-        self.memory = {}
-
-    def resolve(self, name):
-        if name not in self.memory.keys() or self.memory[name] is None:
-            return EmptyValueNode()
+        if memory is not None:
+            self.memory = memory
+        else:
+            self.memory = {}
+
+    def resolveReference(self, name):
+        if name not in self.memory.keys():
+            return None
         return self.memory[name]
 
+    def valueOf(self, node):
+        if issubclass(type(node), SimpleValueNode):
+            value = node.value
+        else:
+            value = node
+        return value
+
     def write(self, key, formula, value=None):
         assert(issubclass(type(formula), Node))
-        assert(value is None or issubclass(type(value), Node))
-        self.memory[key] = value
-        self.formulas[key] = formula
-
-    def writeNumber(self, key, value):
-        self.write(key, IntValueNode(value), IntValueNode(value))
-
-    def writeStr(self, key, value):
-        self.write(key, StrValueNode(value), StrValueNode(value))
-
-    def updateWith(self, function):
-        for key in sorted(self.formulas.keys()):
-            formula = self.formulas[key]
-            updated_value = function(formula, self)
-            self.write(key, formula, updated_value)
+        assert(value is None)
+        self.memory[key] =formula
+
+    def show(self):
+        _keys = set(self.memory.keys())
+        return {key: self.valueOf(self.resolveReference(key)) for key in _keys}
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/Misc/JLogic/OperationMapping.py` & `JestingLang-0.0.0a7/src/JestingLang/Misc/JLogic/OperationMapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from JestingLang.Misc.JLogic.LogicFunctions import variablesIntoIntegers
-from JestingLang.JParsing.JestingAST import operations as astOperations
+from JestingLang.Core.JParsing.JestingAST import operations as astOperations
 
 def operationPlus(variables):
     variables_int, errors = variablesIntoIntegers(variables, "Plus(+)")
     answer = 0
     if len(errors) == 0:
         answer = variables_int[0] + variables_int[1]
     return errors, answer, "INT"
@@ -33,14 +33,21 @@
     answer = 0
     if str(variables[1]) == "0":
         errors.append("Divided by zero")
     if len(errors) == 0:
         answer = variables_int[0] / variables_int[1]
     return errors, answer, "INT"
 
+def operationModulo(variables):
+    variables_int, errors = variablesIntoIntegers(variables, "Modulo(MOD)")
+    answer = 0
+    if len(errors) == 0:
+        answer = variables_int[0] % variables_int[1]
+    return errors, answer, "INT"
+
 def operationConcat(variables):
     return [], str(variables[0] if variables[0] is not None else '') + \
                str(variables[1] if variables[1] is not None else ''), "STR"
 
 
 def operationEquals(variables):
     print(variables)
@@ -55,14 +62,15 @@
 def operationBigger(variables):
     variables_int, errors = variablesIntoIntegers(variables, "Bigger(>)")
     answer = False
     if len(errors) == 0:
         answer = variables_int[0] > variables_int[1]
     return errors, answer, "BOOL"
 
+
 def operationNot(variables):
     return [], not(variables[0]), "BOOL"
 
 operations = {
                 "+": operationPlus,
                 "-": operationMinus,
                 "u-": operationMinus,
@@ -70,10 +78,11 @@
                 "/": operationDivide,
                 "&": operationConcat,
                 "=": operationEquals,
                 '>': operationBigger,
                 'NOT': operationNot,
                 'AND': operationAnd,
                 'OR': operationOr,
+                'MOD': operationModulo,
 }
 
 assert(astOperations == set(operations.keys()))
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang/main.py` & `JestingLang-0.0.0a7/src/JestingLang/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,54 @@
-from JestingLang.JParsing.LexerParser import lexer,parser
-from JestingLang.JVisitors.PrettyPrintingVisitors import PrintingVisitor, TreePrinter
-from JestingLang.JVisitors.ContextfreeInterpreterVisitor import ContextfreeInterpreterVisitor
-from JestingLang.JVisitors.ContextBoundInterpreterVisitor import ContextBoundInterpreterVisitor
-from JestingLang.Misc.JContext.MapContext import MapContext
-
-visitor_pointer = []
-
-
-def intoAST(line):
-    _line = line[1:]
-    lexer.input(_line)
-    _parsed_tree = parser.parse(_line)
-    return _parsed_tree
-
-
-def run(line, visitorp=visitor_pointer):
-    if len(visitorp) == 0:
-        visitorp.append(ContextBoundInterpreterVisitor(MapContext()))
-    if line[0] != "=":
-        return "INVALID LINE!"
-    _line = line[1:]
-    lexer.input(_line)
-    _parsed_tree = parser.parse(_line)
-    _visitor = visitorp[0]
-    return _visitor.visit(_parsed_tree), _parsed_tree
-
+from JestingLang.LexerParser import LexerParser
+from JestingLang.Core.JVisitors.PrettyPrintingVisitors import PrintingVisitor, TreePrinter
+from JestingLang.Core.JVisitors.ContextfreeInterpreterVisitor import ContextfreeInterpreterVisitor
+from JestingLang.Core.JVisitors.ContextBoundInterpreterVisitor import ContextBoundInterpreterVisitor
+from JestingLang.Core.JDereferencer.KeyValueDereferencer import KeyValueDereferencer
 
 if __name__ == "__main__":
 
+    lexerParser = LexerParser()
+    lexer = lexerParser.lexer
+    parser = lexerParser.parser
+
+    def intoAST(line):
+        _line = line[1:]
+        lexer.input(_line)
+        _parsed_tree = parser.parse(_line)
+        return _parsed_tree
+
+    visitor_pointer = []
+
+    def run(line, visitorp=visitor_pointer):
+        if len(visitorp) == 0:
+            visitorp.append(ContextBoundInterpreterVisitor(KeyValueDereferencer(), resolveVolatile=False))
+        if line[0] != "=":
+            return "INVALID LINE!"
+        _line = line[1:]
+        lexer.input(_line)
+        _parsed_tree = parser.parse(_line)
+        _visitor = visitorp[0]
+        return _visitor.visit(_parsed_tree), _parsed_tree
+
     print("Examples of visitors")
     print("--------------------")
 
     visitor1 = PrintingVisitor()
     visitor2 = TreePrinter()
-    visitor3 = ContextfreeInterpreterVisitor()
-    mapContext = MapContext()
-    visitor4 = ContextBoundInterpreterVisitor(mapContext)
+    visitor3 = ContextfreeInterpreterVisitor(resolveVolatile=False)
+    mapContext = KeyValueDereferencer()
+    visitor4 = ContextBoundInterpreterVisitor(mapContext, resolveVolatile=False)
 
     visitors = [visitor1, visitor2, visitor3, visitor4]
     visitors_names=["Printer", "TreePrinter", "ContextFree", "ContextBound"]
 
     response = None
     while response not in map(str, range(4)):
-        response = input("\n".join(["Pick a visitor:"] + ["  {}. {}".format(n,item) for n,item in enumerate(visitors_names)]+['']))
+        response = input("\n".join(["Pick a visitor:"] + ["  {}. {}".format(n,item)
+                                                          for n,item in enumerate(visitors_names)]+['']))
 
     _visitor=visitors[int(response)]
 
     while True:
         try:
             s = input('> ')
         except EOFError:
@@ -74,8 +76,8 @@
             if response == "3":
                 print(mapContext.show())
             else:
                 try:
                     value = tree.value
                     print(value)
                 except:
-                    print(tree)
+                    print(tree)
```

### Comparing `JestingLang-0.0.0a5/src/JestingLang.egg-info/PKG-INFO` & `JestingLang-0.0.0a7/src/JestingLang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JestingLang
-Version: 0.0.0a5
+Version: 0.0.0a7
 Summary: A compiler for the minimalist spreadsheet language Jesting
 Home-page: https://github.com/itruffat/JestingLang
 Author: itrufat
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

