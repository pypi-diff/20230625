# Comparing `tmp/pysipfenn-0.12.0.tar.gz` & `tmp/pysipfenn-0.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysipfenn-0.12.0.tar", last modified: Thu Apr  6 20:34:12 2023, max compression
+gzip compressed data, was "pysipfenn-0.12.1.tar", last modified: Sun Jun 25 16:55:46 2023, max compression
```

## Comparing `pysipfenn-0.12.0.tar` & `pysipfenn-0.12.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.887763 pysipfenn-0.12.0/
--rw-r--r--   0 adam       (501) staff       (20)      104 2023-03-17 23:08:06.000000 pysipfenn-0.12.0/.gitattributes
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.867852 pysipfenn-0.12.0/.github/
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.871106 pysipfenn-0.12.0/.github/workflows/
--rw-r--r--   0 adam       (501) staff       (20)     1406 2023-04-06 16:49:48.000000 pysipfenn-0.12.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 adam       (501) staff       (20)     2667 2023-04-06 15:18:55.000000 pysipfenn-0.12.0/.github/workflows/fullTest.yml
--rw-r--r--   0 adam       (501) staff       (20)      885 2023-04-06 15:18:55.000000 pysipfenn-0.12.0/.github/workflows/partialTest.yml
--rwx------   0 adam       (501) staff       (20)      408 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/.readthedocs.yaml
--rwx------   0 adam       (501) staff       (20)    35149 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/LICENSE
--rwx------   0 adam       (501) staff       (20)      231 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/MANIFEST.in
--rw-r--r--   0 adam       (501) staff       (20)     8456 2023-04-06 20:34:12.887599 pysipfenn-0.12.0/PKG-INFO
--rwx------   0 adam       (501) staff       (20)     7231 2023-04-06 16:22:26.000000 pysipfenn-0.12.0/README.md
--rwx------   0 adam       (501) staff       (20)     1522 2023-04-06 16:01:12.000000 pysipfenn-0.12.0/pyproject.toml
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.871403 pysipfenn-0.12.0/pysipfenn/
--rwx------   0 adam       (501) staff       (20)       38 2023-04-05 20:03:47.000000 pysipfenn-0.12.0/pysipfenn/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.872498 pysipfenn-0.12.0/pysipfenn/core/
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/core/__init__.py
--rwx------   0 adam       (501) staff       (20)    39130 2023-04-06 13:58:04.000000 pysipfenn-0.12.0/pysipfenn/core/pysipfenn.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.876880 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/
--rwx------   0 adam       (501) staff       (20)    28375 2023-04-06 16:33:34.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022.py
--rw-r--r--   0 adam       (501) staff       (20)     2036 2023-04-06 16:33:38.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_TestResult.csv
--rwx------   0 adam       (501) staff       (20)    23904 2023-04-06 16:39:11.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_dilute.py
--rw-r--r--   0 adam       (501) staff       (20)     2035 2023-04-06 16:39:13.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv
--rwx------   0 adam       (501) staff       (20)   141363 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv
--rwx------   0 adam       (501) staff       (20)      702 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Magpie_property_names.txt
--rwx------   0 adam       (501) staff       (20)      151 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/README.md
--rw-r--r--   0 adam       (501) staff       (20)    33100 2023-04-06 16:33:34.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Ward2017.py
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.878094 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/
--rw-------   0 adam       (501) staff       (20)    18268 2023-04-06 16:23:37.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc
--rw-------   0 adam       (501) staff       (20)    18165 2023-02-27 19:53:52.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc
--rw-r--r--   0 adam       (501) staff       (20)    20651 2023-04-06 16:23:35.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc
--rw-------   0 adam       (501) staff       (20)      172 2023-02-27 19:53:51.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/__init__.cpython-39.pyc
--rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_KS2022.csv
--rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
--rwx------   0 adam       (501) staff       (20)     6206 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.878481 pysipfenn-0.12.0/pysipfenn/modelsSIPFENN/
--rwx------   0 adam       (501) staff       (20)       86 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/modelsSIPFENN/README.md
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/modelsSIPFENN/__init__.py
--rwx------   0 adam       (501) staff       (20)     1420 2023-02-28 15:23:16.000000 pysipfenn-0.12.0/pysipfenn/modelsSIPFENN/models.json
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.880515 pysipfenn-0.12.0/pysipfenn/tests/
--rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/__init__.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.881425 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/
--rw-r--r--   0 adam       (501) staff       (20)    13122 2023-04-05 21:14:25.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
--rw-r--r--   0 adam       (501) staff       (20)    18296 2023-04-05 21:14:25.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.886700 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/
--rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
--rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1015 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
--rwx------   0 adam       (501) staff       (20)     1020 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1019 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
--rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
--rwx------   0 adam       (501) staff       (20)     1923 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR
--rwx------   0 adam       (501) staff       (20)     1003 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
--rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
--rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
--rwx------   0 adam       (501) staff       (20)     1023 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
--rwx------   0 adam       (501) staff       (20)      908 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
--rwx------   0 adam       (501) staff       (20)    68010 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.887311 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
--rwx------   0 adam       (501) staff       (20)      743 2023-03-31 18:23:39.000000 pysipfenn-0.12.0/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
--rwx------   0 adam       (501) staff       (20)     2624 2023-04-05 16:12:25.000000 pysipfenn-0.12.0/pysipfenn/tests/test_KS2022.py
--rwx------   0 adam       (501) staff       (20)    21057 2023-04-05 17:50:14.000000 pysipfenn-0.12.0/pysipfenn/tests/test_KS2022_dilute.py
--rwx------   0 adam       (501) staff       (20)     1578 2023-03-31 18:23:39.000000 pysipfenn-0.12.0/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
--rwx------   0 adam       (501) staff       (20)     1800 2023-04-05 17:27:15.000000 pysipfenn-0.12.0/pysipfenn/tests/test_Ward2017.py
--rw-r--r--   0 adam       (501) staff       (20)     2221 2023-03-31 18:23:39.000000 pysipfenn-0.12.0/pysipfenn/tests/test_customModel.py
--rwx------   0 adam       (501) staff       (20)    12132 2023-04-05 21:17:25.000000 pysipfenn-0.12.0/pysipfenn/tests/test_pysipfenn.py
-drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-04-06 20:34:12.872238 pysipfenn-0.12.0/pysipfenn.egg-info/
--rwx------   0 adam       (501) staff       (20)     8456 2023-04-06 20:34:12.000000 pysipfenn-0.12.0/pysipfenn.egg-info/PKG-INFO
--rwx------   0 adam       (501) staff       (20)     4311 2023-04-06 20:34:12.000000 pysipfenn-0.12.0/pysipfenn.egg-info/SOURCES.txt
--rwx------   0 adam       (501) staff       (20)        1 2023-04-06 20:34:12.000000 pysipfenn-0.12.0/pysipfenn.egg-info/dependency_links.txt
--rwx------   0 adam       (501) staff       (20)      147 2023-04-06 20:34:12.000000 pysipfenn-0.12.0/pysipfenn.egg-info/requires.txt
--rwx------   0 adam       (501) staff       (20)       10 2023-04-06 20:34:12.000000 pysipfenn-0.12.0/pysipfenn.egg-info/top_level.txt
--rw-r--r--   0 adam       (501) staff       (20)       38 2023-04-06 20:34:12.887813 pysipfenn-0.12.0/setup.cfg
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.027309 pysipfenn-0.12.1/
+-rw-r--r--   0 adam       (501) staff       (20)      104 2023-03-17 23:08:06.000000 pysipfenn-0.12.1/.gitattributes
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.008392 pysipfenn-0.12.1/.github/
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.011235 pysipfenn-0.12.1/.github/workflows/
+-rw-r--r--   0 adam       (501) staff       (20)     1327 2023-04-06 22:05:43.000000 pysipfenn-0.12.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 adam       (501) staff       (20)     2667 2023-04-06 15:18:55.000000 pysipfenn-0.12.1/.github/workflows/fullTest.yml
+-rw-r--r--   0 adam       (501) staff       (20)      885 2023-04-06 15:18:55.000000 pysipfenn-0.12.1/.github/workflows/partialTest.yml
+-rwx------   0 adam       (501) staff       (20)      408 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/.readthedocs.yaml
+-rwx------   0 adam       (501) staff       (20)    35149 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/LICENSE
+-rwx------   0 adam       (501) staff       (20)      309 2023-06-25 16:55:13.000000 pysipfenn-0.12.1/MANIFEST.in
+-rw-r--r--   0 adam       (501) staff       (20)     8456 2023-06-25 16:55:46.027138 pysipfenn-0.12.1/PKG-INFO
+-rwx------   0 adam       (501) staff       (20)     7231 2023-04-06 16:22:26.000000 pysipfenn-0.12.1/README.md
+-rwx------   0 adam       (501) staff       (20)     1522 2023-06-25 16:52:20.000000 pysipfenn-0.12.1/pyproject.toml
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.011515 pysipfenn-0.12.1/pysipfenn/
+-rwx------   0 adam       (501) staff       (20)       38 2023-04-05 20:03:47.000000 pysipfenn-0.12.1/pysipfenn/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.012436 pysipfenn-0.12.1/pysipfenn/core/
+-rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/core/__init__.py
+-rw-r--r--   0 adam       (501) staff       (20)    39207 2023-06-25 16:52:20.000000 pysipfenn-0.12.1/pysipfenn/core/pysipfenn.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.016272 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/
+-rwx------   0 adam       (501) staff       (20)    28375 2023-04-06 16:33:34.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022.py
+-rw-r--r--   0 adam       (501) staff       (20)     2036 2023-04-06 16:33:38.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_TestResult.csv
+-rwx------   0 adam       (501) staff       (20)    23904 2023-04-06 16:39:11.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py
+-rw-r--r--   0 adam       (501) staff       (20)     2035 2023-04-06 16:39:13.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv
+-rwx------   0 adam       (501) staff       (20)   141363 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv
+-rwx------   0 adam       (501) staff       (20)      702 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_property_names.txt
+-rwx------   0 adam       (501) staff       (20)      151 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/README.md
+-rw-r--r--   0 adam       (501) staff       (20)    33100 2023-04-06 16:33:34.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Ward2017.py
+-rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.017272 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/
+-rw-------   0 adam       (501) staff       (20)    18404 2023-04-06 21:56:10.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc
+-rw-------   0 adam       (501) staff       (20)    15449 2023-04-06 21:56:10.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc
+-rw-r--r--   0 adam       (501) staff       (20)    20791 2023-04-06 21:56:09.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc
+-rw-------   0 adam       (501) staff       (20)      172 2023-02-27 19:53:51.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/__init__.cpython-39.pyc
+-rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv
+-rwx------   0 adam       (501) staff       (20)     5796 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv
+-rwx------   0 adam       (501) staff       (20)     6206 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.017757 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/
+-rwx------   0 adam       (501) staff       (20)       86 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/README.md
+-rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/__init__.py
+-rwx------   0 adam       (501) staff       (20)     1420 2023-02-28 15:23:16.000000 pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/models.json
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.019647 pysipfenn-0.12.1/pysipfenn/tests/
+-rwx------   0 adam       (501) staff       (20)        0 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/__init__.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.020479 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/
+-rw-r--r--   0 adam       (501) staff       (20)    13122 2023-04-05 21:14:25.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv
+-rw-r--r--   0 adam       (501) staff       (20)    18296 2023-04-05 21:14:25.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.026126 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/
+-rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1021 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR
+-rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR
+-rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR
+-rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR
+-rwx------   0 adam       (501) staff       (20)      916 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1015 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1020 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1019 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1018 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1012 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1923 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1003 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1014 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1016 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR
+-rwx------   0 adam       (501) staff       (20)     1023 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR
+-rwx------   0 adam       (501) staff       (20)      908 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR
+-rwx------   0 adam       (501) staff       (20)    68010 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.026766 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/
+-rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR
+-rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR
+-rwx------   0 adam       (501) staff       (20)    15121 2023-02-27 18:54:19.000000 pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR
+-rwx------   0 adam       (501) staff       (20)      743 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py
+-rwx------   0 adam       (501) staff       (20)     3152 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_KS2022.py
+-rwx------   0 adam       (501) staff       (20)    21509 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_KS2022_dilute.py
+-rwx------   0 adam       (501) staff       (20)     1578 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py
+-rwx------   0 adam       (501) staff       (20)     2338 2023-04-06 22:01:56.000000 pysipfenn-0.12.1/pysipfenn/tests/test_Ward2017.py
+-rw-r--r--   0 adam       (501) staff       (20)     2221 2023-03-31 18:23:39.000000 pysipfenn-0.12.1/pysipfenn/tests/test_customModel.py
+-rwx------   0 adam       (501) staff       (20)    12132 2023-04-05 21:17:25.000000 pysipfenn-0.12.1/pysipfenn/tests/test_pysipfenn.py
+drwxr-xr-x   0 adam       (501) staff       (20)        0 2023-06-25 16:55:46.012214 pysipfenn-0.12.1/pysipfenn.egg-info/
+-rwx------   0 adam       (501) staff       (20)     8456 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/PKG-INFO
+-rwx------   0 adam       (501) staff       (20)     4311 2023-06-25 16:55:46.000000 pysipfenn-0.12.1/pysipfenn.egg-info/SOURCES.txt
+-rwx------   0 adam       (501) staff       (20)        1 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/dependency_links.txt
+-rwx------   0 adam       (501) staff       (20)      147 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/requires.txt
+-rwx------   0 adam       (501) staff       (20)       10 2023-06-25 16:55:45.000000 pysipfenn-0.12.1/pysipfenn.egg-info/top_level.txt
+-rw-r--r--   0 adam       (501) staff       (20)       38 2023-06-25 16:55:46.027357 pysipfenn-0.12.1/setup.cfg
```

### Comparing `pysipfenn-0.12.0/.github/workflows/benchmarks.yml` & `pysipfenn-0.12.1/.github/workflows/benchmarks.yml`

 * *Files 14% similar despite different names*

```diff
@@ -22,14 +22,16 @@
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install --upgrade setuptools
           python -m pip install wheel flask
           python -m pip install -e .
 
-      - name: Benchmark KS2022 with command line python call
+      - name: Benchmark KS2022
         run: python -c "from pysipfenn.descriptorDefinitions import KS2022; KS2022.profile(test='JVASP-10001', nRuns=100); KS2022.profile(test='diluteNiAlloy', nRuns=100)"
-      - name: Benchmark KS2022 with command line python call
+
+      - name: Benchmark Ward2017
         run: python -c "from pysipfenn.descriptorDefinitions import Ward2017; Ward2017.profile(test='JVASP-10001', nRuns=100); Ward2017.profile(test='diluteNiAlloy', nRuns=100)"
-      - name: Benchmark KS2022 dilute featurizer with command line python call
-        run: python -c "from pysipfenn.descriptorDefinitions import KS2022; KS2022_dilute.profile(test='diluteNiAlloy', nRuns=100)"
+
+      - name: Benchmark KS2022 dilute featurizer
+        run: python -c "from pysipfenn.descriptorDefinitions import KS2022_dilute; KS2022_dilute.profile(test='diluteNiAlloy', nRuns=250)"
```

### Comparing `pysipfenn-0.12.0/.github/workflows/fullTest.yml` & `pysipfenn-0.12.1/.github/workflows/fullTest.yml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/.github/workflows/partialTest.yml` & `pysipfenn-0.12.1/.github/workflows/partialTest.yml`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/LICENSE` & `pysipfenn-0.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/PKG-INFO` & `pysipfenn-0.12.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysipfenn
-Version: 0.12.0
+Version: 0.12.1
 Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
 Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
 Project-URL: Research Page, https://phaseslab.com/sipfenn
 Project-URL: Homepage, https://pysipfenn.org
 Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pysipfenn-0.12.0/README.md` & `pysipfenn-0.12.1/README.md`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pyproject.toml` & `pysipfenn-0.12.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pysipfenn"
-version = "0.12.0"
+version = "0.12.1"
 authors = [
   { name="Adam Krajewski", email="ak@psu.edu" },
     { name="Jonathan Siegel", email="jwsiegel@tamu.edu" },
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
```

### Comparing `pysipfenn-0.12.0/pysipfenn/core/pysipfenn.py` & `pysipfenn-0.12.1/pysipfenn/core/pysipfenn.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from typing import List, Union, Dict
 
 # Descriptor Generators
 from pysipfenn.descriptorDefinitions import Ward2017, KS2022, KS2022_dilute
 
 # - add new ones here if extending the code
 
-__version__ = '0.11.0post1'
+__version__ = '0.12.1'
 __authors__ = [["Adam Krajewski", "ak@psu.edu"],
                ["Jonathan Siegel", "jwsiegel@tamu.edu"]]
 __name__ = 'pysipfenn'
 
 
 class Calculator:
     """
@@ -72,15 +72,15 @@
             print(f'Loading all available models (autoLoad=True)')
             self.loadModels()
 
         self.toRun = []
         self.descriptorData = []
         self.predictions = []
         self.inputFiles = []
-        print(f'*********  PySIPFENN Successfully Initialized  **********')
+        print(f'*********  PySIPFENN Calculator v{__version__} Successfully Initialized  **********')
 
     def __str__(self):
         printOut = f'PySIPFENN Calculator Object. Version: {__version__}\n'
         printOut += f'Models are located in:\n{resources.files("pysipfenn.modelsSIPFENN")}\n{"-" * 80}\n'
         printOut += f'Loaded Networks: {list(self.loadedModels.keys())}\n'
         if len(self.inputFiles) > 0:
             printOut += f'Last files selected as input: {len(self.inputFiles)}\n'
@@ -350,15 +350,15 @@
         print('Making predictions...')
         # Run for each network
         dataIn = torch.from_numpy(np.array(dataInList)).float()
         for net in toRun:
             t0 = perf_counter()
             model = models[net]
             model.eval()
-            if hasattr(model, 'Dropout_0'):
+            if 'OnnxDropoutDynamic()' in {str(module) for module in list(model._modules.values())}:
                 tempOut = model(dataIn, None)
             else:
                 tempOut = model(dataIn)
             t1 = perf_counter()
             dataOuts.append(tempOut.cpu().detach().numpy())
             print(f'Prediction rate: {round(len(tempOut) / (t1 - t0), 1)} pred/s')
             print(f'Obtained {len(tempOut)} predictions from:  {net}')
```

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022.py` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_TestResult.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_TestResult.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_dilute.py` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/KS2022_dilute_TestResult.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_element_properties.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Magpie_property_names.txt` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Magpie_property_names.txt`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/Ward2017.py` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr  6 16:22:26 2023 UTC, .py size: 28007 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 c2f1 2e64 676d 0000  a..........dgm..
+00000000: 610d 0d0a 0000 0000 5ef4 2e64 d76e 0000  a.......^..d.n..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6401 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
@@ -529,614 +529,623 @@
 00002100: 7275 6374 7572 616c 7226 0000 0072 2600  ructuralr&...r&.
 00002110: 0000 7229 0000 00da 0e6f 6e6c 7953 7472  ..r).....onlyStr
 00002120: 7563 7475 7261 6cd1 0000 0073 1800 0000  uctural....s....
 00002130: 000b 1001 0e01 1001 0401 0601 0601 06fd  ................
 00002140: 0204 06fc 0605 0e02 72c1 0000 00fa 0b4a  ........r......J
 00002150: 5641 5350 2d31 3030 3031 7213 0000 0063  VASP-10001r....c
 00002160: 0200 0000 0000 0000 0000 0000 0700 0000  ................
-00002170: 0800 0000 4300 0000 73ae 0000 007c 0064  ....C...s....|.d
-00002180: 016b 0272 1674 0064 0283 0101 0064 037d  .k.r.t.d.....d.}
-00002190: 026e 227c 0064 046b 0272 2c74 0064 0583  .n"|.d.k.r,t.d..
-000021a0: 0101 0064 067d 026e 0c74 0064 0783 0101  ...d.}.n.t.d....
-000021b0: 0064 0853 0074 01a0 0274 03a0 047c 02a1  .d.S.t...t...|..
-000021c0: 01a1 0167 017c 0114 007d 0374 057c 0383  ...g.|...}.t.|..
-000021d0: 0144 005d 0c7d 0474 067c 0483 017d 0571  .D.].}.t.|...}.q
-000021e0: 5674 0764 0964 0a83 028f 247d 067c 06a0  Vt.d.d....$}.|..
-000021f0: 0864 0b64 0c84 007c 0544 0083 01a1 0101  .d.d...|.D......
-00002200: 0057 0064 0804 0004 0083 0301 006e 1031  .W.d.........n.1
-00002210: 0073 9830 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
-00002220: 0064 0d83 0101 0064 0853 0029 0e7a 4350  .d.....d.S.).zCP
-00002230: 726f 6669 6c65 7320 7468 6520 6465 7363  rofiles the desc
-00002240: 7269 7074 6f72 2069 6e20 7365 7269 6573  riptor in series
-00002250: 2075 7369 6e67 206f 6e65 206f 6620 7468   using one of th
-00002260: 6520 7465 7374 2073 7472 7563 7475 7265  e test structure
-00002270: 732e 72c2 0000 007a 5450 726f 6669 6c69  s.r....zTProfili
-00002280: 6e67 2f74 6573 7469 6e67 2074 6173 6b2e  ng/testing task.
-00002290: 2057 696c 6c20 6361 6c63 756c 6174 6520   Will calculate 
-000022a0: 6120 6465 7363 7269 7074 6f72 2066 6f72  a descriptor for
-000022b0: 204c 6932 205a 7231 2054 6531 204f 3620   Li2 Zr1 Te1 O6 
-000022c0: 284a 5641 5350 2d31 3030 3031 29e1 460a  (JVASP-10001).F.
-000022d0: 0000 7b22 406d 6f64 756c 6522 3a20 2270  ..{"@module": "p
-000022e0: 796d 6174 6765 6e2e 636f 7265 2e73 7472  ymatgen.core.str
-000022f0: 7563 7475 7265 222c 2022 4063 6c61 7373  ucture", "@class
-00002300: 223a 2022 5374 7275 6374 7572 6522 2c20  ": "Structure", 
-00002310: 2263 6861 7267 6522 3a20 6e75 6c6c 2c20  "charge": null, 
-00002320: 226c 6174 7469 6365 223a 207b 226d 6174  "lattice": {"mat
-00002330: 7269 7822 3a20 5b5b 342e 3539 3933 3035  rix": [[4.599305
-00002340: 3635 3236 3632 3435 392c 2030 2e30 3039  652662459, 0.009
-00002350: 3830 3135 3037 3639 3938 3832 332c 2033  8015076998823, 3
-00002360: 2e31 3035 3236 3132 3836 3534 3433 3733  .105261286544373
-00002370: 365d 2c20 5b31 2e36 3535 3332 3537 3732  6], [1.655325772
-00002380: 3632 3034 3635 332c 2034 2e32 3931 3130  6204653, 4.29110
-00002390: 3834 3735 3835 3437 3132 2c20 332e 3130  8475854712, 3.10
-000023a0: 3532 3630 3239 3338 3937 3935 3635 5d2c  52602938979565],
-000023b0: 205b 302e 3031 3432 3534 3132 3134 3931   [0.014254121491
-000023c0: 3937 3439 2c20 302e 3030 3938 3032 3530  9749, 0.00980250
-000023d0: 3939 3939 3631 3331 2c20 352e 3534 3934  99996131, 5.5494
-000023e0: 3139 3134 3138 3636 3335 315d 5d2c 2022  19141866351]], "
-000023f0: 6122 3a20 352e 3534 3934 3436 3437 3831  a": 5.5494464781
-00002400: 3532 3332 362c 2022 6222 3a20 352e 3534  52326, "b": 5.54
-00002410: 3934 3436 3533 3631 3739 3334 332c 2022  9446536179343, "
-00002420: 6322 3a20 352e 3534 3934 3436 3130 3538  c": 5.5494461058
-00002430: 3130 3432 332c 2022 616c 7068 6122 3a20  10423, "alpha": 
-00002440: 3535 2e38 3237 3134 3435 3939 3835 3833  55.8271445998583
-00002450: 322c 2022 6265 7461 223a 2035 352e 3832  2, "beta": 55.82
-00002460: 3731 3430 3134 3238 3933 3731 2c20 2267  714014289371, "g
-00002470: 616d 6d61 223a 2035 352e 3832 3731 3339  amma": 55.827139
-00002480: 3732 3737 3930 3932 2c20 2276 6f6c 756d  72779092, "volum
-00002490: 6522 3a20 3130 392e 3135 3438 3436 3235  e": 109.15484625
-000024a0: 3634 3237 3433 7d2c 2022 7369 7465 7322  642743}, "sites"
-000024b0: 3a20 5b7b 2273 7065 6369 6573 223a 205b  : [{"species": [
-000024c0: 7b22 656c 656d 656e 7422 3a20 224c 6922  {"element": "Li"
-000024d0: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
-000024e0: 2022 6162 6322 3a20 5b30 2e32 3733 3837   "abc": [0.27387
-000024f0: 3834 3837 3236 3639 3932 342c 2030 2e32  84872669924, 0.2
-00002500: 3733 3837 3834 3837 3236 3730 3430 372c  738784872670407,
-00002510: 2030 2e32 3733 3837 3834 3837 3236 3733   0.2738784872673
-00002520: 3033 325d 2c20 2278 797a 223a 205b 312e  032], "xyz": [1.
-00002530: 3731 3639 3132 3839 3034 3030 3730 3633  7169128904007063
-00002540: 2c20 312e 3138 3036 3131 3431 3637 3737  , 1.180611416777
-00002550: 3736 3133 2c20 332e 3232 3037 3934 3737  7613, 3.22079477
-00002560: 3533 3737 3237 385d 2c20 226c 6162 656c  5377278], "label
-00002570: 223a 2022 4c69 222c 2022 7072 6f70 6572  ": "Li", "proper
-00002580: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00002590: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000025a0: 6e74 223a 2022 4c69 222c 2022 6f63 6375  nt": "Li", "occu
-000025b0: 223a 2031 2e30 7d5d 2c20 2261 6263 223a  ": 1.0}], "abc":
-000025c0: 205b 302e 3738 3532 3237 3230 3130 3732   [0.785227201072
-000025d0: 3830 3639 2c20 302e 3738 3532 3237 3230  8069, 0.78522720
-000025e0: 3130 3732 3838 3536 2c20 302e 3738 3532  10728856, 0.7852
-000025f0: 3237 3230 3130 3733 3331 355d 2c20 2278  27201073315], "x
-00002600: 797a 223a 205b 342e 3932 3234 3939 3435  yz": [4.92249945
-00002610: 3137 3339 3936 352c 2033 2e33 3834 3838  1739965, 3.38488
-00002620: 3837 3035 3934 3334 3932 372c 2039 2e32  87059434927, 9.2
-00002630: 3334 3232 3533 3338 3136 3336 3333 5d2c  34225338163633],
-00002640: 2022 6c61 6265 6c22 3a20 224c 6922 2c20   "label": "Li", 
-00002650: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00002660: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00002670: 7b22 656c 656d 656e 7422 3a20 224f 222c  {"element": "O",
-00002680: 2022 6f63 6375 223a 2031 2e30 7d5d 2c20   "occu": 1.0}], 
-00002690: 2261 6263 223a 205b 302e 3836 3639 3936  "abc": [0.866996
-000026a0: 3434 3534 3636 3131 3234 2c20 302e 3630  4454661124, 0.60
-000026b0: 3430 3839 3838 3230 3932 3131 342c 2030  4089882092114, 0
-000026c0: 2e32 3431 3832 3137 3639 3837 3331 3433  .241821769873143
-000026d0: 5d2c 2022 7879 7a22 3a20 5b34 2e39 3930  ], "xyz": [4.990
-000026e0: 3939 3431 3630 3136 3430 3631 2c20 322e  994160164061, 2.
-000026f0: 3630 3330 3833 3534 3538 3736 3835 362c  603083545876856,
-00002700: 2035 2e39 3130 3037 3731 3831 3133 3736   5.9100771811376
-00002710: 3538 5d2c 2022 6c61 6265 6c22 3a20 224f  58], "label": "O
-00002720: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00002730: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00002740: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00002750: 4f22 2c20 226f 6363 7522 3a20 312e 307d  O", "occu": 1.0}
-00002760: 5d2c 2022 6162 6322 3a20 5b30 2e37 3137  ], "abc": [0.717
-00002770: 3834 3038 3934 3532 3937 3838 2c20 302e  840894529788, 0.
-00002780: 3132 3133 3637 3538 3839 3632 3836 3833  1213675889628683
-00002790: 2c20 302e 3339 3335 3337 3030 3931 3836  , 0.393537009186
-000027a0: 3937 335d 2c20 2278 797a 223a 205b 332e  973], "xyz": [3.
-000027b0: 3530 3830 3832 3130 3632 3334 3731 332c  508082106234713,
-000027c0: 2030 2e35 3331 3639 3530 3633 3231 3534   0.5316950632154
-000027d0: 3132 2c20 342e 3738 3938 3633 3330 3634  12, 4.7898633064
-000027e0: 3639 3237 385d 2c20 226c 6162 656c 223a  69278], "label":
-000027f0: 2022 4f22 2c20 2270 726f 7065 7274 6965   "O", "propertie
-00002800: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00002810: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00002820: 3a20 224f 222c 2022 6f63 6375 223a 2031  : "O", "occu": 1
-00002830: 2e30 7d5d 2c20 2261 6263 223a 205b 302e  .0}], "abc": [0.
-00002840: 3132 3133 3637 3538 3839 3633 3834 3032  1213675889638402
-00002850: 2c20 302e 3339 3335 3337 3030 3931 3837  , 0.393537009187
-00002860: 3339 3433 2c20 302e 3731 3738 3430 3839  3943, 0.71784089
-00002870: 3435 3238 3333 3834 5d2c 2022 7879 7a22  45283384], "xyz"
-00002880: 3a20 5b31 2e32 3139 3837 3037 3833 3038  : [1.21987078308
-00002890: 3137 3839 362c 2031 2e36 3936 3933 3632  17896, 1.6969362
-000028a0: 3233 3539 3130 3331 372c 2035 2e35 3832  235910317, 5.582
-000028b0: 3531 3239 3235 3136 3936 345d 2c20 226c  51292516964], "l
-000028c0: 6162 656c 223a 2022 4f22 2c20 2270 726f  abel": "O", "pro
-000028d0: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-000028e0: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-000028f0: 656d 656e 7422 3a20 224f 222c 2022 6f63  ement": "O", "oc
-00002900: 6375 223a 2031 2e30 7d5d 2c20 2261 6263  cu": 1.0}], "abc
-00002910: 223a 205b 302e 3339 3335 3337 3030 3931  ": [0.3935370091
-00002920: 3836 3139 3135 2c20 302e 3731 3738 3430  861915, 0.717840
-00002930: 3839 3435 3239 3338 3536 2c20 302e 3132  8945293856, 0.12
-00002940: 3133 3637 3538 3839 3633 3430 3134 5d2c  13675889634014],
-00002950: 2022 7879 7a22 3a20 5b32 2e39 3939 3938   "xyz": [2.99998
-00002960: 3735 3132 3539 3536 3232 2c20 332e 3038  7512595622, 3.08
-00002970: 3533 3830 3130 3938 3630 3334 342c 2034  5380109860344, 4
-00002980: 2e31 3234 3633 3736 3837 3936 3232 3937  .124637687962297
-00002990: 5d2c 2022 6c61 6265 6c22 3a20 224f 222c  ], "label": "O",
-000029a0: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-000029b0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-000029c0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4f22  [{"element": "O"
-000029d0: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
-000029e0: 2022 6162 6322 3a20 5b30 2e32 3431 3832   "abc": [0.24182
-000029f0: 3137 3639 3837 3231 3537 332c 2030 2e38  17698721573, 0.8
-00002a00: 3636 3939 3634 3435 3436 3731 3232 312c  669964454671221,
-00002a10: 2030 2e36 3034 3038 3938 3832 3039 3231   0.6040898820921
-00002a20: 3531 335d 2c20 2278 797a 223a 205b 322e  513], "xyz": [2.
-00002a30: 3535 3539 3834 3536 3436 3333 3332 392c  555984564633329,
-00002a40: 2033 2e37 3238 3636 3736 3130 3732 3931   3.7286676107291
-00002a50: 3439 2c20 362e 3739 3535 3137 3337 3233  49, 6.7955173723
-00002a60: 3737 3334 335d 2c20 226c 6162 656c 223a  77343], "label":
-00002a70: 2022 4f22 2c20 2270 726f 7065 7274 6965   "O", "propertie
-00002a80: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00002a90: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00002aa0: 3a20 224f 222c 2022 6f63 6375 223a 2031  : "O", "occu": 1
-00002ab0: 2e30 7d5d 2c20 2261 6263 223a 205b 302e  .0}], "abc": [0.
-00002ac0: 3630 3430 3839 3838 3230 3933 3331 3135  6040898820933115
-00002ad0: 2c20 302e 3234 3138 3231 3736 3938 3732  , 0.241821769872
-00002ae0: 3336 3337 2c20 302e 3836 3639 3936 3434  3637, 0.86699644
-00002af0: 3534 3636 3430 3539 5d2c 2022 7879 7a22  54664059], "xyz"
-00002b00: 3a20 5b33 2e31 3931 3034 3630 3930 3134  : [3.19104609014
-00002b10: 3531 3733 2c20 312e 3035 3231 3033 3137  5173, 1.05210317
-00002b20: 3933 3032 3535 3935 2c20 372e 3433 3831  93025595, 7.4381
-00002b30: 3033 3133 3530 3433 3635 3335 5d2c 2022  031350436535], "
-00002b40: 6c61 6265 6c22 3a20 224f 222c 2022 7072  label": "O", "pr
-00002b50: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-00002b60: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-00002b70: 6c65 6d65 6e74 223a 2022 5465 222c 2022  lement": "Te", "
-00002b80: 6f63 6375 223a 2031 2e30 7d5d 2c20 2261  occu": 1.0}], "a
-00002b90: 6263 223a 205b 302e 3439 3635 3930 3536  bc": [0.49659056
-00002ba0: 3130 3530 3733 3533 2c20 302e 3439 3635  10507353, 0.4965
-00002bb0: 3930 3536 3130 3530 3733 3535 2c20 302e  905610507355, 0.
-00002bc0: 3439 3635 3930 3536 3130 3530 3733 3631  4965905610507361
-00002bd0: 5d2c 2022 7879 7a22 3a20 5b33 2e31 3133  ], "xyz": [3.113
-00002be0: 3036 3933 3930 3833 3537 3933 2c20 322e  069390835793, 2.
-00002bf0: 3134 3036 3539 3133 3537 3032 3439 3834  1406591357024984
-00002c00: 2c20 352e 3833 3938 3735 3536 3132 3134  , 5.839875561214
-00002c10: 3636 3234 5d2c 2022 6c61 6265 6c22 3a20  6624], "label": 
-00002c20: 2254 6522 2c20 2270 726f 7065 7274 6965  "Te", "propertie
-00002c30: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00002c40: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00002c50: 3a20 225a 7222 2c20 226f 6363 7522 3a20  : "Zr", "occu": 
-00002c60: 312e 307d 5d2c 2022 6162 6322 3a20 5b30  1.0}], "abc": [0
-00002c70: 2e30 3030 3635 3031 3630 3439 3830 3636  .000650160498066
-00002c80: 382c 2030 2e30 3030 3635 3031 3630 3439  8, 0.00065016049
-00002c90: 3830 3932 382c 2030 2e30 3030 3635 3031  80928, 0.0006501
-00002ca0: 3630 3439 3832 3334 345d 2c20 2278 797a  604982344], "xyz
-00002cb0: 223a 205b 302e 3030 3430 3735 3738 3137  ": [0.0040757817
-00002cc0: 3439 3436 3033 362c 2030 2e30 3032 3830  4946036, 0.00280
-00002cd0: 3236 3534 3938 3139 3435 3139 322c 2030  2654981945192, 0
-00002ce0: 2e30 3037 3634 3538 3438 3931 3832 3633  .007645848918263
-00002cf0: 3037 365d 2c20 226c 6162 656c 223a 2022  076], "label": "
-00002d00: 5a72 222c 2022 7072 6f70 6572 7469 6573  Zr", "properties
-00002d10: 223a 207b 7d7d 5d7d da0d 6469 6c75 7465  ": {}}]}..dilute
-00002d20: 4e69 416c 6c6f 797a 4d50 726f 6669 6c69  NiAlloyzMProfili
-00002d30: 6e67 2f74 6573 7469 6e67 2074 6173 6b2e  ng/testing task.
-00002d40: 2057 696c 6c20 6361 6c63 756c 6174 6520   Will calculate 
-00002d50: 6120 6465 7363 7269 7074 6f72 2066 6f72  a descriptor for
-00002d60: 2061 2064 696c 7574 6520 4643 4320 4e69   a dilute FCC Ni
-00002d70: 3331 4372 312e e1d4 1400 007b 2240 6d6f  31Cr1......{"@mo
-00002d80: 6475 6c65 223a 2022 7079 6d61 7467 656e  dule": "pymatgen
-00002d90: 2e63 6f72 652e 7374 7275 6374 7572 6522  .core.structure"
-00002da0: 2c20 2240 636c 6173 7322 3a20 2253 7472  , "@class": "Str
-00002db0: 7563 7475 7265 222c 2022 6368 6172 6765  ucture", "charge
-00002dc0: 223a 206e 756c 6c2c 2022 6c61 7474 6963  ": null, "lattic
-00002dd0: 6522 3a20 7b22 6d61 7472 6978 223a 205b  e": {"matrix": [
-00002de0: 5b36 2e39 3935 3639 322c 2030 2e30 2c20  [6.995692, 0.0, 
-00002df0: 302e 305d 2c20 5b30 2e30 2c20 362e 3939  0.0], [0.0, 6.99
-00002e00: 3536 3932 2c20 302e 305d 2c20 5b30 2e30  5692, 0.0], [0.0
-00002e10: 2c20 302e 302c 2036 2e39 3935 3639 325d  , 0.0, 6.995692]
-00002e20: 5d2c 2022 6122 3a20 362e 3939 3536 3932  ], "a": 6.995692
-00002e30: 2c20 2262 223a 2036 2e39 3935 3639 322c  , "b": 6.995692,
-00002e40: 2022 6322 3a20 362e 3939 3536 3932 2c20   "c": 6.995692, 
-00002e50: 2261 6c70 6861 223a 2039 302e 302c 2022  "alpha": 90.0, "
-00002e60: 6265 7461 223a 2039 302e 302c 2022 6761  beta": 90.0, "ga
-00002e70: 6d6d 6122 3a20 3930 2e30 2c20 2276 6f6c  mma": 90.0, "vol
-00002e80: 756d 6522 3a20 3334 322e 3336 3731 3133  ume": 342.367113
-00002e90: 3635 3631 3932 3433 7d2c 2022 7369 7465  65619243}, "site
-00002ea0: 7322 3a20 5b7b 2273 7065 6369 6573 223a  s": [{"species":
-00002eb0: 205b 7b22 656c 656d 656e 7422 3a20 2243   [{"element": "C
-00002ec0: 7222 2c20 226f 6363 7522 3a20 317d 5d2c  r", "occu": 1}],
-00002ed0: 2022 6162 6322 3a20 5b30 2e30 2c20 302e   "abc": [0.0, 0.
-00002ee0: 302c 2030 2e30 5d2c 2022 7879 7a22 3a20  0, 0.0], "xyz": 
-00002ef0: 5b30 2e30 2c20 302e 302c 2030 2e30 5d2c  [0.0, 0.0, 0.0],
-00002f00: 2022 6c61 6265 6c22 3a20 2243 7222 2c20   "label": "Cr", 
-00002f10: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00002f20: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00002f30: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-00002f40: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-00002f50: 6162 6322 3a20 5b30 2e30 2c20 302e 302c  abc": [0.0, 0.0,
-00002f60: 2030 2e35 5d2c 2022 7879 7a22 3a20 5b30   0.5], "xyz": [0
-00002f70: 2e30 2c20 302e 302c 2033 2e34 3937 3834  .0, 0.0, 3.49784
-00002f80: 365d 2c20 226c 6162 656c 223a 2022 4e69  6], "label": "Ni
-00002f90: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00002fa0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00002fb0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00002fc0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00002fd0: 2c20 2261 6263 223a 205b 302e 302c 2030  , "abc": [0.0, 0
-00002fe0: 2e35 2c20 302e 305d 2c20 2278 797a 223a  .5, 0.0], "xyz":
-00002ff0: 205b 302e 302c 2033 2e34 3937 3834 362c   [0.0, 3.497846,
-00003000: 2030 2e30 5d2c 2022 6c61 6265 6c22 3a20   0.0], "label": 
-00003010: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-00003020: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00003030: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00003040: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-00003050: 317d 5d2c 2022 6162 6322 3a20 5b30 2e30  1}], "abc": [0.0
-00003060: 2c20 302e 352c 2030 2e35 5d2c 2022 7879  , 0.5, 0.5], "xy
-00003070: 7a22 3a20 5b30 2e30 2c20 332e 3439 3738  z": [0.0, 3.4978
-00003080: 3436 2c20 332e 3439 3738 3436 5d2c 2022  46, 3.497846], "
-00003090: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-000030a0: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-000030b0: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-000030c0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-000030d0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-000030e0: 6322 3a20 5b30 2e35 2c20 302e 302c 2030  c": [0.5, 0.0, 0
-000030f0: 2e30 5d2c 2022 7879 7a22 3a20 5b33 2e34  .0], "xyz": [3.4
-00003100: 3937 3834 362c 2030 2e30 2c20 302e 305d  97846, 0.0, 0.0]
-00003110: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003120: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003130: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003140: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003150: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003160: 2261 6263 223a 205b 302e 352c 2030 2e30  "abc": [0.5, 0.0
-00003170: 2c20 302e 355d 2c20 2278 797a 223a 205b  , 0.5], "xyz": [
-00003180: 332e 3439 3738 3436 2c20 302e 302c 2033  3.497846, 0.0, 3
-00003190: 2e34 3937 3834 365d 2c20 226c 6162 656c  .497846], "label
-000031a0: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-000031b0: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000031c0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000031d0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000031e0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000031f0: 302e 352c 2030 2e35 2c20 302e 305d 2c20  0.5, 0.5, 0.0], 
-00003200: 2278 797a 223a 205b 332e 3439 3738 3436  "xyz": [3.497846
-00003210: 2c20 332e 3439 3738 3436 2c20 302e 305d  , 3.497846, 0.0]
-00003220: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003230: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003240: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003250: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003260: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003270: 2261 6263 223a 205b 302e 352c 2030 2e35  "abc": [0.5, 0.5
-00003280: 2c20 302e 355d 2c20 2278 797a 223a 205b  , 0.5], "xyz": [
-00003290: 332e 3439 3738 3436 2c20 332e 3439 3738  3.497846, 3.4978
-000032a0: 3436 2c20 332e 3439 3738 3436 5d2c 2022  46, 3.497846], "
-000032b0: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-000032c0: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-000032d0: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-000032e0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-000032f0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00003300: 6322 3a20 5b30 2e32 352c 2030 2e32 352c  c": [0.25, 0.25,
-00003310: 2030 2e30 5d2c 2022 7879 7a22 3a20 5b31   0.0], "xyz": [1
-00003320: 2e37 3438 3932 332c 2031 2e37 3438 3932  .748923, 1.74892
-00003330: 332c 2030 2e30 5d2c 2022 6c61 6265 6c22  3, 0.0], "label"
-00003340: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
-00003350: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
-00003360: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
-00003370: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
-00003380: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
-00003390: 2e32 352c 2030 2e32 352c 2030 2e35 5d2c  .25, 0.25, 0.5],
-000033a0: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
-000033b0: 332c 2031 2e37 3438 3932 332c 2033 2e34  3, 1.748923, 3.4
-000033c0: 3937 3834 365d 2c20 226c 6162 656c 223a  97846], "label":
-000033d0: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-000033e0: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-000033f0: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-00003400: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00003410: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-00003420: 3235 2c20 302e 3735 3030 3030 3030 3030  25, 0.7500000000
-00003430: 3030 3030 3031 2c20 302e 305d 2c20 2278  000001, 0.0], "x
-00003440: 797a 223a 205b 312e 3734 3839 3233 2c20  yz": [1.748923, 
-00003450: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
-00003460: 3035 2c20 302e 305d 2c20 226c 6162 656c  05, 0.0], "label
-00003470: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00003480: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003490: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000034a0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000034b0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000034c0: 302e 3235 2c20 302e 3735 3030 3030 3030  0.25, 0.75000000
-000034d0: 3030 3030 3030 3031 2c20 302e 355d 2c20  00000001, 0.5], 
-000034e0: 2278 797a 223a 205b 312e 3734 3839 3233  "xyz": [1.748923
-000034f0: 2c20 352e 3234 3637 3639 3030 3030 3030  , 5.246769000000
-00003500: 3030 3035 2c20 332e 3439 3738 3436 5d2c  0005, 3.497846],
-00003510: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
-00003520: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00003530: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00003540: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-00003550: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-00003560: 6162 6322 3a20 5b30 2e37 3530 3030 3030  abc": [0.7500000
-00003570: 3030 3030 3030 3030 312c 2030 2e32 352c  000000001, 0.25,
-00003580: 2030 2e30 5d2c 2022 7879 7a22 3a20 5b35   0.0], "xyz": [5
-00003590: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
-000035a0: 352c 2031 2e37 3438 3932 332c 2030 2e30  5, 1.748923, 0.0
-000035b0: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
-000035c0: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
-000035d0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
-000035e0: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
-000035f0: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
-00003600: 2022 6162 6322 3a20 5b30 2e37 3530 3030   "abc": [0.75000
-00003610: 3030 3030 3030 3030 3030 312c 2030 2e32  00000000001, 0.2
-00003620: 352c 2030 2e35 5d2c 2022 7879 7a22 3a20  5, 0.5], "xyz": 
-00003630: 5b35 2e32 3436 3736 3930 3030 3030 3030  [5.2467690000000
-00003640: 3030 352c 2031 2e37 3438 3932 332c 2033  005, 1.748923, 3
-00003650: 2e34 3937 3834 365d 2c20 226c 6162 656c  .497846], "label
-00003660: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00003670: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003680: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-00003690: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000036a0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000036b0: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
-000036c0: 3031 2c20 302e 3735 3030 3030 3030 3030  01, 0.7500000000
-000036d0: 3030 3030 3031 2c20 302e 305d 2c20 2278  000001, 0.0], "x
-000036e0: 797a 223a 205b 352e 3234 3637 3639 3030  yz": [5.24676900
-000036f0: 3030 3030 3030 3035 2c20 352e 3234 3637  00000005, 5.2467
-00003700: 3639 3030 3030 3030 3030 3035 2c20 302e  690000000005, 0.
-00003710: 305d 2c20 226c 6162 656c 223a 2022 4e69  0], "label": "Ni
-00003720: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00003730: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00003740: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00003750: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00003760: 2c20 2261 6263 223a 205b 302e 3735 3030  , "abc": [0.7500
-00003770: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
-00003780: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-00003790: 2c20 302e 355d 2c20 2278 797a 223a 205b  , 0.5], "xyz": [
-000037a0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
-000037b0: 3035 2c20 352e 3234 3637 3639 3030 3030  05, 5.2467690000
-000037c0: 3030 3030 3035 2c20 332e 3439 3738 3436  000005, 3.497846
-000037d0: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
-000037e0: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
-000037f0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
-00003800: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
-00003810: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
-00003820: 2022 6162 6322 3a20 5b30 2e32 352c 2030   "abc": [0.25, 0
-00003830: 2e30 2c20 302e 3235 5d2c 2022 7879 7a22  .0, 0.25], "xyz"
-00003840: 3a20 5b31 2e37 3438 3932 332c 2030 2e30  : [1.748923, 0.0
-00003850: 2c20 312e 3734 3839 3233 5d2c 2022 6c61  , 1.748923], "la
-00003860: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003870: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00003880: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00003890: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-000038a0: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-000038b0: 3a20 5b30 2e32 352c 2030 2e30 2c20 302e  : [0.25, 0.0, 0.
-000038c0: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-000038d0: 5d2c 2022 7879 7a22 3a20 5b31 2e37 3438  ], "xyz": [1.748
-000038e0: 3932 332c 2030 2e30 2c20 352e 3234 3637  923, 0.0, 5.2467
-000038f0: 3639 3030 3030 3030 3030 3035 5d2c 2022  690000000005], "
-00003900: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-00003910: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00003920: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00003930: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-00003940: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00003950: 6322 3a20 5b30 2e32 352c 2030 2e35 2c20  c": [0.25, 0.5, 
-00003960: 302e 3235 5d2c 2022 7879 7a22 3a20 5b31  0.25], "xyz": [1
-00003970: 2e37 3438 3932 332c 2033 2e34 3937 3834  .748923, 3.49784
-00003980: 362c 2031 2e37 3438 3932 335d 2c20 226c  6, 1.748923], "l
-00003990: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-000039a0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-000039b0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-000039c0: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
-000039d0: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-000039e0: 223a 205b 302e 3235 2c20 302e 352c 2030  ": [0.25, 0.5, 0
-000039f0: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
-00003a00: 315d 2c20 2278 797a 223a 205b 312e 3734  1], "xyz": [1.74
-00003a10: 3839 3233 2c20 332e 3439 3738 3436 2c20  8923, 3.497846, 
-00003a20: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
-00003a30: 3035 5d2c 2022 6c61 6265 6c22 3a20 224e  05], "label": "N
-00003a40: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003a50: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003a60: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003a70: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00003a80: 5d2c 2022 6162 6322 3a20 5b30 2e37 3530  ], "abc": [0.750
-00003a90: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
-00003aa0: 2e30 2c20 302e 3235 5d2c 2022 7879 7a22  .0, 0.25], "xyz"
-00003ab0: 3a20 5b35 2e32 3436 3736 3930 3030 3030  : [5.24676900000
-00003ac0: 3030 3030 352c 2030 2e30 2c20 312e 3734  00005, 0.0, 1.74
-00003ad0: 3839 3233 5d2c 2022 6c61 6265 6c22 3a20  8923], "label": 
-00003ae0: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-00003af0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00003b00: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00003b10: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-00003b20: 317d 5d2c 2022 6162 6322 3a20 5b30 2e37  1}], "abc": [0.7
-00003b30: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
-00003b40: 2030 2e30 2c20 302e 3735 3030 3030 3030   0.0, 0.75000000
-00003b50: 3030 3030 3030 3031 5d2c 2022 7879 7a22  00000001], "xyz"
-00003b60: 3a20 5b35 2e32 3436 3736 3930 3030 3030  : [5.24676900000
-00003b70: 3030 3030 352c 2030 2e30 2c20 352e 3234  00005, 0.0, 5.24
-00003b80: 3637 3639 3030 3030 3030 3030 3035 5d2c  67690000000005],
-00003b90: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
-00003ba0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00003bb0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00003bc0: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-00003bd0: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-00003be0: 6162 6322 3a20 5b30 2e37 3530 3030 3030  abc": [0.7500000
-00003bf0: 3030 3030 3030 3030 312c 2030 2e35 2c20  000000001, 0.5, 
-00003c00: 302e 3235 5d2c 2022 7879 7a22 3a20 5b35  0.25], "xyz": [5
-00003c10: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
-00003c20: 352c 2033 2e34 3937 3834 362c 2031 2e37  5, 3.497846, 1.7
-00003c30: 3438 3932 335d 2c20 226c 6162 656c 223a  48923], "label":
-00003c40: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-00003c50: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-00003c60: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-00003c70: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00003c80: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-00003c90: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-00003ca0: 2c20 302e 352c 2030 2e37 3530 3030 3030  , 0.5, 0.7500000
-00003cb0: 3030 3030 3030 3030 315d 2c20 2278 797a  000000001], "xyz
-00003cc0: 223a 205b 352e 3234 3637 3639 3030 3030  ": [5.2467690000
-00003cd0: 3030 3030 3035 2c20 332e 3439 3738 3436  000005, 3.497846
-00003ce0: 2c20 352e 3234 3637 3639 3030 3030 3030  , 5.246769000000
-00003cf0: 3030 3035 5d2c 2022 6c61 6265 6c22 3a20  0005], "label": 
-00003d00: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-00003d10: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00003d20: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00003d30: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-00003d40: 317d 5d2c 2022 6162 6322 3a20 5b30 2e30  1}], "abc": [0.0
-00003d50: 2c20 302e 3235 2c20 302e 3235 5d2c 2022  , 0.25, 0.25], "
-00003d60: 7879 7a22 3a20 5b30 2e30 2c20 312e 3734  xyz": [0.0, 1.74
-00003d70: 3839 3233 2c20 312e 3734 3839 3233 5d2c  8923, 1.748923],
-00003d80: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
-00003d90: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00003da0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00003db0: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-00003dc0: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-00003dd0: 6162 6322 3a20 5b30 2e30 2c20 302e 3235  abc": [0.0, 0.25
-00003de0: 2c20 302e 3735 3030 3030 3030 3030 3030  , 0.750000000000
-00003df0: 3030 3031 5d2c 2022 7879 7a22 3a20 5b30  0001], "xyz": [0
-00003e00: 2e30 2c20 312e 3734 3839 3233 2c20 352e  .0, 1.748923, 5.
-00003e10: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
-00003e20: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
-00003e30: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
-00003e40: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
-00003e50: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
-00003e60: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
-00003e70: 2022 6162 6322 3a20 5b30 2e30 2c20 302e   "abc": [0.0, 0.
-00003e80: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-00003e90: 2c20 302e 3235 5d2c 2022 7879 7a22 3a20  , 0.25], "xyz": 
-00003ea0: 5b30 2e30 2c20 352e 3234 3637 3639 3030  [0.0, 5.24676900
-00003eb0: 3030 3030 3030 3035 2c20 312e 3734 3839  00000005, 1.7489
-00003ec0: 3233 5d2c 2022 6c61 6265 6c22 3a20 224e  23], "label": "N
-00003ed0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003ee0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003ef0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003f00: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00003f10: 5d2c 2022 6162 6322 3a20 5b30 2e30 2c20  ], "abc": [0.0, 
-00003f20: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
-00003f30: 3031 2c20 302e 3735 3030 3030 3030 3030  01, 0.7500000000
-00003f40: 3030 3030 3031 5d2c 2022 7879 7a22 3a20  000001], "xyz": 
-00003f50: 5b30 2e30 2c20 352e 3234 3637 3639 3030  [0.0, 5.24676900
-00003f60: 3030 3030 3030 3035 2c20 352e 3234 3637  00000005, 5.2467
-00003f70: 3639 3030 3030 3030 3030 3035 5d2c 2022  690000000005], "
-00003f80: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-00003f90: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00003fa0: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00003fb0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-00003fc0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00003fd0: 6322 3a20 5b30 2e35 2c20 302e 3235 2c20  c": [0.5, 0.25, 
-00003fe0: 302e 3235 5d2c 2022 7879 7a22 3a20 5b33  0.25], "xyz": [3
-00003ff0: 2e34 3937 3834 362c 2031 2e37 3438 3932  .497846, 1.74892
-00004000: 332c 2031 2e37 3438 3932 335d 2c20 226c  3, 1.748923], "l
-00004010: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-00004020: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-00004030: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-00004040: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
-00004050: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-00004060: 223a 205b 302e 352c 2030 2e32 352c 2030  ": [0.5, 0.25, 0
-00004070: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
-00004080: 315d 2c20 2278 797a 223a 205b 332e 3439  1], "xyz": [3.49
-00004090: 3738 3436 2c20 312e 3734 3839 3233 2c20  7846, 1.748923, 
-000040a0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
-000040b0: 3035 5d2c 2022 6c61 6265 6c22 3a20 224e  05], "label": "N
-000040c0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-000040d0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-000040e0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-000040f0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00004100: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
-00004110: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
-00004120: 3031 2c20 302e 3235 5d2c 2022 7879 7a22  01, 0.25], "xyz"
-00004130: 3a20 5b33 2e34 3937 3834 362c 2035 2e32  : [3.497846, 5.2
-00004140: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
-00004150: 2031 2e37 3438 3932 335d 2c20 226c 6162   1.748923], "lab
-00004160: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
-00004170: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00004180: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00004190: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-000041a0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-000041b0: 205b 302e 352c 2030 2e37 3530 3030 3030   [0.5, 0.7500000
-000041c0: 3030 3030 3030 3030 312c 2030 2e37 3530  000000001, 0.750
-000041d0: 3030 3030 3030 3030 3030 3030 315d 2c20  0000000000001], 
-000041e0: 2278 797a 223a 205b 332e 3439 3738 3436  "xyz": [3.497846
-000041f0: 2c20 352e 3234 3637 3639 3030 3030 3030  , 5.246769000000
-00004200: 3030 3035 2c20 352e 3234 3637 3639 3030  0005, 5.24676900
-00004210: 3030 3030 3030 3035 5d2c 2022 6c61 6265  00000005], "labe
-00004220: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
-00004230: 7274 6965 7322 3a20 7b7d 7d5d 2c20 2240  rties": {}}], "@
-00004240: 7665 7273 696f 6e22 3a20 6e75 6c6c 7dfa  version": null}.
-00004250: 1755 6e72 6563 6f67 6e69 7a65 6420 7465  .Unrecognized te
-00004260: 7374 206e 616d 652e 4e7a 154b 5332 3032  st name.Nz.KS202
-00004270: 325f 5465 7374 5265 7375 6c74 2e63 7376  2_TestResult.csv
-00004280: 7a02 772b 6301 0000 0000 0000 0000 0000  z.w+c...........
-00004290: 0002 0000 0004 0000 0053 0000 0073 1600  .........S...s..
-000042a0: 0000 6700 7c00 5d0e 7d01 7c01 9b00 6400  ..g.|.].}.|...d.
-000042b0: 9d02 9102 7104 5300 2901 da01 0a72 2600  ....q.S.)....r&.
-000042c0: 0000 2902 7227 0000 00da 0176 7226 0000  ..).r'.....vr&..
-000042d0: 0072 2600 0000 7229 0000 0072 5f00 0000  .r&...r)...r_...
-000042e0: f800 0000 722b 0000 007a 1b70 726f 6669  ....r+...z.profi
-000042f0: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
-00004300: 7463 6f6d 703e fa05 446f 6e65 2129 09da  tcomp>..Done!)..
-00004310: 0570 7269 6e74 7202 0000 00da 0966 726f  .printr......fro
-00004320: 6d5f 6469 6374 da04 6a73 6f6e da05 6c6f  m_dict..json..lo
-00004330: 6164 7372 0600 0000 72b2 0000 00da 046f  adsr....r......o
-00004340: 7065 6eda 0a77 7269 7465 6c69 6e65 7329  pen..writelines)
-00004350: 07da 0474 6573 74da 056e 5275 6e73 da06  ...test..nRuns..
-00004360: 6d61 7453 7472 da0a 7374 7275 6374 4c69  matStr..structLi
-00004370: 7374 7293 0000 0072 9400 0000 7295 0000  str....r....r...
-00004380: 0072 2600 0000 7226 0000 0072 2900 0000  .r&...r&...r)...
-00004390: da07 7072 6f66 696c 65e9 0000 0073 1c00  ..profile....s..
-000043a0: 0000 0002 0801 0801 0601 0801 0801 0602  ................
-000043b0: 0801 0401 1601 0c01 0a01 0c01 3201 72d4  ............2.r.
-000043c0: 0000 00e9 e803 0000 6302 0000 0000 0000  ........c.......
-000043d0: 0000 0000 0007 0000 0005 0000 0043 0000  .............C..
-000043e0: 0073 6800 0000 6401 6402 6c00 6d01 7d02  .sh...d.d.l.m.}.
-000043f0: 0100 7c00 6403 6b02 721a 6404 7d03 6e1a  ..|.d.k.r.d.}.n.
-00004400: 7c00 6405 6b02 7228 6406 7d03 6e0c 7402  |.d.k.r(d.}.n.t.
-00004410: 6407 8301 0100 6408 5300 7403 a004 7405  d.....d.S.t...t.
-00004420: a006 7c03 a101 a101 7d04 7c04 6701 7c01  ..|.....}.|.g.|.
-00004430: 1400 7d05 7c02 7407 7c05 6409 640a 8d03  ..}.|.t.|.d.d...
-00004440: 7d06 7402 640b 8301 0100 6408 5300 290c  }.t.d.....d.S.).
-00004450: 7a45 5072 6f66 696c 6573 2074 6865 2064  zEProfiles the d
-00004460: 6573 6372 6970 746f 7220 696e 2070 6172  escriptor in par
-00004470: 616c 6c65 6c20 7573 696e 6720 6f6e 6520  allel using one 
-00004480: 6f66 2074 6865 2074 6573 7420 7374 7275  of the test stru
-00004490: 6374 7572 6573 2e72 0100 0000 2901 da0b  ctures.r....)...
-000044a0: 7072 6f63 6573 735f 6d61 7072 c200 0000  process_mapr....
-000044b0: 72c3 0000 0072 c400 0000 72c5 0000 0072  r....r....r....r
-000044c0: c600 0000 4e72 1300 0000 2901 da0b 6d61  ....Nr....)...ma
-000044d0: 785f 776f 726b 6572 7372 c900 0000 2908  x_workersr....).
-000044e0: da17 7471 646d 2e63 6f6e 7472 6962 2e63  ..tqdm.contrib.c
-000044f0: 6f6e 6375 7272 656e 7472 d600 0000 72ca  oncurrentr....r.
-00004500: 0000 0072 0200 0000 72cb 0000 0072 cc00  ...r....r....r..
-00004510: 0000 72cd 0000 0072 b200 0000 2907 72d0  ..r....r....).r.
-00004520: 0000 0072 d100 0000 72d6 0000 0072 d200  ...r....r....r..
-00004530: 0000 7293 0000 0072 d300 0000 da08 6465  ..r....r......de
-00004540: 7363 4c69 7374 7226 0000 0072 2600 0000  scListr&...r&...
-00004550: 7229 0000 00da 0f70 726f 6669 6c65 5061  r).....profilePa
-00004560: 7261 6c6c 656c fb00 0000 7316 0000 0000  rallel....s.....
-00004570: 020c 0108 0106 0108 0106 0208 0104 0110  ................
-00004580: 020a 010e 0172 da00 0000 da08 5f5f 6d61  .....r......__ma
-00004590: 696e 5f5f 2901 72d0 0000 0072 c400 0000  in__).r....r....
-000045a0: 2901 7201 0000 0029 0272 c200 0000 7213  ).r....).r....r.
-000045b0: 0000 0029 0272 c200 0000 72d5 0000 0029  ...).r....r....)
-000045c0: 2872 3700 0000 da04 7469 6d65 da05 6e75  (r7.....time..nu
-000045d0: 6d70 7972 2c00 0000 da02 6f73 da0d 7079  mpyr,.....os..py
-000045e0: 6d61 7467 656e 2e63 6f72 6572 0200 0000  matgen.corer....
-000045f0: 7203 0000 00da 1b70 796d 6174 6765 6e2e  r......pymatgen.
-00004600: 616e 616c 7973 6973 2e6c 6f63 616c 5f65  analysis.local_e
-00004610: 6e76 7204 0000 00da 1a70 796d 6174 6765  nvr......pymatge
-00004620: 6e2e 7379 6d6d 6574 7279 2e61 6e61 6c79  n.symmetry.analy
-00004630: 7a65 7272 0500 0000 72cc 0000 0072 0600  zerr....r....r..
-00004640: 0000 da0b 636f 6c6c 6563 7469 6f6e 7372  ....collectionsr
-00004650: 0700 0000 da06 7479 7069 6e67 7208 0000  ......typingr...
-00004660: 0072 b300 0000 da13 7065 7269 6f64 6963  .r......periodic
-00004670: 5f74 6162 6c65 5f73 697a 65da 076c 6f61  _table_size..loa
-00004680: 6474 7874 da04 7061 7468 da04 6a6f 696e  dtxt..path..join
-00004690: da07 6469 726e 616d 65da 085f 5f66 696c  ..dirname..__fil
-000046a0: 655f 5f72 2e00 0000 da0a 6e61 6e5f 746f  e__r......nan_to
-000046b0: 5f6e 756d 724b 0000 0072 4c00 0000 7266  _numrK...rL...rf
-000046c0: 0000 0072 7a00 0000 7261 0000 0072 bf00  ...rz...ra...r..
-000046d0: 0000 72b2 0000 00da 0373 7472 72b4 0000  ..r......strr...
-000046e0: 0072 c100 0000 72d4 0000 0072 da00 0000  .r....r....r....
-000046f0: 725a 0000 0072 2600 0000 7226 0000 0072  rZ...r&...r&...r
-00004700: 2600 0000 7229 0000 00da 083c 6d6f 6475  &...r).....<modu
-00004710: 6c65 3e05 0000 0073 4000 0000 0801 0801  le>....s@.......
-00004720: 0801 0801 1001 0c01 0c01 0801 0c01 0c01  ................
-00004730: 0c02 0605 0401 2001 0a02 0801 06ff 0603  ...... .........
-00004740: 0833 0e0e 0c0f 0a13 0e05 1248 1204 1418  .3.........H....
-00004750: 0a12 0a10 0a01 0a01 0a01 0a01            ............
+00002170: 0800 0000 4300 0000 73be 0000 007c 0064  ....C...s....|.d
+00002180: 016b 0272 1e74 0064 027c 019b 0064 039d  .k.r.t.d.|...d..
+00002190: 0383 0101 0064 047d 026e 2a7c 0064 056b  .....d.}.n*|.d.k
+000021a0: 0272 3c74 0064 067c 019b 0064 039d 0383  .r<t.d.|...d....
+000021b0: 0101 0064 077d 026e 0c74 0064 0883 0101  ...d.}.n.t.d....
+000021c0: 0064 0953 0074 01a0 0274 03a0 047c 02a1  .d.S.t...t...|..
+000021d0: 01a1 0167 017c 0114 007d 0374 057c 0383  ...g.|...}.t.|..
+000021e0: 0144 005d 0c7d 0474 067c 0483 017d 0571  .D.].}.t.|...}.q
+000021f0: 6674 0764 0a64 0b83 028f 247d 067c 06a0  ft.d.d....$}.|..
+00002200: 0864 0c64 0d84 007c 0544 0083 01a1 0101  .d.d...|.D......
+00002210: 0057 0064 0904 0004 0083 0301 006e 1031  .W.d.........n.1
+00002220: 0073 a830 0001 0001 0001 0059 0001 0074  .s.0.......Y...t
+00002230: 0064 0e83 0101 0064 0953 0029 0f7a 4350  .d.....d.S.).zCP
+00002240: 726f 6669 6c65 7320 7468 6520 6465 7363  rofiles the desc
+00002250: 7269 7074 6f72 2069 6e20 7365 7269 6573  riptor in series
+00002260: 2075 7369 6e67 206f 6e65 206f 6620 7468   using one of th
+00002270: 6520 7465 7374 2073 7472 7563 7475 7265  e test structure
+00002280: 732e 72c2 0000 00fa 5b4b 5332 3032 3220  s.r.....[KS2022 
+00002290: 7072 6f66 696c 696e 672f 7465 7374 696e  profiling/testin
+000022a0: 6720 7461 736b 2077 696c 6c20 6361 6c63  g task will calc
+000022b0: 756c 6174 6520 6120 6465 7363 7269 7074  ulate a descript
+000022c0: 6f72 2066 6f72 204c 6932 205a 7231 2054  or for Li2 Zr1 T
+000022d0: 6531 204f 3620 284a 5641 5350 2d31 3030  e1 O6 (JVASP-100
+000022e0: 3031 2920 7a11 2074 696d 6573 2069 6e20  01) z. times in 
+000022f0: 7365 7269 6573 2ee1 460a 0000 7b22 406d  series..F...{"@m
+00002300: 6f64 756c 6522 3a20 2270 796d 6174 6765  odule": "pymatge
+00002310: 6e2e 636f 7265 2e73 7472 7563 7475 7265  n.core.structure
+00002320: 222c 2022 4063 6c61 7373 223a 2022 5374  ", "@class": "St
+00002330: 7275 6374 7572 6522 2c20 2263 6861 7267  ructure", "charg
+00002340: 6522 3a20 6e75 6c6c 2c20 226c 6174 7469  e": null, "latti
+00002350: 6365 223a 207b 226d 6174 7269 7822 3a20  ce": {"matrix": 
+00002360: 5b5b 342e 3539 3933 3035 3635 3236 3632  [[4.599305652662
+00002370: 3435 392c 2030 2e30 3039 3830 3135 3037  459, 0.009801507
+00002380: 3639 3938 3832 332c 2033 2e31 3035 3236  6998823, 3.10526
+00002390: 3132 3836 3534 3433 3733 365d 2c20 5b31  12865443736], [1
+000023a0: 2e36 3535 3332 3537 3732 3632 3034 3635  .655325772620465
+000023b0: 332c 2034 2e32 3931 3130 3834 3735 3835  3, 4.29110847585
+000023c0: 3437 3132 2c20 332e 3130 3532 3630 3239  4712, 3.10526029
+000023d0: 3338 3937 3935 3635 5d2c 205b 302e 3031  38979565], [0.01
+000023e0: 3432 3534 3132 3134 3931 3937 3439 2c20  42541214919749, 
+000023f0: 302e 3030 3938 3032 3530 3939 3939 3631  0.00980250999961
+00002400: 3331 2c20 352e 3534 3934 3139 3134 3138  31, 5.5494191418
+00002410: 3636 3335 315d 5d2c 2022 6122 3a20 352e  66351]], "a": 5.
+00002420: 3534 3934 3436 3437 3831 3532 3332 362c  549446478152326,
+00002430: 2022 6222 3a20 352e 3534 3934 3436 3533   "b": 5.54944653
+00002440: 3631 3739 3334 332c 2022 6322 3a20 352e  6179343, "c": 5.
+00002450: 3534 3934 3436 3130 3538 3130 3432 332c  549446105810423,
+00002460: 2022 616c 7068 6122 3a20 3535 2e38 3237   "alpha": 55.827
+00002470: 3134 3435 3939 3835 3833 322c 2022 6265  14459985832, "be
+00002480: 7461 223a 2035 352e 3832 3731 3430 3134  ta": 55.82714014
+00002490: 3238 3933 3731 2c20 2267 616d 6d61 223a  289371, "gamma":
+000024a0: 2035 352e 3832 3731 3339 3732 3737 3930   55.827139727790
+000024b0: 3932 2c20 2276 6f6c 756d 6522 3a20 3130  92, "volume": 10
+000024c0: 392e 3135 3438 3436 3235 3634 3237 3433  9.15484625642743
+000024d0: 7d2c 2022 7369 7465 7322 3a20 5b7b 2273  }, "sites": [{"s
+000024e0: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+000024f0: 656e 7422 3a20 224c 6922 2c20 226f 6363  ent": "Li", "occ
+00002500: 7522 3a20 312e 307d 5d2c 2022 6162 6322  u": 1.0}], "abc"
+00002510: 3a20 5b30 2e32 3733 3837 3834 3837 3236  : [0.27387848726
+00002520: 3639 3932 342c 2030 2e32 3733 3837 3834  69924, 0.2738784
+00002530: 3837 3236 3730 3430 372c 2030 2e32 3733  872670407, 0.273
+00002540: 3837 3834 3837 3236 3733 3033 325d 2c20  8784872673032], 
+00002550: 2278 797a 223a 205b 312e 3731 3639 3132  "xyz": [1.716912
+00002560: 3839 3034 3030 3730 3633 2c20 312e 3138  8904007063, 1.18
+00002570: 3036 3131 3431 3637 3737 3736 3133 2c20  06114167777613, 
+00002580: 332e 3232 3037 3934 3737 3533 3737 3237  3.22079477537727
+00002590: 385d 2c20 226c 6162 656c 223a 2022 4c69  8], "label": "Li
+000025a0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000025b0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000025c0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+000025d0: 4c69 222c 2022 6f63 6375 223a 2031 2e30  Li", "occu": 1.0
+000025e0: 7d5d 2c20 2261 6263 223a 205b 302e 3738  }], "abc": [0.78
+000025f0: 3532 3237 3230 3130 3732 3830 3639 2c20  52272010728069, 
+00002600: 302e 3738 3532 3237 3230 3130 3732 3838  0.78522720107288
+00002610: 3536 2c20 302e 3738 3532 3237 3230 3130  56, 0.7852272010
+00002620: 3733 3331 355d 2c20 2278 797a 223a 205b  73315], "xyz": [
+00002630: 342e 3932 3234 3939 3435 3137 3339 3936  4.92249945173996
+00002640: 352c 2033 2e33 3834 3838 3837 3035 3934  5, 3.38488870594
+00002650: 3334 3932 372c 2039 2e32 3334 3232 3533  34927, 9.2342253
+00002660: 3338 3136 3336 3333 5d2c 2022 6c61 6265  38163633], "labe
+00002670: 6c22 3a20 224c 6922 2c20 2270 726f 7065  l": "Li", "prope
+00002680: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00002690: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+000026a0: 656e 7422 3a20 224f 222c 2022 6f63 6375  ent": "O", "occu
+000026b0: 223a 2031 2e30 7d5d 2c20 2261 6263 223a  ": 1.0}], "abc":
+000026c0: 205b 302e 3836 3639 3936 3434 3534 3636   [0.866996445466
+000026d0: 3131 3234 2c20 302e 3630 3430 3839 3838  1124, 0.60408988
+000026e0: 3230 3932 3131 342c 2030 2e32 3431 3832  2092114, 0.24182
+000026f0: 3137 3639 3837 3331 3433 5d2c 2022 7879  1769873143], "xy
+00002700: 7a22 3a20 5b34 2e39 3930 3939 3431 3630  z": [4.990994160
+00002710: 3136 3430 3631 2c20 322e 3630 3330 3833  164061, 2.603083
+00002720: 3534 3538 3736 3835 362c 2035 2e39 3130  545876856, 5.910
+00002730: 3037 3731 3831 3133 3736 3538 5d2c 2022  077181137658], "
+00002740: 6c61 6265 6c22 3a20 224f 222c 2022 7072  label": "O", "pr
+00002750: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00002760: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00002770: 6c65 6d65 6e74 223a 2022 4f22 2c20 226f  lement": "O", "o
+00002780: 6363 7522 3a20 312e 307d 5d2c 2022 6162  ccu": 1.0}], "ab
+00002790: 6322 3a20 5b30 2e37 3137 3834 3038 3934  c": [0.717840894
+000027a0: 3532 3937 3838 2c20 302e 3132 3133 3637  529788, 0.121367
+000027b0: 3538 3839 3632 3836 3833 2c20 302e 3339  5889628683, 0.39
+000027c0: 3335 3337 3030 3931 3836 3937 335d 2c20  3537009186973], 
+000027d0: 2278 797a 223a 205b 332e 3530 3830 3832  "xyz": [3.508082
+000027e0: 3130 3632 3334 3731 332c 2030 2e35 3331  106234713, 0.531
+000027f0: 3639 3530 3633 3231 3534 3132 2c20 342e  695063215412, 4.
+00002800: 3738 3938 3633 3330 3634 3639 3237 385d  789863306469278]
+00002810: 2c20 226c 6162 656c 223a 2022 4f22 2c20  , "label": "O", 
+00002820: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00002830: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00002840: 7b22 656c 656d 656e 7422 3a20 224f 222c  {"element": "O",
+00002850: 2022 6f63 6375 223a 2031 2e30 7d5d 2c20   "occu": 1.0}], 
+00002860: 2261 6263 223a 205b 302e 3132 3133 3637  "abc": [0.121367
+00002870: 3538 3839 3633 3834 3032 2c20 302e 3339  5889638402, 0.39
+00002880: 3335 3337 3030 3931 3837 3339 3433 2c20  35370091873943, 
+00002890: 302e 3731 3738 3430 3839 3435 3238 3333  0.71784089452833
+000028a0: 3834 5d2c 2022 7879 7a22 3a20 5b31 2e32  84], "xyz": [1.2
+000028b0: 3139 3837 3037 3833 3038 3137 3839 362c  198707830817896,
+000028c0: 2031 2e36 3936 3933 3632 3233 3539 3130   1.6969362235910
+000028d0: 3331 372c 2035 2e35 3832 3531 3239 3235  317, 5.582512925
+000028e0: 3136 3936 345d 2c20 226c 6162 656c 223a  16964], "label":
+000028f0: 2022 4f22 2c20 2270 726f 7065 7274 6965   "O", "propertie
+00002900: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00002910: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00002920: 3a20 224f 222c 2022 6f63 6375 223a 2031  : "O", "occu": 1
+00002930: 2e30 7d5d 2c20 2261 6263 223a 205b 302e  .0}], "abc": [0.
+00002940: 3339 3335 3337 3030 3931 3836 3139 3135  3935370091861915
+00002950: 2c20 302e 3731 3738 3430 3839 3435 3239  , 0.717840894529
+00002960: 3338 3536 2c20 302e 3132 3133 3637 3538  3856, 0.12136758
+00002970: 3839 3633 3430 3134 5d2c 2022 7879 7a22  89634014], "xyz"
+00002980: 3a20 5b32 2e39 3939 3938 3735 3132 3539  : [2.99998751259
+00002990: 3536 3232 2c20 332e 3038 3533 3830 3130  5622, 3.08538010
+000029a0: 3938 3630 3334 342c 2034 2e31 3234 3633  9860344, 4.12463
+000029b0: 3736 3837 3936 3232 3937 5d2c 2022 6c61  7687962297], "la
+000029c0: 6265 6c22 3a20 224f 222c 2022 7072 6f70  bel": "O", "prop
+000029d0: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+000029e0: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+000029f0: 6d65 6e74 223a 2022 4f22 2c20 226f 6363  ment": "O", "occ
+00002a00: 7522 3a20 312e 307d 5d2c 2022 6162 6322  u": 1.0}], "abc"
+00002a10: 3a20 5b30 2e32 3431 3832 3137 3639 3837  : [0.24182176987
+00002a20: 3231 3537 332c 2030 2e38 3636 3939 3634  21573, 0.8669964
+00002a30: 3435 3436 3731 3232 312c 2030 2e36 3034  454671221, 0.604
+00002a40: 3038 3938 3832 3039 3231 3531 335d 2c20  0898820921513], 
+00002a50: 2278 797a 223a 205b 322e 3535 3539 3834  "xyz": [2.555984
+00002a60: 3536 3436 3333 3332 392c 2033 2e37 3238  564633329, 3.728
+00002a70: 3636 3736 3130 3732 3931 3439 2c20 362e  667610729149, 6.
+00002a80: 3739 3535 3137 3337 3233 3737 3334 335d  795517372377343]
+00002a90: 2c20 226c 6162 656c 223a 2022 4f22 2c20  , "label": "O", 
+00002aa0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00002ab0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00002ac0: 7b22 656c 656d 656e 7422 3a20 224f 222c  {"element": "O",
+00002ad0: 2022 6f63 6375 223a 2031 2e30 7d5d 2c20   "occu": 1.0}], 
+00002ae0: 2261 6263 223a 205b 302e 3630 3430 3839  "abc": [0.604089
+00002af0: 3838 3230 3933 3331 3135 2c20 302e 3234  8820933115, 0.24
+00002b00: 3138 3231 3736 3938 3732 3336 3337 2c20  18217698723637, 
+00002b10: 302e 3836 3639 3936 3434 3534 3636 3430  0.86699644546640
+00002b20: 3539 5d2c 2022 7879 7a22 3a20 5b33 2e31  59], "xyz": [3.1
+00002b30: 3931 3034 3630 3930 3134 3531 3733 2c20  91046090145173, 
+00002b40: 312e 3035 3231 3033 3137 3933 3032 3535  1.05210317930255
+00002b50: 3935 2c20 372e 3433 3831 3033 3133 3530  95, 7.4381031350
+00002b60: 3433 3635 3335 5d2c 2022 6c61 6265 6c22  436535], "label"
+00002b70: 3a20 224f 222c 2022 7072 6f70 6572 7469  : "O", "properti
+00002b80: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
+00002b90: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
+00002ba0: 223a 2022 5465 222c 2022 6f63 6375 223a  ": "Te", "occu":
+00002bb0: 2031 2e30 7d5d 2c20 2261 6263 223a 205b   1.0}], "abc": [
+00002bc0: 302e 3439 3635 3930 3536 3130 3530 3733  0.49659056105073
+00002bd0: 3533 2c20 302e 3439 3635 3930 3536 3130  53, 0.4965905610
+00002be0: 3530 3733 3535 2c20 302e 3439 3635 3930  507355, 0.496590
+00002bf0: 3536 3130 3530 3733 3631 5d2c 2022 7879  5610507361], "xy
+00002c00: 7a22 3a20 5b33 2e31 3133 3036 3933 3930  z": [3.113069390
+00002c10: 3833 3537 3933 2c20 322e 3134 3036 3539  835793, 2.140659
+00002c20: 3133 3537 3032 3439 3834 2c20 352e 3833  1357024984, 5.83
+00002c30: 3938 3735 3536 3132 3134 3636 3234 5d2c  98755612146624],
+00002c40: 2022 6c61 6265 6c22 3a20 2254 6522 2c20   "label": "Te", 
+00002c50: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00002c60: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00002c70: 7b22 656c 656d 656e 7422 3a20 225a 7222  {"element": "Zr"
+00002c80: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
+00002c90: 2022 6162 6322 3a20 5b30 2e30 3030 3635   "abc": [0.00065
+00002ca0: 3031 3630 3439 3830 3636 382c 2030 2e30  01604980668, 0.0
+00002cb0: 3030 3635 3031 3630 3439 3830 3932 382c  006501604980928,
+00002cc0: 2030 2e30 3030 3635 3031 3630 3439 3832   0.0006501604982
+00002cd0: 3334 345d 2c20 2278 797a 223a 205b 302e  344], "xyz": [0.
+00002ce0: 3030 3430 3735 3738 3137 3439 3436 3033  0040757817494603
+00002cf0: 362c 2030 2e30 3032 3830 3236 3534 3938  6, 0.00280265498
+00002d00: 3139 3435 3139 322c 2030 2e30 3037 3634  1945192, 0.00764
+00002d10: 3538 3438 3931 3832 3633 3037 365d 2c20  5848918263076], 
+00002d20: 226c 6162 656c 223a 2022 5a72 222c 2022  "label": "Zr", "
+00002d30: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+00002d40: 5d7d da0d 6469 6c75 7465 4e69 416c 6c6f  ]}..diluteNiAllo
+00002d50: 79fa 594b 5332 3032 3220 7072 6f66 696c  y.YKS2022 profil
+00002d60: 696e 672f 7465 7374 696e 6720 7461 736b  ing/testing task
+00002d70: 2077 696c 6c20 6361 6c63 756c 6174 6520   will calculate 
+00002d80: 6120 6465 7363 7269 7074 6f72 2066 6f72  a descriptor for
+00002d90: 2061 2064 696c 7574 6520 4643 4320 4e69   a dilute FCC Ni
+00002da0: 3331 4372 3120 616c 6c6f 7920 e1d4 1400  31Cr1 alloy ....
+00002db0: 007b 2240 6d6f 6475 6c65 223a 2022 7079  .{"@module": "py
+00002dc0: 6d61 7467 656e 2e63 6f72 652e 7374 7275  matgen.core.stru
+00002dd0: 6374 7572 6522 2c20 2240 636c 6173 7322  cture", "@class"
+00002de0: 3a20 2253 7472 7563 7475 7265 222c 2022  : "Structure", "
+00002df0: 6368 6172 6765 223a 206e 756c 6c2c 2022  charge": null, "
+00002e00: 6c61 7474 6963 6522 3a20 7b22 6d61 7472  lattice": {"matr
+00002e10: 6978 223a 205b 5b36 2e39 3935 3639 322c  ix": [[6.995692,
+00002e20: 2030 2e30 2c20 302e 305d 2c20 5b30 2e30   0.0, 0.0], [0.0
+00002e30: 2c20 362e 3939 3536 3932 2c20 302e 305d  , 6.995692, 0.0]
+00002e40: 2c20 5b30 2e30 2c20 302e 302c 2036 2e39  , [0.0, 0.0, 6.9
+00002e50: 3935 3639 325d 5d2c 2022 6122 3a20 362e  95692]], "a": 6.
+00002e60: 3939 3536 3932 2c20 2262 223a 2036 2e39  995692, "b": 6.9
+00002e70: 3935 3639 322c 2022 6322 3a20 362e 3939  95692, "c": 6.99
+00002e80: 3536 3932 2c20 2261 6c70 6861 223a 2039  5692, "alpha": 9
+00002e90: 302e 302c 2022 6265 7461 223a 2039 302e  0.0, "beta": 90.
+00002ea0: 302c 2022 6761 6d6d 6122 3a20 3930 2e30  0, "gamma": 90.0
+00002eb0: 2c20 2276 6f6c 756d 6522 3a20 3334 322e  , "volume": 342.
+00002ec0: 3336 3731 3133 3635 3631 3932 3433 7d2c  36711365619243},
+00002ed0: 2022 7369 7465 7322 3a20 5b7b 2273 7065   "sites": [{"spe
+00002ee0: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00002ef0: 7422 3a20 2243 7222 2c20 226f 6363 7522  t": "Cr", "occu"
+00002f00: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00002f10: 2e30 2c20 302e 302c 2030 2e30 5d2c 2022  .0, 0.0, 0.0], "
+00002f20: 7879 7a22 3a20 5b30 2e30 2c20 302e 302c  xyz": [0.0, 0.0,
+00002f30: 2030 2e30 5d2c 2022 6c61 6265 6c22 3a20   0.0], "label": 
+00002f40: 2243 7222 2c20 2270 726f 7065 7274 6965  "Cr", "propertie
+00002f50: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00002f60: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00002f70: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00002f80: 317d 5d2c 2022 6162 6322 3a20 5b30 2e30  1}], "abc": [0.0
+00002f90: 2c20 302e 302c 2030 2e35 5d2c 2022 7879  , 0.0, 0.5], "xy
+00002fa0: 7a22 3a20 5b30 2e30 2c20 302e 302c 2033  z": [0.0, 0.0, 3
+00002fb0: 2e34 3937 3834 365d 2c20 226c 6162 656c  .497846], "label
+00002fc0: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
+00002fd0: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
+00002fe0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
+00002ff0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
+00003000: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
+00003010: 302e 302c 2030 2e35 2c20 302e 305d 2c20  0.0, 0.5, 0.0], 
+00003020: 2278 797a 223a 205b 302e 302c 2033 2e34  "xyz": [0.0, 3.4
+00003030: 3937 3834 362c 2030 2e30 5d2c 2022 6c61  97846, 0.0], "la
+00003040: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00003050: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00003060: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00003070: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+00003080: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00003090: 3a20 5b30 2e30 2c20 302e 352c 2030 2e35  : [0.0, 0.5, 0.5
+000030a0: 5d2c 2022 7879 7a22 3a20 5b30 2e30 2c20  ], "xyz": [0.0, 
+000030b0: 332e 3439 3738 3436 2c20 332e 3439 3738  3.497846, 3.4978
+000030c0: 3436 5d2c 2022 6c61 6265 6c22 3a20 224e  46], "label": "N
+000030d0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+000030e0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+000030f0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00003100: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00003110: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
+00003120: 302e 302c 2030 2e30 5d2c 2022 7879 7a22  0.0, 0.0], "xyz"
+00003130: 3a20 5b33 2e34 3937 3834 362c 2030 2e30  : [3.497846, 0.0
+00003140: 2c20 302e 305d 2c20 226c 6162 656c 223a  , 0.0], "label":
+00003150: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
+00003160: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
+00003170: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
+00003180: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
+00003190: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
+000031a0: 352c 2030 2e30 2c20 302e 355d 2c20 2278  5, 0.0, 0.5], "x
+000031b0: 797a 223a 205b 332e 3439 3738 3436 2c20  yz": [3.497846, 
+000031c0: 302e 302c 2033 2e34 3937 3834 365d 2c20  0.0, 3.497846], 
+000031d0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+000031e0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+000031f0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+00003200: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+00003210: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+00003220: 6263 223a 205b 302e 352c 2030 2e35 2c20  bc": [0.5, 0.5, 
+00003230: 302e 305d 2c20 2278 797a 223a 205b 332e  0.0], "xyz": [3.
+00003240: 3439 3738 3436 2c20 332e 3439 3738 3436  497846, 3.497846
+00003250: 2c20 302e 305d 2c20 226c 6162 656c 223a  , 0.0], "label":
+00003260: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
+00003270: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
+00003280: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
+00003290: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
+000032a0: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
+000032b0: 352c 2030 2e35 2c20 302e 355d 2c20 2278  5, 0.5, 0.5], "x
+000032c0: 797a 223a 205b 332e 3439 3738 3436 2c20  yz": [3.497846, 
+000032d0: 332e 3439 3738 3436 2c20 332e 3439 3738  3.497846, 3.4978
+000032e0: 3436 5d2c 2022 6c61 6265 6c22 3a20 224e  46], "label": "N
+000032f0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00003300: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+00003310: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00003320: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00003330: 5d2c 2022 6162 6322 3a20 5b30 2e32 352c  ], "abc": [0.25,
+00003340: 2030 2e32 352c 2030 2e30 5d2c 2022 7879   0.25, 0.0], "xy
+00003350: 7a22 3a20 5b31 2e37 3438 3932 332c 2031  z": [1.748923, 1
+00003360: 2e37 3438 3932 332c 2030 2e30 5d2c 2022  .748923, 0.0], "
+00003370: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00003380: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00003390: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+000033a0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+000033b0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+000033c0: 6322 3a20 5b30 2e32 352c 2030 2e32 352c  c": [0.25, 0.25,
+000033d0: 2030 2e35 5d2c 2022 7879 7a22 3a20 5b31   0.5], "xyz": [1
+000033e0: 2e37 3438 3932 332c 2031 2e37 3438 3932  .748923, 1.74892
+000033f0: 332c 2033 2e34 3937 3834 365d 2c20 226c  3, 3.497846], "l
+00003400: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00003410: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00003420: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00003430: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00003440: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00003450: 223a 205b 302e 3235 2c20 302e 3735 3030  ": [0.25, 0.7500
+00003460: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00003470: 305d 2c20 2278 797a 223a 205b 312e 3734  0], "xyz": [1.74
+00003480: 3839 3233 2c20 352e 3234 3637 3639 3030  8923, 5.24676900
+00003490: 3030 3030 3030 3035 2c20 302e 305d 2c20  00000005, 0.0], 
+000034a0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+000034b0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+000034c0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+000034d0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+000034e0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+000034f0: 6263 223a 205b 302e 3235 2c20 302e 3735  bc": [0.25, 0.75
+00003500: 3030 3030 3030 3030 3030 3030 3031 2c20  00000000000001, 
+00003510: 302e 355d 2c20 2278 797a 223a 205b 312e  0.5], "xyz": [1.
+00003520: 3734 3839 3233 2c20 352e 3234 3637 3639  748923, 5.246769
+00003530: 3030 3030 3030 3030 3035 2c20 332e 3439  0000000005, 3.49
+00003540: 3738 3436 5d2c 2022 6c61 6265 6c22 3a20  7846], "label": 
+00003550: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00003560: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00003570: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00003580: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00003590: 317d 5d2c 2022 6162 6322 3a20 5b30 2e37  1}], "abc": [0.7
+000035a0: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+000035b0: 2030 2e32 352c 2030 2e30 5d2c 2022 7879   0.25, 0.0], "xy
+000035c0: 7a22 3a20 5b35 2e32 3436 3736 3930 3030  z": [5.246769000
+000035d0: 3030 3030 3030 352c 2031 2e37 3438 3932  0000005, 1.74892
+000035e0: 332c 2030 2e30 5d2c 2022 6c61 6265 6c22  3, 0.0], "label"
+000035f0: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00003600: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00003610: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00003620: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00003630: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00003640: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
+00003650: 312c 2030 2e32 352c 2030 2e35 5d2c 2022  1, 0.25, 0.5], "
+00003660: 7879 7a22 3a20 5b35 2e32 3436 3736 3930  xyz": [5.2467690
+00003670: 3030 3030 3030 3030 352c 2031 2e37 3438  000000005, 1.748
+00003680: 3932 332c 2033 2e34 3937 3834 365d 2c20  923, 3.497846], 
+00003690: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+000036a0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+000036b0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+000036c0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+000036d0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+000036e0: 6263 223a 205b 302e 3735 3030 3030 3030  bc": [0.75000000
+000036f0: 3030 3030 3030 3031 2c20 302e 3735 3030  00000001, 0.7500
+00003700: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00003710: 305d 2c20 2278 797a 223a 205b 352e 3234  0], "xyz": [5.24
+00003720: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00003730: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00003740: 3035 2c20 302e 305d 2c20 226c 6162 656c  05, 0.0], "label
+00003750: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
+00003760: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
+00003770: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
+00003780: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
+00003790: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
+000037a0: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
+000037b0: 3031 2c20 302e 3735 3030 3030 3030 3030  01, 0.7500000000
+000037c0: 3030 3030 3031 2c20 302e 355d 2c20 2278  000001, 0.5], "x
+000037d0: 797a 223a 205b 352e 3234 3637 3639 3030  yz": [5.24676900
+000037e0: 3030 3030 3030 3035 2c20 352e 3234 3637  00000005, 5.2467
+000037f0: 3639 3030 3030 3030 3030 3035 2c20 332e  690000000005, 3.
+00003800: 3439 3738 3436 5d2c 2022 6c61 6265 6c22  497846], "label"
+00003810: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00003820: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00003830: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00003840: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00003850: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00003860: 2e32 352c 2030 2e30 2c20 302e 3235 5d2c  .25, 0.0, 0.25],
+00003870: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
+00003880: 332c 2030 2e30 2c20 312e 3734 3839 3233  3, 0.0, 1.748923
+00003890: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
+000038a0: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
+000038b0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
+000038c0: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
+000038d0: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
+000038e0: 2022 6162 6322 3a20 5b30 2e32 352c 2030   "abc": [0.25, 0
+000038f0: 2e30 2c20 302e 3735 3030 3030 3030 3030  .0, 0.7500000000
+00003900: 3030 3030 3031 5d2c 2022 7879 7a22 3a20  000001], "xyz": 
+00003910: 5b31 2e37 3438 3932 332c 2030 2e30 2c20  [1.748923, 0.0, 
+00003920: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00003930: 3035 5d2c 2022 6c61 6265 6c22 3a20 224e  05], "label": "N
+00003940: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00003950: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+00003960: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00003970: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00003980: 5d2c 2022 6162 6322 3a20 5b30 2e32 352c  ], "abc": [0.25,
+00003990: 2030 2e35 2c20 302e 3235 5d2c 2022 7879   0.5, 0.25], "xy
+000039a0: 7a22 3a20 5b31 2e37 3438 3932 332c 2033  z": [1.748923, 3
+000039b0: 2e34 3937 3834 362c 2031 2e37 3438 3932  .497846, 1.74892
+000039c0: 335d 2c20 226c 6162 656c 223a 2022 4e69  3], "label": "Ni
+000039d0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000039e0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000039f0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+00003a00: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00003a10: 2c20 2261 6263 223a 205b 302e 3235 2c20  , "abc": [0.25, 
+00003a20: 302e 352c 2030 2e37 3530 3030 3030 3030  0.5, 0.750000000
+00003a30: 3030 3030 3030 315d 2c20 2278 797a 223a  0000001], "xyz":
+00003a40: 205b 312e 3734 3839 3233 2c20 332e 3439   [1.748923, 3.49
+00003a50: 3738 3436 2c20 352e 3234 3637 3639 3030  7846, 5.24676900
+00003a60: 3030 3030 3030 3035 5d2c 2022 6c61 6265  00000005], "labe
+00003a70: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+00003a80: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00003a90: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00003aa0: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00003ab0: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00003ac0: 5b30 2e37 3530 3030 3030 3030 3030 3030  [0.7500000000000
+00003ad0: 3030 312c 2030 2e30 2c20 302e 3235 5d2c  001, 0.0, 0.25],
+00003ae0: 2022 7879 7a22 3a20 5b35 2e32 3436 3736   "xyz": [5.24676
+00003af0: 3930 3030 3030 3030 3030 352c 2030 2e30  90000000005, 0.0
+00003b00: 2c20 312e 3734 3839 3233 5d2c 2022 6c61  , 1.748923], "la
+00003b10: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00003b20: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00003b30: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00003b40: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+00003b50: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00003b60: 3a20 5b30 2e37 3530 3030 3030 3030 3030  : [0.75000000000
+00003b70: 3030 3030 312c 2030 2e30 2c20 302e 3735  00001, 0.0, 0.75
+00003b80: 3030 3030 3030 3030 3030 3030 3031 5d2c  00000000000001],
+00003b90: 2022 7879 7a22 3a20 5b35 2e32 3436 3736   "xyz": [5.24676
+00003ba0: 3930 3030 3030 3030 3030 352c 2030 2e30  90000000005, 0.0
+00003bb0: 2c20 352e 3234 3637 3639 3030 3030 3030  , 5.246769000000
+00003bc0: 3030 3035 5d2c 2022 6c61 6265 6c22 3a20  0005], "label": 
+00003bd0: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00003be0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00003bf0: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00003c00: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00003c10: 317d 5d2c 2022 6162 6322 3a20 5b30 2e37  1}], "abc": [0.7
+00003c20: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+00003c30: 2030 2e35 2c20 302e 3235 5d2c 2022 7879   0.5, 0.25], "xy
+00003c40: 7a22 3a20 5b35 2e32 3436 3736 3930 3030  z": [5.246769000
+00003c50: 3030 3030 3030 352c 2033 2e34 3937 3834  0000005, 3.49784
+00003c60: 362c 2031 2e37 3438 3932 335d 2c20 226c  6, 1.748923], "l
+00003c70: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00003c80: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00003c90: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00003ca0: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00003cb0: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00003cc0: 223a 205b 302e 3735 3030 3030 3030 3030  ": [0.7500000000
+00003cd0: 3030 3030 3031 2c20 302e 352c 2030 2e37  000001, 0.5, 0.7
+00003ce0: 3530 3030 3030 3030 3030 3030 3030 315d  500000000000001]
+00003cf0: 2c20 2278 797a 223a 205b 352e 3234 3637  , "xyz": [5.2467
+00003d00: 3639 3030 3030 3030 3030 3035 2c20 332e  690000000005, 3.
+00003d10: 3439 3738 3436 2c20 352e 3234 3637 3639  497846, 5.246769
+00003d20: 3030 3030 3030 3030 3035 5d2c 2022 6c61  0000000005], "la
+00003d30: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00003d40: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00003d50: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00003d60: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+00003d70: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00003d80: 3a20 5b30 2e30 2c20 302e 3235 2c20 302e  : [0.0, 0.25, 0.
+00003d90: 3235 5d2c 2022 7879 7a22 3a20 5b30 2e30  25], "xyz": [0.0
+00003da0: 2c20 312e 3734 3839 3233 2c20 312e 3734  , 1.748923, 1.74
+00003db0: 3839 3233 5d2c 2022 6c61 6265 6c22 3a20  8923], "label": 
+00003dc0: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00003dd0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00003de0: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00003df0: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00003e00: 317d 5d2c 2022 6162 6322 3a20 5b30 2e30  1}], "abc": [0.0
+00003e10: 2c20 302e 3235 2c20 302e 3735 3030 3030  , 0.25, 0.750000
+00003e20: 3030 3030 3030 3030 3031 5d2c 2022 7879  0000000001], "xy
+00003e30: 7a22 3a20 5b30 2e30 2c20 312e 3734 3839  z": [0.0, 1.7489
+00003e40: 3233 2c20 352e 3234 3637 3639 3030 3030  23, 5.2467690000
+00003e50: 3030 3030 3035 5d2c 2022 6c61 6265 6c22  000005], "label"
+00003e60: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00003e70: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00003e80: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00003e90: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00003ea0: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00003eb0: 2e30 2c20 302e 3735 3030 3030 3030 3030  .0, 0.7500000000
+00003ec0: 3030 3030 3031 2c20 302e 3235 5d2c 2022  000001, 0.25], "
+00003ed0: 7879 7a22 3a20 5b30 2e30 2c20 352e 3234  xyz": [0.0, 5.24
+00003ee0: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00003ef0: 312e 3734 3839 3233 5d2c 2022 6c61 6265  1.748923], "labe
+00003f00: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+00003f10: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00003f20: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00003f30: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00003f40: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00003f50: 5b30 2e30 2c20 302e 3735 3030 3030 3030  [0.0, 0.75000000
+00003f60: 3030 3030 3030 3031 2c20 302e 3735 3030  00000001, 0.7500
+00003f70: 3030 3030 3030 3030 3030 3031 5d2c 2022  000000000001], "
+00003f80: 7879 7a22 3a20 5b30 2e30 2c20 352e 3234  xyz": [0.0, 5.24
+00003f90: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00003fa0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00003fb0: 3035 5d2c 2022 6c61 6265 6c22 3a20 224e  05], "label": "N
+00003fc0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00003fd0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+00003fe0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00003ff0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00004000: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
+00004010: 302e 3235 2c20 302e 3235 5d2c 2022 7879  0.25, 0.25], "xy
+00004020: 7a22 3a20 5b33 2e34 3937 3834 362c 2031  z": [3.497846, 1
+00004030: 2e37 3438 3932 332c 2031 2e37 3438 3932  .748923, 1.74892
+00004040: 335d 2c20 226c 6162 656c 223a 2022 4e69  3], "label": "Ni
+00004050: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+00004060: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+00004070: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+00004080: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00004090: 2c20 2261 6263 223a 205b 302e 352c 2030  , "abc": [0.5, 0
+000040a0: 2e32 352c 2030 2e37 3530 3030 3030 3030  .25, 0.750000000
+000040b0: 3030 3030 3030 315d 2c20 2278 797a 223a  0000001], "xyz":
+000040c0: 205b 332e 3439 3738 3436 2c20 312e 3734   [3.497846, 1.74
+000040d0: 3839 3233 2c20 352e 3234 3637 3639 3030  8923, 5.24676900
+000040e0: 3030 3030 3030 3035 5d2c 2022 6c61 6265  00000005], "labe
+000040f0: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+00004100: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00004110: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00004120: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00004130: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00004140: 5b30 2e35 2c20 302e 3735 3030 3030 3030  [0.5, 0.75000000
+00004150: 3030 3030 3030 3031 2c20 302e 3235 5d2c  00000001, 0.25],
+00004160: 2022 7879 7a22 3a20 5b33 2e34 3937 3834   "xyz": [3.49784
+00004170: 362c 2035 2e32 3436 3736 3930 3030 3030  6, 5.24676900000
+00004180: 3030 3030 352c 2031 2e37 3438 3932 335d  00005, 1.748923]
+00004190: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+000041a0: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+000041b0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+000041c0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+000041d0: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+000041e0: 2261 6263 223a 205b 302e 352c 2030 2e37  "abc": [0.5, 0.7
+000041f0: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+00004200: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00004210: 3030 315d 2c20 2278 797a 223a 205b 332e  001], "xyz": [3.
+00004220: 3439 3738 3436 2c20 352e 3234 3637 3639  497846, 5.246769
+00004230: 3030 3030 3030 3030 3035 2c20 352e 3234  0000000005, 5.24
+00004240: 3637 3639 3030 3030 3030 3030 3035 5d2c  67690000000005],
+00004250: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+00004260: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00004270: 7d5d 2c20 2240 7665 7273 696f 6e22 3a20  }], "@version": 
+00004280: 6e75 6c6c 7dfa 1755 6e72 6563 6f67 6e69  null}..Unrecogni
+00004290: 7a65 6420 7465 7374 206e 616d 652e 4e7a  zed test name.Nz
+000042a0: 154b 5332 3032 325f 5465 7374 5265 7375  .KS2022_TestResu
+000042b0: 6c74 2e63 7376 7a02 772b 6301 0000 0000  lt.csvz.w+c.....
+000042c0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+000042d0: 0000 0073 1600 0000 6700 7c00 5d0e 7d01  ...s....g.|.].}.
+000042e0: 7c01 9b00 6400 9d02 9102 7104 5300 2901  |...d.....q.S.).
+000042f0: da01 0a72 2600 0000 2902 7227 0000 00da  ...r&...).r'....
+00004300: 0176 7226 0000 0072 2600 0000 7229 0000  .vr&...r&...r)..
+00004310: 0072 5f00 0000 f800 0000 722b 0000 007a  .r_.......r+...z
+00004320: 1b70 726f 6669 6c65 2e3c 6c6f 6361 6c73  .profile.<locals
+00004330: 3e2e 3c6c 6973 7463 6f6d 703e fa05 446f  >.<listcomp>..Do
+00004340: 6e65 2129 09da 0570 7269 6e74 7202 0000  ne!)...printr...
+00004350: 00da 0966 726f 6d5f 6469 6374 da04 6a73  ...from_dict..js
+00004360: 6f6e da05 6c6f 6164 7372 0600 0000 72b2  on..loadsr....r.
+00004370: 0000 00da 046f 7065 6eda 0a77 7269 7465  .....open..write
+00004380: 6c69 6e65 7329 07da 0474 6573 74da 056e  lines)...test..n
+00004390: 5275 6e73 da06 6d61 7453 7472 da0a 7374  Runs..matStr..st
+000043a0: 7275 6374 4c69 7374 7293 0000 0072 9400  ructListr....r..
+000043b0: 0000 7295 0000 0072 2600 0000 7226 0000  ..r....r&...r&..
+000043c0: 0072 2900 0000 da07 7072 6f66 696c 65e9  .r).....profile.
+000043d0: 0000 0073 1c00 0000 0002 0801 1001 0601  ...s............
+000043e0: 0801 1001 0602 0801 0401 1601 0c01 0a01  ................
+000043f0: 0c01 3201 72d6 0000 00e9 e803 0000 6302  ..2.r.........c.
+00004400: 0000 0000 0000 0000 0000 0007 0000 0005  ................
+00004410: 0000 0043 0000 0073 8800 0000 6401 6402  ...C...s....d.d.
+00004420: 6c00 6d01 7d02 0100 7c00 6403 6b02 722a  l.m.}...|.d.k.r*
+00004430: 7402 6404 7c01 9b00 6405 9d03 8301 0100  t.d.|...d.......
+00004440: 6406 7d03 6e2a 7c00 6407 6b02 7248 7402  d.}.n*|.d.k.rHt.
+00004450: 6408 7c01 9b00 6405 9d03 8301 0100 6409  d.|...d.......d.
+00004460: 7d03 6e0c 7402 640a 8301 0100 640b 5300  }.n.t.d.....d.S.
+00004470: 7403 a004 7405 a006 7c03 a101 a101 7d04  t...t...|.....}.
+00004480: 7c04 6701 7c01 1400 7d05 7c02 7407 7c05  |.g.|...}.|.t.|.
+00004490: 640c 640d 8d03 7d06 7402 640e 8301 0100  d.d...}.t.d.....
+000044a0: 640b 5300 290f 7a45 5072 6f66 696c 6573  d.S.).zEProfiles
+000044b0: 2074 6865 2064 6573 6372 6970 746f 7220   the descriptor 
+000044c0: 696e 2070 6172 616c 6c65 6c20 7573 696e  in parallel usin
+000044d0: 6720 6f6e 6520 6f66 2074 6865 2074 6573  g one of the tes
+000044e0: 7420 7374 7275 6374 7572 6573 2e72 0100  t structures.r..
+000044f0: 0000 2901 da0b 7072 6f63 6573 735f 6d61  ..)...process_ma
+00004500: 7072 c200 0000 72c3 0000 007a 2220 7469  pr....r....z" ti
+00004510: 6d65 7320 696e 2070 6172 616c 6c65 6c20  mes in parallel 
+00004520: 7769 7468 2038 2077 6f72 6b65 7273 2e72  with 8 workers.r
+00004530: c400 0000 72c5 0000 0072 c600 0000 72c7  ....r....r....r.
+00004540: 0000 0072 c800 0000 4e72 8300 0000 2901  ...r....Nr....).
+00004550: da0b 6d61 785f 776f 726b 6572 7372 cb00  ..max_workersr..
+00004560: 0000 2908 da17 7471 646d 2e63 6f6e 7472  ..)...tqdm.contr
+00004570: 6962 2e63 6f6e 6375 7272 656e 7472 d800  ib.concurrentr..
+00004580: 0000 72cc 0000 0072 0200 0000 72cd 0000  ..r....r....r...
+00004590: 0072 ce00 0000 72cf 0000 0072 b200 0000  .r....r....r....
+000045a0: 2907 72d2 0000 0072 d300 0000 72d8 0000  ).r....r....r...
+000045b0: 0072 d400 0000 7293 0000 0072 d500 0000  .r....r....r....
+000045c0: da08 6465 7363 4c69 7374 7226 0000 0072  ..descListr&...r
+000045d0: 2600 0000 7229 0000 00da 0f70 726f 6669  &...r).....profi
+000045e0: 6c65 5061 7261 6c6c 656c fb00 0000 731a  leParallel....s.
+000045f0: 0000 0000 020c 0108 0110 0106 0108 0110  ................
+00004600: 0106 0208 0104 0110 020a 010e 0172 dc00  .............r..
+00004610: 0000 da08 5f5f 6d61 696e 5f5f 2901 72d2  ....__main__).r.
+00004620: 0000 0072 c500 0000 2901 7201 0000 0029  ...r....).r....)
+00004630: 0272 c200 0000 7213 0000 0029 0272 c200  .r....r....).r..
+00004640: 0000 72d7 0000 0029 2872 3700 0000 da04  ..r....)(r7.....
+00004650: 7469 6d65 da05 6e75 6d70 7972 2c00 0000  time..numpyr,...
+00004660: da02 6f73 da0d 7079 6d61 7467 656e 2e63  ..os..pymatgen.c
+00004670: 6f72 6572 0200 0000 7203 0000 00da 1b70  orer....r......p
+00004680: 796d 6174 6765 6e2e 616e 616c 7973 6973  ymatgen.analysis
+00004690: 2e6c 6f63 616c 5f65 6e76 7204 0000 00da  .local_envr.....
+000046a0: 1a70 796d 6174 6765 6e2e 7379 6d6d 6574  .pymatgen.symmet
+000046b0: 7279 2e61 6e61 6c79 7a65 7272 0500 0000  ry.analyzerr....
+000046c0: 72ce 0000 0072 0600 0000 da0b 636f 6c6c  r....r......coll
+000046d0: 6563 7469 6f6e 7372 0700 0000 da06 7479  ectionsr......ty
+000046e0: 7069 6e67 7208 0000 0072 b300 0000 da13  pingr....r......
+000046f0: 7065 7269 6f64 6963 5f74 6162 6c65 5f73  periodic_table_s
+00004700: 697a 65da 076c 6f61 6474 7874 da04 7061  ize..loadtxt..pa
+00004710: 7468 da04 6a6f 696e da07 6469 726e 616d  th..join..dirnam
+00004720: 65da 085f 5f66 696c 655f 5f72 2e00 0000  e..__file__r....
+00004730: da0a 6e61 6e5f 746f 5f6e 756d 724b 0000  ..nan_to_numrK..
+00004740: 0072 4c00 0000 7266 0000 0072 7a00 0000  .rL...rf...rz...
+00004750: 7261 0000 0072 bf00 0000 72b2 0000 00da  ra...r....r.....
+00004760: 0373 7472 72b4 0000 0072 c100 0000 72d6  .strr....r....r.
+00004770: 0000 0072 dc00 0000 725a 0000 0072 2600  ...r....rZ...r&.
+00004780: 0000 7226 0000 0072 2600 0000 7229 0000  ..r&...r&...r)..
+00004790: 00da 083c 6d6f 6475 6c65 3e05 0000 0073  ...<module>....s
+000047a0: 4000 0000 0801 0801 0801 0801 1001 0c01  @...............
+000047b0: 0c01 0801 0c01 0c01 0c02 0605 0401 2001  .............. .
+000047c0: 0a02 0801 06ff 0603 0833 0e0e 0c0f 0a13  .........3......
+000047d0: 0e05 1248 1204 1418 0a12 0a12 0a01 0a01  ...H............
+000047e0: 0a01 0a01                                ....
```

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 27 18:54:19 2023 UTC, .py size: 29490 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 11% similar despite different names*

```diff
@@ -1,1136 +1,1300 @@
-00000000: 610d 0d0a 0000 0000 5bfc fc63 3273 0000  a.......[..c2s..
+00000000: 610d 0d0a 0000 0000 5ef4 2e64 4c81 0000  a.......^..dL...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
+00000020: 0006 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 6400 6401 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
-00000080: 6405 6c0d 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
-00000090: 6d0f 5a0f 0100 6407 5a10 6408 5a11 6503  m.Z...d.Z.d.Z.e.
-000000a0: 6a12 6504 6a13 a014 6504 6a13 a015 6516  j.e.j...e.j...e.
-000000b0: a101 6409 a102 640a 640b 8d02 5a17 6503  ..d...d.d...Z.e.
-000000c0: a018 6517 a101 5a17 6517 6401 6401 8502  ..e...Z.e.d.d...
-000000d0: 6700 640c a201 6602 1900 5a17 640d 640e  g.d...f...Z.d.d.
-000000e0: 8400 5a19 640f 6410 8400 5a1a 6411 6519  ..Z.d.d...Z.d.e.
-000000f0: 6602 6412 6413 8401 5a1b 4700 6414 6415  f.d.d...Z.G.d.d.
-00000100: 8400 6415 8302 5a1c 6425 6416 6417 8401  ..d...Z.d%d.d...
-00000110: 5a1d 6426 6506 6418 9c01 6419 641a 8405  Z.d&e.d...d.d...
-00000120: 5a1e 641b 641c 8400 5a1f 6427 641e 641f  Z.d.d...Z.d'd.d.
-00000130: 8401 5a20 6428 6420 6421 8401 5a21 6522  ..Z d(d d!..Z!e"
-00000140: 6422 6b02 9001 722e 6520 6423 6424 8d01  d"k...r.e d#d$..
-00000150: 0100 6521 6423 6424 8d01 0100 6401 5300  ..e!d#d$....d.S.
-00000160: 2929 e900 0000 004e 2902 da09 5374 7275  )).....N)...Stru
-00000170: 6374 7572 65da 0745 6c65 6d65 6e74 2901  cture..Element).
-00000180: da09 566f 726f 6e6f 694e 4e29 01da 1253  ..VoronoiNN)...S
-00000190: 7061 6365 6772 6f75 7041 6e61 6c79 7a65  pacegroupAnalyze
-000001a0: 7229 01da 0474 7164 6d29 01da 0743 6f75  r)...tqdm)...Cou
-000001b0: 6e74 6572 75f9 0000 004c 2e20 5761 7264  nteru....L. Ward
-000001c0: 2c20 522e 204c 6975 2c20 412e 204b 7269  , R. Liu, A. Kri
-000001d0: 7368 6e61 2c20 562e 2049 2e20 4865 6764  shna, V. I. Hegd
-000001e0: 652c 2041 2e20 4167 7261 7761 6c2c 2041  e, A. Agrawal, A
-000001f0: 2e20 4368 6f75 6468 6172 792c 2061 6e64  . Choudhary, and
-00000200: 2043 2e20 576f 6c76 6572 746f 6e2c 20e2   C. Wolverton, .
-00000210: 809c 496e 636c 7564 696e 6720 6372 7973  ..Including crys
-00000220: 7461 6c20 7374 7275 6374 7572 6520 6174  tal structure at
-00000230: 7472 6962 7574 6573 2069 6e20 6d61 6368  tributes in mach
-00000240: 696e 6520 6c65 6172 6e69 6e67 206d 6f64  ine learning mod
-00000250: 656c 7320 6f66 2066 6f72 6d61 7469 6f6e  els of formation
-00000260: 2065 6e65 7267 6965 7320 7669 6120 566f   energies via Vo
-00000270: 726f 6e6f 6920 7465 7373 656c 6c61 7469  ronoi tessellati
-00000280: 6f6e 732c e280 9d20 5068 7973 6963 616c  ons,... Physical
-00000290: 2052 6576 6965 7720 422c 2076 6f6c 2e20   Review B, vol. 
-000002a0: 3936 2c20 6e6f 2e20 322c 2037 2032 3031  96, no. 2, 7 201
-000002b0: 372e e970 0000 007a 1d4d 6167 7069 655f  7..p...z.Magpie_
-000002c0: 656c 656d 656e 745f 7072 6f70 6572 7469  element_properti
-000002d0: 6573 2e63 7376 fa01 2c29 01da 0964 656c  es.csv..,)...del
-000002e0: 696d 6974 6572 2915 e92d 0000 00e9 2100  imiter)..-....!.
-000002f0: 0000 e902 0000 00e9 2000 0000 e905 0000  ........ .......
-00000300: 00e9 3000 0000 e906 0000 00e9 0a00 0000  ..0.............
-00000310: e92c 0000 00e9 2a00 0000 e926 0000 00e9  .,....*....&....
-00000320: 2800 0000 e924 0000 00e9 2b00 0000 e929  (....$....+....)
-00000330: 0000 00e9 2500 0000 e927 0000 00e9 2300  ....%....'....#.
-00000340: 0000 e912 0000 00e9 0d00 0000 e911 0000  ................
-00000350: 0063 0300 0000 0000 0000 0000 0000 1400  .c..............
-00000360: 0000 0800 0000 4300 0000 7308 0200 0074  ......C...s....t
-00000370: 00a0 0174 026a 0364 0119 00a1 017d 037c  ...t.j.d.....}.|
-00000380: 016a 04a0 05a1 00a0 06a1 0044 005d 2a5c  .j.........D.]*\
-00000390: 027d 047d 057c 037c 0574 0274 077c 0483  .}.}.|.|.t.t.|..
-000003a0: 016a 0864 0118 0064 0064 0085 0266 0219  .j.d...d.d...f..
-000003b0: 0014 0037 007d 0371 1e74 00a0 0174 026a  ...7.}.q.t...t.j
-000003c0: 0364 0119 00a1 017d 0664 027d 0764 027d  .d.....}.d.}.d.}
-000003d0: 087c 00a0 06a1 0044 005d 885c 027d 097d  .|.....D.].\.}.}
-000003e0: 0a74 00a0 0174 026a 0364 0119 00a1 017d  .t...t.j.d.....}
-000003f0: 0b7c 0a64 0319 006a 04a0 05a1 00a0 06a1  .|.d...j........
-00000400: 0044 005d 2a5c 027d 047d 057c 0b7c 0574  .D.]*\.}.}.|.|.t
-00000410: 0274 077c 0483 016a 0864 0118 0064 0064  .t.|...j.d...d.d
-00000420: 0085 0266 0219 0014 0037 007d 0b71 947c  ...f.....7.}.q.|
-00000430: 0674 00a0 097c 037c 0b18 00a1 017c 0a64  .t...|.|.....|.d
-00000440: 0419 0014 0037 007d 067c 077c 0a64 0419  .....7.}.|.|.d..
-00000450: 0037 007d 077c 087c 0a64 0519 0037 007d  .7.}.|.|.d...7.}
-00000460: 0871 6a7c 067c 071b 007c 0367 027d 0c64  .qj|.|...|.g.}.d
-00000470: 027d 0d64 027d 0e7c 00a0 0aa1 0044 005d  .}.d.}.|.....D.]
-00000480: 267d 0a7c 0d7c 0a64 0419 0037 007d 0d7c  &}.|.|.d...7.}.|
-00000490: 0e7c 0a64 0419 007c 0a64 0419 0014 0037  .|.d...|.d.....7
-000004a0: 007d 0e90 0171 107c 0d7c 0d14 007c 0e1b  .}...q.|.|...|..
-000004b0: 007d 0f64 027d 107c 00a0 0aa1 0044 005d  .}.d.}.|.....D.]
-000004c0: 1e7d 0a7c 107c 0a64 0419 0064 0614 007c  .}.|.|.d...d...|
-000004d0: 0a64 0719 0014 0037 007d 1090 0171 507c  .d.....7.}...qP|
-000004e0: 107c 071d 007d 1064 027d 117c 00a0 0aa1  .|...}.d.}.|....
-000004f0: 0044 005d 267d 0a7c 117c 0a64 0419 0074  .D.]&}.|.|.d...t
-00000500: 0964 067c 0a64 0719 0014 007c 1018 0083  .d.|.d.....|....
-00000510: 0114 0037 007d 1190 0171 847c 117c 077c  ...7.}...q.|.|.|
-00000520: 1014 001d 007d 1174 0b64 0864 0984 007c  .....}.t.d.d...|
-00000530: 00a0 0aa1 0044 0083 0183 017d 1264 0a74  .....D.....}.d.t
-00000540: 0c6a 0d14 0074 0ca0 0e7c 1264 0ba1 0214  .j...t...|.d....
-00000550: 007d 1374 00a0 0f7c 0f7c 107c 117c 087c  .}.t...|.|.|.|.|
-00000560: 1367 057c 0c64 0219 0066 02a1 017c 0c64  .g.|.d...f...|.d
-00000570: 0119 0067 0253 0029 0c4e e901 0000 0072  ...g.S.).N.....r
-00000580: 0100 0000 da04 7369 7465 da04 6172 6561  ......site..area
-00000590: da06 766f 6c75 6d65 720d 0000 00da 0966  ..volumer......f
-000005a0: 6163 655f 6469 7374 6301 0000 0000 0000  ace_distc.......
-000005b0: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
-000005c0: 0073 1600 0000 7c00 5d0e 7d01 7c01 6400  .s....|.].}.|.d.
-000005d0: 1900 5600 0100 7102 6401 5300 2902 7224  ..V...q.d.S.).r$
-000005e0: 0000 004e a900 2902 da02 2e30 da0d 6e65  ...N..)....0..ne
-000005f0: 6967 6862 6f72 5f73 6974 6572 2500 0000  ighbor_siter%...
-00000600: 7225 0000 00fa 562f 5573 6572 732f 6164  r%....V/Users/ad
-00000610: 616d 2f50 7963 6861 726d 5072 6f6a 6563  am/PycharmProjec
-00000620: 7473 2f70 7953 4950 4645 4e4e 2f70 7973  ts/pySIPFENN/pys
-00000630: 6970 6665 6e6e 2f64 6573 6372 6970 746f  ipfenn/descripto
-00000640: 7244 6566 696e 6974 696f 6e73 2f4b 5332  rDefinitions/KS2
-00000650: 3032 325f 6469 6c75 7465 2e70 79da 093c  022_dilute.py..<
-00000660: 6765 6e65 7870 723e 4200 0000 f300 0000  genexpr>B.......
-00000670: 007a 256c 6f63 616c 5f65 6e76 5f66 756e  .z%local_env_fun
-00000680: 6374 696f 6e2e 3c6c 6f63 616c 733e 2e3c  ction.<locals>.<
-00000690: 6765 6e65 7870 723e 6755 5555 5555 55f5  genexpr>gUUUUUU.
-000006a0: 3f67 0000 0000 0000 0840 2910 da02 6e70  ?g.......@)...np
-000006b0: da05 7a65 726f 73da 1061 7474 7269 6275  ..zeros..attribu
-000006c0: 7465 5f6d 6174 7269 78da 0573 6861 7065  te_matrix..shape
-000006d0: da07 7370 6563 6965 73da 0f67 6574 5f65  ..species..get_e
-000006e0: 6c5f 616d 745f 6469 6374 da05 6974 656d  l_amt_dict..item
-000006f0: 7372 0300 0000 da01 5ada 0361 6273 da06  sr......Z..abs..
-00000700: 7661 6c75 6573 da03 6d69 6eda 046d 6174  values..min..mat
-00000710: 68da 0270 69da 0370 6f77 da0b 636f 6e63  h..pi..pow..conc
-00000720: 6174 656e 6174 6529 14da 096c 6f63 616c  atenate)...local
-00000730: 5f65 6e76 7221 0000 00da 0673 7472 7563  _envr!.....struc
-00000740: 74da 106c 6f63 616c 5f61 7474 7269 6275  t..local_attribu
-00000750: 7465 73da 036b 6579 da05 7661 6c75 65da  tes..key..value.
-00000760: 0f64 6966 665f 6174 7472 6962 7574 6573  .diff_attributes
-00000770: da0c 746f 7461 6c5f 7765 6967 6874 7223  ..total_weightr#
-00000780: 0000 00da 0369 6e64 7227 0000 00da 136e  .....indr'.....n
-00000790: 6569 6768 626f 725f 6174 7472 6962 7574  eighbor_attribut
-000007a0: 6573 da1f 656c 656d 656e 7461 6c5f 7072  es..elemental_pr
-000007b0: 6f70 6572 7469 6573 5f61 7474 7269 6275  operties_attribu
-000007c0: 7465 73da 0761 7665 7261 6765 da08 7661  tes..average..va
-000007d0: 7269 616e 6365 da0d 6566 665f 636f 6f72  riance..eff_coor
-000007e0: 645f 6e75 6dda 0c62 6c65 6e5f 6176 6572  d_num..blen_aver
-000007f0: 6167 65da 0862 6c65 6e5f 7661 72da 0a73  age..blen_var..s
-00000800: 7068 6572 655f 7261 64da 0d73 7068 6572  phere_rad..spher
-00000810: 655f 766f 6c75 6d65 7225 0000 0072 2500  e_volumer%...r%.
-00000820: 0000 7228 0000 00da 126c 6f63 616c 5f65  ..r(.....local_e
-00000830: 6e76 5f66 756e 6374 696f 6e20 0000 0073  nv_function ...s
-00000840: 4600 0000 0001 1001 1601 2401 1001 0401  F.........$.....
-00000850: 0401 1001 1001 1a01 2401 1a01 0c01 0e01  ........$.......
-00000860: 0c02 0401 0401 0c01 0c01 1801 0c03 0401  ................
-00000870: 0c01 1c01 0802 0401 0c01 2401 0c02 1601  ..........$.....
-00000880: 1601 0401 14ff 0202 06fe 724b 0000 0063  ..........rK...c
-00000890: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000008a0: 0300 0000 0300 0000 7352 0000 007c 006a  ........sR...|.j
-000008b0: 0089 0174 0174 0288 0183 0183 0189 0087  ...t.t..........
-000008c0: 0087 0166 0264 0164 0284 0888 0044 0083  ...f.d.d.....D..
-000008d0: 017d 0174 0388 0083 0174 037c 0183 0118  .}.t.....t.|....
-000008e0: 0064 036b 0272 427c 0164 0419 0053 0074  .d.k.rB|.d...S.t
-000008f0: 0464 0583 0101 0074 0582 0164 0053 0029  .d.....t...d.S.)
-00000900: 064e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
-00000910: 0000 0005 0000 0013 0000 0073 2200 0000  ...........s"...
-00000920: 6700 7c00 5d1a 7d01 8800 7c01 1900 6400  g.|.].}...|...d.
-00000930: 6b02 7204 8801 a000 7c01 a101 9102 7104  k.r.....|.....q.
-00000940: 5300 a901 7220 0000 0029 01da 0569 6e64  S...r ...)...ind
-00000950: 6578 2902 7226 0000 00da 0273 70a9 025a  ex).r&.....sp..Z
-00000960: 0773 7043 6f75 6e74 5a07 7370 6f4c 6973  .spCountZ.spoLis
-00000970: 7472 2500 0000 7228 0000 00da 0a3c 6c69  tr%...r(.....<li
-00000980: 7374 636f 6d70 3e4b 0000 0072 2a00 0000  stcomp>K...r*...
-00000990: 7a1e 6669 6e64 4469 6c75 7465 2e3c 6c6f  z.findDilute.<lo
-000009a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000009b0: 7220 0000 0072 0100 0000 7a6c 4375 7374  r ...r....zlCust
-000009c0: 6f6d 2064 696c 7574 6520 7374 7275 6374  om dilute struct
-000009d0: 7572 6520 6465 7363 7269 7074 6f72 2063  ure descriptor c
-000009e0: 616c 6375 6c61 7469 6f6e 2069 7320 6465  alculation is de
-000009f0: 6669 6e65 6420 6f6e 6c79 206f 6e65 2064  fined only one d
-00000a00: 696c 7574 6520 7370 6563 6965 7320 696e  ilute species in
-00000a10: 2061 2073 696e 676c 6520 656c 656d 656e   a single elemen
-00000a20: 7420 6d61 7472 6978 2906 da10 7370 6563  t matrix)...spec
-00000a30: 6965 735f 616e 645f 6f63 6375 da04 6469  ies_and_occu..di
-00000a40: 6374 7207 0000 00da 036c 656e da05 7072  ctr......len..pr
-00000a50: 696e 74da 0c52 756e 7469 6d65 4572 726f  int..RuntimeErro
-00000a60: 7229 0272 3b00 0000 5a08 7370 4469 6c75  r).r;...Z.spDilu
-00000a70: 7465 7225 0000 0072 4f00 0000 7228 0000  ter%...rO...r(..
-00000a80: 00da 0a66 696e 6444 696c 7574 6548 0000  ...findDiluteH..
-00000a90: 0073 0e00 0000 0001 0601 0c01 1401 1401  .s..............
-00000aa0: 0802 0801 7256 0000 00da 0470 7572 6563  ....rV.....purec
-00000ab0: 0300 0000 0000 0000 0000 0000 1300 0000  ................
-00000ac0: 0600 0000 4300 0000 73fe 0100 0074 007c  ....C...s....t.|
-00000ad0: 007c 0283 027d 0374 017c 0174 0283 0272  .|...}.t.|.t...r
-00000ae0: 7067 007d 0474 0374 047c 016a 057c 006a  pg.}.t.t.|.j.|.j
-00000af0: 0583 0283 0144 005d 205c 027d 055c 027d  .....D.] \.}.\.}
-00000b00: 067d 077c 067c 076b 0372 2a7c 04a0 067c  .}.|.|.k.r*|...|
-00000b10: 05a1 0101 0071 2a71 2a74 077c 0483 0164  .....q*q*t.|...d
-00000b20: 016b 0272 627c 0464 0219 007d 0471 ac74  .k.rb|.d...}.q.t
-00000b30: 0864 0383 0101 0074 0982 016e 3c7c 0164  .d.....t...n<|.d
-00000b40: 046b 0272 a87c 00a0 0aa1 007d 0174 0b7c  .k.r.|.....}.t.|
-00000b50: 016a 0c83 0144 005d 127d 087c 01a0 0d7c  .j...D.].}.|...|
-00000b60: 0864 0569 01a1 0101 0071 8a74 0e7c 0083  .d.i.....q.t.|..
-00000b70: 017d 046e 0474 0982 0174 0f7c 0164 0664  .}.n.t...t.|.d.d
-00000b80: 0764 088d 037d 0974 107c 09a0 11a1 0064  .d...}.t.|.....d
-00000b90: 0919 0083 017d 0a74 1083 007d 0b7c 0ba0  .....}.t...}.|..
-00000ba0: 067c 03a0 127c 04a1 01a1 0101 007c 0b64  .|...|.......|.d
-00000bb0: 0219 0064 0a19 007d 0c74 1374 0474 1474  ...d...}.t.t.t.t
-00000bc0: 077c 0a83 0183 0164 0b64 0c84 007c 0a44  .|.....d.d...|.D
-00000bd0: 0083 0183 0283 017d 0d64 0d7c 0d7c 043c  .......}.d.|.|.<
-00000be0: 007c 0c44 005d 187d 0e7c 0d7c 0e19 00a0  .|.D.].}.|.|....
-00000bf0: 067c 0c7c 0e19 00a1 0101 0090 0171 1869  .|.|.........q.i
-00000c00: 007d 0f7c 0d44 005d 427d 0e64 0ea0 1574  .}.|.D.]B}.d...t
-00000c10: 167c 0d7c 0e19 0083 01a1 017d 107c 107c  .|.|.......}.|.|
-00000c20: 0f76 0090 0172 6a7c 0f7c 1019 00a0 067c  .v...rj|.|.....|
-00000c30: 0ea1 0101 006e 107c 0fa0 177c 107c 0e67  .....n.|...|.|.g
-00000c40: 0169 01a1 0101 0090 0171 3a7c 0f64 0d3d  .i.......q:|.d.=
-00000c50: 0074 1374 0464 0f64 0c84 007c 0fa0 18a1  .t.t.d.d...|....
-00000c60: 0044 0083 0164 1064 0c84 007c 0fa0 18a1  .D...d.d...|....
-00000c70: 0044 0083 0183 0283 017d 117c 1144 005d  .D.......}.|.D.]
-00000c80: 227d 0e7c 03a0 197c 0ea1 0167 017d 127c  "}.|...|...g.}.|
-00000c90: 0b7c 127c 117c 0e19 0014 0037 007d 0b90  .|.|.|.....7.}..
-00000ca0: 0171 b274 1aa0 1b64 1164 0c84 007c 0b44  .q.t...d.d...|.D
-00000cb0: 0083 01a1 0174 1aa0 1b64 1264 0c84 007c  .....t...d.d...|
-00000cc0: 0b44 0083 01a1 0166 0253 0029 134e 7220  .D.....f.S.).Nr 
-00000cd0: 0000 0072 0100 0000 7a49 5369 7465 7320  ...r....zISites 
-00000ce0: 696e 2074 6865 2070 726f 7669 6465 6420  in the provided 
-00000cf0: 6261 7365 2073 7472 7563 7475 7265 206d  base structure m
-00000d00: 6174 6368 6564 2074 6865 2069 6e76 6573  atched the inves
-00000d10: 7469 6761 7465 6420 6f6e 6520 6578 6163  tigated one exac
-00000d20: 746c 7972 5700 0000 da01 4167 fca9 f1d2  tlyrW.....Ag....
-00000d30: 4d62 503f 679a 9999 9999 99b9 3f29 02da  MbP?g.......?)..
-00000d40: 0773 796d 7072 6563 da0f 616e 676c 655f  .symprec..angle_
-00000d50: 746f 6c65 7261 6e63 65da 1065 7175 6976  tolerance..equiv
-00000d60: 616c 656e 745f 6174 6f6d 7372 0d00 0000  alent_atomsr....
-00000d70: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000d80: 0003 0000 0053 0000 0073 1200 0000 6700  .....S...s....g.
-00000d90: 7c00 5d0a 7d01 7c01 6701 9102 7104 5300  |.].}.|.g...q.S.
-00000da0: 7225 0000 0072 2500 0000 2902 7226 0000  r%...r%...).r&..
-00000db0: 00da 0165 7225 0000 0072 2500 0000 7228  ...er%...r%...r(
-00000dc0: 0000 0072 5000 0000 7600 0000 722a 0000  ...rP...v...r*..
-00000dd0: 007a 2f67 656e 6572 6174 655f 766f 726f  .z/generate_voro
-00000de0: 6e6f 695f 6174 7472 6962 7574 6573 2e3c  noi_attributes.<
-00000df0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000e00: 703e 5a06 6469 6c75 7465 da00 6301 0000  p>Z.dilute..c...
-00000e10: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000e20: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
-00000e30: 7d01 7c01 6400 1900 9102 7104 5300 a901  }.|.d.....q.S...
-00000e40: 7201 0000 0072 2500 0000 a902 7226 0000  r....r%.....r&..
-00000e50: 00da 0167 7225 0000 0072 2500 0000 7228  ...gr%...r%...r(
-00000e60: 0000 0072 5000 0000 8600 0000 722a 0000  ...rP.......r*..
-00000e70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000e80: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00000e90: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
-00000ea0: 0453 0072 2500 0000 2901 7253 0000 0072  .S.r%...).rS...r
-00000eb0: 5f00 0000 7225 0000 0072 2500 0000 7228  _...r%...r%...r(
-00000ec0: 0000 0072 5000 0000 8700 0000 722a 0000  ...rP.......r*..
-00000ed0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00000ee0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
-00000ef0: 007c 005d 0c7d 017c 0164 0019 0091 0271  .|.].}.|.d.....q
-00000f00: 0453 0072 5e00 0000 7225 0000 00a9 0272  .S.r^...r%.....r
-00000f10: 2600 0000 723e 0000 0072 2500 0000 7225  &...r>...r%...r%
-00000f20: 0000 0072 2800 0000 7250 0000 008d 0000  ...r(...rP......
-00000f30: 0072 2a00 0000 6301 0000 0000 0000 0000  .r*...c.........
-00000f40: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
-00000f50: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
-00000f60: 1900 9102 7104 5300 724c 0000 0072 2500  ....q.S.rL...r%.
-00000f70: 0000 7261 0000 0072 2500 0000 7225 0000  ..ra...r%...r%..
-00000f80: 0072 2800 0000 7250 0000 008d 0000 0072  .r(...rP.......r
-00000f90: 2a00 0000 291c da17 4c6f 6361 6c41 7474  *...)...LocalAtt
-00000fa0: 7269 6275 7465 4765 6e65 7261 746f 72da  ributeGenerator.
-00000fb0: 0a69 7369 6e73 7461 6e63 6572 0200 0000  .isinstancer....
-00000fc0: da09 656e 756d 6572 6174 65da 037a 6970  ..enumerate..zip
-00000fd0: da05 7369 7465 73da 0661 7070 656e 6472  ..sites..appendr
-00000fe0: 5300 0000 7254 0000 00da 0954 7970 6545  S...rT.....TypeE
-00000ff0: 7272 6f72 da04 636f 7079 da03 7365 7472  rror..copy..setr
-00001000: 2f00 0000 da0f 7265 706c 6163 655f 7370  /.....replace_sp
-00001010: 6563 6965 7372 5600 0000 7205 0000 00da  eciesrV...r.....
-00001020: 046c 6973 74da 1467 6574 5f73 796d 6d65  .list..get_symme
-00001030: 7472 795f 6461 7461 7365 74da 2467 656e  try_dataset.$gen
-00001040: 6572 6174 655f 6c6f 6361 6c5f 6174 7472  erate_local_attr
-00001050: 6962 7574 6573 5f64 696c 7574 6553 6974  ibutes_diluteSit
-00001060: 6572 5200 0000 da05 7261 6e67 65da 046a  erR.....range..j
-00001070: 6f69 6eda 0373 7472 da06 7570 6461 7465  oin..str..update
-00001080: 7234 0000 00da 1967 656e 6572 6174 655f  r4.....generate_
-00001090: 6c6f 6361 6c5f 6174 7472 6962 7574 6573  local_attributes
-000010a0: 722b 0000 00da 0561 7272 6179 2913 723b  r+.....array).r;
-000010b0: 0000 00da 0a62 6173 6553 7472 7563 74da  .....baseStruct.
-000010c0: 0b6c 6f63 616c 5f66 756e 6374 da0f 6c6f  .local_funct..lo
-000010d0: 6361 6c5f 6765 6e65 7261 746f 725a 0a64  cal_generatorZ.d
-000010e0: 696c 7574 6553 6974 65da 0169 5a03 7331  iluteSite..iZ.s1
-000010f0: 735a 0373 3273 724e 0000 005a 0873 7067  sZ.s2srN...Z.spg
-00001100: 4162 6173 655a 136f 7269 6769 6e61 6c45  AbaseZ.originalE
-00001110: 7175 6976 616c 656e 7473 da0e 6174 7472  quivalents..attr
-00001120: 6962 7574 655f 6c69 7374 5a12 6e65 6967  ibute_listZ.neig
-00001130: 6862 6f72 7346 6163 6573 4469 6374 5a0d  hborsFacesDictZ.
-00001140: 7369 7465 4c43 4570 6172 616d 73da 0573  siteLCEparams..s
-00001150: 6974 654e 5a10 6571 7569 7661 6c65 6e74  iteNZ.equivalent
-00001160: 4772 6f75 7073 da06 7061 7261 6d73 da1d  Groups..params..
-00001170: 6571 7569 7661 6c65 6e74 5369 7465 734d  equivalentSitesM
-00001180: 756c 7469 706c 6963 6974 6965 73da 0f6c  ultiplicities..l
-00001190: 6f63 616c 4174 7472 6962 7574 6573 7225  ocalAttributesr%
-000011a0: 0000 0072 2500 0000 7228 0000 00da 1b67  ...r%...r(.....g
-000011b0: 656e 6572 6174 655f 766f 726f 6e6f 695f  enerate_voronoi_
-000011c0: 6174 7472 6962 7574 6573 5200 0000 7354  attributesR...sT
-000011d0: 0000 0000 010a 030a 0104 011e 0108 010a  ................
-000011e0: 0104 010c 010a 0208 0106 0108 0108 010e  ................
-000011f0: 0110 020a 0204 030e 0110 0306 0110 030c  ................
-00001200: 0320 0108 0108 0116 0304 0108 0112 010a  . ..............
-00001210: 0110 0214 0106 0202 0112 0110 ff02 ff04  ................
-00001220: 0408 010c 0114 0272 7e00 0000 6300 0000  .......r~...c...
-00001230: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00001240: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
-00001250: 5a02 6503 6401 6401 6402 8d02 6601 6403  Z.e.d.d.d...f.d.
-00001260: 6404 8401 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-00001270: 6408 8400 5a06 6409 5300 290a 7262 0000  d...Z.d.S.).rb..
-00001280: 0046 2902 da15 636f 6d70 7574 655f 6164  .F)...compute_ad
-00001290: 6a5f 6e65 6967 6862 6f72 73da 0d65 7874  j_neighbors..ext
-000012a0: 7261 5f6e 6e5f 696e 666f 6304 0000 0000  ra_nn_infoc.....
-000012b0: 0000 0000 0000 0004 0000 0002 0000 0043  ...............C
-000012c0: 0000 0073 1600 0000 7c03 7c00 5f00 7c01  ...s....|.|._.|.
-000012d0: 7c00 5f01 7c02 7c00 5f02 6400 5300 a901  |._.|.|._.d.S...
-000012e0: 4e29 03da 0967 656e 6572 6174 6f72 723b  N)...generatorr;
-000012f0: 0000 00da 0866 756e 6374 696f 6e29 04da  .....function)..
-00001300: 0473 656c 6672 3b00 0000 da0e 6c6f 6361  .selfr;.....loca
-00001310: 6c5f 656e 765f 6675 6e63 da0c 6e6e 5f67  l_env_func..nn_g
-00001320: 656e 6572 6174 6f72 7225 0000 0072 2500  eneratorr%...r%.
-00001330: 0000 7228 0000 00da 085f 5f69 6e69 745f  ..r(.....__init_
-00001340: 5f92 0000 0073 0600 0000 0001 0601 0601  _....s..........
-00001350: 7a20 4c6f 6361 6c41 7474 7269 6275 7465  z LocalAttribute
-00001360: 4765 6e65 7261 746f 722e 5f5f 696e 6974  Generator.__init
-00001370: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
-00001380: 0000 0005 0000 0043 0000 0073 2600 0000  .......C...s&...
-00001390: 7c00 6a00 a001 7c00 6a02 7c01 a102 7d02  |.j...|.j.|...}.
-000013a0: 7c00 a003 7c02 7c00 6a02 7c01 1900 7c00  |...|.|.j.|...|.
-000013b0: 6a02 a103 5300 7281 0000 0029 0472 8200  j...S.r....).r..
-000013c0: 0000 da15 6765 745f 766f 726f 6e6f 695f  ....get_voronoi_
-000013d0: 706f 6c79 6865 6472 6172 3b00 0000 7283  polyhedrar;...r.
-000013e0: 0000 0029 0372 8400 0000 da01 6e72 3a00  ...).r......nr:.
-000013f0: 0000 7225 0000 0072 2500 0000 7228 0000  ..r%...r%...r(..
-00001400: 0072 7300 0000 9700 0000 7304 0000 0000  .rs.......s.....
-00001410: 0110 017a 314c 6f63 616c 4174 7472 6962  ...z1LocalAttrib
-00001420: 7574 6547 656e 6572 6174 6f72 2e67 656e  uteGenerator.gen
-00001430: 6572 6174 655f 6c6f 6361 6c5f 6174 7472  erate_local_attr
-00001440: 6962 7574 6573 6302 0000 0000 0000 0000  ibutesc.........
-00001450: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
-00001460: 4600 0000 7c00 6a00 a001 7c00 6a02 7c01  F...|.j...|.j.|.
-00001470: a102 7d02 7c00 a003 7c02 7c00 6a02 7c01  ..}.|...|.|.j.|.
-00001480: 1900 7c00 6a02 a103 7d03 6401 6402 8400  ..|.j...}.d.d...
-00001490: 7c02 a004 a100 4400 8301 7d04 7c03 a005  |.....D...}.|...
-000014a0: 7c04 a101 0100 7c03 5300 2903 4e63 0100  |.....|.S.).Nc..
-000014b0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-000014c0: 0000 5300 0000 7342 0000 0069 007c 005d  ..S...sB...i.|.]
-000014d0: 3a7d 017c 0164 0019 006a 0074 017c 0164  :}.|.d...j.t.|.d
-000014e0: 0019 006a 0283 0174 037c 0164 0119 0064  ...j...t.|.d...d
-000014f0: 0283 0274 037c 0164 0319 0064 0283 027c  ...t.|.d...d...|
-00001500: 0164 0419 0067 0493 0271 0453 0029 0572  .d...g...q.S.).r
-00001510: 2100 0000 7224 0000 0072 0d00 0000 7222  !...r$...r....r"
-00001520: 0000 00da 076e 5f76 6572 7473 2904 724d  .....n_verts).rM
-00001530: 0000 0072 7100 0000 722f 0000 00da 0572  ...rq...r/.....r
-00001540: 6f75 6e64 7261 0000 0072 2500 0000 7225  oundra...r%...r%
-00001550: 0000 0072 2800 0000 da0a 3c64 6963 7463  ...r(.....<dictc
-00001560: 6f6d 703e 9f00 0000 730e 0000 0006 0502  omp>....s.......
-00001570: fb08 010c 010c 010c 0106 fd7a 504c 6f63  ...........zPLoc
-00001580: 616c 4174 7472 6962 7574 6547 656e 6572  alAttributeGener
-00001590: 6174 6f72 2e67 656e 6572 6174 655f 6c6f  ator.generate_lo
-000015a0: 6361 6c5f 6174 7472 6962 7574 6573 5f64  cal_attributes_d
-000015b0: 696c 7574 6553 6974 652e 3c6c 6f63 616c  iluteSite.<local
-000015c0: 733e 2e3c 6469 6374 636f 6d70 3e29 0672  s>.<dictcomp>).r
-000015d0: 8200 0000 7288 0000 0072 3b00 0000 7283  ....r....r;...r.
-000015e0: 0000 0072 3400 0000 7267 0000 0029 0572  ...r4...rg...).r
-000015f0: 8400 0000 7289 0000 0072 3a00 0000 5a10  ....r....r:...Z.
-00001600: 6c6f 6361 6c5f 656e 765f 7265 7375 6c74  local_env_result
-00001610: da0d 6e65 6967 6862 6f72 5f64 6963 7472  ..neighbor_dictr
-00001620: 2500 0000 7225 0000 0072 2800 0000 726e  %...r%...r(...rn
-00001630: 0000 009b 0000 0073 0e00 0000 0001 1001  .......s........
-00001640: 1602 0605 06fb 0607 0a02 7a3c 4c6f 6361  ..........z<Loca
-00001650: 6c41 7474 7269 6275 7465 4765 6e65 7261  lAttributeGenera
-00001660: 746f 722e 6765 6e65 7261 7465 5f6c 6f63  tor.generate_loc
-00001670: 616c 5f61 7474 7269 6275 7465 735f 6469  al_attributes_di
-00001680: 6c75 7465 5369 7465 4e29 07da 085f 5f6e  luteSiteN)...__n
-00001690: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-000016a0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-000016b0: 0400 0000 7287 0000 0072 7300 0000 726e  ....r....rs...rn
-000016c0: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
-000016d0: 0000 7228 0000 0072 6200 0000 9100 0000  ..r(...rb.......
-000016e0: 7306 0000 0008 0114 0508 0472 6200 0000  s..........rb...
-000016f0: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
-00001700: 0007 0000 0043 0000 0073 d400 0000 7400  .....C...s....t.
-00001710: a001 7400 a002 7c00 6400 6400 8502 6401  ..t...|.d.d...d.
-00001720: 6602 1900 a101 a101 7d02 6401 7d03 6700  f.......}.d.}.g.
-00001730: 7d04 7c02 4400 5d62 7d05 7c00 6400 6400  }.|.D.]b}.|.d.d.
-00001740: 8502 6401 6602 1900 7c05 6b02 7d06 7400  ..d.f...|.k.}.t.
-00001750: a003 7400 a004 7c06 7c01 a102 7c01 a102  ..t...|.|...|...
-00001760: 6401 1900 7d07 7c07 7c03 6b04 7278 7c04  d...}.|.|.k.rx|.
-00001770: a005 a100 0100 7c04 a006 7c05 a101 0100  ......|...|.....
-00001780: 7c07 7d03 7128 7c07 7c03 6b02 7228 7c04  |.}.q(|.|.k.r(|.
-00001790: a006 7c05 a101 0100 7128 7400 a007 7c00  ..|.....q(t...|.
-000017a0: 6401 6400 6400 8502 6602 1900 a101 7d08  d.d.d...f.....}.
-000017b0: 7c04 4400 5d20 7d09 7c08 7408 7409 7c09  |.D.] }.|.t.t.|.
-000017c0: 8301 6402 1800 6400 6400 8502 6602 1900  ..d...d.d...f...
-000017d0: 3700 7d08 71a6 7c08 740a 7c04 8301 1b00  7.}.q.|.t.|.....
-000017e0: 5300 2903 4e72 0100 0000 7220 0000 0029  S.).Nr....r ...)
-000017f0: 0b72 2b00 0000 da06 756e 6971 7565 da05  .r+.....unique..
-00001800: 7261 7665 6cda 0b65 7870 616e 645f 6469  ravel..expand_di
-00001810: 6d73 da03 7375 6dda 0563 6c65 6172 7267  ms..sum..clearrg
-00001820: 0000 00da 0a7a 6572 6f73 5f6c 696b 6572  .....zeros_liker
-00001830: 2d00 0000 da03 696e 7472 5300 0000 290a  -.....intrS...).
-00001840: da14 6174 7472 6962 7574 655f 7072 6f70  ..attribute_prop
-00001850: 6572 7469 6573 da04 6178 6973 da06 7363  erties..axis..sc
-00001860: 6f72 6573 da0e 6d61 785f 6f63 6375 7272  ores..max_occurr
-00001870: 656e 6365 da0c 746f 705f 656c 656d 656e  ence..top_elemen
-00001880: 7473 da05 7363 6f72 65da 0874 656d 706c  ts..score..templ
-00001890: 6174 65da 0563 6f75 6e74 da06 6f75 7470  ate..count..outp
-000018a0: 7574 da04 656c 656d 7225 0000 0072 2500  ut..elemr%...r%.
-000018b0: 0000 7228 0000 00da 0b6d 6167 7069 655f  ..r(.....magpie_
-000018c0: 6d6f 6465 ab00 0000 7320 0000 0000 011c  mode....s ......
-000018d0: 0104 0104 0108 0114 0118 0108 0108 010a  ................
-000018e0: 0106 0108 010c 0116 0108 011e 0172 a200  .............r..
-000018f0: 0000 2901 723b 0000 0063 0200 0000 0000  ..).r;...c......
-00001900: 0000 0000 0000 1400 0000 0e00 0000 0300  ................
-00001910: 0000 73be 0300 0074 007c 007c 0164 018d  ..s....t.|.|.d..
-00001920: 025c 027d 027d 0374 01a0 0274 016a 0374  .\.}.}.t...t.j.t
-00001930: 016a 047c 0264 0264 038d 0274 016a 0474  .j.|.d.d...t.j.t
-00001940: 01a0 057c 0274 016a 047c 0264 0264 038d  ...|.t.j.|.d.d..
-00001950: 0218 00a1 0164 0264 038d 0274 016a 067c  .....d.d...t.j.|
-00001960: 0264 0264 038d 0274 016a 077c 0264 0264  .d.d...t.j.|.d.d
-00001970: 038d 0274 016a 077c 0264 0264 038d 0274  ...t.j.|.d.d...t
-00001980: 016a 067c 0264 0264 038d 0218 0066 0564  .j.|.d.d.....f.d
-00001990: 0464 038d 02a0 0864 04a1 0174 016a 0374  .d.....d...t.j.t
-000019a0: 016a 047c 0364 0264 038d 0274 016a 077c  .j.|.d.d...t.j.|
-000019b0: 0364 0264 038d 0274 016a 067c 0364 0264  .d.d...t.j.|.d.d
-000019c0: 038d 0218 0074 016a 0474 01a0 057c 0374  .....t.j.t...|.t
-000019d0: 016a 047c 0364 0264 038d 0218 00a1 0164  .j.|.d.d.......d
-000019e0: 0264 038d 0274 016a 077c 0364 0264 038d  .d...t.j.|.d.d..
-000019f0: 0274 016a 067c 0364 0264 038d 0274 097c  .t.j.|.d.d...t.|
-00001a00: 0383 0166 0664 0464 038d 02a0 0864 04a1  ...f.d.d.....d..
-00001a10: 0166 02a1 017d 047c 0464 0505 0019 007c  .f...}.|.d.....|
-00001a20: 0464 0619 001d 0003 003c 007c 0464 0705  .d.......<.|.d..
-00001a30: 0019 007c 0464 0619 001d 0003 003c 007c  ...|.d.......<.|
-00001a40: 0464 0805 0019 007c 0464 0619 001d 0003  .d.....|.d......
-00001a50: 003c 007c 0464 0905 0019 007c 0464 0a19  .<.|.d.....|.d..
-00001a60: 001d 0003 003c 0074 01a0 0a7c 0467 0064  .....<.t...|.g.d
-00001a70: 0ba2 01a1 027d 047c 0464 0c05 0019 0074  .....}.|.d.....t
-00001a80: 0b7c 0383 017c 006a 0c1b 0039 0003 003c  .|...|.j...9...<
-00001a90: 0069 007d 057c 006a 0d44 005d 567d 067c  .i.}.|.j.D.]V}.|
-00001aa0: 06a0 0ea1 00a0 0fa1 0044 005d 425c 027d  .........D.]B\.}
-00001ab0: 077d 087c 077c 0576 0090 0172 c27c 057c  .}.|.|.v...r.|.|
-00001ac0: 0705 0019 007c 0874 0b7c 006a 0d83 011b  .....|.t.|.j....
-00001ad0: 0037 0003 003c 006e 127c 0874 0b7c 006a  .7...<.n.|.t.|.j
-00001ae0: 0d83 011b 007c 057c 073c 0090 0171 9490  .....|.|.<...q..
-00001af0: 0171 8464 0d7d 0964 0e44 005d 3689 0074  .q.d.}.d.D.]6..t
-00001b00: 01a0 107c 047c 0974 11a0 1274 1387 0066  ...|.|.t...t...f
-00001b10: 0164 0f64 1084 087c 05a0 14a1 0044 0083  .d.d...|.....D..
-00001b20: 0183 0164 1188 001b 00a1 02a1 037d 0490  ...d.........}..
-00001b30: 0171 e474 01a0 107c 047c 0974 0b7c 0583  .q.t...|.|.t.|..
-00001b40: 01a1 037d 0464 0264 0264 0264 0264 129c  ...}.d.d.d.d.d..
-00001b50: 047d 0a64 027d 0b7c 05a0 0fa1 0044 005d  .}.d.}.|.....D.]
-00001b60: a25c 027d 077d 087c 0a64 1305 0019 007c  .\.}.}.|.d.....|
-00001b70: 0874 1574 167c 0783 016a 1764 1418 0019  .t.t.|...j.d....
-00001b80: 0064 0819 0014 0037 0003 003c 007c 0a64  .d.....7...<.|.d
-00001b90: 1505 0019 007c 0874 1574 167c 0783 016a  .....|.t.t.|...j
-00001ba0: 1764 1418 0019 0064 1619 0014 0037 0003  .d.....d.....7..
-00001bb0: 003c 007c 0a64 1705 0019 007c 0874 1574  .<.|.d.....|.t.t
-00001bc0: 167c 0783 016a 1764 1418 0019 0064 1819  .|...j.d.....d..
-00001bd0: 0014 0037 0003 003c 007c 0a64 1905 0019  ...7...<.|.d....
-00001be0: 007c 0874 1574 167c 0783 016a 1764 1418  .|.t.t.|...j.d..
-00001bf0: 0019 0064 1a19 0014 0037 0003 003c 0090  ...d.....7...<..
-00001c00: 0271 4874 1364 1b64 1c84 007c 0aa0 0fa1  .qHt.d.d...|....
-00001c10: 0044 0083 0183 017d 0b64 1244 005d 1a7d  .D.....}.d.D.].}
-00001c20: 0c74 01a0 187c 047c 0a7c 0c19 007c 0b1b  .t...|.|.|...|..
-00001c30: 00a1 027d 0490 0371 0664 027d 0d64 027d  ...}...q.d.}.d.}
-00001c40: 0e7c 05a0 0fa1 0044 005d 625c 027d 0f7d  .|.....D.]b\.}.}
-00001c50: 107c 05a0 0fa1 0044 005d 4e5c 027d 117d  .|.....D.]N\.}.}
-00001c60: 1264 1174 11a0 1964 1d74 167c 0f83 016a  .d.t...d.t.|...j
-00001c70: 1a74 167c 1183 016a 1a18 0064 1e13 0014  .t.|...j...d....
-00001c80: 00a1 0118 007d 137c 137c 0d6b 0490 0372  .....}.|.|.k...r
-00001c90: 7e7c 137d 0d7c 0e7c 137c 1014 007c 1214  ~|.}.|.|.|...|..
-00001ca0: 0037 007d 0e90 0371 4290 0371 3274 01a0  .7.}...qB..q2t..
-00001cb0: 187c 047c 0da1 027d 0474 01a0 187c 047c  .|.|...}.t...|.|
-00001cc0: 0ea1 027d 047c 04a0 1b74 016a 1ca1 017d  ...}.|...t.j...}
-00001cd0: 047c 0453 0029 1f4e 2901 7275 0000 0072  .|.S.).N).ru...r
-00001ce0: 0100 0000 2901 7299 0000 00e9 ffff ffff  ....).r.........
-00001cf0: 7211 0000 0072 0f00 0000 e907 0000 00e9  r....r..........
-00001d00: 0800 0000 e910 0000 00e9 0f00 0000 290c  ..............).
-00001d10: e904 0000 0072 0f00 0000 e909 0000 00e9  .....r..........
-00001d20: 0e00 0000 72a7 0000 0072 1f00 0000 721d  ....r....r....r.
-00001d30: 0000 00e9 1300 0000 e915 0000 00e9 1600  ................
-00001d40: 0000 e917 0000 00e9 1800 0000 e90c 0000  ................
-00001d50: 00e9 7600 0000 2905 7212 0000 0072 a400  ..v...).r....r..
-00001d60: 0000 720f 0000 00e9 0300 0000 720d 0000  ..r.........r...
-00001d70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00001d80: 0000 0500 0000 3300 0000 731a 0000 007c  ......3...s....|
-00001d90: 005d 127d 0174 00a0 017c 0188 00a1 0256  .].}.t...|.....V
-00001da0: 0001 0071 0264 0053 0072 8100 0000 2902  ...q.d.S.r....).
-00001db0: 7236 0000 0072 3800 0000 7261 0000 00a9  r6...r8...ra....
-00001dc0: 01da 0170 7225 0000 0072 2800 0000 7229  ...pr%...r(...r)
-00001dd0: 0000 00e2 0000 0072 2a00 0000 7a26 6765  .......r*...z&ge
-00001de0: 6e65 7261 7465 5f64 6573 6372 6970 746f  nerate_descripto
-00001df0: 722e 3c6c 6f63 616c 733e 2e3c 6765 6e65  r.<locals>.<gene
-00001e00: 7870 723e 6700 0000 0000 00f0 3f29 04da  xpr>g.......?)..
-00001e10: 0173 72b4 0000 00da 0164 da01 6672 b500  .sr......d..fr..
-00001e20: 0000 7220 0000 0072 b400 0000 72a9 0000  ..r ...r....r...
-00001e30: 0072 b600 0000 7212 0000 0072 b700 0000  .r....r....r....
-00001e40: e90b 0000 0063 0100 0000 0000 0000 0000  .....c..........
-00001e50: 0000 0300 0000 0400 0000 5300 0000 7314  ..........S...s.
-00001e60: 0000 0067 007c 005d 0c5c 027d 017d 027c  ...g.|.].\.}.}.|
-00001e70: 0291 0271 0453 0072 2500 0000 7225 0000  ...q.S.r%...r%..
-00001e80: 0029 0372 2600 0000 723d 0000 00da 0376  .).r&...r=.....v
-00001e90: 616c 7225 0000 0072 2500 0000 7228 0000  alr%...r%...r(..
-00001ea0: 0072 5000 0000 ec00 0000 722a 0000 007a  .rP.......r*...z
-00001eb0: 2767 656e 6572 6174 655f 6465 7363 7269  'generate_descri
-00001ec0: 7074 6f72 2e3c 6c6f 6361 6c73 3e2e 3c6c  ptor.<locals>.<l
-00001ed0: 6973 7463 6f6d 703e 6700 0000 0000 00d0  istcomp>g.......
-00001ee0: bf72 0d00 0000 291d 727e 0000 0072 2b00  .r....).r~...r+.
-00001ef0: 0000 7239 0000 00da 0573 7461 636b da04  ..r9.....stack..
-00001f00: 6d65 616e 7233 0000 0072 3500 0000 da03  meanr3...r5.....
-00001f10: 6d61 78da 0772 6573 6861 7065 72a2 0000  max..reshaper...
-00001f20: 00da 0664 656c 6574 6572 5300 0000 7223  ...deleterS...r#
-00001f30: 0000 0072 5100 0000 7230 0000 0072 3100  ...rQ...r0...r1.
-00001f40: 0000 da06 696e 7365 7274 7236 0000 0072  ....insertr6...r
-00001f50: 3800 0000 7294 0000 0072 3400 0000 722d  8...r....r4...r-
-00001f60: 0000 0072 0300 0000 7232 0000 0072 6700  ...r....r2...rg.
-00001f70: 0000 da03 6578 70da 0158 da06 6173 7479  ....exp..X..asty
-00001f80: 7065 da07 666c 6f61 7433 3229 1472 3b00  pe..float32).r;.
-00001f90: 0000 7275 0000 00da 0f64 6966 665f 7072  ..ru.....diff_pr
-00001fa0: 6f70 6572 7469 6573 7298 0000 00da 0a70  opertiesr......p
-00001fb0: 726f 7065 7274 6965 73da 0c65 6c65 6d65  roperties..eleme
-00001fc0: 6e74 5f64 6963 74da 0b63 6f6d 706f 7369  nt_dict..composi
-00001fd0: 7469 6f6e 723d 0000 0072 3e00 0000 da08  tionr=...r>.....
-00001fe0: 706f 7369 7469 6f6e da18 656c 6563 7472  position..electr
-00001ff0: 6f6e 5f6f 6363 7570 6174 696f 6e5f 6469  on_occupation_di
-00002000: 6374 da14 746f 7461 6c5f 7661 6c65 6e63  ct..total_valenc
-00002010: 655f 6661 6374 6f72 da03 6f72 62da 0e6d  e_factor..orb..m
-00002020: 6178 5f69 6f6e 6963 5f63 6861 72da 0d61  ax_ionic_char..a
-00002030: 765f 696f 6e69 635f 6368 6172 da04 6b65  v_ionic_char..ke
-00002040: 7931 da06 7661 6c75 6531 da04 6b65 7932  y1..value1..key2
-00002050: da06 7661 6c75 6532 da0a 696f 6e69 635f  ..value2..ionic_
-00002060: 6368 6172 7225 0000 0072 b300 0000 7228  charr%...r....r(
-00002070: 0000 00da 1367 656e 6572 6174 655f 6465  .....generate_de
-00002080: 7363 7269 7074 6f72 bd00 0000 7386 0000  scriptor....s...
-00002090: 0000 0110 0104 0104 010c 0120 010c 010c  ........... ....
-000020a0: 011a fc02 0402 fb06 0502 fb02 0604 010c  ................
-000020b0: 011a 0120 010c 010c 0106 fb02 0502 fa06  ... ............
-000020c0: 0602 fa02 fa02 ff04 0f14 0114 0114 0214  ................
-000020d0: 0210 021a 0204 010a 0114 010a 011c 021a  ................
-000020e0: 0104 0108 0108 0124 ff08 0212 020e 0104  .......$........
-000020f0: 0110 0126 0126 0126 012a 0116 0108 0118  ...&.&.&.*......
-00002100: 0204 0104 0110 0110 0126 010a 0104 0118  .........&......
-00002110: 010c 010c 010c 0172 d300 0000 6300 0000  .......r....c...
-00002120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
-00002130: 0043 0000 0073 0400 0000 7400 5300 7281  .C...s....t.S.r.
-00002140: 0000 0029 01da 0863 6974 6174 696f 6e72  ...)...citationr
-00002150: 2500 0000 7225 0000 0072 2500 0000 7228  %...r%...r%...r(
-00002160: 0000 00da 0463 6974 65fd 0000 0073 0200  .....cite....s..
-00002170: 0000 0001 72d5 0000 00fa 0b4a 5641 5350  ....r......JVASP
-00002180: 2d31 3030 3031 6301 0000 0000 0000 0000  -10001c.........
-00002190: 0000 0006 0000 0008 0000 0043 0000 0073  ...........C...s
-000021a0: b600 0000 7c00 6401 6b02 7216 7400 6402  ....|.d.k.r.t.d.
-000021b0: 8301 0100 6403 7d01 6e22 7c00 6404 6b02  ....d.}.n"|.d.k.
-000021c0: 722c 7400 6405 8301 0100 6406 7d01 6e0c  r,t.d.....d.}.n.
-000021d0: 7400 6407 8301 0100 6408 5300 7401 a002  t.d.....d.S.t...
-000021e0: 7403 a004 7c01 a101 a101 6701 6409 1400  t...|.....g.d...
-000021f0: 7d02 7405 7c02 8301 4400 5d0c 7d03 7406  }.t.|...D.].}.t.
-00002200: 7c03 8301 7d04 7156 7407 640a 640b 8302  |...}.qVt.d.d...
-00002210: 8f24 7d05 7c05 a008 640c 640d 8400 7c04  .$}.|...d.d...|.
-00002220: 4400 8301 a101 0100 5700 6400 0400 0400  D.......W.d.....
-00002230: 8303 0100 6e10 3100 7398 3000 0100 0100  ....n.1.s.0.....
-00002240: 0100 5900 0100 7400 640e 8301 0100 7400  ..Y...t.d.....t.
-00002250: 7c04 8301 0100 6400 5300 290f 4e72 d600  |.....d.S.).Nr..
-00002260: 0000 fa54 5072 6f66 696c 696e 672f 7465  ...TProfiling/te
-00002270: 7374 696e 6720 7461 736b 2e20 5769 6c6c  sting task. Will
-00002280: 2063 616c 6375 6c61 7465 2061 2064 6573   calculate a des
-00002290: 6372 6970 746f 7220 666f 7220 4c69 3220  criptor for Li2 
-000022a0: 5a72 3120 5465 3120 4f36 2028 4a56 4153  Zr1 Te1 O6 (JVAS
-000022b0: 502d 3130 3030 3129 e146 0a00 007b 2240  P-10001).F...{"@
-000022c0: 6d6f 6475 6c65 223a 2022 7079 6d61 7467  module": "pymatg
-000022d0: 656e 2e63 6f72 652e 7374 7275 6374 7572  en.core.structur
-000022e0: 6522 2c20 2240 636c 6173 7322 3a20 2253  e", "@class": "S
-000022f0: 7472 7563 7475 7265 222c 2022 6368 6172  tructure", "char
-00002300: 6765 223a 206e 756c 6c2c 2022 6c61 7474  ge": null, "latt
-00002310: 6963 6522 3a20 7b22 6d61 7472 6978 223a  ice": {"matrix":
-00002320: 205b 5b34 2e35 3939 3330 3536 3532 3636   [[4.59930565266
-00002330: 3234 3539 2c20 302e 3030 3938 3031 3530  2459, 0.00980150
-00002340: 3736 3939 3838 3233 2c20 332e 3130 3532  76998823, 3.1052
-00002350: 3631 3238 3635 3434 3337 3336 5d2c 205b  612865443736], [
-00002360: 312e 3635 3533 3235 3737 3236 3230 3436  1.65532577262046
-00002370: 3533 2c20 342e 3239 3131 3038 3437 3538  53, 4.2911084758
-00002380: 3534 3731 322c 2033 2e31 3035 3236 3032  54712, 3.1052602
-00002390: 3933 3839 3739 3536 355d 2c20 5b30 2e30  938979565], [0.0
-000023a0: 3134 3235 3431 3231 3439 3139 3734 392c  142541214919749,
-000023b0: 2030 2e30 3039 3830 3235 3039 3939 3936   0.0098025099996
-000023c0: 3133 312c 2035 2e35 3439 3431 3931 3431  131, 5.549419141
-000023d0: 3836 3633 3531 5d5d 2c20 2261 223a 2035  866351]], "a": 5
-000023e0: 2e35 3439 3434 3634 3738 3135 3233 3236  .549446478152326
-000023f0: 2c20 2262 223a 2035 2e35 3439 3434 3635  , "b": 5.5494465
-00002400: 3336 3137 3933 3433 2c20 2263 223a 2035  36179343, "c": 5
-00002410: 2e35 3439 3434 3631 3035 3831 3034 3233  .549446105810423
-00002420: 2c20 2261 6c70 6861 223a 2035 352e 3832  , "alpha": 55.82
-00002430: 3731 3434 3539 3938 3538 3332 2c20 2262  714459985832, "b
-00002440: 6574 6122 3a20 3535 2e38 3237 3134 3031  eta": 55.8271401
-00002450: 3432 3839 3337 312c 2022 6761 6d6d 6122  4289371, "gamma"
-00002460: 3a20 3535 2e38 3237 3133 3937 3237 3739  : 55.82713972779
-00002470: 3039 322c 2022 766f 6c75 6d65 223a 2031  092, "volume": 1
-00002480: 3039 2e31 3534 3834 3632 3536 3432 3734  09.1548462564274
-00002490: 337d 2c20 2273 6974 6573 223a 205b 7b22  3}, "sites": [{"
-000024a0: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-000024b0: 6d65 6e74 223a 2022 4c69 222c 2022 6f63  ment": "Li", "oc
-000024c0: 6375 223a 2031 2e30 7d5d 2c20 2261 6263  cu": 1.0}], "abc
-000024d0: 223a 205b 302e 3237 3338 3738 3438 3732  ": [0.2738784872
-000024e0: 3636 3939 3234 2c20 302e 3237 3338 3738  669924, 0.273878
-000024f0: 3438 3732 3637 3034 3037 2c20 302e 3237  4872670407, 0.27
-00002500: 3338 3738 3438 3732 3637 3330 3332 5d2c  38784872673032],
-00002510: 2022 7879 7a22 3a20 5b31 2e37 3136 3931   "xyz": [1.71691
-00002520: 3238 3930 3430 3037 3036 332c 2031 2e31  28904007063, 1.1
-00002530: 3830 3631 3134 3136 3737 3737 3631 332c  806114167777613,
-00002540: 2033 2e32 3230 3739 3437 3735 3337 3732   3.2207947753772
-00002550: 3738 5d2c 2022 6c61 6265 6c22 3a20 224c  78], "label": "L
-00002560: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00002570: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00002580: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00002590: 224c 6922 2c20 226f 6363 7522 3a20 312e  "Li", "occu": 1.
-000025a0: 307d 5d2c 2022 6162 6322 3a20 5b30 2e37  0}], "abc": [0.7
-000025b0: 3835 3232 3732 3031 3037 3238 3036 392c  852272010728069,
-000025c0: 2030 2e37 3835 3232 3732 3031 3037 3238   0.7852272010728
-000025d0: 3835 362c 2030 2e37 3835 3232 3732 3031  856, 0.785227201
-000025e0: 3037 3333 3135 5d2c 2022 7879 7a22 3a20  073315], "xyz": 
-000025f0: 5b34 2e39 3232 3439 3934 3531 3733 3939  [4.9224994517399
-00002600: 3635 2c20 332e 3338 3438 3838 3730 3539  65, 3.3848887059
-00002610: 3433 3439 3237 2c20 392e 3233 3432 3235  434927, 9.234225
-00002620: 3333 3831 3633 3633 335d 2c20 226c 6162  338163633], "lab
-00002630: 656c 223a 2022 4c69 222c 2022 7072 6f70  el": "Li", "prop
-00002640: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00002650: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00002660: 6d65 6e74 223a 2022 4f22 2c20 226f 6363  ment": "O", "occ
-00002670: 7522 3a20 312e 307d 5d2c 2022 6162 6322  u": 1.0}], "abc"
-00002680: 3a20 5b30 2e38 3636 3939 3634 3435 3436  : [0.86699644546
-00002690: 3631 3132 342c 2030 2e36 3034 3038 3938  61124, 0.6040898
-000026a0: 3832 3039 3231 3134 2c20 302e 3234 3138  82092114, 0.2418
-000026b0: 3231 3736 3938 3733 3134 335d 2c20 2278  21769873143], "x
-000026c0: 797a 223a 205b 342e 3939 3039 3934 3136  yz": [4.99099416
-000026d0: 3031 3634 3036 312c 2032 2e36 3033 3038  0164061, 2.60308
-000026e0: 3335 3435 3837 3638 3536 2c20 352e 3931  3545876856, 5.91
-000026f0: 3030 3737 3138 3131 3337 3635 385d 2c20  0077181137658], 
-00002700: 226c 6162 656c 223a 2022 4f22 2c20 2270  "label": "O", "p
-00002710: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00002720: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00002730: 656c 656d 656e 7422 3a20 224f 222c 2022  element": "O", "
-00002740: 6f63 6375 223a 2031 2e30 7d5d 2c20 2261  occu": 1.0}], "a
-00002750: 6263 223a 205b 302e 3731 3738 3430 3839  bc": [0.71784089
-00002760: 3435 3239 3738 382c 2030 2e31 3231 3336  4529788, 0.12136
-00002770: 3735 3838 3936 3238 3638 332c 2030 2e33  75889628683, 0.3
-00002780: 3933 3533 3730 3039 3138 3639 3733 5d2c  93537009186973],
-00002790: 2022 7879 7a22 3a20 5b33 2e35 3038 3038   "xyz": [3.50808
-000027a0: 3231 3036 3233 3437 3133 2c20 302e 3533  2106234713, 0.53
-000027b0: 3136 3935 3036 3332 3135 3431 322c 2034  1695063215412, 4
-000027c0: 2e37 3839 3836 3333 3036 3436 3932 3738  .789863306469278
-000027d0: 5d2c 2022 6c61 6265 6c22 3a20 224f 222c  ], "label": "O",
-000027e0: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-000027f0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00002800: 5b7b 2265 6c65 6d65 6e74 223a 2022 4f22  [{"element": "O"
-00002810: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
-00002820: 2022 6162 6322 3a20 5b30 2e31 3231 3336   "abc": [0.12136
-00002830: 3735 3838 3936 3338 3430 322c 2030 2e33  75889638402, 0.3
-00002840: 3933 3533 3730 3039 3138 3733 3934 332c  935370091873943,
-00002850: 2030 2e37 3137 3834 3038 3934 3532 3833   0.7178408945283
-00002860: 3338 345d 2c20 2278 797a 223a 205b 312e  384], "xyz": [1.
-00002870: 3231 3938 3730 3738 3330 3831 3738 3936  2198707830817896
-00002880: 2c20 312e 3639 3639 3336 3232 3335 3931  , 1.696936223591
-00002890: 3033 3137 2c20 352e 3538 3235 3132 3932  0317, 5.58251292
-000028a0: 3531 3639 3634 5d2c 2022 6c61 6265 6c22  516964], "label"
-000028b0: 3a20 224f 222c 2022 7072 6f70 6572 7469  : "O", "properti
-000028c0: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-000028d0: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-000028e0: 223a 2022 4f22 2c20 226f 6363 7522 3a20  ": "O", "occu": 
-000028f0: 312e 307d 5d2c 2022 6162 6322 3a20 5b30  1.0}], "abc": [0
-00002900: 2e33 3933 3533 3730 3039 3138 3631 3931  .393537009186191
-00002910: 352c 2030 2e37 3137 3834 3038 3934 3532  5, 0.71784089452
-00002920: 3933 3835 362c 2030 2e31 3231 3336 3735  93856, 0.1213675
-00002930: 3838 3936 3334 3031 345d 2c20 2278 797a  889634014], "xyz
-00002940: 223a 205b 322e 3939 3939 3837 3531 3235  ": [2.9999875125
-00002950: 3935 3632 322c 2033 2e30 3835 3338 3031  95622, 3.0853801
-00002960: 3039 3836 3033 3434 2c20 342e 3132 3436  09860344, 4.1246
-00002970: 3337 3638 3739 3632 3239 375d 2c20 226c  37687962297], "l
-00002980: 6162 656c 223a 2022 4f22 2c20 2270 726f  abel": "O", "pro
-00002990: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-000029a0: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-000029b0: 656d 656e 7422 3a20 224f 222c 2022 6f63  ement": "O", "oc
-000029c0: 6375 223a 2031 2e30 7d5d 2c20 2261 6263  cu": 1.0}], "abc
-000029d0: 223a 205b 302e 3234 3138 3231 3736 3938  ": [0.2418217698
-000029e0: 3732 3135 3733 2c20 302e 3836 3639 3936  721573, 0.866996
-000029f0: 3434 3534 3637 3132 3231 2c20 302e 3630  4454671221, 0.60
-00002a00: 3430 3839 3838 3230 3932 3135 3133 5d2c  40898820921513],
-00002a10: 2022 7879 7a22 3a20 5b32 2e35 3535 3938   "xyz": [2.55598
-00002a20: 3435 3634 3633 3333 3239 2c20 332e 3732  4564633329, 3.72
-00002a30: 3836 3637 3631 3037 3239 3134 392c 2036  8667610729149, 6
-00002a40: 2e37 3935 3531 3733 3732 3337 3733 3433  .795517372377343
-00002a50: 5d2c 2022 6c61 6265 6c22 3a20 224f 222c  ], "label": "O",
-00002a60: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00002a70: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00002a80: 5b7b 2265 6c65 6d65 6e74 223a 2022 4f22  [{"element": "O"
-00002a90: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
-00002aa0: 2022 6162 6322 3a20 5b30 2e36 3034 3038   "abc": [0.60408
-00002ab0: 3938 3832 3039 3333 3131 352c 2030 2e32  98820933115, 0.2
-00002ac0: 3431 3832 3137 3639 3837 3233 3633 372c  418217698723637,
-00002ad0: 2030 2e38 3636 3939 3634 3435 3436 3634   0.8669964454664
-00002ae0: 3035 395d 2c20 2278 797a 223a 205b 332e  059], "xyz": [3.
-00002af0: 3139 3130 3436 3039 3031 3435 3137 332c  191046090145173,
-00002b00: 2031 2e30 3532 3130 3331 3739 3330 3235   1.0521031793025
-00002b10: 3539 352c 2037 2e34 3338 3130 3331 3335  595, 7.438103135
-00002b20: 3034 3336 3533 355d 2c20 226c 6162 656c  0436535], "label
-00002b30: 223a 2022 4f22 2c20 2270 726f 7065 7274  ": "O", "propert
-00002b40: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
-00002b50: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
-00002b60: 7422 3a20 2254 6522 2c20 226f 6363 7522  t": "Te", "occu"
-00002b70: 3a20 312e 307d 5d2c 2022 6162 6322 3a20  : 1.0}], "abc": 
-00002b80: 5b30 2e34 3936 3539 3035 3631 3035 3037  [0.4965905610507
-00002b90: 3335 332c 2030 2e34 3936 3539 3035 3631  353, 0.496590561
-00002ba0: 3035 3037 3335 352c 2030 2e34 3936 3539  0507355, 0.49659
-00002bb0: 3035 3631 3035 3037 3336 315d 2c20 2278  05610507361], "x
-00002bc0: 797a 223a 205b 332e 3131 3330 3639 3339  yz": [3.11306939
-00002bd0: 3038 3335 3739 332c 2032 2e31 3430 3635  0835793, 2.14065
-00002be0: 3931 3335 3730 3234 3938 342c 2035 2e38  91357024984, 5.8
-00002bf0: 3339 3837 3535 3631 3231 3436 3632 345d  398755612146624]
-00002c00: 2c20 226c 6162 656c 223a 2022 5465 222c  , "label": "Te",
-00002c10: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00002c20: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00002c30: 5b7b 2265 6c65 6d65 6e74 223a 2022 5a72  [{"element": "Zr
-00002c40: 222c 2022 6f63 6375 223a 2031 2e30 7d5d  ", "occu": 1.0}]
-00002c50: 2c20 2261 6263 223a 205b 302e 3030 3036  , "abc": [0.0006
-00002c60: 3530 3136 3034 3938 3036 3638 2c20 302e  501604980668, 0.
-00002c70: 3030 3036 3530 3136 3034 3938 3039 3238  0006501604980928
-00002c80: 2c20 302e 3030 3036 3530 3136 3034 3938  , 0.000650160498
-00002c90: 3233 3434 5d2c 2022 7879 7a22 3a20 5b30  2344], "xyz": [0
-00002ca0: 2e30 3034 3037 3537 3831 3734 3934 3630  .004075781749460
-00002cb0: 3336 2c20 302e 3030 3238 3032 3635 3439  36, 0.0028026549
-00002cc0: 3831 3934 3531 3932 2c20 302e 3030 3736  81945192, 0.0076
-00002cd0: 3435 3834 3839 3138 3236 3330 3736 5d2c  45848918263076],
-00002ce0: 2022 6c61 6265 6c22 3a20 225a 7222 2c20   "label": "Zr", 
-00002cf0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00002d00: 7d5d 7dda 0d64 696c 7574 654e 6941 6c6c  }]}..diluteNiAll
-00002d10: 6f79 fa4d 5072 6f66 696c 696e 672f 7465  oy.MProfiling/te
-00002d20: 7374 696e 6720 7461 736b 2e20 5769 6c6c  sting task. Will
-00002d30: 2063 616c 6375 6c61 7465 2061 2064 6573   calculate a des
-00002d40: 6372 6970 746f 7220 666f 7220 6120 6469  criptor for a di
-00002d50: 6c75 7465 2046 4343 204e 6933 3143 7231  lute FCC Ni31Cr1
-00002d60: 2ee1 d414 0000 7b22 406d 6f64 756c 6522  ......{"@module"
-00002d70: 3a20 2270 796d 6174 6765 6e2e 636f 7265  : "pymatgen.core
-00002d80: 2e73 7472 7563 7475 7265 222c 2022 4063  .structure", "@c
-00002d90: 6c61 7373 223a 2022 5374 7275 6374 7572  lass": "Structur
-00002da0: 6522 2c20 2263 6861 7267 6522 3a20 6e75  e", "charge": nu
-00002db0: 6c6c 2c20 226c 6174 7469 6365 223a 207b  ll, "lattice": {
-00002dc0: 226d 6174 7269 7822 3a20 5b5b 362e 3939  "matrix": [[6.99
-00002dd0: 3536 3932 2c20 302e 302c 2030 2e30 5d2c  5692, 0.0, 0.0],
-00002de0: 205b 302e 302c 2036 2e39 3935 3639 322c   [0.0, 6.995692,
-00002df0: 2030 2e30 5d2c 205b 302e 302c 2030 2e30   0.0], [0.0, 0.0
-00002e00: 2c20 362e 3939 3536 3932 5d5d 2c20 2261  , 6.995692]], "a
-00002e10: 223a 2036 2e39 3935 3639 322c 2022 6222  ": 6.995692, "b"
-00002e20: 3a20 362e 3939 3536 3932 2c20 2263 223a  : 6.995692, "c":
-00002e30: 2036 2e39 3935 3639 322c 2022 616c 7068   6.995692, "alph
-00002e40: 6122 3a20 3930 2e30 2c20 2262 6574 6122  a": 90.0, "beta"
-00002e50: 3a20 3930 2e30 2c20 2267 616d 6d61 223a  : 90.0, "gamma":
-00002e60: 2039 302e 302c 2022 766f 6c75 6d65 223a   90.0, "volume":
-00002e70: 2033 3432 2e33 3637 3131 3336 3536 3139   342.36711365619
-00002e80: 3234 337d 2c20 2273 6974 6573 223a 205b  243}, "sites": [
-00002e90: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-00002ea0: 6c65 6d65 6e74 223a 2022 4372 222c 2022  lement": "Cr", "
-00002eb0: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-00002ec0: 223a 205b 302e 302c 2030 2e30 2c20 302e  ": [0.0, 0.0, 0.
-00002ed0: 305d 2c20 2278 797a 223a 205b 302e 302c  0], "xyz": [0.0,
-00002ee0: 2030 2e30 2c20 302e 305d 2c20 226c 6162   0.0, 0.0], "lab
-00002ef0: 656c 223a 2022 4372 222c 2022 7072 6f70  el": "Cr", "prop
-00002f00: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00002f10: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00002f20: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-00002f30: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-00002f40: 205b 302e 302c 2030 2e30 2c20 302e 355d   [0.0, 0.0, 0.5]
-00002f50: 2c20 2278 797a 223a 205b 302e 302c 2030  , "xyz": [0.0, 0
-00002f60: 2e30 2c20 332e 3439 3738 3436 5d2c 2022  .0, 3.497846], "
-00002f70: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-00002f80: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00002f90: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00002fa0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-00002fb0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00002fc0: 6322 3a20 5b30 2e30 2c20 302e 352c 2030  c": [0.0, 0.5, 0
-00002fd0: 2e30 5d2c 2022 7879 7a22 3a20 5b30 2e30  .0], "xyz": [0.0
-00002fe0: 2c20 332e 3439 3738 3436 2c20 302e 305d  , 3.497846, 0.0]
-00002ff0: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003000: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003010: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003020: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003030: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003040: 2261 6263 223a 205b 302e 302c 2030 2e35  "abc": [0.0, 0.5
-00003050: 2c20 302e 355d 2c20 2278 797a 223a 205b  , 0.5], "xyz": [
-00003060: 302e 302c 2033 2e34 3937 3834 362c 2033  0.0, 3.497846, 3
-00003070: 2e34 3937 3834 365d 2c20 226c 6162 656c  .497846], "label
-00003080: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00003090: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000030a0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000030b0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000030c0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000030d0: 302e 352c 2030 2e30 2c20 302e 305d 2c20  0.5, 0.0, 0.0], 
-000030e0: 2278 797a 223a 205b 332e 3439 3738 3436  "xyz": [3.497846
-000030f0: 2c20 302e 302c 2030 2e30 5d2c 2022 6c61  , 0.0, 0.0], "la
-00003100: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003110: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00003120: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00003130: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-00003140: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-00003150: 3a20 5b30 2e35 2c20 302e 302c 2030 2e35  : [0.5, 0.0, 0.5
-00003160: 5d2c 2022 7879 7a22 3a20 5b33 2e34 3937  ], "xyz": [3.497
-00003170: 3834 362c 2030 2e30 2c20 332e 3439 3738  846, 0.0, 3.4978
-00003180: 3436 5d2c 2022 6c61 6265 6c22 3a20 224e  46], "label": "N
-00003190: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-000031a0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-000031b0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-000031c0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-000031d0: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
-000031e0: 302e 352c 2030 2e30 5d2c 2022 7879 7a22  0.5, 0.0], "xyz"
-000031f0: 3a20 5b33 2e34 3937 3834 362c 2033 2e34  : [3.497846, 3.4
-00003200: 3937 3834 362c 2030 2e30 5d2c 2022 6c61  97846, 0.0], "la
-00003210: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003220: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00003230: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00003240: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-00003250: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-00003260: 3a20 5b30 2e35 2c20 302e 352c 2030 2e35  : [0.5, 0.5, 0.5
-00003270: 5d2c 2022 7879 7a22 3a20 5b33 2e34 3937  ], "xyz": [3.497
-00003280: 3834 362c 2033 2e34 3937 3834 362c 2033  846, 3.497846, 3
-00003290: 2e34 3937 3834 365d 2c20 226c 6162 656c  .497846], "label
-000032a0: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-000032b0: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000032c0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000032d0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000032e0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000032f0: 302e 3235 2c20 302e 3235 2c20 302e 305d  0.25, 0.25, 0.0]
-00003300: 2c20 2278 797a 223a 205b 312e 3734 3839  , "xyz": [1.7489
-00003310: 3233 2c20 312e 3734 3839 3233 2c20 302e  23, 1.748923, 0.
-00003320: 305d 2c20 226c 6162 656c 223a 2022 4e69  0], "label": "Ni
-00003330: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00003340: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00003350: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00003360: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00003370: 2c20 2261 6263 223a 205b 302e 3235 2c20  , "abc": [0.25, 
-00003380: 302e 3235 2c20 302e 355d 2c20 2278 797a  0.25, 0.5], "xyz
-00003390: 223a 205b 312e 3734 3839 3233 2c20 312e  ": [1.748923, 1.
-000033a0: 3734 3839 3233 2c20 332e 3439 3738 3436  748923, 3.497846
-000033b0: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
-000033c0: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
-000033d0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
-000033e0: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
-000033f0: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
-00003400: 2022 6162 6322 3a20 5b30 2e32 352c 2030   "abc": [0.25, 0
-00003410: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
-00003420: 312c 2030 2e30 5d2c 2022 7879 7a22 3a20  1, 0.0], "xyz": 
-00003430: 5b31 2e37 3438 3932 332c 2035 2e32 3436  [1.748923, 5.246
-00003440: 3736 3930 3030 3030 3030 3030 352c 2030  7690000000005, 0
-00003450: 2e30 5d2c 2022 6c61 6265 6c22 3a20 224e  .0], "label": "N
-00003460: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003470: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003480: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003490: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-000034a0: 5d2c 2022 6162 6322 3a20 5b30 2e32 352c  ], "abc": [0.25,
-000034b0: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
-000034c0: 3030 312c 2030 2e35 5d2c 2022 7879 7a22  001, 0.5], "xyz"
-000034d0: 3a20 5b31 2e37 3438 3932 332c 2035 2e32  : [1.748923, 5.2
-000034e0: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
-000034f0: 2033 2e34 3937 3834 365d 2c20 226c 6162   3.497846], "lab
-00003500: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
-00003510: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00003520: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00003530: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-00003540: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-00003550: 205b 302e 3735 3030 3030 3030 3030 3030   [0.750000000000
-00003560: 3030 3031 2c20 302e 3235 2c20 302e 305d  0001, 0.25, 0.0]
-00003570: 2c20 2278 797a 223a 205b 352e 3234 3637  , "xyz": [5.2467
-00003580: 3639 3030 3030 3030 3030 3035 2c20 312e  690000000005, 1.
-00003590: 3734 3839 3233 2c20 302e 305d 2c20 226c  748923, 0.0], "l
-000035a0: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-000035b0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-000035c0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-000035d0: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
-000035e0: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-000035f0: 223a 205b 302e 3735 3030 3030 3030 3030  ": [0.7500000000
-00003600: 3030 3030 3031 2c20 302e 3235 2c20 302e  000001, 0.25, 0.
-00003610: 355d 2c20 2278 797a 223a 205b 352e 3234  5], "xyz": [5.24
-00003620: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
-00003630: 312e 3734 3839 3233 2c20 332e 3439 3738  1.748923, 3.4978
-00003640: 3436 5d2c 2022 6c61 6265 6c22 3a20 224e  46], "label": "N
-00003650: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003660: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003670: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003680: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00003690: 5d2c 2022 6162 6322 3a20 5b30 2e37 3530  ], "abc": [0.750
-000036a0: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
-000036b0: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
-000036c0: 312c 2030 2e30 5d2c 2022 7879 7a22 3a20  1, 0.0], "xyz": 
-000036d0: 5b35 2e32 3436 3736 3930 3030 3030 3030  [5.2467690000000
-000036e0: 3030 352c 2035 2e32 3436 3736 3930 3030  005, 5.246769000
-000036f0: 3030 3030 3030 352c 2030 2e30 5d2c 2022  0000005, 0.0], "
-00003700: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-00003710: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00003720: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00003730: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-00003740: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00003750: 6322 3a20 5b30 2e37 3530 3030 3030 3030  c": [0.750000000
-00003760: 3030 3030 3030 312c 2030 2e37 3530 3030  0000001, 0.75000
-00003770: 3030 3030 3030 3030 3030 312c 2030 2e35  00000000001, 0.5
-00003780: 5d2c 2022 7879 7a22 3a20 5b35 2e32 3436  ], "xyz": [5.246
-00003790: 3736 3930 3030 3030 3030 3030 352c 2035  7690000000005, 5
-000037a0: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
-000037b0: 352c 2033 2e34 3937 3834 365d 2c20 226c  5, 3.497846], "l
-000037c0: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-000037d0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-000037e0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-000037f0: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
-00003800: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-00003810: 223a 205b 302e 3235 2c20 302e 302c 2030  ": [0.25, 0.0, 0
-00003820: 2e32 355d 2c20 2278 797a 223a 205b 312e  .25], "xyz": [1.
-00003830: 3734 3839 3233 2c20 302e 302c 2031 2e37  748923, 0.0, 1.7
-00003840: 3438 3932 335d 2c20 226c 6162 656c 223a  48923], "label":
-00003850: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-00003860: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-00003870: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-00003880: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00003890: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-000038a0: 3235 2c20 302e 302c 2030 2e37 3530 3030  25, 0.0, 0.75000
-000038b0: 3030 3030 3030 3030 3030 315d 2c20 2278  00000000001], "x
-000038c0: 797a 223a 205b 312e 3734 3839 3233 2c20  yz": [1.748923, 
-000038d0: 302e 302c 2035 2e32 3436 3736 3930 3030  0.0, 5.246769000
-000038e0: 3030 3030 3030 355d 2c20 226c 6162 656c  0000005], "label
-000038f0: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00003900: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003910: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-00003920: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-00003930: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-00003940: 302e 3235 2c20 302e 352c 2030 2e32 355d  0.25, 0.5, 0.25]
-00003950: 2c20 2278 797a 223a 205b 312e 3734 3839  , "xyz": [1.7489
-00003960: 3233 2c20 332e 3439 3738 3436 2c20 312e  23, 3.497846, 1.
-00003970: 3734 3839 3233 5d2c 2022 6c61 6265 6c22  748923], "label"
-00003980: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
-00003990: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
-000039a0: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
-000039b0: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
-000039c0: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
-000039d0: 2e32 352c 2030 2e35 2c20 302e 3735 3030  .25, 0.5, 0.7500
-000039e0: 3030 3030 3030 3030 3030 3031 5d2c 2022  000000000001], "
-000039f0: 7879 7a22 3a20 5b31 2e37 3438 3932 332c  xyz": [1.748923,
-00003a00: 2033 2e34 3937 3834 362c 2035 2e32 3436   3.497846, 5.246
-00003a10: 3736 3930 3030 3030 3030 3030 355d 2c20  7690000000005], 
-00003a20: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
-00003a30: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
-00003a40: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
-00003a50: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
-00003a60: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
-00003a70: 6263 223a 205b 302e 3735 3030 3030 3030  bc": [0.75000000
-00003a80: 3030 3030 3030 3031 2c20 302e 302c 2030  00000001, 0.0, 0
-00003a90: 2e32 355d 2c20 2278 797a 223a 205b 352e  .25], "xyz": [5.
-00003aa0: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
-00003ab0: 2c20 302e 302c 2031 2e37 3438 3932 335d  , 0.0, 1.748923]
-00003ac0: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003ad0: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003ae0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003af0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003b00: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003b10: 2261 6263 223a 205b 302e 3735 3030 3030  "abc": [0.750000
-00003b20: 3030 3030 3030 3030 3031 2c20 302e 302c  0000000001, 0.0,
-00003b30: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
-00003b40: 3030 315d 2c20 2278 797a 223a 205b 352e  001], "xyz": [5.
-00003b50: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
-00003b60: 2c20 302e 302c 2035 2e32 3436 3736 3930  , 0.0, 5.2467690
-00003b70: 3030 3030 3030 3030 355d 2c20 226c 6162  000000005], "lab
-00003b80: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
-00003b90: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00003ba0: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00003bb0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-00003bc0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-00003bd0: 205b 302e 3735 3030 3030 3030 3030 3030   [0.750000000000
-00003be0: 3030 3031 2c20 302e 352c 2030 2e32 355d  0001, 0.5, 0.25]
-00003bf0: 2c20 2278 797a 223a 205b 352e 3234 3637  , "xyz": [5.2467
-00003c00: 3639 3030 3030 3030 3030 3035 2c20 332e  690000000005, 3.
-00003c10: 3439 3738 3436 2c20 312e 3734 3839 3233  497846, 1.748923
-00003c20: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
-00003c30: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
-00003c40: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
-00003c50: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
-00003c60: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
-00003c70: 2022 6162 6322 3a20 5b30 2e37 3530 3030   "abc": [0.75000
-00003c80: 3030 3030 3030 3030 3030 312c 2030 2e35  00000000001, 0.5
-00003c90: 2c20 302e 3735 3030 3030 3030 3030 3030  , 0.750000000000
-00003ca0: 3030 3031 5d2c 2022 7879 7a22 3a20 5b35  0001], "xyz": [5
-00003cb0: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
-00003cc0: 352c 2033 2e34 3937 3834 362c 2035 2e32  5, 3.497846, 5.2
-00003cd0: 3436 3736 3930 3030 3030 3030 3030 355d  467690000000005]
-00003ce0: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003cf0: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003d00: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003d10: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003d20: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003d30: 2261 6263 223a 205b 302e 302c 2030 2e32  "abc": [0.0, 0.2
-00003d40: 352c 2030 2e32 355d 2c20 2278 797a 223a  5, 0.25], "xyz":
-00003d50: 205b 302e 302c 2031 2e37 3438 3932 332c   [0.0, 1.748923,
-00003d60: 2031 2e37 3438 3932 335d 2c20 226c 6162   1.748923], "lab
-00003d70: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
-00003d80: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00003d90: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00003da0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-00003db0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-00003dc0: 205b 302e 302c 2030 2e32 352c 2030 2e37   [0.0, 0.25, 0.7
-00003dd0: 3530 3030 3030 3030 3030 3030 3030 315d  500000000000001]
-00003de0: 2c20 2278 797a 223a 205b 302e 302c 2031  , "xyz": [0.0, 1
-00003df0: 2e37 3438 3932 332c 2035 2e32 3436 3736  .748923, 5.24676
-00003e00: 3930 3030 3030 3030 3030 355d 2c20 226c  90000000005], "l
-00003e10: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-00003e20: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
-00003e30: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
-00003e40: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
-00003e50: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
-00003e60: 223a 205b 302e 302c 2030 2e37 3530 3030  ": [0.0, 0.75000
-00003e70: 3030 3030 3030 3030 3030 312c 2030 2e32  00000000001, 0.2
-00003e80: 355d 2c20 2278 797a 223a 205b 302e 302c  5], "xyz": [0.0,
-00003e90: 2035 2e32 3436 3736 3930 3030 3030 3030   5.2467690000000
-00003ea0: 3030 352c 2031 2e37 3438 3932 335d 2c20  005, 1.748923], 
-00003eb0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
-00003ec0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
-00003ed0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
-00003ee0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
-00003ef0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
-00003f00: 6263 223a 205b 302e 302c 2030 2e37 3530  bc": [0.0, 0.750
-00003f10: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
-00003f20: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
-00003f30: 315d 2c20 2278 797a 223a 205b 302e 302c  1], "xyz": [0.0,
-00003f40: 2035 2e32 3436 3736 3930 3030 3030 3030   5.2467690000000
-00003f50: 3030 352c 2035 2e32 3436 3736 3930 3030  005, 5.246769000
-00003f60: 3030 3030 3030 355d 2c20 226c 6162 656c  0000005], "label
-00003f70: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00003f80: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003f90: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-00003fa0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-00003fb0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-00003fc0: 302e 352c 2030 2e32 352c 2030 2e32 355d  0.5, 0.25, 0.25]
-00003fd0: 2c20 2278 797a 223a 205b 332e 3439 3738  , "xyz": [3.4978
-00003fe0: 3436 2c20 312e 3734 3839 3233 2c20 312e  46, 1.748923, 1.
-00003ff0: 3734 3839 3233 5d2c 2022 6c61 6265 6c22  748923], "label"
-00004000: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
-00004010: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
-00004020: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
-00004030: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
-00004040: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
-00004050: 2e35 2c20 302e 3235 2c20 302e 3735 3030  .5, 0.25, 0.7500
-00004060: 3030 3030 3030 3030 3030 3031 5d2c 2022  000000000001], "
-00004070: 7879 7a22 3a20 5b33 2e34 3937 3834 362c  xyz": [3.497846,
-00004080: 2031 2e37 3438 3932 332c 2035 2e32 3436   1.748923, 5.246
-00004090: 3736 3930 3030 3030 3030 3030 355d 2c20  7690000000005], 
-000040a0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
-000040b0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
-000040c0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
-000040d0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
-000040e0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
-000040f0: 6263 223a 205b 302e 352c 2030 2e37 3530  bc": [0.5, 0.750
-00004100: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
-00004110: 2e32 355d 2c20 2278 797a 223a 205b 332e  .25], "xyz": [3.
-00004120: 3439 3738 3436 2c20 352e 3234 3637 3639  497846, 5.246769
-00004130: 3030 3030 3030 3030 3035 2c20 312e 3734  0000000005, 1.74
-00004140: 3839 3233 5d2c 2022 6c61 6265 6c22 3a20  8923], "label": 
-00004150: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-00004160: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00004170: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00004180: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-00004190: 317d 5d2c 2022 6162 6322 3a20 5b30 2e35  1}], "abc": [0.5
-000041a0: 2c20 302e 3735 3030 3030 3030 3030 3030  , 0.750000000000
-000041b0: 3030 3031 2c20 302e 3735 3030 3030 3030  0001, 0.75000000
-000041c0: 3030 3030 3030 3031 5d2c 2022 7879 7a22  00000001], "xyz"
-000041d0: 3a20 5b33 2e34 3937 3834 362c 2035 2e32  : [3.497846, 5.2
-000041e0: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
-000041f0: 2035 2e32 3436 3736 3930 3030 3030 3030   5.2467690000000
-00004200: 3030 355d 2c20 226c 6162 656c 223a 2022  005], "label": "
-00004210: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
-00004220: 223a 207b 7d7d 5d2c 2022 4076 6572 7369  ": {}}], "@versi
-00004230: 6f6e 223a 206e 756c 6c7d fa17 556e 7265  on": null}..Unre
-00004240: 636f 676e 697a 6564 2074 6573 7420 6e61  cognized test na
-00004250: 6d65 2e72 0100 0000 7212 0000 007a 154b  me.r....r....z.K
-00004260: 5332 3032 325f 5465 7374 5265 7375 6c74  S2022_TestResult
-00004270: 2e63 7376 7a02 772b 6301 0000 0000 0000  .csvz.w+c.......
-00004280: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
-00004290: 0073 1600 0000 6700 7c00 5d0e 7d01 7c01  .s....g.|.].}.|.
-000042a0: 9b00 6400 9d02 9102 7104 5300 2901 da01  ..d.....q.S.)...
-000042b0: 0a72 2500 0000 2902 7226 0000 00da 0176  .r%...).r&.....v
-000042c0: 7225 0000 0072 2500 0000 7228 0000 0072  r%...r%...r(...r
-000042d0: 5000 0000 0e01 0000 722a 0000 007a 1b70  P.......r*...z.p
-000042e0: 726f 6669 6c65 2e3c 6c6f 6361 6c73 3e2e  rofile.<locals>.
-000042f0: 3c6c 6973 7463 6f6d 703e fa05 446f 6e65  <listcomp>..Done
-00004300: 2129 0972 5400 0000 7202 0000 00da 0966  !).rT...r......f
-00004310: 726f 6d5f 6469 6374 da04 6a73 6f6e da05  rom_dict..json..
-00004320: 6c6f 6164 7372 0600 0000 72d3 0000 00da  loadsr....r.....
-00004330: 046f 7065 6eda 0a77 7269 7465 6c69 6e65  .open..writeline
-00004340: 7329 06da 0474 6573 74da 066d 6174 5374  s)...test..matSt
-00004350: 72da 0373 3130 72b5 0000 0072 b600 0000  r..s10r....r....
-00004360: 72b7 0000 0072 2500 0000 7225 0000 0072  r....r%...r%...r
-00004370: 2800 0000 da07 7072 6f66 696c 6500 0100  (.....profile...
-00004380: 0073 1e00 0000 0001 0801 0801 0601 0801  .s..............
-00004390: 0801 0602 0801 0401 1601 0c01 0a01 0c01  ................
-000043a0: 3201 0801 72e8 0000 0063 0100 0000 0000  2...r....c......
-000043b0: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
-000043c0: 0000 7378 0000 0064 0164 026c 006d 017d  ..sx...d.d.l.m.}
-000043d0: 0101 007c 0064 036b 0272 2274 0264 0483  ...|.d.k.r"t.d..
-000043e0: 0101 0064 057d 026e 227c 0064 066b 0272  ...d.}.n"|.d.k.r
-000043f0: 3874 0264 0783 0101 0064 087d 026e 0c74  8t.d.....d.}.n.t
-00004400: 0264 0983 0101 0064 0153 0074 03a0 0474  .d.....d.S.t...t
-00004410: 05a0 067c 02a1 01a1 017d 037c 0367 0164  ...|.....}.|.g.d
-00004420: 0a14 007d 047c 0174 077c 0464 0b64 0c8d  ...}.|.t.|.d.d..
-00004430: 037d 0574 0264 0d83 0101 0064 0e53 0029  .}.t.d.....d.S.)
-00004440: 0f4e 7201 0000 0029 01da 0b70 726f 6365  .Nr....)...proce
-00004450: 7373 5f6d 6170 72d6 0000 0072 d700 0000  ss_mapr....r....
-00004460: 72d8 0000 0072 d900 0000 72da 0000 0072  r....r....r....r
-00004470: db00 0000 72dc 0000 0069 e803 0000 7212  ....r....i....r.
-00004480: 0000 0029 01da 0b6d 6178 5f77 6f72 6b65  ...)...max_worke
-00004490: 7273 72df 0000 0072 2000 0000 2908 da17  rsr....r ...)...
-000044a0: 7471 646d 2e63 6f6e 7472 6962 2e63 6f6e  tqdm.contrib.con
-000044b0: 6375 7272 656e 7472 e900 0000 7254 0000  currentr....rT..
-000044c0: 0072 0200 0000 72e0 0000 0072 e100 0000  .r....r....r....
-000044d0: 72e2 0000 0072 d300 0000 2906 72e5 0000  r....r....).r...
-000044e0: 0072 e900 0000 72e6 0000 0072 b500 0000  .r....r....r....
-000044f0: da05 7331 3030 30da 0864 6573 634c 6973  ..s1000..descLis
-00004500: 7472 2500 0000 7225 0000 0072 2800 0000  tr%...r%...r(...
-00004510: da0f 7072 6f66 696c 6550 6172 616c 6c65  ..profileParalle
-00004520: 6c12 0100 0073 1c00 0000 0001 0c01 0801  l....s..........
-00004530: 0801 0601 0801 0801 0602 0801 0401 1002  ................
-00004540: 0a01 0e01 0801 72ee 0000 00da 085f 5f6d  ......r......__m
-00004550: 6169 6e5f 5f72 d900 0000 2901 72e5 0000  ain__r....).r...
-00004560: 0029 0172 0100 0000 2901 7257 0000 0029  .).r....).rW...)
-00004570: 0172 d600 0000 2901 72d6 0000 0029 2372  .r....).r....)#r
-00004580: 3600 0000 da04 7469 6d65 da05 6e75 6d70  6.....time..nump
-00004590: 7972 2b00 0000 da02 6f73 da0d 7079 6d61  yr+.....os..pyma
-000045a0: 7467 656e 2e63 6f72 6572 0200 0000 7203  tgen.corer....r.
-000045b0: 0000 00da 1b70 796d 6174 6765 6e2e 616e  .....pymatgen.an
-000045c0: 616c 7973 6973 2e6c 6f63 616c 5f65 6e76  alysis.local_env
-000045d0: 7204 0000 00da 1a70 796d 6174 6765 6e2e  r......pymatgen.
-000045e0: 7379 6d6d 6574 7279 2e61 6e61 6c79 7a65  symmetry.analyze
-000045f0: 7272 0500 0000 72e1 0000 0072 0600 0000  rr....r....r....
-00004600: da0b 636f 6c6c 6563 7469 6f6e 7372 0700  ..collectionsr..
-00004610: 0000 72d4 0000 00da 1370 6572 696f 6469  ..r......periodi
-00004620: 635f 7461 626c 655f 7369 7a65 da07 6c6f  c_table_size..lo
-00004630: 6164 7478 74da 0470 6174 6872 7000 0000  adtxt..pathrp...
-00004640: da07 6469 726e 616d 65da 085f 5f66 696c  ..dirname..__fil
-00004650: 655f 5f72 2d00 0000 da0a 6e61 6e5f 746f  e__r-.....nan_to
-00004660: 5f6e 756d 724b 0000 0072 5600 0000 727e  _numrK...rV...r~
-00004670: 0000 0072 6200 0000 72a2 0000 0072 d300  ...rb...r....r..
-00004680: 0000 72d5 0000 0072 e800 0000 72ee 0000  ..r....r....r...
-00004690: 0072 8e00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-000046a0: 7225 0000 0072 2800 0000 da08 3c6d 6f64  r%...r(.....<mod
-000046b0: 756c 653e 0a00 0000 7338 0000 0008 0108  ule>....s8......
-000046c0: 0108 0108 0110 010c 010c 0108 010c 010c  ................
-000046d0: 0204 0204 0120 010a 0208 0106 ff06 0508  ..... ..........
-000046e0: 2808 0a0e 3f0e 1a0a 1210 4008 030a 120a  (...?.....@.....
-000046f0: 120a 020a 03                             .....
+00000070: 6d0a 5a0a 0100 6400 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
+00000080: 0100 6406 6407 6702 5a0d 6408 5a0e 6503  ..d.d.g.Z.d.Z.e.
+00000090: 6a0f 6504 6a10 a011 6504 6a10 a012 6513  j.e.j...e.j...e.
+000000a0: a101 6409 a102 640a 640b 8d02 5a14 6503  ..d...d.d...Z.e.
+000000b0: a015 6514 a101 5a14 6514 6401 6401 8502  ..e...Z.e.d.d...
+000000c0: 6700 640c a201 6602 1900 5a14 6516 640d  g.d...f...Z.e.d.
+000000d0: 9c01 640e 640f 8404 5a17 4700 6410 6411  ..d.d...Z.G.d.d.
+000000e0: 8400 6411 8302 5a18 6517 6601 6506 6412  ..d...Z.e.f.e.d.
+000000f0: 9c01 6413 6414 8405 5a19 6506 650c 651a  ..d.d...Z.e.e.e.
+00000100: 1900 6415 9c02 6416 6417 8404 5a1b 6429  ..d...d.d...Z.d)
+00000110: 6418 6419 8401 5a1c 6506 6503 6a1d 641a  d.d...Z.e.e.j.d.
+00000120: 9c02 641b 641c 8404 5a1e 650c 651f 1900  ..d.d...Z.e.e...
+00000130: 640d 9c01 641d 641e 8404 5a20 642a 6421  d...d.d...Z d*d!
+00000140: 6422 8401 5a21 642b 6424 6425 8401 5a22  d"..Z!d+d$d%..Z"
+00000150: 6523 6426 6b02 9001 7254 6521 641f 6427  e#d&k...rTe!d.d'
+00000160: 8d01 0100 6521 6428 6427 8d01 0100 6522  ....e!d(d'....e"
+00000170: 641f 6427 8d01 0100 6522 6428 6427 8d01  d.d'....e"d(d'..
+00000180: 0100 6401 5300 292c e900 0000 004e 2902  ..d.S.),.....N).
+00000190: da09 5374 7275 6374 7572 65da 0745 6c65  ..Structure..Ele
+000001a0: 6d65 6e74 2901 da09 566f 726f 6e6f 694e  ment)...VoronoiN
+000001b0: 4e29 01da 0474 7164 6d29 01da 044c 6973  N)...tqdm)...Lis
+000001c0: 747a f541 6461 6d20 4d2e 204b 7261 6a65  tz.Adam M. Kraje
+000001d0: 7773 6b69 2c20 4a6f 6e61 7468 616e 2057  wski, Jonathan W
+000001e0: 2e20 5369 6567 656c 2c20 4a69 6e63 6861  . Siegel, Jincha
+000001f0: 6f20 5875 2c20 5a69 2d4b 7569 204c 6975  o Xu, Zi-Kui Liu
+00000200: 2c20 4578 7465 6e73 6962 6c65 2053 7472  , Extensible Str
+00000210: 7563 7475 7265 2d49 6e66 6f72 6d65 6420  ucture-Informed 
+00000220: 5072 6564 6963 7469 6f6e 206f 6620 466f  Prediction of Fo
+00000230: 726d 6174 696f 6e20 456e 6572 6779 2077  rmation Energy w
+00000240: 6974 6820 696d 7072 6f76 6564 2061 6363  ith improved acc
+00000250: 7572 6163 7920 616e 6420 7573 6162 696c  uracy and usabil
+00000260: 6974 7920 656d 706c 6f79 696e 6720 6e65  ity employing ne
+00000270: 7572 616c 206e 6574 776f 726b 732c 2043  ural networks, C
+00000280: 6f6d 7075 7461 7469 6f6e 616c 204d 6174  omputational Mat
+00000290: 6572 6961 6c73 2053 6369 656e 6365 2c20  erials Science, 
+000002a0: 566f 6c75 6d65 2032 3038 2c20 3230 3232  Volume 208, 2022
+000002b0: 2c20 3131 3132 3534 75f9 0000 004c 2e20  , 111254u....L. 
+000002c0: 5761 7264 2c20 522e 204c 6975 2c20 412e  Ward, R. Liu, A.
+000002d0: 204b 7269 7368 6e61 2c20 562e 2049 2e20   Krishna, V. I. 
+000002e0: 4865 6764 652c 2041 2e20 4167 7261 7761  Hegde, A. Agrawa
+000002f0: 6c2c 2041 2e20 4368 6f75 6468 6172 792c  l, A. Choudhary,
+00000300: 2061 6e64 2043 2e20 576f 6c76 6572 746f   and C. Wolverto
+00000310: 6e2c 20e2 809c 496e 636c 7564 696e 6720  n, ...Including 
+00000320: 6372 7973 7461 6c20 7374 7275 6374 7572  crystal structur
+00000330: 6520 6174 7472 6962 7574 6573 2069 6e20  e attributes in 
+00000340: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
+00000350: 206d 6f64 656c 7320 6f66 2066 6f72 6d61   models of forma
+00000360: 7469 6f6e 2065 6e65 7267 6965 7320 7669  tion energies vi
+00000370: 6120 566f 726f 6e6f 6920 7465 7373 656c  a Voronoi tessel
+00000380: 6c61 7469 6f6e 732c e280 9d20 5068 7973  lations,... Phys
+00000390: 6963 616c 2052 6576 6965 7720 422c 2076  ical Review B, v
+000003a0: 6f6c 2e20 3936 2c20 6e6f 2e20 322c 2037  ol. 96, no. 2, 7
+000003b0: 2032 3031 372e e970 0000 007a 1d4d 6167   2017..p...z.Mag
+000003c0: 7069 655f 656c 656d 656e 745f 7072 6f70  pie_element_prop
+000003d0: 6572 7469 6573 2e63 7376 fa01 2c29 01da  erties.csv..,)..
+000003e0: 0964 656c 696d 6974 6572 2916 e92d 0000  .delimiter)..-..
+000003f0: 00e9 2100 0000 e902 0000 00e9 2000 0000  ..!......... ...
+00000400: e905 0000 00e9 3000 0000 e906 0000 00e9  ......0.........
+00000410: 0a00 0000 e92c 0000 00e9 2a00 0000 e926  .....,....*....&
+00000420: 0000 00e9 2800 0000 e924 0000 00e9 2b00  ....(....$....+.
+00000430: 0000 e929 0000 00e9 2500 0000 e927 0000  ...)....%....'..
+00000440: 00e9 2300 0000 e912 0000 00e9 0d00 0000  ..#.............
+00000450: e911 0000 00e9 3200 0000 2901 da06 7265  ......2...)...re
+00000460: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
+00000470: 001c 0000 0008 0000 0043 0000 0073 9202  .........C...s..
+00000480: 0000 7400 a001 7402 6a03 6401 1900 a101  ..t...t.j.d.....
+00000490: 7d03 7c01 6a04 a005 a100 a006 a100 4400  }.|.j.........D.
+000004a0: 5d2a 5c02 7d04 7d05 7c03 7c05 7402 7407  ]*\.}.}.|.|.t.t.
+000004b0: 7c04 8301 6a08 6401 1800 6402 6402 8502  |...j.d...d.d...
+000004c0: 6602 1900 1400 3700 7d03 711e 7400 a001  f.....7.}.q.t...
+000004d0: 7402 6a03 6401 1900 a101 7d06 6403 7d07  t.j.d.....}.d.}.
+000004e0: 6403 7d08 6404 6405 8400 7c00 a009 a100  d.}.d.d...|.....
+000004f0: 4400 8301 7d09 7c00 a006 a100 4400 5d88  D...}.|.....D.].
+00000500: 5c02 7d0a 7d0b 7400 a001 7402 6a03 6401  \.}.}.t...t.j.d.
+00000510: 1900 a101 7d0c 7c0b 6406 1900 6a04 a005  ....}.|.d...j...
+00000520: a100 a006 a100 4400 5d2a 5c02 7d04 7d05  ......D.]*\.}.}.
+00000530: 7c0c 7c05 7402 7407 7c04 8301 6a08 6401  |.|.t.t.|...j.d.
+00000540: 1800 6402 6402 8502 6602 1900 1400 3700  ..d.d...f.....7.
+00000550: 7d0c 71a6 7c06 7400 a00a 7c03 7c0c 1800  }.q.|.t...|.|...
+00000560: a101 7c0b 6407 1900 1400 3700 7d06 7c07  ..|.d.....7.}.|.
+00000570: 7c0b 6407 1900 3700 7d07 7c08 7c0b 6408  |.d...7.}.|.|.d.
+00000580: 1900 3700 7d08 717c 7c06 7c07 1b00 7c03  ..7.}.q||.|...|.
+00000590: 6702 7d0d 6403 7d0e 6403 7d0f 7c00 a009  g.}.d.}.d.}.|...
+000005a0: a100 4400 5d26 7d0b 7c0e 7c0b 6407 1900  ..D.]&}.|.|.d...
+000005b0: 3700 7d0e 7c0f 7c0b 6407 1900 7c0b 6407  7.}.|.|.d...|.d.
+000005c0: 1900 1400 3700 7d0f 9001 7122 7c0e 7c0e  ....7.}...q"|.|.
+000005d0: 1400 7c0f 1b00 7d10 6403 7d11 7c00 a009  ..|...}.d.}.|...
+000005e0: a100 4400 5d1e 7d0b 7c11 7c0b 6407 1900  ..D.].}.|.|.d...
+000005f0: 6409 1400 7c0b 640a 1900 1400 3700 7d11  d...|.d.....7.}.
+00000600: 9001 7162 7c11 7c07 1d00 7d11 6403 7d12  ..qb|.|...}.d.}.
+00000610: 7c00 a009 a100 4400 5d26 7d0b 7c12 7c0b  |.....D.]&}.|.|.
+00000620: 6407 1900 740a 6409 7c0b 640a 1900 1400  d...t.d.|.d.....
+00000630: 7c11 1800 8301 1400 3700 7d12 9001 7196  |.......7.}...q.
+00000640: 7c12 7c07 7c11 1400 1d00 7d12 6900 7d13  |.|.|.....}.i.}.
+00000650: 6403 7d14 6900 7d15 6403 7d16 6900 7d17  d.}.i.}.d.}.i.}.
+00000660: 6403 7d18 7c00 a009 a100 4400 5d54 7d19  d.}.|.....D.]T}.
+00000670: 7c14 7c19 6407 1900 3700 7d14 7c0b 6406  |.|.d...7.}.|.d.
+00000680: 1900 6a04 a005 a100 4400 5d32 7d04 7c04  ..j.....D.]2}.|.
+00000690: 7c13 7600 9002 722c 7c13 7c04 0500 1900  |.v...r,|.|.....
+000006a0: 7c19 6407 1900 3700 0300 3c00 6e0c 7c19  |.d...7...<.n.|.
+000006b0: 6407 1900 7c13 7c04 3c00 9002 7108 9001  d...|.|.<...q...
+000006c0: 71ea 740b 640b 640c 8400 7c00 a009 a100  q.t.d.d...|.....
+000006d0: 4400 8301 8301 7d1a 640d 740c 6a0d 1400  D.....}.d.t.j...
+000006e0: 740c a00e 7c1a 640e a102 1400 7d1b 7400  t...|.d.....}.t.
+000006f0: a00f 7c10 7c11 7c12 7c08 7c1b 6705 7c0d  ..|.|.|.|.|.g.|.
+00000700: 6403 1900 6602 a101 7c0d 6401 1900 7c09  d...f...|.d...|.
+00000710: 6703 5300 290f 618e 0100 0041 2070 726f  g.S.).a....A pro
+00000720: 746f 7479 7065 2066 756e 6374 696f 6e20  totype function 
+00000730: 7768 6963 6820 636f 6d70 7574 6573 2061  which computes a
+00000740: 2077 6569 6768 7465 6420 6176 6572 6167   weighted averag
+00000750: 6520 6f76 6572 206e 6569 6768 626f 7273  e over neighbors
+00000760: 2c20 7765 6967 6874 6564 2062 7920 7468  , weighted by th
+00000770: 6520 6172 6561 206f 6620 7468 6520 766f  e area of the vo
+00000780: 726f 6e6f 6920 6365 6c6c 0a20 2020 2062  ronoi cell.    b
+00000790: 6574 7765 656e 2074 6865 6d2e 0a0a 2020  etween them...  
+000007a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000007b0: 6c6f 6361 6c5f 656e 763a 2041 2064 6963  local_env: A dic
+000007c0: 7469 6f6e 6172 7920 6f66 2074 6865 206c  tionary of the l
+000007d0: 6f63 616c 2065 6e76 6972 6f6e 6d65 6e74  ocal environment
+000007e0: 206f 6620 6120 7369 7465 2c20 6173 2072   of a site, as r
+000007f0: 6574 7572 6e65 6420 6279 2061 2056 6f72  eturned by a Vor
+00000800: 6f6e 6f69 4e4e 2067 656e 6572 6174 6f72  onoiNN generator
+00000810: 2e0a 2020 2020 2020 2020 7369 7465 3a20  ..        site: 
+00000820: 5468 6520 7369 7465 206e 756d 6265 7220  The site number 
+00000830: 666f 7220 7768 6963 6820 7468 6520 6c6f  for which the lo
+00000840: 6361 6c20 656e 7669 726f 6e6d 656e 7420  cal environment 
+00000850: 6973 2062 6569 6e67 2063 6f6d 7075 7465  is being compute
+00000860: 642e 0a0a 2020 2020 5265 7475 726e 733a  d...    Returns:
+00000870: 0a20 2020 2020 2020 2041 206c 6973 7420  .        A list 
+00000880: 6f66 2074 6865 206c 6f63 616c 2065 6e76  of the local env
+00000890: 6972 6f6e 6d65 6e74 2061 7474 7269 6275  ironment attribu
+000008a0: 7465 732e 0a20 2020 20e9 0100 0000 4e72  tes..    .....Nr
+000008b0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
+000008c0: 0002 0000 0005 0000 0053 0000 0073 1c00  .........S...s..
+000008d0: 0000 6700 7c00 5d14 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+000008e0: 7c01 6401 1900 6702 9102 7104 5300 2902  |.d...g...q.S.).
+000008f0: da04 7369 7465 da04 6172 6561 a900 a902  ..site..area....
+00000900: da02 2e30 da05 7661 6c75 6572 2400 0000  ...0..valuer$...
+00000910: 7224 0000 00fa 512f 5573 6572 732f 6164  r$....Q/Users/ad
+00000920: 616d 2f50 7963 6861 726d 5072 6f6a 6563  am/PycharmProjec
+00000930: 7473 2f70 7953 4950 4645 4e4e 2f70 7973  ts/pySIPFENN/pys
+00000940: 6970 6665 6e6e 2f64 6573 6372 6970 746f  ipfenn/descripto
+00000950: 7244 6566 696e 6974 696f 6e73 2f57 6172  rDefinitions/War
+00000960: 6432 3031 372e 7079 da0a 3c6c 6973 7463  d2017.py..<listc
+00000970: 6f6d 703e 3400 0000 f300 0000 007a 266c  omp>4........z&l
+00000980: 6f63 616c 5f65 6e76 5f66 756e 6374 696f  ocal_env_functio
+00000990: 6e2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  n.<locals>.<list
+000009a0: 636f 6d70 3e72 2200 0000 7223 0000 00da  comp>r"...r#....
+000009b0: 0676 6f6c 756d 6572 0c00 0000 da09 6661  .volumer......fa
+000009c0: 6365 5f64 6973 7463 0100 0000 0000 0000  ce_distc........
+000009d0: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
+000009e0: 7316 0000 007c 005d 0e7d 017c 0164 0019  s....|.].}.|.d..
+000009f0: 0056 0001 0071 0264 0153 0029 0272 2c00  .V...q.d.S.).r,.
+00000a00: 0000 4e72 2400 0000 2902 7226 0000 00da  ..Nr$...).r&....
+00000a10: 0d6e 6569 6768 626f 725f 7369 7465 7224  .neighbor_siter$
+00000a20: 0000 0072 2400 0000 7228 0000 00da 093c  ...r$...r(.....<
+00000a30: 6765 6e65 7870 723e 5c00 0000 722a 0000  genexpr>\...r*..
+00000a40: 007a 256c 6f63 616c 5f65 6e76 5f66 756e  .z%local_env_fun
+00000a50: 6374 696f 6e2e 3c6c 6f63 616c 733e 2e3c  ction.<locals>.<
+00000a60: 6765 6e65 7870 723e 6755 5555 5555 55f5  genexpr>gUUUUUU.
+00000a70: 3f67 0000 0000 0000 0840 2910 da02 6e70  ?g.......@)...np
+00000a80: da05 7a65 726f 73da 1061 7474 7269 6275  ..zeros..attribu
+00000a90: 7465 5f6d 6174 7269 78da 0573 6861 7065  te_matrix..shape
+00000aa0: da07 7370 6563 6965 73da 0f67 6574 5f65  ..species..get_e
+00000ab0: 6c5f 616d 745f 6469 6374 da05 6974 656d  l_amt_dict..item
+00000ac0: 7372 0300 0000 da01 5ada 0676 616c 7565  sr......Z..value
+00000ad0: 73da 0361 6273 da03 6d69 6eda 046d 6174  s..abs..min..mat
+00000ae0: 68da 0270 69da 0370 6f77 da0b 636f 6e63  h..pi..pow..conc
+00000af0: 6174 656e 6174 6529 1cda 096c 6f63 616c  atenate)...local
+00000b00: 5f65 6e76 7222 0000 00da 0c65 6c65 6d65  _envr".....eleme
+00000b10: 6e74 5f64 6963 745a 106c 6f63 616c 5f61  nt_dictZ.local_a
+00000b20: 7474 7269 6275 7465 73da 036b 6579 7227  ttributes..keyr'
+00000b30: 0000 005a 0f64 6966 665f 6174 7472 6962  ...Z.diff_attrib
+00000b40: 7574 6573 da0c 746f 7461 6c5f 7765 6967  utes..total_weig
+00000b50: 6874 722b 0000 005a 0d6e 6569 6768 626f  htr+...Z.neighbo
+00000b60: 725f 6c69 7374 da03 696e 6472 2d00 0000  r_list..indr-...
+00000b70: 5a13 6e65 6967 6862 6f72 5f61 7474 7269  Z.neighbor_attri
+00000b80: 6275 7465 735a 1f65 6c65 6d65 6e74 616c  butesZ.elemental
+00000b90: 5f70 726f 7065 7274 6965 735f 6174 7472  _properties_attr
+00000ba0: 6962 7574 6573 da07 6176 6572 6167 65da  ibutes..average.
+00000bb0: 0876 6172 6961 6e63 655a 0d65 6666 5f63  .varianceZ.eff_c
+00000bc0: 6f6f 7264 5f6e 756d 5a0c 626c 656e 5f61  oord_numZ.blen_a
+00000bd0: 7665 7261 6765 5a08 626c 656e 5f76 6172  verageZ.blen_var
+00000be0: 5a0b 7061 7468 5f64 6963 745f 315a 0e74  Z.path_dict_1Z.t
+00000bf0: 6f74 616c 5f77 6569 6768 745f 315a 0b70  otal_weight_1Z.p
+00000c00: 6174 685f 6469 6374 5f32 5a0e 746f 7461  ath_dict_2Z.tota
+00000c10: 6c5f 7765 6967 6874 5f32 5a0b 7061 7468  l_weight_2Z.path
+00000c20: 5f64 6963 745f 335a 0e74 6f74 616c 5f77  _dict_3Z.total_w
+00000c30: 6569 6768 745f 335a 0f6e 6569 6768 626f  eight_3Z.neighbo
+00000c40: 725f 7369 7465 5f31 5a0a 7370 6865 7265  r_site_1Z.sphere
+00000c50: 5f72 6164 5a0d 7370 6865 7265 5f76 6f6c  _radZ.sphere_vol
+00000c60: 756d 6572 2400 0000 7224 0000 0072 2800  umer$...r$...r(.
+00000c70: 0000 da12 6c6f 6361 6c5f 656e 765f 6675  ....local_env_fu
+00000c80: 6e63 7469 6f6e 2200 0000 7360 0000 0000  nction"...s`....
+00000c90: 0c10 0116 0124 0110 0104 0104 0112 0110  .....$..........
+00000ca0: 0110 011a 0124 011a 010c 010e 010c 0204  .....$..........
+00000cb0: 0104 010c 010c 0118 010c 0204 010c 011c  ................
+00000cc0: 0108 0104 010c 0124 010c 0204 0104 0104  .......$........
+00000cd0: 0104 0104 0104 010c 010c 0112 010a 0116  ................
+00000ce0: 0214 0216 0116 0104 0114 ff02 0208 fe72  ...............r
+00000cf0: 4500 0000 6300 0000 0000 0000 0000 0000  E...c...........
+00000d00: 0000 0000 0004 0000 0040 0000 0073 3200  .........@...s2.
+00000d10: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
+00000d20: 6402 6402 6403 8d02 6601 6404 6405 8401  d.d.d...f.d.d...
+00000d30: 5a05 6506 6406 9c01 6407 6408 8404 5a07  Z.e.d...d.d...Z.
+00000d40: 6409 5300 290a da17 4c6f 6361 6c41 7474  d.S.)...LocalAtt
+00000d50: 7269 6275 7465 4765 6e65 7261 746f 727a  ributeGeneratorz
+00000d60: b141 2077 7261 7070 6572 2063 6c61 7373  .A wrapper class
+00000d70: 2077 6869 6368 2063 6f6e 7461 696e 7320   which contains 
+00000d80: 616e 2069 6e73 7461 6e63 6520 6f66 2061  an instance of a
+00000d90: 6e20 4e4e 2067 656e 6572 6174 6f72 2028  n NN generator (
+00000da0: 7468 6520 6465 6661 756c 7420 6973 2061  the default is a
+00000db0: 2056 6f72 6f6e 6f69 4e4e 292c 2061 2073   VoronoiNN), a s
+00000dc0: 7472 7563 7475 7265 2c20 616e 640a 2020  tructure, and.  
+00000dd0: 2020 6120 6675 6e63 7469 6f6e 2077 6869    a function whi
+00000de0: 6368 2063 6f6d 7075 7465 7320 7468 6520  ch computes the 
+00000df0: 6c6f 6361 6c20 656e 7669 726f 6e6d 656e  local environmen
+00000e00: 7420 6174 7472 6962 7574 6573 2e0a 2020  t attributes..  
+00000e10: 2020 4629 025a 1563 6f6d 7075 7465 5f61    F).Z.compute_a
+00000e20: 646a 5f6e 6569 6768 626f 7273 5a0d 6578  dj_neighborsZ.ex
+00000e30: 7472 615f 6e6e 5f69 6e66 6f63 0500 0000  tra_nn_infoc....
+00000e40: 0000 0000 0000 0000 0500 0000 0200 0000  ................
+00000e50: 4300 0000 731c 0000 007c 047c 005f 007c  C...s....|.|._.|
+00000e60: 017c 005f 017c 027c 005f 027c 037c 005f  .|._.|.|._.|.|._
+00000e70: 0364 0053 00a9 014e 2904 da09 6765 6e65  .d.S...N)...gene
+00000e80: 7261 746f 72da 0673 7472 7563 74da 0866  rator..struct..f
+00000e90: 756e 6374 696f 6e72 3f00 0000 2905 da04  unctionr?...)...
+00000ea0: 7365 6c66 7249 0000 005a 0e6c 6f63 616c  selfrI...Z.local
+00000eb0: 5f65 6e76 5f66 756e 6372 3f00 0000 5a0c  _env_funcr?...Z.
+00000ec0: 6e6e 5f67 656e 6572 6174 6f72 7224 0000  nn_generatorr$..
+00000ed0: 0072 2400 0000 7228 0000 00da 085f 5f69  .r$...r(.....__i
+00000ee0: 6e69 745f 5f68 0000 0073 0800 0000 0002  nit__h...s......
+00000ef0: 0601 0601 0601 7a20 4c6f 6361 6c41 7474  ......z LocalAtt
+00000f00: 7269 6275 7465 4765 6e65 7261 746f 722e  ributeGenerator.
+00000f10: 5f5f 696e 6974 5f5f 2901 da01 6e63 0200  __init__)...nc..
+00000f20: 0000 0000 0000 0000 0000 0300 0000 0500  ................
+00000f30: 0000 4300 0000 7326 0000 007c 006a 00a0  ..C...s&...|.j..
+00000f40: 017c 006a 027c 01a1 027d 027c 00a0 037c  .|.j.|...}.|...|
+00000f50: 027c 006a 027c 0119 007c 006a 04a1 0353  .|.j.|...|.j...S
+00000f60: 0029 017a 4d47 656e 6572 6174 6573 2074  .).zMGenerates t
+00000f70: 6865 206c 6f63 616c 2065 6e76 6972 6f6e  he local environ
+00000f80: 6d65 6e74 2061 7474 7269 6275 7465 7320  ment attributes 
+00000f90: 666f 7220 6120 6769 7665 6e20 7369 7465  for a given site
+00000fa0: 2069 6e20 7468 6520 7374 7275 6374 7572   in the structur
+00000fb0: 652e 2905 7248 0000 005a 1567 6574 5f76  e.).rH...Z.get_v
+00000fc0: 6f72 6f6e 6f69 5f70 6f6c 7968 6564 7261  oronoi_polyhedra
+00000fd0: 7249 0000 0072 4a00 0000 723f 0000 0029  rI...rJ...r?...)
+00000fe0: 0372 4b00 0000 724d 0000 0072 3e00 0000  .rK...rM...r>...
+00000ff0: 7224 0000 0072 2400 0000 7228 0000 00da  r$...r$...r(....
+00001000: 1967 656e 6572 6174 655f 6c6f 6361 6c5f  .generate_local_
+00001010: 6174 7472 6962 7574 6573 6f00 0000 7304  attributeso...s.
+00001020: 0000 0000 0210 017a 314c 6f63 616c 4174  .......z1LocalAt
+00001030: 7472 6962 7574 6547 656e 6572 6174 6f72  tributeGenerator
+00001040: 2e67 656e 6572 6174 655f 6c6f 6361 6c5f  .generate_local_
+00001050: 6174 7472 6962 7574 6573 4e29 08da 085f  attributesN)..._
+00001060: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00001070: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00001080: 5fda 075f 5f64 6f63 5f5f 7204 0000 0072  _..__doc__r....r
+00001090: 4c00 0000 da03 696e 7472 4e00 0000 7224  L.....intrN...r$
+000010a0: 0000 0072 2400 0000 7224 0000 0072 2800  ...r$...r$...r(.
+000010b0: 0000 7246 0000 0063 0000 0073 0800 0000  ..rF...c...s....
+000010c0: 0801 0405 0aff 0a07 7246 0000 0029 0172  ........rF...).r
+000010d0: 4900 0000 6302 0000 0000 0000 0000 0000  I...c...........
+000010e0: 0008 0000 0008 0000 0043 0000 0073 be00  .........C...s..
+000010f0: 0000 6900 7d02 7c00 6a00 4400 5d50 7d03  ..i.}.|.j.D.]P}.
+00001100: 7c03 a001 a100 a002 a100 4400 5d3e 5c02  |.........D.]>\.
+00001110: 7d04 7d05 7c04 7c02 7600 7246 7c02 7c04  }.}.|.|.v.rF|.|.
+00001120: 0500 1900 7c05 7403 7c00 6a00 8301 1b00  ....|.t.|.j.....
+00001130: 3700 0300 3c00 711a 7c05 7403 7c00 6a00  7...<.q.|.t.|.j.
+00001140: 8301 1b00 7c02 7c04 3c00 711a 710a 7404  ....|.|.<.q.q.t.
+00001150: 7c00 7c01 7c02 8303 7d06 7405 7c06 6a06  |.|.|...}.t.|.j.
+00001160: 7407 7403 7c00 6a08 8301 8301 8302 7d07  t.t.|.j.......}.
+00001170: 7409 7c07 8301 7d07 740a a00b 6401 6402  t.|...}.t...d.d.
+00001180: 8400 7c07 4400 8301 a101 740a a00b 6403  ..|.D.....t...d.
+00001190: 6402 8400 7c07 4400 8301 a101 6404 6405  d...|.D.....d.d.
+000011a0: 8400 740c 7c07 8301 4400 8301 6603 5300  ..t.|...D...f.S.
+000011b0: 2906 616c 0100 0047 656e 6572 6174 6573  ).al...Generates
+000011c0: 2074 6865 206c 6f63 616c 2065 6e76 6972   the local envir
+000011d0: 6f6e 6d65 6e74 2061 7474 7269 6275 7465  onment attribute
+000011e0: 7320 666f 7220 6120 6769 7665 6e20 7374  s for a given st
+000011f0: 7275 6374 7572 6520 7573 696e 6720 6120  ructure using a 
+00001200: 566f 726f 6e6f 694e 4e20 6765 6e65 7261  VoronoiNN genera
+00001210: 746f 722e 200a 2020 2020 2020 2054 6865  tor. .       The
+00001220: 206c 6f63 616c 2065 6e76 6972 6f6e 6d65   local environme
+00001230: 6e74 2061 7474 7269 6275 7465 7320 636f  nt attributes co
+00001240: 6e73 6973 7420 6f66 2061 7665 7261 6765  nsist of average
+00001250: 7320 6f76 6572 2074 6865 206e 6569 6768  s over the neigh
+00001260: 626f 7273 206f 6620 6561 6368 2073 6974  bors of each sit
+00001270: 6520 696e 2074 6865 2073 7472 7563 7475  e in the structu
+00001280: 7265 2e0a 0a20 2020 2041 7267 733a 0a20  re...    Args:. 
+00001290: 2020 2020 2020 2073 7472 7563 743a 2041         struct: A
+000012a0: 2070 796d 6174 6765 6e20 5374 7275 6374   pymatgen Struct
+000012b0: 7572 6520 6f62 6a65 6374 2e0a 2020 2020  ure object..    
+000012c0: 2020 2020 6c6f 6361 6c5f 6675 6e63 743a      local_funct:
+000012d0: 2041 2066 756e 6374 696f 6e20 7768 6963   A function whic
+000012e0: 6820 636f 6d70 7574 6573 2074 6865 206c  h computes the l
+000012f0: 6f63 616c 2065 6e76 6972 6f6e 6d65 6e74  ocal environment
+00001300: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
+00001310: 6120 6769 7665 6e20 7369 7465 2e0a 0a20  a given site... 
+00001320: 2020 2063 0100 0000 0000 0000 0000 0000     c............
+00001330: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
+00001340: 0067 007c 005d 0c7d 017c 0164 0019 0091  .g.|.].}.|.d....
+00001350: 0271 0453 0029 0172 0100 0000 7224 0000  .q.S.).r....r$..
+00001360: 0072 2500 0000 7224 0000 0072 2400 0000  .r%...r$...r$...
+00001370: 7228 0000 0072 2900 0000 8900 0000 722a  r(...r).......r*
+00001380: 0000 007a 2f67 656e 6572 6174 655f 766f  ...z/generate_vo
+00001390: 726f 6e6f 695f 6174 7472 6962 7574 6573  ronoi_attributes
+000013a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+000013b0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
+000013c0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
+000013d0: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
+000013e0: 9102 7104 5300 2901 7221 0000 0072 2400  ..q.S.).r!...r$.
+000013f0: 0000 7225 0000 0072 2400 0000 7224 0000  ..r%...r$...r$..
+00001400: 0072 2800 0000 7229 0000 0089 0000 0072  .r(...r).......r
+00001410: 2a00 0000 6301 0000 0000 0000 0000 0000  *...c...........
+00001420: 0003 0000 0005 0000 0053 0000 0073 1a00  .........S...s..
+00001430: 0000 6900 7c00 5d12 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
+00001440: 7c02 6400 1900 9302 7104 5300 2901 720c  |.d.....q.S.).r.
+00001450: 0000 0072 2400 0000 2903 7226 0000 00da  ...r$...).r&....
+00001460: 0169 7227 0000 0072 2400 0000 7224 0000  .ir'...r$...r$..
+00001470: 0072 2800 0000 da0a 3c64 6963 7463 6f6d  .r(.....<dictcom
+00001480: 703e 8900 0000 7302 0000 0006 017a 2f67  p>....s......z/g
+00001490: 656e 6572 6174 655f 766f 726f 6e6f 695f  enerate_voronoi_
+000014a0: 6174 7472 6962 7574 6573 2e3c 6c6f 6361  attributes.<loca
+000014b0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 290d  ls>.<dictcomp>).
+000014c0: da10 7370 6563 6965 735f 616e 645f 6f63  ..species_and_oc
+000014d0: 6375 7234 0000 0072 3500 0000 da03 6c65  cur4...r5.....le
+000014e0: 6e72 4600 0000 da03 6d61 7072 4e00 0000  nrF.....maprN...
+000014f0: da05 7261 6e67 65da 0573 6974 6573 da04  ..range..sites..
+00001500: 6c69 7374 722f 0000 00da 0561 7272 6179  listr/.....array
+00001510: da09 656e 756d 6572 6174 6529 0872 4900  ..enumerate).rI.
+00001520: 0000 5a0b 6c6f 6361 6c5f 6675 6e63 7472  ..Z.local_functr
+00001530: 3f00 0000 da0b 636f 6d70 6f73 6974 696f  ?.....compositio
+00001540: 6e72 4000 0000 7227 0000 005a 0f6c 6f63  nr@...r'...Z.loc
+00001550: 616c 5f67 656e 6572 6174 6f72 5a0e 6174  al_generatorZ.at
+00001560: 7472 6962 7574 655f 6c69 7374 7224 0000  tribute_listr$..
+00001570: 0072 2400 0000 7228 0000 00da 1b67 656e  .r$...r(.....gen
+00001580: 6572 6174 655f 766f 726f 6e6f 695f 6174  erate_voronoi_at
+00001590: 7472 6962 7574 6573 7500 0000 7318 0000  tributesu...s...
+000015a0: 0000 0a04 010a 0114 0108 011c 0216 010c  ................
+000015b0: 0116 0108 012a 0106 ff72 5f00 0000 2902  .....*...r_...).
+000015c0: da04 7374 7263 7220 0000 0063 0300 0000  ..strcr ...c....
+000015d0: 0000 0000 0000 0000 1700 0000 0b00 0000  ................
+000015e0: 0300 0000 7390 0200 0074 007c 006a 0183  ....s....t.|.j..
+000015f0: 0164 016b 0272 1864 0267 017c 0214 0053  .d.k.r.d.g.|...S
+00001600: 0067 0089 007c 0044 005d 127d 0388 00a0  .g...|.D.].}....
+00001610: 027c 03a0 03a1 00a1 0101 0071 2087 0066  .|.........q ..f
+00001620: 0164 0364 0484 087c 01a0 04a1 0044 0083  .d.d...|.....D..
+00001630: 017d 0474 057c 006a 016a 066a 07a0 04a1  .}.t.|.j.j.j....
+00001640: 008e 005c 027d 057d 0667 007d 0764 0564  ...\.}.}.g.}.d.d
+00001650: 0484 0074 0874 007c 0083 0183 0144 0083  ...t.t.|.....D..
+00001660: 017d 0874 087c 0283 0144 0090 025d 067d  .}.t.|...D...].}
+00001670: 0974 09a0 0a74 007c 0083 0174 007c 0583  .t...t.|...t.|..
+00001680: 0166 02a1 017d 0a74 0874 007c 0083 0183  .f...}.t.t.|....
+00001690: 0144 0090 015d c87d 0b7c 087c 0b19 007d  .D...].}.|.|...}
+000016a0: 0c69 007c 087c 0b3c 007c 0ca0 04a1 0044  .i.|.|.<.|.....D
+000016b0: 0090 015d 7e5c 027d 0d7d 0e7c 0d64 0219  ...]~\.}.}.|.d..
+000016c0: 007d 0f7c 0d64 0119 007d 107c 0d64 0619  .}.|.d...}.|.d..
+000016d0: 007d 1164 027d 1264 077d 137c 047c 1019  .}.d.}.d.}.|.|..
+000016e0: 0044 005d 407d 147c 1464 0219 007c 0f6b  .D.]@}.|.d...|.k
+000016f0: 0390 0173 2874 0b7c 1464 0119 007c 1118  ...s(t.|.d...|..
+00001700: 0083 0164 086b 0490 0173 287c 1390 0172  ...d.k...s(|...r
+00001710: 367c 127c 1464 0119 0037 007d 1271 fa64  6|.|.d...7.}.q.d
+00001720: 097d 1371 fa64 077d 137c 047c 1019 0044  .}.q.d.}.|.|...D
+00001730: 005d fe7d 147c 1464 0219 007c 0f6b 0390  .].}.|.d...|.k..
+00001740: 0173 7674 0b7c 1464 0119 007c 1118 0083  .svt.|.d...|....
+00001750: 0164 086b 0490 0173 767c 1390 0272 407c  .d.k...sv|...r@|
+00001760: 007c 1464 0219 0019 006a 0ca0 04a1 0044  .|.d.....j.....D
+00001770: 005d 345c 027d 157d 167c 0a7c 0b7c 05a0  .]4\.}.}.|.|.|..
+00001780: 0d7c 15a1 0166 0205 0019 007c 167c 1464  .|...f.....|.|.d
+00001790: 0119 0014 007c 0e14 007c 121b 0037 0003  .....|...|...7..
+000017a0: 003c 0090 0171 887c 097c 0264 0118 006b  .<...q.|.|.d...k
+000017b0: 0090 0272 447c 107c 1464 0219 007c 1464  ...rD|.|.d...|.d
+000017c0: 0119 0066 037c 087c 0b19 0076 0090 0272  ...f.|.|...v...r
+000017d0: 187c 087c 0b19 007c 107c 1464 0219 007c  .|.|...|.|.d...|
+000017e0: 1464 0119 0066 0305 0019 007c 1464 0119  .d...f.....|.d..
+000017f0: 007c 0e14 007c 121b 0037 0003 003c 006e  .|...|...7...<.n
+00001800: 267c 1464 0119 007c 0e14 007c 121b 007c  &|.d...|...|...|
+00001810: 087c 0b19 007c 107c 1464 0219 007c 1464  .|...|.|.d...|.d
+00001820: 0119 0066 033c 006e 0464 097d 1390 0171  ...f.<.n.d.}...q
+00001830: 4871 c864 017c 0a7c 0b64 0a64 0a85 0266  Hq.d.|.|.d.d...f
+00001840: 0219 0074 09a0 0e7c 06a1 011b 0018 007c  ...t...|.......|
+00001850: 0a7c 0b64 0a64 0a85 0266 023c 0071 aa7c  .|.d.d...f.<.q.|
+00001860: 07a0 0274 09a0 0b7c 0aa1 01a0 0fa1 00a1  ...t...|........
+00001870: 0101 0071 827c 0753 0029 0b61 c001 0000  ...q.|.S.).a....
+00001880: 4765 6e65 7261 7465 7320 7468 6520 5743  Generates the WC
+00001890: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
+000018a0: 6120 6769 7665 6e20 7374 7275 6374 7572  a given structur
+000018b0: 652e 2054 6865 2057 4320 6174 7472 6962  e. The WC attrib
+000018c0: 7574 6573 2061 7265 2074 6865 206f 7264  utes are the ord
+000018d0: 6572 696e 6720 7061 7261 6d65 7465 7273  ering parameters
+000018e0: 2066 6f72 2065 6163 680a 2020 2020 7368   for each.    sh
+000018f0: 656c 6c20 6f66 2074 6865 2056 6f72 6f6e  ell of the Voron
+00001900: 6f69 2074 6573 7365 6c6c 6174 696f 6e2e  oi tessellation.
+00001910: 2053 6c69 6768 746c 7920 6469 6666 6572   Slightly differ
+00001920: 656e 7420 7468 616e 2077 6861 7420 6973  ent than what is
+00001930: 2069 6d70 6c65 6d65 6e74 6564 2062 7920   implemented by 
+00001940: 5761 7264 2d57 6f6c 7665 7274 6f6e 2e20  Ward-Wolverton. 
+00001950: 4f6e 6c79 2063 6f6e 7369 6465 7273 0a20  Only considers. 
+00001960: 2020 2069 6d6d 6564 6961 7465 2062 6163     immediate bac
+00001970: 6b74 7261 636b 696e 672e 0a0a 2020 2020  ktracking...    
+00001980: 4172 6773 3a0a 2020 2020 2020 2020 7374  Args:.        st
+00001990: 7263 3a20 4120 7079 6d61 7467 656e 2053  rc: A pymatgen S
+000019a0: 7472 7563 7475 7265 206f 626a 6563 742e  tructure object.
+000019b0: 0a20 2020 2020 2020 206e 6569 6768 626f  .        neighbo
+000019c0: 725f 6469 6374 5f72 6177 3a20 4120 6469  r_dict_raw: A di
+000019d0: 6374 696f 6e61 7279 206f 6620 7468 6520  ctionary of the 
+000019e0: 6e65 6967 6862 6f72 7320 6f66 2065 6163  neighbors of eac
+000019f0: 6820 7369 7465 2069 6e20 7468 6520 7374  h site in the st
+00001a00: 7275 6374 7572 652e 0a20 2020 2020 2020  ructure..       
+00001a10: 206c 6576 656c 733a 2054 6865 206e 756d   levels: The num
+00001a20: 6265 7220 6f66 2073 6865 6c6c 7320 746f  ber of shells to
+00001a30: 2063 6f6e 7369 6465 722e 0a0a 2020 2020   consider...    
+00001a40: 7221 0000 0072 0100 0000 6301 0000 0000  r!...r....c.....
+00001a50: 0000 0000 0000 0003 0000 0006 0000 0013  ................
+00001a60: 0000 0073 2400 0000 6900 7c00 5d1c 5c02  ...s$...i.|.].\.
+00001a70: 7d01 7d02 7c01 8700 6601 6400 6401 8408  }.}.|...f.d.d...
+00001a80: 7c02 4400 8301 9302 7104 5300 2902 6301  |.D.....q.S.).c.
+00001a90: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00001aa0: 0000 0013 0000 0073 2600 0000 6700 7c00  .......s&...g.|.
+00001ab0: 5d1e 7d01 8800 a000 7c01 6400 1900 a001  ].}.....|.d.....
+00001ac0: a100 a101 7c01 6401 1900 6702 9102 7104  ....|.d...g...q.
+00001ad0: 5300 2902 7201 0000 0072 2100 0000 2902  S.).r....r!...).
+00001ae0: da05 696e 6465 78da 0c74 6f5f 756e 6974  ..index..to_unit
+00001af0: 5f63 656c 6c72 2500 0000 a901 5a0e 7374  _cellr%.....Z.st
+00001b00: 7263 5f75 6e69 745f 6365 6c6c 7224 0000  rc_unit_cellr$..
+00001b10: 0072 2800 0000 7229 0000 009e 0000 0072  .r(...r).......r
+00001b20: 2a00 0000 7a35 6765 6e65 7261 7465 5f57  *...z5generate_W
+00001b30: 435f 6174 7472 6962 7574 6573 2e3c 6c6f  C_attributes.<lo
+00001b40: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00001b50: 2e3c 6c69 7374 636f 6d70 3e72 2400 0000  .<listcomp>r$...
+00001b60: 2903 7226 0000 0072 4000 0000 5a07 7370  ).r&...r@...Z.sp
+00001b70: 5f6c 6973 7472 6300 0000 7224 0000 0072  _listrc...r$...r
+00001b80: 2800 0000 7255 0000 009e 0000 0073 0400  (...rU.......s..
+00001b90: 0000 0601 06ff 7a2a 6765 6e65 7261 7465  ......z*generate
+00001ba0: 5f57 435f 6174 7472 6962 7574 6573 2e3c  _WC_attributes.<
+00001bb0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00001bc0: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
+00001bd0: 0000 0006 0000 0053 0000 0073 1c00 0000  .......S...s....
+00001be0: 6900 7c00 5d14 7d01 7c01 7c01 7c01 6400  i.|.].}.|.|.|.d.
+00001bf0: 6603 6401 6901 9302 7104 5300 2902 6700  f.d.i...q.S.).g.
+00001c00: 0000 0000 0000 00e7 0000 0000 0000 f03f  ...............?
+00001c10: 7224 0000 0029 0272 2600 0000 7254 0000  r$...).r&...rT..
+00001c20: 0072 2400 0000 7224 0000 0072 2800 0000  .r$...r$...r(...
+00001c30: 7255 0000 00a7 0000 0072 2a00 0000 720c  rU.......r*...r.
+00001c40: 0000 0046 6795 d626 e80b 2e11 3e54 4e29  ...Fg..&....>TN)
+00001c50: 1072 5700 0000 725e 0000 00da 0661 7070  .rW...r^.....app
+00001c60: 656e 6472 6200 0000 7235 0000 00da 037a  endrb...r5.....z
+00001c70: 6970 da13 656c 656d 656e 745f 636f 6d70  ip..element_comp
+00001c80: 6f73 6974 696f 6eda 1666 7261 6374 696f  osition..fractio
+00001c90: 6e61 6c5f 636f 6d70 6f73 6974 696f 6e72  nal_compositionr
+00001ca0: 5900 0000 722f 0000 0072 3000 0000 7238  Y...r/...r0...r8
+00001cb0: 0000 0072 3300 0000 7261 0000 0072 5c00  ...r3...ra...r\.
+00001cc0: 0000 da04 6d65 616e 2917 7260 0000 005a  ....mean).r`...Z
+00001cd0: 116e 6569 6768 626f 725f 6469 6374 5f72  .neighbor_dict_r
+00001ce0: 6177 da06 6c65 7665 6c73 da03 706f 73da  aw..levels..pos.
+00001cf0: 0d6e 6569 6768 626f 725f 6469 6374 da05  .neighbor_dict..
+00001d00: 656c 656d 735a 0566 7261 6373 da06 6f75  elemsZ.fracs..ou
+00001d10: 7470 7574 5a0e 7265 6163 6861 626c 655f  tputZ.reachable_
+00001d20: 696e 6473 da05 7368 656c 6cda 086f 7264  inds..shell..ord
+00001d30: 6572 696e 675a 0873 6974 655f 6964 785a  eringZ.site_idxZ
+00001d40: 0672 5f69 6e64 73da 0469 6478 73da 0677  .r_inds..idxs..w
+00001d50: 6569 6768 74da 0570 5f69 6478 da03 6964  eight..p_idx..id
+00001d60: 785a 0966 6163 655f 6172 6561 5a14 7765  xZ.face_areaZ.we
+00001d70: 6967 6874 5f6e 6f72 6d61 6c69 7a61 7469  ight_normalizati
+00001d80: 6f6e da07 736b 6970 7065 64da 056e 5f69  on..skipped..n_i
+00001d90: 6478 7240 0000 0072 2700 0000 7224 0000  dxr@...r'...r$..
+00001da0: 0072 6300 0000 7228 0000 00da 1667 656e  .rc...r(.....gen
+00001db0: 6572 6174 655f 5743 5f61 7474 7269 6275  erate_WC_attribu
+00001dc0: 7465 738d 0000 0073 5800 0000 000b 0e01  tes....sX.......
+00001dd0: 0a02 0401 0801 1001 0a01 06ff 0604 0201  ................
+00001de0: 0cff 0804 0401 1601 0e02 1603 1201 0801  ................
+00001df0: 0801 1201 0801 0801 0801 0401 0401 0c01  ................
+00001e00: 2a01 0e02 0601 0401 0c01 2a01 1a01 2e01  *.........*.....
+00001e10: 0e01 1c01 1a01 0eff 0804 0eff 1a03 0a03  ................
+00001e20: 2c03 1602 7277 0000 0063 0200 0000 0000  ,...rw...c......
+00001e30: 0000 0000 0000 0a00 0000 0700 0000 4300  ..............C.
+00001e40: 0000 73d4 0000 0074 00a0 0174 00a0 027c  ..s....t...t...|
+00001e50: 0064 0164 0185 0264 0266 0219 00a1 01a1  .d.d...d.f......
+00001e60: 017d 0264 027d 0367 007d 047c 0244 005d  .}.d.}.g.}.|.D.]
+00001e70: 627d 057c 0064 0164 0185 0264 0266 0219  b}.|.d.d...d.f..
+00001e80: 007c 056b 027d 0674 00a0 0374 00a0 047c  .|.k.}.t...t...|
+00001e90: 067c 01a1 027c 01a1 0264 0219 007d 077c  .|...|...d...}.|
+00001ea0: 077c 036b 0472 787c 04a0 05a1 0001 007c  .|.k.rx|.......|
+00001eb0: 04a0 067c 05a1 0101 007c 077d 0371 287c  ...|.....|.}.q(|
+00001ec0: 077c 036b 0272 287c 04a0 067c 05a1 0101  .|.k.r(|...|....
+00001ed0: 0071 2874 00a0 077c 0064 0264 0164 0185  .q(t...|.d.d.d..
+00001ee0: 0266 0219 00a1 017d 087c 0444 005d 207d  .f.....}.|.D.] }
+00001ef0: 097c 0874 0874 097c 0983 0164 0318 0064  .|.t.t.|...d...d
+00001f00: 0164 0185 0266 0219 0037 007d 0871 a67c  .d...f...7.}.q.|
+00001f10: 0874 0a7c 0483 011b 0053 0029 047a 4443  .t.|.....S.).zDC
+00001f20: 616c 6375 6c61 7465 7320 7468 6520 6174  alculates the at
+00001f30: 7472 6962 7574 6573 2063 6f72 7265 7370  tributes corresp
+00001f40: 6f6e 6469 6e67 2074 6f20 7468 6520 6d6f  onding to the mo
+00001f50: 7374 2063 6f6d 6d6f 6e20 656c 656d 656e  st common elemen
+00001f60: 7473 2e4e 7201 0000 0072 2100 0000 290b  ts.Nr....r!...).
+00001f70: 722f 0000 00da 0675 6e69 7175 65da 0572  r/.....unique..r
+00001f80: 6176 656c da0b 6578 7061 6e64 5f64 696d  avel..expand_dim
+00001f90: 73da 0373 756d da05 636c 6561 7272 6500  s..sum..clearre.
+00001fa0: 0000 da0a 7a65 726f 735f 6c69 6b65 7231  ....zeros_liker1
+00001fb0: 0000 0072 5300 0000 7257 0000 0029 0ada  ...rS...rW...)..
+00001fc0: 1461 7474 7269 6275 7465 5f70 726f 7065  .attribute_prope
+00001fd0: 7274 6965 73da 0461 7869 73da 0673 636f  rties..axis..sco
+00001fe0: 7265 735a 0e6d 6178 5f6f 6363 7572 7265  resZ.max_occurre
+00001ff0: 6e63 65da 0c74 6f70 5f65 6c65 6d65 6e74  nce..top_element
+00002000: 73da 0573 636f 7265 da08 7465 6d70 6c61  s..score..templa
+00002010: 7465 da05 636f 756e 7472 6e00 0000 da04  te..countrn.....
+00002020: 656c 656d 7224 0000 0072 2400 0000 7228  elemr$...r$...r(
+00002030: 0000 00da 0b6d 6167 7069 655f 6d6f 6465  .....magpie_mode
+00002040: d300 0000 7320 0000 0000 021c 0104 0104  ....s ..........
+00002050: 0108 0114 0118 0108 0108 010a 0106 0108  ................
+00002060: 010c 0116 0108 011e 0172 8600 0000 2902  .........r....).
+00002070: 7249 0000 0072 2000 0000 6301 0000 0000  rI...r ...c.....
+00002080: 0000 0000 0000 0019 0000 000e 0000 0003  ................
+00002090: 0000 0073 2c04 0000 7400 7c00 8301 5c03  ...s,...t.|...\.
+000020a0: 7d01 7d02 7d03 7401 a002 7401 6a03 7401  }.}.}.t...t.j.t.
+000020b0: 6a04 7c01 6401 6402 8d02 7401 6a04 7401  j.|.d.d...t.j.t.
+000020c0: a005 7c01 7401 6a04 7c01 6401 6402 8d02  ..|.t.j.|.d.d...
+000020d0: 1800 a101 6401 6402 8d02 7401 6a06 7c01  ....d.d...t.j.|.
+000020e0: 6401 6402 8d02 7401 6a07 7c01 6401 6402  d.d...t.j.|.d.d.
+000020f0: 8d02 7401 6a07 7c01 6401 6402 8d02 7401  ..t.j.|.d.d...t.
+00002100: 6a06 7c01 6401 6402 8d02 1800 6605 6403  j.|.d.d.....f.d.
+00002110: 6402 8d02 a008 6403 a101 7401 6a03 7401  d.....d...t.j.t.
+00002120: 6a04 7c02 6401 6402 8d02 7401 6a07 7c02  j.|.d.d...t.j.|.
+00002130: 6401 6402 8d02 7401 6a06 7c02 6401 6402  d.d...t.j.|.d.d.
+00002140: 8d02 1800 7401 6a04 7401 a005 7c02 7401  ....t.j.t...|.t.
+00002150: 6a04 7c02 6401 6402 8d02 1800 a101 6401  j.|.d.d.......d.
+00002160: 6402 8d02 7401 6a07 7c02 6401 6402 8d02  d...t.j.|.d.d...
+00002170: 7401 6a06 7c02 6401 6402 8d02 7409 7c02  t.j.|.d.d...t.|.
+00002180: 8301 6606 6403 6402 8d02 a008 6403 a101  ..f.d.d.....d...
+00002190: 6602 a101 7d04 7c04 6404 0500 1900 7c04  f...}.|.d.....|.
+000021a0: 6405 1900 1d00 0300 3c00 7c04 6406 0500  d.......<.|.d...
+000021b0: 1900 7c04 6405 1900 1d00 0300 3c00 7c04  ..|.d.......<.|.
+000021c0: 6407 0500 1900 7c04 6405 1900 1d00 0300  d.....|.d.......
+000021d0: 3c00 7c04 6408 0500 1900 7c04 6409 1900  <.|.d.....|.d...
+000021e0: 1d00 0300 3c00 7401 a00a 7c04 6700 640a  ....<.t...|.g.d.
+000021f0: a201 a102 7d04 7c04 640b 0500 1900 740b  ....}.|.d.....t.
+00002200: 7c02 8301 7c00 6a0c 1b00 3900 0300 3c00  |...|.j...9...<.
+00002210: 740d 7c00 7c03 640c 8303 7d05 740e 7c05  t.|.|.d...}.t.|.
+00002220: 8301 4400 5d14 7d06 7401 a00f 7c04 640b  ..D.].}.t...|.d.
+00002230: 7c06 a103 7d04 9001 718c 6900 7d07 7c00  |...}...q.i.}.|.
+00002240: 6a10 4400 5d56 7d08 7c08 a011 a100 a012  j.D.]V}.|.......
+00002250: a100 4400 5d42 5c02 7d09 7d0a 7c09 7c07  ..D.]B\.}.}.|.|.
+00002260: 7600 9001 72ea 7c07 7c09 0500 1900 7c0a  v...r.|.|.....|.
+00002270: 740b 7c00 6a10 8301 1b00 3700 0300 3c00  t.|.j.....7...<.
+00002280: 6e12 7c0a 740b 7c00 6a10 8301 1b00 7c07  n.|.t.|.j.....|.
+00002290: 7c09 3c00 9001 71bc 9001 71ac 640d 7d0b  |.<...q...q.d.}.
+000022a0: 640e 4400 5d36 8900 7401 a00f 7c04 7c0b  d.D.]6..t...|.|.
+000022b0: 7413 a014 7415 8700 6601 640f 6410 8408  t...t...f.d.d...
+000022c0: 7c07 a016 a100 4400 8301 8301 6411 8800  |.....D.....d...
+000022d0: 1b00 a102 a103 7d04 9002 710c 7401 a00f  ......}...q.t...
+000022e0: 7c04 7c0b 740b 7c07 8301 a103 7d04 6401  |.|.t.|.....}.d.
+000022f0: 6401 6401 6401 6412 9c04 7d0c 6401 7d0d  d.d.d.d...}.d.}.
+00002300: 7c07 a012 a100 4400 5da2 5c02 7d09 7d0a  |.....D.].\.}.}.
+00002310: 7c0c 6413 0500 1900 7c0a 7417 7418 7c09  |.d.....|.t.t.|.
+00002320: 8301 6a19 6414 1800 1900 6407 1900 1400  ..j.d.....d.....
+00002330: 3700 0300 3c00 7c0c 6415 0500 1900 7c0a  7...<.|.d.....|.
+00002340: 7417 7418 7c09 8301 6a19 6414 1800 1900  t.t.|...j.d.....
+00002350: 6416 1900 1400 3700 0300 3c00 7c0c 6417  d.....7...<.|.d.
+00002360: 0500 1900 7c0a 7417 7418 7c09 8301 6a19  ....|.t.t.|...j.
+00002370: 6414 1800 1900 6418 1900 1400 3700 0300  d.....d.....7...
+00002380: 3c00 7c0c 6419 0500 1900 7c0a 7417 7418  <.|.d.....|.t.t.
+00002390: 7c09 8301 6a19 6414 1800 1900 641a 1900  |...j.d.....d...
+000023a0: 1400 3700 0300 3c00 9002 7170 7415 641b  ..7...<...qpt.d.
+000023b0: 641c 8400 7c0c a012 a100 4400 8301 8301  d...|.....D.....
+000023c0: 7d0d 6412 4400 5d1a 7d0e 7401 a01a 7c04  }.d.D.].}.t...|.
+000023d0: 7c0c 7c0e 1900 7c0d 1b00 a102 7d04 9003  |.|...|.....}...
+000023e0: 712e 6401 7d0f 6401 7d10 641d 7d11 641e  q.d.}.d.}.d.}.d.
+000023f0: 7d12 7c00 6a1b a01c a100 6a1d 4400 5d26  }.|.j.....j.D.]&
+00002400: 7d13 7c13 6a1e 6401 6b04 9003 727a 641e  }.|.j.d.k...rzd.
+00002410: 7d11 7c13 6a1e 6401 6b00 9003 7266 641e  }.|.j.d.k...rfd.
+00002420: 7d12 9003 7166 7c07 a012 a100 4400 5d62  }...qf|.....D.]b
+00002430: 5c02 7d14 7d15 7c07 a012 a100 4400 5d4e  \.}.}.|.....D.]N
+00002440: 5c02 7d16 7d17 6411 7413 a01f 641f 7418  \.}.}.d.t...d.t.
+00002450: 7c14 8301 6a20 7418 7c16 8301 6a20 1800  |...j t.|...j ..
+00002460: 6420 1300 1400 a101 1800 7d18 7c18 7c0f  d ........}.|.|.
+00002470: 6b04 9003 72e2 7c18 7d0f 7c10 7c18 7c15  k...r.|.}.|.|.|.
+00002480: 1400 7c17 1400 3700 7d10 9003 71a6 9003  ..|...7.}...q...
+00002490: 7196 7401 a01a 7c04 7421 7c11 9004 6f0a  q.t...|.t!|...o.
+000024a0: 7c12 8301 a102 7d04 7401 a01a 7c04 7c0f  |.....}.t...|.|.
+000024b0: a102 7d04 7401 a01a 7c04 7c10 a102 7d04  ..}.t...|.|...}.
+000024c0: 7c04 5300 2921 7acb 4d61 696e 2066 756e  |.S.)!z.Main fun
+000024d0: 6374 696f 6e61 6c69 7479 2e20 4765 6e65  ctionality. Gene
+000024e0: 7261 7465 7320 7468 6520 5761 7264 3230  rates the Ward20
+000024f0: 3137 2064 6573 6372 6970 746f 7220 666f  17 descriptor fo
+00002500: 7220 6120 6769 7665 6e20 7374 7275 6374  r a given struct
+00002510: 7572 652e 0a0a 2020 2020 4172 6773 3a0a  ure...    Args:.
+00002520: 2020 2020 2020 2020 7374 7275 6374 3a20          struct: 
+00002530: 4120 7079 6d61 7467 656e 2053 7472 7563  A pymatgen Struc
+00002540: 7475 7265 206f 626a 6563 742e 0a0a 2020  ture object...  
+00002550: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00002560: 2020 2041 2032 3731 2d6c 656e 6768 7420     A 271-lenght 
+00002570: 6e75 6d70 7920 6172 7261 7920 6f66 2074  numpy array of t
+00002580: 6865 2064 6573 6372 6970 746f 722e 0a20  he descriptor.. 
+00002590: 2020 2072 0100 0000 2901 727f 0000 00e9     r....).r.....
+000025a0: ffff ffff 7210 0000 0072 0e00 0000 e907  ....r....r......
+000025b0: 0000 00e9 0800 0000 e910 0000 00e9 0f00  ................
+000025c0: 0000 290c e904 0000 0072 0e00 0000 e909  ..)......r......
+000025d0: 0000 00e9 0e00 0000 728b 0000 0072 1e00  ........r....r..
+000025e0: 0000 721c 0000 00e9 1300 0000 e915 0000  ..r.............
+000025f0: 00e9 1600 0000 e917 0000 00e9 1800 0000  ................
+00002600: e90c 0000 00e9 0300 0000 e97e 0000 0029  ...........~...)
+00002610: 0572 1100 0000 7288 0000 0072 0e00 0000  .r....r....r....
+00002620: 7295 0000 0072 0c00 0000 6301 0000 0000  r....r....c.....
+00002630: 0000 0000 0000 0002 0000 0005 0000 0033  ...............3
+00002640: 0000 0073 1a00 0000 7c00 5d12 7d01 7400  ...s....|.].}.t.
+00002650: a001 7c01 8800 a102 5600 0100 7102 6400  ..|.....V...q.d.
+00002660: 5300 7247 0000 0029 0272 3a00 0000 723c  S.rG...).r:...r<
+00002670: 0000 0072 2500 0000 a901 da01 7072 2400  ...r%.......pr$.
+00002680: 0000 7228 0000 0072 2e00 0000 1901 0000  ..r(...r........
+00002690: 722a 0000 007a 2667 656e 6572 6174 655f  r*...z&generate_
+000026a0: 6465 7363 7269 7074 6f72 2e3c 6c6f 6361  descriptor.<loca
+000026b0: 6c73 3e2e 3c67 656e 6578 7072 3e72 6400  ls>.<genexpr>rd.
+000026c0: 0000 2904 da01 7372 9800 0000 da01 64da  ..)...sr......d.
+000026d0: 0166 7299 0000 0072 2100 0000 7298 0000  .fr....r!...r...
+000026e0: 0072 8d00 0000 729a 0000 0072 1100 0000  .r....r....r....
+000026f0: 729b 0000 00e9 0b00 0000 6301 0000 0000  r.........c.....
+00002700: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
+00002710: 0000 0073 1400 0000 6700 7c00 5d0c 5c02  ...s....g.|.].\.
+00002720: 7d01 7d02 7c02 9102 7104 5300 7224 0000  }.}.|...q.S.r$..
+00002730: 0072 2400 0000 2903 7226 0000 0072 4000  .r$...).r&...r@.
+00002740: 0000 da03 7661 6c72 2400 0000 7224 0000  ....valr$...r$..
+00002750: 0072 2800 0000 7229 0000 0023 0100 0072  .r(...r)...#...r
+00002760: 2a00 0000 7a27 6765 6e65 7261 7465 5f64  *...z'generate_d
+00002770: 6573 6372 6970 746f 722e 3c6c 6f63 616c  escriptor.<local
+00002780: 733e 2e3c 6c69 7374 636f 6d70 3e46 5467  s>.<listcomp>FTg
+00002790: 0000 0000 0000 d0bf 720c 0000 0029 2272  ........r....)"r
+000027a0: 5f00 0000 722f 0000 0072 3d00 0000 da05  _...r/...r=.....
+000027b0: 7374 6163 6b72 6900 0000 7238 0000 0072  stackri...r8...r
+000027c0: 3900 0000 da03 6d61 78da 0772 6573 6861  9.....max..resha
+000027d0: 7065 7286 0000 00da 0664 656c 6574 6572  per......deleter
+000027e0: 5700 0000 722b 0000 0072 7700 0000 da08  W...r+...rw.....
+000027f0: 7265 7665 7273 6564 da06 696e 7365 7274  reversed..insert
+00002800: 7256 0000 0072 3400 0000 7235 0000 0072  rV...r4...r5...r
+00002810: 3a00 0000 723c 0000 0072 7b00 0000 7237  :...r<...r{...r7
+00002820: 0000 0072 3100 0000 7203 0000 0072 3600  ...r1...r....r6.
+00002830: 0000 7265 0000 0072 5e00 0000 da22 6164  ..re...r^...."ad
+00002840: 645f 6368 6172 6765 735f 6672 6f6d 5f6f  d_charges_from_o
+00002850: 7869 5f73 7461 7465 5f67 7565 7373 6573  xi_state_guesses
+00002860: da08 656c 656d 656e 7473 da09 6f78 695f  ..elements..oxi_
+00002870: 7374 6174 65da 0365 7870 da01 58da 0566  state..exp..X..f
+00002880: 6c6f 6174 2919 7249 0000 005a 0f64 6966  loat).rI...Z.dif
+00002890: 665f 7072 6f70 6572 7469 6573 727e 0000  f_propertiesr~..
+000028a0: 0072 6c00 0000 da0a 7072 6f70 6572 7469  .rl.....properti
+000028b0: 6573 5a0d 7763 5f61 7474 7269 6275 7465  esZ.wc_attribute
+000028c0: 73da 0961 7474 7269 6275 7465 723f 0000  s..attributer?..
+000028d0: 0072 5e00 0000 7240 0000 0072 2700 0000  .r^...r@...r'...
+000028e0: da08 706f 7369 7469 6f6e 5a18 656c 6563  ..positionZ.elec
+000028f0: 7472 6f6e 5f6f 6363 7570 6174 696f 6e5f  tron_occupation_
+00002900: 6469 6374 5a14 746f 7461 6c5f 7661 6c65  dictZ.total_vale
+00002910: 6e63 655f 6661 6374 6f72 5a03 6f72 625a  nce_factorZ.orbZ
+00002920: 0e6d 6178 5f69 6f6e 6963 5f63 6861 725a  .max_ionic_charZ
+00002930: 0d61 765f 696f 6e69 635f 6368 6172 5a0a  .av_ionic_charZ.
+00002940: 6861 735f 616e 696f 6e73 5a0b 6861 735f  has_anionsZ.has_
+00002950: 6361 7469 6f6e 73da 0265 6cda 046b 6579  cations..el..key
+00002960: 315a 0676 616c 7565 31da 046b 6579 325a  1Z.value1..key2Z
+00002970: 0676 616c 7565 325a 0a69 6f6e 6963 5f63  .value2Z.ionic_c
+00002980: 6861 7272 2400 0000 7297 0000 0072 2800  harr$...r....r(.
+00002990: 0000 da13 6765 6e65 7261 7465 5f64 6573  ....generate_des
+000029a0: 6372 6970 746f 72e7 0000 0073 a000 0000  criptor....s....
+000029b0: 0009 0e01 1401 2001 0c01 0c01 0c01 0cff  ...... .........
+000029c0: 02fc 0205 02fb 0605 02fb 0206 1001 0c01  ................
+000029d0: 0cff 0202 1a01 02ff 0402 0c01 0c01 06f9  ................
+000029e0: 0207 02f9 0607 02f9 02fa 060f 1401 1401  ................
+000029f0: 1402 1402 1002 1a02 0c01 0c01 1202 0401  ................
+00002a00: 0a01 1401 0a01 1c02 1a01 0401 0801 0601  ................
+00002a10: 0201 24fe 0803 1202 0e01 0401 1001 2601  ..$...........&.
+00002a20: 2601 2601 2a01 1601 0801 1802 0401 0401  &.&.*...........
+00002a30: 0401 0401 1001 0c01 0401 0c01 0801 1001  ................
+00002a40: 1001 2601 0a01 0401 1801 1601 0c01 0c01  ..&.............
+00002a50: 72b0 0000 0063 0000 0000 0000 0000 0000  r....c..........
+00002a60: 0000 0000 0000 0100 0000 4300 0000 7304  ..........C...s.
+00002a70: 0000 0074 0053 0029 017a 1e43 6974 6174  ...t.S.).z.Citat
+00002a80: 696f 6e2f 7320 666f 7220 7468 6520 6465  ion/s for the de
+00002a90: 7363 7269 7074 6f72 2e29 01da 0963 6974  scriptor.)...cit
+00002aa0: 6174 696f 6e73 7224 0000 0072 2400 0000  ationsr$...r$...
+00002ab0: 7224 0000 0072 2800 0000 da04 6369 7465  r$...r(.....cite
+00002ac0: 3c01 0000 7302 0000 0000 0272 b200 0000  <...s......r....
+00002ad0: fa0b 4a56 4153 502d 3130 3030 3172 1100  ..JVASP-10001r..
+00002ae0: 0000 6302 0000 0000 0000 0000 0000 0007  ..c.............
+00002af0: 0000 0008 0000 0043 0000 0073 be00 0000  .......C...s....
+00002b00: 7c00 6401 6b02 721e 7400 6402 7c01 9b00  |.d.k.r.t.d.|...
+00002b10: 6403 9d03 8301 0100 6404 7d02 6e2a 7c00  d.......d.}.n*|.
+00002b20: 6405 6b02 723c 7400 6406 7c01 9b00 6403  d.k.r<t.d.|...d.
+00002b30: 9d03 8301 0100 6407 7d02 6e0c 7400 6408  ......d.}.n.t.d.
+00002b40: 8301 0100 6409 5300 7401 a002 7403 a004  ....d.S.t...t...
+00002b50: 7c02 a101 a101 6701 7c01 1400 7d03 7405  |.....g.|...}.t.
+00002b60: 7c03 8301 4400 5d0c 7d04 7406 7c04 8301  |...D.].}.t.|...
+00002b70: 7d05 7166 7407 640a 640b 8302 8f24 7d06  }.qft.d.d....$}.
+00002b80: 7c06 a008 640c 640d 8400 7c05 4400 8301  |...d.d...|.D...
+00002b90: a101 0100 5700 6409 0400 0400 8303 0100  ....W.d.........
+00002ba0: 6e10 3100 73a8 3000 0100 0100 0100 5900  n.1.s.0.......Y.
+00002bb0: 0100 7400 640e 8301 0100 6409 5300 290f  ..t.d.....d.S.).
+00002bc0: 7a43 5072 6f66 696c 6573 2074 6865 2064  zCProfiles the d
+00002bd0: 6573 6372 6970 746f 7220 696e 2073 6572  escriptor in ser
+00002be0: 6965 7320 7573 696e 6720 6f6e 6520 6f66  ies using one of
+00002bf0: 2074 6865 2074 6573 7420 7374 7275 6374   the test struct
+00002c00: 7572 6573 2e72 b300 0000 fa5d 5761 7264  ures.r.....]Ward
+00002c10: 3230 3137 2070 726f 6669 6c69 6e67 2f74  2017 profiling/t
+00002c20: 6573 7469 6e67 2074 6173 6b20 7769 6c6c  esting task will
+00002c30: 2063 616c 6375 6c61 7465 2061 2064 6573   calculate a des
+00002c40: 6372 6970 746f 7220 666f 7220 4c69 3220  criptor for Li2 
+00002c50: 5a72 3120 5465 3120 4f36 2028 4a56 4153  Zr1 Te1 O6 (JVAS
+00002c60: 502d 3130 3030 3129 207a 1120 7469 6d65  P-10001) z. time
+00002c70: 7320 696e 2073 6572 6965 732e e146 0a00  s in series..F..
+00002c80: 007b 2240 6d6f 6475 6c65 223a 2022 7079  .{"@module": "py
+00002c90: 6d61 7467 656e 2e63 6f72 652e 7374 7275  matgen.core.stru
+00002ca0: 6374 7572 6522 2c20 2240 636c 6173 7322  cture", "@class"
+00002cb0: 3a20 2253 7472 7563 7475 7265 222c 2022  : "Structure", "
+00002cc0: 6368 6172 6765 223a 206e 756c 6c2c 2022  charge": null, "
+00002cd0: 6c61 7474 6963 6522 3a20 7b22 6d61 7472  lattice": {"matr
+00002ce0: 6978 223a 205b 5b34 2e35 3939 3330 3536  ix": [[4.5993056
+00002cf0: 3532 3636 3234 3539 2c20 302e 3030 3938  52662459, 0.0098
+00002d00: 3031 3530 3736 3939 3838 3233 2c20 332e  015076998823, 3.
+00002d10: 3130 3532 3631 3238 3635 3434 3337 3336  1052612865443736
+00002d20: 5d2c 205b 312e 3635 3533 3235 3737 3236  ], [1.6553257726
+00002d30: 3230 3436 3533 2c20 342e 3239 3131 3038  204653, 4.291108
+00002d40: 3437 3538 3534 3731 322c 2033 2e31 3035  475854712, 3.105
+00002d50: 3236 3032 3933 3839 3739 3536 355d 2c20  2602938979565], 
+00002d60: 5b30 2e30 3134 3235 3431 3231 3439 3139  [0.0142541214919
+00002d70: 3734 392c 2030 2e30 3039 3830 3235 3039  749, 0.009802509
+00002d80: 3939 3936 3133 312c 2035 2e35 3439 3431  9996131, 5.54941
+00002d90: 3931 3431 3836 3633 3531 5d5d 2c20 2261  9141866351]], "a
+00002da0: 223a 2035 2e35 3439 3434 3634 3738 3135  ": 5.54944647815
+00002db0: 3233 3236 2c20 2262 223a 2035 2e35 3439  2326, "b": 5.549
+00002dc0: 3434 3635 3336 3137 3933 3433 2c20 2263  446536179343, "c
+00002dd0: 223a 2035 2e35 3439 3434 3631 3035 3831  ": 5.54944610581
+00002de0: 3034 3233 2c20 2261 6c70 6861 223a 2035  0423, "alpha": 5
+00002df0: 352e 3832 3731 3434 3539 3938 3538 3332  5.82714459985832
+00002e00: 2c20 2262 6574 6122 3a20 3535 2e38 3237  , "beta": 55.827
+00002e10: 3134 3031 3432 3839 3337 312c 2022 6761  14014289371, "ga
+00002e20: 6d6d 6122 3a20 3535 2e38 3237 3133 3937  mma": 55.8271397
+00002e30: 3237 3739 3039 322c 2022 766f 6c75 6d65  2779092, "volume
+00002e40: 223a 2031 3039 2e31 3534 3834 3632 3536  ": 109.154846256
+00002e50: 3432 3734 337d 2c20 2273 6974 6573 223a  42743}, "sites":
+00002e60: 205b 7b22 7370 6563 6965 7322 3a20 5b7b   [{"species": [{
+00002e70: 2265 6c65 6d65 6e74 223a 2022 4c69 222c  "element": "Li",
+00002e80: 2022 6f63 6375 223a 2031 2e30 7d5d 2c20   "occu": 1.0}], 
+00002e90: 2261 6263 223a 205b 302e 3237 3338 3738  "abc": [0.273878
+00002ea0: 3438 3732 3636 3939 3234 2c20 302e 3237  4872669924, 0.27
+00002eb0: 3338 3738 3438 3732 3637 3034 3037 2c20  38784872670407, 
+00002ec0: 302e 3237 3338 3738 3438 3732 3637 3330  0.27387848726730
+00002ed0: 3332 5d2c 2022 7879 7a22 3a20 5b31 2e37  32], "xyz": [1.7
+00002ee0: 3136 3931 3238 3930 3430 3037 3036 332c  169128904007063,
+00002ef0: 2031 2e31 3830 3631 3134 3136 3737 3737   1.1806114167777
+00002f00: 3631 332c 2033 2e32 3230 3739 3437 3735  613, 3.220794775
+00002f10: 3337 3732 3738 5d2c 2022 6c61 6265 6c22  377278], "label"
+00002f20: 3a20 224c 6922 2c20 2270 726f 7065 7274  : "Li", "propert
+00002f30: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00002f40: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00002f50: 7422 3a20 224c 6922 2c20 226f 6363 7522  t": "Li", "occu"
+00002f60: 3a20 312e 307d 5d2c 2022 6162 6322 3a20  : 1.0}], "abc": 
+00002f70: 5b30 2e37 3835 3232 3732 3031 3037 3238  [0.7852272010728
+00002f80: 3036 392c 2030 2e37 3835 3232 3732 3031  069, 0.785227201
+00002f90: 3037 3238 3835 362c 2030 2e37 3835 3232  0728856, 0.78522
+00002fa0: 3732 3031 3037 3333 3135 5d2c 2022 7879  7201073315], "xy
+00002fb0: 7a22 3a20 5b34 2e39 3232 3439 3934 3531  z": [4.922499451
+00002fc0: 3733 3939 3635 2c20 332e 3338 3438 3838  739965, 3.384888
+00002fd0: 3730 3539 3433 3439 3237 2c20 392e 3233  7059434927, 9.23
+00002fe0: 3432 3235 3333 3831 3633 3633 335d 2c20  4225338163633], 
+00002ff0: 226c 6162 656c 223a 2022 4c69 222c 2022  "label": "Li", "
+00003000: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+00003010: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+00003020: 2265 6c65 6d65 6e74 223a 2022 4f22 2c20  "element": "O", 
+00003030: 226f 6363 7522 3a20 312e 307d 5d2c 2022  "occu": 1.0}], "
+00003040: 6162 6322 3a20 5b30 2e38 3636 3939 3634  abc": [0.8669964
+00003050: 3435 3436 3631 3132 342c 2030 2e36 3034  454661124, 0.604
+00003060: 3038 3938 3832 3039 3231 3134 2c20 302e  089882092114, 0.
+00003070: 3234 3138 3231 3736 3938 3733 3134 335d  241821769873143]
+00003080: 2c20 2278 797a 223a 205b 342e 3939 3039  , "xyz": [4.9909
+00003090: 3934 3136 3031 3634 3036 312c 2032 2e36  94160164061, 2.6
+000030a0: 3033 3038 3335 3435 3837 3638 3536 2c20  03083545876856, 
+000030b0: 352e 3931 3030 3737 3138 3131 3337 3635  5.91007718113765
+000030c0: 385d 2c20 226c 6162 656c 223a 2022 4f22  8], "label": "O"
+000030d0: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
+000030e0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
+000030f0: 205b 7b22 656c 656d 656e 7422 3a20 224f   [{"element": "O
+00003100: 222c 2022 6f63 6375 223a 2031 2e30 7d5d  ", "occu": 1.0}]
+00003110: 2c20 2261 6263 223a 205b 302e 3731 3738  , "abc": [0.7178
+00003120: 3430 3839 3435 3239 3738 382c 2030 2e31  40894529788, 0.1
+00003130: 3231 3336 3735 3838 3936 3238 3638 332c  213675889628683,
+00003140: 2030 2e33 3933 3533 3730 3039 3138 3639   0.3935370091869
+00003150: 3733 5d2c 2022 7879 7a22 3a20 5b33 2e35  73], "xyz": [3.5
+00003160: 3038 3038 3231 3036 3233 3437 3133 2c20  08082106234713, 
+00003170: 302e 3533 3136 3935 3036 3332 3135 3431  0.53169506321541
+00003180: 322c 2034 2e37 3839 3836 3333 3036 3436  2, 4.78986330646
+00003190: 3932 3738 5d2c 2022 6c61 6265 6c22 3a20  9278], "label": 
+000031a0: 224f 222c 2022 7072 6f70 6572 7469 6573  "O", "properties
+000031b0: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
+000031c0: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
+000031d0: 2022 4f22 2c20 226f 6363 7522 3a20 312e   "O", "occu": 1.
+000031e0: 307d 5d2c 2022 6162 6322 3a20 5b30 2e31  0}], "abc": [0.1
+000031f0: 3231 3336 3735 3838 3936 3338 3430 322c  213675889638402,
+00003200: 2030 2e33 3933 3533 3730 3039 3138 3733   0.3935370091873
+00003210: 3934 332c 2030 2e37 3137 3834 3038 3934  943, 0.717840894
+00003220: 3532 3833 3338 345d 2c20 2278 797a 223a  5283384], "xyz":
+00003230: 205b 312e 3231 3938 3730 3738 3330 3831   [1.219870783081
+00003240: 3738 3936 2c20 312e 3639 3639 3336 3232  7896, 1.69693622
+00003250: 3335 3931 3033 3137 2c20 352e 3538 3235  35910317, 5.5825
+00003260: 3132 3932 3531 3639 3634 5d2c 2022 6c61  1292516964], "la
+00003270: 6265 6c22 3a20 224f 222c 2022 7072 6f70  bel": "O", "prop
+00003280: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00003290: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+000032a0: 6d65 6e74 223a 2022 4f22 2c20 226f 6363  ment": "O", "occ
+000032b0: 7522 3a20 312e 307d 5d2c 2022 6162 6322  u": 1.0}], "abc"
+000032c0: 3a20 5b30 2e33 3933 3533 3730 3039 3138  : [0.39353700918
+000032d0: 3631 3931 352c 2030 2e37 3137 3834 3038  61915, 0.7178408
+000032e0: 3934 3532 3933 3835 362c 2030 2e31 3231  945293856, 0.121
+000032f0: 3336 3735 3838 3936 3334 3031 345d 2c20  3675889634014], 
+00003300: 2278 797a 223a 205b 322e 3939 3939 3837  "xyz": [2.999987
+00003310: 3531 3235 3935 3632 322c 2033 2e30 3835  512595622, 3.085
+00003320: 3338 3031 3039 3836 3033 3434 2c20 342e  380109860344, 4.
+00003330: 3132 3436 3337 3638 3739 3632 3239 375d  124637687962297]
+00003340: 2c20 226c 6162 656c 223a 2022 4f22 2c20  , "label": "O", 
+00003350: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00003360: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00003370: 7b22 656c 656d 656e 7422 3a20 224f 222c  {"element": "O",
+00003380: 2022 6f63 6375 223a 2031 2e30 7d5d 2c20   "occu": 1.0}], 
+00003390: 2261 6263 223a 205b 302e 3234 3138 3231  "abc": [0.241821
+000033a0: 3736 3938 3732 3135 3733 2c20 302e 3836  7698721573, 0.86
+000033b0: 3639 3936 3434 3534 3637 3132 3231 2c20  69964454671221, 
+000033c0: 302e 3630 3430 3839 3838 3230 3932 3135  0.60408988209215
+000033d0: 3133 5d2c 2022 7879 7a22 3a20 5b32 2e35  13], "xyz": [2.5
+000033e0: 3535 3938 3435 3634 3633 3333 3239 2c20  55984564633329, 
+000033f0: 332e 3732 3836 3637 3631 3037 3239 3134  3.72866761072914
+00003400: 392c 2036 2e37 3935 3531 3733 3732 3337  9, 6.79551737237
+00003410: 3733 3433 5d2c 2022 6c61 6265 6c22 3a20  7343], "label": 
+00003420: 224f 222c 2022 7072 6f70 6572 7469 6573  "O", "properties
+00003430: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
+00003440: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
+00003450: 2022 4f22 2c20 226f 6363 7522 3a20 312e   "O", "occu": 1.
+00003460: 307d 5d2c 2022 6162 6322 3a20 5b30 2e36  0}], "abc": [0.6
+00003470: 3034 3038 3938 3832 3039 3333 3131 352c  040898820933115,
+00003480: 2030 2e32 3431 3832 3137 3639 3837 3233   0.2418217698723
+00003490: 3633 372c 2030 2e38 3636 3939 3634 3435  637, 0.866996445
+000034a0: 3436 3634 3035 395d 2c20 2278 797a 223a  4664059], "xyz":
+000034b0: 205b 332e 3139 3130 3436 3039 3031 3435   [3.191046090145
+000034c0: 3137 332c 2031 2e30 3532 3130 3331 3739  173, 1.052103179
+000034d0: 3330 3235 3539 352c 2037 2e34 3338 3130  3025595, 7.43810
+000034e0: 3331 3335 3034 3336 3533 355d 2c20 226c  31350436535], "l
+000034f0: 6162 656c 223a 2022 4f22 2c20 2270 726f  abel": "O", "pro
+00003500: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00003510: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00003520: 656d 656e 7422 3a20 2254 6522 2c20 226f  ement": "Te", "o
+00003530: 6363 7522 3a20 312e 307d 5d2c 2022 6162  ccu": 1.0}], "ab
+00003540: 6322 3a20 5b30 2e34 3936 3539 3035 3631  c": [0.496590561
+00003550: 3035 3037 3335 332c 2030 2e34 3936 3539  0507353, 0.49659
+00003560: 3035 3631 3035 3037 3335 352c 2030 2e34  05610507355, 0.4
+00003570: 3936 3539 3035 3631 3035 3037 3336 315d  965905610507361]
+00003580: 2c20 2278 797a 223a 205b 332e 3131 3330  , "xyz": [3.1130
+00003590: 3639 3339 3038 3335 3739 332c 2032 2e31  69390835793, 2.1
+000035a0: 3430 3635 3931 3335 3730 3234 3938 342c  406591357024984,
+000035b0: 2035 2e38 3339 3837 3535 3631 3231 3436   5.8398755612146
+000035c0: 3632 345d 2c20 226c 6162 656c 223a 2022  624], "label": "
+000035d0: 5465 222c 2022 7072 6f70 6572 7469 6573  Te", "properties
+000035e0: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
+000035f0: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
+00003600: 2022 5a72 222c 2022 6f63 6375 223a 2031   "Zr", "occu": 1
+00003610: 2e30 7d5d 2c20 2261 6263 223a 205b 302e  .0}], "abc": [0.
+00003620: 3030 3036 3530 3136 3034 3938 3036 3638  0006501604980668
+00003630: 2c20 302e 3030 3036 3530 3136 3034 3938  , 0.000650160498
+00003640: 3039 3238 2c20 302e 3030 3036 3530 3136  0928, 0.00065016
+00003650: 3034 3938 3233 3434 5d2c 2022 7879 7a22  04982344], "xyz"
+00003660: 3a20 5b30 2e30 3034 3037 3537 3831 3734  : [0.00407578174
+00003670: 3934 3630 3336 2c20 302e 3030 3238 3032  946036, 0.002802
+00003680: 3635 3439 3831 3934 3531 3932 2c20 302e  654981945192, 0.
+00003690: 3030 3736 3435 3834 3839 3138 3236 3330  0076458489182630
+000036a0: 3736 5d2c 2022 6c61 6265 6c22 3a20 225a  76], "label": "Z
+000036b0: 7222 2c20 2270 726f 7065 7274 6965 7322  r", "properties"
+000036c0: 3a20 7b7d 7d5d 7dda 0d64 696c 7574 654e  : {}}]}..diluteN
+000036d0: 6941 6c6c 6f79 fa5b 5761 7264 3230 3137  iAlloy.[Ward2017
+000036e0: 2070 726f 6669 6c69 6e67 2f74 6573 7469   profiling/testi
+000036f0: 6e67 2074 6173 6b20 7769 6c6c 2063 616c  ng task will cal
+00003700: 6375 6c61 7465 2061 2064 6573 6372 6970  culate a descrip
+00003710: 746f 7220 666f 7220 6120 6469 6c75 7465  tor for a dilute
+00003720: 2046 4343 204e 6933 3143 7231 2061 6c6c   FCC Ni31Cr1 all
+00003730: 6f79 20e1 d414 0000 7b22 406d 6f64 756c  oy .....{"@modul
+00003740: 6522 3a20 2270 796d 6174 6765 6e2e 636f  e": "pymatgen.co
+00003750: 7265 2e73 7472 7563 7475 7265 222c 2022  re.structure", "
+00003760: 4063 6c61 7373 223a 2022 5374 7275 6374  @class": "Struct
+00003770: 7572 6522 2c20 2263 6861 7267 6522 3a20  ure", "charge": 
+00003780: 6e75 6c6c 2c20 226c 6174 7469 6365 223a  null, "lattice":
+00003790: 207b 226d 6174 7269 7822 3a20 5b5b 362e   {"matrix": [[6.
+000037a0: 3939 3536 3932 2c20 302e 302c 2030 2e30  995692, 0.0, 0.0
+000037b0: 5d2c 205b 302e 302c 2036 2e39 3935 3639  ], [0.0, 6.99569
+000037c0: 322c 2030 2e30 5d2c 205b 302e 302c 2030  2, 0.0], [0.0, 0
+000037d0: 2e30 2c20 362e 3939 3536 3932 5d5d 2c20  .0, 6.995692]], 
+000037e0: 2261 223a 2036 2e39 3935 3639 322c 2022  "a": 6.995692, "
+000037f0: 6222 3a20 362e 3939 3536 3932 2c20 2263  b": 6.995692, "c
+00003800: 223a 2036 2e39 3935 3639 322c 2022 616c  ": 6.995692, "al
+00003810: 7068 6122 3a20 3930 2e30 2c20 2262 6574  pha": 90.0, "bet
+00003820: 6122 3a20 3930 2e30 2c20 2267 616d 6d61  a": 90.0, "gamma
+00003830: 223a 2039 302e 302c 2022 766f 6c75 6d65  ": 90.0, "volume
+00003840: 223a 2033 3432 2e33 3637 3131 3336 3536  ": 342.367113656
+00003850: 3139 3234 337d 2c20 2273 6974 6573 223a  19243}, "sites":
+00003860: 205b 7b22 7370 6563 6965 7322 3a20 5b7b   [{"species": [{
+00003870: 2265 6c65 6d65 6e74 223a 2022 4372 222c  "element": "Cr",
+00003880: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+00003890: 6263 223a 205b 302e 302c 2030 2e30 2c20  bc": [0.0, 0.0, 
+000038a0: 302e 305d 2c20 2278 797a 223a 205b 302e  0.0], "xyz": [0.
+000038b0: 302c 2030 2e30 2c20 302e 305d 2c20 226c  0, 0.0, 0.0], "l
+000038c0: 6162 656c 223a 2022 4372 222c 2022 7072  abel": "Cr", "pr
+000038d0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+000038e0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+000038f0: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00003900: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00003910: 223a 205b 302e 302c 2030 2e30 2c20 302e  ": [0.0, 0.0, 0.
+00003920: 355d 2c20 2278 797a 223a 205b 302e 302c  5], "xyz": [0.0,
+00003930: 2030 2e30 2c20 332e 3439 3738 3436 5d2c   0.0, 3.497846],
+00003940: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+00003950: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00003960: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00003970: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
+00003980: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
+00003990: 6162 6322 3a20 5b30 2e30 2c20 302e 352c  abc": [0.0, 0.5,
+000039a0: 2030 2e30 5d2c 2022 7879 7a22 3a20 5b30   0.0], "xyz": [0
+000039b0: 2e30 2c20 332e 3439 3738 3436 2c20 302e  .0, 3.497846, 0.
+000039c0: 305d 2c20 226c 6162 656c 223a 2022 4e69  0], "label": "Ni
+000039d0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000039e0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000039f0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+00003a00: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00003a10: 2c20 2261 6263 223a 205b 302e 302c 2030  , "abc": [0.0, 0
+00003a20: 2e35 2c20 302e 355d 2c20 2278 797a 223a  .5, 0.5], "xyz":
+00003a30: 205b 302e 302c 2033 2e34 3937 3834 362c   [0.0, 3.497846,
+00003a40: 2033 2e34 3937 3834 365d 2c20 226c 6162   3.497846], "lab
+00003a50: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+00003a60: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00003a70: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+00003a80: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+00003a90: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+00003aa0: 205b 302e 352c 2030 2e30 2c20 302e 305d   [0.5, 0.0, 0.0]
+00003ab0: 2c20 2278 797a 223a 205b 332e 3439 3738  , "xyz": [3.4978
+00003ac0: 3436 2c20 302e 302c 2030 2e30 5d2c 2022  46, 0.0, 0.0], "
+00003ad0: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00003ae0: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00003af0: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+00003b00: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+00003b10: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+00003b20: 6322 3a20 5b30 2e35 2c20 302e 302c 2030  c": [0.5, 0.0, 0
+00003b30: 2e35 5d2c 2022 7879 7a22 3a20 5b33 2e34  .5], "xyz": [3.4
+00003b40: 3937 3834 362c 2030 2e30 2c20 332e 3439  97846, 0.0, 3.49
+00003b50: 3738 3436 5d2c 2022 6c61 6265 6c22 3a20  7846], "label": 
+00003b60: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00003b70: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00003b80: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00003b90: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00003ba0: 317d 5d2c 2022 6162 6322 3a20 5b30 2e35  1}], "abc": [0.5
+00003bb0: 2c20 302e 352c 2030 2e30 5d2c 2022 7879  , 0.5, 0.0], "xy
+00003bc0: 7a22 3a20 5b33 2e34 3937 3834 362c 2033  z": [3.497846, 3
+00003bd0: 2e34 3937 3834 362c 2030 2e30 5d2c 2022  .497846, 0.0], "
+00003be0: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00003bf0: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00003c00: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+00003c10: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+00003c20: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+00003c30: 6322 3a20 5b30 2e35 2c20 302e 352c 2030  c": [0.5, 0.5, 0
+00003c40: 2e35 5d2c 2022 7879 7a22 3a20 5b33 2e34  .5], "xyz": [3.4
+00003c50: 3937 3834 362c 2033 2e34 3937 3834 362c  97846, 3.497846,
+00003c60: 2033 2e34 3937 3834 365d 2c20 226c 6162   3.497846], "lab
+00003c70: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+00003c80: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00003c90: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+00003ca0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+00003cb0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+00003cc0: 205b 302e 3235 2c20 302e 3235 2c20 302e   [0.25, 0.25, 0.
+00003cd0: 305d 2c20 2278 797a 223a 205b 312e 3734  0], "xyz": [1.74
+00003ce0: 3839 3233 2c20 312e 3734 3839 3233 2c20  8923, 1.748923, 
+00003cf0: 302e 305d 2c20 226c 6162 656c 223a 2022  0.0], "label": "
+00003d00: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
+00003d10: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
+00003d20: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
+00003d30: 2022 4e69 222c 2022 6f63 6375 223a 2031   "Ni", "occu": 1
+00003d40: 7d5d 2c20 2261 6263 223a 205b 302e 3235  }], "abc": [0.25
+00003d50: 2c20 302e 3235 2c20 302e 355d 2c20 2278  , 0.25, 0.5], "x
+00003d60: 797a 223a 205b 312e 3734 3839 3233 2c20  yz": [1.748923, 
+00003d70: 312e 3734 3839 3233 2c20 332e 3439 3738  1.748923, 3.4978
+00003d80: 3436 5d2c 2022 6c61 6265 6c22 3a20 224e  46], "label": "N
+00003d90: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00003da0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+00003db0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00003dc0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00003dd0: 5d2c 2022 6162 6322 3a20 5b30 2e32 352c  ], "abc": [0.25,
+00003de0: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00003df0: 3030 312c 2030 2e30 5d2c 2022 7879 7a22  001, 0.0], "xyz"
+00003e00: 3a20 5b31 2e37 3438 3932 332c 2035 2e32  : [1.748923, 5.2
+00003e10: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
+00003e20: 2030 2e30 5d2c 2022 6c61 6265 6c22 3a20   0.0], "label": 
+00003e30: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00003e40: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00003e50: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00003e60: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00003e70: 317d 5d2c 2022 6162 6322 3a20 5b30 2e32  1}], "abc": [0.2
+00003e80: 352c 2030 2e37 3530 3030 3030 3030 3030  5, 0.75000000000
+00003e90: 3030 3030 312c 2030 2e35 5d2c 2022 7879  00001, 0.5], "xy
+00003ea0: 7a22 3a20 5b31 2e37 3438 3932 332c 2035  z": [1.748923, 5
+00003eb0: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
+00003ec0: 352c 2033 2e34 3937 3834 365d 2c20 226c  5, 3.497846], "l
+00003ed0: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00003ee0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00003ef0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00003f00: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00003f10: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00003f20: 223a 205b 302e 3735 3030 3030 3030 3030  ": [0.7500000000
+00003f30: 3030 3030 3031 2c20 302e 3235 2c20 302e  000001, 0.25, 0.
+00003f40: 305d 2c20 2278 797a 223a 205b 352e 3234  0], "xyz": [5.24
+00003f50: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00003f60: 312e 3734 3839 3233 2c20 302e 305d 2c20  1.748923, 0.0], 
+00003f70: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+00003f80: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+00003f90: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+00003fa0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+00003fb0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+00003fc0: 6263 223a 205b 302e 3735 3030 3030 3030  bc": [0.75000000
+00003fd0: 3030 3030 3030 3031 2c20 302e 3235 2c20  00000001, 0.25, 
+00003fe0: 302e 355d 2c20 2278 797a 223a 205b 352e  0.5], "xyz": [5.
+00003ff0: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
+00004000: 2c20 312e 3734 3839 3233 2c20 332e 3439  , 1.748923, 3.49
+00004010: 3738 3436 5d2c 2022 6c61 6265 6c22 3a20  7846], "label": 
+00004020: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00004030: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00004040: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00004050: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00004060: 317d 5d2c 2022 6162 6322 3a20 5b30 2e37  1}], "abc": [0.7
+00004070: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+00004080: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00004090: 3030 312c 2030 2e30 5d2c 2022 7879 7a22  001, 0.0], "xyz"
+000040a0: 3a20 5b35 2e32 3436 3736 3930 3030 3030  : [5.24676900000
+000040b0: 3030 3030 352c 2035 2e32 3436 3736 3930  00005, 5.2467690
+000040c0: 3030 3030 3030 3030 352c 2030 2e30 5d2c  000000005, 0.0],
+000040d0: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+000040e0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+000040f0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00004100: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
+00004110: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
+00004120: 6162 6322 3a20 5b30 2e37 3530 3030 3030  abc": [0.7500000
+00004130: 3030 3030 3030 3030 312c 2030 2e37 3530  000000001, 0.750
+00004140: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
+00004150: 2e35 5d2c 2022 7879 7a22 3a20 5b35 2e32  .5], "xyz": [5.2
+00004160: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
+00004170: 2035 2e32 3436 3736 3930 3030 3030 3030   5.2467690000000
+00004180: 3030 352c 2033 2e34 3937 3834 365d 2c20  005, 3.497846], 
+00004190: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+000041a0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+000041b0: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+000041c0: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+000041d0: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+000041e0: 6263 223a 205b 302e 3235 2c20 302e 302c  bc": [0.25, 0.0,
+000041f0: 2030 2e32 355d 2c20 2278 797a 223a 205b   0.25], "xyz": [
+00004200: 312e 3734 3839 3233 2c20 302e 302c 2031  1.748923, 0.0, 1
+00004210: 2e37 3438 3932 335d 2c20 226c 6162 656c  .748923], "label
+00004220: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
+00004230: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
+00004240: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
+00004250: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
+00004260: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
+00004270: 302e 3235 2c20 302e 302c 2030 2e37 3530  0.25, 0.0, 0.750
+00004280: 3030 3030 3030 3030 3030 3030 315d 2c20  0000000000001], 
+00004290: 2278 797a 223a 205b 312e 3734 3839 3233  "xyz": [1.748923
+000042a0: 2c20 302e 302c 2035 2e32 3436 3736 3930  , 0.0, 5.2467690
+000042b0: 3030 3030 3030 3030 355d 2c20 226c 6162  000000005], "lab
+000042c0: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+000042d0: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+000042e0: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+000042f0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+00004300: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+00004310: 205b 302e 3235 2c20 302e 352c 2030 2e32   [0.25, 0.5, 0.2
+00004320: 355d 2c20 2278 797a 223a 205b 312e 3734  5], "xyz": [1.74
+00004330: 3839 3233 2c20 332e 3439 3738 3436 2c20  8923, 3.497846, 
+00004340: 312e 3734 3839 3233 5d2c 2022 6c61 6265  1.748923], "labe
+00004350: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+00004360: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00004370: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00004380: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00004390: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+000043a0: 5b30 2e32 352c 2030 2e35 2c20 302e 3735  [0.25, 0.5, 0.75
+000043b0: 3030 3030 3030 3030 3030 3030 3031 5d2c  00000000000001],
+000043c0: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
+000043d0: 332c 2033 2e34 3937 3834 362c 2035 2e32  3, 3.497846, 5.2
+000043e0: 3436 3736 3930 3030 3030 3030 3030 355d  467690000000005]
+000043f0: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+00004400: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+00004410: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+00004420: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+00004430: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+00004440: 2261 6263 223a 205b 302e 3735 3030 3030  "abc": [0.750000
+00004450: 3030 3030 3030 3030 3031 2c20 302e 302c  0000000001, 0.0,
+00004460: 2030 2e32 355d 2c20 2278 797a 223a 205b   0.25], "xyz": [
+00004470: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00004480: 3035 2c20 302e 302c 2031 2e37 3438 3932  05, 0.0, 1.74892
+00004490: 335d 2c20 226c 6162 656c 223a 2022 4e69  3], "label": "Ni
+000044a0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000044b0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000044c0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+000044d0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+000044e0: 2c20 2261 6263 223a 205b 302e 3735 3030  , "abc": [0.7500
+000044f0: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00004500: 302c 2030 2e37 3530 3030 3030 3030 3030  0, 0.75000000000
+00004510: 3030 3030 315d 2c20 2278 797a 223a 205b  00001], "xyz": [
+00004520: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00004530: 3035 2c20 302e 302c 2035 2e32 3436 3736  05, 0.0, 5.24676
+00004540: 3930 3030 3030 3030 3030 355d 2c20 226c  90000000005], "l
+00004550: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00004560: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00004570: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00004580: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00004590: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+000045a0: 223a 205b 302e 3735 3030 3030 3030 3030  ": [0.7500000000
+000045b0: 3030 3030 3031 2c20 302e 352c 2030 2e32  000001, 0.5, 0.2
+000045c0: 355d 2c20 2278 797a 223a 205b 352e 3234  5], "xyz": [5.24
+000045d0: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+000045e0: 332e 3439 3738 3436 2c20 312e 3734 3839  3.497846, 1.7489
+000045f0: 3233 5d2c 2022 6c61 6265 6c22 3a20 224e  23], "label": "N
+00004600: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00004610: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
+00004620: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
+00004630: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
+00004640: 5d2c 2022 6162 6322 3a20 5b30 2e37 3530  ], "abc": [0.750
+00004650: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
+00004660: 2e35 2c20 302e 3735 3030 3030 3030 3030  .5, 0.7500000000
+00004670: 3030 3030 3031 5d2c 2022 7879 7a22 3a20  000001], "xyz": 
+00004680: 5b35 2e32 3436 3736 3930 3030 3030 3030  [5.2467690000000
+00004690: 3030 352c 2033 2e34 3937 3834 362c 2035  005, 3.497846, 5
+000046a0: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
+000046b0: 355d 2c20 226c 6162 656c 223a 2022 4e69  5], "label": "Ni
+000046c0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000046d0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000046e0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+000046f0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00004700: 2c20 2261 6263 223a 205b 302e 302c 2030  , "abc": [0.0, 0
+00004710: 2e32 352c 2030 2e32 355d 2c20 2278 797a  .25, 0.25], "xyz
+00004720: 223a 205b 302e 302c 2031 2e37 3438 3932  ": [0.0, 1.74892
+00004730: 332c 2031 2e37 3438 3932 335d 2c20 226c  3, 1.748923], "l
+00004740: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00004750: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00004760: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00004770: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00004780: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00004790: 223a 205b 302e 302c 2030 2e32 352c 2030  ": [0.0, 0.25, 0
+000047a0: 2e37 3530 3030 3030 3030 3030 3030 3030  .750000000000000
+000047b0: 315d 2c20 2278 797a 223a 205b 302e 302c  1], "xyz": [0.0,
+000047c0: 2031 2e37 3438 3932 332c 2035 2e32 3436   1.748923, 5.246
+000047d0: 3736 3930 3030 3030 3030 3030 355d 2c20  7690000000005], 
+000047e0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
+000047f0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
+00004800: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
+00004810: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
+00004820: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
+00004830: 6263 223a 205b 302e 302c 2030 2e37 3530  bc": [0.0, 0.750
+00004840: 3030 3030 3030 3030 3030 3030 312c 2030  0000000000001, 0
+00004850: 2e32 355d 2c20 2278 797a 223a 205b 302e  .25], "xyz": [0.
+00004860: 302c 2035 2e32 3436 3736 3930 3030 3030  0, 5.24676900000
+00004870: 3030 3030 352c 2031 2e37 3438 3932 335d  00005, 1.748923]
+00004880: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+00004890: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+000048a0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+000048b0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+000048c0: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+000048d0: 2261 6263 223a 205b 302e 302c 2030 2e37  "abc": [0.0, 0.7
+000048e0: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+000048f0: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00004900: 3030 315d 2c20 2278 797a 223a 205b 302e  001], "xyz": [0.
+00004910: 302c 2035 2e32 3436 3736 3930 3030 3030  0, 5.24676900000
+00004920: 3030 3030 352c 2035 2e32 3436 3736 3930  00005, 5.2467690
+00004930: 3030 3030 3030 3030 355d 2c20 226c 6162  000000005], "lab
+00004940: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+00004950: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00004960: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+00004970: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+00004980: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+00004990: 205b 302e 352c 2030 2e32 352c 2030 2e32   [0.5, 0.25, 0.2
+000049a0: 355d 2c20 2278 797a 223a 205b 332e 3439  5], "xyz": [3.49
+000049b0: 3738 3436 2c20 312e 3734 3839 3233 2c20  7846, 1.748923, 
+000049c0: 312e 3734 3839 3233 5d2c 2022 6c61 6265  1.748923], "labe
+000049d0: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+000049e0: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+000049f0: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00004a00: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00004a10: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00004a20: 5b30 2e35 2c20 302e 3235 2c20 302e 3735  [0.5, 0.25, 0.75
+00004a30: 3030 3030 3030 3030 3030 3030 3031 5d2c  00000000000001],
+00004a40: 2022 7879 7a22 3a20 5b33 2e34 3937 3834   "xyz": [3.49784
+00004a50: 362c 2031 2e37 3438 3932 332c 2035 2e32  6, 1.748923, 5.2
+00004a60: 3436 3736 3930 3030 3030 3030 3030 355d  467690000000005]
+00004a70: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+00004a80: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+00004a90: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+00004aa0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+00004ab0: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+00004ac0: 2261 6263 223a 205b 302e 352c 2030 2e37  "abc": [0.5, 0.7
+00004ad0: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
+00004ae0: 2030 2e32 355d 2c20 2278 797a 223a 205b   0.25], "xyz": [
+00004af0: 332e 3439 3738 3436 2c20 352e 3234 3637  3.497846, 5.2467
+00004b00: 3639 3030 3030 3030 3030 3035 2c20 312e  690000000005, 1.
+00004b10: 3734 3839 3233 5d2c 2022 6c61 6265 6c22  748923], "label"
+00004b20: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00004b30: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00004b40: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00004b50: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00004b60: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00004b70: 2e35 2c20 302e 3735 3030 3030 3030 3030  .5, 0.7500000000
+00004b80: 3030 3030 3031 2c20 302e 3735 3030 3030  000001, 0.750000
+00004b90: 3030 3030 3030 3030 3031 5d2c 2022 7879  0000000001], "xy
+00004ba0: 7a22 3a20 5b33 2e34 3937 3834 362c 2035  z": [3.497846, 5
+00004bb0: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
+00004bc0: 352c 2035 2e32 3436 3736 3930 3030 3030  5, 5.24676900000
+00004bd0: 3030 3030 355d 2c20 226c 6162 656c 223a  00005], "label":
+00004be0: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
+00004bf0: 6573 223a 207b 7d7d 5d2c 2022 4076 6572  es": {}}], "@ver
+00004c00: 7369 6f6e 223a 206e 756c 6c7d fa17 556e  sion": null}..Un
+00004c10: 7265 636f 676e 697a 6564 2074 6573 7420  recognized test 
+00004c20: 6e61 6d65 2e4e 7a15 4b53 3230 3232 5f54  name.Nz.KS2022_T
+00004c30: 6573 7452 6573 756c 742e 6373 767a 0277  estResult.csvz.w
+00004c40: 2b63 0100 0000 0000 0000 0000 0000 0200  +c..............
+00004c50: 0000 0400 0000 5300 0000 7316 0000 0067  ......S...s....g
+00004c60: 007c 005d 0e7d 017c 019b 0064 009d 0291  .|.].}.|...d....
+00004c70: 0271 0453 0029 01da 010a 7224 0000 0029  .q.S.)....r$...)
+00004c80: 0272 2600 0000 da01 7672 2400 0000 7224  .r&.....vr$...r$
+00004c90: 0000 0072 2800 0000 7229 0000 0050 0100  ...r(...r)...P..
+00004ca0: 0072 2a00 0000 7a1b 7072 6f66 696c 652e  .r*...z.profile.
+00004cb0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00004cc0: 6d70 3efa 0544 6f6e 6521 2909 da05 7072  mp>..Done!)...pr
+00004cd0: 696e 7472 0200 0000 da09 6672 6f6d 5f64  intr......from_d
+00004ce0: 6963 74da 046a 736f 6eda 056c 6f61 6473  ict..json..loads
+00004cf0: 7205 0000 0072 b000 0000 da04 6f70 656e  r....r......open
+00004d00: da0a 7772 6974 656c 696e 6573 2907 da04  ..writelines)...
+00004d10: 7465 7374 da05 6e52 756e 73da 066d 6174  test..nRuns..mat
+00004d20: 5374 72da 0a73 7472 7563 744c 6973 7472  Str..structListr
+00004d30: 9900 0000 729a 0000 0072 9b00 0000 7224  ....r....r....r$
+00004d40: 0000 0072 2400 0000 7228 0000 00da 0770  ...r$...r(.....p
+00004d50: 726f 6669 6c65 4101 0000 731c 0000 0000  rofileA...s.....
+00004d60: 0208 0110 0106 0108 0110 0106 0208 0104  ................
+00004d70: 0116 010c 010a 010c 0132 0172 c700 0000  .........2.r....
+00004d80: e9e8 0300 0063 0200 0000 0000 0000 0000  .....c..........
+00004d90: 0000 0700 0000 0500 0000 4300 0000 7388  ..........C...s.
+00004da0: 0000 0064 0164 026c 006d 017d 0201 007c  ...d.d.l.m.}...|
+00004db0: 0064 036b 0272 2a74 0264 047c 019b 0064  .d.k.r*t.d.|...d
+00004dc0: 059d 0383 0101 0064 067d 036e 2a7c 0064  .......d.}.n*|.d
+00004dd0: 076b 0272 4874 0264 087c 019b 0064 059d  .k.rHt.d.|...d..
+00004de0: 0383 0101 0064 097d 036e 0c74 0264 0a83  .....d.}.n.t.d..
+00004df0: 0101 0064 0b53 0074 03a0 0474 05a0 067c  ...d.S.t...t...|
+00004e00: 03a1 01a1 017d 047c 0467 017c 0114 007d  .....}.|.g.|...}
+00004e10: 057c 0274 077c 0564 0c64 0d8d 037d 0674  .|.t.|.d.d...}.t
+00004e20: 0264 0e83 0101 0064 0b53 0029 0f7a 4550  .d.....d.S.).zEP
+00004e30: 726f 6669 6c65 7320 7468 6520 6465 7363  rofiles the desc
+00004e40: 7269 7074 6f72 2069 6e20 7061 7261 6c6c  riptor in parall
+00004e50: 656c 2075 7369 6e67 206f 6e65 206f 6620  el using one of 
+00004e60: 7468 6520 7465 7374 2073 7472 7563 7475  the test structu
+00004e70: 7265 732e 7201 0000 0029 01da 0b70 726f  res.r....)...pro
+00004e80: 6365 7373 5f6d 6170 72b3 0000 0072 b400  cess_mapr....r..
+00004e90: 0000 7a22 2074 696d 6573 2069 6e20 7061  ..z" times in pa
+00004ea0: 7261 6c6c 656c 2077 6974 6820 3820 776f  rallel with 8 wo
+00004eb0: 726b 6572 732e 72b5 0000 0072 b600 0000  rkers.r....r....
+00004ec0: 72b7 0000 0072 b800 0000 72b9 0000 004e  r....r....r....N
+00004ed0: 7289 0000 0029 01da 0b6d 6178 5f77 6f72  r....)...max_wor
+00004ee0: 6b65 7273 72bc 0000 0029 08da 1774 7164  kersr....)...tqd
+00004ef0: 6d2e 636f 6e74 7269 622e 636f 6e63 7572  m.contrib.concur
+00004f00: 7265 6e74 72c9 0000 0072 bd00 0000 7202  rentr....r....r.
+00004f10: 0000 0072 be00 0000 72bf 0000 0072 c000  ...r....r....r..
+00004f20: 0000 72b0 0000 0029 0772 c300 0000 72c4  ..r....).r....r.
+00004f30: 0000 0072 c900 0000 72c5 0000 0072 9900  ...r....r....r..
+00004f40: 0000 72c6 0000 00da 0864 6573 634c 6973  ..r......descLis
+00004f50: 7472 2400 0000 7224 0000 0072 2800 0000  tr$...r$...r(...
+00004f60: da0f 7072 6f66 696c 6550 6172 616c 6c65  ..profileParalle
+00004f70: 6c53 0100 0073 1a00 0000 0002 0c01 0801  lS...s..........
+00004f80: 1001 0601 0801 1001 0602 0801 0401 1002  ................
+00004f90: 0a01 0e01 72cd 0000 00da 085f 5f6d 6169  ....r......__mai
+00004fa0: 6e5f 5f29 0172 c300 0000 72b6 0000 0029  n__).r....r....)
+00004fb0: 0172 0100 0000 2902 72b3 0000 0072 1100  .r....).r....r..
+00004fc0: 0000 2902 72b3 0000 0072 c800 0000 2924  ..).r....r....)$
+00004fd0: 723a 0000 0072 bf00 0000 da05 6e75 6d70  r:...r......nump
+00004fe0: 7972 2f00 0000 da02 6f73 da0d 7079 6d61  yr/.....os..pyma
+00004ff0: 7467 656e 2e63 6f72 6572 0200 0000 7203  tgen.corer....r.
+00005000: 0000 005a 1b70 796d 6174 6765 6e2e 616e  ...Z.pymatgen.an
+00005010: 616c 7973 6973 2e6c 6f63 616c 5f65 6e76  alysis.local_env
+00005020: 7204 0000 0072 0500 0000 da06 7479 7069  r....r......typi
+00005030: 6e67 7206 0000 0072 b100 0000 5a13 7065  ngr....r....Z.pe
+00005040: 7269 6f64 6963 5f74 6162 6c65 5f73 697a  riodic_table_siz
+00005050: 65da 076c 6f61 6474 7874 da04 7061 7468  e..loadtxt..path
+00005060: da04 6a6f 696e da07 6469 726e 616d 65da  ..join..dirname.
+00005070: 085f 5f66 696c 655f 5f72 3100 0000 da0a  .__file__r1.....
+00005080: 6e61 6e5f 746f 5f6e 756d 725b 0000 0072  nan_to_numr[...r
+00005090: 4500 0000 7246 0000 0072 5f00 0000 72a9  E...rF...r_...r.
+000050a0: 0000 0072 7700 0000 7286 0000 00da 076e  ...rw...r......n
+000050b0: 6461 7272 6179 72b0 0000 00da 0373 7472  darrayr......str
+000050c0: 72b2 0000 0072 c700 0000 72cd 0000 0072  r....r....r....r
+000050d0: 4f00 0000 7224 0000 0072 2400 0000 7224  O...r$...r$...r$
+000050e0: 0000 0072 2800 0000 da08 3c6d 6f64 756c  ...r(.....<modul
+000050f0: 653e 0a00 0000 733c 0000 0008 0108 0108  e>....s<........
+00005100: 0108 0110 010c 010c 010c 0202 0302 fd04  ................
+00005110: 0804 0120 010a 0208 0106 ff06 030e 410e  ... ..........A.
+00005120: 1212 1814 460a 1412 5512 050a 120a 130a  ....F...U.......
+00005130: 010a 010a 010a 01                        .......
```

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/__pycache__/Ward2017.cpython-39.pyc` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/__pycache__/KS2022_dilute.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Thu Apr  6 16:22:26 2023 UTC, .py size: 32724 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,1291 +1,966 @@
-00000000: 610d 0d0a 0000 0000 c2f1 2e64 d47f 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 aff5 2e64 605d 0000  a..........d`]..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 5801 0000 6400  .....@...sX...d.
+00000020: 0006 0000 0040 0000 0073 3201 0000 6400  .....@...s2...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6401 6c04 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 6d07 5a07 0100 6400  d.l.m.Z.m.Z...d.
 00000060: 6403 6c08 6d09 5a09 0100 6400 6404 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0a 5a0a 0100 6400 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6406 6407 6702 5a0d 6408 5a0e 6503  ..d.d.g.Z.d.Z.e.
-00000090: 6a0f 6504 6a10 a011 6504 6a10 a012 6513  j.e.j...e.j...e.
-000000a0: a101 6409 a102 640a 640b 8d02 5a14 6503  ..d...d.d...Z.e.
-000000b0: a015 6514 a101 5a14 6514 6401 6401 8502  ..e...Z.e.d.d...
-000000c0: 6700 640c a201 6602 1900 5a14 6516 640d  g.d...f...Z.e.d.
-000000d0: 9c01 640e 640f 8404 5a17 4700 6410 6411  ..d.d...Z.G.d.d.
-000000e0: 8400 6411 8302 5a18 6517 6601 6506 6412  ..d...Z.e.f.e.d.
-000000f0: 9c01 6413 6414 8405 5a19 6506 650c 651a  ..d.d...Z.e.e.e.
-00000100: 1900 6415 9c02 6416 6417 8404 5a1b 6429  ..d...d.d...Z.d)
-00000110: 6418 6419 8401 5a1c 6506 6503 6a1d 641a  d.d...Z.e.e.j.d.
-00000120: 9c02 641b 641c 8404 5a1e 650c 651f 1900  ..d.d...Z.e.e...
-00000130: 640d 9c01 641d 641e 8404 5a20 642a 6421  d...d.d...Z d*d!
-00000140: 6422 8401 5a21 642b 6424 6425 8401 5a22  d"..Z!d+d$d%..Z"
-00000150: 6523 6426 6b02 9001 7254 6521 641f 6427  e#d&k...rTe!d.d'
-00000160: 8d01 0100 6521 6428 6427 8d01 0100 6522  ....e!d(d'....e"
-00000170: 641f 6427 8d01 0100 6522 6428 6427 8d01  d.d'....e"d(d'..
-00000180: 0100 6401 5300 292c e900 0000 004e 2902  ..d.S.),.....N).
-00000190: da09 5374 7275 6374 7572 65da 0745 6c65  ..Structure..Ele
-000001a0: 6d65 6e74 2901 da09 566f 726f 6e6f 694e  ment)...VoronoiN
-000001b0: 4e29 01da 0474 7164 6d29 01da 044c 6973  N)...tqdm)...Lis
-000001c0: 747a f541 6461 6d20 4d2e 204b 7261 6a65  tz.Adam M. Kraje
-000001d0: 7773 6b69 2c20 4a6f 6e61 7468 616e 2057  wski, Jonathan W
-000001e0: 2e20 5369 6567 656c 2c20 4a69 6e63 6861  . Siegel, Jincha
-000001f0: 6f20 5875 2c20 5a69 2d4b 7569 204c 6975  o Xu, Zi-Kui Liu
-00000200: 2c20 4578 7465 6e73 6962 6c65 2053 7472  , Extensible Str
-00000210: 7563 7475 7265 2d49 6e66 6f72 6d65 6420  ucture-Informed 
-00000220: 5072 6564 6963 7469 6f6e 206f 6620 466f  Prediction of Fo
-00000230: 726d 6174 696f 6e20 456e 6572 6779 2077  rmation Energy w
-00000240: 6974 6820 696d 7072 6f76 6564 2061 6363  ith improved acc
-00000250: 7572 6163 7920 616e 6420 7573 6162 696c  uracy and usabil
-00000260: 6974 7920 656d 706c 6f79 696e 6720 6e65  ity employing ne
-00000270: 7572 616c 206e 6574 776f 726b 732c 2043  ural networks, C
-00000280: 6f6d 7075 7461 7469 6f6e 616c 204d 6174  omputational Mat
-00000290: 6572 6961 6c73 2053 6369 656e 6365 2c20  erials Science, 
-000002a0: 566f 6c75 6d65 2032 3038 2c20 3230 3232  Volume 208, 2022
-000002b0: 2c20 3131 3132 3534 75f9 0000 004c 2e20  , 111254u....L. 
-000002c0: 5761 7264 2c20 522e 204c 6975 2c20 412e  Ward, R. Liu, A.
-000002d0: 204b 7269 7368 6e61 2c20 562e 2049 2e20   Krishna, V. I. 
-000002e0: 4865 6764 652c 2041 2e20 4167 7261 7761  Hegde, A. Agrawa
-000002f0: 6c2c 2041 2e20 4368 6f75 6468 6172 792c  l, A. Choudhary,
-00000300: 2061 6e64 2043 2e20 576f 6c76 6572 746f   and C. Wolverto
-00000310: 6e2c 20e2 809c 496e 636c 7564 696e 6720  n, ...Including 
-00000320: 6372 7973 7461 6c20 7374 7275 6374 7572  crystal structur
-00000330: 6520 6174 7472 6962 7574 6573 2069 6e20  e attributes in 
-00000340: 6d61 6368 696e 6520 6c65 6172 6e69 6e67  machine learning
-00000350: 206d 6f64 656c 7320 6f66 2066 6f72 6d61   models of forma
-00000360: 7469 6f6e 2065 6e65 7267 6965 7320 7669  tion energies vi
-00000370: 6120 566f 726f 6e6f 6920 7465 7373 656c  a Voronoi tessel
-00000380: 6c61 7469 6f6e 732c e280 9d20 5068 7973  lations,... Phys
-00000390: 6963 616c 2052 6576 6965 7720 422c 2076  ical Review B, v
-000003a0: 6f6c 2e20 3936 2c20 6e6f 2e20 322c 2037  ol. 96, no. 2, 7
-000003b0: 2032 3031 372e e970 0000 007a 1d4d 6167   2017..p...z.Mag
-000003c0: 7069 655f 656c 656d 656e 745f 7072 6f70  pie_element_prop
-000003d0: 6572 7469 6573 2e63 7376 fa01 2c29 01da  erties.csv..,)..
-000003e0: 0964 656c 696d 6974 6572 2916 e92d 0000  .delimiter)..-..
-000003f0: 00e9 2100 0000 e902 0000 00e9 2000 0000  ..!......... ...
-00000400: e905 0000 00e9 3000 0000 e906 0000 00e9  ......0.........
-00000410: 0a00 0000 e92c 0000 00e9 2a00 0000 e926  .....,....*....&
-00000420: 0000 00e9 2800 0000 e924 0000 00e9 2b00  ....(....$....+.
-00000430: 0000 e929 0000 00e9 2500 0000 e927 0000  ...)....%....'..
-00000440: 00e9 2300 0000 e912 0000 00e9 0d00 0000  ..#.............
-00000450: e911 0000 00e9 3200 0000 2901 da06 7265  ......2...)...re
-00000460: 7475 726e 6303 0000 0000 0000 0000 0000  turnc...........
-00000470: 001c 0000 0008 0000 0043 0000 0073 9202  .........C...s..
-00000480: 0000 7400 a001 7402 6a03 6401 1900 a101  ..t...t.j.d.....
-00000490: 7d03 7c01 6a04 a005 a100 a006 a100 4400  }.|.j.........D.
-000004a0: 5d2a 5c02 7d04 7d05 7c03 7c05 7402 7407  ]*\.}.}.|.|.t.t.
-000004b0: 7c04 8301 6a08 6401 1800 6402 6402 8502  |...j.d...d.d...
-000004c0: 6602 1900 1400 3700 7d03 711e 7400 a001  f.....7.}.q.t...
-000004d0: 7402 6a03 6401 1900 a101 7d06 6403 7d07  t.j.d.....}.d.}.
-000004e0: 6403 7d08 6404 6405 8400 7c00 a009 a100  d.}.d.d...|.....
-000004f0: 4400 8301 7d09 7c00 a006 a100 4400 5d88  D...}.|.....D.].
-00000500: 5c02 7d0a 7d0b 7400 a001 7402 6a03 6401  \.}.}.t...t.j.d.
-00000510: 1900 a101 7d0c 7c0b 6406 1900 6a04 a005  ....}.|.d...j...
-00000520: a100 a006 a100 4400 5d2a 5c02 7d04 7d05  ......D.]*\.}.}.
-00000530: 7c0c 7c05 7402 7407 7c04 8301 6a08 6401  |.|.t.t.|...j.d.
-00000540: 1800 6402 6402 8502 6602 1900 1400 3700  ..d.d...f.....7.
-00000550: 7d0c 71a6 7c06 7400 a00a 7c03 7c0c 1800  }.q.|.t...|.|...
-00000560: a101 7c0b 6407 1900 1400 3700 7d06 7c07  ..|.d.....7.}.|.
-00000570: 7c0b 6407 1900 3700 7d07 7c08 7c0b 6408  |.d...7.}.|.|.d.
-00000580: 1900 3700 7d08 717c 7c06 7c07 1b00 7c03  ..7.}.q||.|...|.
-00000590: 6702 7d0d 6403 7d0e 6403 7d0f 7c00 a009  g.}.d.}.d.}.|...
-000005a0: a100 4400 5d26 7d0b 7c0e 7c0b 6407 1900  ..D.]&}.|.|.d...
-000005b0: 3700 7d0e 7c0f 7c0b 6407 1900 7c0b 6407  7.}.|.|.d...|.d.
-000005c0: 1900 1400 3700 7d0f 9001 7122 7c0e 7c0e  ....7.}...q"|.|.
-000005d0: 1400 7c0f 1b00 7d10 6403 7d11 7c00 a009  ..|...}.d.}.|...
-000005e0: a100 4400 5d1e 7d0b 7c11 7c0b 6407 1900  ..D.].}.|.|.d...
-000005f0: 6409 1400 7c0b 640a 1900 1400 3700 7d11  d...|.d.....7.}.
-00000600: 9001 7162 7c11 7c07 1d00 7d11 6403 7d12  ..qb|.|...}.d.}.
-00000610: 7c00 a009 a100 4400 5d26 7d0b 7c12 7c0b  |.....D.]&}.|.|.
-00000620: 6407 1900 740a 6409 7c0b 640a 1900 1400  d...t.d.|.d.....
-00000630: 7c11 1800 8301 1400 3700 7d12 9001 7196  |.......7.}...q.
-00000640: 7c12 7c07 7c11 1400 1d00 7d12 6900 7d13  |.|.|.....}.i.}.
-00000650: 6403 7d14 6900 7d15 6403 7d16 6900 7d17  d.}.i.}.d.}.i.}.
-00000660: 6403 7d18 7c00 a009 a100 4400 5d54 7d19  d.}.|.....D.]T}.
-00000670: 7c14 7c19 6407 1900 3700 7d14 7c0b 6406  |.|.d...7.}.|.d.
-00000680: 1900 6a04 a005 a100 4400 5d32 7d04 7c04  ..j.....D.]2}.|.
-00000690: 7c13 7600 9002 722c 7c13 7c04 0500 1900  |.v...r,|.|.....
-000006a0: 7c19 6407 1900 3700 0300 3c00 6e0c 7c19  |.d...7...<.n.|.
-000006b0: 6407 1900 7c13 7c04 3c00 9002 7108 9001  d...|.|.<...q...
-000006c0: 71ea 740b 640b 640c 8400 7c00 a009 a100  q.t.d.d...|.....
-000006d0: 4400 8301 8301 7d1a 640d 740c 6a0d 1400  D.....}.d.t.j...
-000006e0: 740c a00e 7c1a 640e a102 1400 7d1b 7400  t...|.d.....}.t.
-000006f0: a00f 7c10 7c11 7c12 7c08 7c1b 6705 7c0d  ..|.|.|.|.|.g.|.
-00000700: 6403 1900 6602 a101 7c0d 6401 1900 7c09  d...f...|.d...|.
-00000710: 6703 5300 290f 618e 0100 0041 2070 726f  g.S.).a....A pro
-00000720: 746f 7479 7065 2066 756e 6374 696f 6e20  totype function 
-00000730: 7768 6963 6820 636f 6d70 7574 6573 2061  which computes a
-00000740: 2077 6569 6768 7465 6420 6176 6572 6167   weighted averag
-00000750: 6520 6f76 6572 206e 6569 6768 626f 7273  e over neighbors
-00000760: 2c20 7765 6967 6874 6564 2062 7920 7468  , weighted by th
-00000770: 6520 6172 6561 206f 6620 7468 6520 766f  e area of the vo
-00000780: 726f 6e6f 6920 6365 6c6c 0a20 2020 2062  ronoi cell.    b
-00000790: 6574 7765 656e 2074 6865 6d2e 0a0a 2020  etween them...  
-000007a0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000007b0: 6c6f 6361 6c5f 656e 763a 2041 2064 6963  local_env: A dic
-000007c0: 7469 6f6e 6172 7920 6f66 2074 6865 206c  tionary of the l
-000007d0: 6f63 616c 2065 6e76 6972 6f6e 6d65 6e74  ocal environment
-000007e0: 206f 6620 6120 7369 7465 2c20 6173 2072   of a site, as r
-000007f0: 6574 7572 6e65 6420 6279 2061 2056 6f72  eturned by a Vor
-00000800: 6f6e 6f69 4e4e 2067 656e 6572 6174 6f72  onoiNN generator
-00000810: 2e0a 2020 2020 2020 2020 7369 7465 3a20  ..        site: 
-00000820: 5468 6520 7369 7465 206e 756d 6265 7220  The site number 
-00000830: 666f 7220 7768 6963 6820 7468 6520 6c6f  for which the lo
-00000840: 6361 6c20 656e 7669 726f 6e6d 656e 7420  cal environment 
-00000850: 6973 2062 6569 6e67 2063 6f6d 7075 7465  is being compute
-00000860: 642e 0a0a 2020 2020 5265 7475 726e 733a  d...    Returns:
-00000870: 0a20 2020 2020 2020 2041 206c 6973 7420  .        A list 
-00000880: 6f66 2074 6865 206c 6f63 616c 2065 6e76  of the local env
-00000890: 6972 6f6e 6d65 6e74 2061 7474 7269 6275  ironment attribu
-000008a0: 7465 732e 0a20 2020 20e9 0100 0000 4e72  tes..    .....Nr
-000008b0: 0100 0000 6301 0000 0000 0000 0000 0000  ....c...........
-000008c0: 0002 0000 0005 0000 0053 0000 0073 1c00  .........S...s..
-000008d0: 0000 6700 7c00 5d14 7d01 7c01 6400 1900  ..g.|.].}.|.d...
-000008e0: 7c01 6401 1900 6702 9102 7104 5300 2902  |.d...g...q.S.).
-000008f0: da04 7369 7465 da04 6172 6561 a900 a902  ..site..area....
-00000900: da02 2e30 da05 7661 6c75 6572 2400 0000  ...0..valuer$...
-00000910: 7224 0000 00fa 512f 5573 6572 732f 6164  r$....Q/Users/ad
-00000920: 616d 2f50 7963 6861 726d 5072 6f6a 6563  am/PycharmProjec
-00000930: 7473 2f70 7953 4950 4645 4e4e 2f70 7973  ts/pySIPFENN/pys
-00000940: 6970 6665 6e6e 2f64 6573 6372 6970 746f  ipfenn/descripto
-00000950: 7244 6566 696e 6974 696f 6e73 2f57 6172  rDefinitions/War
-00000960: 6432 3031 372e 7079 da0a 3c6c 6973 7463  d2017.py..<listc
-00000970: 6f6d 703e 3400 0000 f300 0000 007a 266c  omp>4........z&l
-00000980: 6f63 616c 5f65 6e76 5f66 756e 6374 696f  ocal_env_functio
-00000990: 6e2e 3c6c 6f63 616c 733e 2e3c 6c69 7374  n.<locals>.<list
-000009a0: 636f 6d70 3e72 2200 0000 7223 0000 00da  comp>r"...r#....
-000009b0: 0676 6f6c 756d 6572 0c00 0000 da09 6661  .volumer......fa
-000009c0: 6365 5f64 6973 7463 0100 0000 0000 0000  ce_distc........
-000009d0: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
-000009e0: 7316 0000 007c 005d 0e7d 017c 0164 0019  s....|.].}.|.d..
-000009f0: 0056 0001 0071 0264 0153 0029 0272 2c00  .V...q.d.S.).r,.
-00000a00: 0000 4e72 2400 0000 2902 7226 0000 00da  ..Nr$...).r&....
-00000a10: 0d6e 6569 6768 626f 725f 7369 7465 7224  .neighbor_siter$
-00000a20: 0000 0072 2400 0000 7228 0000 00da 093c  ...r$...r(.....<
-00000a30: 6765 6e65 7870 723e 5c00 0000 722a 0000  genexpr>\...r*..
-00000a40: 007a 256c 6f63 616c 5f65 6e76 5f66 756e  .z%local_env_fun
-00000a50: 6374 696f 6e2e 3c6c 6f63 616c 733e 2e3c  ction.<locals>.<
-00000a60: 6765 6e65 7870 723e 6755 5555 5555 55f5  genexpr>gUUUUUU.
-00000a70: 3f67 0000 0000 0000 0840 2910 da02 6e70  ?g.......@)...np
-00000a80: da05 7a65 726f 73da 1061 7474 7269 6275  ..zeros..attribu
-00000a90: 7465 5f6d 6174 7269 78da 0573 6861 7065  te_matrix..shape
-00000aa0: da07 7370 6563 6965 73da 0f67 6574 5f65  ..species..get_e
-00000ab0: 6c5f 616d 745f 6469 6374 da05 6974 656d  l_amt_dict..item
-00000ac0: 7372 0300 0000 da01 5ada 0676 616c 7565  sr......Z..value
-00000ad0: 73da 0361 6273 da03 6d69 6eda 046d 6174  s..abs..min..mat
-00000ae0: 68da 0270 69da 0370 6f77 da0b 636f 6e63  h..pi..pow..conc
-00000af0: 6174 656e 6174 6529 1cda 096c 6f63 616c  atenate)...local
-00000b00: 5f65 6e76 7222 0000 00da 0c65 6c65 6d65  _envr".....eleme
-00000b10: 6e74 5f64 6963 745a 106c 6f63 616c 5f61  nt_dictZ.local_a
-00000b20: 7474 7269 6275 7465 73da 036b 6579 7227  ttributes..keyr'
-00000b30: 0000 005a 0f64 6966 665f 6174 7472 6962  ...Z.diff_attrib
-00000b40: 7574 6573 da0c 746f 7461 6c5f 7765 6967  utes..total_weig
-00000b50: 6874 722b 0000 005a 0d6e 6569 6768 626f  htr+...Z.neighbo
-00000b60: 725f 6c69 7374 da03 696e 6472 2d00 0000  r_list..indr-...
-00000b70: 5a13 6e65 6967 6862 6f72 5f61 7474 7269  Z.neighbor_attri
-00000b80: 6275 7465 735a 1f65 6c65 6d65 6e74 616c  butesZ.elemental
-00000b90: 5f70 726f 7065 7274 6965 735f 6174 7472  _properties_attr
-00000ba0: 6962 7574 6573 da07 6176 6572 6167 65da  ibutes..average.
-00000bb0: 0876 6172 6961 6e63 655a 0d65 6666 5f63  .varianceZ.eff_c
-00000bc0: 6f6f 7264 5f6e 756d 5a0c 626c 656e 5f61  oord_numZ.blen_a
-00000bd0: 7665 7261 6765 5a08 626c 656e 5f76 6172  verageZ.blen_var
-00000be0: 5a0b 7061 7468 5f64 6963 745f 315a 0e74  Z.path_dict_1Z.t
-00000bf0: 6f74 616c 5f77 6569 6768 745f 315a 0b70  otal_weight_1Z.p
-00000c00: 6174 685f 6469 6374 5f32 5a0e 746f 7461  ath_dict_2Z.tota
-00000c10: 6c5f 7765 6967 6874 5f32 5a0b 7061 7468  l_weight_2Z.path
-00000c20: 5f64 6963 745f 335a 0e74 6f74 616c 5f77  _dict_3Z.total_w
-00000c30: 6569 6768 745f 335a 0f6e 6569 6768 626f  eight_3Z.neighbo
-00000c40: 725f 7369 7465 5f31 5a0a 7370 6865 7265  r_site_1Z.sphere
-00000c50: 5f72 6164 5a0d 7370 6865 7265 5f76 6f6c  _radZ.sphere_vol
-00000c60: 756d 6572 2400 0000 7224 0000 0072 2800  umer$...r$...r(.
-00000c70: 0000 da12 6c6f 6361 6c5f 656e 765f 6675  ....local_env_fu
-00000c80: 6e63 7469 6f6e 2200 0000 7360 0000 0000  nction"...s`....
-00000c90: 0c10 0116 0124 0110 0104 0104 0112 0110  .....$..........
-00000ca0: 0110 011a 0124 011a 010c 010e 010c 0204  .....$..........
-00000cb0: 0104 010c 010c 0118 010c 0204 010c 011c  ................
-00000cc0: 0108 0104 010c 0124 010c 0204 0104 0104  .......$........
-00000cd0: 0104 0104 0104 010c 010c 0112 010a 0116  ................
-00000ce0: 0214 0216 0116 0104 0114 ff02 0208 fe72  ...............r
-00000cf0: 4500 0000 6300 0000 0000 0000 0000 0000  E...c...........
-00000d00: 0000 0000 0004 0000 0040 0000 0073 3200  .........@...s2.
-00000d10: 0000 6500 5a01 6400 5a02 6401 5a03 6504  ..e.Z.d.Z.d.Z.e.
-00000d20: 6402 6402 6403 8d02 6601 6404 6405 8401  d.d.d...f.d.d...
-00000d30: 5a05 6506 6406 9c01 6407 6408 8404 5a07  Z.e.d...d.d...Z.
-00000d40: 6409 5300 290a da17 4c6f 6361 6c41 7474  d.S.)...LocalAtt
-00000d50: 7269 6275 7465 4765 6e65 7261 746f 727a  ributeGeneratorz
-00000d60: b141 2077 7261 7070 6572 2063 6c61 7373  .A wrapper class
-00000d70: 2077 6869 6368 2063 6f6e 7461 696e 7320   which contains 
-00000d80: 616e 2069 6e73 7461 6e63 6520 6f66 2061  an instance of a
-00000d90: 6e20 4e4e 2067 656e 6572 6174 6f72 2028  n NN generator (
-00000da0: 7468 6520 6465 6661 756c 7420 6973 2061  the default is a
-00000db0: 2056 6f72 6f6e 6f69 4e4e 292c 2061 2073   VoronoiNN), a s
-00000dc0: 7472 7563 7475 7265 2c20 616e 640a 2020  tructure, and.  
-00000dd0: 2020 6120 6675 6e63 7469 6f6e 2077 6869    a function whi
-00000de0: 6368 2063 6f6d 7075 7465 7320 7468 6520  ch computes the 
-00000df0: 6c6f 6361 6c20 656e 7669 726f 6e6d 656e  local environmen
-00000e00: 7420 6174 7472 6962 7574 6573 2e0a 2020  t attributes..  
-00000e10: 2020 4629 025a 1563 6f6d 7075 7465 5f61    F).Z.compute_a
-00000e20: 646a 5f6e 6569 6768 626f 7273 5a0d 6578  dj_neighborsZ.ex
-00000e30: 7472 615f 6e6e 5f69 6e66 6f63 0500 0000  tra_nn_infoc....
-00000e40: 0000 0000 0000 0000 0500 0000 0200 0000  ................
-00000e50: 4300 0000 731c 0000 007c 047c 005f 007c  C...s....|.|._.|
-00000e60: 017c 005f 017c 027c 005f 027c 037c 005f  .|._.|.|._.|.|._
-00000e70: 0364 0053 00a9 014e 2904 da09 6765 6e65  .d.S...N)...gene
-00000e80: 7261 746f 72da 0673 7472 7563 74da 0866  rator..struct..f
-00000e90: 756e 6374 696f 6e72 3f00 0000 2905 da04  unctionr?...)...
-00000ea0: 7365 6c66 7249 0000 005a 0e6c 6f63 616c  selfrI...Z.local
-00000eb0: 5f65 6e76 5f66 756e 6372 3f00 0000 5a0c  _env_funcr?...Z.
-00000ec0: 6e6e 5f67 656e 6572 6174 6f72 7224 0000  nn_generatorr$..
-00000ed0: 0072 2400 0000 7228 0000 00da 085f 5f69  .r$...r(.....__i
-00000ee0: 6e69 745f 5f68 0000 0073 0800 0000 0002  nit__h...s......
-00000ef0: 0601 0601 0601 7a20 4c6f 6361 6c41 7474  ......z LocalAtt
-00000f00: 7269 6275 7465 4765 6e65 7261 746f 722e  ributeGenerator.
-00000f10: 5f5f 696e 6974 5f5f 2901 da01 6e63 0200  __init__)...nc..
-00000f20: 0000 0000 0000 0000 0000 0300 0000 0500  ................
-00000f30: 0000 4300 0000 7326 0000 007c 006a 00a0  ..C...s&...|.j..
-00000f40: 017c 006a 027c 01a1 027d 027c 00a0 037c  .|.j.|...}.|...|
-00000f50: 027c 006a 027c 0119 007c 006a 04a1 0353  .|.j.|...|.j...S
-00000f60: 0029 017a 4d47 656e 6572 6174 6573 2074  .).zMGenerates t
-00000f70: 6865 206c 6f63 616c 2065 6e76 6972 6f6e  he local environ
-00000f80: 6d65 6e74 2061 7474 7269 6275 7465 7320  ment attributes 
-00000f90: 666f 7220 6120 6769 7665 6e20 7369 7465  for a given site
-00000fa0: 2069 6e20 7468 6520 7374 7275 6374 7572   in the structur
-00000fb0: 652e 2905 7248 0000 005a 1567 6574 5f76  e.).rH...Z.get_v
-00000fc0: 6f72 6f6e 6f69 5f70 6f6c 7968 6564 7261  oronoi_polyhedra
-00000fd0: 7249 0000 0072 4a00 0000 723f 0000 0029  rI...rJ...r?...)
-00000fe0: 0372 4b00 0000 724d 0000 0072 3e00 0000  .rK...rM...r>...
-00000ff0: 7224 0000 0072 2400 0000 7228 0000 00da  r$...r$...r(....
-00001000: 1967 656e 6572 6174 655f 6c6f 6361 6c5f  .generate_local_
-00001010: 6174 7472 6962 7574 6573 6f00 0000 7304  attributeso...s.
-00001020: 0000 0000 0210 017a 314c 6f63 616c 4174  .......z1LocalAt
-00001030: 7472 6962 7574 6547 656e 6572 6174 6f72  tributeGenerator
-00001040: 2e67 656e 6572 6174 655f 6c6f 6361 6c5f  .generate_local_
-00001050: 6174 7472 6962 7574 6573 4e29 08da 085f  attributesN)..._
-00001060: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
-00001070: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
-00001080: 5fda 075f 5f64 6f63 5f5f 7204 0000 0072  _..__doc__r....r
-00001090: 4c00 0000 da03 696e 7472 4e00 0000 7224  L.....intrN...r$
-000010a0: 0000 0072 2400 0000 7224 0000 0072 2800  ...r$...r$...r(.
-000010b0: 0000 7246 0000 0063 0000 0073 0800 0000  ..rF...c...s....
-000010c0: 0801 0405 0aff 0a07 7246 0000 0029 0172  ........rF...).r
-000010d0: 4900 0000 6302 0000 0000 0000 0000 0000  I...c...........
-000010e0: 0008 0000 0008 0000 0043 0000 0073 be00  .........C...s..
-000010f0: 0000 6900 7d02 7c00 6a00 4400 5d50 7d03  ..i.}.|.j.D.]P}.
-00001100: 7c03 a001 a100 a002 a100 4400 5d3e 5c02  |.........D.]>\.
-00001110: 7d04 7d05 7c04 7c02 7600 7246 7c02 7c04  }.}.|.|.v.rF|.|.
-00001120: 0500 1900 7c05 7403 7c00 6a00 8301 1b00  ....|.t.|.j.....
-00001130: 3700 0300 3c00 711a 7c05 7403 7c00 6a00  7...<.q.|.t.|.j.
-00001140: 8301 1b00 7c02 7c04 3c00 711a 710a 7404  ....|.|.<.q.q.t.
-00001150: 7c00 7c01 7c02 8303 7d06 7405 7c06 6a06  |.|.|...}.t.|.j.
-00001160: 7407 7403 7c00 6a08 8301 8301 8302 7d07  t.t.|.j.......}.
-00001170: 7409 7c07 8301 7d07 740a a00b 6401 6402  t.|...}.t...d.d.
-00001180: 8400 7c07 4400 8301 a101 740a a00b 6403  ..|.D.....t...d.
-00001190: 6402 8400 7c07 4400 8301 a101 6404 6405  d...|.D.....d.d.
-000011a0: 8400 740c 7c07 8301 4400 8301 6603 5300  ..t.|...D...f.S.
-000011b0: 2906 616c 0100 0047 656e 6572 6174 6573  ).al...Generates
-000011c0: 2074 6865 206c 6f63 616c 2065 6e76 6972   the local envir
-000011d0: 6f6e 6d65 6e74 2061 7474 7269 6275 7465  onment attribute
-000011e0: 7320 666f 7220 6120 6769 7665 6e20 7374  s for a given st
-000011f0: 7275 6374 7572 6520 7573 696e 6720 6120  ructure using a 
-00001200: 566f 726f 6e6f 694e 4e20 6765 6e65 7261  VoronoiNN genera
-00001210: 746f 722e 200a 2020 2020 2020 2054 6865  tor. .       The
-00001220: 206c 6f63 616c 2065 6e76 6972 6f6e 6d65   local environme
-00001230: 6e74 2061 7474 7269 6275 7465 7320 636f  nt attributes co
-00001240: 6e73 6973 7420 6f66 2061 7665 7261 6765  nsist of average
-00001250: 7320 6f76 6572 2074 6865 206e 6569 6768  s over the neigh
-00001260: 626f 7273 206f 6620 6561 6368 2073 6974  bors of each sit
-00001270: 6520 696e 2074 6865 2073 7472 7563 7475  e in the structu
-00001280: 7265 2e0a 0a20 2020 2041 7267 733a 0a20  re...    Args:. 
-00001290: 2020 2020 2020 2073 7472 7563 743a 2041         struct: A
-000012a0: 2070 796d 6174 6765 6e20 5374 7275 6374   pymatgen Struct
-000012b0: 7572 6520 6f62 6a65 6374 2e0a 2020 2020  ure object..    
-000012c0: 2020 2020 6c6f 6361 6c5f 6675 6e63 743a      local_funct:
-000012d0: 2041 2066 756e 6374 696f 6e20 7768 6963   A function whic
-000012e0: 6820 636f 6d70 7574 6573 2074 6865 206c  h computes the l
-000012f0: 6f63 616c 2065 6e76 6972 6f6e 6d65 6e74  ocal environment
-00001300: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
-00001310: 6120 6769 7665 6e20 7369 7465 2e0a 0a20  a given site... 
-00001320: 2020 2063 0100 0000 0000 0000 0000 0000     c............
-00001330: 0200 0000 0400 0000 5300 0000 7314 0000  ........S...s...
-00001340: 0067 007c 005d 0c7d 017c 0164 0019 0091  .g.|.].}.|.d....
-00001350: 0271 0453 0029 0172 0100 0000 7224 0000  .q.S.).r....r$..
-00001360: 0072 2500 0000 7224 0000 0072 2400 0000  .r%...r$...r$...
-00001370: 7228 0000 0072 2900 0000 8900 0000 722a  r(...r).......r*
-00001380: 0000 007a 2f67 656e 6572 6174 655f 766f  ...z/generate_vo
-00001390: 726f 6e6f 695f 6174 7472 6962 7574 6573  ronoi_attributes
-000013a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-000013b0: 6f6d 703e 6301 0000 0000 0000 0000 0000  omp>c...........
-000013c0: 0002 0000 0004 0000 0053 0000 0073 1400  .........S...s..
-000013d0: 0000 6700 7c00 5d0c 7d01 7c01 6400 1900  ..g.|.].}.|.d...
-000013e0: 9102 7104 5300 2901 7221 0000 0072 2400  ..q.S.).r!...r$.
-000013f0: 0000 7225 0000 0072 2400 0000 7224 0000  ..r%...r$...r$..
-00001400: 0072 2800 0000 7229 0000 0089 0000 0072  .r(...r).......r
-00001410: 2a00 0000 6301 0000 0000 0000 0000 0000  *...c...........
-00001420: 0003 0000 0005 0000 0053 0000 0073 1a00  .........S...s..
-00001430: 0000 6900 7c00 5d12 5c02 7d01 7d02 7c01  ..i.|.].\.}.}.|.
-00001440: 7c02 6400 1900 9302 7104 5300 2901 720c  |.d.....q.S.).r.
-00001450: 0000 0072 2400 0000 2903 7226 0000 00da  ...r$...).r&....
-00001460: 0169 7227 0000 0072 2400 0000 7224 0000  .ir'...r$...r$..
-00001470: 0072 2800 0000 da0a 3c64 6963 7463 6f6d  .r(.....<dictcom
-00001480: 703e 8900 0000 7302 0000 0006 017a 2f67  p>....s......z/g
-00001490: 656e 6572 6174 655f 766f 726f 6e6f 695f  enerate_voronoi_
-000014a0: 6174 7472 6962 7574 6573 2e3c 6c6f 6361  attributes.<loca
-000014b0: 6c73 3e2e 3c64 6963 7463 6f6d 703e 290d  ls>.<dictcomp>).
-000014c0: da10 7370 6563 6965 735f 616e 645f 6f63  ..species_and_oc
-000014d0: 6375 7234 0000 0072 3500 0000 da03 6c65  cur4...r5.....le
-000014e0: 6e72 4600 0000 da03 6d61 7072 4e00 0000  nrF.....maprN...
-000014f0: da05 7261 6e67 65da 0573 6974 6573 da04  ..range..sites..
-00001500: 6c69 7374 722f 0000 00da 0561 7272 6179  listr/.....array
-00001510: da09 656e 756d 6572 6174 6529 0872 4900  ..enumerate).rI.
-00001520: 0000 5a0b 6c6f 6361 6c5f 6675 6e63 7472  ..Z.local_functr
-00001530: 3f00 0000 da0b 636f 6d70 6f73 6974 696f  ?.....compositio
-00001540: 6e72 4000 0000 7227 0000 005a 0f6c 6f63  nr@...r'...Z.loc
-00001550: 616c 5f67 656e 6572 6174 6f72 5a0e 6174  al_generatorZ.at
-00001560: 7472 6962 7574 655f 6c69 7374 7224 0000  tribute_listr$..
-00001570: 0072 2400 0000 7228 0000 00da 1b67 656e  .r$...r(.....gen
-00001580: 6572 6174 655f 766f 726f 6e6f 695f 6174  erate_voronoi_at
-00001590: 7472 6962 7574 6573 7500 0000 7318 0000  tributesu...s...
-000015a0: 0000 0a04 010a 0114 0108 011c 0216 010c  ................
-000015b0: 0116 0108 012a 0106 ff72 5f00 0000 2902  .....*...r_...).
-000015c0: da04 7374 7263 7220 0000 0063 0300 0000  ..strcr ...c....
-000015d0: 0000 0000 0000 0000 1700 0000 0b00 0000  ................
-000015e0: 0300 0000 7390 0200 0074 007c 006a 0183  ....s....t.|.j..
-000015f0: 0164 016b 0272 1864 0267 017c 0214 0053  .d.k.r.d.g.|...S
-00001600: 0067 0089 007c 0044 005d 127d 0388 00a0  .g...|.D.].}....
-00001610: 027c 03a0 03a1 00a1 0101 0071 2087 0066  .|.........q ..f
-00001620: 0164 0364 0484 087c 01a0 04a1 0044 0083  .d.d...|.....D..
-00001630: 017d 0474 057c 006a 016a 066a 07a0 04a1  .}.t.|.j.j.j....
-00001640: 008e 005c 027d 057d 0667 007d 0764 0564  ...\.}.}.g.}.d.d
-00001650: 0484 0074 0874 007c 0083 0183 0144 0083  ...t.t.|.....D..
-00001660: 017d 0874 087c 0283 0144 0090 025d 067d  .}.t.|...D...].}
-00001670: 0974 09a0 0a74 007c 0083 0174 007c 0583  .t...t.|...t.|..
-00001680: 0166 02a1 017d 0a74 0874 007c 0083 0183  .f...}.t.t.|....
-00001690: 0144 0090 015d c87d 0b7c 087c 0b19 007d  .D...].}.|.|...}
-000016a0: 0c69 007c 087c 0b3c 007c 0ca0 04a1 0044  .i.|.|.<.|.....D
-000016b0: 0090 015d 7e5c 027d 0d7d 0e7c 0d64 0219  ...]~\.}.}.|.d..
-000016c0: 007d 0f7c 0d64 0119 007d 107c 0d64 0619  .}.|.d...}.|.d..
-000016d0: 007d 1164 027d 1264 077d 137c 047c 1019  .}.d.}.d.}.|.|..
-000016e0: 0044 005d 407d 147c 1464 0219 007c 0f6b  .D.]@}.|.d...|.k
-000016f0: 0390 0173 2874 0b7c 1464 0119 007c 1118  ...s(t.|.d...|..
-00001700: 0083 0164 086b 0490 0173 287c 1390 0172  ...d.k...s(|...r
-00001710: 367c 127c 1464 0119 0037 007d 1271 fa64  6|.|.d...7.}.q.d
-00001720: 097d 1371 fa64 077d 137c 047c 1019 0044  .}.q.d.}.|.|...D
-00001730: 005d fe7d 147c 1464 0219 007c 0f6b 0390  .].}.|.d...|.k..
-00001740: 0173 7674 0b7c 1464 0119 007c 1118 0083  .svt.|.d...|....
-00001750: 0164 086b 0490 0173 767c 1390 0272 407c  .d.k...sv|...r@|
-00001760: 007c 1464 0219 0019 006a 0ca0 04a1 0044  .|.d.....j.....D
-00001770: 005d 345c 027d 157d 167c 0a7c 0b7c 05a0  .]4\.}.}.|.|.|..
-00001780: 0d7c 15a1 0166 0205 0019 007c 167c 1464  .|...f.....|.|.d
-00001790: 0119 0014 007c 0e14 007c 121b 0037 0003  .....|...|...7..
-000017a0: 003c 0090 0171 887c 097c 0264 0118 006b  .<...q.|.|.d...k
-000017b0: 0090 0272 447c 107c 1464 0219 007c 1464  ...rD|.|.d...|.d
-000017c0: 0119 0066 037c 087c 0b19 0076 0090 0272  ...f.|.|...v...r
-000017d0: 187c 087c 0b19 007c 107c 1464 0219 007c  .|.|...|.|.d...|
-000017e0: 1464 0119 0066 0305 0019 007c 1464 0119  .d...f.....|.d..
-000017f0: 007c 0e14 007c 121b 0037 0003 003c 006e  .|...|...7...<.n
-00001800: 267c 1464 0119 007c 0e14 007c 121b 007c  &|.d...|...|...|
-00001810: 087c 0b19 007c 107c 1464 0219 007c 1464  .|...|.|.d...|.d
-00001820: 0119 0066 033c 006e 0464 097d 1390 0171  ...f.<.n.d.}...q
-00001830: 4871 c864 017c 0a7c 0b64 0a64 0a85 0266  Hq.d.|.|.d.d...f
-00001840: 0219 0074 09a0 0e7c 06a1 011b 0018 007c  ...t...|.......|
-00001850: 0a7c 0b64 0a64 0a85 0266 023c 0071 aa7c  .|.d.d...f.<.q.|
-00001860: 07a0 0274 09a0 0b7c 0aa1 01a0 0fa1 00a1  ...t...|........
-00001870: 0101 0071 827c 0753 0029 0b61 c001 0000  ...q.|.S.).a....
-00001880: 4765 6e65 7261 7465 7320 7468 6520 5743  Generates the WC
-00001890: 2061 7474 7269 6275 7465 7320 666f 7220   attributes for 
-000018a0: 6120 6769 7665 6e20 7374 7275 6374 7572  a given structur
-000018b0: 652e 2054 6865 2057 4320 6174 7472 6962  e. The WC attrib
-000018c0: 7574 6573 2061 7265 2074 6865 206f 7264  utes are the ord
-000018d0: 6572 696e 6720 7061 7261 6d65 7465 7273  ering parameters
-000018e0: 2066 6f72 2065 6163 680a 2020 2020 7368   for each.    sh
-000018f0: 656c 6c20 6f66 2074 6865 2056 6f72 6f6e  ell of the Voron
-00001900: 6f69 2074 6573 7365 6c6c 6174 696f 6e2e  oi tessellation.
-00001910: 2053 6c69 6768 746c 7920 6469 6666 6572   Slightly differ
-00001920: 656e 7420 7468 616e 2077 6861 7420 6973  ent than what is
-00001930: 2069 6d70 6c65 6d65 6e74 6564 2062 7920   implemented by 
-00001940: 5761 7264 2d57 6f6c 7665 7274 6f6e 2e20  Ward-Wolverton. 
-00001950: 4f6e 6c79 2063 6f6e 7369 6465 7273 0a20  Only considers. 
-00001960: 2020 2069 6d6d 6564 6961 7465 2062 6163     immediate bac
-00001970: 6b74 7261 636b 696e 672e 0a0a 2020 2020  ktracking...    
-00001980: 4172 6773 3a0a 2020 2020 2020 2020 7374  Args:.        st
-00001990: 7263 3a20 4120 7079 6d61 7467 656e 2053  rc: A pymatgen S
-000019a0: 7472 7563 7475 7265 206f 626a 6563 742e  tructure object.
-000019b0: 0a20 2020 2020 2020 206e 6569 6768 626f  .        neighbo
-000019c0: 725f 6469 6374 5f72 6177 3a20 4120 6469  r_dict_raw: A di
-000019d0: 6374 696f 6e61 7279 206f 6620 7468 6520  ctionary of the 
-000019e0: 6e65 6967 6862 6f72 7320 6f66 2065 6163  neighbors of eac
-000019f0: 6820 7369 7465 2069 6e20 7468 6520 7374  h site in the st
-00001a00: 7275 6374 7572 652e 0a20 2020 2020 2020  ructure..       
-00001a10: 206c 6576 656c 733a 2054 6865 206e 756d   levels: The num
-00001a20: 6265 7220 6f66 2073 6865 6c6c 7320 746f  ber of shells to
-00001a30: 2063 6f6e 7369 6465 722e 0a0a 2020 2020   consider...    
-00001a40: 7221 0000 0072 0100 0000 6301 0000 0000  r!...r....c.....
-00001a50: 0000 0000 0000 0003 0000 0006 0000 0013  ................
-00001a60: 0000 0073 2400 0000 6900 7c00 5d1c 5c02  ...s$...i.|.].\.
-00001a70: 7d01 7d02 7c01 8700 6601 6400 6401 8408  }.}.|...f.d.d...
-00001a80: 7c02 4400 8301 9302 7104 5300 2902 6301  |.D.....q.S.).c.
-00001a90: 0000 0000 0000 0000 0000 0002 0000 0006  ................
-00001aa0: 0000 0013 0000 0073 2600 0000 6700 7c00  .......s&...g.|.
-00001ab0: 5d1e 7d01 8800 a000 7c01 6400 1900 a001  ].}.....|.d.....
-00001ac0: a100 a101 7c01 6401 1900 6702 9102 7104  ....|.d...g...q.
-00001ad0: 5300 2902 7201 0000 0072 2100 0000 2902  S.).r....r!...).
-00001ae0: da05 696e 6465 78da 0c74 6f5f 756e 6974  ..index..to_unit
-00001af0: 5f63 656c 6c72 2500 0000 a901 5a0e 7374  _cellr%.....Z.st
-00001b00: 7263 5f75 6e69 745f 6365 6c6c 7224 0000  rc_unit_cellr$..
-00001b10: 0072 2800 0000 7229 0000 009e 0000 0072  .r(...r).......r
-00001b20: 2a00 0000 7a35 6765 6e65 7261 7465 5f57  *...z5generate_W
-00001b30: 435f 6174 7472 6962 7574 6573 2e3c 6c6f  C_attributes.<lo
-00001b40: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
-00001b50: 2e3c 6c69 7374 636f 6d70 3e72 2400 0000  .<listcomp>r$...
-00001b60: 2903 7226 0000 0072 4000 0000 5a07 7370  ).r&...r@...Z.sp
-00001b70: 5f6c 6973 7472 6300 0000 7224 0000 0072  _listrc...r$...r
-00001b80: 2800 0000 7255 0000 009e 0000 0073 0400  (...rU.......s..
-00001b90: 0000 0601 06ff 7a2a 6765 6e65 7261 7465  ......z*generate
-00001ba0: 5f57 435f 6174 7472 6962 7574 6573 2e3c  _WC_attributes.<
-00001bb0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
-00001bc0: 703e 6301 0000 0000 0000 0000 0000 0002  p>c.............
-00001bd0: 0000 0006 0000 0053 0000 0073 1c00 0000  .......S...s....
-00001be0: 6900 7c00 5d14 7d01 7c01 7c01 7c01 6400  i.|.].}.|.|.|.d.
-00001bf0: 6603 6401 6901 9302 7104 5300 2902 6700  f.d.i...q.S.).g.
-00001c00: 0000 0000 0000 00e7 0000 0000 0000 f03f  ...............?
-00001c10: 7224 0000 0029 0272 2600 0000 7254 0000  r$...).r&...rT..
-00001c20: 0072 2400 0000 7224 0000 0072 2800 0000  .r$...r$...r(...
-00001c30: 7255 0000 00a7 0000 0072 2a00 0000 720c  rU.......r*...r.
-00001c40: 0000 0046 6795 d626 e80b 2e11 3e54 4e29  ...Fg..&....>TN)
-00001c50: 1072 5700 0000 725e 0000 00da 0661 7070  .rW...r^.....app
-00001c60: 656e 6472 6200 0000 7235 0000 00da 037a  endrb...r5.....z
-00001c70: 6970 da13 656c 656d 656e 745f 636f 6d70  ip..element_comp
-00001c80: 6f73 6974 696f 6eda 1666 7261 6374 696f  osition..fractio
-00001c90: 6e61 6c5f 636f 6d70 6f73 6974 696f 6e72  nal_compositionr
-00001ca0: 5900 0000 722f 0000 0072 3000 0000 7238  Y...r/...r0...r8
-00001cb0: 0000 0072 3300 0000 7261 0000 0072 5c00  ...r3...ra...r\.
-00001cc0: 0000 da04 6d65 616e 2917 7260 0000 005a  ....mean).r`...Z
-00001cd0: 116e 6569 6768 626f 725f 6469 6374 5f72  .neighbor_dict_r
-00001ce0: 6177 da06 6c65 7665 6c73 da03 706f 73da  aw..levels..pos.
-00001cf0: 0d6e 6569 6768 626f 725f 6469 6374 da05  .neighbor_dict..
-00001d00: 656c 656d 735a 0566 7261 6373 da06 6f75  elemsZ.fracs..ou
-00001d10: 7470 7574 5a0e 7265 6163 6861 626c 655f  tputZ.reachable_
-00001d20: 696e 6473 da05 7368 656c 6c5a 086f 7264  inds..shellZ.ord
-00001d30: 6572 696e 675a 0873 6974 655f 6964 785a  eringZ.site_idxZ
-00001d40: 0672 5f69 6e64 73da 0469 6478 73da 0677  .r_inds..idxs..w
-00001d50: 6569 6768 74da 0570 5f69 6478 da03 6964  eight..p_idx..id
-00001d60: 785a 0966 6163 655f 6172 6561 5a14 7765  xZ.face_areaZ.we
-00001d70: 6967 6874 5f6e 6f72 6d61 6c69 7a61 7469  ight_normalizati
-00001d80: 6f6e da07 736b 6970 7065 64da 056e 5f69  on..skipped..n_i
-00001d90: 6478 7240 0000 0072 2700 0000 7224 0000  dxr@...r'...r$..
-00001da0: 0072 6300 0000 7228 0000 00da 1667 656e  .rc...r(.....gen
-00001db0: 6572 6174 655f 5743 5f61 7474 7269 6275  erate_WC_attribu
-00001dc0: 7465 738d 0000 0073 5800 0000 000b 0e01  tes....sX.......
-00001dd0: 0a02 0401 0801 1001 0a01 06ff 0604 0201  ................
-00001de0: 0cff 0804 0401 1601 0e02 1603 1201 0801  ................
-00001df0: 0801 1201 0801 0801 0801 0401 0401 0c01  ................
-00001e00: 2a01 0e02 0601 0401 0c01 2a01 1a01 2e01  *.........*.....
-00001e10: 0e01 1c01 1a01 0eff 0804 0eff 1a03 0a03  ................
-00001e20: 2c03 1602 7276 0000 0063 0200 0000 0000  ,...rv...c......
-00001e30: 0000 0000 0000 0a00 0000 0700 0000 4300  ..............C.
-00001e40: 0000 73d4 0000 0074 00a0 0174 00a0 027c  ..s....t...t...|
-00001e50: 0064 0164 0185 0264 0266 0219 00a1 01a1  .d.d...d.f......
-00001e60: 017d 0264 027d 0367 007d 047c 0244 005d  .}.d.}.g.}.|.D.]
-00001e70: 627d 057c 0064 0164 0185 0264 0266 0219  b}.|.d.d...d.f..
-00001e80: 007c 056b 027d 0674 00a0 0374 00a0 047c  .|.k.}.t...t...|
-00001e90: 067c 01a1 027c 01a1 0264 0219 007d 077c  .|...|...d...}.|
-00001ea0: 077c 036b 0472 787c 04a0 05a1 0001 007c  .|.k.rx|.......|
-00001eb0: 04a0 067c 05a1 0101 007c 077d 0371 287c  ...|.....|.}.q(|
-00001ec0: 077c 036b 0272 287c 04a0 067c 05a1 0101  .|.k.r(|...|....
-00001ed0: 0071 2874 00a0 077c 0064 0264 0164 0185  .q(t...|.d.d.d..
-00001ee0: 0266 0219 00a1 017d 087c 0444 005d 207d  .f.....}.|.D.] }
-00001ef0: 097c 0874 0874 097c 0983 0164 0318 0064  .|.t.t.|...d...d
-00001f00: 0164 0185 0266 0219 0037 007d 0871 a67c  .d...f...7.}.q.|
-00001f10: 0874 0a7c 0483 011b 0053 0029 047a 4443  .t.|.....S.).zDC
-00001f20: 616c 6375 6c61 7465 7320 7468 6520 6174  alculates the at
-00001f30: 7472 6962 7574 6573 2063 6f72 7265 7370  tributes corresp
-00001f40: 6f6e 6469 6e67 2074 6f20 7468 6520 6d6f  onding to the mo
-00001f50: 7374 2063 6f6d 6d6f 6e20 656c 656d 656e  st common elemen
-00001f60: 7473 2e4e 7201 0000 0072 2100 0000 290b  ts.Nr....r!...).
-00001f70: 722f 0000 00da 0675 6e69 7175 65da 0572  r/.....unique..r
-00001f80: 6176 656c da0b 6578 7061 6e64 5f64 696d  avel..expand_dim
-00001f90: 73da 0373 756d da05 636c 6561 7272 6500  s..sum..clearre.
-00001fa0: 0000 da0a 7a65 726f 735f 6c69 6b65 7231  ....zeros_liker1
-00001fb0: 0000 0072 5300 0000 7257 0000 0029 0ada  ...rS...rW...)..
-00001fc0: 1461 7474 7269 6275 7465 5f70 726f 7065  .attribute_prope
-00001fd0: 7274 6965 73da 0461 7869 73da 0673 636f  rties..axis..sco
-00001fe0: 7265 735a 0e6d 6178 5f6f 6363 7572 7265  resZ.max_occurre
-00001ff0: 6e63 655a 0c74 6f70 5f65 6c65 6d65 6e74  nceZ.top_element
-00002000: 73da 0573 636f 7265 da08 7465 6d70 6c61  s..score..templa
-00002010: 7465 da05 636f 756e 7472 6e00 0000 da04  te..countrn.....
-00002020: 656c 656d 7224 0000 0072 2400 0000 7228  elemr$...r$...r(
-00002030: 0000 00da 0b6d 6167 7069 655f 6d6f 6465  .....magpie_mode
-00002040: d300 0000 7320 0000 0000 021c 0104 0104  ....s ..........
-00002050: 0108 0114 0118 0108 0108 010a 0106 0108  ................
-00002060: 010c 0116 0108 011e 0172 8400 0000 2902  .........r....).
-00002070: 7249 0000 0072 2000 0000 6301 0000 0000  rI...r ...c.....
-00002080: 0000 0000 0000 0019 0000 000e 0000 0003  ................
-00002090: 0000 0073 2c04 0000 7400 7c00 8301 5c03  ...s,...t.|...\.
-000020a0: 7d01 7d02 7d03 7401 a002 7401 6a03 7401  }.}.}.t...t.j.t.
-000020b0: 6a04 7c01 6401 6402 8d02 7401 6a04 7401  j.|.d.d...t.j.t.
-000020c0: a005 7c01 7401 6a04 7c01 6401 6402 8d02  ..|.t.j.|.d.d...
-000020d0: 1800 a101 6401 6402 8d02 7401 6a06 7c01  ....d.d...t.j.|.
-000020e0: 6401 6402 8d02 7401 6a07 7c01 6401 6402  d.d...t.j.|.d.d.
-000020f0: 8d02 7401 6a07 7c01 6401 6402 8d02 7401  ..t.j.|.d.d...t.
-00002100: 6a06 7c01 6401 6402 8d02 1800 6605 6403  j.|.d.d.....f.d.
-00002110: 6402 8d02 a008 6403 a101 7401 6a03 7401  d.....d...t.j.t.
-00002120: 6a04 7c02 6401 6402 8d02 7401 6a07 7c02  j.|.d.d...t.j.|.
-00002130: 6401 6402 8d02 7401 6a06 7c02 6401 6402  d.d...t.j.|.d.d.
-00002140: 8d02 1800 7401 6a04 7401 a005 7c02 7401  ....t.j.t...|.t.
-00002150: 6a04 7c02 6401 6402 8d02 1800 a101 6401  j.|.d.d.......d.
-00002160: 6402 8d02 7401 6a07 7c02 6401 6402 8d02  d...t.j.|.d.d...
-00002170: 7401 6a06 7c02 6401 6402 8d02 7409 7c02  t.j.|.d.d...t.|.
-00002180: 8301 6606 6403 6402 8d02 a008 6403 a101  ..f.d.d.....d...
-00002190: 6602 a101 7d04 7c04 6404 0500 1900 7c04  f...}.|.d.....|.
-000021a0: 6405 1900 1d00 0300 3c00 7c04 6406 0500  d.......<.|.d...
-000021b0: 1900 7c04 6405 1900 1d00 0300 3c00 7c04  ..|.d.......<.|.
-000021c0: 6407 0500 1900 7c04 6405 1900 1d00 0300  d.....|.d.......
-000021d0: 3c00 7c04 6408 0500 1900 7c04 6409 1900  <.|.d.....|.d...
-000021e0: 1d00 0300 3c00 7401 a00a 7c04 6700 640a  ....<.t...|.g.d.
-000021f0: a201 a102 7d04 7c04 640b 0500 1900 740b  ....}.|.d.....t.
-00002200: 7c02 8301 7c00 6a0c 1b00 3900 0300 3c00  |...|.j...9...<.
-00002210: 740d 7c00 7c03 640c 8303 7d05 740e 7c05  t.|.|.d...}.t.|.
-00002220: 8301 4400 5d14 7d06 7401 a00f 7c04 640b  ..D.].}.t...|.d.
-00002230: 7c06 a103 7d04 9001 718c 6900 7d07 7c00  |...}...q.i.}.|.
-00002240: 6a10 4400 5d56 7d08 7c08 a011 a100 a012  j.D.]V}.|.......
-00002250: a100 4400 5d42 5c02 7d09 7d0a 7c09 7c07  ..D.]B\.}.}.|.|.
-00002260: 7600 9001 72ea 7c07 7c09 0500 1900 7c0a  v...r.|.|.....|.
-00002270: 740b 7c00 6a10 8301 1b00 3700 0300 3c00  t.|.j.....7...<.
-00002280: 6e12 7c0a 740b 7c00 6a10 8301 1b00 7c07  n.|.t.|.j.....|.
-00002290: 7c09 3c00 9001 71bc 9001 71ac 640d 7d0b  |.<...q...q.d.}.
-000022a0: 640e 4400 5d36 8900 7401 a00f 7c04 7c0b  d.D.]6..t...|.|.
-000022b0: 7413 a014 7415 8700 6601 640f 6410 8408  t...t...f.d.d...
-000022c0: 7c07 a016 a100 4400 8301 8301 6411 8800  |.....D.....d...
-000022d0: 1b00 a102 a103 7d04 9002 710c 7401 a00f  ......}...q.t...
-000022e0: 7c04 7c0b 740b 7c07 8301 a103 7d04 6401  |.|.t.|.....}.d.
-000022f0: 6401 6401 6401 6412 9c04 7d0c 6401 7d0d  d.d.d.d...}.d.}.
-00002300: 7c07 a012 a100 4400 5da2 5c02 7d09 7d0a  |.....D.].\.}.}.
-00002310: 7c0c 6413 0500 1900 7c0a 7417 7418 7c09  |.d.....|.t.t.|.
-00002320: 8301 6a19 6414 1800 1900 6407 1900 1400  ..j.d.....d.....
-00002330: 3700 0300 3c00 7c0c 6415 0500 1900 7c0a  7...<.|.d.....|.
-00002340: 7417 7418 7c09 8301 6a19 6414 1800 1900  t.t.|...j.d.....
-00002350: 6416 1900 1400 3700 0300 3c00 7c0c 6417  d.....7...<.|.d.
-00002360: 0500 1900 7c0a 7417 7418 7c09 8301 6a19  ....|.t.t.|...j.
-00002370: 6414 1800 1900 6418 1900 1400 3700 0300  d.....d.....7...
-00002380: 3c00 7c0c 6419 0500 1900 7c0a 7417 7418  <.|.d.....|.t.t.
-00002390: 7c09 8301 6a19 6414 1800 1900 641a 1900  |...j.d.....d...
-000023a0: 1400 3700 0300 3c00 9002 7170 7415 641b  ..7...<...qpt.d.
-000023b0: 641c 8400 7c0c a012 a100 4400 8301 8301  d...|.....D.....
-000023c0: 7d0d 6412 4400 5d1a 7d0e 7401 a01a 7c04  }.d.D.].}.t...|.
-000023d0: 7c0c 7c0e 1900 7c0d 1b00 a102 7d04 9003  |.|...|.....}...
-000023e0: 712e 6401 7d0f 6401 7d10 641d 7d11 641e  q.d.}.d.}.d.}.d.
-000023f0: 7d12 7c00 6a1b a01c a100 6a1d 4400 5d26  }.|.j.....j.D.]&
-00002400: 7d13 7c13 6a1e 6401 6b04 9003 727a 641e  }.|.j.d.k...rzd.
-00002410: 7d11 7c13 6a1e 6401 6b00 9003 7266 641e  }.|.j.d.k...rfd.
-00002420: 7d12 9003 7166 7c07 a012 a100 4400 5d62  }...qf|.....D.]b
-00002430: 5c02 7d14 7d15 7c07 a012 a100 4400 5d4e  \.}.}.|.....D.]N
-00002440: 5c02 7d16 7d17 6411 7413 a01f 641f 7418  \.}.}.d.t...d.t.
-00002450: 7c14 8301 6a20 7418 7c16 8301 6a20 1800  |...j t.|...j ..
-00002460: 6420 1300 1400 a101 1800 7d18 7c18 7c0f  d ........}.|.|.
-00002470: 6b04 9003 72e2 7c18 7d0f 7c10 7c18 7c15  k...r.|.}.|.|.|.
-00002480: 1400 7c17 1400 3700 7d10 9003 71a6 9003  ..|...7.}...q...
-00002490: 7196 7401 a01a 7c04 7421 7c11 9004 6f0a  q.t...|.t!|...o.
-000024a0: 7c12 8301 a102 7d04 7401 a01a 7c04 7c0f  |.....}.t...|.|.
-000024b0: a102 7d04 7401 a01a 7c04 7c10 a102 7d04  ..}.t...|.|...}.
-000024c0: 7c04 5300 2921 7acb 4d61 696e 2066 756e  |.S.)!z.Main fun
-000024d0: 6374 696f 6e61 6c69 7479 2e20 4765 6e65  ctionality. Gene
-000024e0: 7261 7465 7320 7468 6520 5761 7264 3230  rates the Ward20
-000024f0: 3137 2064 6573 6372 6970 746f 7220 666f  17 descriptor fo
-00002500: 7220 6120 6769 7665 6e20 7374 7275 6374  r a given struct
-00002510: 7572 652e 0a0a 2020 2020 4172 6773 3a0a  ure...    Args:.
-00002520: 2020 2020 2020 2020 7374 7275 6374 3a20          struct: 
-00002530: 4120 7079 6d61 7467 656e 2053 7472 7563  A pymatgen Struc
-00002540: 7475 7265 206f 626a 6563 742e 0a0a 2020  ture object...  
-00002550: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00002560: 2020 2041 2032 3731 2d6c 656e 6768 7420     A 271-lenght 
-00002570: 6e75 6d70 7920 6172 7261 7920 6f66 2074  numpy array of t
-00002580: 6865 2064 6573 6372 6970 746f 722e 0a20  he descriptor.. 
-00002590: 2020 2072 0100 0000 2901 727e 0000 00e9     r....).r~....
-000025a0: ffff ffff 7210 0000 0072 0e00 0000 e907  ....r....r......
-000025b0: 0000 00e9 0800 0000 e910 0000 00e9 0f00  ................
-000025c0: 0000 290c e904 0000 0072 0e00 0000 e909  ..)......r......
-000025d0: 0000 00e9 0e00 0000 7289 0000 0072 1e00  ........r....r..
-000025e0: 0000 721c 0000 00e9 1300 0000 e915 0000  ..r.............
-000025f0: 00e9 1600 0000 e917 0000 00e9 1800 0000  ................
-00002600: e90c 0000 00e9 0300 0000 e97e 0000 0029  ...........~...)
-00002610: 0572 1100 0000 7286 0000 0072 0e00 0000  .r....r....r....
-00002620: 7293 0000 0072 0c00 0000 6301 0000 0000  r....r....c.....
-00002630: 0000 0000 0000 0002 0000 0005 0000 0033  ...............3
-00002640: 0000 0073 1a00 0000 7c00 5d12 7d01 7400  ...s....|.].}.t.
-00002650: a001 7c01 8800 a102 5600 0100 7102 6400  ..|.....V...q.d.
-00002660: 5300 7247 0000 0029 0272 3a00 0000 723c  S.rG...).r:...r<
-00002670: 0000 0072 2500 0000 a901 da01 7072 2400  ...r%.......pr$.
-00002680: 0000 7228 0000 0072 2e00 0000 1901 0000  ..r(...r........
-00002690: 722a 0000 007a 2667 656e 6572 6174 655f  r*...z&generate_
-000026a0: 6465 7363 7269 7074 6f72 2e3c 6c6f 6361  descriptor.<loca
-000026b0: 6c73 3e2e 3c67 656e 6578 7072 3e72 6400  ls>.<genexpr>rd.
-000026c0: 0000 2904 da01 7372 9600 0000 da01 64da  ..)...sr......d.
-000026d0: 0166 7297 0000 0072 2100 0000 7296 0000  .fr....r!...r...
-000026e0: 0072 8b00 0000 7298 0000 0072 1100 0000  .r....r....r....
-000026f0: 7299 0000 00e9 0b00 0000 6301 0000 0000  r.........c.....
-00002700: 0000 0000 0000 0003 0000 0004 0000 0053  ...............S
-00002710: 0000 0073 1400 0000 6700 7c00 5d0c 5c02  ...s....g.|.].\.
-00002720: 7d01 7d02 7c02 9102 7104 5300 7224 0000  }.}.|...q.S.r$..
-00002730: 0072 2400 0000 2903 7226 0000 0072 4000  .r$...).r&...r@.
-00002740: 0000 da03 7661 6c72 2400 0000 7224 0000  ....valr$...r$..
-00002750: 0072 2800 0000 7229 0000 0023 0100 0072  .r(...r)...#...r
-00002760: 2a00 0000 7a27 6765 6e65 7261 7465 5f64  *...z'generate_d
-00002770: 6573 6372 6970 746f 722e 3c6c 6f63 616c  escriptor.<local
-00002780: 733e 2e3c 6c69 7374 636f 6d70 3e46 5467  s>.<listcomp>FTg
-00002790: 0000 0000 0000 d0bf 720c 0000 0029 2272  ........r....)"r
-000027a0: 5f00 0000 722f 0000 0072 3d00 0000 da05  _...r/...r=.....
-000027b0: 7374 6163 6b72 6900 0000 7238 0000 0072  stackri...r8...r
-000027c0: 3900 0000 da03 6d61 78da 0772 6573 6861  9.....max..resha
-000027d0: 7065 7284 0000 00da 0664 656c 6574 6572  per......deleter
-000027e0: 5700 0000 722b 0000 0072 7600 0000 da08  W...r+...rv.....
-000027f0: 7265 7665 7273 6564 da06 696e 7365 7274  reversed..insert
-00002800: 7256 0000 0072 3400 0000 7235 0000 0072  rV...r4...r5...r
-00002810: 3a00 0000 723c 0000 0072 7a00 0000 7237  :...r<...rz...r7
-00002820: 0000 0072 3100 0000 7203 0000 0072 3600  ...r1...r....r6.
-00002830: 0000 7265 0000 0072 5e00 0000 da22 6164  ..re...r^...."ad
-00002840: 645f 6368 6172 6765 735f 6672 6f6d 5f6f  d_charges_from_o
-00002850: 7869 5f73 7461 7465 5f67 7565 7373 6573  xi_state_guesses
-00002860: da08 656c 656d 656e 7473 da09 6f78 695f  ..elements..oxi_
-00002870: 7374 6174 65da 0365 7870 da01 58da 0566  state..exp..X..f
-00002880: 6c6f 6174 2919 7249 0000 005a 0f64 6966  loat).rI...Z.dif
-00002890: 665f 7072 6f70 6572 7469 6573 727d 0000  f_propertiesr}..
-000028a0: 0072 6c00 0000 da0a 7072 6f70 6572 7469  .rl.....properti
-000028b0: 6573 5a0d 7763 5f61 7474 7269 6275 7465  esZ.wc_attribute
-000028c0: 73da 0961 7474 7269 6275 7465 723f 0000  s..attributer?..
-000028d0: 0072 5e00 0000 7240 0000 0072 2700 0000  .r^...r@...r'...
-000028e0: da08 706f 7369 7469 6f6e 5a18 656c 6563  ..positionZ.elec
-000028f0: 7472 6f6e 5f6f 6363 7570 6174 696f 6e5f  tron_occupation_
-00002900: 6469 6374 5a14 746f 7461 6c5f 7661 6c65  dictZ.total_vale
-00002910: 6e63 655f 6661 6374 6f72 5a03 6f72 625a  nce_factorZ.orbZ
-00002920: 0e6d 6178 5f69 6f6e 6963 5f63 6861 725a  .max_ionic_charZ
-00002930: 0d61 765f 696f 6e69 635f 6368 6172 5a0a  .av_ionic_charZ.
-00002940: 6861 735f 616e 696f 6e73 5a0b 6861 735f  has_anionsZ.has_
-00002950: 6361 7469 6f6e 73da 0265 6cda 046b 6579  cations..el..key
-00002960: 315a 0676 616c 7565 31da 046b 6579 325a  1Z.value1..key2Z
-00002970: 0676 616c 7565 325a 0a69 6f6e 6963 5f63  .value2Z.ionic_c
-00002980: 6861 7272 2400 0000 7295 0000 0072 2800  harr$...r....r(.
-00002990: 0000 da13 6765 6e65 7261 7465 5f64 6573  ....generate_des
-000029a0: 6372 6970 746f 72e7 0000 0073 a000 0000  criptor....s....
-000029b0: 0009 0e01 1401 2001 0c01 0c01 0c01 0cff  ...... .........
-000029c0: 02fc 0205 02fb 0605 02fb 0206 1001 0c01  ................
-000029d0: 0cff 0202 1a01 02ff 0402 0c01 0c01 06f9  ................
-000029e0: 0207 02f9 0607 02f9 02fa 060f 1401 1401  ................
-000029f0: 1402 1402 1002 1a02 0c01 0c01 1202 0401  ................
-00002a00: 0a01 1401 0a01 1c02 1a01 0401 0801 0601  ................
-00002a10: 0201 24fe 0803 1202 0e01 0401 1001 2601  ..$...........&.
-00002a20: 2601 2601 2a01 1601 0801 1802 0401 0401  &.&.*...........
-00002a30: 0401 0401 1001 0c01 0401 0c01 0801 1001  ................
-00002a40: 1001 2601 0a01 0401 1801 1601 0c01 0c01  ..&.............
-00002a50: 72ae 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00002a60: 0000 0000 0000 0100 0000 4300 0000 7304  ..........C...s.
-00002a70: 0000 0074 0053 0029 017a 1e43 6974 6174  ...t.S.).z.Citat
-00002a80: 696f 6e2f 7320 666f 7220 7468 6520 6465  ion/s for the de
-00002a90: 7363 7269 7074 6f72 2e29 01da 0963 6974  scriptor.)...cit
-00002aa0: 6174 696f 6e73 7224 0000 0072 2400 0000  ationsr$...r$...
-00002ab0: 7224 0000 0072 2800 0000 da04 6369 7465  r$...r(.....cite
-00002ac0: 3c01 0000 7302 0000 0000 0272 b000 0000  <...s......r....
-00002ad0: fa0b 4a56 4153 502d 3130 3030 3172 1100  ..JVASP-10001r..
-00002ae0: 0000 6302 0000 0000 0000 0000 0000 0007  ..c.............
-00002af0: 0000 0008 0000 0043 0000 0073 ae00 0000  .......C...s....
-00002b00: 7c00 6401 6b02 7216 7400 6402 8301 0100  |.d.k.r.t.d.....
-00002b10: 6403 7d02 6e22 7c00 6404 6b02 722c 7400  d.}.n"|.d.k.r,t.
-00002b20: 6405 8301 0100 6406 7d02 6e0c 7400 6407  d.....d.}.n.t.d.
-00002b30: 8301 0100 6408 5300 7401 a002 7403 a004  ....d.S.t...t...
-00002b40: 7c02 a101 a101 6701 7c01 1400 7d03 7405  |.....g.|...}.t.
-00002b50: 7c03 8301 4400 5d0c 7d04 7406 7c04 8301  |...D.].}.t.|...
-00002b60: 7d05 7156 7407 6409 640a 8302 8f24 7d06  }.qVt.d.d....$}.
-00002b70: 7c06 a008 640b 640c 8400 7c05 4400 8301  |...d.d...|.D...
-00002b80: a101 0100 5700 6408 0400 0400 8303 0100  ....W.d.........
-00002b90: 6e10 3100 7398 3000 0100 0100 0100 5900  n.1.s.0.......Y.
-00002ba0: 0100 7400 640d 8301 0100 6408 5300 290e  ..t.d.....d.S.).
-00002bb0: 7a43 5072 6f66 696c 6573 2074 6865 2064  zCProfiles the d
-00002bc0: 6573 6372 6970 746f 7220 696e 2073 6572  escriptor in ser
-00002bd0: 6965 7320 7573 696e 6720 6f6e 6520 6f66  ies using one of
-00002be0: 2074 6865 2074 6573 7420 7374 7275 6374   the test struct
-00002bf0: 7572 6573 2e72 b100 0000 7a54 5072 6f66  ures.r....zTProf
-00002c00: 696c 696e 672f 7465 7374 696e 6720 7461  iling/testing ta
-00002c10: 736b 2e20 5769 6c6c 2063 616c 6375 6c61  sk. Will calcula
-00002c20: 7465 2061 2064 6573 6372 6970 746f 7220  te a descriptor 
-00002c30: 666f 7220 4c69 3220 5a72 3120 5465 3120  for Li2 Zr1 Te1 
-00002c40: 4f36 2028 4a56 4153 502d 3130 3030 3129  O6 (JVASP-10001)
-00002c50: e146 0a00 007b 2240 6d6f 6475 6c65 223a  .F...{"@module":
-00002c60: 2022 7079 6d61 7467 656e 2e63 6f72 652e   "pymatgen.core.
-00002c70: 7374 7275 6374 7572 6522 2c20 2240 636c  structure", "@cl
-00002c80: 6173 7322 3a20 2253 7472 7563 7475 7265  ass": "Structure
-00002c90: 222c 2022 6368 6172 6765 223a 206e 756c  ", "charge": nul
-00002ca0: 6c2c 2022 6c61 7474 6963 6522 3a20 7b22  l, "lattice": {"
-00002cb0: 6d61 7472 6978 223a 205b 5b34 2e35 3939  matrix": [[4.599
-00002cc0: 3330 3536 3532 3636 3234 3539 2c20 302e  305652662459, 0.
-00002cd0: 3030 3938 3031 3530 3736 3939 3838 3233  0098015076998823
-00002ce0: 2c20 332e 3130 3532 3631 3238 3635 3434  , 3.105261286544
-00002cf0: 3337 3336 5d2c 205b 312e 3635 3533 3235  3736], [1.655325
-00002d00: 3737 3236 3230 3436 3533 2c20 342e 3239  7726204653, 4.29
-00002d10: 3131 3038 3437 3538 3534 3731 322c 2033  1108475854712, 3
-00002d20: 2e31 3035 3236 3032 3933 3839 3739 3536  .105260293897956
-00002d30: 355d 2c20 5b30 2e30 3134 3235 3431 3231  5], [0.014254121
-00002d40: 3439 3139 3734 392c 2030 2e30 3039 3830  4919749, 0.00980
-00002d50: 3235 3039 3939 3936 3133 312c 2035 2e35  25099996131, 5.5
-00002d60: 3439 3431 3931 3431 3836 3633 3531 5d5d  49419141866351]]
-00002d70: 2c20 2261 223a 2035 2e35 3439 3434 3634  , "a": 5.5494464
-00002d80: 3738 3135 3233 3236 2c20 2262 223a 2035  78152326, "b": 5
-00002d90: 2e35 3439 3434 3635 3336 3137 3933 3433  .549446536179343
-00002da0: 2c20 2263 223a 2035 2e35 3439 3434 3631  , "c": 5.5494461
-00002db0: 3035 3831 3034 3233 2c20 2261 6c70 6861  05810423, "alpha
-00002dc0: 223a 2035 352e 3832 3731 3434 3539 3938  ": 55.8271445998
-00002dd0: 3538 3332 2c20 2262 6574 6122 3a20 3535  5832, "beta": 55
-00002de0: 2e38 3237 3134 3031 3432 3839 3337 312c  .82714014289371,
-00002df0: 2022 6761 6d6d 6122 3a20 3535 2e38 3237   "gamma": 55.827
-00002e00: 3133 3937 3237 3739 3039 322c 2022 766f  13972779092, "vo
-00002e10: 6c75 6d65 223a 2031 3039 2e31 3534 3834  lume": 109.15484
-00002e20: 3632 3536 3432 3734 337d 2c20 2273 6974  625642743}, "sit
-00002e30: 6573 223a 205b 7b22 7370 6563 6965 7322  es": [{"species"
-00002e40: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00002e50: 4c69 222c 2022 6f63 6375 223a 2031 2e30  Li", "occu": 1.0
-00002e60: 7d5d 2c20 2261 6263 223a 205b 302e 3237  }], "abc": [0.27
-00002e70: 3338 3738 3438 3732 3636 3939 3234 2c20  38784872669924, 
-00002e80: 302e 3237 3338 3738 3438 3732 3637 3034  0.27387848726704
-00002e90: 3037 2c20 302e 3237 3338 3738 3438 3732  07, 0.2738784872
-00002ea0: 3637 3330 3332 5d2c 2022 7879 7a22 3a20  673032], "xyz": 
-00002eb0: 5b31 2e37 3136 3931 3238 3930 3430 3037  [1.7169128904007
-00002ec0: 3036 332c 2031 2e31 3830 3631 3134 3136  063, 1.180611416
-00002ed0: 3737 3737 3631 332c 2033 2e32 3230 3739  7777613, 3.22079
-00002ee0: 3437 3735 3337 3732 3738 5d2c 2022 6c61  4775377278], "la
-00002ef0: 6265 6c22 3a20 224c 6922 2c20 2270 726f  bel": "Li", "pro
-00002f00: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00002f10: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00002f20: 656d 656e 7422 3a20 224c 6922 2c20 226f  ement": "Li", "o
-00002f30: 6363 7522 3a20 312e 307d 5d2c 2022 6162  ccu": 1.0}], "ab
-00002f40: 6322 3a20 5b30 2e37 3835 3232 3732 3031  c": [0.785227201
-00002f50: 3037 3238 3036 392c 2030 2e37 3835 3232  0728069, 0.78522
-00002f60: 3732 3031 3037 3238 3835 362c 2030 2e37  72010728856, 0.7
-00002f70: 3835 3232 3732 3031 3037 3333 3135 5d2c  85227201073315],
-00002f80: 2022 7879 7a22 3a20 5b34 2e39 3232 3439   "xyz": [4.92249
-00002f90: 3934 3531 3733 3939 3635 2c20 332e 3338  9451739965, 3.38
-00002fa0: 3438 3838 3730 3539 3433 3439 3237 2c20  48887059434927, 
-00002fb0: 392e 3233 3432 3235 3333 3831 3633 3633  9.23422533816363
-00002fc0: 335d 2c20 226c 6162 656c 223a 2022 4c69  3], "label": "Li
-00002fd0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00002fe0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00002ff0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00003000: 4f22 2c20 226f 6363 7522 3a20 312e 307d  O", "occu": 1.0}
-00003010: 5d2c 2022 6162 6322 3a20 5b30 2e38 3636  ], "abc": [0.866
-00003020: 3939 3634 3435 3436 3631 3132 342c 2030  9964454661124, 0
-00003030: 2e36 3034 3038 3938 3832 3039 3231 3134  .604089882092114
-00003040: 2c20 302e 3234 3138 3231 3736 3938 3733  , 0.241821769873
-00003050: 3134 335d 2c20 2278 797a 223a 205b 342e  143], "xyz": [4.
-00003060: 3939 3039 3934 3136 3031 3634 3036 312c  990994160164061,
-00003070: 2032 2e36 3033 3038 3335 3435 3837 3638   2.6030835458768
-00003080: 3536 2c20 352e 3931 3030 3737 3138 3131  56, 5.9100771811
-00003090: 3337 3635 385d 2c20 226c 6162 656c 223a  37658], "label":
-000030a0: 2022 4f22 2c20 2270 726f 7065 7274 6965   "O", "propertie
-000030b0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-000030c0: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-000030d0: 3a20 224f 222c 2022 6f63 6375 223a 2031  : "O", "occu": 1
-000030e0: 2e30 7d5d 2c20 2261 6263 223a 205b 302e  .0}], "abc": [0.
-000030f0: 3731 3738 3430 3839 3435 3239 3738 382c  717840894529788,
-00003100: 2030 2e31 3231 3336 3735 3838 3936 3238   0.1213675889628
-00003110: 3638 332c 2030 2e33 3933 3533 3730 3039  683, 0.393537009
-00003120: 3138 3639 3733 5d2c 2022 7879 7a22 3a20  186973], "xyz": 
-00003130: 5b33 2e35 3038 3038 3231 3036 3233 3437  [3.5080821062347
-00003140: 3133 2c20 302e 3533 3136 3935 3036 3332  13, 0.5316950632
-00003150: 3135 3431 322c 2034 2e37 3839 3836 3333  15412, 4.7898633
-00003160: 3036 3436 3932 3738 5d2c 2022 6c61 6265  06469278], "labe
-00003170: 6c22 3a20 224f 222c 2022 7072 6f70 6572  l": "O", "proper
-00003180: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003190: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000031a0: 6e74 223a 2022 4f22 2c20 226f 6363 7522  nt": "O", "occu"
-000031b0: 3a20 312e 307d 5d2c 2022 6162 6322 3a20  : 1.0}], "abc": 
-000031c0: 5b30 2e31 3231 3336 3735 3838 3936 3338  [0.1213675889638
-000031d0: 3430 322c 2030 2e33 3933 3533 3730 3039  402, 0.393537009
-000031e0: 3138 3733 3934 332c 2030 2e37 3137 3834  1873943, 0.71784
-000031f0: 3038 3934 3532 3833 3338 345d 2c20 2278  08945283384], "x
-00003200: 797a 223a 205b 312e 3231 3938 3730 3738  yz": [1.21987078
-00003210: 3330 3831 3738 3936 2c20 312e 3639 3639  30817896, 1.6969
-00003220: 3336 3232 3335 3931 3033 3137 2c20 352e  362235910317, 5.
-00003230: 3538 3235 3132 3932 3531 3639 3634 5d2c  58251292516964],
-00003240: 2022 6c61 6265 6c22 3a20 224f 222c 2022   "label": "O", "
-00003250: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
-00003260: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
-00003270: 2265 6c65 6d65 6e74 223a 2022 4f22 2c20  "element": "O", 
-00003280: 226f 6363 7522 3a20 312e 307d 5d2c 2022  "occu": 1.0}], "
-00003290: 6162 6322 3a20 5b30 2e33 3933 3533 3730  abc": [0.3935370
-000032a0: 3039 3138 3631 3931 352c 2030 2e37 3137  091861915, 0.717
-000032b0: 3834 3038 3934 3532 3933 3835 362c 2030  8408945293856, 0
-000032c0: 2e31 3231 3336 3735 3838 3936 3334 3031  .121367588963401
-000032d0: 345d 2c20 2278 797a 223a 205b 322e 3939  4], "xyz": [2.99
-000032e0: 3939 3837 3531 3235 3935 3632 322c 2033  9987512595622, 3
-000032f0: 2e30 3835 3338 3031 3039 3836 3033 3434  .085380109860344
-00003300: 2c20 342e 3132 3436 3337 3638 3739 3632  , 4.124637687962
-00003310: 3239 375d 2c20 226c 6162 656c 223a 2022  297], "label": "
-00003320: 4f22 2c20 2270 726f 7065 7274 6965 7322  O", "properties"
-00003330: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003340: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003350: 224f 222c 2022 6f63 6375 223a 2031 2e30  "O", "occu": 1.0
-00003360: 7d5d 2c20 2261 6263 223a 205b 302e 3234  }], "abc": [0.24
-00003370: 3138 3231 3736 3938 3732 3135 3733 2c20  18217698721573, 
-00003380: 302e 3836 3639 3936 3434 3534 3637 3132  0.86699644546712
-00003390: 3231 2c20 302e 3630 3430 3839 3838 3230  21, 0.6040898820
-000033a0: 3932 3135 3133 5d2c 2022 7879 7a22 3a20  921513], "xyz": 
-000033b0: 5b32 2e35 3535 3938 3435 3634 3633 3333  [2.5559845646333
-000033c0: 3239 2c20 332e 3732 3836 3637 3631 3037  29, 3.7286676107
-000033d0: 3239 3134 392c 2036 2e37 3935 3531 3733  29149, 6.7955173
-000033e0: 3732 3337 3733 3433 5d2c 2022 6c61 6265  72377343], "labe
-000033f0: 6c22 3a20 224f 222c 2022 7072 6f70 6572  l": "O", "proper
-00003400: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00003410: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-00003420: 6e74 223a 2022 4f22 2c20 226f 6363 7522  nt": "O", "occu"
-00003430: 3a20 312e 307d 5d2c 2022 6162 6322 3a20  : 1.0}], "abc": 
-00003440: 5b30 2e36 3034 3038 3938 3832 3039 3333  [0.6040898820933
-00003450: 3131 352c 2030 2e32 3431 3832 3137 3639  115, 0.241821769
-00003460: 3837 3233 3633 372c 2030 2e38 3636 3939  8723637, 0.86699
-00003470: 3634 3435 3436 3634 3035 395d 2c20 2278  64454664059], "x
-00003480: 797a 223a 205b 332e 3139 3130 3436 3039  yz": [3.19104609
-00003490: 3031 3435 3137 332c 2031 2e30 3532 3130  0145173, 1.05210
-000034a0: 3331 3739 3330 3235 3539 352c 2037 2e34  31793025595, 7.4
-000034b0: 3338 3130 3331 3335 3034 3336 3533 355d  381031350436535]
-000034c0: 2c20 226c 6162 656c 223a 2022 4f22 2c20  , "label": "O", 
-000034d0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-000034e0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-000034f0: 7b22 656c 656d 656e 7422 3a20 2254 6522  {"element": "Te"
-00003500: 2c20 226f 6363 7522 3a20 312e 307d 5d2c  , "occu": 1.0}],
-00003510: 2022 6162 6322 3a20 5b30 2e34 3936 3539   "abc": [0.49659
-00003520: 3035 3631 3035 3037 3335 332c 2030 2e34  05610507353, 0.4
-00003530: 3936 3539 3035 3631 3035 3037 3335 352c  965905610507355,
-00003540: 2030 2e34 3936 3539 3035 3631 3035 3037   0.4965905610507
-00003550: 3336 315d 2c20 2278 797a 223a 205b 332e  361], "xyz": [3.
-00003560: 3131 3330 3639 3339 3038 3335 3739 332c  113069390835793,
-00003570: 2032 2e31 3430 3635 3931 3335 3730 3234   2.1406591357024
-00003580: 3938 342c 2035 2e38 3339 3837 3535 3631  984, 5.839875561
-00003590: 3231 3436 3632 345d 2c20 226c 6162 656c  2146624], "label
-000035a0: 223a 2022 5465 222c 2022 7072 6f70 6572  ": "Te", "proper
-000035b0: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000035c0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000035d0: 6e74 223a 2022 5a72 222c 2022 6f63 6375  nt": "Zr", "occu
-000035e0: 223a 2031 2e30 7d5d 2c20 2261 6263 223a  ": 1.0}], "abc":
-000035f0: 205b 302e 3030 3036 3530 3136 3034 3938   [0.000650160498
-00003600: 3036 3638 2c20 302e 3030 3036 3530 3136  0668, 0.00065016
-00003610: 3034 3938 3039 3238 2c20 302e 3030 3036  04980928, 0.0006
-00003620: 3530 3136 3034 3938 3233 3434 5d2c 2022  501604982344], "
-00003630: 7879 7a22 3a20 5b30 2e30 3034 3037 3537  xyz": [0.0040757
-00003640: 3831 3734 3934 3630 3336 2c20 302e 3030  8174946036, 0.00
-00003650: 3238 3032 3635 3439 3831 3934 3531 3932  2802654981945192
-00003660: 2c20 302e 3030 3736 3435 3834 3839 3138  , 0.007645848918
-00003670: 3236 3330 3736 5d2c 2022 6c61 6265 6c22  263076], "label"
-00003680: 3a20 225a 7222 2c20 2270 726f 7065 7274  : "Zr", "propert
-00003690: 6965 7322 3a20 7b7d 7d5d 7dda 0d64 696c  ies": {}}]}..dil
-000036a0: 7574 654e 6941 6c6c 6f79 7a4d 5072 6f66  uteNiAlloyzMProf
-000036b0: 696c 696e 672f 7465 7374 696e 6720 7461  iling/testing ta
-000036c0: 736b 2e20 5769 6c6c 2063 616c 6375 6c61  sk. Will calcula
-000036d0: 7465 2061 2064 6573 6372 6970 746f 7220  te a descriptor 
-000036e0: 666f 7220 6120 6469 6c75 7465 2046 4343  for a dilute FCC
-000036f0: 204e 6933 3143 7231 2ee1 d414 0000 7b22   Ni31Cr1......{"
-00003700: 406d 6f64 756c 6522 3a20 2270 796d 6174  @module": "pymat
-00003710: 6765 6e2e 636f 7265 2e73 7472 7563 7475  gen.core.structu
-00003720: 7265 222c 2022 4063 6c61 7373 223a 2022  re", "@class": "
-00003730: 5374 7275 6374 7572 6522 2c20 2263 6861  Structure", "cha
-00003740: 7267 6522 3a20 6e75 6c6c 2c20 226c 6174  rge": null, "lat
-00003750: 7469 6365 223a 207b 226d 6174 7269 7822  tice": {"matrix"
-00003760: 3a20 5b5b 362e 3939 3536 3932 2c20 302e  : [[6.995692, 0.
-00003770: 302c 2030 2e30 5d2c 205b 302e 302c 2036  0, 0.0], [0.0, 6
-00003780: 2e39 3935 3639 322c 2030 2e30 5d2c 205b  .995692, 0.0], [
-00003790: 302e 302c 2030 2e30 2c20 362e 3939 3536  0.0, 0.0, 6.9956
-000037a0: 3932 5d5d 2c20 2261 223a 2036 2e39 3935  92]], "a": 6.995
-000037b0: 3639 322c 2022 6222 3a20 362e 3939 3536  692, "b": 6.9956
-000037c0: 3932 2c20 2263 223a 2036 2e39 3935 3639  92, "c": 6.99569
-000037d0: 322c 2022 616c 7068 6122 3a20 3930 2e30  2, "alpha": 90.0
-000037e0: 2c20 2262 6574 6122 3a20 3930 2e30 2c20  , "beta": 90.0, 
-000037f0: 2267 616d 6d61 223a 2039 302e 302c 2022  "gamma": 90.0, "
-00003800: 766f 6c75 6d65 223a 2033 3432 2e33 3637  volume": 342.367
-00003810: 3131 3336 3536 3139 3234 337d 2c20 2273  11365619243}, "s
-00003820: 6974 6573 223a 205b 7b22 7370 6563 6965  ites": [{"specie
-00003830: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
-00003840: 2022 4372 222c 2022 6f63 6375 223a 2031   "Cr", "occu": 1
-00003850: 7d5d 2c20 2261 6263 223a 205b 302e 302c  }], "abc": [0.0,
-00003860: 2030 2e30 2c20 302e 305d 2c20 2278 797a   0.0, 0.0], "xyz
-00003870: 223a 205b 302e 302c 2030 2e30 2c20 302e  ": [0.0, 0.0, 0.
-00003880: 305d 2c20 226c 6162 656c 223a 2022 4372  0], "label": "Cr
-00003890: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-000038a0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-000038b0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-000038c0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-000038d0: 2c20 2261 6263 223a 205b 302e 302c 2030  , "abc": [0.0, 0
-000038e0: 2e30 2c20 302e 355d 2c20 2278 797a 223a  .0, 0.5], "xyz":
-000038f0: 205b 302e 302c 2030 2e30 2c20 332e 3439   [0.0, 0.0, 3.49
-00003900: 3738 3436 5d2c 2022 6c61 6265 6c22 3a20  7846], "label": 
-00003910: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-00003920: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-00003930: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-00003940: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-00003950: 317d 5d2c 2022 6162 6322 3a20 5b30 2e30  1}], "abc": [0.0
-00003960: 2c20 302e 352c 2030 2e30 5d2c 2022 7879  , 0.5, 0.0], "xy
-00003970: 7a22 3a20 5b30 2e30 2c20 332e 3439 3738  z": [0.0, 3.4978
-00003980: 3436 2c20 302e 305d 2c20 226c 6162 656c  46, 0.0], "label
-00003990: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-000039a0: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000039b0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000039c0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000039d0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000039e0: 302e 302c 2030 2e35 2c20 302e 355d 2c20  0.0, 0.5, 0.5], 
-000039f0: 2278 797a 223a 205b 302e 302c 2033 2e34  "xyz": [0.0, 3.4
-00003a00: 3937 3834 362c 2033 2e34 3937 3834 365d  97846, 3.497846]
-00003a10: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003a20: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003a30: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003a40: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003a50: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003a60: 2261 6263 223a 205b 302e 352c 2030 2e30  "abc": [0.5, 0.0
-00003a70: 2c20 302e 305d 2c20 2278 797a 223a 205b  , 0.0], "xyz": [
-00003a80: 332e 3439 3738 3436 2c20 302e 302c 2030  3.497846, 0.0, 0
-00003a90: 2e30 5d2c 2022 6c61 6265 6c22 3a20 224e  .0], "label": "N
-00003aa0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003ab0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003ac0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003ad0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00003ae0: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
-00003af0: 302e 302c 2030 2e35 5d2c 2022 7879 7a22  0.0, 0.5], "xyz"
-00003b00: 3a20 5b33 2e34 3937 3834 362c 2030 2e30  : [3.497846, 0.0
-00003b10: 2c20 332e 3439 3738 3436 5d2c 2022 6c61  , 3.497846], "la
-00003b20: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003b30: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00003b40: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00003b50: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-00003b60: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-00003b70: 3a20 5b30 2e35 2c20 302e 352c 2030 2e30  : [0.5, 0.5, 0.0
-00003b80: 5d2c 2022 7879 7a22 3a20 5b33 2e34 3937  ], "xyz": [3.497
-00003b90: 3834 362c 2033 2e34 3937 3834 362c 2030  846, 3.497846, 0
-00003ba0: 2e30 5d2c 2022 6c61 6265 6c22 3a20 224e  .0], "label": "N
-00003bb0: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
-00003bc0: 3a20 7b7d 7d2c 207b 2273 7065 6369 6573  : {}}, {"species
-00003bd0: 223a 205b 7b22 656c 656d 656e 7422 3a20  ": [{"element": 
-00003be0: 224e 6922 2c20 226f 6363 7522 3a20 317d  "Ni", "occu": 1}
-00003bf0: 5d2c 2022 6162 6322 3a20 5b30 2e35 2c20  ], "abc": [0.5, 
-00003c00: 302e 352c 2030 2e35 5d2c 2022 7879 7a22  0.5, 0.5], "xyz"
-00003c10: 3a20 5b33 2e34 3937 3834 362c 2033 2e34  : [3.497846, 3.4
-00003c20: 3937 3834 362c 2033 2e34 3937 3834 365d  97846, 3.497846]
-00003c30: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00003c40: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00003c50: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00003c60: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00003c70: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00003c80: 2261 6263 223a 205b 302e 3235 2c20 302e  "abc": [0.25, 0.
-00003c90: 3235 2c20 302e 305d 2c20 2278 797a 223a  25, 0.0], "xyz":
-00003ca0: 205b 312e 3734 3839 3233 2c20 312e 3734   [1.748923, 1.74
-00003cb0: 3839 3233 2c20 302e 305d 2c20 226c 6162  8923, 0.0], "lab
-00003cc0: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
-00003cd0: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
-00003ce0: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
-00003cf0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
-00003d00: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
-00003d10: 205b 302e 3235 2c20 302e 3235 2c20 302e   [0.25, 0.25, 0.
-00003d20: 355d 2c20 2278 797a 223a 205b 312e 3734  5], "xyz": [1.74
-00003d30: 3839 3233 2c20 312e 3734 3839 3233 2c20  8923, 1.748923, 
-00003d40: 332e 3439 3738 3436 5d2c 2022 6c61 6265  3.497846], "labe
-00003d50: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
-00003d60: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
-00003d70: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
-00003d80: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
-00003d90: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
-00003da0: 5b30 2e32 352c 2030 2e37 3530 3030 3030  [0.25, 0.7500000
-00003db0: 3030 3030 3030 3030 312c 2030 2e30 5d2c  000000001, 0.0],
-00003dc0: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
-00003dd0: 332c 2035 2e32 3436 3736 3930 3030 3030  3, 5.24676900000
-00003de0: 3030 3030 352c 2030 2e30 5d2c 2022 6c61  00005, 0.0], "la
-00003df0: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003e00: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00003e10: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00003e20: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-00003e30: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-00003e40: 3a20 5b30 2e32 352c 2030 2e37 3530 3030  : [0.25, 0.75000
-00003e50: 3030 3030 3030 3030 3030 312c 2030 2e35  00000000001, 0.5
-00003e60: 5d2c 2022 7879 7a22 3a20 5b31 2e37 3438  ], "xyz": [1.748
-00003e70: 3932 332c 2035 2e32 3436 3736 3930 3030  923, 5.246769000
-00003e80: 3030 3030 3030 352c 2033 2e34 3937 3834  0000005, 3.49784
-00003e90: 365d 2c20 226c 6162 656c 223a 2022 4e69  6], "label": "Ni
-00003ea0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00003eb0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00003ec0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00003ed0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00003ee0: 2c20 2261 6263 223a 205b 302e 3735 3030  , "abc": [0.7500
-00003ef0: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
-00003f00: 3235 2c20 302e 305d 2c20 2278 797a 223a  25, 0.0], "xyz":
-00003f10: 205b 352e 3234 3637 3639 3030 3030 3030   [5.246769000000
-00003f20: 3030 3035 2c20 312e 3734 3839 3233 2c20  0005, 1.748923, 
-00003f30: 302e 305d 2c20 226c 6162 656c 223a 2022  0.0], "label": "
-00003f40: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
-00003f50: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
-00003f60: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
-00003f70: 2022 4e69 222c 2022 6f63 6375 223a 2031   "Ni", "occu": 1
-00003f80: 7d5d 2c20 2261 6263 223a 205b 302e 3735  }], "abc": [0.75
-00003f90: 3030 3030 3030 3030 3030 3030 3031 2c20  00000000000001, 
-00003fa0: 302e 3235 2c20 302e 355d 2c20 2278 797a  0.25, 0.5], "xyz
-00003fb0: 223a 205b 352e 3234 3637 3639 3030 3030  ": [5.2467690000
-00003fc0: 3030 3030 3035 2c20 312e 3734 3839 3233  000005, 1.748923
-00003fd0: 2c20 332e 3439 3738 3436 5d2c 2022 6c61  , 3.497846], "la
-00003fe0: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
-00003ff0: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
-00004000: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
-00004010: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
-00004020: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
-00004030: 3a20 5b30 2e37 3530 3030 3030 3030 3030  : [0.75000000000
-00004040: 3030 3030 312c 2030 2e37 3530 3030 3030  00001, 0.7500000
-00004050: 3030 3030 3030 3030 312c 2030 2e30 5d2c  000000001, 0.0],
-00004060: 2022 7879 7a22 3a20 5b35 2e32 3436 3736   "xyz": [5.24676
-00004070: 3930 3030 3030 3030 3030 352c 2035 2e32  90000000005, 5.2
-00004080: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
-00004090: 2030 2e30 5d2c 2022 6c61 6265 6c22 3a20   0.0], "label": 
-000040a0: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
-000040b0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
-000040c0: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
-000040d0: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
-000040e0: 317d 5d2c 2022 6162 6322 3a20 5b30 2e37  1}], "abc": [0.7
-000040f0: 3530 3030 3030 3030 3030 3030 3030 312c  500000000000001,
-00004100: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
-00004110: 3030 312c 2030 2e35 5d2c 2022 7879 7a22  001, 0.5], "xyz"
-00004120: 3a20 5b35 2e32 3436 3736 3930 3030 3030  : [5.24676900000
-00004130: 3030 3030 352c 2035 2e32 3436 3736 3930  00005, 5.2467690
-00004140: 3030 3030 3030 3030 352c 2033 2e34 3937  000000005, 3.497
-00004150: 3834 365d 2c20 226c 6162 656c 223a 2022  846], "label": "
-00004160: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
-00004170: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
-00004180: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
-00004190: 2022 4e69 222c 2022 6f63 6375 223a 2031   "Ni", "occu": 1
-000041a0: 7d5d 2c20 2261 6263 223a 205b 302e 3235  }], "abc": [0.25
-000041b0: 2c20 302e 302c 2030 2e32 355d 2c20 2278  , 0.0, 0.25], "x
-000041c0: 797a 223a 205b 312e 3734 3839 3233 2c20  yz": [1.748923, 
-000041d0: 302e 302c 2031 2e37 3438 3932 335d 2c20  0.0, 1.748923], 
-000041e0: 226c 6162 656c 223a 2022 4e69 222c 2022  "label": "Ni", "
-000041f0: 7072 6f70 6572 7469 6573 223a 207b 7d7d  properties": {}}
-00004200: 2c20 7b22 7370 6563 6965 7322 3a20 5b7b  , {"species": [{
-00004210: 2265 6c65 6d65 6e74 223a 2022 4e69 222c  "element": "Ni",
-00004220: 2022 6f63 6375 223a 2031 7d5d 2c20 2261   "occu": 1}], "a
-00004230: 6263 223a 205b 302e 3235 2c20 302e 302c  bc": [0.25, 0.0,
-00004240: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
-00004250: 3030 315d 2c20 2278 797a 223a 205b 312e  001], "xyz": [1.
-00004260: 3734 3839 3233 2c20 302e 302c 2035 2e32  748923, 0.0, 5.2
-00004270: 3436 3736 3930 3030 3030 3030 3030 355d  467690000000005]
-00004280: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00004290: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-000042a0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-000042b0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-000042c0: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-000042d0: 2261 6263 223a 205b 302e 3235 2c20 302e  "abc": [0.25, 0.
-000042e0: 352c 2030 2e32 355d 2c20 2278 797a 223a  5, 0.25], "xyz":
-000042f0: 205b 312e 3734 3839 3233 2c20 332e 3439   [1.748923, 3.49
-00004300: 3738 3436 2c20 312e 3734 3839 3233 5d2c  7846, 1.748923],
-00004310: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
-00004320: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-00004330: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-00004340: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-00004350: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-00004360: 6162 6322 3a20 5b30 2e32 352c 2030 2e35  abc": [0.25, 0.5
-00004370: 2c20 302e 3735 3030 3030 3030 3030 3030  , 0.750000000000
-00004380: 3030 3031 5d2c 2022 7879 7a22 3a20 5b31  0001], "xyz": [1
-00004390: 2e37 3438 3932 332c 2033 2e34 3937 3834  .748923, 3.49784
-000043a0: 362c 2035 2e32 3436 3736 3930 3030 3030  6, 5.24676900000
-000043b0: 3030 3030 355d 2c20 226c 6162 656c 223a  00005], "label":
-000043c0: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-000043d0: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-000043e0: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-000043f0: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00004400: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-00004410: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-00004420: 2c20 302e 302c 2030 2e32 355d 2c20 2278  , 0.0, 0.25], "x
-00004430: 797a 223a 205b 352e 3234 3637 3639 3030  yz": [5.24676900
-00004440: 3030 3030 3030 3035 2c20 302e 302c 2031  00000005, 0.0, 1
-00004450: 2e37 3438 3932 335d 2c20 226c 6162 656c  .748923], "label
-00004460: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00004470: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-00004480: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-00004490: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000044a0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000044b0: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
-000044c0: 3031 2c20 302e 302c 2030 2e37 3530 3030  01, 0.0, 0.75000
-000044d0: 3030 3030 3030 3030 3030 315d 2c20 2278  00000000001], "x
-000044e0: 797a 223a 205b 352e 3234 3637 3639 3030  yz": [5.24676900
-000044f0: 3030 3030 3030 3035 2c20 302e 302c 2035  00000005, 0.0, 5
-00004500: 2e32 3436 3736 3930 3030 3030 3030 3030  .246769000000000
-00004510: 355d 2c20 226c 6162 656c 223a 2022 4e69  5], "label": "Ni
-00004520: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00004530: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00004540: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00004550: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00004560: 2c20 2261 6263 223a 205b 302e 3735 3030  , "abc": [0.7500
-00004570: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
-00004580: 352c 2030 2e32 355d 2c20 2278 797a 223a  5, 0.25], "xyz":
-00004590: 205b 352e 3234 3637 3639 3030 3030 3030   [5.246769000000
-000045a0: 3030 3035 2c20 332e 3439 3738 3436 2c20  0005, 3.497846, 
-000045b0: 312e 3734 3839 3233 5d2c 2022 6c61 6265  1.748923], "labe
-000045c0: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
-000045d0: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
-000045e0: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
-000045f0: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
-00004600: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
-00004610: 5b30 2e37 3530 3030 3030 3030 3030 3030  [0.7500000000000
-00004620: 3030 312c 2030 2e35 2c20 302e 3735 3030  001, 0.5, 0.7500
-00004630: 3030 3030 3030 3030 3030 3031 5d2c 2022  000000000001], "
-00004640: 7879 7a22 3a20 5b35 2e32 3436 3736 3930  xyz": [5.2467690
-00004650: 3030 3030 3030 3030 352c 2033 2e34 3937  000000005, 3.497
-00004660: 3834 362c 2035 2e32 3436 3736 3930 3030  846, 5.246769000
-00004670: 3030 3030 3030 355d 2c20 226c 6162 656c  0000005], "label
-00004680: 223a 2022 4e69 222c 2022 7072 6f70 6572  ": "Ni", "proper
-00004690: 7469 6573 223a 207b 7d7d 2c20 7b22 7370  ties": {}}, {"sp
-000046a0: 6563 6965 7322 3a20 5b7b 2265 6c65 6d65  ecies": [{"eleme
-000046b0: 6e74 223a 2022 4e69 222c 2022 6f63 6375  nt": "Ni", "occu
-000046c0: 223a 2031 7d5d 2c20 2261 6263 223a 205b  ": 1}], "abc": [
-000046d0: 302e 302c 2030 2e32 352c 2030 2e32 355d  0.0, 0.25, 0.25]
-000046e0: 2c20 2278 797a 223a 205b 302e 302c 2031  , "xyz": [0.0, 1
-000046f0: 2e37 3438 3932 332c 2031 2e37 3438 3932  .748923, 1.74892
-00004700: 335d 2c20 226c 6162 656c 223a 2022 4e69  3], "label": "Ni
-00004710: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
-00004720: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
-00004730: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
-00004740: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
-00004750: 2c20 2261 6263 223a 205b 302e 302c 2030  , "abc": [0.0, 0
-00004760: 2e32 352c 2030 2e37 3530 3030 3030 3030  .25, 0.750000000
-00004770: 3030 3030 3030 315d 2c20 2278 797a 223a  0000001], "xyz":
-00004780: 205b 302e 302c 2031 2e37 3438 3932 332c   [0.0, 1.748923,
-00004790: 2035 2e32 3436 3736 3930 3030 3030 3030   5.2467690000000
-000047a0: 3030 355d 2c20 226c 6162 656c 223a 2022  005], "label": "
-000047b0: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
-000047c0: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
-000047d0: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
-000047e0: 2022 4e69 222c 2022 6f63 6375 223a 2031   "Ni", "occu": 1
-000047f0: 7d5d 2c20 2261 6263 223a 205b 302e 302c  }], "abc": [0.0,
-00004800: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
-00004810: 3030 312c 2030 2e32 355d 2c20 2278 797a  001, 0.25], "xyz
-00004820: 223a 205b 302e 302c 2035 2e32 3436 3736  ": [0.0, 5.24676
-00004830: 3930 3030 3030 3030 3030 352c 2031 2e37  90000000005, 1.7
-00004840: 3438 3932 335d 2c20 226c 6162 656c 223a  48923], "label":
-00004850: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-00004860: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-00004870: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-00004880: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00004890: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-000048a0: 302c 2030 2e37 3530 3030 3030 3030 3030  0, 0.75000000000
-000048b0: 3030 3030 312c 2030 2e37 3530 3030 3030  00001, 0.7500000
-000048c0: 3030 3030 3030 3030 315d 2c20 2278 797a  000000001], "xyz
-000048d0: 223a 205b 302e 302c 2035 2e32 3436 3736  ": [0.0, 5.24676
-000048e0: 3930 3030 3030 3030 3030 352c 2035 2e32  90000000005, 5.2
-000048f0: 3436 3736 3930 3030 3030 3030 3030 355d  467690000000005]
-00004900: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
-00004910: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
-00004920: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
-00004930: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
-00004940: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
-00004950: 2261 6263 223a 205b 302e 352c 2030 2e32  "abc": [0.5, 0.2
-00004960: 352c 2030 2e32 355d 2c20 2278 797a 223a  5, 0.25], "xyz":
-00004970: 205b 332e 3439 3738 3436 2c20 312e 3734   [3.497846, 1.74
-00004980: 3839 3233 2c20 312e 3734 3839 3233 5d2c  8923, 1.748923],
-00004990: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
-000049a0: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
-000049b0: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
-000049c0: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
-000049d0: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
-000049e0: 6162 6322 3a20 5b30 2e35 2c20 302e 3235  abc": [0.5, 0.25
-000049f0: 2c20 302e 3735 3030 3030 3030 3030 3030  , 0.750000000000
-00004a00: 3030 3031 5d2c 2022 7879 7a22 3a20 5b33  0001], "xyz": [3
-00004a10: 2e34 3937 3834 362c 2031 2e37 3438 3932  .497846, 1.74892
-00004a20: 332c 2035 2e32 3436 3736 3930 3030 3030  3, 5.24676900000
-00004a30: 3030 3030 355d 2c20 226c 6162 656c 223a  00005], "label":
-00004a40: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
-00004a50: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
-00004a60: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
-00004a70: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
-00004a80: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
-00004a90: 352c 2030 2e37 3530 3030 3030 3030 3030  5, 0.75000000000
-00004aa0: 3030 3030 312c 2030 2e32 355d 2c20 2278  00001, 0.25], "x
-00004ab0: 797a 223a 205b 332e 3439 3738 3436 2c20  yz": [3.497846, 
-00004ac0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
-00004ad0: 3035 2c20 312e 3734 3839 3233 5d2c 2022  05, 1.748923], "
-00004ae0: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
-00004af0: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
-00004b00: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
-00004b10: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
-00004b20: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
-00004b30: 6322 3a20 5b30 2e35 2c20 302e 3735 3030  c": [0.5, 0.7500
-00004b40: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
-00004b50: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
-00004b60: 5d2c 2022 7879 7a22 3a20 5b33 2e34 3937  ], "xyz": [3.497
-00004b70: 3834 362c 2035 2e32 3436 3736 3930 3030  846, 5.246769000
-00004b80: 3030 3030 3030 352c 2035 2e32 3436 3736  0000005, 5.24676
-00004b90: 3930 3030 3030 3030 3030 355d 2c20 226c  90000000005], "l
-00004ba0: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
-00004bb0: 6f70 6572 7469 6573 223a 207b 7d7d 5d2c  operties": {}}],
-00004bc0: 2022 4076 6572 7369 6f6e 223a 206e 756c   "@version": nul
-00004bd0: 6c7d fa17 556e 7265 636f 676e 697a 6564  l}..Unrecognized
-00004be0: 2074 6573 7420 6e61 6d65 2e4e 7a15 4b53   test name.Nz.KS
-00004bf0: 3230 3232 5f54 6573 7452 6573 756c 742e  2022_TestResult.
-00004c00: 6373 767a 0277 2b63 0100 0000 0000 0000  csvz.w+c........
-00004c10: 0000 0000 0200 0000 0400 0000 5300 0000  ............S...
-00004c20: 7316 0000 0067 007c 005d 0e7d 017c 019b  s....g.|.].}.|..
-00004c30: 0064 009d 0291 0271 0453 0029 01da 010a  .d.....q.S.)....
-00004c40: 7224 0000 0029 0272 2600 0000 da01 7672  r$...).r&.....vr
-00004c50: 2400 0000 7224 0000 0072 2800 0000 7229  $...r$...r(...r)
-00004c60: 0000 0050 0100 0072 2a00 0000 7a1b 7072  ...P...r*...z.pr
-00004c70: 6f66 696c 652e 3c6c 6f63 616c 733e 2e3c  ofile.<locals>.<
-00004c80: 6c69 7374 636f 6d70 3efa 0544 6f6e 6521  listcomp>..Done!
-00004c90: 2909 da05 7072 696e 7472 0200 0000 da09  )...printr......
-00004ca0: 6672 6f6d 5f64 6963 74da 046a 736f 6eda  from_dict..json.
-00004cb0: 056c 6f61 6473 7205 0000 0072 ae00 0000  .loadsr....r....
-00004cc0: da04 6f70 656e da0a 7772 6974 656c 696e  ..open..writelin
-00004cd0: 6573 2907 da04 7465 7374 da05 6e52 756e  es)...test..nRun
-00004ce0: 73da 066d 6174 5374 72da 0a73 7472 7563  s..matStr..struc
-00004cf0: 744c 6973 7472 9700 0000 7298 0000 0072  tListr....r....r
-00004d00: 9900 0000 7224 0000 0072 2400 0000 7228  ....r$...r$...r(
-00004d10: 0000 00da 0770 726f 6669 6c65 4101 0000  .....profileA...
-00004d20: 731c 0000 0000 0208 0108 0106 0108 0108  s...............
-00004d30: 0106 0208 0104 0116 010c 010a 010c 0132  ...............2
-00004d40: 0172 c300 0000 e9e8 0300 0063 0200 0000  .r.........c....
-00004d50: 0000 0000 0000 0000 0700 0000 0500 0000  ................
-00004d60: 4300 0000 7368 0000 0064 0164 026c 006d  C...sh...d.d.l.m
-00004d70: 017d 0201 007c 0064 036b 0272 1a64 047d  .}...|.d.k.r.d.}
-00004d80: 036e 1a7c 0064 056b 0272 2864 067d 036e  .n.|.d.k.r(d.}.n
-00004d90: 0c74 0264 0783 0101 0064 0853 0074 03a0  .t.d.....d.S.t..
-00004da0: 0474 05a0 067c 03a1 01a1 017d 047c 0467  .t...|.....}.|.g
-00004db0: 017c 0114 007d 057c 0274 077c 0564 0964  .|...}.|.t.|.d.d
-00004dc0: 0a8d 037d 0674 0264 0b83 0101 0064 0853  ...}.t.d.....d.S
-00004dd0: 0029 0c7a 4550 726f 6669 6c65 7320 7468  .).zEProfiles th
-00004de0: 6520 6465 7363 7269 7074 6f72 2069 6e20  e descriptor in 
-00004df0: 7061 7261 6c6c 656c 2075 7369 6e67 206f  parallel using o
-00004e00: 6e65 206f 6620 7468 6520 7465 7374 2073  ne of the test s
-00004e10: 7472 7563 7475 7265 732e 7201 0000 0029  tructures.r....)
-00004e20: 01da 0b70 726f 6365 7373 5f6d 6170 72b1  ...process_mapr.
-00004e30: 0000 0072 b200 0000 72b3 0000 0072 b400  ...r....r....r..
-00004e40: 0000 72b5 0000 004e 7211 0000 0029 01da  ..r....Nr....)..
-00004e50: 0b6d 6178 5f77 6f72 6b65 7273 72b8 0000  .max_workersr...
-00004e60: 0029 08da 1774 7164 6d2e 636f 6e74 7269  .)...tqdm.contri
-00004e70: 622e 636f 6e63 7572 7265 6e74 72c5 0000  b.concurrentr...
-00004e80: 0072 b900 0000 7202 0000 0072 ba00 0000  .r....r....r....
-00004e90: 72bb 0000 0072 bc00 0000 72ae 0000 0029  r....r....r....)
-00004ea0: 0772 bf00 0000 72c0 0000 0072 c500 0000  .r....r....r....
-00004eb0: 72c1 0000 0072 9700 0000 72c2 0000 00da  r....r....r.....
-00004ec0: 0864 6573 634c 6973 7472 2400 0000 7224  .descListr$...r$
-00004ed0: 0000 0072 2800 0000 da0f 7072 6f66 696c  ...r(.....profil
-00004ee0: 6550 6172 616c 6c65 6c53 0100 0073 1600  eParallelS...s..
-00004ef0: 0000 0002 0c01 0801 0601 0801 0602 0801  ................
-00004f00: 0401 1002 0a01 0e01 72c9 0000 00da 085f  ........r......_
-00004f10: 5f6d 6169 6e5f 5f29 0172 bf00 0000 72b3  _main__).r....r.
-00004f20: 0000 0029 0172 0100 0000 2902 72b1 0000  ...).r....).r...
-00004f30: 0072 1100 0000 2902 72b1 0000 0072 c400  .r....).r....r..
-00004f40: 0000 2924 723a 0000 0072 bb00 0000 da05  ..)$r:...r......
-00004f50: 6e75 6d70 7972 2f00 0000 da02 6f73 da0d  numpyr/.....os..
-00004f60: 7079 6d61 7467 656e 2e63 6f72 6572 0200  pymatgen.corer..
-00004f70: 0000 7203 0000 005a 1b70 796d 6174 6765  ..r....Z.pymatge
-00004f80: 6e2e 616e 616c 7973 6973 2e6c 6f63 616c  n.analysis.local
-00004f90: 5f65 6e76 7204 0000 0072 0500 0000 da06  _envr....r......
-00004fa0: 7479 7069 6e67 7206 0000 0072 af00 0000  typingr....r....
-00004fb0: 5a13 7065 7269 6f64 6963 5f74 6162 6c65  Z.periodic_table
-00004fc0: 5f73 697a 65da 076c 6f61 6474 7874 da04  _size..loadtxt..
-00004fd0: 7061 7468 da04 6a6f 696e da07 6469 726e  path..join..dirn
-00004fe0: 616d 65da 085f 5f66 696c 655f 5f72 3100  ame..__file__r1.
-00004ff0: 0000 da0a 6e61 6e5f 746f 5f6e 756d 725b  ....nan_to_numr[
-00005000: 0000 0072 4500 0000 7246 0000 0072 5f00  ...rE...rF...r_.
-00005010: 0000 72a7 0000 0072 7600 0000 7284 0000  ..r....rv...r...
-00005020: 00da 076e 6461 7272 6179 72ae 0000 00da  ...ndarrayr.....
-00005030: 0373 7472 72b0 0000 0072 c300 0000 72c9  .strr....r....r.
-00005040: 0000 0072 4f00 0000 7224 0000 0072 2400  ...rO...r$...r$.
-00005050: 0000 7224 0000 0072 2800 0000 da08 3c6d  ..r$...r(.....<m
-00005060: 6f64 756c 653e 0a00 0000 733c 0000 0008  odule>....s<....
-00005070: 0108 0108 0108 0110 010c 010c 010c 0202  ................
-00005080: 0302 fd04 0804 0120 010a 0208 0106 ff06  ....... ........
-00005090: 030e 410e 1212 1814 460a 1412 5512 050a  ..A.....F...U...
-000050a0: 120a 110a 010a 010a 010a 01              ...........
+00000070: 6d0b 5a0b 0100 6400 6401 6c0c 5a0c 6400  m.Z...d.d.l.Z.d.
+00000080: 6405 6c0d 6d0d 5a0d 0100 6400 6406 6c0e  d.l.m.Z...d.d.l.
+00000090: 6d0f 5a0f 0100 6407 5a10 6408 5a11 6503  m.Z...d.Z.d.Z.e.
+000000a0: 6a12 6504 6a13 a014 6504 6a13 a015 6516  j.e.j...e.j...e.
+000000b0: a101 6409 a102 640a 640b 8d02 5a17 6503  ..d...d.d...Z.e.
+000000c0: a018 6517 a101 5a17 6517 6401 6401 8502  ..e...Z.e.d.d...
+000000d0: 6700 640c a201 6602 1900 5a17 640d 640e  g.d...f...Z.d.d.
+000000e0: 8400 5a19 640f 6410 8400 5a1a 6411 6519  ..Z.d.d...Z.d.e.
+000000f0: 6602 6412 6413 8401 5a1b 4700 6414 6415  f.d.d...Z.G.d.d.
+00000100: 8400 6415 8302 5a1c 6427 6416 6417 8401  ..d...Z.d'd.d...
+00000110: 5a1d 6428 6506 6418 9c01 6419 641a 8405  Z.d(e.d...d.d...
+00000120: 5a1e 641b 641c 8400 5a1f 6429 641f 6420  Z.d.d...Z.d)d.d 
+00000130: 8401 5a20 642a 6422 6423 8401 5a21 6522  ..Z d*d"d#..Z!e"
+00000140: 6424 6b02 9001 722e 6520 6425 6426 8d01  d$k...r.e d%d&..
+00000150: 0100 6521 6425 6426 8d01 0100 6401 5300  ..e!d%d&....d.S.
+00000160: 292b e900 0000 004e 2902 da09 5374 7275  )+.....N)...Stru
+00000170: 6374 7572 65da 0745 6c65 6d65 6e74 2901  cture..Element).
+00000180: da09 566f 726f 6e6f 694e 4e29 01da 1253  ..VoronoiNN)...S
+00000190: 7061 6365 6772 6f75 7041 6e61 6c79 7a65  pacegroupAnalyze
+000001a0: 7229 01da 0474 7164 6d29 01da 0743 6f75  r)...tqdm)...Cou
+000001b0: 6e74 6572 75f9 0000 004c 2e20 5761 7264  nteru....L. Ward
+000001c0: 2c20 522e 204c 6975 2c20 412e 204b 7269  , R. Liu, A. Kri
+000001d0: 7368 6e61 2c20 562e 2049 2e20 4865 6764  shna, V. I. Hegd
+000001e0: 652c 2041 2e20 4167 7261 7761 6c2c 2041  e, A. Agrawal, A
+000001f0: 2e20 4368 6f75 6468 6172 792c 2061 6e64  . Choudhary, and
+00000200: 2043 2e20 576f 6c76 6572 746f 6e2c 20e2   C. Wolverton, .
+00000210: 809c 496e 636c 7564 696e 6720 6372 7973  ..Including crys
+00000220: 7461 6c20 7374 7275 6374 7572 6520 6174  tal structure at
+00000230: 7472 6962 7574 6573 2069 6e20 6d61 6368  tributes in mach
+00000240: 696e 6520 6c65 6172 6e69 6e67 206d 6f64  ine learning mod
+00000250: 656c 7320 6f66 2066 6f72 6d61 7469 6f6e  els of formation
+00000260: 2065 6e65 7267 6965 7320 7669 6120 566f   energies via Vo
+00000270: 726f 6e6f 6920 7465 7373 656c 6c61 7469  ronoi tessellati
+00000280: 6f6e 732c e280 9d20 5068 7973 6963 616c  ons,... Physical
+00000290: 2052 6576 6965 7720 422c 2076 6f6c 2e20   Review B, vol. 
+000002a0: 3936 2c20 6e6f 2e20 322c 2037 2032 3031  96, no. 2, 7 201
+000002b0: 372e e970 0000 007a 1d4d 6167 7069 655f  7..p...z.Magpie_
+000002c0: 656c 656d 656e 745f 7072 6f70 6572 7469  element_properti
+000002d0: 6573 2e63 7376 fa01 2c29 01da 0964 656c  es.csv..,)...del
+000002e0: 696d 6974 6572 2915 e92d 0000 00e9 2100  imiter)..-....!.
+000002f0: 0000 e902 0000 00e9 2000 0000 e905 0000  ........ .......
+00000300: 00e9 3000 0000 e906 0000 00e9 0a00 0000  ..0.............
+00000310: e92c 0000 00e9 2a00 0000 e926 0000 00e9  .,....*....&....
+00000320: 2800 0000 e924 0000 00e9 2b00 0000 e929  (....$....+....)
+00000330: 0000 00e9 2500 0000 e927 0000 00e9 2300  ....%....'....#.
+00000340: 0000 e912 0000 00e9 0d00 0000 e911 0000  ................
+00000350: 0063 0300 0000 0000 0000 0000 0000 1400  .c..............
+00000360: 0000 0800 0000 4300 0000 7308 0200 0074  ......C...s....t
+00000370: 00a0 0174 026a 0364 0119 00a1 017d 037c  ...t.j.d.....}.|
+00000380: 016a 04a0 05a1 00a0 06a1 0044 005d 2a5c  .j.........D.]*\
+00000390: 027d 047d 057c 037c 0574 0274 077c 0483  .}.}.|.|.t.t.|..
+000003a0: 016a 0864 0118 0064 0064 0085 0266 0219  .j.d...d.d...f..
+000003b0: 0014 0037 007d 0371 1e74 00a0 0174 026a  ...7.}.q.t...t.j
+000003c0: 0364 0119 00a1 017d 0664 027d 0764 027d  .d.....}.d.}.d.}
+000003d0: 087c 00a0 06a1 0044 005d 885c 027d 097d  .|.....D.].\.}.}
+000003e0: 0a74 00a0 0174 026a 0364 0119 00a1 017d  .t...t.j.d.....}
+000003f0: 0b7c 0a64 0319 006a 04a0 05a1 00a0 06a1  .|.d...j........
+00000400: 0044 005d 2a5c 027d 047d 057c 0b7c 0574  .D.]*\.}.}.|.|.t
+00000410: 0274 077c 0483 016a 0864 0118 0064 0064  .t.|...j.d...d.d
+00000420: 0085 0266 0219 0014 0037 007d 0b71 947c  ...f.....7.}.q.|
+00000430: 0674 00a0 097c 037c 0b18 00a1 017c 0a64  .t...|.|.....|.d
+00000440: 0419 0014 0037 007d 067c 077c 0a64 0419  .....7.}.|.|.d..
+00000450: 0037 007d 077c 087c 0a64 0519 0037 007d  .7.}.|.|.d...7.}
+00000460: 0871 6a7c 067c 071b 007c 0367 027d 0c64  .qj|.|...|.g.}.d
+00000470: 027d 0d64 027d 0e7c 00a0 0aa1 0044 005d  .}.d.}.|.....D.]
+00000480: 267d 0a7c 0d7c 0a64 0419 0037 007d 0d7c  &}.|.|.d...7.}.|
+00000490: 0e7c 0a64 0419 007c 0a64 0419 0014 0037  .|.d...|.d.....7
+000004a0: 007d 0e90 0171 107c 0d7c 0d14 007c 0e1b  .}...q.|.|...|..
+000004b0: 007d 0f64 027d 107c 00a0 0aa1 0044 005d  .}.d.}.|.....D.]
+000004c0: 1e7d 0a7c 107c 0a64 0419 0064 0614 007c  .}.|.|.d...d...|
+000004d0: 0a64 0719 0014 0037 007d 1090 0171 507c  .d.....7.}...qP|
+000004e0: 107c 071d 007d 1064 027d 117c 00a0 0aa1  .|...}.d.}.|....
+000004f0: 0044 005d 267d 0a7c 117c 0a64 0419 0074  .D.]&}.|.|.d...t
+00000500: 0964 067c 0a64 0719 0014 007c 1018 0083  .d.|.d.....|....
+00000510: 0114 0037 007d 1190 0171 847c 117c 077c  ...7.}...q.|.|.|
+00000520: 1014 001d 007d 1174 0b64 0864 0984 007c  .....}.t.d.d...|
+00000530: 00a0 0aa1 0044 0083 0183 017d 1264 0a74  .....D.....}.d.t
+00000540: 0c6a 0d14 0074 0ca0 0e7c 1264 0ba1 0214  .j...t...|.d....
+00000550: 007d 1374 00a0 0f7c 0f7c 107c 117c 087c  .}.t...|.|.|.|.|
+00000560: 1367 057c 0c64 0219 0066 02a1 017c 0c64  .g.|.d...f...|.d
+00000570: 0119 0067 0253 0029 0c4e e901 0000 0072  ...g.S.).N.....r
+00000580: 0100 0000 da04 7369 7465 da04 6172 6561  ......site..area
+00000590: da06 766f 6c75 6d65 720d 0000 00da 0966  ..volumer......f
+000005a0: 6163 655f 6469 7374 6301 0000 0000 0000  ace_distc.......
+000005b0: 0000 0000 0002 0000 0003 0000 0073 0000  .............s..
+000005c0: 0073 1600 0000 7c00 5d0e 7d01 7c01 6400  .s....|.].}.|.d.
+000005d0: 1900 5600 0100 7102 6401 5300 2902 7224  ..V...q.d.S.).r$
+000005e0: 0000 004e a900 2902 da02 2e30 da0d 6e65  ...N..)....0..ne
+000005f0: 6967 6862 6f72 5f73 6974 6572 2500 0000  ighbor_siter%...
+00000600: 7225 0000 00fa 562f 5573 6572 732f 6164  r%....V/Users/ad
+00000610: 616d 2f50 7963 6861 726d 5072 6f6a 6563  am/PycharmProjec
+00000620: 7473 2f70 7953 4950 4645 4e4e 2f70 7973  ts/pySIPFENN/pys
+00000630: 6970 6665 6e6e 2f64 6573 6372 6970 746f  ipfenn/descripto
+00000640: 7244 6566 696e 6974 696f 6e73 2f4b 5332  rDefinitions/KS2
+00000650: 3032 325f 6469 6c75 7465 2e70 79da 093c  022_dilute.py..<
+00000660: 6765 6e65 7870 723e 4200 0000 f300 0000  genexpr>B.......
+00000670: 007a 256c 6f63 616c 5f65 6e76 5f66 756e  .z%local_env_fun
+00000680: 6374 696f 6e2e 3c6c 6f63 616c 733e 2e3c  ction.<locals>.<
+00000690: 6765 6e65 7870 723e 6755 5555 5555 55f5  genexpr>gUUUUUU.
+000006a0: 3f67 0000 0000 0000 0840 2910 da02 6e70  ?g.......@)...np
+000006b0: da05 7a65 726f 73da 1061 7474 7269 6275  ..zeros..attribu
+000006c0: 7465 5f6d 6174 7269 78da 0573 6861 7065  te_matrix..shape
+000006d0: da07 7370 6563 6965 73da 0f67 6574 5f65  ..species..get_e
+000006e0: 6c5f 616d 745f 6469 6374 da05 6974 656d  l_amt_dict..item
+000006f0: 7372 0300 0000 da01 5ada 0361 6273 da06  sr......Z..abs..
+00000700: 7661 6c75 6573 da03 6d69 6eda 046d 6174  values..min..mat
+00000710: 68da 0270 69da 0370 6f77 da0b 636f 6e63  h..pi..pow..conc
+00000720: 6174 656e 6174 6529 14da 096c 6f63 616c  atenate)...local
+00000730: 5f65 6e76 7221 0000 00da 0673 7472 7563  _envr!.....struc
+00000740: 74da 106c 6f63 616c 5f61 7474 7269 6275  t..local_attribu
+00000750: 7465 73da 036b 6579 da05 7661 6c75 65da  tes..key..value.
+00000760: 0f64 6966 665f 6174 7472 6962 7574 6573  .diff_attributes
+00000770: da0c 746f 7461 6c5f 7765 6967 6874 7223  ..total_weightr#
+00000780: 0000 00da 0369 6e64 7227 0000 00da 136e  .....indr'.....n
+00000790: 6569 6768 626f 725f 6174 7472 6962 7574  eighbor_attribut
+000007a0: 6573 da1f 656c 656d 656e 7461 6c5f 7072  es..elemental_pr
+000007b0: 6f70 6572 7469 6573 5f61 7474 7269 6275  operties_attribu
+000007c0: 7465 73da 0761 7665 7261 6765 da08 7661  tes..average..va
+000007d0: 7269 616e 6365 da0d 6566 665f 636f 6f72  riance..eff_coor
+000007e0: 645f 6e75 6dda 0c62 6c65 6e5f 6176 6572  d_num..blen_aver
+000007f0: 6167 65da 0862 6c65 6e5f 7661 72da 0a73  age..blen_var..s
+00000800: 7068 6572 655f 7261 64da 0d73 7068 6572  phere_rad..spher
+00000810: 655f 766f 6c75 6d65 7225 0000 0072 2500  e_volumer%...r%.
+00000820: 0000 7228 0000 00da 126c 6f63 616c 5f65  ..r(.....local_e
+00000830: 6e76 5f66 756e 6374 696f 6e20 0000 0073  nv_function ...s
+00000840: 4600 0000 0001 1001 1601 2401 1001 0401  F.........$.....
+00000850: 0401 1001 1001 1a01 2401 1a01 0c01 0e01  ........$.......
+00000860: 0c02 0401 0401 0c01 0c01 1801 0c03 0401  ................
+00000870: 0c01 1c01 0802 0401 0c01 2401 0c02 1601  ..........$.....
+00000880: 1601 0401 14ff 0202 06fe 724b 0000 0063  ..........rK...c
+00000890: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000008a0: 0300 0000 0300 0000 7352 0000 007c 006a  ........sR...|.j
+000008b0: 0089 0174 0174 0288 0183 0183 0189 0087  ...t.t..........
+000008c0: 0087 0166 0264 0164 0284 0888 0044 0083  ...f.d.d.....D..
+000008d0: 017d 0174 0388 0083 0174 037c 0183 0118  .}.t.....t.|....
+000008e0: 0064 036b 0272 427c 0164 0419 0053 0074  .d.k.rB|.d...S.t
+000008f0: 0464 0583 0101 0074 0582 0164 0053 0029  .d.....t...d.S.)
+00000900: 064e 6301 0000 0000 0000 0000 0000 0002  .Nc.............
+00000910: 0000 0005 0000 0013 0000 0073 2200 0000  ...........s"...
+00000920: 6700 7c00 5d1a 7d01 8800 7c01 1900 6400  g.|.].}...|...d.
+00000930: 6b02 7204 8801 a000 7c01 a101 9102 7104  k.r.....|.....q.
+00000940: 5300 a901 7220 0000 0029 01da 0569 6e64  S...r ...)...ind
+00000950: 6578 2902 7226 0000 00da 0273 70a9 025a  ex).r&.....sp..Z
+00000960: 0773 7043 6f75 6e74 5a07 7370 6f4c 6973  .spCountZ.spoLis
+00000970: 7472 2500 0000 7228 0000 00da 0a3c 6c69  tr%...r(.....<li
+00000980: 7374 636f 6d70 3e4b 0000 0072 2a00 0000  stcomp>K...r*...
+00000990: 7a1e 6669 6e64 4469 6c75 7465 2e3c 6c6f  z.findDilute.<lo
+000009a0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+000009b0: 7220 0000 0072 0100 0000 7a6c 4375 7374  r ...r....zlCust
+000009c0: 6f6d 2064 696c 7574 6520 7374 7275 6374  om dilute struct
+000009d0: 7572 6520 6465 7363 7269 7074 6f72 2063  ure descriptor c
+000009e0: 616c 6375 6c61 7469 6f6e 2069 7320 6465  alculation is de
+000009f0: 6669 6e65 6420 6f6e 6c79 206f 6e65 2064  fined only one d
+00000a00: 696c 7574 6520 7370 6563 6965 7320 696e  ilute species in
+00000a10: 2061 2073 696e 676c 6520 656c 656d 656e   a single elemen
+00000a20: 7420 6d61 7472 6978 2906 da10 7370 6563  t matrix)...spec
+00000a30: 6965 735f 616e 645f 6f63 6375 da04 6469  ies_and_occu..di
+00000a40: 6374 7207 0000 00da 036c 656e da05 7072  ctr......len..pr
+00000a50: 696e 74da 0c52 756e 7469 6d65 4572 726f  int..RuntimeErro
+00000a60: 7229 0272 3b00 0000 5a08 7370 4469 6c75  r).r;...Z.spDilu
+00000a70: 7465 7225 0000 0072 4f00 0000 7228 0000  ter%...rO...r(..
+00000a80: 00da 0a66 696e 6444 696c 7574 6548 0000  ...findDiluteH..
+00000a90: 0073 0e00 0000 0001 0601 0c01 1401 1401  .s..............
+00000aa0: 0802 0801 7256 0000 00da 0470 7572 6563  ....rV.....purec
+00000ab0: 0300 0000 0000 0000 0000 0000 1300 0000  ................
+00000ac0: 0600 0000 4300 0000 73fe 0100 0074 007c  ....C...s....t.|
+00000ad0: 007c 0283 027d 0374 017c 0174 0283 0272  .|...}.t.|.t...r
+00000ae0: 7067 007d 0474 0374 047c 016a 057c 006a  pg.}.t.t.|.j.|.j
+00000af0: 0583 0283 0144 005d 205c 027d 055c 027d  .....D.] \.}.\.}
+00000b00: 067d 077c 067c 076b 0372 2a7c 04a0 067c  .}.|.|.k.r*|...|
+00000b10: 05a1 0101 0071 2a71 2a74 077c 0483 0164  .....q*q*t.|...d
+00000b20: 016b 0272 627c 0464 0219 007d 0471 ac74  .k.rb|.d...}.q.t
+00000b30: 0864 0383 0101 0074 0982 016e 3c7c 0164  .d.....t...n<|.d
+00000b40: 046b 0272 a87c 00a0 0aa1 007d 0174 0b7c  .k.r.|.....}.t.|
+00000b50: 016a 0c83 0144 005d 127d 087c 01a0 0d7c  .j...D.].}.|...|
+00000b60: 0864 0569 01a1 0101 0071 8a74 0e7c 0083  .d.i.....q.t.|..
+00000b70: 017d 046e 0474 0982 0174 0f7c 0164 0664  .}.n.t...t.|.d.d
+00000b80: 0764 088d 037d 0974 107c 09a0 11a1 0064  .d...}.t.|.....d
+00000b90: 0919 0083 017d 0a74 1083 007d 0b7c 0ba0  .....}.t...}.|..
+00000ba0: 067c 03a0 127c 04a1 01a1 0101 007c 0b64  .|...|.......|.d
+00000bb0: 0219 0064 0a19 007d 0c74 1374 0474 1474  ...d...}.t.t.t.t
+00000bc0: 077c 0a83 0183 0164 0b64 0c84 007c 0a44  .|.....d.d...|.D
+00000bd0: 0083 0183 0283 017d 0d64 0d7c 0d7c 043c  .......}.d.|.|.<
+00000be0: 007c 0c44 005d 187d 0e7c 0d7c 0e19 00a0  .|.D.].}.|.|....
+00000bf0: 067c 0c7c 0e19 00a1 0101 0090 0171 1869  .|.|.........q.i
+00000c00: 007d 0f7c 0d44 005d 427d 0e64 0ea0 1574  .}.|.D.]B}.d...t
+00000c10: 167c 0d7c 0e19 0083 01a1 017d 107c 107c  .|.|.......}.|.|
+00000c20: 0f76 0090 0172 6a7c 0f7c 1019 00a0 067c  .v...rj|.|.....|
+00000c30: 0ea1 0101 006e 107c 0fa0 177c 107c 0e67  .....n.|...|.|.g
+00000c40: 0169 01a1 0101 0090 0171 3a7c 0f64 0d3d  .i.......q:|.d.=
+00000c50: 0074 1374 0464 0f64 0c84 007c 0fa0 18a1  .t.t.d.d...|....
+00000c60: 0044 0083 0164 1064 0c84 007c 0fa0 18a1  .D...d.d...|....
+00000c70: 0044 0083 0183 0283 017d 117c 1144 005d  .D.......}.|.D.]
+00000c80: 227d 0e7c 03a0 197c 0ea1 0167 017d 127c  "}.|...|...g.}.|
+00000c90: 0b7c 127c 117c 0e19 0014 0037 007d 0b90  .|.|.|.....7.}..
+00000ca0: 0171 b274 1aa0 1b64 1164 0c84 007c 0b44  .q.t...d.d...|.D
+00000cb0: 0083 01a1 0174 1aa0 1b64 1264 0c84 007c  .....t...d.d...|
+00000cc0: 0b44 0083 01a1 0166 0253 0029 134e 7220  .D.....f.S.).Nr 
+00000cd0: 0000 0072 0100 0000 7a49 5369 7465 7320  ...r....zISites 
+00000ce0: 696e 2074 6865 2070 726f 7669 6465 6420  in the provided 
+00000cf0: 6261 7365 2073 7472 7563 7475 7265 206d  base structure m
+00000d00: 6174 6368 6564 2074 6865 2069 6e76 6573  atched the inves
+00000d10: 7469 6761 7465 6420 6f6e 6520 6578 6163  tigated one exac
+00000d20: 746c 7972 5700 0000 da01 4167 fca9 f1d2  tlyrW.....Ag....
+00000d30: 4d62 503f 679a 9999 9999 99b9 3f29 02da  MbP?g.......?)..
+00000d40: 0773 796d 7072 6563 da0f 616e 676c 655f  .symprec..angle_
+00000d50: 746f 6c65 7261 6e63 65da 1065 7175 6976  tolerance..equiv
+00000d60: 616c 656e 745f 6174 6f6d 7372 0d00 0000  alent_atomsr....
+00000d70: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00000d80: 0003 0000 0053 0000 0073 1200 0000 6700  .....S...s....g.
+00000d90: 7c00 5d0a 7d01 7c01 6701 9102 7104 5300  |.].}.|.g...q.S.
+00000da0: 7225 0000 0072 2500 0000 2902 7226 0000  r%...r%...).r&..
+00000db0: 00da 0165 7225 0000 0072 2500 0000 7228  ...er%...r%...r(
+00000dc0: 0000 0072 5000 0000 7600 0000 722a 0000  ...rP...v...r*..
+00000dd0: 007a 2f67 656e 6572 6174 655f 766f 726f  .z/generate_voro
+00000de0: 6e6f 695f 6174 7472 6962 7574 6573 2e3c  noi_attributes.<
+00000df0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+00000e00: 703e 5a06 6469 6c75 7465 da00 6301 0000  p>Z.dilute..c...
+00000e10: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00000e20: 0053 0000 0073 1400 0000 6700 7c00 5d0c  .S...s....g.|.].
+00000e30: 7d01 7c01 6400 1900 9102 7104 5300 a901  }.|.d.....q.S...
+00000e40: 7201 0000 0072 2500 0000 a902 7226 0000  r....r%.....r&..
+00000e50: 00da 0167 7225 0000 0072 2500 0000 7228  ...gr%...r%...r(
+00000e60: 0000 0072 5000 0000 8600 0000 722a 0000  ...rP.......r*..
+00000e70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000e80: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00000e90: 007c 005d 0c7d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+00000ea0: 0453 0072 2500 0000 2901 7253 0000 0072  .S.r%...).rS...r
+00000eb0: 5f00 0000 7225 0000 0072 2500 0000 7228  _...r%...r%...r(
+00000ec0: 0000 0072 5000 0000 8700 0000 722a 0000  ...rP.......r*..
+00000ed0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00000ee0: 0000 0400 0000 5300 0000 7314 0000 0067  ......S...s....g
+00000ef0: 007c 005d 0c7d 017c 0164 0019 0091 0271  .|.].}.|.d.....q
+00000f00: 0453 0072 5e00 0000 7225 0000 00a9 0272  .S.r^...r%.....r
+00000f10: 2600 0000 723e 0000 0072 2500 0000 7225  &...r>...r%...r%
+00000f20: 0000 0072 2800 0000 7250 0000 008d 0000  ...r(...rP......
+00000f30: 0072 2a00 0000 6301 0000 0000 0000 0000  .r*...c.........
+00000f40: 0000 0002 0000 0004 0000 0053 0000 0073  ...........S...s
+00000f50: 1400 0000 6700 7c00 5d0c 7d01 7c01 6400  ....g.|.].}.|.d.
+00000f60: 1900 9102 7104 5300 724c 0000 0072 2500  ....q.S.rL...r%.
+00000f70: 0000 7261 0000 0072 2500 0000 7225 0000  ..ra...r%...r%..
+00000f80: 0072 2800 0000 7250 0000 008d 0000 0072  .r(...rP.......r
+00000f90: 2a00 0000 291c da17 4c6f 6361 6c41 7474  *...)...LocalAtt
+00000fa0: 7269 6275 7465 4765 6e65 7261 746f 72da  ributeGenerator.
+00000fb0: 0a69 7369 6e73 7461 6e63 6572 0200 0000  .isinstancer....
+00000fc0: da09 656e 756d 6572 6174 65da 037a 6970  ..enumerate..zip
+00000fd0: da05 7369 7465 73da 0661 7070 656e 6472  ..sites..appendr
+00000fe0: 5300 0000 7254 0000 00da 0954 7970 6545  S...rT.....TypeE
+00000ff0: 7272 6f72 da04 636f 7079 da03 7365 7472  rror..copy..setr
+00001000: 2f00 0000 da0f 7265 706c 6163 655f 7370  /.....replace_sp
+00001010: 6563 6965 7372 5600 0000 7205 0000 00da  eciesrV...r.....
+00001020: 046c 6973 74da 1467 6574 5f73 796d 6d65  .list..get_symme
+00001030: 7472 795f 6461 7461 7365 74da 2467 656e  try_dataset.$gen
+00001040: 6572 6174 655f 6c6f 6361 6c5f 6174 7472  erate_local_attr
+00001050: 6962 7574 6573 5f64 696c 7574 6553 6974  ibutes_diluteSit
+00001060: 6572 5200 0000 da05 7261 6e67 65da 046a  erR.....range..j
+00001070: 6f69 6eda 0373 7472 da06 7570 6461 7465  oin..str..update
+00001080: 7234 0000 00da 1967 656e 6572 6174 655f  r4.....generate_
+00001090: 6c6f 6361 6c5f 6174 7472 6962 7574 6573  local_attributes
+000010a0: 722b 0000 00da 0561 7272 6179 2913 723b  r+.....array).r;
+000010b0: 0000 00da 0a62 6173 6553 7472 7563 74da  .....baseStruct.
+000010c0: 0b6c 6f63 616c 5f66 756e 6374 da0f 6c6f  .local_funct..lo
+000010d0: 6361 6c5f 6765 6e65 7261 746f 725a 0a64  cal_generatorZ.d
+000010e0: 696c 7574 6553 6974 65da 0169 5a03 7331  iluteSite..iZ.s1
+000010f0: 735a 0373 3273 724e 0000 005a 0873 7067  sZ.s2srN...Z.spg
+00001100: 4162 6173 655a 136f 7269 6769 6e61 6c45  AbaseZ.originalE
+00001110: 7175 6976 616c 656e 7473 da0e 6174 7472  quivalents..attr
+00001120: 6962 7574 655f 6c69 7374 5a12 6e65 6967  ibute_listZ.neig
+00001130: 6862 6f72 7346 6163 6573 4469 6374 5a0d  hborsFacesDictZ.
+00001140: 7369 7465 4c43 4570 6172 616d 73da 0573  siteLCEparams..s
+00001150: 6974 654e 5a10 6571 7569 7661 6c65 6e74  iteNZ.equivalent
+00001160: 4772 6f75 7073 da06 7061 7261 6d73 da1d  Groups..params..
+00001170: 6571 7569 7661 6c65 6e74 5369 7465 734d  equivalentSitesM
+00001180: 756c 7469 706c 6963 6974 6965 73da 0f6c  ultiplicities..l
+00001190: 6f63 616c 4174 7472 6962 7574 6573 7225  ocalAttributesr%
+000011a0: 0000 0072 2500 0000 7228 0000 00da 1b67  ...r%...r(.....g
+000011b0: 656e 6572 6174 655f 766f 726f 6e6f 695f  enerate_voronoi_
+000011c0: 6174 7472 6962 7574 6573 5200 0000 7354  attributesR...sT
+000011d0: 0000 0000 010a 030a 0104 011e 0108 010a  ................
+000011e0: 0104 010c 010a 0208 0106 0108 0108 010e  ................
+000011f0: 0110 020a 0204 030e 0110 0306 0110 030c  ................
+00001200: 0320 0108 0108 0116 0304 0108 0112 010a  . ..............
+00001210: 0110 0214 0106 0202 0112 0110 ff02 ff04  ................
+00001220: 0408 010c 0114 0272 7e00 0000 6300 0000  .......r~...c...
+00001230: 0000 0000 0000 0000 0000 0000 0004 0000  ................
+00001240: 0040 0000 0073 3000 0000 6500 5a01 6400  .@...s0...e.Z.d.
+00001250: 5a02 6503 6401 6401 6402 8d02 6601 6403  Z.e.d.d.d...f.d.
+00001260: 6404 8401 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
+00001270: 6408 8400 5a06 6409 5300 290a 7262 0000  d...Z.d.S.).rb..
+00001280: 0046 2902 da15 636f 6d70 7574 655f 6164  .F)...compute_ad
+00001290: 6a5f 6e65 6967 6862 6f72 73da 0d65 7874  j_neighbors..ext
+000012a0: 7261 5f6e 6e5f 696e 666f 6304 0000 0000  ra_nn_infoc.....
+000012b0: 0000 0000 0000 0004 0000 0002 0000 0043  ...............C
+000012c0: 0000 0073 1600 0000 7c03 7c00 5f00 7c01  ...s....|.|._.|.
+000012d0: 7c00 5f01 7c02 7c00 5f02 6400 5300 a901  |._.|.|._.d.S...
+000012e0: 4e29 03da 0967 656e 6572 6174 6f72 723b  N)...generatorr;
+000012f0: 0000 00da 0866 756e 6374 696f 6e29 04da  .....function)..
+00001300: 0473 656c 6672 3b00 0000 da0e 6c6f 6361  .selfr;.....loca
+00001310: 6c5f 656e 765f 6675 6e63 da0c 6e6e 5f67  l_env_func..nn_g
+00001320: 656e 6572 6174 6f72 7225 0000 0072 2500  eneratorr%...r%.
+00001330: 0000 7228 0000 00da 085f 5f69 6e69 745f  ..r(.....__init_
+00001340: 5f92 0000 0073 0600 0000 0001 0601 0601  _....s..........
+00001350: 7a20 4c6f 6361 6c41 7474 7269 6275 7465  z LocalAttribute
+00001360: 4765 6e65 7261 746f 722e 5f5f 696e 6974  Generator.__init
+00001370: 5f5f 6302 0000 0000 0000 0000 0000 0003  __c.............
+00001380: 0000 0005 0000 0043 0000 0073 2600 0000  .......C...s&...
+00001390: 7c00 6a00 a001 7c00 6a02 7c01 a102 7d02  |.j...|.j.|...}.
+000013a0: 7c00 a003 7c02 7c00 6a02 7c01 1900 7c00  |...|.|.j.|...|.
+000013b0: 6a02 a103 5300 7281 0000 0029 0472 8200  j...S.r....).r..
+000013c0: 0000 da15 6765 745f 766f 726f 6e6f 695f  ....get_voronoi_
+000013d0: 706f 6c79 6865 6472 6172 3b00 0000 7283  polyhedrar;...r.
+000013e0: 0000 0029 0372 8400 0000 da01 6e72 3a00  ...).r......nr:.
+000013f0: 0000 7225 0000 0072 2500 0000 7228 0000  ..r%...r%...r(..
+00001400: 0072 7300 0000 9700 0000 7304 0000 0000  .rs.......s.....
+00001410: 0110 017a 314c 6f63 616c 4174 7472 6962  ...z1LocalAttrib
+00001420: 7574 6547 656e 6572 6174 6f72 2e67 656e  uteGenerator.gen
+00001430: 6572 6174 655f 6c6f 6361 6c5f 6174 7472  erate_local_attr
+00001440: 6962 7574 6573 6302 0000 0000 0000 0000  ibutesc.........
+00001450: 0000 0005 0000 0005 0000 0043 0000 0073  ...........C...s
+00001460: 4600 0000 7c00 6a00 a001 7c00 6a02 7c01  F...|.j...|.j.|.
+00001470: a102 7d02 7c00 a003 7c02 7c00 6a02 7c01  ..}.|...|.|.j.|.
+00001480: 1900 7c00 6a02 a103 7d03 6401 6402 8400  ..|.j...}.d.d...
+00001490: 7c02 a004 a100 4400 8301 7d04 7c03 a005  |.....D...}.|...
+000014a0: 7c04 a101 0100 7c03 5300 2903 4e63 0100  |.....|.S.).Nc..
+000014b0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
+000014c0: 0000 5300 0000 7342 0000 0069 007c 005d  ..S...sB...i.|.]
+000014d0: 3a7d 017c 0164 0019 006a 0074 017c 0164  :}.|.d...j.t.|.d
+000014e0: 0019 006a 0283 0174 037c 0164 0119 0064  ...j...t.|.d...d
+000014f0: 0283 0274 037c 0164 0319 0064 0283 027c  ...t.|.d...d...|
+00001500: 0164 0419 0067 0493 0271 0453 0029 0572  .d...g...q.S.).r
+00001510: 2100 0000 7224 0000 0072 0d00 0000 7222  !...r$...r....r"
+00001520: 0000 00da 076e 5f76 6572 7473 2904 724d  .....n_verts).rM
+00001530: 0000 0072 7100 0000 722f 0000 00da 0572  ...rq...r/.....r
+00001540: 6f75 6e64 7261 0000 0072 2500 0000 7225  oundra...r%...r%
+00001550: 0000 0072 2800 0000 da0a 3c64 6963 7463  ...r(.....<dictc
+00001560: 6f6d 703e 9f00 0000 730e 0000 0006 0502  omp>....s.......
+00001570: fb08 010c 010c 010c 0106 fd7a 504c 6f63  ...........zPLoc
+00001580: 616c 4174 7472 6962 7574 6547 656e 6572  alAttributeGener
+00001590: 6174 6f72 2e67 656e 6572 6174 655f 6c6f  ator.generate_lo
+000015a0: 6361 6c5f 6174 7472 6962 7574 6573 5f64  cal_attributes_d
+000015b0: 696c 7574 6553 6974 652e 3c6c 6f63 616c  iluteSite.<local
+000015c0: 733e 2e3c 6469 6374 636f 6d70 3e29 0672  s>.<dictcomp>).r
+000015d0: 8200 0000 7288 0000 0072 3b00 0000 7283  ....r....r;...r.
+000015e0: 0000 0072 3400 0000 7267 0000 0029 0572  ...r4...rg...).r
+000015f0: 8400 0000 7289 0000 0072 3a00 0000 5a10  ....r....r:...Z.
+00001600: 6c6f 6361 6c5f 656e 765f 7265 7375 6c74  local_env_result
+00001610: da0d 6e65 6967 6862 6f72 5f64 6963 7472  ..neighbor_dictr
+00001620: 2500 0000 7225 0000 0072 2800 0000 726e  %...r%...r(...rn
+00001630: 0000 009b 0000 0073 0e00 0000 0001 1001  .......s........
+00001640: 1602 0605 06fb 0607 0a02 7a3c 4c6f 6361  ..........z<Loca
+00001650: 6c41 7474 7269 6275 7465 4765 6e65 7261  lAttributeGenera
+00001660: 746f 722e 6765 6e65 7261 7465 5f6c 6f63  tor.generate_loc
+00001670: 616c 5f61 7474 7269 6275 7465 735f 6469  al_attributes_di
+00001680: 6c75 7465 5369 7465 4e29 07da 085f 5f6e  luteSiteN)...__n
+00001690: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
+000016a0: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
+000016b0: 0400 0000 7287 0000 0072 7300 0000 726e  ....r....rs...rn
+000016c0: 0000 0072 2500 0000 7225 0000 0072 2500  ...r%...r%...r%.
+000016d0: 0000 7228 0000 0072 6200 0000 9100 0000  ..r(...rb.......
+000016e0: 7306 0000 0008 0114 0508 0472 6200 0000  s..........rb...
+000016f0: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
+00001700: 0007 0000 0043 0000 0073 d400 0000 7400  .....C...s....t.
+00001710: a001 7400 a002 7c00 6400 6400 8502 6401  ..t...|.d.d...d.
+00001720: 6602 1900 a101 a101 7d02 6401 7d03 6700  f.......}.d.}.g.
+00001730: 7d04 7c02 4400 5d62 7d05 7c00 6400 6400  }.|.D.]b}.|.d.d.
+00001740: 8502 6401 6602 1900 7c05 6b02 7d06 7400  ..d.f...|.k.}.t.
+00001750: a003 7400 a004 7c06 7c01 a102 7c01 a102  ..t...|.|...|...
+00001760: 6401 1900 7d07 7c07 7c03 6b04 7278 7c04  d...}.|.|.k.rx|.
+00001770: a005 a100 0100 7c04 a006 7c05 a101 0100  ......|...|.....
+00001780: 7c07 7d03 7128 7c07 7c03 6b02 7228 7c04  |.}.q(|.|.k.r(|.
+00001790: a006 7c05 a101 0100 7128 7400 a007 7c00  ..|.....q(t...|.
+000017a0: 6401 6400 6400 8502 6602 1900 a101 7d08  d.d.d...f.....}.
+000017b0: 7c04 4400 5d20 7d09 7c08 7408 7409 7c09  |.D.] }.|.t.t.|.
+000017c0: 8301 6402 1800 6400 6400 8502 6602 1900  ..d...d.d...f...
+000017d0: 3700 7d08 71a6 7c08 740a 7c04 8301 1b00  7.}.q.|.t.|.....
+000017e0: 5300 2903 4e72 0100 0000 7220 0000 0029  S.).Nr....r ...)
+000017f0: 0b72 2b00 0000 da06 756e 6971 7565 da05  .r+.....unique..
+00001800: 7261 7665 6cda 0b65 7870 616e 645f 6469  ravel..expand_di
+00001810: 6d73 da03 7375 6dda 0563 6c65 6172 7267  ms..sum..clearrg
+00001820: 0000 00da 0a7a 6572 6f73 5f6c 696b 6572  .....zeros_liker
+00001830: 2d00 0000 da03 696e 7472 5300 0000 290a  -.....intrS...).
+00001840: da14 6174 7472 6962 7574 655f 7072 6f70  ..attribute_prop
+00001850: 6572 7469 6573 da04 6178 6973 da06 7363  erties..axis..sc
+00001860: 6f72 6573 da0e 6d61 785f 6f63 6375 7272  ores..max_occurr
+00001870: 656e 6365 da0c 746f 705f 656c 656d 656e  ence..top_elemen
+00001880: 7473 da05 7363 6f72 65da 0874 656d 706c  ts..score..templ
+00001890: 6174 65da 0563 6f75 6e74 da06 6f75 7470  ate..count..outp
+000018a0: 7574 da04 656c 656d 7225 0000 0072 2500  ut..elemr%...r%.
+000018b0: 0000 7228 0000 00da 0b6d 6167 7069 655f  ..r(.....magpie_
+000018c0: 6d6f 6465 ab00 0000 7320 0000 0000 011c  mode....s ......
+000018d0: 0104 0104 0108 0114 0118 0108 0108 010a  ................
+000018e0: 0106 0108 010c 0116 0108 011e 0172 a200  .............r..
+000018f0: 0000 2901 723b 0000 0063 0200 0000 0000  ..).r;...c......
+00001900: 0000 0000 0000 1400 0000 0e00 0000 0300  ................
+00001910: 0000 73be 0300 0074 007c 007c 0164 018d  ..s....t.|.|.d..
+00001920: 025c 027d 027d 0374 01a0 0274 016a 0374  .\.}.}.t...t.j.t
+00001930: 016a 047c 0264 0264 038d 0274 016a 0474  .j.|.d.d...t.j.t
+00001940: 01a0 057c 0274 016a 047c 0264 0264 038d  ...|.t.j.|.d.d..
+00001950: 0218 00a1 0164 0264 038d 0274 016a 067c  .....d.d...t.j.|
+00001960: 0264 0264 038d 0274 016a 077c 0264 0264  .d.d...t.j.|.d.d
+00001970: 038d 0274 016a 077c 0264 0264 038d 0274  ...t.j.|.d.d...t
+00001980: 016a 067c 0264 0264 038d 0218 0066 0564  .j.|.d.d.....f.d
+00001990: 0464 038d 02a0 0864 04a1 0174 016a 0374  .d.....d...t.j.t
+000019a0: 016a 047c 0364 0264 038d 0274 016a 077c  .j.|.d.d...t.j.|
+000019b0: 0364 0264 038d 0274 016a 067c 0364 0264  .d.d...t.j.|.d.d
+000019c0: 038d 0218 0074 016a 0474 01a0 057c 0374  .....t.j.t...|.t
+000019d0: 016a 047c 0364 0264 038d 0218 00a1 0164  .j.|.d.d.......d
+000019e0: 0264 038d 0274 016a 077c 0364 0264 038d  .d...t.j.|.d.d..
+000019f0: 0274 016a 067c 0364 0264 038d 0274 097c  .t.j.|.d.d...t.|
+00001a00: 0383 0166 0664 0464 038d 02a0 0864 04a1  ...f.d.d.....d..
+00001a10: 0166 02a1 017d 047c 0464 0505 0019 007c  .f...}.|.d.....|
+00001a20: 0464 0619 001d 0003 003c 007c 0464 0705  .d.......<.|.d..
+00001a30: 0019 007c 0464 0619 001d 0003 003c 007c  ...|.d.......<.|
+00001a40: 0464 0805 0019 007c 0464 0619 001d 0003  .d.....|.d......
+00001a50: 003c 007c 0464 0905 0019 007c 0464 0a19  .<.|.d.....|.d..
+00001a60: 001d 0003 003c 0074 01a0 0a7c 0467 0064  .....<.t...|.g.d
+00001a70: 0ba2 01a1 027d 047c 0464 0c05 0019 0074  .....}.|.d.....t
+00001a80: 0b7c 0383 017c 006a 0c1b 0039 0003 003c  .|...|.j...9...<
+00001a90: 0069 007d 057c 006a 0d44 005d 567d 067c  .i.}.|.j.D.]V}.|
+00001aa0: 06a0 0ea1 00a0 0fa1 0044 005d 425c 027d  .........D.]B\.}
+00001ab0: 077d 087c 077c 0576 0090 0172 c27c 057c  .}.|.|.v...r.|.|
+00001ac0: 0705 0019 007c 0874 0b7c 006a 0d83 011b  .....|.t.|.j....
+00001ad0: 0037 0003 003c 006e 127c 0874 0b7c 006a  .7...<.n.|.t.|.j
+00001ae0: 0d83 011b 007c 057c 073c 0090 0171 9490  .....|.|.<...q..
+00001af0: 0171 8464 0d7d 0964 0e44 005d 3689 0074  .q.d.}.d.D.]6..t
+00001b00: 01a0 107c 047c 0974 11a0 1274 1387 0066  ...|.|.t...t...f
+00001b10: 0164 0f64 1084 087c 05a0 14a1 0044 0083  .d.d...|.....D..
+00001b20: 0183 0164 1188 001b 00a1 02a1 037d 0490  ...d.........}..
+00001b30: 0171 e474 01a0 107c 047c 0974 0b7c 0583  .q.t...|.|.t.|..
+00001b40: 01a1 037d 0464 0264 0264 0264 0264 129c  ...}.d.d.d.d.d..
+00001b50: 047d 0a64 027d 0b7c 05a0 0fa1 0044 005d  .}.d.}.|.....D.]
+00001b60: a25c 027d 077d 087c 0a64 1305 0019 007c  .\.}.}.|.d.....|
+00001b70: 0874 1574 167c 0783 016a 1764 1418 0019  .t.t.|...j.d....
+00001b80: 0064 0819 0014 0037 0003 003c 007c 0a64  .d.....7...<.|.d
+00001b90: 1505 0019 007c 0874 1574 167c 0783 016a  .....|.t.t.|...j
+00001ba0: 1764 1418 0019 0064 1619 0014 0037 0003  .d.....d.....7..
+00001bb0: 003c 007c 0a64 1705 0019 007c 0874 1574  .<.|.d.....|.t.t
+00001bc0: 167c 0783 016a 1764 1418 0019 0064 1819  .|...j.d.....d..
+00001bd0: 0014 0037 0003 003c 007c 0a64 1905 0019  ...7...<.|.d....
+00001be0: 007c 0874 1574 167c 0783 016a 1764 1418  .|.t.t.|...j.d..
+00001bf0: 0019 0064 1a19 0014 0037 0003 003c 0090  ...d.....7...<..
+00001c00: 0271 4874 1364 1b64 1c84 007c 0aa0 0fa1  .qHt.d.d...|....
+00001c10: 0044 0083 0183 017d 0b64 1244 005d 1a7d  .D.....}.d.D.].}
+00001c20: 0c74 01a0 187c 047c 0a7c 0c19 007c 0b1b  .t...|.|.|...|..
+00001c30: 00a1 027d 0490 0371 0664 027d 0d64 027d  ...}...q.d.}.d.}
+00001c40: 0e7c 05a0 0fa1 0044 005d 625c 027d 0f7d  .|.....D.]b\.}.}
+00001c50: 107c 05a0 0fa1 0044 005d 4e5c 027d 117d  .|.....D.]N\.}.}
+00001c60: 1264 1174 11a0 1964 1d74 167c 0f83 016a  .d.t...d.t.|...j
+00001c70: 1a74 167c 1183 016a 1a18 0064 1e13 0014  .t.|...j...d....
+00001c80: 00a1 0118 007d 137c 137c 0d6b 0490 0372  .....}.|.|.k...r
+00001c90: 7e7c 137d 0d7c 0e7c 137c 1014 007c 1214  ~|.}.|.|.|...|..
+00001ca0: 0037 007d 0e90 0371 4290 0371 3274 01a0  .7.}...qB..q2t..
+00001cb0: 187c 047c 0da1 027d 0474 01a0 187c 047c  .|.|...}.t...|.|
+00001cc0: 0ea1 027d 047c 04a0 1b74 016a 1ca1 017d  ...}.|...t.j...}
+00001cd0: 047c 0453 0029 1f4e 2901 7275 0000 0072  .|.S.).N).ru...r
+00001ce0: 0100 0000 2901 7299 0000 00e9 ffff ffff  ....).r.........
+00001cf0: 7211 0000 0072 0f00 0000 e907 0000 00e9  r....r..........
+00001d00: 0800 0000 e910 0000 00e9 0f00 0000 290c  ..............).
+00001d10: e904 0000 0072 0f00 0000 e909 0000 00e9  .....r..........
+00001d20: 0e00 0000 72a7 0000 0072 1f00 0000 721d  ....r....r....r.
+00001d30: 0000 00e9 1300 0000 e915 0000 00e9 1600  ................
+00001d40: 0000 e917 0000 00e9 1800 0000 e90c 0000  ................
+00001d50: 00e9 7600 0000 2905 7212 0000 0072 a400  ..v...).r....r..
+00001d60: 0000 720f 0000 00e9 0300 0000 720d 0000  ..r.........r...
+00001d70: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001d80: 0000 0500 0000 3300 0000 731a 0000 007c  ......3...s....|
+00001d90: 005d 127d 0174 00a0 017c 0188 00a1 0256  .].}.t...|.....V
+00001da0: 0001 0071 0264 0053 0072 8100 0000 2902  ...q.d.S.r....).
+00001db0: 7236 0000 0072 3800 0000 7261 0000 00a9  r6...r8...ra....
+00001dc0: 01da 0170 7225 0000 0072 2800 0000 7229  ...pr%...r(...r)
+00001dd0: 0000 00e2 0000 0072 2a00 0000 7a26 6765  .......r*...z&ge
+00001de0: 6e65 7261 7465 5f64 6573 6372 6970 746f  nerate_descripto
+00001df0: 722e 3c6c 6f63 616c 733e 2e3c 6765 6e65  r.<locals>.<gene
+00001e00: 7870 723e 6700 0000 0000 00f0 3f29 04da  xpr>g.......?)..
+00001e10: 0173 72b4 0000 00da 0164 da01 6672 b500  .sr......d..fr..
+00001e20: 0000 7220 0000 0072 b400 0000 72a9 0000  ..r ...r....r...
+00001e30: 0072 b600 0000 7212 0000 0072 b700 0000  .r....r....r....
+00001e40: e90b 0000 0063 0100 0000 0000 0000 0000  .....c..........
+00001e50: 0000 0300 0000 0400 0000 5300 0000 7314  ..........S...s.
+00001e60: 0000 0067 007c 005d 0c5c 027d 017d 027c  ...g.|.].\.}.}.|
+00001e70: 0291 0271 0453 0072 2500 0000 7225 0000  ...q.S.r%...r%..
+00001e80: 0029 0372 2600 0000 723d 0000 00da 0376  .).r&...r=.....v
+00001e90: 616c 7225 0000 0072 2500 0000 7228 0000  alr%...r%...r(..
+00001ea0: 0072 5000 0000 ec00 0000 722a 0000 007a  .rP.......r*...z
+00001eb0: 2767 656e 6572 6174 655f 6465 7363 7269  'generate_descri
+00001ec0: 7074 6f72 2e3c 6c6f 6361 6c73 3e2e 3c6c  ptor.<locals>.<l
+00001ed0: 6973 7463 6f6d 703e 6700 0000 0000 00d0  istcomp>g.......
+00001ee0: bf72 0d00 0000 291d 727e 0000 0072 2b00  .r....).r~...r+.
+00001ef0: 0000 7239 0000 00da 0573 7461 636b da04  ..r9.....stack..
+00001f00: 6d65 616e 7233 0000 0072 3500 0000 da03  meanr3...r5.....
+00001f10: 6d61 78da 0772 6573 6861 7065 72a2 0000  max..reshaper...
+00001f20: 00da 0664 656c 6574 6572 5300 0000 7223  ...deleterS...r#
+00001f30: 0000 0072 5100 0000 7230 0000 0072 3100  ...rQ...r0...r1.
+00001f40: 0000 da06 696e 7365 7274 7236 0000 0072  ....insertr6...r
+00001f50: 3800 0000 7294 0000 0072 3400 0000 722d  8...r....r4...r-
+00001f60: 0000 0072 0300 0000 7232 0000 0072 6700  ...r....r2...rg.
+00001f70: 0000 da03 6578 70da 0158 da06 6173 7479  ....exp..X..asty
+00001f80: 7065 da07 666c 6f61 7433 3229 1472 3b00  pe..float32).r;.
+00001f90: 0000 7275 0000 00da 0f64 6966 665f 7072  ..ru.....diff_pr
+00001fa0: 6f70 6572 7469 6573 7298 0000 00da 0a70  opertiesr......p
+00001fb0: 726f 7065 7274 6965 73da 0c65 6c65 6d65  roperties..eleme
+00001fc0: 6e74 5f64 6963 74da 0b63 6f6d 706f 7369  nt_dict..composi
+00001fd0: 7469 6f6e 723d 0000 0072 3e00 0000 da08  tionr=...r>.....
+00001fe0: 706f 7369 7469 6f6e da18 656c 6563 7472  position..electr
+00001ff0: 6f6e 5f6f 6363 7570 6174 696f 6e5f 6469  on_occupation_di
+00002000: 6374 da14 746f 7461 6c5f 7661 6c65 6e63  ct..total_valenc
+00002010: 655f 6661 6374 6f72 da03 6f72 62da 0e6d  e_factor..orb..m
+00002020: 6178 5f69 6f6e 6963 5f63 6861 72da 0d61  ax_ionic_char..a
+00002030: 765f 696f 6e69 635f 6368 6172 da04 6b65  v_ionic_char..ke
+00002040: 7931 da06 7661 6c75 6531 da04 6b65 7932  y1..value1..key2
+00002050: da06 7661 6c75 6532 da0a 696f 6e69 635f  ..value2..ionic_
+00002060: 6368 6172 7225 0000 0072 b300 0000 7228  charr%...r....r(
+00002070: 0000 00da 1367 656e 6572 6174 655f 6465  .....generate_de
+00002080: 7363 7269 7074 6f72 bd00 0000 7386 0000  scriptor....s...
+00002090: 0000 0110 0104 0104 010c 0120 010c 010c  ........... ....
+000020a0: 011a fc02 0402 fb06 0502 fb02 0604 010c  ................
+000020b0: 011a 0120 010c 010c 0106 fb02 0502 fa06  ... ............
+000020c0: 0602 fa02 fa02 ff04 0f14 0114 0114 0214  ................
+000020d0: 0210 021a 0204 010a 0114 010a 011c 021a  ................
+000020e0: 0104 0108 0108 0124 ff08 0212 020e 0104  .......$........
+000020f0: 0110 0126 0126 0126 012a 0116 0108 0118  ...&.&.&.*......
+00002100: 0204 0104 0110 0110 0126 010a 0104 0118  .........&......
+00002110: 010c 010c 010c 0172 d300 0000 6300 0000  .......r....c...
+00002120: 0000 0000 0000 0000 0000 0000 0001 0000  ................
+00002130: 0043 0000 0073 0400 0000 7400 5300 7281  .C...s....t.S.r.
+00002140: 0000 0029 01da 0863 6974 6174 696f 6e72  ...)...citationr
+00002150: 2500 0000 7225 0000 0072 2500 0000 7228  %...r%...r%...r(
+00002160: 0000 00da 0463 6974 65fd 0000 0073 0200  .....cite....s..
+00002170: 0000 0001 72d5 0000 00fa 0b4a 5641 5350  ....r......JVASP
+00002180: 2d31 3030 3031 7212 0000 0063 0200 0000  -10001r....c....
+00002190: 0000 0000 0000 0000 0700 0000 0800 0000  ................
+000021a0: 4300 0000 73a0 0000 007c 0064 016b 0272  C...s....|.d.k.r
+000021b0: 1e74 0064 027c 019b 0064 039d 0383 0101  .t.d.|...d......
+000021c0: 0064 047d 026e 0c74 0064 0583 0101 0064  .d.}.n.t.d.....d
+000021d0: 0053 0074 01a0 0274 03a0 047c 02a1 01a1  .S.t...t...|....
+000021e0: 0167 017c 0114 007d 0374 057c 0383 0144  .g.|...}.t.|...D
+000021f0: 005d 0c7d 0474 067c 0483 017d 0571 4874  .].}.t.|...}.qHt
+00002200: 0764 0664 0783 028f 247d 067c 06a0 0864  .d.d....$}.|...d
+00002210: 0864 0984 007c 0544 0083 01a1 0101 0057  .d...|.D.......W
+00002220: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
+00002230: 8a30 0001 0001 0001 0059 0001 0074 0064  .0.......Y...t.d
+00002240: 0a83 0101 0064 0053 0029 0b4e da0d 6469  .....d.S.).N..di
+00002250: 6c75 7465 4e69 416c 6c6f 79fa 504b 5332  luteNiAlloy.PKS2
+00002260: 3032 3220 7072 6f66 696c 696e 672f 7465  022 profiling/te
+00002270: 7374 696e 6720 7461 736b 2077 696c 6c20  sting task will 
+00002280: 6361 6c63 756c 6174 6520 6120 6465 7363  calculate a desc
+00002290: 7269 7074 6f72 2066 6f72 2061 2064 696c  riptor for a dil
+000022a0: 7574 6520 4e69 2061 6c6c 6f79 207a 1120  ute Ni alloy z. 
+000022b0: 7469 6d65 7320 696e 2073 6572 6965 732e  times in series.
+000022c0: e1d4 1400 007b 2240 6d6f 6475 6c65 223a  .....{"@module":
+000022d0: 2022 7079 6d61 7467 656e 2e63 6f72 652e   "pymatgen.core.
+000022e0: 7374 7275 6374 7572 6522 2c20 2240 636c  structure", "@cl
+000022f0: 6173 7322 3a20 2253 7472 7563 7475 7265  ass": "Structure
+00002300: 222c 2022 6368 6172 6765 223a 206e 756c  ", "charge": nul
+00002310: 6c2c 2022 6c61 7474 6963 6522 3a20 7b22  l, "lattice": {"
+00002320: 6d61 7472 6978 223a 205b 5b36 2e39 3935  matrix": [[6.995
+00002330: 3639 322c 2030 2e30 2c20 302e 305d 2c20  692, 0.0, 0.0], 
+00002340: 5b30 2e30 2c20 362e 3939 3536 3932 2c20  [0.0, 6.995692, 
+00002350: 302e 305d 2c20 5b30 2e30 2c20 302e 302c  0.0], [0.0, 0.0,
+00002360: 2036 2e39 3935 3639 325d 5d2c 2022 6122   6.995692]], "a"
+00002370: 3a20 362e 3939 3536 3932 2c20 2262 223a  : 6.995692, "b":
+00002380: 2036 2e39 3935 3639 322c 2022 6322 3a20   6.995692, "c": 
+00002390: 362e 3939 3536 3932 2c20 2261 6c70 6861  6.995692, "alpha
+000023a0: 223a 2039 302e 302c 2022 6265 7461 223a  ": 90.0, "beta":
+000023b0: 2039 302e 302c 2022 6761 6d6d 6122 3a20   90.0, "gamma": 
+000023c0: 3930 2e30 2c20 2276 6f6c 756d 6522 3a20  90.0, "volume": 
+000023d0: 3334 322e 3336 3731 3133 3635 3631 3932  342.367113656192
+000023e0: 3433 7d2c 2022 7369 7465 7322 3a20 5b7b  43}, "sites": [{
+000023f0: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00002400: 656d 656e 7422 3a20 2243 7222 2c20 226f  ement": "Cr", "o
+00002410: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00002420: 3a20 5b30 2e30 2c20 302e 302c 2030 2e30  : [0.0, 0.0, 0.0
+00002430: 5d2c 2022 7879 7a22 3a20 5b30 2e30 2c20  ], "xyz": [0.0, 
+00002440: 302e 302c 2030 2e30 5d2c 2022 6c61 6265  0.0, 0.0], "labe
+00002450: 6c22 3a20 2243 7222 2c20 2270 726f 7065  l": "Cr", "prope
+00002460: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00002470: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00002480: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00002490: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+000024a0: 5b30 2e30 2c20 302e 302c 2030 2e35 5d2c  [0.0, 0.0, 0.5],
+000024b0: 2022 7879 7a22 3a20 5b30 2e30 2c20 302e   "xyz": [0.0, 0.
+000024c0: 302c 2033 2e34 3937 3834 365d 2c20 226c  0, 3.497846], "l
+000024d0: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+000024e0: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+000024f0: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00002500: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00002510: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00002520: 223a 205b 302e 302c 2030 2e35 2c20 302e  ": [0.0, 0.5, 0.
+00002530: 305d 2c20 2278 797a 223a 205b 302e 302c  0], "xyz": [0.0,
+00002540: 2033 2e34 3937 3834 362c 2030 2e30 5d2c   3.497846, 0.0],
+00002550: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+00002560: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00002570: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00002580: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
+00002590: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
+000025a0: 6162 6322 3a20 5b30 2e30 2c20 302e 352c  abc": [0.0, 0.5,
+000025b0: 2030 2e35 5d2c 2022 7879 7a22 3a20 5b30   0.5], "xyz": [0
+000025c0: 2e30 2c20 332e 3439 3738 3436 2c20 332e  .0, 3.497846, 3.
+000025d0: 3439 3738 3436 5d2c 2022 6c61 6265 6c22  497846], "label"
+000025e0: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+000025f0: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00002600: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00002610: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00002620: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00002630: 2e35 2c20 302e 302c 2030 2e30 5d2c 2022  .5, 0.0, 0.0], "
+00002640: 7879 7a22 3a20 5b33 2e34 3937 3834 362c  xyz": [3.497846,
+00002650: 2030 2e30 2c20 302e 305d 2c20 226c 6162   0.0, 0.0], "lab
+00002660: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+00002670: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00002680: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+00002690: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+000026a0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+000026b0: 205b 302e 352c 2030 2e30 2c20 302e 355d   [0.5, 0.0, 0.5]
+000026c0: 2c20 2278 797a 223a 205b 332e 3439 3738  , "xyz": [3.4978
+000026d0: 3436 2c20 302e 302c 2033 2e34 3937 3834  46, 0.0, 3.49784
+000026e0: 365d 2c20 226c 6162 656c 223a 2022 4e69  6], "label": "Ni
+000026f0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+00002700: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+00002710: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+00002720: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00002730: 2c20 2261 6263 223a 205b 302e 352c 2030  , "abc": [0.5, 0
+00002740: 2e35 2c20 302e 305d 2c20 2278 797a 223a  .5, 0.0], "xyz":
+00002750: 205b 332e 3439 3738 3436 2c20 332e 3439   [3.497846, 3.49
+00002760: 3738 3436 2c20 302e 305d 2c20 226c 6162  7846, 0.0], "lab
+00002770: 656c 223a 2022 4e69 222c 2022 7072 6f70  el": "Ni", "prop
+00002780: 6572 7469 6573 223a 207b 7d7d 2c20 7b22  erties": {}}, {"
+00002790: 7370 6563 6965 7322 3a20 5b7b 2265 6c65  species": [{"ele
+000027a0: 6d65 6e74 223a 2022 4e69 222c 2022 6f63  ment": "Ni", "oc
+000027b0: 6375 223a 2031 7d5d 2c20 2261 6263 223a  cu": 1}], "abc":
+000027c0: 205b 302e 352c 2030 2e35 2c20 302e 355d   [0.5, 0.5, 0.5]
+000027d0: 2c20 2278 797a 223a 205b 332e 3439 3738  , "xyz": [3.4978
+000027e0: 3436 2c20 332e 3439 3738 3436 2c20 332e  46, 3.497846, 3.
+000027f0: 3439 3738 3436 5d2c 2022 6c61 6265 6c22  497846], "label"
+00002800: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00002810: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00002820: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00002830: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00002840: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00002850: 2e32 352c 2030 2e32 352c 2030 2e30 5d2c  .25, 0.25, 0.0],
+00002860: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
+00002870: 332c 2031 2e37 3438 3932 332c 2030 2e30  3, 1.748923, 0.0
+00002880: 5d2c 2022 6c61 6265 6c22 3a20 224e 6922  ], "label": "Ni"
+00002890: 2c20 2270 726f 7065 7274 6965 7322 3a20  , "properties": 
+000028a0: 7b7d 7d2c 207b 2273 7065 6369 6573 223a  {}}, {"species":
+000028b0: 205b 7b22 656c 656d 656e 7422 3a20 224e   [{"element": "N
+000028c0: 6922 2c20 226f 6363 7522 3a20 317d 5d2c  i", "occu": 1}],
+000028d0: 2022 6162 6322 3a20 5b30 2e32 352c 2030   "abc": [0.25, 0
+000028e0: 2e32 352c 2030 2e35 5d2c 2022 7879 7a22  .25, 0.5], "xyz"
+000028f0: 3a20 5b31 2e37 3438 3932 332c 2031 2e37  : [1.748923, 1.7
+00002900: 3438 3932 332c 2033 2e34 3937 3834 365d  48923, 3.497846]
+00002910: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+00002920: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+00002930: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+00002940: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+00002950: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+00002960: 2261 6263 223a 205b 302e 3235 2c20 302e  "abc": [0.25, 0.
+00002970: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
+00002980: 2c20 302e 305d 2c20 2278 797a 223a 205b  , 0.0], "xyz": [
+00002990: 312e 3734 3839 3233 2c20 352e 3234 3637  1.748923, 5.2467
+000029a0: 3639 3030 3030 3030 3030 3035 2c20 302e  690000000005, 0.
+000029b0: 305d 2c20 226c 6162 656c 223a 2022 4e69  0], "label": "Ni
+000029c0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+000029d0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+000029e0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+000029f0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00002a00: 2c20 2261 6263 223a 205b 302e 3235 2c20  , "abc": [0.25, 
+00002a10: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
+00002a20: 3031 2c20 302e 355d 2c20 2278 797a 223a  01, 0.5], "xyz":
+00002a30: 205b 312e 3734 3839 3233 2c20 352e 3234   [1.748923, 5.24
+00002a40: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00002a50: 332e 3439 3738 3436 5d2c 2022 6c61 6265  3.497846], "labe
+00002a60: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+00002a70: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00002a80: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00002a90: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00002aa0: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00002ab0: 5b30 2e37 3530 3030 3030 3030 3030 3030  [0.7500000000000
+00002ac0: 3030 312c 2030 2e32 352c 2030 2e30 5d2c  001, 0.25, 0.0],
+00002ad0: 2022 7879 7a22 3a20 5b35 2e32 3436 3736   "xyz": [5.24676
+00002ae0: 3930 3030 3030 3030 3030 352c 2031 2e37  90000000005, 1.7
+00002af0: 3438 3932 332c 2030 2e30 5d2c 2022 6c61  48923, 0.0], "la
+00002b00: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00002b10: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00002b20: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00002b30: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+00002b40: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00002b50: 3a20 5b30 2e37 3530 3030 3030 3030 3030  : [0.75000000000
+00002b60: 3030 3030 312c 2030 2e32 352c 2030 2e35  00001, 0.25, 0.5
+00002b70: 5d2c 2022 7879 7a22 3a20 5b35 2e32 3436  ], "xyz": [5.246
+00002b80: 3736 3930 3030 3030 3030 3030 352c 2031  7690000000005, 1
+00002b90: 2e37 3438 3932 332c 2033 2e34 3937 3834  .748923, 3.49784
+00002ba0: 365d 2c20 226c 6162 656c 223a 2022 4e69  6], "label": "Ni
+00002bb0: 222c 2022 7072 6f70 6572 7469 6573 223a  ", "properties":
+00002bc0: 207b 7d7d 2c20 7b22 7370 6563 6965 7322   {}}, {"species"
+00002bd0: 3a20 5b7b 2265 6c65 6d65 6e74 223a 2022  : [{"element": "
+00002be0: 4e69 222c 2022 6f63 6375 223a 2031 7d5d  Ni", "occu": 1}]
+00002bf0: 2c20 2261 6263 223a 205b 302e 3735 3030  , "abc": [0.7500
+00002c00: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00002c10: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
+00002c20: 2c20 302e 305d 2c20 2278 797a 223a 205b  , 0.0], "xyz": [
+00002c30: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00002c40: 3035 2c20 352e 3234 3637 3639 3030 3030  05, 5.2467690000
+00002c50: 3030 3030 3035 2c20 302e 305d 2c20 226c  000005, 0.0], "l
+00002c60: 6162 656c 223a 2022 4e69 222c 2022 7072  abel": "Ni", "pr
+00002c70: 6f70 6572 7469 6573 223a 207b 7d7d 2c20  operties": {}}, 
+00002c80: 7b22 7370 6563 6965 7322 3a20 5b7b 2265  {"species": [{"e
+00002c90: 6c65 6d65 6e74 223a 2022 4e69 222c 2022  lement": "Ni", "
+00002ca0: 6f63 6375 223a 2031 7d5d 2c20 2261 6263  occu": 1}], "abc
+00002cb0: 223a 205b 302e 3735 3030 3030 3030 3030  ": [0.7500000000
+00002cc0: 3030 3030 3031 2c20 302e 3735 3030 3030  000001, 0.750000
+00002cd0: 3030 3030 3030 3030 3031 2c20 302e 355d  0000000001, 0.5]
+00002ce0: 2c20 2278 797a 223a 205b 352e 3234 3637  , "xyz": [5.2467
+00002cf0: 3639 3030 3030 3030 3030 3035 2c20 352e  690000000005, 5.
+00002d00: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
+00002d10: 2c20 332e 3439 3738 3436 5d2c 2022 6c61  , 3.497846], "la
+00002d20: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00002d30: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00002d40: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+00002d50: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+00002d60: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+00002d70: 3a20 5b30 2e32 352c 2030 2e30 2c20 302e  : [0.25, 0.0, 0.
+00002d80: 3235 5d2c 2022 7879 7a22 3a20 5b31 2e37  25], "xyz": [1.7
+00002d90: 3438 3932 332c 2030 2e30 2c20 312e 3734  48923, 0.0, 1.74
+00002da0: 3839 3233 5d2c 2022 6c61 6265 6c22 3a20  8923], "label": 
+00002db0: 224e 6922 2c20 2270 726f 7065 7274 6965  "Ni", "propertie
+00002dc0: 7322 3a20 7b7d 7d2c 207b 2273 7065 6369  s": {}}, {"speci
+00002dd0: 6573 223a 205b 7b22 656c 656d 656e 7422  es": [{"element"
+00002de0: 3a20 224e 6922 2c20 226f 6363 7522 3a20  : "Ni", "occu": 
+00002df0: 317d 5d2c 2022 6162 6322 3a20 5b30 2e32  1}], "abc": [0.2
+00002e00: 352c 2030 2e30 2c20 302e 3735 3030 3030  5, 0.0, 0.750000
+00002e10: 3030 3030 3030 3030 3031 5d2c 2022 7879  0000000001], "xy
+00002e20: 7a22 3a20 5b31 2e37 3438 3932 332c 2030  z": [1.748923, 0
+00002e30: 2e30 2c20 352e 3234 3637 3639 3030 3030  .0, 5.2467690000
+00002e40: 3030 3030 3035 5d2c 2022 6c61 6265 6c22  000005], "label"
+00002e50: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+00002e60: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+00002e70: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00002e80: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00002e90: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00002ea0: 2e32 352c 2030 2e35 2c20 302e 3235 5d2c  .25, 0.5, 0.25],
+00002eb0: 2022 7879 7a22 3a20 5b31 2e37 3438 3932   "xyz": [1.74892
+00002ec0: 332c 2033 2e34 3937 3834 362c 2031 2e37  3, 3.497846, 1.7
+00002ed0: 3438 3932 335d 2c20 226c 6162 656c 223a  48923], "label":
+00002ee0: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
+00002ef0: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
+00002f00: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
+00002f10: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
+00002f20: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
+00002f30: 3235 2c20 302e 352c 2030 2e37 3530 3030  25, 0.5, 0.75000
+00002f40: 3030 3030 3030 3030 3030 315d 2c20 2278  00000000001], "x
+00002f50: 797a 223a 205b 312e 3734 3839 3233 2c20  yz": [1.748923, 
+00002f60: 332e 3439 3738 3436 2c20 352e 3234 3637  3.497846, 5.2467
+00002f70: 3639 3030 3030 3030 3030 3035 5d2c 2022  690000000005], "
+00002f80: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00002f90: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00002fa0: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+00002fb0: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+00002fc0: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+00002fd0: 6322 3a20 5b30 2e37 3530 3030 3030 3030  c": [0.750000000
+00002fe0: 3030 3030 3030 312c 2030 2e30 2c20 302e  0000001, 0.0, 0.
+00002ff0: 3235 5d2c 2022 7879 7a22 3a20 5b35 2e32  25], "xyz": [5.2
+00003000: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
+00003010: 2030 2e30 2c20 312e 3734 3839 3233 5d2c   0.0, 1.748923],
+00003020: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+00003030: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00003040: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00003050: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
+00003060: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
+00003070: 6162 6322 3a20 5b30 2e37 3530 3030 3030  abc": [0.7500000
+00003080: 3030 3030 3030 3030 312c 2030 2e30 2c20  000000001, 0.0, 
+00003090: 302e 3735 3030 3030 3030 3030 3030 3030  0.75000000000000
+000030a0: 3031 5d2c 2022 7879 7a22 3a20 5b35 2e32  01], "xyz": [5.2
+000030b0: 3436 3736 3930 3030 3030 3030 3030 352c  467690000000005,
+000030c0: 2030 2e30 2c20 352e 3234 3637 3639 3030   0.0, 5.24676900
+000030d0: 3030 3030 3030 3035 5d2c 2022 6c61 6265  00000005], "labe
+000030e0: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+000030f0: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+00003100: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00003110: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00003120: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00003130: 5b30 2e37 3530 3030 3030 3030 3030 3030  [0.7500000000000
+00003140: 3030 312c 2030 2e35 2c20 302e 3235 5d2c  001, 0.5, 0.25],
+00003150: 2022 7879 7a22 3a20 5b35 2e32 3436 3736   "xyz": [5.24676
+00003160: 3930 3030 3030 3030 3030 352c 2033 2e34  90000000005, 3.4
+00003170: 3937 3834 362c 2031 2e37 3438 3932 335d  97846, 1.748923]
+00003180: 2c20 226c 6162 656c 223a 2022 4e69 222c  , "label": "Ni",
+00003190: 2022 7072 6f70 6572 7469 6573 223a 207b   "properties": {
+000031a0: 7d7d 2c20 7b22 7370 6563 6965 7322 3a20  }}, {"species": 
+000031b0: 5b7b 2265 6c65 6d65 6e74 223a 2022 4e69  [{"element": "Ni
+000031c0: 222c 2022 6f63 6375 223a 2031 7d5d 2c20  ", "occu": 1}], 
+000031d0: 2261 6263 223a 205b 302e 3735 3030 3030  "abc": [0.750000
+000031e0: 3030 3030 3030 3030 3031 2c20 302e 352c  0000000001, 0.5,
+000031f0: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00003200: 3030 315d 2c20 2278 797a 223a 205b 352e  001], "xyz": [5.
+00003210: 3234 3637 3639 3030 3030 3030 3030 3035  2467690000000005
+00003220: 2c20 332e 3439 3738 3436 2c20 352e 3234  , 3.497846, 5.24
+00003230: 3637 3639 3030 3030 3030 3030 3035 5d2c  67690000000005],
+00003240: 2022 6c61 6265 6c22 3a20 224e 6922 2c20   "label": "Ni", 
+00003250: 2270 726f 7065 7274 6965 7322 3a20 7b7d  "properties": {}
+00003260: 7d2c 207b 2273 7065 6369 6573 223a 205b  }, {"species": [
+00003270: 7b22 656c 656d 656e 7422 3a20 224e 6922  {"element": "Ni"
+00003280: 2c20 226f 6363 7522 3a20 317d 5d2c 2022  , "occu": 1}], "
+00003290: 6162 6322 3a20 5b30 2e30 2c20 302e 3235  abc": [0.0, 0.25
+000032a0: 2c20 302e 3235 5d2c 2022 7879 7a22 3a20  , 0.25], "xyz": 
+000032b0: 5b30 2e30 2c20 312e 3734 3839 3233 2c20  [0.0, 1.748923, 
+000032c0: 312e 3734 3839 3233 5d2c 2022 6c61 6265  1.748923], "labe
+000032d0: 6c22 3a20 224e 6922 2c20 2270 726f 7065  l": "Ni", "prope
+000032e0: 7274 6965 7322 3a20 7b7d 7d2c 207b 2273  rties": {}}, {"s
+000032f0: 7065 6369 6573 223a 205b 7b22 656c 656d  pecies": [{"elem
+00003300: 656e 7422 3a20 224e 6922 2c20 226f 6363  ent": "Ni", "occ
+00003310: 7522 3a20 317d 5d2c 2022 6162 6322 3a20  u": 1}], "abc": 
+00003320: 5b30 2e30 2c20 302e 3235 2c20 302e 3735  [0.0, 0.25, 0.75
+00003330: 3030 3030 3030 3030 3030 3030 3031 5d2c  00000000000001],
+00003340: 2022 7879 7a22 3a20 5b30 2e30 2c20 312e   "xyz": [0.0, 1.
+00003350: 3734 3839 3233 2c20 352e 3234 3637 3639  748923, 5.246769
+00003360: 3030 3030 3030 3030 3035 5d2c 2022 6c61  0000000005], "la
+00003370: 6265 6c22 3a20 224e 6922 2c20 2270 726f  bel": "Ni", "pro
+00003380: 7065 7274 6965 7322 3a20 7b7d 7d2c 207b  perties": {}}, {
+00003390: 2273 7065 6369 6573 223a 205b 7b22 656c  "species": [{"el
+000033a0: 656d 656e 7422 3a20 224e 6922 2c20 226f  ement": "Ni", "o
+000033b0: 6363 7522 3a20 317d 5d2c 2022 6162 6322  ccu": 1}], "abc"
+000033c0: 3a20 5b30 2e30 2c20 302e 3735 3030 3030  : [0.0, 0.750000
+000033d0: 3030 3030 3030 3030 3031 2c20 302e 3235  0000000001, 0.25
+000033e0: 5d2c 2022 7879 7a22 3a20 5b30 2e30 2c20  ], "xyz": [0.0, 
+000033f0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00003400: 3035 2c20 312e 3734 3839 3233 5d2c 2022  05, 1.748923], "
+00003410: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00003420: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00003430: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+00003440: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+00003450: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+00003460: 6322 3a20 5b30 2e30 2c20 302e 3735 3030  c": [0.0, 0.7500
+00003470: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00003480: 3735 3030 3030 3030 3030 3030 3030 3031  7500000000000001
+00003490: 5d2c 2022 7879 7a22 3a20 5b30 2e30 2c20  ], "xyz": [0.0, 
+000034a0: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+000034b0: 3035 2c20 352e 3234 3637 3639 3030 3030  05, 5.2467690000
+000034c0: 3030 3030 3035 5d2c 2022 6c61 6265 6c22  000005], "label"
+000034d0: 3a20 224e 6922 2c20 2270 726f 7065 7274  : "Ni", "propert
+000034e0: 6965 7322 3a20 7b7d 7d2c 207b 2273 7065  ies": {}}, {"spe
+000034f0: 6369 6573 223a 205b 7b22 656c 656d 656e  cies": [{"elemen
+00003500: 7422 3a20 224e 6922 2c20 226f 6363 7522  t": "Ni", "occu"
+00003510: 3a20 317d 5d2c 2022 6162 6322 3a20 5b30  : 1}], "abc": [0
+00003520: 2e35 2c20 302e 3235 2c20 302e 3235 5d2c  .5, 0.25, 0.25],
+00003530: 2022 7879 7a22 3a20 5b33 2e34 3937 3834   "xyz": [3.49784
+00003540: 362c 2031 2e37 3438 3932 332c 2031 2e37  6, 1.748923, 1.7
+00003550: 3438 3932 335d 2c20 226c 6162 656c 223a  48923], "label":
+00003560: 2022 4e69 222c 2022 7072 6f70 6572 7469   "Ni", "properti
+00003570: 6573 223a 207b 7d7d 2c20 7b22 7370 6563  es": {}}, {"spec
+00003580: 6965 7322 3a20 5b7b 2265 6c65 6d65 6e74  ies": [{"element
+00003590: 223a 2022 4e69 222c 2022 6f63 6375 223a  ": "Ni", "occu":
+000035a0: 2031 7d5d 2c20 2261 6263 223a 205b 302e   1}], "abc": [0.
+000035b0: 352c 2030 2e32 352c 2030 2e37 3530 3030  5, 0.25, 0.75000
+000035c0: 3030 3030 3030 3030 3030 315d 2c20 2278  00000000001], "x
+000035d0: 797a 223a 205b 332e 3439 3738 3436 2c20  yz": [3.497846, 
+000035e0: 312e 3734 3839 3233 2c20 352e 3234 3637  1.748923, 5.2467
+000035f0: 3639 3030 3030 3030 3030 3035 5d2c 2022  690000000005], "
+00003600: 6c61 6265 6c22 3a20 224e 6922 2c20 2270  label": "Ni", "p
+00003610: 726f 7065 7274 6965 7322 3a20 7b7d 7d2c  roperties": {}},
+00003620: 207b 2273 7065 6369 6573 223a 205b 7b22   {"species": [{"
+00003630: 656c 656d 656e 7422 3a20 224e 6922 2c20  element": "Ni", 
+00003640: 226f 6363 7522 3a20 317d 5d2c 2022 6162  "occu": 1}], "ab
+00003650: 6322 3a20 5b30 2e35 2c20 302e 3735 3030  c": [0.5, 0.7500
+00003660: 3030 3030 3030 3030 3030 3031 2c20 302e  000000000001, 0.
+00003670: 3235 5d2c 2022 7879 7a22 3a20 5b33 2e34  25], "xyz": [3.4
+00003680: 3937 3834 362c 2035 2e32 3436 3736 3930  97846, 5.2467690
+00003690: 3030 3030 3030 3030 352c 2031 2e37 3438  000000005, 1.748
+000036a0: 3932 335d 2c20 226c 6162 656c 223a 2022  923], "label": "
+000036b0: 4e69 222c 2022 7072 6f70 6572 7469 6573  Ni", "properties
+000036c0: 223a 207b 7d7d 2c20 7b22 7370 6563 6965  ": {}}, {"specie
+000036d0: 7322 3a20 5b7b 2265 6c65 6d65 6e74 223a  s": [{"element":
+000036e0: 2022 4e69 222c 2022 6f63 6375 223a 2031   "Ni", "occu": 1
+000036f0: 7d5d 2c20 2261 6263 223a 205b 302e 352c  }], "abc": [0.5,
+00003700: 2030 2e37 3530 3030 3030 3030 3030 3030   0.7500000000000
+00003710: 3030 312c 2030 2e37 3530 3030 3030 3030  001, 0.750000000
+00003720: 3030 3030 3030 315d 2c20 2278 797a 223a  0000001], "xyz":
+00003730: 205b 332e 3439 3738 3436 2c20 352e 3234   [3.497846, 5.24
+00003740: 3637 3639 3030 3030 3030 3030 3035 2c20  67690000000005, 
+00003750: 352e 3234 3637 3639 3030 3030 3030 3030  5.24676900000000
+00003760: 3035 5d2c 2022 6c61 6265 6c22 3a20 224e  05], "label": "N
+00003770: 6922 2c20 2270 726f 7065 7274 6965 7322  i", "properties"
+00003780: 3a20 7b7d 7d5d 2c20 2240 7665 7273 696f  : {}}], "@versio
+00003790: 6e22 3a20 6e75 6c6c 7dfa 1755 6e72 6563  n": null}..Unrec
+000037a0: 6f67 6e69 7a65 6420 7465 7374 206e 616d  ognized test nam
+000037b0: 652e 7a1c 4b53 3230 3232 5f64 696c 7574  e.z.KS2022_dilut
+000037c0: 655f 5465 7374 5265 7375 6c74 2e63 7376  e_TestResult.csv
+000037d0: 7a02 772b 6301 0000 0000 0000 0000 0000  z.w+c...........
+000037e0: 0002 0000 0004 0000 0053 0000 0073 1600  .........S...s..
+000037f0: 0000 6700 7c00 5d0e 7d01 7c01 9b00 6400  ..g.|.].}.|...d.
+00003800: 9d02 9102 7104 5300 2901 da01 0a72 2500  ....q.S.)....r%.
+00003810: 0000 2902 7226 0000 00da 0176 7225 0000  ..).r&.....vr%..
+00003820: 0072 2500 0000 7228 0000 0072 5000 0000  .r%...r(...rP...
+00003830: 0b01 0000 722a 0000 007a 1b70 726f 6669  ....r*...z.profi
+00003840: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
+00003850: 7463 6f6d 703e fa05 446f 6e65 2129 0972  tcomp>..Done!).r
+00003860: 5400 0000 7202 0000 00da 0966 726f 6d5f  T...r......from_
+00003870: 6469 6374 da04 6a73 6f6e da05 6c6f 6164  dict..json..load
+00003880: 7372 0600 0000 72d3 0000 00da 046f 7065  sr....r......ope
+00003890: 6eda 0a77 7269 7465 6c69 6e65 7329 07da  n..writelines)..
+000038a0: 0474 6573 74da 056e 5275 6e73 da06 6d61  .test..nRuns..ma
+000038b0: 7453 7472 da05 734c 6973 7472 b500 0000  tStr..sListr....
+000038c0: 72b6 0000 0072 b700 0000 7225 0000 0072  r....r....r%...r
+000038d0: 2500 0000 7228 0000 00da 0770 726f 6669  %...r(.....profi
+000038e0: 6c65 0001 0000 7316 0000 0000 0108 0110  le....s.........
+000038f0: 0106 0208 0104 0116 010c 010a 010c 0132  ...............2
+00003900: 0172 e700 0000 e9e8 0300 0063 0200 0000  .r.........c....
+00003910: 0000 0000 0000 0000 0700 0000 0500 0000  ................
+00003920: 4300 0000 736a 0000 0064 0164 026c 006d  C...sj...d.d.l.m
+00003930: 017d 0201 007c 0064 036b 0272 2a74 0264  .}...|.d.k.r*t.d
+00003940: 047c 019b 0064 059d 0383 0101 0064 067d  .|...d.......d.}
+00003950: 036e 0c74 0264 0783 0101 0064 0053 0074  .n.t.d.....d.S.t
+00003960: 03a0 0474 05a0 067c 03a1 01a1 017d 047c  ...t...|.....}.|
+00003970: 0467 017c 0114 007d 057c 0274 077c 0564  .g.|...}.|.t.|.d
+00003980: 0864 098d 037d 0674 0264 0a83 0101 0064  .d...}.t.d.....d
+00003990: 0053 0029 0b4e 7201 0000 0029 01da 0b70  .S.).Nr....)...p
+000039a0: 726f 6365 7373 5f6d 6170 72d7 0000 0072  rocess_mapr....r
+000039b0: d800 0000 7a22 2074 696d 6573 2069 6e20  ....z" times in 
+000039c0: 7061 7261 6c6c 656c 2077 6974 6820 3820  parallel with 8 
+000039d0: 776f 726b 6572 732e 72d9 0000 0072 da00  workers.r....r..
+000039e0: 0000 72a5 0000 0029 01da 0b6d 6178 5f77  ..r....)...max_w
+000039f0: 6f72 6b65 7273 72dd 0000 0029 08da 1774  orkersr....)...t
+00003a00: 7164 6d2e 636f 6e74 7269 622e 636f 6e63  qdm.contrib.conc
+00003a10: 7572 7265 6e74 72e9 0000 0072 5400 0000  urrentr....rT...
+00003a20: 7202 0000 0072 de00 0000 72df 0000 0072  r....r....r....r
+00003a30: e000 0000 72d3 0000 0029 0772 e300 0000  ....r....).r....
+00003a40: 72e4 0000 0072 e900 0000 72e5 0000 0072  r....r....r....r
+00003a50: b500 0000 72e6 0000 00da 0864 6573 634c  ....r......descL
+00003a60: 6973 7472 2500 0000 7225 0000 0072 2800  istr%...r%...r(.
+00003a70: 0000 da0f 7072 6f66 696c 6550 6172 616c  ....profileParal
+00003a80: 6c65 6c0e 0100 0073 1400 0000 0001 0c01  lel....s........
+00003a90: 0801 1001 0602 0801 0401 1002 0a01 0e01  ................
+00003aa0: 72ed 0000 00da 085f 5f6d 6169 6e5f 5f72  r......__main__r
+00003ab0: d700 0000 2901 72e3 0000 0029 0172 0100  ....).r....).r..
+00003ac0: 0000 2901 7257 0000 0029 0272 d600 0000  ..).rW...).r....
+00003ad0: 7212 0000 0029 0272 d600 0000 72e8 0000  r....).r....r...
+00003ae0: 0029 2372 3600 0000 da04 7469 6d65 da05  .)#r6.....time..
+00003af0: 6e75 6d70 7972 2b00 0000 da02 6f73 da0d  numpyr+.....os..
+00003b00: 7079 6d61 7467 656e 2e63 6f72 6572 0200  pymatgen.corer..
+00003b10: 0000 7203 0000 00da 1b70 796d 6174 6765  ..r......pymatge
+00003b20: 6e2e 616e 616c 7973 6973 2e6c 6f63 616c  n.analysis.local
+00003b30: 5f65 6e76 7204 0000 00da 1a70 796d 6174  _envr......pymat
+00003b40: 6765 6e2e 7379 6d6d 6574 7279 2e61 6e61  gen.symmetry.ana
+00003b50: 6c79 7a65 7272 0500 0000 72df 0000 0072  lyzerr....r....r
+00003b60: 0600 0000 da0b 636f 6c6c 6563 7469 6f6e  ......collection
+00003b70: 7372 0700 0000 72d4 0000 00da 1370 6572  sr....r......per
+00003b80: 696f 6469 635f 7461 626c 655f 7369 7a65  iodic_table_size
+00003b90: da07 6c6f 6164 7478 74da 0470 6174 6872  ..loadtxt..pathr
+00003ba0: 7000 0000 da07 6469 726e 616d 65da 085f  p.....dirname.._
+00003bb0: 5f66 696c 655f 5f72 2d00 0000 da0a 6e61  _file__r-.....na
+00003bc0: 6e5f 746f 5f6e 756d 724b 0000 0072 5600  n_to_numrK...rV.
+00003bd0: 0000 727e 0000 0072 6200 0000 72a2 0000  ..r~...rb...r...
+00003be0: 0072 d300 0000 72d5 0000 0072 e700 0000  .r....r....r....
+00003bf0: 72ed 0000 0072 8e00 0000 7225 0000 0072  r....r....r%...r
+00003c00: 2500 0000 7225 0000 0072 2800 0000 da08  %...r%...r(.....
+00003c10: 3c6d 6f64 756c 653e 0a00 0000 7338 0000  <module>....s8..
+00003c20: 0008 0108 0108 0108 0110 010c 010c 0108  ................
+00003c30: 010c 010c 0204 0204 0120 010a 0208 0106  ......... ......
+00003c40: ff06 0508 2808 0a0e 3f0e 1a0a 1210 4008  ....(...?.....@.
+00003c50: 030a 0e0a 0e0a 010a 01                   .........
```

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_KS2022.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_KS2022_dilute.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/descriptorDefinitions/labels_Ward2017.csv` & `pysipfenn-0.12.1/pysipfenn/descriptorDefinitions/labels_Ward2017.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/modelsSIPFENN/models.json` & `pysipfenn-0.12.1/pysipfenn/modelsSIPFENN/models.json`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_enumerated.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/TestFile_DescriptorData_4_KS2022_labeled_named.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/0-Cr8Fe18Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/1-Cr16Fe8Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/10-Ce4Ti4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/11-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/12-Gd4Cr4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/13-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/14-Fe24Ni6.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/15-Ta4Tl4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/16-Fe18Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/17-Pr4Ga4O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/18-Fe28Ni2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/19-Fe4Ni26.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/2-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/20-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/21-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/22-Fe10Ni20.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/23-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/24-Fe16Ni14.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/25-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/26-Fe8Ni22.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/27-Cr28Fe2.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/28-Fe26Ni4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/29-Fe12Ni18.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/3-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/30-Cr26Fe4.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/31-Li24Al4Ni32.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/4-Fe30.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/5-Cr22Fe8.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/6-Fe2Ni28.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/7-Cr18Fe12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/8-Cr2Fe16Ni12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles/9-Pb8O12.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFilesDescriptorTable.csv`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/1-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/2-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR` & `pysipfenn-0.12.1/pysipfenn/tests/testCaseFiles/exampleInputFiles_500atom/3-Zr220Cu280.POSCAR`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_AllCompatibleONNX_Ward2017.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_KS2022_dilute.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_KS2022_dilute.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,12 +74,18 @@
                     p_fo_relative = p_fo/p_trd
                     with self.subTest(msg=f'{name:<16} diff in {l}'):
                         self.assertAlmostEqual(p_fo_relative, 1, places=2)
                 else:
                     with self.subTest(msg=f'{name:<16} diff in {l}'):
                         self.assertAlmostEqual(p_fo, p_trd, places=6)
 
-
+class TestKS2022_diluteProfiling(unittest.TestCase):
+    '''Test the dilute version of KS2022 descriptor generation by profiling the execution time of the descriptor generation function
+        for one example structures in serial and parallel (8 workers) mode.'''
+    def test_serial(self):
+        KS2022_dilute.profile(test='diluteNiAlloy', nRuns=10)
+    def test_parallel(self):
+        KS2022_dilute.profileParallel(test='diluteNiAlloy', nRuns=64)
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_Krajewski2020_NN9NN20NN24_ONNX.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_Ward2017.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_Ward2017.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,9 +32,22 @@
     def test_resutls(self):
         for fo, trd, name in zip(self.functionOutput, self.testReferenceData, self.exampleInputFiles):
             for p_fo, p_trd, l in zip(fo, trd, self.labels):
                 if l not in self.skipLabels:
                     with self.subTest(msg=f'Testing {l} calculated for {name}'):
                         self.assertAlmostEqual(p_fo, p_trd, places=6)
 
+
+class TestWard2017Profiling(unittest.TestCase):
+    '''Test the Ward2017 descriptor generation by profiling the execution time of the descriptor generation function
+    for two example structures in serial and parallel (8 workers) mode.'''
+    def test_serial(self):
+        Ward2017.profile(test='JVASP-10001', nRuns=4)
+        Ward2017.profile(test='diluteNiAlloy', nRuns=4)
+
+    def test_parallel(self):
+        Ward2017.profileParallel(test='JVASP-10001', nRuns=24)
+        Ward2017.profileParallel(test='diluteNiAlloy', nRuns=24)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_customModel.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_customModel.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn/tests/test_pysipfenn.py` & `pysipfenn-0.12.1/pysipfenn/tests/test_pysipfenn.py`

 * *Files identical despite different names*

### Comparing `pysipfenn-0.12.0/pysipfenn.egg-info/PKG-INFO` & `pysipfenn-0.12.1/pysipfenn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysipfenn
-Version: 0.12.0
+Version: 0.12.1
 Summary: Easily extensible Python package for featurizing periodic atomic structures and running Structure-Informed Prediction of Formation Energy using Neural Networks (SIPFENN)
 Author-email: Adam Krajewski <ak@psu.edu>, Jonathan Siegel <jwsiegel@tamu.edu>
 Project-URL: Research Page, https://phaseslab.com/sipfenn
 Project-URL: Homepage, https://pysipfenn.org
 Project-URL: Bug Tracker, https://github.com/PhasesResearchLab/pySIPFENN/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pysipfenn-0.12.0/pysipfenn.egg-info/SOURCES.txt` & `pysipfenn-0.12.1/pysipfenn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

