# Comparing `tmp/ovmfkeyenroll-1.1.0.tar.gz` & `tmp/ovmfkeyenroll-1.2.0.tar.gz`

## Comparing `ovmfkeyenroll-1.1.0.tar` & `ovmfkeyenroll-1.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/LICENSE
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/Makefile
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/README.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/pyproject.toml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/ovmfkeyenroll/SecureBootEnable.bin
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/ovmfkeyenroll/__init__.py
--rw-r--r--   0        0        0    10413 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/ovmfkeyenroll/secure_boot.py
--rw-r--r--   0        0        0    32648 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/ovmfkeyenroll/var_enroll.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/ovmfkeyenroll/SecureBootEnable.bin
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/ovmfkeyenroll/__init__.py
+-rw-r--r--   0        0        0    10411 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/ovmfkeyenroll/secure_boot.py
+-rw-r--r--   0        0        0    32700 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/ovmfkeyenroll/var_enroll.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/README.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 ovmfkeyenroll-1.2.0/PKG-INFO
```

### Comparing `ovmfkeyenroll-1.1.0/LICENSE` & `ovmfkeyenroll-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ovmfkeyenroll-1.1.0/README.md` & `ovmfkeyenroll-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ovmfkeyenroll-1.1.0/pyproject.toml` & `ovmfkeyenroll-1.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ovmfkeyenroll"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Xu, Min", email="min.m.xu@intel.com" },
   { name="Feng, Jialei", email="jialei.feng@intel.com" },
 ]
 readme = "README.md"
 description = "OVMF PK, KEK and DB Keys Enrolling"
 requires-python = ">=3.6.8"
```

### Comparing `ovmfkeyenroll-1.1.0/ovmfkeyenroll/secure_boot.py` & `ovmfkeyenroll-1.2.0/ovmfkeyenroll/secure_boot.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 
     return result
 
 def print_usage():
     '''
     helper function
     '''
-    usage = '''tdvf-key-enroll -fd <absolute-path-to-OVMF_VARS.fd>
+    usage = '''ovmfkeyenroll -fd <absolute-path-to-OVMF_VARS.fd>
     -pk <pk-key-guid> <absolute-path-to-PK.cer>
     -kek <kek-guid> <absolute-path-to-KEK.cer>
     -db <db-key-guid> <absolute-path-to-DB.cer>
     [-o outputdir]'''
     print(usage)
     sys.exit()
```

### Comparing `ovmfkeyenroll-1.1.0/ovmfkeyenroll/var_enroll.py` & `ovmfkeyenroll-1.2.0/ovmfkeyenroll/var_enroll.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import os
 from enum import Enum
 
 EFI_GLOBAL_VARIABLE = '8BE4DF61-93CA-11d2-AA0D-00E098032B8C'
 EFI_IMAGE_SECURITY_DATABASE_GUID = "d719b2cb-3d3a-4596-a3bc-dad00e67656f"
 EFI_CERT_X509_GUID = "a5c059a1-94e4-4aa7-87b5-ab155c2bf072"
 
-# pylint: disable=broad-except
+# pylint: disable=broad-exception-raised
+# pylint: disable=broad-exception-caught
 # pylint: disable=consider-using-f-string
 
 def is_guid(string):
     '''if a string matches guid'''
     if not isinstance(string, str):
         return False
     pattern = re.compile('[0-9a-f]{8}-[0-9a-f]{4}-[1-5][0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}')
```

### Comparing `ovmfkeyenroll-1.1.0/PKG-INFO` & `ovmfkeyenroll-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: ovmfkeyenroll
-Version: 1.1.0
+Version: 1.2.0
 Summary: OVMF PK, KEK and DB Keys Enrolling
-Project-URL: Bug Tracker, https://github.com/intel/tdx-tools/issues
 Project-URL: Homepage, https://github.com/intel/tdx-tools/tree/main/utils/ovmfkeyenroll
+Project-URL: Bug Tracker, https://github.com/intel/tdx-tools/issues
 Author-email: "Xu, Min" <min.m.xu@intel.com>, "Feng, Jialei" <jialei.feng@intel.com>
+License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Boot
 Requires-Python: >=3.6.8
```

