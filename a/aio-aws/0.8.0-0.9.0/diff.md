# Comparing `tmp/aio-aws-0.8.0.tar.gz` & `tmp/aio-aws-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-aws-0.8.0.tar", last modified: Tue Mar  9 01:34:07 2021, max compression
+gzip compressed data, was "aio-aws-0.9.0.tar", last modified: Mon Mar 29 20:08:23 2021, max compression
```

## Comparing `aio-aws-0.8.0.tar` & `aio-aws-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2020-03-29 20:20:45.857284 aio-aws-0.8.0/LICENSE
--rw-r--r--   0        0        0     3707 2021-03-09 01:32:08.048616 aio-aws-0.8.0/README.md
--rw-r--r--   0        0        0      646 2021-03-09 01:31:32.366784 aio-aws-0.8.0/aio_aws/__init__.py
--rwxr-xr-x   0        0        0    45143 2021-02-16 04:57:46.153190 aio-aws-0.8.0/aio_aws/aio_aws_batch.py
--rw-r--r--   0        0        0    11679 2021-03-09 01:31:32.366784 aio-aws-0.8.0/aio_aws/aio_aws_config.py
--rwxr-xr-x   0        0        0    10128 2021-02-16 04:57:46.153190 aio-aws-0.8.0/aio_aws/aio_aws_lambda.py
--rwxr-xr-x   0        0        0    24580 2021-02-13 23:16:08.256320 aio-aws-0.8.0/aio_aws/aio_aws_s3.py
--rwxr-xr-x   0        0        0    13922 2021-02-16 04:57:46.157192 aio-aws-0.8.0/aio_aws/async_executor.py
--rwxr-xr-x   0        0        0      955 2021-02-16 04:57:46.157192 aio-aws-0.8.0/aio_aws/async_main.py
--rw-r--r--   0        0        0     1088 2021-02-13 23:16:08.256320 aio-aws-0.8.0/aio_aws/logger.py
--rw-r--r--   0        0        0      280 2021-03-09 01:32:08.048616 aio-aws-0.8.0/aio_aws/version.py
--rw-r--r--   0        0        0     1956 2021-03-09 01:32:08.048616 aio-aws-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4739 2021-03-09 01:34:07.169259 aio-aws-0.8.0/setup.py
--rw-r--r--   0        0        0     4911 2021-03-09 01:34:07.169545 aio-aws-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2020-03-29 20:20:45.857284 aio-aws-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3707 2021-03-29 18:33:19.503891 aio-aws-0.9.0/README.md
+-rw-r--r--   0        0        0      646 2021-03-09 01:31:32.366784 aio-aws-0.9.0/aio_aws/__init__.py
+-rwxr-xr-x   0        0        0    45143 2021-02-16 04:57:46.153190 aio-aws-0.9.0/aio_aws/aio_aws_batch.py
+-rw-r--r--   0        0        0    11679 2021-03-09 01:31:32.366784 aio-aws-0.9.0/aio_aws/aio_aws_config.py
+-rwxr-xr-x   0        0        0    10140 2021-03-29 18:32:44.371608 aio-aws-0.9.0/aio_aws/aio_aws_lambda.py
+-rwxr-xr-x   0        0        0    24580 2021-03-29 20:08:14.974832 aio-aws-0.9.0/aio_aws/aio_aws_s3.py
+-rwxr-xr-x   0        0        0    13922 2021-02-16 04:57:46.157192 aio-aws-0.9.0/aio_aws/async_executor.py
+-rwxr-xr-x   0        0        0      955 2021-02-16 04:57:46.157192 aio-aws-0.9.0/aio_aws/async_main.py
+-rw-r--r--   0        0        0     1088 2021-02-13 23:16:08.256320 aio-aws-0.9.0/aio_aws/logger.py
+-rw-r--r--   0        0        0      280 2021-03-29 18:33:19.503891 aio-aws-0.9.0/aio_aws/version.py
+-rw-r--r--   0        0        0     1956 2021-03-29 18:33:19.503891 aio-aws-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4739 2021-03-29 20:08:23.484491 aio-aws-0.9.0/setup.py
+-rw-r--r--   0        0        0     4911 2021-03-29 20:08:23.484843 aio-aws-0.9.0/PKG-INFO
```

### Comparing `aio-aws-0.8.0/LICENSE` & `aio-aws-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/README.md` & `aio-aws-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/__init__.py` & `aio-aws-0.9.0/aio_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/aio_aws_batch.py` & `aio-aws-0.9.0/aio_aws/aio_aws_batch.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/aio_aws_config.py` & `aio-aws-0.9.0/aio_aws/aio_aws_config.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/aio_aws_lambda.py` & `aio-aws-0.9.0/aio_aws/aio_aws_lambda.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
             params["Payload"] = self.payload
         if self.qualifier:
             params["Qualifier"] = self.qualifier
         return params
 
     async def invoke(
         self, config: AioAWSConfig, lambda_client: aiobotocore.client.AioBaseClient
-    ) -> Dict:
+    ) -> "AWSLambdaFunction":
         """
         Asynchronous coroutine to invoke a lambda function; this
         updates the ``response`` and calls the py:meth:`.read_response`
         method to handle the response.
 
         :param config: aio session and client settings
         :param lambda_client: aio client for lambda
@@ -173,15 +173,16 @@
                         elif self.error:
                             LOGGER.error(
                                 "AWS Lambda (%s) error: ", self.name, self.error
                             )
                     else:
                         # TODO: are there some failures that could be recovered here?
                         LOGGER.error("AWS Lambda (%s) invoke failure.", self.name)
-                    return response
+
+                    return self
 
                 except botocore.exceptions.ClientError as err:
                     error = err.response.get("Error", {})
                     if error.get("Code") == "TooManyRequestsException":
                         if tries < config.retries:
                             # add an extra random sleep period to avoid API throttle
                             await jitter(
```

### Comparing `aio-aws-0.8.0/aio_aws/aio_aws_s3.py` & `aio-aws-0.9.0/aio_aws/aio_aws_s3.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/async_executor.py` & `aio-aws-0.9.0/aio_aws/async_executor.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/async_main.py` & `aio-aws-0.9.0/aio_aws/async_main.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/aio_aws/logger.py` & `aio-aws-0.9.0/aio_aws/logger.py`

 * *Files identical despite different names*

### Comparing `aio-aws-0.8.0/pyproject.toml` & `aio-aws-0.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-aws"
-version = "0.8.0"
+version = "0.9.0"
 description = "aio-aws"
 authors = [
     "Darren Weber <dazza-codes@github.com>",
 ]
 license = "Apache-2.0"
 
 readme = "README.md"  # Markdown files are supported
```

### Comparing `aio-aws-0.8.0/setup.py` & `aio-aws-0.9.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
  'requests>=2.23.0,<3.0.0',
  'tinydb>=3.15,<4.0',
  'typer>=0.3.2,<0.4.0']
 
 extras_require = \
 {'all': ['aiofiles>=0.4.0,<0.5.0',
          'aioredis>=1.3,<2.0',
-         'databases[sqlite,postgresql,mysql]'],
+         'databases[sqlite,mysql,postgresql]'],
  'awscli': ['awscli>=1.18,<2.0']}
 
 setup_kwargs = {
     'name': 'aio-aws',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'aio-aws',
     'long_description': '[![Build Status](https://travis-ci.com/dazza-codes/aio-aws.svg?branch=master)](https://travis-ci.com/dazza-codes/aio-aws)\n\n# aio-aws\n\nAsynchronous functions and tools for AWS services.  There is a\nlimited focus on s3 and AWS Batch and Lambda.  Additional services could be\nadded, but this project is likely to retain a limited focus.\nFor general client solutions, see\n[aioboto3](https://github.com/terrycain/aioboto3) and\n[aiobotocore](https://github.com/aio-libs/aiobotocore), which wrap\n[botocore](https://botocore.amazonaws.com/v1/documentation/api/latest/index.html)\n\nThe API documentation is published as github pages at:\n- http://dazza-codes.github.io/aio-aws\n\n# Getting Started\n\nTo use the source code, it can be cloned directly. To\ncontribute to the project, first fork it and clone the forked repository.\n\nThe following setup assumes that\n[miniconda3](https://docs.conda.io/en/latest/miniconda.html) and\n[poetry](https://python-poetry.org/docs/) are installed already\n(and `make` 4.x).\n\n- https://docs.conda.io/en/latest/miniconda.html\n    - recommended for creating virtual environments with required versions of python\n    - see https://github.com/dazza-codes/conda_container/blob/master/conda_venv.sh\n- https://python-poetry.org/docs/\n    - recommended for managing a python project with pip dependencies for\n      both the project itself and development dependencies\n\n```shell\ngit clone https://github.com/dazza-codes/aio-aws\ncd aio-aws\nconda create -n aio-aws python=3.7\nconda activate aio-aws\nmake init  # calls poetry install\nmake test\n```\n\n# Install\n\nThis project has a very limited focus.  For general client solutions, see\n[aioboto3](https://github.com/terrycain/aioboto3) and\n[aiobotocore](https://github.com/aio-libs/aiobotocore), which wrap\n[botocore](https://botocore.amazonaws.com/v1/documentation/api/latest/index.html)\nto patch it with features for async coroutines using\n[aiohttp](https://aiohttp.readthedocs.io/en/latest/) and\n[asyncio](https://docs.python.org/3/library/asyncio.html).\n\nThis project is alpha-status with a 0.x.y API version that could break.\nThere is no promise to support or develop it extensively, at this time.\nFor the curious, it can be used directly from a github tag.  Note that\nany 0.x releases are likely to have breaking API changes.\n\n## pip\n\n```shell\npip install -U aio-aws[all]\npip check  # pip might not guarantee consistent packages\n```\n\n## poetry\n\npoetry will try to guarantee consistent packages or fail.\n\n```shell\n# with optional extras\npoetry add aio-aws --extras all\n```\n\n```toml\n# pyproject.toml snippet\n\n[tool.poetry.dependencies]\npython = "^3.7"\n\n# with optional extras\naio-aws = {version = "^0.1.0", extras = ["all"]}\n\n# or, to make it an optional extra\naio-aws = {version = "^0.1.0", extras = ["all"], optional = true}\n[tool.poetry.extras]\naio-aws = ["aio-aws"]\n\n```\n\n# License\n\n```text\nCopyright 2019-2020 Darren Weber\n\nLicensed under the Apache License, Version 2.0 (the "License");\nyou may not use this file except in compliance with the License.\nYou may obtain a copy of the License at\n\n   http://www.apache.org/licenses/LICENSE-2.0\n\nUnless required by applicable law or agreed to in writing, software\ndistributed under the License is distributed on an "AS IS" BASIS,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the License for the specific language governing permissions and\nlimitations under the License.\n```\n\n# Notices\n\nThis project is inspired by and uses various open source projects that use\nthe Apache 2 license, including but not limited to:\n- Apache Airflow: https://github.com/apache/airflow\n- aiobotocore: https://github.com/aio-libs/aiobotocore\n- botocore: https://github.com/boto/botocore\n',
     'author': 'Darren Weber',
     'author_email': 'dazza-codes@github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/dazza-codes/aio-aws',
```

### Comparing `aio-aws-0.8.0/PKG-INFO` & `aio-aws-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-aws
-Version: 0.8.0
+Version: 0.9.0
 Summary: aio-aws
 Home-page: https://github.com/dazza-codes/aio-aws
 License: Apache-2.0
 Keywords: Development Status :: 2 - Pre-Alpha,Intended Audience :: Developers,Operating System :: OS Independent,Programming Language :: Python :: 3,Topic :: Utilities
 Author: Darren Weber
 Author-email: dazza-codes@github.com
 Requires-Python: >=3.7,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Provides-Extra: awscli
 Requires-Dist: aiobotocore[boto3] (>=1.1.0,<2.0.0)
 Requires-Dist: aiofiles (>=0.4.0,<0.5.0); extra == "all"
 Requires-Dist: aioredis (>=1.3,<2.0); extra == "all"
 Requires-Dist: awscli (>=1.18,<2.0); extra == "awscli"
-Requires-Dist: databases[sqlite,postgresql,mysql]; extra == "all"
+Requires-Dist: databases[sqlite,mysql,postgresql]; extra == "all"
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: tinydb (>=3.15,<4.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Project-URL: Repository, https://github.com/dazza-codes/aio-aws.git
 Description-Content-Type: text/markdown
 
 [![Build Status](https://travis-ci.com/dazza-codes/aio-aws.svg?branch=master)](https://travis-ci.com/dazza-codes/aio-aws)
```

