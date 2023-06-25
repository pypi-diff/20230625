# Comparing `tmp/meilisearch-fastapi-0.9.1.tar.gz` & `tmp/meilisearch-fastapi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meilisearch-fastapi-0.9.1.tar", max compression
+gzip compressed data, was "meilisearch-fastapi-0.9.2.tar", max compression
```

## Comparing `meilisearch-fastapi-0.9.1.tar` & `meilisearch-fastapi-0.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1069 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/LICENSE
--rw-r--r--   0        0        0     3785 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/README.md
--rw-r--r--   0        0        0        0 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/__init__.py
--rw-r--r--   0        0        0      337 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/_config.py
--rw-r--r--   0        0        0      857 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/__init__.py
--rw-r--r--   0        0        0      430 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/document_info.py
--rw-r--r--   0        0        0     1367 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/index.py
--rw-r--r--   0        0        0      104 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/meili_message.py
--rw-r--r--   0        0        0      580 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/search_parameters.py
--rw-r--r--   0        0        0      132 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/settings.py
--rw-r--r--   0        0        0        0 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/py.typed
--rw-r--r--   0        0        0        0 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/__init__.py
--rw-r--r--   0        0        0     6212 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/document_routes.py
--rw-r--r--   0        0        0    14487 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/index_routes.py
--rw-r--r--   0        0        0     1361 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/meilisearch_routes.py
--rw-r--r--   0        0        0     1331 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/search_routes.py
--rw-r--r--   0        0        0     1985 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/settings_routes.py
--rw-r--r--   0        0        0     1706 2021-10-04 23:09:08.327586 meilisearch-fastapi-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4698 2021-10-04 23:09:47.530688 meilisearch-fastapi-0.9.1/setup.py
--rw-r--r--   0        0        0     4783 2021-10-04 23:09:47.531207 meilisearch-fastapi-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/LICENSE
+-rw-r--r--   0        0        0     3785 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/__init__.py
+-rw-r--r--   0        0        0      337 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/_config.py
+-rw-r--r--   0        0        0      857 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/__init__.py
+-rw-r--r--   0        0        0      430 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/document_info.py
+-rw-r--r--   0        0        0     1367 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/index.py
+-rw-r--r--   0        0        0      104 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/meili_message.py
+-rw-r--r--   0        0        0      580 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/search_parameters.py
+-rw-r--r--   0        0        0      132 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/settings.py
+-rw-r--r--   0        0        0        0 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/py.typed
+-rw-r--r--   0        0        0        0 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/__init__.py
+-rw-r--r--   0        0        0     6212 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/document_routes.py
+-rw-r--r--   0        0        0    14487 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/index_routes.py
+-rw-r--r--   0        0        0     1361 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/meilisearch_routes.py
+-rw-r--r--   0        0        0     1331 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/search_routes.py
+-rw-r--r--   0        0        0     1985 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/settings_routes.py
+-rw-r--r--   0        0        0     1706 2021-10-11 18:03:06.482998 meilisearch-fastapi-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4698 2021-10-11 18:03:52.101774 meilisearch-fastapi-0.9.2/setup.py
+-rw-r--r--   0        0        0     4783 2021-10-11 18:03:52.102230 meilisearch-fastapi-0.9.2/PKG-INFO
```

### Comparing `meilisearch-fastapi-0.9.1/LICENSE` & `meilisearch-fastapi-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/README.md` & `meilisearch-fastapi-0.9.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -70,12 +70,12 @@
 MEILISEARCH_API_KEY=masterKey  # This is the API key for your MeiliSearch instance
 ```
 
 Now the MeiliSearch routes will be available in your FastAPI app. Documentation for the routes can be viewed in the OpenAPI documentation of the FastAPI app. To view this start your FastAPI app and naviate to the docs `http://localhost:8000/docs` replacing the url with the correct url for your app.
 
 ## Compatibility with MeiliSearch
 
