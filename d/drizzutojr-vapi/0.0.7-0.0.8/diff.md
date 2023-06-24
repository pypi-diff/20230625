# Comparing `tmp/drizzutojr_vapi-0.0.7-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4294 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-24 22:54 vapi/__init__.py
--rw-r--r--  2.0 unx     1344 b- defN 23-Jun-24 22:54 vapi/exceptions.py
--rw-r--r--  2.0 unx     6979 b- defN 23-Jun-24 22:54 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      642 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/RECORD
-8 files, 10372 bytes uncompressed, 3168 bytes compressed:  69.5%
+Zip file size: 4295 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-24 23:36 vapi/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jun-24 23:36 vapi/exceptions.py
+-rw-r--r--  2.0 unx     6969 b- defN 23-Jun-24 23:36 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-24 23:38 drizzutojr_vapi-0.0.8.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-24 23:38 drizzutojr_vapi-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 23:38 drizzutojr_vapi-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-24 23:38 drizzutojr_vapi-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-24 23:38 drizzutojr_vapi-0.0.8.dist-info/RECORD
+8 files, 10362 bytes uncompressed, 3169 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.7.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.8.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.7.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.7.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.7.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.7.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/vapi.py

```diff
@@ -93,17 +93,17 @@
         url = f"{self.addr.rstrip('/')}/{url}"
         return url
 
     def _format_response(self, response, accepted_status_codes):
         if response.status_code in accepted_status_codes:
             try:
                 json_response = response.json()
-                if "wrap_info" in json_response.keys():
+                if json_response.get("wrap_info"):
                     return json_response["wrap_info"]
-                elif "data" in json_response.keys():
+                elif json_response.get("data"):
                     return json_response["data"]
                 else:
                     return json_response
             except ValueError:
                 return {}
         else:
             if response.status_code == 403:
```

## Comparing `drizzutojr_vapi-0.0.7.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.8.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `drizzutojr_vapi-0.0.7.dist-info/RECORD` & `drizzutojr_vapi-0.0.8.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 vapi/__init__.py,sha256=1X3SDUjKbFmf8wgwfVDgHy1HiwSUqn3iFwLekAIJwME,49
 vapi/exceptions.py,sha256=v0czLkP4PxdlGbaTvVeT01OU_7YAewW0kw9rbMXcl6A,1344
-vapi/vapi.py,sha256=XsQ3WLKYZk5mbRQB8e1bADh-piTtBpU6znJd_jpOmeA,6979
-drizzutojr_vapi-0.0.7.dist-info/LICENSE.md,sha256=S1pJL407BwTTXzZK0BQPNM7ZZs57uj1pTSfVZ8Whx30,1061
-drizzutojr_vapi-0.0.7.dist-info/METADATA,sha256=DfviTJwDc-coNyHuC-RypoPazfS3kAr8Y7pAbFLZM4U,200
-drizzutojr_vapi-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-drizzutojr_vapi-0.0.7.dist-info/top_level.txt,sha256=WtIjxGq4gkdnp4MLZf6yEo-HMdTp5sRLDYmbTyoPhyE,5
-drizzutojr_vapi-0.0.7.dist-info/RECORD,,
+vapi/vapi.py,sha256=WmGSQVCo4wpIPIgkQXyJ7nkGN1cJ7i-jZDTOEE42pVQ,6969
+drizzutojr_vapi-0.0.8.dist-info/LICENSE.md,sha256=S1pJL407BwTTXzZK0BQPNM7ZZs57uj1pTSfVZ8Whx30,1061
+drizzutojr_vapi-0.0.8.dist-info/METADATA,sha256=ZwDW8x6Y2A4Jp45ZhbBgRrf_y_JLviY9dwxzYJjU3RY,200
+drizzutojr_vapi-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+drizzutojr_vapi-0.0.8.dist-info/top_level.txt,sha256=WtIjxGq4gkdnp4MLZf6yEo-HMdTp5sRLDYmbTyoPhyE,5
+drizzutojr_vapi-0.0.8.dist-info/RECORD,,
```

