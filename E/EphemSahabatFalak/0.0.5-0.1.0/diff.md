# Comparing `tmp/EphemSahabatFalak-0.0.5.tar.gz` & `tmp/EphemSahabatFalak-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EphemSahabatFalak-0.0.5.tar", last modified: Tue Jun 13 03:57:30 2023, max compression
+gzip compressed data, was "EphemSahabatFalak-0.1.0.tar", last modified: Sun Jun 25 03:32:11 2023, max compression
```

## Comparing `EphemSahabatFalak-0.0.5.tar` & `EphemSahabatFalak-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.438851 EphemSahabatFalak-0.0.5/
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.435486 EphemSahabatFalak-0.0.5/EphemSahabatFalak/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    51556 2023-06-13 03:48:16.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak/KiraanWaktuSolat.py
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       53 2023-06-11 17:41:20.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak/__init__.py
-drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-13 03:57:30.438052 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13856 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      290 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/SOURCES.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/dependency_links.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       46 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/requires.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-06-13 03:57:30.000000 EphemSahabatFalak-0.0.5/EphemSahabatFalak.egg-info/top_level.txt
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13856 2023-06-13 03:57:30.438485 EphemSahabatFalak-0.0.5/PKG-INFO
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    13213 2023-06-12 05:12:54.000000 EphemSahabatFalak-0.0.5/README.md
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-13 03:57:30.438937 EphemSahabatFalak-0.0.5/setup.cfg
--rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1228 2023-06-13 03:57:06.000000 EphemSahabatFalak-0.0.5/setup.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.812730 EphemSahabatFalak-0.1.0/
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.811098 EphemSahabatFalak-0.1.0/EphemSahabatFalak/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)   100342 2023-06-25 03:09:48.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/KiraanWaktuSolat.py
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49515 2023-06-24 23:21:37.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/Takwim_Madinah_Awal_Bulan_Mabims2021.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)    49659 2023-06-23 14:51:37.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/Tarikh_Hijri_Awal_Tahun_Pulau_Pinang.csv
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       53 2023-06-11 17:41:20.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak/__init__.py
+drwxr-xr-x   0 muhammadizzatmohdzubir   (501) staff       (20)        0 2023-06-25 03:32:11.812263 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      420 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/SOURCES.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)        1 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/dependency_links.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       78 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/requires.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       18 2023-06-25 03:32:11.000000 EphemSahabatFalak-0.1.0/EphemSahabatFalak.egg-info/top_level.txt
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      152 2023-06-25 03:25:43.000000 EphemSahabatFalak-0.1.0/MANIFEST.in
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1463 2023-06-25 03:32:11.812562 EphemSahabatFalak-0.1.0/PKG-INFO
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)      876 2023-06-25 03:26:42.000000 EphemSahabatFalak-0.1.0/README.md
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)       38 2023-06-25 03:32:11.812799 EphemSahabatFalak-0.1.0/setup.cfg
+-rw-r--r--   0 muhammadizzatmohdzubir   (501) staff       (20)     1302 2023-06-25 03:27:48.000000 EphemSahabatFalak-0.1.0/setup.py
```

### Comparing `EphemSahabatFalak-0.0.5/setup.py` & `EphemSahabatFalak-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.5'
+VERSION = '0.1.0'
 DESCRIPTION = 'Sebuah pakej yang boleh menghasilkan pelbagai data berkenaan falak'
 LONG_DESCRIPTION = 'Sebuah pakej python yang menggunakan ephemeris dari JPL Horizon bagi menghasilkan hitungan falak'
 
 # Setting up
 setup(
     name="EphemSahabatFalak",
     version=VERSION,
     author="cartcosine (izzatzubir)",
     author_email="<cart.cosine.0x@icloud.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['skyfield', 'pytz', 'datetime', 'DateTime', 'mpmath', 'pandas'],
-    keywords=['python', 'falak', 'solat', 'hilal', 'waktu', 'matahari', 'bulan'],
+    include_package_data = True,
+    install_requires=['skyfield', 'pytz', 'datetime', 'DateTime', 'mpmath', 'pandas', 'timezonefinder', 'matplotlib', 'numpy'],
+    keywords=['falak', 'solat', 'hilal', 'waktu', 'matahari', 'bulan', 'kiblat'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