-This package only guarantees the compatibility with [version v0.22 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.22.0).
+This package only guarantees the compatibility with [version v0.23 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.23.0).
 
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/__init__.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/index.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/index.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/models/search_parameters.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/models/search_parameters.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/document_routes.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/document_routes.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/index_routes.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/index_routes.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/meilisearch_routes.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/meilisearch_routes.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/search_routes.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/search_routes.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/meilisearch_fastapi/routes/settings_routes.py` & `meilisearch-fastapi-0.9.2/meilisearch_fastapi/routes/settings_routes.py`

 * *Files identical despite different names*

### Comparing `meilisearch-fastapi-0.9.1/pyproject.toml` & `meilisearch-fastapi-0.9.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meilisearch-fastapi"
-version = "0.9.1"
+version = "0.9.2"
 description = "MeiliSearch integration with FastAPI"
 authors = ["Paul Sanders <psanders1@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/sanders41/meilisearch-fastapi"
 homepage = "https://github.com/sanders41/meilisearch-fastapi"
 documentation = "https://github.com/sanders41/meilisearch-fastapi"
@@ -17,17 +17,17 @@
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 include = ["meilisearch_fastapi/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-fastapi = ">=0.65.1,<0.69.0"
+fastapi = ">=0.65.1,<0.71.0"
 pydantic = {version = "^1.8.2", extras = ["dotenv"]}
-meilisearch-python-async = "^0.16.0"
+meilisearch-python-async = "^0.17.0"
 
 [tool.poetry.dev-dependencies]
 black = "^21.9b0"
 flake8 = "^3.9.2"
 isort = "^5.9.3"
 mypy = "^0.910"
 pre-commit = "^2.15.0"
```

### Comparing `meilisearch-fastapi-0.9.1/setup.py` & `meilisearch-fastapi-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
  'meilisearch_fastapi.models',
  'meilisearch_fastapi.routes']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['fastapi>=0.65.1,<0.69.0',
- 'meilisearch-python-async>=0.16.0,<0.17.0',
+['fastapi>=0.65.1,<0.71.0',
+ 'meilisearch-python-async>=0.17.0,<0.18.0',
  'pydantic[dotenv]>=1.8.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'meilisearch-fastapi',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'MeiliSearch integration with FastAPI',
-    'long_description': '# MeiliSearch FastAPI\n\n![CI Status](https://github.com/sanders41/meilisearch-fastapi/workflows/CI/badge.svg?branch=main&event=push)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/meilisearch-fastapi/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/meilisearch-fastapi/main)\n[![Coverage](https://codecov.io/gh/sanders41/meilisearch-fastapi/branch/main/graphs/badge.svg?branch=main)](https://codecov.io/gh/sanders41/meilisearch-fastapi)\n[![PyPI version](https://badge.fury.io/py/meilisearch-fastapi.svg)](https://badge.fury.io/py/meilisearch-fastapi)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/meilisearch-fastapi?color=5cc141)](https://github.com/sanders41/meilisearch-fastapi)\n\nMeiliSearch FastAPI provides [FastAPI](https://fastapi.tiangolo.com/) routes for interacting with [MeiliSearch](https://www.meilisearch.com/).\n\n## Installation\n\nUsing a virtual environmnet is recommended for installing this package. Once the virtual environment is created and activated install the package with:\n\n```sh\npip install meilisearch-fastapi\n```\n\n## Useage\n\nRoutes are split in groups so that different dependencies can be injected, and therefore different levels of access, can be given to different groups of routes.\n\n### Example with no authentication require for routes\n\n```py\nfrom fastapi import APIRouter, FastAPI\nfrom meilisearch_fastapi.routes import (\n    document_routes,\n    index_routes,\n    meilisearch_routes,\n    search_routes,\n    settings_routes,\n)\n\napp = FastAPI()\napi_router = APIRouter()\napi_router.include_router(document_routes.router, prefix="/documents")\napi_router.include_router(index_routes.router, prefix="/indexes")\napi_router.include_router(meilisearch_routes.router, prefix="/meilisearch")\napi_router.include_router(search_routes.router, prefix="/search")\napi_router.include_router(settings_routes.router, prefix="/settings")\n\napp.include_router(api_router)\n```\n\n### Example with routes requiring authentication\n\n```py\nfrom fastapi import APIRouter, FastAPI\nfrom meilisearch_fastapi import routes\n\nfrom my_app import my_authentication\n\napp = FastAPI()\napi_router = APIRouter()\napi_router.include_router(document_routes.router, prefix="/documents", dependeincies=[Depends(my_authentication)])\napi_router.include_router(index_routes.router, prefix="/indexes", dependeincies=[Depends(my_authentication)])\napi_router.include_router(meilisearch_routes.router, prefix="/meilisearch", dependeincies=[Depends(my_authentication)])\napi_router.include_router(search_routes.router, prefix="/search", dependeincies=[Depends(my_authentication)])\napi_router.include_router(settings_routes.router, prefix="/settings", dependeincies=[Depends(my_authentication)])\n\napp.include_router(api_router)\n```\n\nThe url for MeiliSearch and API key are read from environment variables. Putting these into a .env\nfile will keep you from having to set these variables each time the terminal is restarted.\n\n```txt\nMEILISEARCH_URL=http://localhost:7700  # This is the url for your instance of MeiliSearch\nMEILISEARCH_API_KEY=masterKey  # This is the API key for your MeiliSearch instance\n```\n\nNow the MeiliSearch routes will be available in your FastAPI app. Documentation for the routes can be viewed in the OpenAPI documentation of the FastAPI app. To view this start your FastAPI app and naviate to the docs `http://localhost:8000/docs` replacing the url with the correct url for your app.\n\n## Compatibility with MeiliSearch\n\nThis package only guarantees the compatibility with [version v0.22 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.22.0).\n\n## Contributing\n\nContributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)\n',
+    'long_description': '# MeiliSearch FastAPI\n\n![CI Status](https://github.com/sanders41/meilisearch-fastapi/workflows/CI/badge.svg?branch=main&event=push)\n[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/sanders41/meilisearch-fastapi/main.svg)](https://results.pre-commit.ci/latest/github/sanders41/meilisearch-fastapi/main)\n[![Coverage](https://codecov.io/gh/sanders41/meilisearch-fastapi/branch/main/graphs/badge.svg?branch=main)](https://codecov.io/gh/sanders41/meilisearch-fastapi)\n[![PyPI version](https://badge.fury.io/py/meilisearch-fastapi.svg)](https://badge.fury.io/py/meilisearch-fastapi)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/meilisearch-fastapi?color=5cc141)](https://github.com/sanders41/meilisearch-fastapi)\n\nMeiliSearch FastAPI provides [FastAPI](https://fastapi.tiangolo.com/) routes for interacting with [MeiliSearch](https://www.meilisearch.com/).\n\n## Installation\n\nUsing a virtual environmnet is recommended for installing this package. Once the virtual environment is created and activated install the package with:\n\n```sh\npip install meilisearch-fastapi\n```\n\n## Useage\n\nRoutes are split in groups so that different dependencies can be injected, and therefore different levels of access, can be given to different groups of routes.\n\n### Example with no authentication require for routes\n\n```py\nfrom fastapi import APIRouter, FastAPI\nfrom meilisearch_fastapi.routes import (\n    document_routes,\n    index_routes,\n    meilisearch_routes,\n    search_routes,\n    settings_routes,\n)\n\napp = FastAPI()\napi_router = APIRouter()\napi_router.include_router(document_routes.router, prefix="/documents")\napi_router.include_router(index_routes.router, prefix="/indexes")\napi_router.include_router(meilisearch_routes.router, prefix="/meilisearch")\napi_router.include_router(search_routes.router, prefix="/search")\napi_router.include_router(settings_routes.router, prefix="/settings")\n\napp.include_router(api_router)\n```\n\n### Example with routes requiring authentication\n\n```py\nfrom fastapi import APIRouter, FastAPI\nfrom meilisearch_fastapi import routes\n\nfrom my_app import my_authentication\n\napp = FastAPI()\napi_router = APIRouter()\napi_router.include_router(document_routes.router, prefix="/documents", dependeincies=[Depends(my_authentication)])\napi_router.include_router(index_routes.router, prefix="/indexes", dependeincies=[Depends(my_authentication)])\napi_router.include_router(meilisearch_routes.router, prefix="/meilisearch", dependeincies=[Depends(my_authentication)])\napi_router.include_router(search_routes.router, prefix="/search", dependeincies=[Depends(my_authentication)])\napi_router.include_router(settings_routes.router, prefix="/settings", dependeincies=[Depends(my_authentication)])\n\napp.include_router(api_router)\n```\n\nThe url for MeiliSearch and API key are read from environment variables. Putting these into a .env\nfile will keep you from having to set these variables each time the terminal is restarted.\n\n```txt\nMEILISEARCH_URL=http://localhost:7700  # This is the url for your instance of MeiliSearch\nMEILISEARCH_API_KEY=masterKey  # This is the API key for your MeiliSearch instance\n```\n\nNow the MeiliSearch routes will be available in your FastAPI app. Documentation for the routes can be viewed in the OpenAPI documentation of the FastAPI app. To view this start your FastAPI app and naviate to the docs `http://localhost:8000/docs` replacing the url with the correct url for your app.\n\n## Compatibility with MeiliSearch\n\nThis package only guarantees the compatibility with [version v0.23 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.23.0).\n\n## Contributing\n\nContributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)\n',
     'author': 'Paul Sanders',
     'author_email': 'psanders1@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sanders41/meilisearch-fastapi',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `meilisearch-fastapi-0.9.1/PKG-INFO` & `meilisearch-fastapi-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: meilisearch-fastapi
-Version: 0.9.1
+Version: 0.9.2
 Summary: MeiliSearch integration with FastAPI
 Home-page: https://github.com/sanders41/meilisearch-fastapi
 License: MIT
 Keywords: meilisearch,fastapi,async,search
 Author: Paul Sanders
 Author-email: psanders1@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: fastapi (>=0.65.1,<0.69.0)
-Requires-Dist: meilisearch-python-async (>=0.16.0,<0.17.0)
+Requires-Dist: fastapi (>=0.65.1,<0.71.0)
+Requires-Dist: meilisearch-python-async (>=0.17.0,<0.18.0)
 Requires-Dist: pydantic[dotenv] (>=1.8.2,<2.0.0)
 Project-URL: Documentation, https://github.com/sanders41/meilisearch-fastapi
 Project-URL: Repository, https://github.com/sanders41/meilisearch-fastapi
 Description-Content-Type: text/markdown
 
 # MeiliSearch FastAPI
 
@@ -94,13 +94,13 @@
 MEILISEARCH_API_KEY=masterKey  # This is the API key for your MeiliSearch instance
 ```
 
 Now the MeiliSearch routes will be available in your FastAPI app. Documentation for the routes can be viewed in the OpenAPI documentation of the FastAPI app. To view this start your FastAPI app and naviate to the docs `http://localhost:8000/docs` replacing the url with the correct url for your app.
 
 ## Compatibility with MeiliSearch
 
-This package only guarantees the compatibility with [version v0.22 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.22.0).
+This package only guarantees the compatibility with [version v0.23 of MeiliSearch](https://github.com/meilisearch/MeiliSearch/releases/tag/v0.23.0).
 
 ## Contributing
 
 Contributions to this project are welcome. If you are interesting in contributing please see our [contributing guide](CONTRIBUTING.md)
```

