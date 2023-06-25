# Comparing `tmp/pxutil-0.0.8.tar.gz` & `tmp/pxutil-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pxutil-0.0.8.tar", last modified: Tue Dec  7 02:56:33 2021, max compression
+gzip compressed data, was "dist/pxutil-0.0.9.tar", last modified: Wed Dec 22 09:06:35 2021, max compression
```

## Comparing `pxutil-0.0.8.tar` & `pxutil-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:56:33.000000 pxutil-0.0.8/
--rw-r--r--   0 root         (0) root         (0)     1073 2019-12-02 19:26:43.000000 pxutil-0.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2055 2021-12-07 02:56:33.000000 pxutil-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      783 2020-08-08 08:52:36.000000 pxutil-0.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:56:33.000000 pxutil-0.0.8/pxutil/
--rw-r--r--   0 root         (0) root         (0)      394 2021-06-12 12:11:50.000000 pxutil-0.0.8/pxutil/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8000 2021-12-07 02:55:22.000000 pxutil-0.0.8/pxutil/pxutil.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:56:33.000000 pxutil-0.0.8/pxutil.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2055 2021-12-07 02:56:32.000000 pxutil-0.0.8/pxutil.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      222 2021-12-07 02:56:33.000000 pxutil-0.0.8/pxutil.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-07 02:56:32.000000 pxutil-0.0.8/pxutil.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2021-12-07 02:56:32.000000 pxutil-0.0.8/pxutil.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-07 02:56:33.000000 pxutil-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1134 2021-12-07 02:54:41.000000 pxutil-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-07 02:56:33.000000 pxutil-0.0.8/tests/
--rw-r--r--   0 root         (0) root         (0)       48 2020-05-24 02:58:28.000000 pxutil-0.0.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1446 2021-06-12 12:10:43.000000 pxutil-0.0.8/tests/test_pxutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 09:06:35.000000 pxutil-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)     1073 2019-12-02 19:26:43.000000 pxutil-0.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2091 2021-12-22 09:06:35.000000 pxutil-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      785 2021-12-22 09:06:06.000000 pxutil-0.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil/
+-rw-r--r--   0 root         (0) root         (0)      394 2021-06-12 12:11:50.000000 pxutil-0.0.9/pxutil/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8353 2021-12-22 08:06:12.000000 pxutil-0.0.9/pxutil/pxutil.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2091 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      222 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2021-12-22 09:06:35.000000 pxutil-0.0.9/pxutil.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-12-22 09:06:35.000000 pxutil-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1183 2021-12-22 09:04:50.000000 pxutil-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-22 09:06:35.000000 pxutil-0.0.9/tests/
+-rw-r--r--   0 root         (0) root         (0)       48 2020-05-24 02:58:28.000000 pxutil-0.0.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2021-12-22 08:46:23.000000 pxutil-0.0.9/tests/test_pxutil.py
```

### Comparing `pxutil-0.0.8/LICENSE` & `pxutil-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pxutil-0.0.8/PKG-INFO` & `pxutil-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pxutil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Some handy Python utilities
 Home-page: https://github.com/peterjpxie/pxutil.git
 Author: Peter Jiping Xie
 Author-email: peter.jp.xie@gmail.com
 License: MIT
 Description: pxutil
         ======
@@ -21,17 +21,15 @@
         or 
         
         pip install .
         
         Build distributions (source and binary wheel)
         =============================================
         
