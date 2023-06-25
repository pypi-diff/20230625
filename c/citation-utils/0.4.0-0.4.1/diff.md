# Comparing `tmp/citation_utils-0.4.0.tar.gz` & `tmp/citation_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citation_utils-0.4.0.tar", max compression
+gzip compressed data, was "citation_utils-0.4.1.tar", max compression
```

## Comparing `citation_utils-0.4.0.tar` & `citation_utils-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.0/LICENSE
--rw-r--r--   0        0        0      653 2023-06-23 10:27:21.228547 citation_utils-0.4.0/citation_utils/__init__.py
--rw-r--r--   0        0        0    13224 2023-06-23 10:27:21.228689 citation_utils-0.4.0/citation_utils/citation.py
--rw-r--r--   0        0        0     1179 2023-06-23 10:27:21.228818 citation_utils-0.4.0/citation_utils/dockets/__init__.py
--rw-r--r--   0        0        0     3155 2023-06-23 10:27:21.228950 citation_utils-0.4.0/citation_utils/dockets/constructed_ac.py
--rw-r--r--   0        0        0     3194 2023-06-23 10:27:21.229021 citation_utils-0.4.0/citation_utils/dockets/constructed_am.py
--rw-r--r--   0        0        0     2457 2023-06-23 10:27:21.229092 citation_utils-0.4.0/citation_utils/dockets/constructed_bm.py
--rw-r--r--   0        0        0     2893 2023-06-23 10:27:21.229189 citation_utils-0.4.0/citation_utils/dockets/constructed_gr.py
--rw-r--r--   0        0        0     2094 2023-06-23 10:27:21.229296 citation_utils-0.4.0/citation_utils/dockets/constructed_jib.py
--rw-r--r--   0        0        0     2385 2023-06-23 10:27:21.229386 citation_utils-0.4.0/citation_utils/dockets/constructed_oca.py
--rw-r--r--   0        0        0     1597 2023-06-23 10:27:21.229484 citation_utils-0.4.0/citation_utils/dockets/constructed_pet.py
--rw-r--r--   0        0        0     1767 2023-06-23 10:27:21.229558 citation_utils-0.4.0/citation_utils/dockets/constructed_udk.py
--rw-r--r--   0        0        0      349 2023-06-23 10:27:21.229679 citation_utils-0.4.0/citation_utils/dockets/models/__init__.py
--rw-r--r--   0        0        0     4834 2023-06-23 10:27:21.229791 citation_utils-0.4.0/citation_utils/dockets/models/constructor.py
--rw-r--r--   0        0        0     1373 2023-06-23 10:27:21.229898 citation_utils-0.4.0/citation_utils/dockets/models/docket_category.py
--rw-r--r--   0        0        0     1696 2023-06-23 10:27:21.229985 citation_utils-0.4.0/citation_utils/dockets/models/docket_citation.py
--rw-r--r--   0        0        0     3375 2023-06-23 10:27:21.230105 citation_utils-0.4.0/citation_utils/dockets/models/docket_model.py
--rw-r--r--   0        0        0     1419 2023-06-23 10:27:21.230196 citation_utils-0.4.0/citation_utils/dockets/models/docket_rules.py
--rw-r--r--   0        0        0     2911 2023-06-23 10:27:21.230290 citation_utils-0.4.0/citation_utils/dockets/models/gr_clean.py
--rw-r--r--   0        0        0       81 2023-06-23 10:27:21.230427 citation_utils-0.4.0/citation_utils/dockets/models/misc/__init__.py
--rw-r--r--   0        0        0      746 2023-06-23 10:27:21.230521 citation_utils-0.4.0/citation_utils/dockets/models/misc/extra.py
--rw-r--r--   0        0        0     1514 2023-06-23 10:27:21.230609 citation_utils-0.4.0/citation_utils/dockets/models/misc/num.py
--rw-r--r--   0        0        0      242 2023-06-23 10:27:21.230693 citation_utils-0.4.0/citation_utils/dockets/models/misc/x.py
--rw-r--r--   0        0        0     5760 2023-06-23 10:27:21.230811 citation_utils-0.4.0/citation_utils/document.py
--rw-r--r--   0        0        0     2531 2023-06-23 10:27:21.231091 citation_utils-0.4.0/citation_utils/special.py
--rw-r--r--   0        0        0     1312 2023-06-23 10:29:13.617295 citation_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-23 10:27:21.228309 citation_utils-0.4.1/LICENSE
+-rw-r--r--   0        0        0      653 2023-06-23 10:27:21.228547 citation_utils-0.4.1/citation_utils/__init__.py
+-rw-r--r--   0        0        0    15416 2023-06-25 01:19:08.970634 citation_utils-0.4.1/citation_utils/citation.py
+-rw-r--r--   0        0        0     1179 2023-06-23 10:27:21.228818 citation_utils-0.4.1/citation_utils/dockets/__init__.py
+-rw-r--r--   0        0        0     3155 2023-06-23 10:27:21.228950 citation_utils-0.4.1/citation_utils/dockets/constructed_ac.py
+-rw-r--r--   0        0        0     3194 2023-06-23 10:27:21.229021 citation_utils-0.4.1/citation_utils/dockets/constructed_am.py
+-rw-r--r--   0        0        0     2457 2023-06-23 10:27:21.229092 citation_utils-0.4.1/citation_utils/dockets/constructed_bm.py
+-rw-r--r--   0        0        0     2893 2023-06-23 10:27:21.229189 citation_utils-0.4.1/citation_utils/dockets/constructed_gr.py
+-rw-r--r--   0        0        0     2094 2023-06-23 10:27:21.229296 citation_utils-0.4.1/citation_utils/dockets/constructed_jib.py
+-rw-r--r--   0        0        0     2385 2023-06-23 10:27:21.229386 citation_utils-0.4.1/citation_utils/dockets/constructed_oca.py
+-rw-r--r--   0        0        0     1597 2023-06-23 10:27:21.229484 citation_utils-0.4.1/citation_utils/dockets/constructed_pet.py
+-rw-r--r--   0        0        0     1767 2023-06-23 10:27:21.229558 citation_utils-0.4.1/citation_utils/dockets/constructed_udk.py
+-rw-r--r--   0        0        0      349 2023-06-23 10:27:21.229679 citation_utils-0.4.1/citation_utils/dockets/models/__init__.py
+-rw-r--r--   0        0        0     4834 2023-06-23 10:27:21.229791 citation_utils-0.4.1/citation_utils/dockets/models/constructor.py
+-rw-r--r--   0        0        0     1373 2023-06-23 10:27:21.229898 citation_utils-0.4.1/citation_utils/dockets/models/docket_category.py
+-rw-r--r--   0        0        0     1696 2023-06-23 10:27:21.229985 citation_utils-0.4.1/citation_utils/dockets/models/docket_citation.py
+-rw-r--r--   0        0        0     3564 2023-06-25 01:18:23.240029 citation_utils-0.4.1/citation_utils/dockets/models/docket_model.py
+-rw-r--r--   0        0        0     1419 2023-06-23 10:27:21.230196 citation_utils-0.4.1/citation_utils/dockets/models/docket_rules.py
+-rw-r--r--   0        0        0     2911 2023-06-23 10:27:21.230290 citation_utils-0.4.1/citation_utils/dockets/models/gr_clean.py
+-rw-r--r--   0        0        0       81 2023-06-23 10:27:21.230427 citation_utils-0.4.1/citation_utils/dockets/models/misc/__init__.py
+-rw-r--r--   0        0        0      746 2023-06-23 10:27:21.230521 citation_utils-0.4.1/citation_utils/dockets/models/misc/extra.py
+-rw-r--r--   0        0        0     1514 2023-06-23 10:27:21.230609 citation_utils-0.4.1/citation_utils/dockets/models/misc/num.py
+-rw-r--r--   0        0        0      242 2023-06-23 10:27:21.230693 citation_utils-0.4.1/citation_utils/dockets/models/misc/x.py
+-rw-r--r--   0        0        0     5760 2023-06-23 10:27:21.230811 citation_utils-0.4.1/citation_utils/document.py
+-rw-r--r--   0        0        0     2531 2023-06-23 10:27:21.231091 citation_utils-0.4.1/citation_utils/special.py
+-rw-r--r--   0        0        0     1312 2023-06-24 07:19:52.340761 citation_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      759 1970-01-01 00:00:00.000000 citation_utils-0.4.1/PKG-INFO
```

### Comparing `citation_utils-0.4.0/LICENSE` & `citation_utils-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/__init__.py` & `citation_utils-0.4.1/citation_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/citation.py` & `citation_utils-0.4.1/citation_utils/citation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import datetime
 import logging
