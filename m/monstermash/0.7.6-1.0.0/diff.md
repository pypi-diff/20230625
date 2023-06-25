# Comparing `tmp/monstermash-0.7.6.tar.gz` & `tmp/monstermash-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monstermash-0.7.6.tar", max compression
+gzip compressed data, was "monstermash-1.0.0.tar", max compression
```

## Comparing `monstermash-0.7.6.tar` & `monstermash-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1366 2023-06-18 05:34:43.840450 monstermash-0.7.6/README.md
--rw-r--r--   0        0        0     1046 2023-06-18 05:34:43.840450 monstermash-0.7.6/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/__init__.py
--rw-r--r--   0        0        0     1968 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/__main__.py
--rw-r--r--   0        0        0     1530 2023-06-18 05:34:43.840450 monstermash-0.7.6/src/monstermash/crypt.py
--rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1366 2023-06-25 03:26:09.252761 monstermash-1.0.0/README.md
+-rw-r--r--   0        0        0     1055 2023-06-25 03:26:09.252761 monstermash-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/__init__.py
+-rw-r--r--   0        0        0     1627 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/__main__.py
+-rw-r--r--   0        0        0     1772 2023-06-25 03:26:09.256761 monstermash-1.0.0/src/monstermash/crypt.py
+-rw-r--r--   0        0        0     1926 1970-01-01 00:00:00.000000 monstermash-1.0.0/PKG-INFO
```

### Comparing `monstermash-0.7.6/README.md` & `monstermash-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ##  🧟 Monstermash
 
-> 1️⃣ version: 0.7.6
+> 1️⃣ version: 1.0.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

