# Comparing `tmp/inventree-wled-locator-0.2.0.tar.gz` & `tmp/inventree-wled-locator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/inventree-wled-locator/inventree-wled-locator/dist/.tmp-111vhst7/inventree-wled-locator-0.2.0.tar", last modified: Sun Jun 25 19:49:46 2023, max compression
+gzip compressed data, was "/home/runner/work/inventree-wled-locator/inventree-wled-locator/dist/.tmp-4m9_h04n/inventree-wled-locator-0.2.1.tar", last modified: Sun Jun 25 19:56:32 2023, max compression
```

## Comparing `inventree-wled-locator-0.2.0.tar` & `inventree-wled-locator-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator/
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator/WledPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 19:49:31.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 19:49:46.000000 inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/WledPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-25 19:56:14.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-25 19:56:32.000000 inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/top_level.txt
```

### Comparing `inventree-wled-locator-0.2.0/LICENSE` & `inventree-wled-locator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inventree-wled-locator-0.2.0/PKG-INFO` & `inventree-wled-locator-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wled-locator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use WLED to locate InvenTree StockLocations.
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-wled-locator
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-wled-locator/issues
 Keywords: inventree,inventree-plugin,inventree-wled-locator
 Classifier: Programming Language :: Python :: 3
```

### Comparing `inventree-wled-locator-0.2.0/README.md` & `inventree-wled-locator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `inventree-wled-locator-0.2.0/pyproject.toml` & `inventree-wled-locator-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools", "wheel", "pyyaml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "inventree-wled-locator"
-version =  "0.2.0"
+version =  "0.2.1"
 description="Use WLED to locate InvenTree StockLocations."
 readme = "README.md"
 license = {text = "MIT license"}
 keywords = ["inventree", "inventree-plugin", "inventree-wled-locator"]
 authors = [
     {name = "Matthias Mair", email =  "code@mjmair.com"}
 ]
```

### Comparing `inventree-wled-locator-0.2.0/src/inventree_wled_locator/WledPlugin.py` & `inventree-wled-locator-0.2.1/src/inventree_wled_locator/WledPlugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Use WLED to locate InvenTree StockLocations.."""
 
 import logging
 
 import requests
 from common.notifications import NotificationBody
+from django.conf.urls import url
 from django.contrib.auth import get_user_model
 from django.core.validators import MinValueValidator
+from django.shortcuts import redirect
+from django.urls import reverse
 from django.utils.translation import ugettext_lazy as _
 from InvenTree.helpers_model import notify_users
 from plugin import InvenTreePlugin
-from plugin.mixins import LocateMixin, SettingsMixin
+from plugin.mixins import LocateMixin, SettingsMixin, UrlsMixin
 from stock.models import StockLocation
 
 logger = logging.getLogger('inventree')
 
 
-class WledPlugin(LocateMixin, SettingsMixin, InvenTreePlugin):
+class WledPlugin(UrlsMixin, LocateMixin, SettingsMixin, InvenTreePlugin):
     """Use WLED to locate InvenTree StockLocations.."""
 
     NAME = 'WledPlugin'
     SLUG = 'inventree-wled-locator'
     TITLE = "WLED Locator"
 
     NO_LED_NOTIFICATION = NotificationBody(
@@ -39,40 +42,58 @@
             'default': 1,
             'validator': [int, MinValueValidator(1), ],
         },
     }
 
     superusers = list(get_user_model().objects.filter(is_superuser=True).all())
 
-    def set_led(self, target_led: int = None):
-        """Turn on a specific LED."""
-        base_url = f'http://{self.get_setting("ADDRESS")}/json/state'
-        color_black = '000000'
-        color_marked = 'FF0000'
-
-        # Turn off all segments
-        requests.post(base_url, json={"seg": {"i": [0, self.get_setting("MAX_LEDS"), color_black]}})
-
-        # Turn on target led
-        if target_led:
-            requests.post(base_url, json={"seg": {"i": [target_led, color_marked]}})
-
     def locate_stock_location(self, location_pk):
         """Locate a StockLocation.
 
         Args:
             location_pk: primary key for location
         """
         logger.info(f"Attempting to locate location ID {location_pk}")
 
         try:
             location = StockLocation.objects.get(pk=location_pk)
             led_nbr = location.get_metadata('wled_led')
             if led_nbr:
-                self.set_led(led_nbr)
+                self._set_led(led_nbr)
             else:
                 # notify superusers that a location has no LED number
                 logger.error(f"Location ID {location_pk} has no WLED LED number!")
                 notify_users(self.superusers, location, StockLocation, content=self.NO_LED_NOTIFICATION)
 
         except (ValueError, StockLocation.DoesNotExist):  # pragma: no cover
             logger.error(f"Location ID {location_pk} does not exist!")
+
+    def view_off(self, request):
+        """Turn off all LEDs."""
+        self._set_led()
+        return redirect(self.settings_url)
+
+    def setup_urls(self):
+        """Return the URLs defined by this plugin."""
+        return [
+            url(r'off/', self.view_off, name='off'),
+        ]
+
+    def get_settings_content(self, request):
+        """Add context to the settings panel."""
+        return f"""
+        <h3>WLED controlls</h3>
+        <p>Turn off all LEDs: <a href="{reverse('plugin:inventree-wled-locator:off')}">turn off</a></p>
+        """
+
+    def _set_led(self, target_led: int = None):
+        """Turn on a specific LED."""
+        base_url = f'http://{self.get_setting("ADDRESS")}/json/state'
+        color_black = '000000'
+        color_marked = 'FF0000'
+
+        # Turn off all segments
+        requests.post(base_url, json={"seg": {"i": [0, self.get_setting("MAX_LEDS"), color_black]}})
+
+        # Turn on target led
+        if target_led:
+            requests.post(base_url, json={"seg": {"i": [target_led, color_marked]}})
```

### Comparing `inventree-wled-locator-0.2.0/src/inventree_wled_locator.egg-info/PKG-INFO` & `inventree-wled-locator-0.2.1/src/inventree_wled_locator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inventree-wled-locator
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use WLED to locate InvenTree StockLocations.
 Author-email: Matthias Mair <code@mjmair.com>
 License: MIT license
 Project-URL: Repository, https://github.com/matmair/inventree-wled-locator
 Project-URL: Bug Tracker, https://github.com/matmair/inventree-wled-locator/issues
 Keywords: inventree,inventree-plugin,inventree-wled-locator
 Classifier: Programming Language :: Python :: 3
```

