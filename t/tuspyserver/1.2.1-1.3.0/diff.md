# Comparing `tmp/tuspyserver-1.2.1.tar.gz` & `tmp/tuspyserver-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuspyserver-1.2.1.tar", last modified: Tue Feb 28 16:55:02 2023, max compression
+gzip compressed data, was "tuspyserver-1.3.0.tar", last modified: Sun Jun 25 13:25:46 2023, max compression
```

## Comparing `tuspyserver-1.2.1.tar` & `tuspyserver-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 16:55:02.750517 tuspyserver-1.2.1/
--rw-rw-rw-   0        0        0     1107 2022-12-30 11:20:31.000000 tuspyserver-1.2.1/LICENSE
--rw-rw-rw-   0        0        0     2073 2023-02-28 16:55:02.749497 tuspyserver-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1393 2023-02-19 16:25:46.000000 tuspyserver-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-02-28 16:55:02.750517 tuspyserver-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1155 2023-02-28 16:54:57.000000 tuspyserver-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-28 16:55:02.744640 tuspyserver-1.2.1/tuspyserver.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-02-28 16:55:02.000000 tuspyserver-1.2.1/tuspyserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-02-28 16:55:02.000000 tuspyserver-1.2.1/tuspyserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 16:55:02.000000 tuspyserver-1.2.1/tuspyserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-02-28 16:55:02.000000 tuspyserver-1.2.1/tuspyserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-02-28 16:55:02.000000 tuspyserver-1.2.1/tuspyserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-28 16:55:02.748389 tuspyserver-1.2.1/tusserver/
--rw-rw-rw-   0        0        0       23 2023-01-02 11:51:05.000000 tuspyserver-1.2.1/tusserver/__init__.py
--rw-rw-rw-   0        0        0      770 2022-12-30 20:58:07.000000 tuspyserver-1.2.1/tusserver/metadata.py
--rw-rw-rw-   0        0        0    10919 2023-02-28 16:54:16.000000 tuspyserver-1.2.1/tusserver/tus.py
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910954 tuspyserver-1.3.0/
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1086 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/LICENSE
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:25:46.910840 tuspyserver-1.3.0/PKG-INFO
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1393 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/README.md
+-rw-r--r--   0 edihasaj   (501) staff       (20)       38 2023-06-25 13:25:46.910992 tuspyserver-1.3.0/setup.cfg
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1116 2023-06-25 13:24:39.000000 tuspyserver-1.3.0/setup.py
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910339 tuspyserver-1.3.0/tuspyserver.egg-info/
+-rw-r--r--   0 edihasaj   (501) staff       (20)     1997 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/PKG-INFO
+-rw-r--r--   0 edihasaj   (501) staff       (20)      261 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/SOURCES.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)        1 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/dependency_links.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)       51 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/requires.txt
+-rw-r--r--   0 edihasaj   (501) staff       (20)       10 2023-06-25 13:25:46.000000 tuspyserver-1.3.0/tuspyserver.egg-info/top_level.txt
+drwxr-xr-x   0 edihasaj   (501) staff       (20)        0 2023-06-25 13:25:46.910673 tuspyserver-1.3.0/tusserver/
+-rw-r--r--   0 edihasaj   (501) staff       (20)       22 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/tusserver/__init__.py
+-rw-r--r--   0 edihasaj   (501) staff       (20)      736 2023-06-25 12:40:59.000000 tuspyserver-1.3.0/tusserver/metadata.py
+-rw-r--r--   0 edihasaj   (501) staff       (20)    11358 2023-06-25 13:20:51.000000 tuspyserver-1.3.0/tusserver/tus.py
```

### Comparing `tuspyserver-1.2.1/LICENSE` & `tuspyserver-1.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Tus Server for FastAPI Python
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Tus Server for FastAPI Python
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `tuspyserver-1.2.1/PKG-INFO` & `tuspyserver-1.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-Metadata-Version: 2.1
-Name: tuspyserver
-Version: 1.2.1
-Summary: TUS py protocol implementation in FastAPI
-Home-page: https://github.com/edihasaj/tuspy-fast-api
-Author: Edi Hasaj
-Author-email: edihasaj@outlook.com
-License: MIT
-Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FastAPI Tus
-
-FastAPI Extension implementing the Tus.io server protocol
-
-### Prerequisites `FastAPI`
-
-## Installation
-
-Installation from PyPi repository (recommended for latest stable release)
-
-```
-pip install tuspyserver
-```
-
-## Usage
-
-### main.py
-
-```python
-from fastapi import FastAPI
-from starlette.middleware.cors import CORSMiddleware
-from starlette.staticfiles import StaticFiles
-
-from tusserver.tus import create_api_router
-
-app = FastAPI()
-app.add_middleware(
-    CORSMiddleware,
-    allow_origins=['*'],
-    allow_methods=["*"],
-    allow_headers=["*"],
-)
-app.mount("/static", StaticFiles(directory="static"), name="static")
-
-
-def on_upload_complete(file_path: str):
-    print('Upload complete')
-    print(file_path)
-
-
-app.include_router(
-    create_api_router(
-        files_dir='/tmp/different_dir', # OPTIONAL
-        location='http://127.0.0.1:8000/files', # OPTIONAL
-        max_size=128849018880, # OPTIONAL
-        on_upload_complete=on_upload_complete # OPTIONAL
-    ),
-    prefix="/files"
-)
-```
-
-This package has the ability to upload, download, delete (including a scheduler) files.
-
-```python setup.py sdist bdist_wheel```
-
-Any contribution is welcomed.
-
-<a href="https://www.buymeacoffee.com/edihasaj" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+Metadata-Version: 2.1
+Name: tuspyserver
+Version: 1.3.0
+Summary: TUS py protocol implementation in FastAPI
+Home-page: https://github.com/edihasaj/tuspy-fast-api
+Author: Edi Hasaj
+Author-email: edihasaj@outlook.com
+License: MIT
+Platform: any
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FastAPI Tus
+
+FastAPI Extension implementing the Tus.io server protocol
+
+### Prerequisites `FastAPI`
+
+## Installation
+
+Installation from PyPi repository (recommended for latest stable release)
+
+```
+pip install tuspyserver
+```
+
+## Usage
+
+### main.py
+
+```python
+from fastapi import FastAPI
+from starlette.middleware.cors import CORSMiddleware
+from starlette.staticfiles import StaticFiles
+
+from tusserver.tus import create_api_router
+
+app = FastAPI()
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=['*'],
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
+app.mount("/static", StaticFiles(directory="static"), name="static")
+
+
+def on_upload_complete(file_path: str):
+    print('Upload complete')
+    print(file_path)
+
+
+app.include_router(
+    create_api_router(
+        files_dir='/tmp/different_dir', # OPTIONAL
+        location='http://127.0.0.1:8000/files', # OPTIONAL
+        max_size=128849018880, # OPTIONAL
+        on_upload_complete=on_upload_complete # OPTIONAL
+    ),
+    prefix="/files"
+)
+```
+
+This package has the ability to upload, download, delete (including a scheduler) files.
+
+```python setup.py sdist bdist_wheel```
+
+Any contribution is welcomed.
+
+<a href="https://www.buymeacoffee.com/edihasaj" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tuspyserver Version: 1.2.1 Summary: TUS py protocol
+Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.0 Summary: TUS py protocol
 implementation in FastAPI Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj Author-email: edihasaj@outlook.com License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown License-File: LICENSE # FastAPI Tus
```

