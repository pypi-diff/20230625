# Comparing `tmp/dashscope-1.3.0-py3-none-any.whl.zip` & `tmp/dashscope-1.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 56147 bytes, number of entries: 47
+Zip file size: 56152 bytes, number of entries: 47
 -rw-r--r--  2.0 unx     1131 b- defN 23-Jun-20 06:30 dashscope/__init__.py
 -rw-r--r--  2.0 unx    13474 b- defN 23-May-16 06:21 dashscope/cli.py
 -rw-r--r--  2.0 unx     3445 b- defN 23-Mar-30 08:43 dashscope/deployment.py
 -rw-r--r--  2.0 unx     3753 b- defN 23-Mar-30 08:43 dashscope/file.py
 -rw-r--r--  2.0 unx     4808 b- defN 23-Mar-30 08:43 dashscope/finetune.py
 -rw-r--r--  2.0 unx     1696 b- defN 23-Mar-30 08:43 dashscope/model.py
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-20 10:39 dashscope/version.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-25 08:03 dashscope/version.py
 -rw-r--r--  2.0 unx      239 b- defN 23-May-16 06:21 dashscope/aigc/__init__.py
 -rw-r--r--  2.0 unx     8844 b- defN 23-May-17 12:24 dashscope/aigc/conversation.py
--rw-r--r--  2.0 unx     5064 b- defN 23-May-17 12:24 dashscope/aigc/generation.py
+-rw-r--r--  2.0 unx     5084 b- defN 23-Jun-25 08:03 dashscope/aigc/generation.py
 -rw-r--r--  2.0 unx     7669 b- defN 23-May-16 06:21 dashscope/aigc/image_synthesis.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/api_entities/__init__.py
 -rw-r--r--  2.0 unx    10361 b- defN 23-Apr-06 08:21 dashscope/api_entities/aiohttp_request.py
 -rw-r--r--  2.0 unx     5331 b- defN 23-May-30 06:21 dashscope/api_entities/api_request_data.py
 -rw-r--r--  2.0 unx     4057 b- defN 23-Apr-06 03:24 dashscope/api_entities/api_request_factory.py
 -rw-r--r--  2.0 unx      928 b- defN 23-May-24 01:18 dashscope/api_entities/base_request.py
 -rw-r--r--  2.0 unx     9654 b- defN 23-Jun-20 06:30 dashscope/api_entities/dashscope_response.py
@@ -36,14 +36,14 @@
 -rw-r--r--  2.0 unx     4038 b- defN 23-May-16 06:21 dashscope/common/utils.py
 -rw-r--r--  2.0 unx       69 b- defN 23-May-30 06:21 dashscope/embeddings/__init__.py
 -rw-r--r--  2.0 unx     1666 b- defN 23-May-30 06:21 dashscope/embeddings/text_embedding.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/io/__init__.py
 -rw-r--r--  2.0 unx     3941 b- defN 23-May-30 06:21 dashscope/io/input_output.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-23 09:23 dashscope/protocol/__init__.py
 -rw-r--r--  2.0 unx      561 b- defN 23-Mar-23 09:23 dashscope/protocol/websocket.py
--rw-r--r--  2.0 unx    11413 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7201 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     4049 b- defN 23-Jun-20 10:39 dashscope-1.3.0.dist-info/RECORD
-47 files, 200904 bytes uncompressed, 49645 bytes compressed:  75.3%
+-rw-r--r--  2.0 unx    11413 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7201 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     4049 b- defN 23-Jun-25 08:03 dashscope-1.3.1.dist-info/RECORD
+47 files, 200924 bytes uncompressed, 49650 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -117,26 +117,26 @@
 
 Filename: dashscope/protocol/__init__.py
 Comment: 
 
 Filename: dashscope/protocol/websocket.py
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/LICENSE
+Filename: dashscope-1.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/METADATA
+Filename: dashscope-1.3.1.dist-info/METADATA
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/WHEEL
+Filename: dashscope-1.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/entry_points.txt
+Filename: dashscope-1.3.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/top_level.txt
+Filename: dashscope-1.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: dashscope-1.3.0.dist-info/RECORD
+Filename: dashscope-1.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dashscope/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.3.0'
+__version__ = '1.3.1'
```

## dashscope/aigc/generation.py

```diff
@@ -89,16 +89,17 @@
             return GenerationResponse.from_api_response(response)
 
     @classmethod
     def _build_input_parameters(cls, model, prompt, history, **kwargs):
         parameters = {}
         input = {
             PROMPT: prompt,
-            HISTORY: history if history else [],
         }
+        if history is not None:
+            input[HISTORY] = history
         if model.startswith('qwen'):
             enable_search = kwargs.pop('enable_search', False)
             QWEN_NUM_WEB_SEARCH = 0
             if enable_search:
                 QWEN_NUM_WEB_SEARCH = 5
             parameters['QWEN_NUM_WEB_SEARCH'] = QWEN_NUM_WEB_SEARCH
             parameters['QWEN_SEARCH_IN_FIRST_QUERY'] = 0
```

## Comparing `dashscope-1.3.0.dist-info/LICENSE` & `dashscope-1.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dashscope-1.3.0.dist-info/METADATA` & `dashscope-1.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dashscope
-Version: 1.3.0
+Version: 1.3.1
 Summary: dashscope client sdk library
 Home-page: https://dashscope.aliyun.com/
 Author: Alibaba
 Author-email: dashscope@alibaba-inc.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