-        rm -rf dist/*
-        
-        python setup.py sdist bdist_wheel
+        rm -rf dist/* && python setup.py sdist bdist_wheel
         
         Publish to pypi
         ===============
         
         twine upload dist/*
         
         Usage
@@ -74,9 +72,10 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5
```

### Comparing `pxutil-0.0.8/README.rst` & `pxutil-0.0.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 or 
 
 pip install .
 
 Build distributions (source and binary wheel)
 =============================================
 
-rm -rf dist/*
-
-python setup.py sdist bdist_wheel
+rm -rf dist/* && python setup.py sdist bdist_wheel
 
 Publish to pypi
 ===============
 
 twine upload dist/*
 
 Usage
```

### Comparing `pxutil-0.0.8/pxutil/pxutil.py` & `pxutil-0.0.9/pxutil/pxutil.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,40 +63,51 @@
         # Alternately can call Popen directly, but it will return stderr, stdout as bytes and need to decode first. Don't bother, just upgrade Python version.
         """ Example
         p = Popen(cmd, shell=True, stdout=PIPE, stderr=PIPE)
         stdout, stderr = p.communicate()
         code = p.returncode
         """
 
-def bashx(cmd):
+def bashx(cmd, x=True, e=False):
     """    
-    run system cmd like sh -x
+    run system cmd like bash -x
     
     Print the cmd with + prefix before executing
     Don't capture the output or error 
     
-    cmd: string 
+    Arguments
+    ---------
+    cmd: string - command to run
+    x: When True, print the command with prefix + like shell 'bash -x' before running it 
+    e: When True, exit the python program when returncode is not 0, like shell 'bash -e'.
+    
     return: CompletedProcess object with only returncode.
     
     Usage example: 
     ret = shx('ls')
     print(ret.returncode)
     
     Warning of using shell=True: https://docs.python.org/3/library/subprocess.html#security-considerations
     """
     from subprocess import run # CompletedProcess
     import sys
-    import locale
 
     if sys.version_info >= (
         3,
         5,
     ):  # version_info is actually a tuple, so compare with a tuple
-        print('+ %s' % cmd)
-        return run(cmd, shell=True)
+        if x:
+            print('+ %s' % cmd)
+
+        ret=run(cmd, shell=True)
+        
+        if e and ret.returncode !=0:
+            sys.exit(1)
+        else:
+            return ret
     else:
         raise Exception("Require python 3.5 or above.")
 
 def trim_docstring(docstring):
     """
     Trim leading indents, leading and trailing blank lines from multiple liner using triple quote like docstring.
```

### Comparing `pxutil-0.0.8/pxutil.egg-info/PKG-INFO` & `pxutil-0.0.9/pxutil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: pxutil
-Version: 0.0.8
+Version: 0.0.9
 Summary: Some handy Python utilities
 Home-page: https://github.com/peterjpxie/pxutil.git
 Author: Peter Jiping Xie
 Author-email: peter.jp.xie@gmail.com
 License: MIT
 Description: pxutil
         ======
@@ -21,17 +21,15 @@
         or 
         
         pip install .
         
         Build distributions (source and binary wheel)
         =============================================
         
-        rm -rf dist/*
-        
-        python setup.py sdist bdist_wheel
+        rm -rf dist/* && python setup.py sdist bdist_wheel
         
         Publish to pypi
         ===============
         
         twine upload dist/*
         
         Usage
@@ -74,9 +72,10 @@
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.5
```

### Comparing `pxutil-0.0.8/setup.py` & `pxutil-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst") as readme:
     long_description = readme.read()
     print(long_description)
 
 setup(
     name="pxutil",
-    version="0.0.8",
+    version="0.0.9",
     description="Some handy Python utilities",
     long_description=long_description,
     # long_description_content_type="text/markdown", # default is rst
     author="Peter Jiping Xie",
     author_email="peter.jp.xie@gmail.com",
     url="https://github.com/peterjpxie/pxutil.git",
     license="MIT",
@@ -25,10 +25,11 @@
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

### Comparing `pxutil-0.0.8/tests/test_pxutil.py` & `pxutil-0.0.9/tests/test_pxutil.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,24 +3,48 @@
 For pytest to support importing local modules, must create a __init__.py file to indicate it is a package.
 """
 # Note: relative imports must use this syntax: from <> import <>
 # from ..pxutil import bash, grep, trim_docstring
 # Somehow direct import works with magic with pytest, even without tox or install pxutil as a system package.
 # Not sure how it works exactly, rename __init__.py and setup.py from parent folder but it still works.
 import pxutil as px
-
+import pytest
 
 def test_bash():
-    ret = px.bash("ls")
+    ret = px.bash("pwd")
     assert ret.returncode == 0
 
 def test_bashx():
-    ret = px.bashx("ls")
+    cmd = 'pwd'
+    ret = px.bashx(cmd)
+    assert ret.returncode == 0
+    
+    ## test x=False
+    import io
+    import sys
+
+    capturedOutput = io.StringIO()   # Create StringIO object
+    sys.stdout = capturedOutput      # and redirect stdout.
+
+    ret = px.bashx(cmd, x=False)   # capture stdout of print
+    standard_output = capturedOutput.getvalue()
+    
+    sys.stdout = sys.__stdout__      # Reset redirect.
+    assert ('+ %s' % cmd) not in standard_output
     assert ret.returncode == 0
 
+    ## test e=True
+    # Ref: https://docs.pytest.org/en/6.2.x/assert.html#assertions-about-expected-exceptions
+    cmd = 'ls not_exit'
+    # Capture SystemExit exception raised by sys.exit
+    with pytest.raises(SystemExit) as excinfo:
+        px.bashx(cmd, e=True)
+
+    assert excinfo.type == SystemExit
+
 def test_grep():
     ret = px.grep("de", "abc\ndef")
     assert ret == ["def"]
 
 def test_trim_docstring():
     ret = px.trim_docstring(
         """
```

