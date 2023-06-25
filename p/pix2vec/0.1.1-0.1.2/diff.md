# Comparing `tmp/pix2vec-0.1.1.tar.gz` & `tmp/pix2vec-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pix2vec-0.1.1.tar", last modified: Fri Jun 23 19:47:44 2023, max compression
+gzip compressed data, was "dist/pix2vec-0.1.2.tar", last modified: Sun Jun 25 19:42:24 2023, max compression
```

## Comparing `pix2vec-0.1.1.tar` & `pix2vec-0.1.2.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/
--rw-r--r--   0 alf        (501) staff       (20)     5394 2023-06-23 19:47:44.000000 pix2vec-0.1.1/PKG-INFO
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/
--rw-r--r--   0 alf        (501) staff       (20)     5394 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/PKG-INFO
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.1/pix2vec.egg-info/not-zip-safe
--rw-r--r--   0 alf        (501) staff       (20)      818 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/SOURCES.txt
--rw-r--r--   0 alf        (501) staff       (20)       46 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/entry_points.txt
--rw-r--r--   0 alf        (501) staff       (20)        8 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/top_level.txt
--rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec.egg-info/dependency_links.txt
--rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.1/LICENSE
--rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.1/Makefile
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/tests/
--rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tests/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tests/test_pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.1/MANIFEST.in
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/
--rw-r--r--   0 alf        (501) staff       (20)      551 2023-06-22 16:49:30.000000 pix2vec-0.1.1/docs/index.rst
--rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/contributing.rst
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/images/
--rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.1/docs/images/m3cube-c.png
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.1/docs/images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/Makefile
--rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.1/docs/conf.py
--rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 19:26:42.000000 pix2vec-0.1.1/docs/modules.rst
--rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.1/docs/usage.rst
--rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/make.bat
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/_static/
--rw-r--r--   0 alf        (501) staff       (20)       90 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/plus.png
--rw-r--r--   0 alf        (501) staff       (20)      286 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/file.png
--rw-r--r--   0 alf        (501) staff       (20)       90 2023-06-23 19:26:02.000000 pix2vec-0.1.1/docs/_build/html/_static/minus.png
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/docs/_build/html/_images/
--rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.1/docs/_build/html/_images/m3cube-a.png
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/history.rst
--rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.1/docs/installation.rst
--rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/authors.rst
--rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.1/docs/readme.rst
--rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 19:26:42.000000 pix2vec-0.1.1/docs/pix2vec.rst
--rw-r--r--   0 alf        (501) staff       (20)     1413 2023-06-23 19:46:19.000000 pix2vec-0.1.1/setup.py
--rw-r--r--   0 alf        (501) staff       (20)       89 2023-06-21 09:12:34.000000 pix2vec-0.1.1/HISTORY.rst
--rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.1/tox.ini
--rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.1/AUTHORS.rst
--rw-r--r--   0 alf        (501) staff       (20)      379 2023-06-23 19:47:44.000000 pix2vec-0.1.1/setup.cfg
-drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-23 19:47:44.000000 pix2vec-0.1.1/pix2vec/
--rw-r--r--   0 alf        (501) staff       (20)     2180 2023-06-22 16:05:48.000000 pix2vec-0.1.1/pix2vec/__init__.py
--rw-r--r--   0 alf        (501) staff       (20)     1785 2023-06-21 13:22:16.000000 pix2vec-0.1.1/pix2vec/cli.py
--rw-r--r--   0 alf        (501) staff       (20)     6857 2023-06-22 16:17:11.000000 pix2vec-0.1.1/pix2vec/pix2vec.py
--rw-r--r--   0 alf        (501) staff       (20)     3605 2023-06-23 19:15:56.000000 pix2vec-0.1.1/README.rst
--rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.1/.readthedocs.yaml
--rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.1/requirements_dev.txt
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/
+-rw-r--r--   0 alf        (501) staff       (20)     6264 2023-06-25 19:42:24.000000 pix2vec-0.1.2/PKG-INFO
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/
+-rw-r--r--   0 alf        (501) staff       (20)     6264 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/PKG-INFO
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-21 09:26:55.000000 pix2vec-0.1.2/pix2vec.egg-info/not-zip-safe
+-rw-r--r--   0 alf        (501) staff       (20)      874 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 alf        (501) staff       (20)       46 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/entry_points.txt
+-rw-r--r--   0 alf        (501) staff       (20)        8 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/top_level.txt
+-rw-r--r--   0 alf        (501) staff       (20)        1 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 alf        (501) staff       (20)     1564 2023-06-21 09:12:34.000000 pix2vec-0.1.2/LICENSE
+-rw-r--r--   0 alf        (501) staff       (20)     3524 2023-06-22 08:52:00.000000 pix2vec-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 alf        (501) staff       (20)     2295 2023-06-21 09:12:34.000000 pix2vec-0.1.2/Makefile
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/tests/
+-rw-r--r--   0 alf        (501) staff       (20)       37 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tests/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)      387 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tests/test_pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)      262 2023-06-21 09:12:34.000000 pix2vec-0.1.2/MANIFEST.in
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/
+-rw-r--r--   0 alf        (501) staff       (20)      552 2023-06-23 21:34:41.000000 pix2vec-0.1.2/docs/index.rst
+-rw-r--r--   0 alf        (501) staff       (20)       33 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/contributing.rst
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/images/
+-rw-r--r--   0 alf        (501) staff       (20)   948490 2023-06-23 18:50:51.000000 pix2vec-0.1.2/docs/images/m3cube-c.png
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.2/docs/images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)   337959 2023-06-23 23:06:07.000000 pix2vec-0.1.2/docs/images/m3-detail.png
+-rw-r--r--   0 alf        (501) staff       (20)   339139 2023-06-23 23:06:07.000000 pix2vec-0.1.2/docs/images/m3-PixelValue.png
+-rw-r--r--   0 alf        (501) staff       (20)      608 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/Makefile
+-rwxr-xr-x   0 alf        (501) staff       (20)     4876 2023-06-21 10:42:06.000000 pix2vec-0.1.2/docs/conf.py
+-rw-r--r--   0 alf        (501) staff       (20)       58 2023-06-23 20:25:10.000000 pix2vec-0.1.2/docs/modules.rst
+-rw-r--r--   0 alf        (501) staff       (20)      181 2023-06-21 14:04:55.000000 pix2vec-0.1.2/docs/usage.rst
+-rw-r--r--   0 alf        (501) staff       (20)      805 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/make.bat
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/_static/
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 alf        (501) staff       (20)      286 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/file.png
+-rw-r--r--   0 alf        (501) staff       (20)       90 2021-10-12 12:18:02.000000 pix2vec-0.1.2/docs/_build/html/_static/minus.png
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/docs/_build/html/_images/
+-rw-r--r--   0 alf        (501) staff       (20)   530877 2023-06-21 13:49:17.000000 pix2vec-0.1.2/docs/_build/html/_images/m3cube-a.png
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/history.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1114 2023-06-22 08:51:18.000000 pix2vec-0.1.2/docs/installation.rst
+-rw-r--r--   0 alf        (501) staff       (20)       28 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/authors.rst
+-rw-r--r--   0 alf        (501) staff       (20)       27 2023-06-21 09:12:34.000000 pix2vec-0.1.2/docs/readme.rst
+-rw-r--r--   0 alf        (501) staff       (20)      423 2023-06-23 20:25:10.000000 pix2vec-0.1.2/docs/pix2vec.rst
+-rw-r--r--   0 alf        (501) staff       (20)     1583 2023-06-25 19:42:22.000000 pix2vec-0.1.2/setup.py
+-rw-r--r--   0 alf        (501) staff       (20)      351 2023-06-25 19:40:58.000000 pix2vec-0.1.2/HISTORY.rst
+-rw-r--r--   0 alf        (501) staff       (20)      268 2023-06-21 09:12:34.000000 pix2vec-0.1.2/tox.ini
+-rw-r--r--   0 alf        (501) staff       (20)      212 2023-06-21 09:38:53.000000 pix2vec-0.1.2/AUTHORS.rst
+-rw-r--r--   0 alf        (501) staff       (20)      379 2023-06-25 19:42:24.000000 pix2vec-0.1.2/setup.cfg
+drwxr-xr-x   0 alf        (501) staff       (20)        0 2023-06-25 19:42:24.000000 pix2vec-0.1.2/pix2vec/
+-rw-r--r--   0 alf        (501) staff       (20)      202 2023-06-25 15:07:15.000000 pix2vec-0.1.2/pix2vec/__init__.py
+-rw-r--r--   0 alf        (501) staff       (20)     2012 2023-06-23 21:09:46.000000 pix2vec-0.1.2/pix2vec/cli.py
+-rw-r--r--   0 alf        (501) staff       (20)     8802 2023-06-23 21:01:11.000000 pix2vec-0.1.2/pix2vec/pix2vec.py
+-rw-r--r--   0 alf        (501) staff       (20)     3946 2023-06-25 19:38:29.000000 pix2vec-0.1.2/README.rst
+-rw-r--r--   0 alf        (501) staff       (20)      205 2023-06-21 10:32:57.000000 pix2vec-0.1.2/.readthedocs.yaml
+-rw-r--r--   0 alf        (501) staff       (20)      185 2023-06-23 19:30:11.000000 pix2vec-0.1.2/requirements_dev.txt
```

### Comparing `pix2vec-0.1.1/pix2vec.egg-info/SOURCES.txt` & `pix2vec-0.1.2/pix2vec.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 docs/pix2vec.rst
 docs/readme.rst
 docs/usage.rst
 docs/_build/html/_images/m3cube-a.png
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
+docs/images/m3-PixelValue.png
+docs/images/m3-detail.png
 docs/images/m3cube-a.png
 docs/images/m3cube-c.png
 pix2vec/__init__.py
 pix2vec/cli.py
 pix2vec/pix2vec.py
 pix2vec.egg-info/PKG-INFO
 pix2vec.egg-info/SOURCES.txt