+import re
 from collections.abc import Iterator
 from typing import Self
 
 from citation_report import Report
 from citation_report.main import is_eq
 from pydantic import BaseModel, ConfigDict, Field
 
 from .dockets import DocketCategory
 from .document import CitableDocument
 
+docket_serial_export_pattern = re.compile(r"^[a-z0-9-]+$")
+"""Alphanumeric lowercase with dash"""
+
 
 class Citation(BaseModel):
     """
     A Philippine Supreme Court `Citation` consists of:
 
     1. `Docket` includes:
         1. _category_,
@@ -85,14 +89,74 @@
                         ok_serial and (self.docket_serial == other.docket_serial),
                         ok_date and (self.docket_date == other.docket_date),
                     ]
                 ),
             ]
         )
 
+    def is_serial_ok(self) -> bool:
+        """If a serial number exists, ensure it meets criteria prior to row creation."""
+        if self.docket_serial:
+            if docket_serial_export_pattern.search(self.docket_serial.lower()):
+                return True
+            return False
+        return True
+
+    def make_decision_row(self):
+        """This presumes that a valid docket exists. Although a citation can
+        be a non-docket, e.g. phil, scra, etc., for purposes of creating a
+        a route-based row for a prospective decision object, the identifier will be
+        based on a docket id."""
+        if not self.is_serial_ok():
+            logging.error(f"Invalid {self.docket_serial=}")
+            return None
+
+        docket_id = None
+        if self.docket_category and self.docket_serial and self.docket_date:
+            cat = self.docket_category.name.lower()
+            num = self.docket_serial.lower()
+            date = self.docket_date.isoformat()
+            docket_id = "-".join([cat, num, date])
+            return {
+                "id": docket_id,
+                "cat": cat,
+                "num": self.docket_serial,
+                "date": date,
+                "phil": self.phil,
+                "scra": self.scra,
+                "offg": self.offg,
+            }
+        logging.error(f"Could not make docket slug: {self.docket=}")
+        return None
+
+    def make_generic_row(self):
+        """Unlike `make_decision_row()`, this citation is spotted in the wild;
+        may not contain a docket or the docket not yet yet properly formatted."""
+
+        cat = None
+        if self.docket_category:
+            cat = self.docket_category.name.lower()
+
+        num = None
+        if self.docket_serial:
+            num = self.docket_serial.lower()
+
+        date = None
+        if self.docket_date:
+            date = self.docket_date.isoformat()
+
+        return {
+            "cat": cat,
+            "num": num,
+            "date": date,
+            "phil": self.phil,
+            "scra": self.scra,
+            "offg": self.offg,
+        }
+
     @classmethod
     def _set_report(cls, text: str):
         try:
             obj = next(Report.extract_reports(text))
             return cls(
                 docket=None,
                 docket_category=None,
```

### Comparing `citation_utils-0.4.0/citation_utils/dockets/__init__.py` & `citation_utils-0.4.1/citation_utils/dockets/__init__.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_ac.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_ac.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_am.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_am.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_bm.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_bm.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_gr.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_gr.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_jib.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_jib.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_oca.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_oca.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_pet.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_pet.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/constructed_udk.py` & `citation_utils-0.4.1/citation_utils/dockets/constructed_udk.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/constructor.py` & `citation_utils-0.4.1/citation_utils/dockets/models/constructor.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/docket_category.py` & `citation_utils-0.4.1/citation_utils/dockets/models/docket_category.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/docket_citation.py` & `citation_utils-0.4.1/citation_utils/dockets/models/docket_citation.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/docket_model.py` & `citation_utils-0.4.1/citation_utils/dockets/models/docket_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from datetime import date
 from typing import Self
 
 from citation_date import DOCKET_DATE_FORMAT
 from citation_report.main import is_eq
 from pydantic import BaseModel, ConfigDict, Field
 
@@ -13,50 +14,58 @@
     """
     The Docket is the modern identifier of a Supreme Court decision.
 
     It is based on a `category`, a `serial id`, and a `date`.
 
     Field | Type | Description
     --:|:--:|:--
