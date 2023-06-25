# Comparing `tmp/cbpi4-buzzer-0.0.7.tar.gz` & `tmp/cbpi4-buzzer-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-buzzer-0.0.7.tar", last modified: Sat Jun 10 12:37:23 2023, max compression
+gzip compressed data, was "cbpi4-buzzer-0.0.8.tar", last modified: Sun Jun 25 11:30:42 2023, max compression
```

## Comparing `cbpi4-buzzer-0.0.7.tar` & `cbpi4-buzzer-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:22.999913 cbpi4-buzzer-0.0.7/
--rw-rw-rw-   0        0        0    35129 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       33 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1210 2023-06-10 12:37:22.998913 cbpi4-buzzer-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      869 2023-06-10 12:37:00.000000 cbpi4-buzzer-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:22.955920 cbpi4-buzzer-0.0.7/cbpi4-buzzer/
--rw-rw-rw-   0        0        0    16128 2023-04-16 15:31:44.000000 cbpi4-buzzer-0.0.7/cbpi4-buzzer/__init__.py
--rw-rw-rw-   0        0        0       29 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.7/cbpi4-buzzer/config.yaml
-drwxrwxrwx   0        0        0        0 2023-06-10 12:37:22.994915 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/
--rw-rw-rw-   0        0        0     1210 2023-06-10 12:37:22.000000 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-06-10 12:37:22.000000 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 12:37:22.000000 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-10 12:37:22.000000 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-10 12:37:22.000000 cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-10 12:37:23.000915 cbpi4-buzzer-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      978 2023-06-10 12:36:29.000000 cbpi4-buzzer-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 11:30:42.378427 cbpi4-buzzer-0.0.8/
+-rw-rw-rw-   0        0        0    35129 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       33 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1319 2023-06-25 11:30:42.374428 cbpi4-buzzer-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      978 2023-06-25 11:29:45.000000 cbpi4-buzzer-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 11:30:42.310424 cbpi4-buzzer-0.0.8/cbpi4-buzzer/
+-rw-rw-rw-   0        0        0    16100 2023-06-25 11:28:40.000000 cbpi4-buzzer-0.0.8/cbpi4-buzzer/__init__.py
+-rw-rw-rw-   0        0        0       29 2021-04-17 11:11:38.000000 cbpi4-buzzer-0.0.8/cbpi4-buzzer/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-25 11:30:42.371428 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/
+-rw-rw-rw-   0        0        0     1319 2023-06-25 11:30:42.000000 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-25 11:30:42.000000 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 11:30:42.000000 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-25 11:30:42.000000 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-25 11:30:42.000000 cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 11:30:42.379425 cbpi4-buzzer-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      978 2023-06-25 11:29:53.000000 cbpi4-buzzer-0.0.8/setup.py
```

### Comparing `cbpi4-buzzer-0.0.7/LICENSE` & `cbpi4-buzzer-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-buzzer-0.0.7/PKG-INFO` & `cbpi4-buzzer-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.7
+Version: 0.0.8
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -19,14 +19,15 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 25.06.23: (0.0.8) internal change on startup with respect to logging of parameter check for gpio_inverted
 - 10.06.23: (0.0.7) fix issues in setup.py
 - 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
```

### Comparing `cbpi4-buzzer-0.0.7/README.md` & `cbpi4-buzzer-0.0.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 25.06.23: (0.0.8) internal change on startup with respect to logging of parameter check for gpio_inverted
 - 10.06.23: (0.0.7) fix issues in setup.py
 - 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
```

### Comparing `cbpi4-buzzer-0.0.7/cbpi4-buzzer/__init__.py` & `cbpi4-buzzer-0.0.8/cbpi4-buzzer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.sound = {'standard':["H", 0.1, "L", 0.1, "H", 0.1, "L", 0.1, "H", 0.1, "L"],
                       'warning':["H", 0.2, "L", 0.1, "H", 0.1, "L", 0.1, "H", 0.2, "L"],
                       'error':["H", 0.3, "L", 0.1, "H", 0.3, "L", 0.1, "H", 0.3, "L"]}
         logger.info('Starting Buzzer background task')
         await self.buzzer_settings()
         if buzzer_gpio is None or buzzer_gpio == "" or not buzzer_gpio:
             logger.warning('Check buzzer GPIO is set')
-        if buzzer_gpio_inverted is None or buzzer_gpio_inverted == "" or not buzzer_gpio_inverted:
+        if buzzer_gpio_inverted is None or buzzer_gpio_inverted == "":
             logger.warning('Check buzzer GPIO Inverted is set')
         if buzzer_level is None or buzzer_level == "" or not buzzer_level:
             logger.warning('Check buzzer level is set') 
         else:
             self.listener_ID = self.cbpi.notification.add_listener(self.buzzerEvent)
             logger.info("Buzzer Lisetener ID: {}".format(self.listener_ID))
             GPIO.setmode(GPIO.BCM)
```

### Comparing `cbpi4-buzzer-0.0.7/cbpi4_buzzer.egg-info/PKG-INFO` & `cbpi4-buzzer-0.0.8/cbpi4_buzzer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbpi4-buzzer
-Version: 0.0.7
+Version: 0.0.8
 Summary: CraftBeerPi4 Buzzer Plugin
 Home-page: https://github.com/PiBrewing/cbpi4-buzzer
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
 Keywords: globalsettings
 Platform: UNKNOWN
@@ -19,14 +19,15 @@
 - buzzer_gpio: GPIO your buzzer is conected to
 - buzzer_gpio_inverted: Set to 'yes', if your buzzer is connected via inverted GPIO (High on Low)
 - buzzer_level: Sound level(High or Low)
 - Different sounds for error, warning and other message types
 
 ### Changelog
 
+- 25.06.23: (0.0.8) internal change on startup with respect to logging of parameter check for gpio_inverted
 - 10.06.23: (0.0.7) fix issues in setup.py
 - 10.06.23: (0.0.6) bump version to release
 - 02.06.23: (0.0.6.rc1) added cbpi version requirement
 - 16.04.23: (0.0.6.a4) bug fix for parameter generation
 - 05.04.23: (0.0.6.a3) Test for plugin settings selection test branch of cbpi
 - 12.03.23: (0.0.4) Added option for inverted GPIO
 - 10.04.21: (0.0.3) changed from asyncio.sleep to a thread as buzzer sound was impacted by asyncio.sleep accuracy
```

### Comparing `cbpi4-buzzer-0.0.7/setup.py` & `cbpi4-buzzer-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-buzzer',
-      version='0.0.7',
+      version='0.0.8',
       description='CraftBeerPi4 Buzzer Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
       url='https://github.com/PiBrewing/cbpi4-buzzer',
       license='GPLv3',
       keywords='globalsettings',
       include_package_data=True,
```

