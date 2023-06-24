# Comparing `tmp/drizzutojr_vapi-0.0.6-py3-none-any.whl.zip` & `tmp/drizzutojr_vapi-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4279 bytes, number of entries: 8
--rw-r--r--  2.0 unx       49 b- defN 23-Jun-24 21:03 vapi/__init__.py
--rw-r--r--  2.0 unx     1344 b- defN 23-Jun-24 21:03 vapi/exceptions.py
--rw-r--r--  2.0 unx     6867 b- defN 23-Jun-24 21:03 vapi/vapi.py
--rw-r--r--  2.0 unx     1061 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      200 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      642 b- defN 23-Jun-24 21:05 drizzutojr_vapi-0.0.6.dist-info/RECORD
-8 files, 10260 bytes uncompressed, 3153 bytes compressed:  69.3%
+Zip file size: 4294 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       49 b- defN 23-Jun-24 22:54 vapi/__init__.py
+-rw-r--r--  2.0 unx     1344 b- defN 23-Jun-24 22:54 vapi/exceptions.py
+-rw-r--r--  2.0 unx     6979 b- defN 23-Jun-24 22:54 vapi/vapi.py
+-rw-r--r--  2.0 unx     1061 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      200 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      642 b- defN 23-Jun-24 22:56 drizzutojr_vapi-0.0.7.dist-info/RECORD
+8 files, 10372 bytes uncompressed, 3168 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: vapi/exceptions.py
 Comment: 
 
 Filename: vapi/vapi.py
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.6.dist-info/LICENSE.md
+Filename: drizzutojr_vapi-0.0.7.dist-info/LICENSE.md
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.6.dist-info/METADATA
+Filename: drizzutojr_vapi-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.6.dist-info/WHEEL
+Filename: drizzutojr_vapi-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.6.dist-info/top_level.txt
+Filename: drizzutojr_vapi-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: drizzutojr_vapi-0.0.6.dist-info/RECORD
+Filename: drizzutojr_vapi-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vapi/vapi.py

```diff
@@ -93,15 +93,17 @@
         url = f"{self.addr.rstrip('/')}/{url}"
         return url
 
     def _format_response(self, response, accepted_status_codes):
         if response.status_code in accepted_status_codes:
             try:
                 json_response = response.json()
-                if "data" in json_response.keys():
+                if "wrap_info" in json_response.keys():
+                    return json_response["wrap_info"]
+                elif "data" in json_response.keys():
                     return json_response["data"]
                 else:
                     return json_response
             except ValueError:
                 return {}
         else:
             if response.status_code == 403:
```

## Comparing `drizzutojr_vapi-0.0.6.dist-info/LICENSE.md` & `drizzutojr_vapi-0.0.7.dist-info/LICENSE.md`

 * *Files identical despite different names*

