# Comparing `tmp/django_tabler_icons-0.1.0.tar.gz` & `tmp/django_tabler_icons-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_tabler_icons-0.1.0.tar", last modified: Mon Feb 20 11:20:48 2023, max compression
+gzip compressed data, was "django_tabler_icons-0.2.0.tar", last modified: Sun Jun 25 06:54:16 2023, max compression
```

## Comparing `django_tabler_icons-0.1.0.tar` & `django_tabler_icons-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/
--rw-rw-r--   0 demestav  (1000) demestav  (1000)     1743 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/PKG-INFO
--rw-rw-r--   0 demestav  (1000) demestav  (1000)     1380 2023-02-20 11:13:57.000000 django_tabler_icons-0.1.0/README.md
--rw-rw-r--   0 demestav  (1000) demestav  (1000)      244 2023-01-30 13:56:37.000000 django_tabler_icons-0.1.0/pyproject.toml
--rw-rw-r--   0 demestav  (1000) demestav  (1000)      578 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/setup.cfg
-drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/src/
-drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/
--rw-rw-r--   0 demestav  (1000) demestav  (1000)     1743 2023-02-20 11:20:48.000000 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/PKG-INFO
--rw-rw-r--   0 demestav  (1000) demestav  (1000)      385 2023-02-20 11:20:48.000000 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/SOURCES.txt
--rw-rw-r--   0 demestav  (1000) demestav  (1000)        1 2023-02-20 11:20:48.000000 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/dependency_links.txt
--rw-rw-r--   0 demestav  (1000) demestav  (1000)       12 2023-02-20 11:20:48.000000 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/requires.txt
--rw-rw-r--   0 demestav  (1000) demestav  (1000)       13 2023-02-20 11:20:48.000000 django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/top_level.txt
-drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/src/tabler_icons/
--rw-rw-r--   0 demestav  (1000) demestav  (1000)      282 2023-02-20 09:50:38.000000 django_tabler_icons-0.1.0/src/tabler_icons/__init__.py
-drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-02-20 11:20:48.758409 django_tabler_icons-0.1.0/src/tabler_icons/templatetags/
--rw-rw-r--   0 demestav  (1000) demestav  (1000)        0 2023-01-30 13:48:12.000000 django_tabler_icons-0.1.0/src/tabler_icons/templatetags/__init__.py
--rw-rw-r--   0 demestav  (1000) demestav  (1000)     1222 2023-02-20 11:09:47.000000 django_tabler_icons-0.1.0/src/tabler_icons/templatetags/tabler_icons.py
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)     1743 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/PKG-INFO
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)     1380 2023-02-20 11:13:57.000000 django_tabler_icons-0.2.0/README.md
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)      244 2023-01-30 13:56:37.000000 django_tabler_icons-0.2.0/pyproject.toml
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)      578 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/setup.cfg
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)     1743 2023-06-25 06:54:16.000000 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/PKG-INFO
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)      555 2023-06-25 06:54:16.000000 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/SOURCES.txt
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)        1 2023-06-25 06:54:16.000000 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/dependency_links.txt
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)       12 2023-06-25 06:54:16.000000 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/requires.txt
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)       13 2023-06-25 06:54:16.000000 django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/top_level.txt
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/tabler_icons/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)      282 2023-02-20 09:50:38.000000 django_tabler_icons-0.2.0/src/tabler_icons/__init__.py
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/tabler_icons/management/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:52:47.000000 django_tabler_icons-0.2.0/src/tabler_icons/management/__init__.py
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/tabler_icons/management/commands/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:52:57.000000 django_tabler_icons-0.2.0/src/tabler_icons/management/commands/__init__.py
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)     1234 2023-02-20 11:10:26.000000 django_tabler_icons-0.2.0/src/tabler_icons/management/commands/download_icons.py
+drwxrwxr-x   0 demestav  (1000) demestav  (1000)        0 2023-06-25 06:54:16.987669 django_tabler_icons-0.2.0/src/tabler_icons/templatetags/
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)        0 2023-01-30 13:48:12.000000 django_tabler_icons-0.2.0/src/tabler_icons/templatetags/__init__.py
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)     1066 2023-02-24 13:38:09.000000 django_tabler_icons-0.2.0/src/tabler_icons/templatetags/tabler_icons.py
+-rw-rw-r--   0 demestav  (1000) demestav  (1000)      426 2023-02-24 13:37:48.000000 django_tabler_icons-0.2.0/src/tabler_icons/utils.py
```

### Comparing `django_tabler_icons-0.1.0/PKG-INFO` & `django_tabler_icons-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_tabler_icons
-Version: 0.1.0
+Version: 0.2.0
 Summary: Use tabler icons with django templates
 Home-page: https://github.com/demestav/django-tabler-icons
 Author: Demetris Stavrou
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `django_tabler_icons-0.1.0/README.md` & `django_tabler_icons-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `django_tabler_icons-0.1.0/setup.cfg` & `django_tabler_icons-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_tabler_icons
-version = 0.1.0
+version = 0.2.0
 description = Use tabler icons with django templates
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/demestav/django-tabler-icons
 author = Demetris Stavrou
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `django_tabler_icons-0.1.0/src/django_tabler_icons.egg-info/PKG-INFO` & `django_tabler_icons-0.2.0/src/django_tabler_icons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tabler-icons
-Version: 0.1.0
+Version: 0.2.0
 Summary: Use tabler icons with django templates
 Home-page: https://github.com/demestav/django-tabler-icons
 Author: Demetris Stavrou
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `django_tabler_icons-0.1.0/src/tabler_icons/templatetags/tabler_icons.py` & `django_tabler_icons-0.2.0/src/tabler_icons/templatetags/tabler_icons.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 from __future__ import annotations
 
 import re
 
 from django import template
 from django.utils.html import mark_safe
-from tabler_icons import icon_directory
+from tabler_icons.utils import read_icon
 
 register = template.Library()
 
 
 @register.simple_tag
 def tabler_icon(icon_name, classes=None, keep_default_classes="yes"):
     if classes is None:
         classes = []
     elif isinstance(classes, str):
         classes = classes.split(",")
 
-    icon_path = icon_directory / f"{icon_name}.svg"
-
-    if not icon_path:
-        raise ValueError("Icon %s not found" % icon_name)
-
-    with open(icon_path) as f:
-        icon_code = mark_safe(f.read())
+    icon_code = mark_safe(read_icon(icon_name))
 
     class_attribute_regex = re.compile(r'class="(.*?)"')
     match = class_attribute_regex.search(icon_code)
 
     # Set classes
     if match is None:
         updated_icon_code = class_attribute_regex.sub(
```

