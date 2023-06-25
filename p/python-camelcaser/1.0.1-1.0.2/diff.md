# Comparing `tmp/python_camelcaser-1.0.1-py3-none-any.whl.zip` & `tmp/python_camelcaser-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1089570 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     3755 b- defN 23-Jun-25 11:30 camelcaser/__init__.py
+Zip file size: 1089575 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     3771 b- defN 23-Jun-25 12:06 camelcaser/__init__.py
 -rw-rw-r--  2.0 unx  3864812 b- defN 23-Jun-22 19:06 camelcaser/word_lists/alpha_words.txt
--rw-rw-r--  2.0 unx     6282 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      514 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/RECORD
-6 files, 3875466 bytes uncompressed, 1088638 bytes compressed:  71.9%
+-rw-rw-r--  2.0 unx     6282 b- defN 23-Jun-25 12:08 python_camelcaser-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-25 12:08 python_camelcaser-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-25 12:08 python_camelcaser-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      514 b- defN 23-Jun-25 12:08 python_camelcaser-1.0.2.dist-info/RECORD
+6 files, 3875482 bytes uncompressed, 1088643 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: camelcaser/__init__.py
 Comment: 
 
 Filename: camelcaser/word_lists/alpha_words.txt
 Comment: 
 
-Filename: python_camelcaser-1.0.1.dist-info/METADATA
+Filename: python_camelcaser-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: python_camelcaser-1.0.1.dist-info/WHEEL
+Filename: python_camelcaser-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: python_camelcaser-1.0.1.dist-info/top_level.txt
+Filename: python_camelcaser-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: python_camelcaser-1.0.1.dist-info/RECORD
+Filename: python_camelcaser-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## camelcaser/__init__.py

```diff
@@ -56,23 +56,23 @@
     
     elif (mode == "lower_camel_case"):
         camel_case = ''.join(word.capitalize() for word in words_list)
         return camel_case[0].lower() + camel_case[1:]
     
     elif (mode == "snake_case"):
         snake_case = '_'.join(word for word in words_list)
-        return snake_case
+        return snake_case.lower()
     
     elif (mode == "upper_snake_case"):
         snake_case = '_'.join(word.capitalize() for word in words_list)
         return snake_case
 
     elif (mode == "kebab_case"):
         kebab_case = '-'.join(word for word in words_list)
-        return kebab_case
+        return kebab_case.lower()
 
     elif (mode == "upper_kebab_case"):
         kebab_case = '-'.join(word.capitalize() for word in words_list)
         return kebab_case
 
     else:
         raise Exception("Unknown mode.")
```

## Comparing `python_camelcaser-1.0.1.dist-info/METADATA` & `python_camelcaser-1.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-camelcaser
-Version: 1.0.1
+Version: 1.0.2
 Summary: Convert strings to camel, snake and kebab case - even if separation is unknown.
 Home-page: https://github.com/benschaedlich/python-camelcaser
 Author: Benjamin Schaedlich
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/benschaedlich/python-camelcaser
 Project-URL: Source, https://github.com/benschaedlich/python-camelcaser
 Platform: UNKNOWN
```