## Comparing `dashscope-1.3.0.dist-info/RECORD` & `dashscope-1.3.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 dashscope/__init__.py,sha256=OIQFNWbRNTCTCTZZaTR0dw1sR20Bvsrh5krvV_v7B-I,1131
 dashscope/cli.py,sha256=FHz1UGh8dCDBV25FQttJM1uxZT3rNKGDp_krfCel7rY,13474
 dashscope/deployment.py,sha256=OA7FMkFTXwKDTcLLZe57_ZlCk38S29krdijy-_W64G4,3445
 dashscope/file.py,sha256=maMrfMB5_WVltYEyGN4QcAH0Xxj0eHkScisP8AXx4RQ,3753
 dashscope/finetune.py,sha256=jUj43EmwtCDYNqMvjKimuCQigG0Ux2EvZBypGcmkqHg,4808
 dashscope/model.py,sha256=kLXawzbbq4VkFFFjruz06MkuY-uEMUWCqs-4quqV7Us,1696
-dashscope/version.py,sha256=zi_LaUT_OsChAtsPXbOeRpQkCohSsOyeXfavQPM0GoE,22
+dashscope/version.py,sha256=P2DFKJQEJRlJhF0IW0Lwt4G4uMYyJJ5ymhv-XrCcPGo,22
 dashscope/aigc/__init__.py,sha256=llQdhMk9N11SKlTSAvYK-E4xT46GcXUAF51I-oDDDMM,239
 dashscope/aigc/conversation.py,sha256=H46NzB7CvCNBVFeD61bG-IBxcdfe3hjenszvI4M0AeY,8844
-dashscope/aigc/generation.py,sha256=LwyYEu-aRZGbXBilaaYQqkk2MF7Ojc1kBl-UU8nOAbI,5064
+dashscope/aigc/generation.py,sha256=ZpiVcm8Vf5MGyBeQsfmDXiq-VwzCsPveHJWN0tPp1iA,5084
 dashscope/aigc/image_synthesis.py,sha256=zZhpny20azLinMhhvAgyLY4qHugtl1EEApJQ5vuHNZI,7669
 dashscope/api_entities/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/api_entities/aiohttp_request.py,sha256=LpUM-BGKTHUeBnZ6cOfmdlp4-7czWLkhdNSzS2ydOh0,10361
 dashscope/api_entities/api_request_data.py,sha256=THH0jHQazlmjGId0e8-4aJG5jH71_jMm-CulGCZ6DV4,5331
 dashscope/api_entities/api_request_factory.py,sha256=4COz8WMEJOBP2_7jkW62Rua21SpoyrthCOMT0yg_z_k,4057
 dashscope/api_entities/base_request.py,sha256=y1SmJQ2csMy43y3c66BrC_usfn93XmJyhyu3Ge5aRKI,928
 dashscope/api_entities/dashscope_response.py,sha256=slVvNjW-tu3Di6HNVV4FnZ3dMyS1HiL1CnWrELJS5rs,9654
@@ -35,13 +35,13 @@
 dashscope/common/utils.py,sha256=F5GOEMIzB2Sh1ohzx_nNgGKe752F92aQQpsaqFh-4nM,4038
 dashscope/embeddings/__init__.py,sha256=InVIZayFfGZq9Q13Mok6c_ocdV3PCFcbxjURBcLYMEg,69
 dashscope/embeddings/text_embedding.py,sha256=nI-d4zcuZA_tpfu7ktI5SZ8V-dGngVclZwxGFAh4qmE,1666
 dashscope/io/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/io/input_output.py,sha256=iZ1X1x1btdoZK2VeC9JsKkag2eaXwqfNT3Q6SrmRi2w,3941
 dashscope/protocol/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 dashscope/protocol/websocket.py,sha256=z-v6PGx3L4zYBANuC48s7SWSQSwRCDoh0zcfhv9Bf8U,561
-dashscope-1.3.0.dist-info/LICENSE,sha256=Izp5L1DF1Mbza6qojkqNNWlE_mYLnr4rmzx2EBF8YFw,11413
-dashscope-1.3.0.dist-info/METADATA,sha256=8HX7YB2f0qpcDbW5QhivJfOL5up9hQfpjtJRnBQjVKM,7201
-dashscope-1.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-dashscope-1.3.0.dist-info/entry_points.txt,sha256=raEp5dOuj8whJ7yqZlDM8WQ5p2RfnGrGNo0QLQEnatY,50
-dashscope-1.3.0.dist-info/top_level.txt,sha256=woqavFJK9zas5xTqynmALqOtlafghjsk63Xk86powTU,10
-dashscope-1.3.0.dist-info/RECORD,,
+dashscope-1.3.1.dist-info/LICENSE,sha256=Izp5L1DF1Mbza6qojkqNNWlE_mYLnr4rmzx2EBF8YFw,11413
+dashscope-1.3.1.dist-info/METADATA,sha256=SPOZfPLAaswQUKAhDQpsIgZW9IhHZEgd0Jc9eSATIlo,7201
+dashscope-1.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+dashscope-1.3.1.dist-info/entry_points.txt,sha256=raEp5dOuj8whJ7yqZlDM8WQ5p2RfnGrGNo0QLQEnatY,50
+dashscope-1.3.1.dist-info/top_level.txt,sha256=woqavFJK9zas5xTqynmALqOtlafghjsk63Xk86powTU,10
+dashscope-1.3.1.dist-info/RECORD,,
```