```

### Comparing `pix2vec-0.1.1/LICENSE` & `pix2vec-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/CONTRIBUTING.rst` & `pix2vec-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/Makefile` & `pix2vec-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/index.rst` & `pix2vec-0.1.2/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Welcome to pix2vec's documentation!
 ======================================
 
 **pix2vec** is a command line program to process hyperspectral data 
 cubes into vector GIS files.  
 
 The vector representation of the cube ground pixels is saved into a 
-geopackage file, thus the data can be queried as you would with a database.
+geopackage file, thus, the data can be queried as you would with a database.
 
 .. toctree::
    :maxdepth: 2
    :caption: Contents:
 
    readme
    installation
```

### Comparing `pix2vec-0.1.1/docs/images/m3cube-c.png` & `pix2vec-0.1.2/docs/images/m3cube-c.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/images/m3cube-a.png` & `pix2vec-0.1.2/docs/images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/Makefile` & `pix2vec-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/conf.py` & `pix2vec-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/make.bat` & `pix2vec-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/_build/html/_images/m3cube-a.png` & `pix2vec-0.1.2/docs/_build/html/_images/m3cube-a.png`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/docs/installation.rst` & `pix2vec-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pix2vec-0.1.1/setup.py` & `pix2vec-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 
 setup(
     author="Alessandro Frigeri",
     author_email='alessandro.frigeri@inaf.it',
     python_requires='>=3.6',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
+        'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
+	'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Vector Representation of Hyperspectral Data",
+    description="pix2vec produces a vector representation of planetary mapping spectrometers starting from hyperspectral an ISIS data cube",
     entry_points={
         'console_scripts': [
             'pix2vec=pix2vec.cli:main',
         ],
     },
     install_requires=requirements,
     license="GNU General Public License v3",
@@ -40,10 +42,10 @@
     include_package_data=True,
     keywords='pix2vec',
     name='pix2vec',
     packages=find_packages(include=['pix2vec', 'pix2vec.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/afrigeri/pix2vec',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `pix2vec-0.1.1/pix2vec/cli.py` & `pix2vec-0.1.2/pix2vec/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 from .pix2vec import Cube, GndPixels
 import os
 
 def main():
     """Console script for pix2vec."""
     parser = argparse.ArgumentParser()
 	
