# Comparing `tmp/monstermash-1.0.0.tar.gz` & `tmp/monstermash-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-1.0.0.tar", max compression
+gzip compressed data, was "monstermash-1.0.1.tar", max compression
```

## Comparing `monstermash-1.0.0.tar` & `monstermash-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1366 2023-06-25 03:26:09.252761 monstermash-1.0.0/README.md
--rw-r--r--   0        0        0     1055 2023-06-25 03:26:09.252761 monstermash-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/__init__.py
--rw-r--r--   0        0        0     1627 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1772 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/crypt.py
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1366 2023-06-25 04:08:12.643755 monstermash-1.0.1/README.md
+-rw-r--r--   0        0        0     1055 2023-06-25 04:08:12.643755 monstermash-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     1646 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1772 2023-06-25 04:08:12.643755 monstermash-1.0.1/src/monstermash/crypt.py
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-1.0.1/PKG-INFO
```

### Comparing `monstermash-1.0.0/README.md` & `monstermash-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.0.0
+> 1️⃣ version: 1.0.1
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-1.0.0/pyproject.toml` & `monstermash-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monstermash"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
```

### Comparing `monstermash-1.0.0/src/monstermash/__main__.py` & `monstermash-1.0.1/src/monstermash/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,27 +34,28 @@
     click.echo('-----------------')
 
 
 @main.command()
 def encrypt():
     private_key = questionary.password('Enter your private key:').ask()
     public_key = questionary.text('Enter the public key:').ask()
+
     crypt = Crypt(private_key.encode())
 
     input_type = questionary.select(
         'What type of data do you want to encrypt?', choices=['file', 'text']
     ).ask()
 
     if input_type == 'file':
         file = questionary.text('Enter the file path:').ask()
         data = open_file(file)
     else:
         data = questionary.password('Enter (or paste) the text to encrypt:').ask()
 
-    encrypted = crypt.encrypt(data, public_key)
+    encrypted = crypt.encrypt(data.encode(), public_key.encode())
     click.echo(encrypted)
 
 
 @main.command()
 def decrypt():
     private_key = questionary.password('Enter your private key:').ask()
     crypt = Crypt(private_key.encode())
```

### Comparing `monstermash-1.0.0/src/monstermash/crypt.py` & `monstermash-1.0.1/src/monstermash/crypt.py`

 * *Files identical despite different names*

### Comparing `monstermash-1.0.0/PKG-INFO` & `monstermash-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Mitchell Lisle
 Author-email: m.lisle90@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ##  🧟 Monstermash
 
-> 1️⃣ version: 1.0.0
+> 1️⃣ version: 1.0.1
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

