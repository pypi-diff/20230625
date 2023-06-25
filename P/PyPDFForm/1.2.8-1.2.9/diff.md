# Comparing `tmp/PyPDFForm-1.2.8.tar.gz` & `tmp/PyPDFForm-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFForm-1.2.8.tar", last modified: Sun Apr 23 16:09:49 2023, max compression
+gzip compressed data, was "PyPDFForm-1.2.9.tar", last modified: Sun Jun 11 04:10:16 2023, max compression
```

## Comparing `PyPDFForm-1.2.8.tar` & `PyPDFForm-1.2.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.059944 PyPDFForm-1.2.8/PyPDFForm/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/filler.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)    10028 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/core/watermark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/dropdown.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/element.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/middleware/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/PyPDFForm/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/PyPDFForm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-23 16:09:49.000000 PyPDFForm-1.2.8/PyPDFForm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 16:09:49.063944 PyPDFForm-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-04-23 16:09:38.000000 PyPDFForm-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.078910 PyPDFForm-1.2.9/PyPDFForm/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.082911 PyPDFForm-1.2.9/PyPDFForm/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/filler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/font_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10862 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/core/watermark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/PyPDFForm/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/dropdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/middleware/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/PyPDFForm/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 04:10:16.082911 PyPDFForm-1.2.9/PyPDFForm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-11 04:10:16.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 04:10:15.000000 PyPDFForm-1.2.9/PyPDFForm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 04:10:16.086911 PyPDFForm-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-11 04:09:59.000000 PyPDFForm-1.2.9/setup.py
```

### Comparing `PyPDFForm-1.2.8/LICENSE` & `PyPDFForm-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PKG-INFO` & `PyPDFForm-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.8
+Version: 1.2.9
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.8 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.9 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/filler.py` & `PyPDFForm-1.2.9/PyPDFForm/core/filler.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict
 
 import pdfrw
 
 from ..middleware.checkbox import Checkbox
 from ..middleware.constants import ELEMENT_TYPES
 from ..middleware.radio import Radio
+from . import font_size as font_size_core
 from . import template, utils
 from . import watermark as watermark_core
 
 
 def fill(
     template_stream: bytes,
     elements: Dict[str, ELEMENT_TYPES],
@@ -29,15 +30,15 @@
         texts_to_draw[page] = []
         text_watermarks.append(b"")
         for _element in _elements:
             key = template.get_element_key(_element)
 
             if isinstance(elements[key], Checkbox):
                 if elements[key].value:
-                    font_size = utils.checkbox_radio_font_size(_element)
+                    font_size = font_size_core.checkbox_radio_font_size(_element)
                     _to_draw = utils.checkbox_radio_to_draw(elements[key], font_size)
                     x, y = template.get_draw_checkbox_radio_coordinates(
                         _element, _to_draw
                     )
                     texts_to_draw[page].append(
                         [
                             _to_draw,
@@ -47,15 +48,15 @@
                     )
             elif isinstance(elements[key], Radio):
                 if key not in radio_button_tracker:
                     radio_button_tracker[key] = 0
                 radio_button_tracker[key] += 1
 
                 if elements[key].value == radio_button_tracker[key] - 1:
-                    font_size = utils.checkbox_radio_font_size(_element)
+                    font_size = font_size_core.checkbox_radio_font_size(_element)
                     _to_draw = utils.checkbox_radio_to_draw(elements[key], font_size)
                     x, y = template.get_draw_checkbox_radio_coordinates(
                         _element, _to_draw
                     )
                     texts_to_draw[page].append(
                         [
                             _to_draw,
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/font.py` & `PyPDFForm-1.2.9/PyPDFForm/core/font.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/image.py` & `PyPDFForm-1.2.9/PyPDFForm/core/image.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/patterns.py` & `PyPDFForm-1.2.9/PyPDFForm/core/patterns.py`

 * *Files 22% similar despite different names*

```diff
@@ -77,7 +77,17 @@
     {constants.PARENT_KEY: {constants.CHOICES_IDENTIFIER: True}},
 ]
 
 ELEMENT_ALIGNMENT_PATTERNS = [
     {constants.TEXT_FIELD_ALIGNMENT_IDENTIFIER: True},
     {constants.PARENT_KEY: {constants.TEXT_FIELD_ALIGNMENT_IDENTIFIER: True}},
 ]
+
+TEXT_FIELD_FLAG_PATTERNS = [
+    {constants.FIELD_FLAG_KEY: True},
+    {constants.PARENT_KEY: {constants.FIELD_FLAG_KEY: True}},
+]
+
+TEXT_FIELD_APPEARANCE_PATTERNS = [
+    {constants.TEXT_FIELD_APPEARANCE_IDENTIFIER: True},
+    {constants.PARENT_KEY: {constants.TEXT_FIELD_APPEARANCE_IDENTIFIER: True}},
+]
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/template.py` & `PyPDFForm-1.2.9/PyPDFForm/core/template.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 import pdfrw
 from reportlab.pdfbase.pdfmetrics import stringWidth
 
 from ..middleware.constants import ELEMENT_TYPES
 from ..middleware.text import Text
 from . import constants, utils
 from .patterns import (DROPDOWN_CHOICE_PATTERNS, ELEMENT_ALIGNMENT_PATTERNS,
-                       ELEMENT_KEY_PATTERNS, ELEMENT_TYPE_PATTERNS)
+                       ELEMENT_KEY_PATTERNS, ELEMENT_TYPE_PATTERNS,
+                       TEXT_FIELD_APPEARANCE_PATTERNS,
+                       TEXT_FIELD_FLAG_PATTERNS)
 
 
 def remove_all_elements(pdf: bytes) -> bytes:
     """Removes all elements from a pdfrw parsed PDF form."""
 
     pdf = pdfrw.PdfReader(fdata=pdf)
 
@@ -148,14 +150,32 @@
             element_middleware.font_size,
         )
         / 2,
         (height_mid_point - string_height / 2 + height_mid_point) / 2,
     )
 
 