-    parser.add_argument('_', nargs='*')
-    parser.add_argument('-c','--cube')
-    parser.add_argument('-o','--output')
-    parser.add_argument('-l', '--lines')
-    parser.add_argument('-s', '--samples')
+    parser.add_argument('-c','--cube', required=True)
+    parser.add_argument('-o','--output',help='geopackage GIS output file')
+    parser.add_argument('-l', '--lines',help='the range of lines to be included in the output file\n \
+	                                          e.g. 1,10 to set line 1 to 10 (extreme included)')
+    parser.add_argument('-s', '--samples',help='the range of samples to be included in the output file')
     parser.add_argument('-d', '--debug')
     parser.add_argument('-i', '--info', action='store_true', dest='info')
 	
     args = parser.parse_args()
 
     #print("Arguments: " + str(args._))
     print("pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica")
```

### Comparing `pix2vec-0.1.1/README.rst` & `pix2vec-0.1.2/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,61 @@
 ===============
 pix2vec
 ===============
-*Geospatial Vector Representation of Remote Sensing Hyperspectral Data*
+*Geospatial Vector Representation of Planetary Remote Sensing Hyperspectral Data*
 
 ---------------------------------
 
 
 .. image:: https://img.shields.io/pypi/v/pix2vec.svg
         :target: https://pypi.python.org/pypi/pix2vec
 