-    `context` | optional (str) | Full texted matched by the regex pattern
-    `category` | optional (DocketCategory) | See [docket-category-model][]
+    `context` | optional (str) | Full text matched by the regex pattern
+    `category` | optional (DocketCategory) | Whether GR, AC, etc.
     `ids` | optional (str) | The serial number of the docket category
     `docket_date` | optional (date) | The date associated with the docket
 
     Sample Citation | Category | Serial | Date
     :-- |:--:|:--:|:--:
     _G.R. Nos. 138570, October 10, 2000_ | GR | 74910 | October 10, 2000
     _A.M. RTJ-12-2317 (Formerly OCA I.P.I. No. 10-3378-RTJ), Jan 1, 2000_ | AM | RTJ-12-2317 |Jan 1, 2000
     _A.C. No. 10179 (Formerly CBD 11-2985), March 04, 2014_ | AC | 10179 | Mar. 4, 2014
 
     The Docket is often paired with a Report, which is the traditional
     identifier based on volume and page numbers.
+
+    # TODO: need further cleaning of serial_text
     """  # noqa: E501
 
     model_config = ConfigDict(use_enum_values=True)
     context: str = Field(..., description="Full text matched by regex pattern.")
     category: DocketCategory = Field(..., description="e.g. General Register, etc.")
-    ids: str = Field(..., description="Ok for a csv token, e.g. '24141, 14234, 12'")
-    docket_date: date = Field(..., description="Either in UK, US styles")
+    ids: str = Field(..., description="May be comma-separated, e.g. '12, 32, and 41'")
+    docket_date: date = Field(...)
 
     def __repr__(self) -> str:
         return f"<Docket: {self.category} {self.serial_text}, {self.formatted_date}>"
 
     def __str__(self) -> str:
         if self.serial_text:
-            return f"{self.category} {self.serial_text}, {self.formatted_date}"
+            return f"{self.category} No. {self.serial_text.upper()}, {self.formatted_date}"  # noqa: E501
         return "No proper string detected."
 
     def __eq__(self, other: Self) -> bool:
         opt_1 = is_eq(self.category.name, other.category.name)
         opt_2 = is_eq(self.first_id, other.first_id)
         opt_3 = is_eq(self.docket_date.isoformat(), other.docket_date.isoformat())
         return all([opt_1, opt_2, opt_3])
 
     @property
+    def slug(self):
+        return "-".join(
+            [self.category.name, self.serial_text, self.docket_date.isoformat()]
+        )
+
+    @property
     def serial_text(self) -> str:
         """From raw `ids`, get the `cleaned_ids`, and of these `cleaned_ids`,
             extract the `@first_id` found to deal with compound ids, e.g.
             ids separated by 'and' and ','
 
         Returns:
             str: Singular text identifier