### Comparing `tuspyserver-1.2.1/README.md` & `tuspyserver-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tuspyserver-1.2.1/tuspyserver.egg-info/PKG-INFO` & `tuspyserver-1.3.0/tuspyserver.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-Metadata-Version: 2.1
-Name: tuspyserver
-Version: 1.2.1
-Summary: TUS py protocol implementation in FastAPI
-Home-page: https://github.com/edihasaj/tuspy-fast-api
-Author: Edi Hasaj
-Author-email: edihasaj@outlook.com
-License: MIT
-Platform: any
-Classifier: Environment :: Web Environment
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# FastAPI Tus
-
-FastAPI Extension implementing the Tus.io server protocol
-
-### Prerequisites `FastAPI`
-
-## Installation
-
-Installation from PyPi repository (recommended for latest stable release)
-
-```
-pip install tuspyserver
-```
-
-## Usage
-
-### main.py
-
-```python
-from fastapi import FastAPI
-from starlette.middleware.cors import CORSMiddleware
-from starlette.staticfiles import StaticFiles
-
-from tusserver.tus import create_api_router
-
-app = FastAPI()
-app.add_middleware(
-    CORSMiddleware,
-    allow_origins=['*'],
-    allow_methods=["*"],
-    allow_headers=["*"],
-)
-app.mount("/static", StaticFiles(directory="static"), name="static")
-
-
-def on_upload_complete(file_path: str):
-    print('Upload complete')
-    print(file_path)
-
-
-app.include_router(
-    create_api_router(
-        files_dir='/tmp/different_dir', # OPTIONAL
-        location='http://127.0.0.1:8000/files', # OPTIONAL
-        max_size=128849018880, # OPTIONAL
-        on_upload_complete=on_upload_complete # OPTIONAL
-    ),
-    prefix="/files"
-)
-```
-
-This package has the ability to upload, download, delete (including a scheduler) files.
-
-```python setup.py sdist bdist_wheel```
-
-Any contribution is welcomed.
-
-<a href="https://www.buymeacoffee.com/edihasaj" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
+Metadata-Version: 2.1
+Name: tuspyserver
+Version: 1.3.0
+Summary: TUS py protocol implementation in FastAPI
+Home-page: https://github.com/edihasaj/tuspy-fast-api
+Author: Edi Hasaj
+Author-email: edihasaj@outlook.com
+License: MIT
+Platform: any
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# FastAPI Tus
+
+FastAPI Extension implementing the Tus.io server protocol
+
+### Prerequisites `FastAPI`
+
+## Installation
+
+Installation from PyPi repository (recommended for latest stable release)
+
+```
+pip install tuspyserver
+```
+
+## Usage
+
+### main.py
+
+```python
+from fastapi import FastAPI
+from starlette.middleware.cors import CORSMiddleware
+from starlette.staticfiles import StaticFiles
+
+from tusserver.tus import create_api_router
+
+app = FastAPI()
+app.add_middleware(
+    CORSMiddleware,
+    allow_origins=['*'],
+    allow_methods=["*"],
+    allow_headers=["*"],
+)
+app.mount("/static", StaticFiles(directory="static"), name="static")
+
+
+def on_upload_complete(file_path: str):
+    print('Upload complete')
+    print(file_path)
+
+
+app.include_router(
+    create_api_router(
+        files_dir='/tmp/different_dir', # OPTIONAL
+        location='http://127.0.0.1:8000/files', # OPTIONAL
+        max_size=128849018880, # OPTIONAL
+        on_upload_complete=on_upload_complete # OPTIONAL
+    ),
+    prefix="/files"
+)
+```
+
+This package has the ability to upload, download, delete (including a scheduler) files.
+
+```python setup.py sdist bdist_wheel```
+
+Any contribution is welcomed.
+
+<a href="https://www.buymeacoffee.com/edihasaj" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-red.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tuspyserver Version: 1.2.1 Summary: TUS py protocol
+Metadata-Version: 2.1 Name: tuspyserver Version: 1.3.0 Summary: TUS py protocol
 implementation in FastAPI Home-page: https://github.com/edihasaj/tuspy-fast-api
 Author: Edi Hasaj Author-email: edihasaj@outlook.com License: MIT Platform: any
 Classifier: Environment :: Web Environment Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown License-File: LICENSE # FastAPI Tus
