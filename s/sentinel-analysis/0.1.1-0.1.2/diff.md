# Comparing `tmp/sentinel_analysis-0.1.1.tar.gz` & `tmp/sentinel_analysis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentinel_analysis-0.1.1.tar", max compression
+gzip compressed data, was "sentinel_analysis-0.1.2.tar", max compression
```

## Comparing `sentinel_analysis-0.1.1.tar` & `sentinel_analysis-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.1/README.md
--rw-r--r--   0        0        0      476 2023-06-25 12:08:37.630695 sentinel_analysis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0  2426645 2023-06-25 11:58:26.983350 sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIP.dat
--rw-r--r--   0        0        0  6025934 2023-06-25 11:58:26.991351 sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat
--rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.1/sentinel_analysis/__init__.py
--rw-r--r--   0        0        0     7219 2023-06-25 11:58:27.047352 sentinel_analysis-0.1.1/sentinel_analysis/__main__.py
--rw-r--r--   0        0        0     3670 2023-06-25 11:59:13.928759 sentinel_analysis-0.1.1/sentinel_analysis/alert.py
--rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.1/sentinel_analysis/report.py
--rw-r--r--   0        0        0      450 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.2/README.md
+-rw-r--r--   0        0        0      643 2023-06-25 16:03:24.260032 sentinel_analysis-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0  2426645 2023-06-25 11:58:26.983350 sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIP.dat
+-rw-r--r--   0        0        0  6025934 2023-06-25 11:58:26.991351 sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat
+-rw-r--r--   0        0        0        0 2023-06-25 11:58:02.658620 sentinel_analysis-0.1.2/sentinel_analysis/__init__.py
+-rw-r--r--   0        0        0     3670 2023-06-25 11:59:13.928759 sentinel_analysis-0.1.2/sentinel_analysis/alert.py
+-rw-r--r--   0        0        0     7140 2023-06-25 16:02:24.386229 sentinel_analysis-0.1.2/sentinel_analysis/main.py
+-rw-r--r--   0        0        0      478 2023-06-25 11:58:27.079353 sentinel_analysis-0.1.2/sentinel_analysis/report.py
+-rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 sentinel_analysis-0.1.2/PKG-INFO
```

### Comparing `sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIP.dat` & `sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIP.dat`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.1/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat` & `sentinel_analysis-0.1.2/sentinel_analysis/GeoIP_DBs/GeoIPASNum.dat`

 * *Files identical despite different names*

### Comparing `sentinel_analysis-0.1.1/sentinel_analysis/__main__.py` & `sentinel_analysis-0.1.2/sentinel_analysis/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,20 @@
 import ipaddress
 import math
 import os
 
 import matplotlib.pyplot as plt
 import pandas as pd
 import pygeoip
-import report
-from alert import BotnetAlert, ExfiltrationAlert
+from . import report
+from .alert import BotnetAlert, ExfiltrationAlert
 from scipy.stats import norm
 
 alerts = {}
 
-if not os.path.exists("images"):
-    os.mkdir("images")
-
-
 def printq(*args):
     if not arguments.quiet:
         print(*args)
 
 
 def dataExfiltration(percentage):
     printq(
@@ -143,15 +139,15 @@
     ax.set_ylabel("Number of connection")
 
     for i, v in enumerate(volume):
         ax.text(v, i, str(v), va="center")
 
     ax.set_title("Number of connection per country")
 
-    filepath = "images/volumexcountry"
+    filepath = "volumexcountry"
     fig.savefig(fname=filepath)
 
     return f"""
 # Connection volume by country
 
 The correlation between connection volume and country of destination can be viewed in the graphic bellow.
 
@@ -166,15 +162,15 @@
     fig, ax = plt.subplots(figsize=(10, 6))
     ax.bar(hourly.index,hourly.values)
     ax.set_xlabel("Hours")
     ax.set_ylabel("Number of connections")
     ax.set_title("Connections per hour during a day")
     ax.set_xticks(range(24))
     
-    filepath = "images/connectionsxhour"
+    filepath = "connectionsxhour"
     fig.savefig(fname=filepath)
 
     printq(hourly)
 
     return f"""
 # Connection volume per hour
 
@@ -210,15 +206,16 @@
                 intro += r
 
     # Print results to pdf
     if dict(arguments._get_kwargs())["pdf"]:
         report.printReport(alerts, intro)
 
 
-if __name__ == "__main__":
+
+def cli():
     parser = argparse.ArgumentParser(description="Traffic analysis tool.")
     parser.add_argument(
         "--data", type=str, help="Path to datafile to analyze", required=True
     )
 
     parser.add_argument(
         "-dx",
```

### Comparing `sentinel_analysis-0.1.1/sentinel_analysis/alert.py` & `sentinel_analysis-0.1.2/sentinel_analysis/alert.py`

 * *Files identical despite different names*