+def get_text_field_font_size(element: pdfrw.PdfDict) -> Union[float, int]:
+    """Returns the font size of the text field if presented or zero."""
+
+    result = 0
+    for pattern in TEXT_FIELD_APPEARANCE_PATTERNS:
+        text_appearance = traverse_pattern(pattern, element)
+        if text_appearance:
+            properties = text_appearance.split(" ")
+            if len(properties) > 1:
+                try:
+                    result = float(properties[1])
+                    break
+                except ValueError:
+                    pass
+
+    return result
+
+
 def get_text_field_max_length(element: pdfrw.PdfDict) -> Union[int, None]:
     """Returns the max length of the text field if presented or None."""
 
     return (
         int(element[constants.TEXT_FIELD_MAX_LENGTH_KEY])
         if constants.TEXT_FIELD_MAX_LENGTH_KEY in element
         else None
@@ -170,16 +190,25 @@
     except IndexError:
         return False
 
 
 def is_text_multiline(element: pdfrw.PdfDict) -> bool:
     """Returns true if a text field is a paragraph field."""
 
+    field_flag = None
+    for pattern in TEXT_FIELD_FLAG_PATTERNS:
+        field_flag = traverse_pattern(pattern, element)
+        if field_flag is not None:
+            break
+
+    if field_flag is None:
+        return False
+
     try:
-        return "{0:b}".format(int(element[constants.FIELD_FLAG_KEY]))[::-1][12] == "1"
+        return "{0:b}".format(int(field_flag))[::-1][12] == "1"
     except (IndexError, TypeError):
         return False
 
 
 def get_dropdown_choices(element: pdfrw.PdfDict) -> Union[Tuple[str], None]:
     """Returns string options of a dropdown field."""
 
@@ -285,29 +314,23 @@
     string_height = element_middleware.font_size * 96 / 72
     height_mid_point = (
         float(element[constants.ANNOTATION_RECTANGLE_KEY][1])
         + float(element[constants.ANNOTATION_RECTANGLE_KEY][3])
     ) / 2
     y = (height_mid_point - string_height / 2 + height_mid_point) / 2
     if is_text_multiline(element):
-        y = float(element[constants.ANNOTATION_RECTANGLE_KEY][3]) - string_height / 2
+        y = float(element[constants.ANNOTATION_RECTANGLE_KEY][3]) - string_height / 1.5
 
-    return (
-        x
-        - (
-            character_paddings[0]
-            + stringWidth(
-                element_value[:1],
-                element_middleware.font,
-                element_middleware.font_size,
+    if int(alignment) == 1 and element_middleware.comb is True and length != 0:
+        x -= character_paddings[0] / 2
+        if length % 2 == 0:
+            x -= (
+                character_paddings[0]
+                + stringWidth(
+                    element_value[:1],
+                    element_middleware.font,
+                    element_middleware.font_size,
+                )
+                / 2
             )
-            / 2
-            if (
-                element_middleware.comb is True
-                and length != 0
-                and length % 2 == 0
-                and int(alignment) == 1
-            )
-            else 0
-        ),
-        y,
-    )
+
+    return x, y
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/utils.py` & `PyPDFForm-1.2.9/PyPDFForm/core/font_size.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 # -*- coding: utf-8 -*-
-"""Contains utility helpers."""
+"""Contains helpers for calculating font sizes."""
 
-from io import BytesIO
 from math import sqrt
-from typing import Union
+from typing import Dict, Union
 
 import pdfrw
 
-from ..middleware import constants as middleware_constants
-from ..middleware.checkbox import Checkbox
-from ..middleware.radio import Radio
+from ..middleware.constants import ELEMENT_TYPES, GLOBAL_FONT_SIZE
 from ..middleware.text import Text
-from . import constants
+from . import constants, template
 
 
-def generate_stream(pdf: pdfrw.PdfReader) -> bytes:
-    """Generates new stream for manipulated PDF form."""
+def update_text_field_font_sizes(
+    template_stream: bytes,
+    elements: Dict[str, ELEMENT_TYPES],
+) -> None:
+    """Updates text fields' font sizes."""
 
-    result_stream = BytesIO()
+    template_pdf = pdfrw.PdfReader(fdata=template_stream)
 
-    pdfrw.PdfWriter().write(result_stream, pdf)
-    result_stream.seek(0)
+    for _, _elements in template.get_elements_by_page(template_pdf).items():
+        for _element in _elements:
+            key = template.get_element_key(_element)
 
-    result = result_stream.read()
-    result_stream.close()
+            if isinstance(elements[key], Text) and elements[key].font_size is None:
+                elements[key].font_size = template.get_text_field_font_size(
+                    _element
+                ) or text_field_font_size(_element)
 
-    return result
+
+def text_field_font_size(element: pdfrw.PdfDict) -> Union[float, int]:
+    """
+    Calculates the font size it should be drawn with
+    given a text field element.
+    """
+
+    if template.is_text_multiline(element):
+        return GLOBAL_FONT_SIZE
+
+    height = abs(
+        float(element[constants.ANNOTATION_RECTANGLE_KEY][1])
+        - float(element[constants.ANNOTATION_RECTANGLE_KEY][3])
+    )
+
+    return height * 2 / 3
 
 
 def checkbox_radio_font_size(element: pdfrw.PdfDict) -> Union[float, int]:
     """
     Calculates the font size it should be drawn with
     given a checkbox/radio button element.
     """
@@ -39,50 +57,7 @@
         - float(element[constants.ANNOTATION_RECTANGLE_KEY][2])
     ) * abs(
         float(element[constants.ANNOTATION_RECTANGLE_KEY][1])
         - float(element[constants.ANNOTATION_RECTANGLE_KEY][3])
     )
 
     return sqrt(area) * 72 / 96
-
-
-def checkbox_radio_to_draw(
-    element: Union[Checkbox, Radio],
-    font_size: Union[float, int] = middleware_constants.GLOBAL_FONT_SIZE,
-) -> Text:
-    """Converts a checkbox/radio element to a drawable text element."""
-
-    new_element = Text(
-        element_name=element.name,
-        element_value="",
-    )
-    new_element.font = "Helvetica"
-    new_element.font_size = font_size
-    new_element.font_color = (0, 0, 0)
-    new_element.text_x_offset = 0
-    new_element.text_y_offset = 0
-    new_element.text_wrap_length = 100
-
-    if isinstance(element, Checkbox):
-        new_element.value = constants.CHECKBOX_TO_DRAW
-    elif isinstance(element, Radio):
-        new_element.value = constants.RADIO_TO_DRAW
-
-    return new_element
-
-
-def merge_two_pdfs(pdf: bytes, other: bytes) -> bytes:
-    """Merges two PDFs into one PDF."""
-
-    writer = pdfrw.PdfWriter()
-
-    writer.addpages(pdfrw.PdfReader(fdata=pdf).pages)
-    writer.addpages(pdfrw.PdfReader(fdata=other).pages)
-
-    result_stream = BytesIO()
-    writer.write(result_stream)
-    result_stream.seek(0)
-
-    result = result_stream.read()
-    result_stream.close()
-
-    return result
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/core/watermark.py` & `PyPDFForm-1.2.9/PyPDFForm/core/watermark.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/adapter.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/adapter.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/checkbox.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/checkbox.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/dropdown.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/dropdown.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/element.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/element.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/radio.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/radio.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/template.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/template.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
 def dropdown_to_text(dropdown: Dropdown) -> Text:
     """Converts a dropdown element to a text element."""
 
     result = Text(dropdown.name)
 
     result.font = constants.GLOBAL_FONT
-    result.font_size = constants.GLOBAL_FONT_SIZE
     result.font_color = constants.GLOBAL_FONT_COLOR
     result.text_x_offset = constants.GLOBAL_TEXT_X_OFFSET
     result.text_y_offset = constants.GLOBAL_TEXT_Y_OFFSET
     result.text_wrap_length = constants.GLOBAL_TEXT_WRAP_LENGTH
 
     if dropdown.value is not None:
         result.value = (
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm/middleware/text.py` & `PyPDFForm-1.2.9/PyPDFForm/middleware/text.py`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/PyPDFForm/wrapper.py` & `PyPDFForm-1.2.9/PyPDFForm/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """Contains user API for PyPDFForm."""
 
 from __future__ import annotations
 
 from typing import BinaryIO, Dict, Union
 
-from .core import filler, font
+from .core import filler, font, font_size
 from .core import image as image_core
 from .core import template as template_core
 from .core import utils
 from .core import watermark as watermark_core
 from .middleware import adapter, constants
 from .middleware import template as template_middleware
 from .middleware.dropdown import Dropdown
@@ -30,17 +30,15 @@
         self.elements = (
             template_middleware.build_elements(self.stream) if self.stream else {}
         )
 
         for each in self.elements.values():
             if isinstance(each, Text):
                 each.font = kwargs.get("global_font", constants.GLOBAL_FONT)
-                each.font_size = kwargs.get(
-                    "global_font_size", constants.GLOBAL_FONT_SIZE
-                )
+                each.font_size = kwargs.get("global_font_size")
                 each.font_color = kwargs.get(
                     "global_font_color", constants.GLOBAL_FONT_COLOR
                 )
                 each.text_x_offset = kwargs.get(
                     "global_text_x_offset", constants.GLOBAL_TEXT_X_OFFSET
                 )
                 each.text_y_offset = kwargs.get(
@@ -79,14 +77,15 @@
             if key in self.elements:
                 self.elements[key].value = value
 
         for key, value in self.elements.items():
             if isinstance(value, Dropdown):
                 self.elements[key] = template_middleware.dropdown_to_text(value)
 
+        font_size.update_text_field_font_sizes(self.stream, self.elements)
         if self.read():
             self.elements = template_middleware.set_character_x_paddings(
                 self.stream, self.elements
             )
 
         self.stream = template_core.remove_all_elements(
             filler.fill(self.stream, self.elements)
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm.egg-info/PKG-INFO` & `PyPDFForm-1.2.9/PyPDFForm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFForm
-Version: 1.2.8
+Version: 1.2.9
 Summary: The Python library for PDF forms.
 Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.8 Summary: The Python
+Metadata-Version: 2.1 Name: PyPDFForm Version: 1.2.9 Summary: The Python
 library for PDF forms. Home-page: https://github.com/chinapandaman/PyPDFForm
 Author: Jinge Li Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
 License-File: LICENSE
        [https://github.com/chinapandaman/PyPDFForm/raw/master/logo.png]
   [https://github.com/chinapandaman/PyPDFForm/actions/workflows/python-black-
```

### Comparing `PyPDFForm-1.2.8/PyPDFForm.egg-info/SOURCES.txt` & `PyPDFForm-1.2.9/PyPDFForm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 PyPDFForm.egg-info/dependency_links.txt
 PyPDFForm.egg-info/requires.txt
 PyPDFForm.egg-info/top_level.txt
 PyPDFForm/core/__init__.py
 PyPDFForm/core/constants.py
 PyPDFForm/core/filler.py
 PyPDFForm/core/font.py
+PyPDFForm/core/font_size.py
 PyPDFForm/core/image.py
 PyPDFForm/core/patterns.py
 PyPDFForm/core/template.py
 PyPDFForm/core/utils.py
 PyPDFForm/core/watermark.py
 PyPDFForm/middleware/__init__.py
 PyPDFForm/middleware/adapter.py
```

### Comparing `PyPDFForm-1.2.8/README.md` & `PyPDFForm-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `PyPDFForm-1.2.8/setup.py` & `PyPDFForm-1.2.9/setup.py`

 * *Files identical despite different names*