```

### Comparing `tuspyserver-1.2.1/tusserver/tus.py` & `tuspyserver-1.3.0/tusserver/tus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import base64
 import json
 import os
 from datetime import datetime, timedelta
-from typing import Callable
+from typing import Callable, Optional
 from uuid import uuid4
 
 from fastapi import Header, HTTPException, Response, Request, status, Depends, Path, APIRouter
 from starlette.responses import FileResponse
 
 from tusserver.metadata import FileMetadata
 
 
 def create_api_router(
         files_dir='/tmp/files',
         location='http://127.0.0.1:8000/files',
         max_size=128849018880,
-        on_upload_complete: Callable[[str], None] = None,
+        on_upload_complete: Optional[Callable[[str], None]] = None,
+        auth: Optional[Callable[[], None]] = None,
+        days_to_keep: int = 5,
 ):
     router = APIRouter()
 
     tus_version = '1.0.0'
     tus_extension = 'creation,creation-defer-length,creation-with-upload,expiration,termination'
-    days_to_keep = 5
 
     async def _get_request_chunk(request: Request, uuid: str = Path(...), post_request: bool = False) -> bool | None:
         meta = _read_metadata(uuid)
         if not meta or not _file_exists(uuid):
             return False
 
         with open(f"{files_dir}/{uuid}", "ab") as f:
@@ -43,15 +44,15 @@
                 _write_metadata(meta)
 
             f.close()
 
         return True
 
     @router.head("/{uuid}", status_code=status.HTTP_200_OK)
-    def get_upload_metadata(response: Response, uuid: str) -> Response:
+    def get_upload_metadata(response: Response, uuid: str, _=Depends(auth)) -> Response:
         meta = _read_metadata(uuid)
         if meta is None or not _file_exists(uuid):
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND)
 
         response.headers["Tus-Resumable"] = tus_version
         response.headers["Content-Length"] = str(meta.size)
         response.headers["Upload-Length"] = str(meta.size)
@@ -67,30 +68,28 @@
     def upload_chunk(
             response: Response,
             uuid: str,
             content_type: str = Header(None),
             content_length: int = Header(None),
             upload_offset: int = Header(None),
             _=Depends(_get_request_chunk),
+            __=Depends(auth)
     ) -> Response:
         response_headers = _get_and_save_the_file(
             response,
             uuid,
             content_type,
             content_length,
             upload_offset,
         )
 
-        if on_upload_complete:
-            on_upload_complete(os.path.join(files_dir, f'{uuid}'))
-
         return response_headers
 
     @router.options("/", status_code=status.HTTP_204_NO_CONTENT)
-    def options_create_upload(response: Response) -> Response:
+    def options_create_upload(response: Response, __=Depends(auth)) -> Response:
         response.headers["Tus-Extension"] = tus_extension
         response.headers["Tus-Resumable"] = tus_version
         response.headers["Tus-Version"] = tus_version
         response.headers["Tus-Max-Size"] = str(max_size)
         response.headers["Content-Length"] = str(0)
         response.status_code = status.HTTP_204_NO_CONTENT
         return response
@@ -98,14 +97,15 @@
     @router.post("/", status_code=status.HTTP_201_CREATED)
     async def create_upload(
             request: Request,
             response: Response,
             upload_metadata: str = Header(None),
             upload_length: int = Header(None),
             upload_defer_length: int = Header(None),
+            _=Depends(auth)
     ) -> Response:
         if upload_defer_length is not None and upload_defer_length != 1:
             raise HTTPException(status_code=400, detail="Invalid Upload-Defer-Length")
 
         defer_length = upload_defer_length is not None
 
         # Create a new upload and store the file and metadata in the mapping
