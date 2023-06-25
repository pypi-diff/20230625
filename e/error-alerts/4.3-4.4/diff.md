# Comparing `tmp/error-alerts-4.3.tar.gz` & `tmp/error-alerts-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error-alerts-4.3.tar", last modified: Thu Jun 22 14:54:28 2023, max compression
+gzip compressed data, was "error-alerts-4.4.tar", last modified: Sun Jun 25 16:11:00 2023, max compression
```

## Comparing `error-alerts-4.3.tar` & `error-alerts-4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.424728 error-alerts-4.3/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.3/.gitignore
--rw-rw-rw-   0        0        0     1305 2023-06-22 14:54:28.424728 error-alerts-4.3/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.419732 error-alerts-4.3/error_alerts/
--rw-rw-rw-   0        0        0     2406 2023-06-22 14:54:25.000000 error-alerts-4.3/error_alerts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 14:54:28.423729 error-alerts-4.3/error_alerts.egg-info/
--rw-rw-rw-   0        0        0     1305 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-22 14:54:28.000000 error-alerts-4.3/error_alerts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 14:54:28.425728 error-alerts-4.3/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-06-22 14:54:21.000000 error-alerts-4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:11:00.478936 error-alerts-4.4/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:39:52.000000 error-alerts-4.4/.gitignore
+-rw-rw-rw-   0        0        0     1305 2023-06-25 16:11:00.479935 error-alerts-4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-01-08 12:52:11.000000 error-alerts-4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 16:11:00.474939 error-alerts-4.4/error_alerts/
+-rw-rw-rw-   0        0        0     2513 2023-06-25 16:10:54.000000 error-alerts-4.4/error_alerts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 16:11:00.478936 error-alerts-4.4/error_alerts.egg-info/
+-rw-rw-rw-   0        0        0     1305 2023-06-25 16:11:00.000000 error-alerts-4.4/error_alerts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-06-25 16:11:00.000000 error-alerts-4.4/error_alerts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 16:11:00.000000 error-alerts-4.4/error_alerts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-25 16:11:00.000000 error-alerts-4.4/error_alerts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-25 16:11:00.000000 error-alerts-4.4/error_alerts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-25 16:11:00.479935 error-alerts-4.4/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-06-25 16:10:57.000000 error-alerts-4.4/setup.py
```

### Comparing `error-alerts-4.3/PKG-INFO` & `error-alerts-4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.3
+Version: 4.4
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

### Comparing `error-alerts-4.3/README.md` & `error-alerts-4.4/README.md`

 * *Files identical despite different names*

### Comparing `error-alerts-4.3/error_alerts/__init__.py` & `error-alerts-4.4/error_alerts/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import traceback
 from telegram import Bot
 
 class telegram:
     def __init__(self, token=None, channel=None, logger=None, full_error=True, raise_error=False, resend_repeat_errors=True):
         if token:
             self.bot = Bot(token=token)
+            self.username = self.bot.username
         self.channel = channel
         self.logger = logger
         self.full_error = full_error
         self.raise_error = raise_error
         self.resend_repeat_errors = resend_repeat_errors
         self.last_error = None
     def send(self, title='Error', exception=None, channel=None):
@@ -38,17 +39,19 @@
         for message in messages:
             final_message += message
             final_message += ' '
         if print_message:
             self.printer(final_message, current_time=current_time)
         if channel:
             try:
-                self.bot.send_message(channel, final_message[:4096])
+                message = self.bot.send_message(channel, final_message[:4096])
+                return message
             except Exception as telegram_error:
                 self.printer('Error sending message to Telegram:', telegram_error, level='error')
+        return None
     
     def printer(self, *items, level='info', current_time=True):
         if self.logger:
             if current_time:
                 self.logger.current_time(*items, level=level)
             else:
                 self.logger.log(*items, level=level)
```

### Comparing `error-alerts-4.3/error_alerts.egg-info/PKG-INFO` & `error-alerts-4.4/error_alerts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: error-alerts
-Version: 4.3
+Version: 4.4
 Summary: Error alerts via Telegram
 Home-page: https://github.com/xjxckk/error-alerts/
 Download-URL: https://github.com/xjxckk/error-alerts/archive/refs/tags/v2.tar.gz
 Description-Content-Type: text/markdown
 
 ### error-alerts
 Python error alerts via Telegram
```