-.. image:: https://img.shields.io/travis/afrigeri/pix2vec.svg
-        :target: https://travis-ci.com/afrigeri/pix2vec
-
 .. image:: https://readthedocs.org/projects/pix2vec/badge/?version=latest
         :target: https://pix2vec.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
-
-
-
-pix2vec: Vector Representation of Hyperspectral Data Cubes
+pix2vec: Vector Representation of Planetary Hyperspectral Data Cubes
 
 
 * Free software: GNU General Public License v3
 * Documentation: https://pix2vec.readthedocs.io.
 
 
 Features
 --------
 
 * Produces a vector representation of the raster representation of HSI data 'cubes' generated by ISIS
 
-
 Requirements
 ------------
 
-* a relatively recent ISIS installation
-
+* a relatively recent `Integrated Software for Imagers and Spectrometers (ISIS) <https://isis.astrogeology.usgs.gov>`_ installation and the `kalasiris <https://github.com/rbeyer/kalasiris>`_ module (which will be installed automatically).
+ 
 Cite in your work
 -------------------
 
 Frigeri, A. and Hare, T. 2023. Geospatial Vector Representation of 
-Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.
+Planetary Mapping Spectrometer Data. 6th Planetay Data Workshop, Flagstaff, Arizona 26-28th June 2023, Abstract #7088.::
+
+ @INPROCEEDINGS{FrigeriHare2023,
+       author = {{Frigeri}, A. and {Hare}, T.},
+        title = "{Geospatial Vector Representation of Planetary Mapping Spectrometer Data}",
+    booktitle = {6th Planetay Data Workshop},
+         year = 2023,
+       series = {LPI},
+        month = jun,
+          eid = {7088},
+        pages = {7088}
+ }
 
 
 installation
 ------------
 
-within a working ISIS environment, run:
+within a working ISIS environment, run::
 
     pip install pix2vect
 
 
 
 pix2vec in brief
 -----------------
@@ -62,19 +66,25 @@
 
     (ISIS) $ pix2vec -i -c M3G20090103T084105_V03_L1B.cub 
     pix2vect - 2023 Alessandro Frigeri - Istituto Nazionale di Astrofisica
     Cube Type:M3 samples:304 lines:11739 file:M3G20090103T084105_V03_L1B.cub
 
 now we create a vector GIS file representing the geometry of the sensor's pixel on the lunar surface::
 
-    pix2vec -c M3G20090103T084105_V03_L1B.cub -s 152,162 -l5864,5874 -o M3G20090103T084105_V03_L1B_center.gpkg 
+    pix2vec -c M3G20090103T084105_V03_L1B.cub -s 1,150 -l 3050,3200 -o M3G20090103T084105_V03_L1B_subset.gpkg 
 
-the vector file can then be loaded in your favorite GIS, and we can plot the `PixelValue` field:
+the vector file can then be loaded in your favorite GIS, and we can plot the file with a `PixelValue` greyscale:
 
-.. image:: docs/images/m3cube-c.png
+.. image:: /docs/images/m3-PixelValue.png
+        :alt: M3-PixelValue
+        :width: 600
+
+each ground pixel element holds information that can be accessed:
+
+.. image:: /docs/images/m3-detail.png
         :alt: M3-subcube
         :width: 600
 
 for each ground-projected pixel, you now have access to these fields::
 
 	Filename Sample Line PixelValue RightAscension Declination 
 	PlanetocentricLatitude PlanetographicLatitude PositiveEast360Longitude 
@@ -89,22 +99,12 @@
 	LocalSolarTime SolarLongitude LookDirectionBodyFixedX LookDirectionBodyFixedY 
 	LookDirectionBodyFixedZ LookDirectionJ2000X LookDirectionJ2000Y 
 	LookDirectionJ2000Z LookDirectionCameraX LookDirectionCameraY 
 	LookDirectionCameraZ ObliqueDetectorResolution ObliquePixelResolution 
 	ObliqueLineResolution ObliqueSampleResolution Error
 
 
-
-
 Documentation
 -------------
 
 Documentation is available at https://pix2vec.readthedocs.io
 
-
-Credits
--------
-
-This package was created with Cookiecutter_ and the `audreyr/cookiecutter-pypackage`_ project template.
-
-.. _Cookiecutter: https://github.com/audreyr/cookiecutter
-.. _`audreyr/cookiecutter-pypackage`: https://github.com/audreyr/cookiecutter-pypackage
```