@@ -117,15 +117,20 @@
                 decoded_value = base64.b64decode(value.strip()).decode("utf-8")
                 metadata[key.strip()] = decoded_value
 
         uuid = str(uuid4().hex)
 
         date_expiry = datetime.now() + timedelta(days=days_to_keep)
         saved_meta_data = FileMetadata.from_request(
-            uuid, metadata, upload_length, str(datetime.now()), defer_length, str(date_expiry.isoformat())
+            uuid,
+            metadata,
+            upload_length,
+            str(datetime.now()),
+            defer_length,
+            str(date_expiry.isoformat()),
         )
         _write_metadata(saved_meta_data)
 
         _initialize_file(uuid)
 
         chunk: bool | None = await _get_request_chunk(request, uuid, True)
         if chunk:
@@ -139,15 +144,15 @@
         response.headers["Location"] = f"{location}/{uuid}"
         response.headers["Tus-Resumable"] = tus_version
         response.headers["Content-Length"] = str(0)
         response.status_code = status.HTTP_201_CREATED
         return response
 
     @router.options("/{uuid}", status_code=status.HTTP_204_NO_CONTENT)
-    def options_upload_chunk(response: Response, uuid: str) -> Response:
+    def options_upload_chunk(response: Response, uuid: str, _=Depends(auth)) -> Response:
         meta = _read_metadata(uuid)
         if meta is None or not _file_exists(uuid):
             raise HTTPException(status_code=status.HTTP_404_NOT_FOUND)
 
         response.headers["Tus-Extension"] = tus_extension
         response.headers["Tus-Resumable"] = tus_version
         response.headers["Tus-Version"] = tus_version
@@ -171,15 +176,15 @@
             headers={
                 "Content-Length": str(meta.offset),
                 "Tus-Resumable": tus_version
             }
         )
 
     @router.delete("/{uuid}", status_code=status.HTTP_204_NO_CONTENT)
-    def delete_upload(uuid: str, response: Response) -> Response:
+    def delete_upload(uuid: str, response: Response, _=Depends(auth)) -> Response:
         meta = _read_metadata(uuid)
 
         # Check if the upload ID is valid
         if not meta or uuid != meta.uid or not _file_exists(uuid):
             raise HTTPException(status_code=404, detail="Upload not found")
 
         # Delete the file and metadata for the upload from the mapping
@@ -246,32 +251,39 @@
             raise HTTPException(status_code=415)
 
         meta = _read_metadata(uuid)
         # Check if the upload ID is valid
         if not meta or uuid != meta.uid:
             raise HTTPException(status_code=404)
 
-        if meta.defer_length and upload_length is None:
-            raise HTTPException(status_code=400, detail="Upload-Length header is required")
-
         # Check if the Upload Offset with Content-Length header is correct
         if meta.offset != upload_length + content_length:
             raise HTTPException(status_code=409)
 
         if meta.defer_length:
             meta.size = upload_length
 
         if not meta.expires:
             date_expiry = datetime.now() + timedelta(days=days_to_keep)
             meta.expires = str(date_expiry.isoformat())
         _write_metadata(meta)
 
+        if meta.size == meta.offset:
+            response.headers["Tus-Resumable"] = tus_version
+            response.headers["Upload-Offset"] = str(str(meta.offset) if meta.offset > 0 else str(content_length))
+            response.headers["Upload-Expires"] = str(meta.expires)
+            response.status_code = status.HTTP_204_NO_CONTENT
+            if on_upload_complete:
+                on_upload_complete(os.path.join(files_dir, f'{uuid}'))
+
+            return response
+
         response.headers["Tus-Resumable"] = tus_version
         response.headers["Upload-Offset"] = str(meta.offset)
-        # response.headers["Upload-Expires"] = str(datetime.fromisoformat(meta.expires).strftime("%a, %d %b %G %T %Z"))
+        response.headers["Upload-Expires"] = str(meta.expires)
         response.status_code = status.HTTP_204_NO_CONTENT
         return response
 
     def remove_expired_files():
         file_list = os.listdir(files_dir)
 
         file_list_to_remove = []
```

