# Comparing `tmp/python_camelcaser-1.0.0-py3-none-any.whl.zip` & `tmp/python_camelcaser-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1089551 bytes, number of entries: 6
--rw-rw-r--  2.0 unx     3716 b- defN 23-Jun-23 10:08 camelcaser/__init__.py
+Zip file size: 1089570 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     3755 b- defN 23-Jun-25 11:30 camelcaser/__init__.py
 -rw-rw-r--  2.0 unx  3864812 b- defN 23-Jun-22 19:06 camelcaser/word_lists/alpha_words.txt
--rw-rw-r--  2.0 unx     6172 b- defN 23-Jun-23 11:06 python_camelcaser-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-23 11:06 python_camelcaser-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Jun-23 11:06 python_camelcaser-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      514 b- defN 23-Jun-23 11:06 python_camelcaser-1.0.0.dist-info/RECORD
-6 files, 3875317 bytes uncompressed, 1088619 bytes compressed:  71.9%
+-rw-rw-r--  2.0 unx     6282 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      514 b- defN 23-Jun-25 11:31 python_camelcaser-1.0.1.dist-info/RECORD
+6 files, 3875466 bytes uncompressed, 1088638 bytes compressed:  71.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: camelcaser/__init__.py
 Comment: 
 
 Filename: camelcaser/word_lists/alpha_words.txt
 Comment: 
 
-Filename: python_camelcaser-1.0.0.dist-info/METADATA
+Filename: python_camelcaser-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: python_camelcaser-1.0.0.dist-info/WHEEL
+Filename: python_camelcaser-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: python_camelcaser-1.0.0.dist-info/top_level.txt
+Filename: python_camelcaser-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: python_camelcaser-1.0.0.dist-info/RECORD
+Filename: python_camelcaser-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## camelcaser/__init__.py

```diff
@@ -30,24 +30,26 @@
 
 def detect_real_words(word_list):
     english_dict = enchant.Dict("en_US")
     real_words = [word for word in word_list if english_dict.check(word)]
     return real_words
 
 
-def has_seperator(string):
+def has_separator(string):
     pattern = r'[A-Z_-]'
     matches = re.findall(pattern, string)
     if matches:
         sorted_matches = sorted(matches, key=lambda x: (not x.isalpha(), x))
         return sorted_matches[0] if sorted_matches else False
     return False
 
 
 def split_camel_case(string):
+    if not string[0].isupper():
+        string = string[0].upper() + string[1:]
     return re.findall('[A-Z][a-z]*', string)
 
 
 def format_string(words_list, mode):
     if mode == "camel_case":
         camel_case = ''.join(word.capitalize() for word in words_list)
         return camel_case
@@ -76,19 +78,18 @@
         raise Exception("Unknown mode.")
 
 
 
 
 def make_notation(string, max_iteration=30, mode="camel_case", separator=None):
     if not separator:
-        separator = has_seperator(string)
+        separator = has_separator(string)
 
     if separator:
         if separator.isalpha():
-            string = string.capitalize()
             words = split_camel_case(string)
         else:
             words = string.split(separator)
         return format_string(words, mode.lower())
 
 
     string = normalize_string(string)
```

## Comparing `python_camelcaser-1.0.0.dist-info/METADATA` & `python_camelcaser-1.0.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: python-camelcaser
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert strings to camel, snake and kebab case - even if separation is unknown.
 Home-page: https://github.com/benschaedlich/python-camelcaser
 Author: Benjamin Schaedlich
-Author-email: dev@benjamin-schaedlich.de
 License: UNKNOWN
+Project-URL: Documentation, https://github.com/benschaedlich/python-camelcaser
+Project-URL: Source, https://github.com/benschaedlich/python-camelcaser
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pyenchant (==3.2.2)
```

## Comparing `python_camelcaser-1.0.0.dist-info/RECORD` & `python_camelcaser-1.0.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-camelcaser/__init__.py,sha256=hQh4qIIZrqJog2Mdl94TYcWm8HToeKjlNenBoG3SsSo,3716
+camelcaser/__init__.py,sha256=PcN8Kqyiuy52I8OMXEKHBgoikhIC5piRmKElZ2foL44,3755
 camelcaser/word_lists/alpha_words.txt,sha256=SAqRRXyy4uESJvDzfZHov84tnAKCXgKguNLeKnCkW8w,3864812
-python_camelcaser-1.0.0.dist-info/METADATA,sha256=EwUABZ6p00-Bbd-de67GHT2zh0U8Vn-p4nb9c2_eBZw,6172
-python_camelcaser-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-python_camelcaser-1.0.0.dist-info/top_level.txt,sha256=lSgJkvGKa60VJ98a9FD09FG7lgVY9BOtn18S8gNwG0U,11
-python_camelcaser-1.0.0.dist-info/RECORD,,
+python_camelcaser-1.0.1.dist-info/METADATA,sha256=-YhqnK3Dpo3Dt-yyCMqyVi8nAXP0YS_UfKfbPLi31xI,6282
+python_camelcaser-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+python_camelcaser-1.0.1.dist-info/top_level.txt,sha256=lSgJkvGKa60VJ98a9FD09FG7lgVY9BOtn18S8gNwG0U,11
+python_camelcaser-1.0.1.dist-info/RECORD,,
```