### Comparing `monstermash-0.7.6/pyproject.toml` & `monstermash-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monstermash"
-version = "0.7.6"
+version = "1.0.0"
 description = ""
 authors = ["Mitchell Lisle <m.lisle90@gmail.com>"]
 readme = "README.md"
 packages = [{include = "monstermash", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
@@ -17,25 +17,25 @@
 [tool.poetry.group.dev.dependencies]
 bumpversion = "^0.6.0"
 twine = "^4.0.2"
 flake8 = "^6.0.0"
 dlint = "^0.14.0"
 mypy = "^1.1.1"
 pre-commit = "^3.2.1"
-setuptools = "^67.6.0"
+setuptools = ">=67.6,<69.0"
 flake8-bugbear = "^23.3.23"
 pep8-naming = "^0.13.3"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.1.4"
-mkdocs-gen-files = "^0.4.0"
+mkdocs-gen-files = ">=0.4,<0.6"
 mkdocs-literate-nav = "^0.6.0"
-mkdocstrings = {extras = ["python"], version = ">=0.20,<0.22"}
+mkdocstrings = {extras = ["python"], version = ">=0.20,<0.23"}
 mkautodoc = "^0.2.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.2.2"
 pytest-dotenv = "^0.5.2"
 pytest-cov = "^4.0.0"
```

### Comparing `monstermash-0.7.6/src/monstermash/__main__.py` & `monstermash-1.0.0/src/monstermash/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 import json
 import re
-from functools import partial
 
 import click
 import questionary
 
 from monstermash.crypt import Crypt
 
-red = partial(click.style, fg='yellow')
-blue = partial(click.style, fg='blue')
-green = partial(click.style, fg='green')
-danger = partial(click.style, fg='red')
-
 
 def open_file(file):
     if re.search('.json$', file):
         with open(file, 'r') as f:
             data = json.load(f)
     else:
         with open(file, 'r') as f:
@@ -29,18 +23,18 @@
 
 
 @main.command()
 def generate():
     keys = Crypt.generate()
 
     click.echo('-----------------')
-    click.echo(red('Private Key (keep is secret, keep it safe)'))
-    click.echo(red(keys.private_key.get_secret_value()))
-    click.echo(blue('Public Key (you can share this one)'))
-    click.echo(blue(keys.public_key.get_secret_value()))
+    click.echo('Private Key (keep is secret, keep it safe)')
+    click.echo(keys.private_key.get_secret_value())
+    click.echo('Public Key (you can share this one)')
+    click.echo(keys.public_key)
     click.echo('-----------------')
 
 
 @main.command()
 def encrypt():
     private_key = questionary.password('Enter your private key:').ask()
     public_key = questionary.text('Enter the public key:').ask()
@@ -52,25 +46,24 @@
 
     if input_type == 'file':
         file = questionary.text('Enter the file path:').ask()
         data = open_file(file)
     else:
         data = questionary.password('Enter (or paste) the text to encrypt:').ask()
 
-    encrypted = crypt.encrypt(data.encode(), public_key)
-    click.echo(green(encrypted))
+    encrypted = crypt.encrypt(data, public_key)
+    click.echo(encrypted)
 
 
 @main.command()
 def decrypt():
     private_key = questionary.password('Enter your private key:').ask()
-    public_key = questionary.text('Enter the public key:').ask()
     crypt = Crypt(private_key.encode())
 
     data = questionary.text('Enter the encrypted text:').ask()
 
-    decrypted = crypt.decrypt(data.encode(), public_key)
-    click.echo(green(decrypted.decode()))
+    decrypted = crypt.decrypt(data.encode())
+    click.echo(decrypted)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `monstermash-0.7.6/src/monstermash/crypt.py` & `monstermash-1.0.0/src/monstermash/crypt.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,49 @@
-from nacl.encoding import Base64Encoder, HexEncoder
+from nacl.encoding import HexEncoder
 from nacl.public import Box, PrivateKey, PublicKey
 from pydantic import BaseModel, SecretStr
 
 
 class KeyPair(BaseModel):
     private_key: SecretStr
-    public_key: SecretStr
+    public_key: str
 
 
 class Crypt:
-    def __init__(self, private_key: bytes, msg_encoder=Base64Encoder, key_encoder=HexEncoder):
+    key_length: int = 32
+
+    def __init__(self, private_key: bytes, msg_encoder=HexEncoder, key_encoder=HexEncoder):
         self.msg_encoder = msg_encoder
         self.key_encoder = key_encoder
         self._private_key = PrivateKey(private_key, encoder=self.key_encoder)
 
     @property
+    def private_key(self) -> bytes:
+        return self._private_key.encode(self.key_encoder)
+
+    @property
     def public_key(self) -> bytes:
         return self._private_key.public_key._public_key
 
     @property
     def encoded_public_key(self) -> bytes:
         return self.key_encoder.encode(self.public_key)
 
     @classmethod
     def generate(cls, encoder=HexEncoder) -> KeyPair:
         private_key = PrivateKey.generate()
         private_key_encoded = private_key.encode(encoder)
         public_key_encoded = private_key.public_key.encode(encoder)
         return KeyPair(private_key=private_key_encoded, public_key=public_key_encoded)
 
-    def encrypt(self, msg: bytes, public_key: bytes) -> str:
+    def encrypt(self, msg: bytes, public_key: bytes) -> bytes:
         secret = Box(self._private_key, PublicKey(public_key, encoder=self.key_encoder))
         encrypted = secret.encrypt(msg)
-        return self.msg_encoder.encode(encrypted).decode()
+        formatted = b''.join([self.public_key, encrypted])
+        return self.msg_encoder.encode(formatted)
 
-    def decrypt(self, msg: bytes, public_key: bytes) -> bytes:
+    def decrypt(self, msg: bytes) -> bytes:
         decoded = self.msg_encoder.decode(msg)
-        secret = Box(self._private_key, PublicKey(public_key, encoder=self.key_encoder))
-        return secret.decrypt(decoded)
+        key = self.key_encoder.encode(decoded[: self.key_length])
+        data = decoded[self.key_length :]
+        secret = Box(self._private_key, PublicKey(key, encoder=self.key_encoder))
+        return secret.decrypt(data)
```

### Comparing `monstermash-0.7.6/PKG-INFO` & `monstermash-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monstermash
-Version: 0.7.6
+Version: 1.0.0
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
 
-> 1️⃣ version: 0.7.6
+> 1️⃣ version: 1.0.0
 
 > ✍️ author: Mitchell Lisle
 
 ## Install
 Install from PyPi
 
 ```shell
```