```

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/docket_rules.py` & `citation_utils-0.4.1/citation_utils/dockets/models/docket_rules.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/gr_clean.py` & `citation_utils-0.4.1/citation_utils/dockets/models/gr_clean.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/misc/extra.py` & `citation_utils-0.4.1/citation_utils/dockets/models/misc/extra.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/dockets/models/misc/num.py` & `citation_utils-0.4.1/citation_utils/dockets/models/misc/num.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/document.py` & `citation_utils-0.4.1/citation_utils/document.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/citation_utils/special.py` & `citation_utils-0.4.1/citation_utils/special.py`

 * *Files identical despite different names*

### Comparing `citation_utils-0.4.0/pyproject.toml` & `citation_utils-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "citation_utils"
-version = "0.4.0"
+version = "0.4.1"
 description = "Pattern matching Philippine Supreme Court citations."
 authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 homepage = "https://lawsql.com"
 repository = "https://github.com/justmars/citation-utils"
 documentation = "https://justmars.github.io/citation-utils"
 classifiers = [
   "Topic :: Text Processing :: General",
```

### Comparing `citation_utils-0.4.0/PKG-INFO` & `citation_utils-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citation-utils
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pattern matching Philippine Supreme Court citations.
 Home-page: https://lawsql.com
 Author: Marcelino G. Veloso III
 Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pydantic
```

