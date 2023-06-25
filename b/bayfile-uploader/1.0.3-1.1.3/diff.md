# Comparing `tmp/bayfile_uploader-1.0.3-py3-none-any.whl.zip` & `tmp/bayfile_uploader-1.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3371 bytes, number of entries: 8
+Zip file size: 3436 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-25 09:38 bayfile_uploader/__init__.py
--rw-rw-r--  2.0 unx      752 b- defN 23-Jun-25 09:39 bayfile_uploader/uploader.py
--rw-rw-r--  2.0 unx     1068 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1088 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       67 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       17 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      701 b- defN 23-Jun-25 09:53 bayfile_uploader-1.0.3.dist-info/RECORD
-8 files, 3785 bytes uncompressed, 2123 bytes compressed:  43.9%
+-rw-rw-r--  2.0 unx      864 b- defN 23-Jun-25 10:21 bayfile_uploader/uploader.py
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       67 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      701 b- defN 23-Jun-25 10:26 bayfile_uploader-1.1.3.dist-info/RECORD
+8 files, 3935 bytes uncompressed, 2188 bytes compressed:  44.4%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: bayfile_uploader/__init__.py
 Comment: 
 
 Filename: bayfile_uploader/uploader.py
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/LICENSE
+Filename: bayfile_uploader-1.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/METADATA
+Filename: bayfile_uploader-1.1.3.dist-info/METADATA
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/WHEEL
+Filename: bayfile_uploader-1.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/entry_points.txt
+Filename: bayfile_uploader-1.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/top_level.txt
+Filename: bayfile_uploader-1.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: bayfile_uploader-1.0.3.dist-info/RECORD
+Filename: bayfile_uploader-1.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## bayfile_uploader/uploader.py

```diff
@@ -1,33 +1,36 @@
 from requests import post
 from json import loads
-import sys
 from os import path
+import click
+import sys
 
 
 url = 'https://api.bayfiles.com/upload'
 
 
 def upload_file(file_name: str) -> None:
     with open(file_name, 'rb') as f:
         response = post(url, files={'file': f})
         json_data = loads(response.text)
         if response.status_code == 200:
             print(json_data['data']['file']['url']['full'])
         else:
-            print(json_data['error']['message'], file_name)
+            print(json_data['error']['message'], file_name, file=sys.stderr)
 
 
-def main():
-    if len(sys.argv) > 1:
-        file = sys.argv[1]
-        if path.exists(file):
-            upload_file(sys.argv[1])
-        else:
-            print(f'Invalid file: {file}')
-
+@click.command()
+@click.option(
+        '--file', 
+        prompt='Enter the file you want to upload', 
+        help='The file you wanto to upload', 
+        type=click.File('r')
+)
+def main(file):
+    if path.exists(file.name):
+        upload_file(file.name)
     else:
-        print('missing parameter for file.')
+        print(f'File not found: {file}', file=sys.stderr)
 
 
 if __name__ == '__main__':
     main()
```

## Comparing `bayfile_uploader-1.0.3.dist-info/LICENSE` & `bayfile_uploader-1.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bayfile_uploader-1.0.3.dist-info/METADATA` & `bayfile_uploader-1.1.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: bayfile-uploader
-Version: 1.0.3
+Version: 1.1.3
 Summary: File Uploader, uploads files to bayfiles.com
 Home-page: https://github.com/roymanigley/bayfile-uploader
 Author: Roy Manigley
 Author-email: roy.manigley@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click (>=8.1.3)
 Requires-Dist: requests (>=2.28.1)
 
 # Bayfile Uploader
 > Uploads a file to [bayfiles.com](https://bayfiles.com/docs/api)
 
 ## Installation
 ```
@@ -35,11 +36,11 @@
 from bayfile_uploader.uploader import upload_file
 
 link = upload_file('/path/to/file')
 print(f'The file is uploaded: {link}')
 ```
 or from the commandline
 ```
-bayfile_upload /path/to/file
+bayfile_upload --file /path/to/file
 ```
```

