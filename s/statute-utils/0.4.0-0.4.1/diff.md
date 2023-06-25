# Comparing `tmp/statute_utils-0.4.0.tar.gz` & `tmp/statute_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statute_utils-0.4.0.tar", max compression
+gzip compressed data, was "statute_utils-0.4.1.tar", max compression
```

## Comparing `statute_utils-0.4.0.tar` & `statute_utils-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.0/LICENSE
--rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.0/README.md
--rw-r--r--   0        0        0     1449 2023-06-23 10:42:11.417437 statute_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      368 2023-06-22 07:34:05.597276 statute_utils-0.4.0/statute_utils/__init__.py
--rw-r--r--   0        0        0      319 2023-06-22 05:28:27.921068 statute_utils-0.4.0/statute_utils/components/__init__.py
--rw-r--r--   0        0        0     9198 2023-06-23 10:40:49.094740 statute_utils-0.4.0/statute_utils/components/category.py
--rw-r--r--   0        0        0     3517 2023-06-22 07:34:05.598060 statute_utils-0.4.0/statute_utils/components/details.py
--rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.0/statute_utils/components/rule.py
--rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.0/statute_utils/components/short.py
--rw-r--r--   0        0        0     3326 2023-06-22 06:12:44.626570 statute_utils-0.4.0/statute_utils/components/utils.py
--rw-r--r--   0        0        0     4192 2023-06-23 10:44:32.008135 statute_utils-0.4.0/statute_utils/main.py
--rw-r--r--   0        0        0     5170 2023-06-23 10:41:31.532335 statute_utils-0.4.0/statute_utils/models.py
--rw-r--r--   0        0        0     4434 2023-06-22 06:12:44.627800 statute_utils-0.4.0/statute_utils/names.py
--rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.0/statute_utils/recipes/__init__.py
--rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.0/statute_utils/recipes/const.py
--rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.0/statute_utils/recipes/digits.py
--rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.0/statute_utils/recipes/roc.py
--rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.0/statute_utils/recipes/spain.py
--rw-r--r--   0        0        0     6618 2023-06-22 06:11:13.995177 statute_utils-0.4.0/statute_utils/serials.py
--rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-21 15:08:07.621911 statute_utils-0.4.1/LICENSE
+-rw-r--r--   0        0        0      898 2023-06-21 15:08:07.622003 statute_utils-0.4.1/README.md
+-rw-r--r--   0        0        0     1449 2023-06-24 07:19:59.600641 statute_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      358 2023-06-24 05:47:47.855210 statute_utils-0.4.1/statute_utils/__init__.py
+-rw-r--r--   0        0        0     4189 2023-06-24 05:47:52.231137 statute_utils-0.4.1/statute_utils/main.py
+-rw-r--r--   0        0        0     5167 2023-06-24 05:47:54.905008 statute_utils-0.4.1/statute_utils/models.py
+-rw-r--r--   0        0        0     4431 2023-06-24 05:47:56.695048 statute_utils-0.4.1/statute_utils/names.py
+-rw-r--r--   0        0        0      249 2023-06-22 05:28:27.922206 statute_utils-0.4.1/statute_utils/recipes/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-22 05:28:27.922298 statute_utils-0.4.1/statute_utils/recipes/const.py
+-rw-r--r--   0        0        0     2649 2023-06-22 05:28:27.922412 statute_utils-0.4.1/statute_utils/recipes/digits.py
+-rw-r--r--   0        0        0      311 2023-06-22 05:28:27.922524 statute_utils-0.4.1/statute_utils/recipes/roc.py
+-rw-r--r--   0        0        0      667 2023-06-22 05:28:27.922641 statute_utils-0.4.1/statute_utils/recipes/spain.py
+-rw-r--r--   0        0        0     6615 2023-06-24 05:47:58.345784 statute_utils-0.4.1/statute_utils/serials.py
+-rw-r--r--   0        0        0      327 2023-06-24 05:48:44.544520 statute_utils-0.4.1/statute_utils/statute/__init__.py
+-rw-r--r--   0        0        0     9198 2023-06-24 05:48:08.172327 statute_utils-0.4.1/statute_utils/statute/category.py
+-rw-r--r--   0        0        0     4423 2023-06-25 01:07:27.204571 statute_utils-0.4.1/statute_utils/statute/main.py
+-rw-r--r--   0        0        0     4679 2023-06-23 10:46:22.018647 statute_utils-0.4.1/statute_utils/statute/rule.py
+-rw-r--r--   0        0        0     2015 2023-06-22 05:28:27.921653 statute_utils-0.4.1/statute_utils/statute/short.py
+-rw-r--r--   0        0        0     4667 2023-06-24 03:15:09.551113 statute_utils-0.4.1/statute_utils/statute/utils.py
+-rw-r--r--   0        0        0     1734 1970-01-01 00:00:00.000000 statute_utils-0.4.1/PKG-INFO
```

### Comparing `statute_utils-0.4.0/LICENSE` & `statute_utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/README.md` & `statute_utils-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/pyproject.toml` & `statute_utils-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "statute-utils"
-version = "0.4.0"
+version = "0.4.1"
 description = "Philippine statutory law pattern matching and unit retrieval."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/statute-utils"
 documentation = "https://justmars.github.io/statute-utils"
 classifiers = [
```

### Comparing `statute_utils-0.4.0/statute_utils/components/category.py` & `statute_utils-0.4.1/statute_utils/statute/category.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/statute_utils/components/details.py` & `statute_utils-0.4.1/statute_utils/statute/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import datetime
 from pathlib import Path
 
 import yaml
 from dateutil.parser import parse
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 from .category import StatuteSerialCategory, StatuteTitle
 from .rule import Rule
-from .utils import walk
+from .utils import set_node_ids, walk
 
 STATUTE_DIR = Path().home().joinpath("code/corpus-statutes")
 
 
-class StatuteDetails(BaseModel):
+class Statute(BaseModel):
     """A instance is dependent on a statute path from a fixed
     `STATUTE_DIR`. The shape of the Python object will be different
     from the shape of the dumpable `.yml` export."""
 
-    titles: list[StatuteTitle]
-    rule: Rule
-    variant: int
-    date: datetime.date
-    units: list[dict]
+    titles: list[StatuteTitle] = Field(...)
+    rule: Rule = Field(...)
+    variant: int = Field(...)
+    date: datetime.date = Field(...)
+    units: list[dict] = Field(...)
 
     def __str__(self) -> str:
         return f"{self.rule.__str__()}, {self.date.strftime('%b %d, %Y')}"
 
     def __repr__(self) -> str:
         return "/".join(
             [
@@ -34,27 +34,50 @@
                 self.date.isoformat(),
                 f"{str(self.variant)}.yml",
             ]
         )
 
     @property
     def slug(self):
-        return self.__repr__().removesuffix(".yml").replace("/", ".")
+        return self.__repr__().removesuffix(".yml").replace("/", "-")
+
+    def make_title_rows(self):
+        for counter, title in enumerate(self.titles, start=1):
+            row = {"id": f"{self.slug}-{counter}", "statute_id": self.slug}
+            yield row | {"cat": title.category.name.lower(), "text": title.text}
+
+    def make_row(self):
+        """All nodes in the tree are marked by a material path.
+
+        The units key is manipulated to add a root node. This is
+        useful for repeals and other changes since affecting the root node, affects all nodes.
+
+        The root node for every key should be `1.`
+        """  # noqa: E501
+        set_node_ids(self.units)
+        return {
+            "id": self.slug,
+            "cat": self.rule.cat.value,
+            "num": self.rule.id,
+            "date": self.date,
+            "variant": self.variant,
+            "units": [{"id": "1.", "units": self.units}],
+        }
 
     def to_file(self):
         f = STATUTE_DIR.joinpath(self.__repr__())
         f.parent.mkdir(parents=True, exist_ok=True)
         data = self.model_dump()
         data["units"] = walk(data["units"])
         text = yaml.dump(data, width=60)
         return f.write_text(text)
 
     @classmethod
     def from_file(cls, file: Path):
-        """Assumes the following path routing structure: `cat` / `num` / `date` / `variant`.yml,
+        """Assumes strict path routing structure: `cat` / `num` / `date` / `variant`.yml,
         e.g. `ra/386/1946-06-18/1.yml` where each file contains the following metadata, the
         mandatory ones being "title" and "units". See example:
 
         ```yaml
         title: An Act to Ordain and Institute the Civil Code of the Philippines
         aliases:
         - New Civil Code
@@ -75,33 +98,33 @@
                   content: >-
                     Laws shall take effect after fifteen days following the
                     completion of their publication either in the Official
                     Gazette or in a newspaper of general circulation in the
                     Philippines, unless it is otherwise provided. (1a)
         ```
         """  # noqa: E501
-        statute_path = file.parent.parent
+        cat, num, date, variant = file.parts[-4:]
 
         data = yaml.safe_load(file.read_bytes())
         official = data.get("title")
         if not official:
             return None
 
-        category = StatuteSerialCategory(statute_path.parent.stem)
+        category = StatuteSerialCategory(cat)
         if not category:
             return None
 
-        serial = category.serialize(statute_path.stem)
+        serial = category.serialize(num)
         if not serial:
             return None
 
         return cls(
-            rule=Rule(cat=category, id=statute_path.stem),
-            variant=int(file.stem),
-            date=parse(file.parent.stem).date(),
+            rule=Rule(cat=category, id=num),
+            variant=int(variant.removesuffix(".yml")),
+            date=parse(date).date(),
             units=data.get("units"),
             titles=list(
                 StatuteTitle.generate(
                     official=official,
                     serial=serial,
                     short=data.get("short"),
                     aliases=data.get("aliases"),
```

### Comparing `statute_utils-0.4.0/statute_utils/components/rule.py` & `statute_utils-0.4.1/statute_utils/statute/rule.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/statute_utils/components/short.py` & `statute_utils-0.4.1/statute_utils/statute/short.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/statute_utils/main.py` & `statute_utils-0.4.1/statute_utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import Counter
 from collections.abc import Iterator
 from typing import Self
 
 from pydantic import Field
 
-from .components import Rule, StatuteSerialCategory
 from .names import NamedRules
 from .serials import SerializedRules
+from .statute import Rule, StatuteSerialCategory
 
 
 def extract_rules(text: str) -> Iterator[Rule]:
     """If text contains [serialized][serial-pattern] (e.g. _Republic Act No. 386_)
     and [named][named-pattern] rules (_the Civil Code of the Philippines_),
     extract the [`Rules`][rule-model] into their canonical serial variants.
```

### Comparing `statute_utils-0.4.0/statute_utils/models.py` & `statute_utils-0.4.1/statute_utils/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from collections.abc import Iterator
 from re import Pattern
 
 from pydantic import Field
 
-from .components import BaseCollection, BasePattern, Rule, StatuteSerialCategory, stx
 from .recipes import split_digits
+from .statute import BaseCollection, BasePattern, Rule, StatuteSerialCategory, stx
 
 
 class NamedPattern(BasePattern):
     """A [`Rule`][rule-model] can be extracted from a `NamedPattern`"""
 
     name: str
     regex_base: str
```

### Comparing `statute_utils-0.4.0/statute_utils/names.py` & `statute_utils-0.4.1/statute_utils/names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from .components import Rule, StatuteSerialCategory
 from .models import NamedPattern, NamedPatternCollection
 from .recipes import CONST, ROC, SP_CIVIL, SP_COMMERCE, SP_PENAL
+from .statute import Rule, StatuteSerialCategory
 
 
 def make_spanish(name: str, regex: str):
     return NamedPattern(
         name=f"Old {name.title()} Code",
         regex_base=regex,
         rule=Rule(cat=StatuteSerialCategory.Spain, id=name),
```

### Comparing `statute_utils-0.4.0/statute_utils/recipes/digits.py` & `statute_utils-0.4.1/statute_utils/recipes/digits.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/statute_utils/recipes/spain.py` & `statute_utils-0.4.1/statute_utils/recipes/spain.py`

 * *Files identical despite different names*

### Comparing `statute_utils-0.4.0/statute_utils/serials.py` & `statute_utils-0.4.1/statute_utils/serials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from .components import (
-    StatuteSerialCategory,
-    add_blg,
-    add_num,
-    limited_acts,
-    ltr,
-)
 from .models import SerialPattern, SerialPatternCollection
 from .recipes import (
     ACT_DIGITS,
     BP_DIGITS,
     CA_DIGITS,
     PD_DIGITS_PLUS,
     RA_DIGITS,
     digitize,
 )
+from .statute import (
+    StatuteSerialCategory,
+    add_blg,
+    add_num,
+    limited_acts,
+    ltr,
+)
 
 """MODERN"""
 
 ra = SerialPattern(
     cat=StatuteSerialCategory.RepublicAct,
     regex_bases=[
         add_num(ltr("R", "A")),
```

### Comparing `statute_utils-0.4.0/PKG-INFO` & `statute_utils-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statute-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Philippine statutory law pattern matching and unit retrieval.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

