# Comparing `tmp/fastapi_mail-1.2.9.tar.gz` & `tmp/fastapi_mail-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mail-1.2.9.tar", max compression
+gzip compressed data, was "fastapi_mail-1.3.0.tar", max compression
```

## Comparing `fastapi_mail-1.2.9.tar` & `fastapi_mail-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1072 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/LICENSE
--rwxr-xr-x   0        0        0     3407 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/README.md
--rwxr-xr-x   0        0        0      385 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/config.py
--rw-r--r--   0        0        0     1848 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/connection.py
--rw-r--r--   0        0        0      122 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/email_utils/__init__.py
--rw-r--r--   0        0        0    16451 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/email_utils/email_check.py
--rwxr-xr-x   0        0        0      530 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/errors.py
--rwxr-xr-x   0        0        0     4004 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/fastmail.py
--rw-r--r--   0        0        0     5731 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/msg.py
--rw-r--r--   0        0        0     3590 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/schemas.py
--rw-r--r--   0        0        0     1871 2023-06-25 12:16:39.586939 fastapi_mail-1.2.9/pyproject.toml
--rw-r--r--   0        0        0     4670 1970-01-01 00:00:00.000000 fastapi_mail-1.2.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/LICENSE
+-rwxr-xr-x   0        0        0     3407 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/README.md
+-rwxr-xr-x   0        0        0      385 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/config.py
+-rw-r--r--   0        0        0     1848 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/connection.py
+-rw-r--r--   0        0        0      122 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/email_utils/__init__.py
+-rw-r--r--   0        0        0    16451 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/email_utils/email_check.py
+-rwxr-xr-x   0        0        0      530 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/errors.py
+-rwxr-xr-x   0        0        0     4004 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/fastmail.py
+-rw-r--r--   0        0        0     5731 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/msg.py
+-rw-r--r--   0        0        0     3354 2023-06-25 17:47:33.061693 fastapi_mail-1.3.0/fastapi_mail/schemas.py
+-rw-r--r--   0        0        0     1871 2023-06-25 17:47:47.857779 fastapi_mail-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4670 1970-01-01 00:00:00.000000 fastapi_mail-1.3.0/PKG-INFO
```

### Comparing `fastapi_mail-1.2.9/LICENSE` & `fastapi_mail-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/README.md` & `fastapi_mail-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/config.py` & `fastapi_mail-1.3.0/fastapi_mail/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/connection.py` & `fastapi_mail-1.3.0/fastapi_mail/connection.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/email_utils/email_check.py` & `fastapi_mail-1.3.0/fastapi_mail/email_utils/email_check.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/errors.py` & `fastapi_mail-1.3.0/fastapi_mail/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/fastmail.py` & `fastapi_mail-1.3.0/fastapi_mail/fastmail.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/msg.py` & `fastapi_mail-1.3.0/fastapi_mail/msg.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.9/fastapi_mail/schemas.py` & `fastapi_mail-1.3.0/fastapi_mail/schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,23 +84,14 @@
                 temp.append((file, file_meta))
             else:
                 raise WrongFile(
                     "attachments field type incorrect, must be UploadFile or path"
                 )
         return temp
 
-    @validator("subtype")
-    def validate_subtype(cls, value, values, config, field):
-        """
-        Validate subtype field
-        """
-        if values["template_body"]:
-            return MessageType.html
-        return value
-
     @root_validator
     def validate_alternative_body(cls, values):
         """
         Validate alternative_body field
         """
         if (
             values["multipart_subtype"] != MultipartSubtypeEnum.alternative
```

### Comparing `fastapi_mail-1.2.9/pyproject.toml` & `fastapi_mail-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mail"
-version = "1.2.9"
+version = "1.3.0"
 description = "Simple lightweight mail library for FastApi"
 authors = ["Sabuhi Shukurov <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mail"
 repository = "https://github.com/sabuhish/fastapi-mail"
 classifiers = [
```

### Comparing `fastapi_mail-1.2.9/PKG-INFO` & `fastapi_mail-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-mail
-Version: 1.2.9
+Version: 1.3.0
 Summary: Simple lightweight mail library for FastApi
 Home-page: https://github.com/sabuhish/fastapi-mail
 License: MIT
 Author: Sabuhi Shukurov
 Author-email: sabuhi.shukurov@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Intended Audience :: Developers
```

