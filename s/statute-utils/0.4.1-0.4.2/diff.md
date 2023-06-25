# Comparing `tmp/statute_utils-0.4.1.tar.gz` & `tmp/statute_utils-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.4.1.tar", max compression
+gzip compressed data, was "statute_utils-0.4.2.tar", max compression
```

## Comparing `statute_utils-0.4.1.tar` & `statute_utils-0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.1/LICENSE
--rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.1/README.md
--rw-r--r--   0        0        0     1449 2023-06-24 07:19:59.600641 statute_utils-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      358 2023-06-24 05:47:47.855210 statute_utils-0.4.1/statute_utils/__init__.py
--rw-r--r--   0        0        0     4189 2023-06-24 05:47:52.231137 statute_utils-0.4.1/statute_utils/main.py
--rw-r--r--   0        0        0     5167 2023-06-24 05:47:54.905008 statute_utils-0.4.1/statute_utils/models.py
--rw-r--r--   0        0        0     4431 2023-06-24 05:47:56.695048 statute_utils-0.4.1/statute_utils/names.py
--rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.1/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.1/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.1/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.1/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.1/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6615 2023-06-24 05:47:58.345784 statute_utils-0.4.1/statute_utils/serials.py
--rw-r--r--   0        0        0      327 2023-06-24 05:48:44.544520 statute_utils-0.4.1/statute_utils/statute/__init__.py
--rw-r--r--   0        0        0     9198 2023-06-24 05:48:08.172327 statute_utils-0.4.1/statute_utils/statute/category.py
--rw-r--r--   0        0        0     4423 2023-06-25 01:07:27.204571 statute_utils-0.4.1/statute_utils/statute/main.py
--rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.1/statute_utils/statute/rule.py
--rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.1/statute_utils/statute/short.py
--rw-r--r--   0        0        0     4667 2023-06-24 03:15:09.551113 statute_utils-0.4.1/statute_utils/statute/utils.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.2/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.2/README.md
+-rw-r--r--   0        0        0     1449 2023-06-25 10:37:56.128314 statute_utils-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      361 2023-06-25 10:37:32.201516 statute_utils-0.4.2/statute_utils/__init__.py
+-rw-r--r--   0        0        0     4210 2023-06-25 10:37:43.462905 statute_utils-0.4.2/statute_utils/main.py
+-rw-r--r--   0        0        0     5167 2023-06-24 05:47:54.905008 statute_utils-0.4.2/statute_utils/models.py
+-rw-r--r--   0        0        0     4431 2023-06-24 05:47:56.695048 statute_utils-0.4.2/statute_utils/names.py
+-rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.2/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.2/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.2/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.2/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.2/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6615 2023-06-24 05:47:58.345784 statute_utils-0.4.2/statute_utils/serials.py
+-rw-r--r--   0        0        0      327 2023-06-24 05:48:44.544520 statute_utils-0.4.2/statute_utils/statute/__init__.py
+-rw-r--r--   0        0        0     9198 2023-06-24 05:48:08.172327 statute_utils-0.4.2/statute_utils/statute/category.py
+-rw-r--r--   0        0        0     4423 2023-06-25 01:07:27.204571 statute_utils-0.4.2/statute_utils/statute/main.py
+-rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.2/statute_utils/statute/rule.py
+-rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.2/statute_utils/statute/short.py
+-rw-r--r--   0        0        0     4667 2023-06-24 03:15:09.551113 statute_utils-0.4.2/statute_utils/statute/utils.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.2/PKG-INFO
```

### Comparing `statute_utils-0.4.1/LICENSE` & `statute_utils-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/README.md` & `statute_utils-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/pyproject.toml` & `statute_utils-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.4.1"
+version = "0.4.2"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.4.1/statute_utils/main.py` & `statute_utils-0.4.2/statute_utils/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,35 +46,35 @@
     """  # noqa: E501
     try:
         return next(extract_rules(text))
     except StopIteration:
         return None
 
 
-class CountedRule(Rule):
+class CountedStatute(Rule):
     """Based on results from [`extract_rules()`][extract-rules], get count of each
     unique rule found."""
 
     mentions: int = Field(...)
 
     def __repr__(self) -> str:
         return f"{self.cat} {self.id}: {self.mentions}"
 
     @classmethod
     def from_source(cls, text: str) -> Iterator[Self]:
         """Detect counted rules from source `text`.
 
         Examples:
             >>> text = "The Civil Code of the Philippines, the old Spanish Civil Code; Rep Act No. 386"
-            >>> results = list(CountedRule.from_source(text))
+            >>> results = list(CountedStatute.from_source(text))
             >>> results
             [ra 386: 2, spain civil: 1]
-            >>> results[0] == CountedRule(cat=StatuteSerialCategory('ra'),id='386', mentions=2)
+            >>> results[0] == CountedStatute(cat=StatuteSerialCategory('ra'),id='386', mentions=2)
             True
-            >>> results[1] == CountedRule(cat=StatuteSerialCategory('spain'),id='civil', mentions=1)
+            >>> results[1] == CountedStatute(cat=StatuteSerialCategory('spain'),id='civil', mentions=1)
             True
 
         Args:
             text (str): Legalese containing statutory rules in various formats.
 
         Yields:
             Iterator[Self]: Each counted rule found.
@@ -85,15 +85,15 @@
 
     @classmethod
     def from_repr_format(cls, repr_texts: list[str]) -> Iterator[Self]:
         """Generate their pydantic counterparts from `<cat> <id>: <mentions>` format.
 
         Examples:
             >>> repr_texts = ['ra 386: 2', 'spain civil: 1']
-            >>> results = list(CountedRule.from_repr_format(repr_texts))
+            >>> results = list(CountedStatute.from_repr_format(repr_texts))
             >>> results
             [ra 386: 2, spain civil: 1]
             >>> results[0].cat
             'ra'
             >>> results[0].id
             '386'
             >>> results[0].mentions
@@ -101,18 +101,18 @@
             >>> str(results[0])
             'Republic Act No. 386'
             >>> repr(results[0])
             'ra 386: 2'
 
 
         Args:
-            repr_texts (str): list of texts having `__repr__` format of a `CountedRule`
+            repr_texts (str): list of texts having `__repr__` format of a `CountedStatute`
 
         Yields:
-            Iterator[Self]: Instances of CountedRule
+            Iterator[Self]: Instances of CountedStatute
         """
         for text in repr_texts:
             counted_bits = text.split(":")
             if len(counted_bits) == 2:
                 statute_bits = counted_bits[0].split()
                 mentions = counted_bits[1]
                 is_cat_id = len(statute_bits) == 2
```

### Comparing `statute_utils-0.4.1/statute_utils/models.py` & `statute_utils-0.4.2/statute_utils/models.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/names.py` & `statute_utils-0.4.2/statute_utils/names.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/recipes/digits.py` & `statute_utils-0.4.2/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/recipes/spain.py` & `statute_utils-0.4.2/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/serials.py` & `statute_utils-0.4.2/statute_utils/serials.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/statute/category.py` & `statute_utils-0.4.2/statute_utils/statute/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/statute/main.py` & `statute_utils-0.4.2/statute_utils/statute/main.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/statute/rule.py` & `statute_utils-0.4.2/statute_utils/statute/rule.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/statute/short.py` & `statute_utils-0.4.2/statute_utils/statute/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/statute_utils/statute/utils.py` & `statute_utils-0.4.2/statute_utils/statute/utils.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.1/PKG-INFO` & `statute_utils-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.4.1
+Version: 0.4.2
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

