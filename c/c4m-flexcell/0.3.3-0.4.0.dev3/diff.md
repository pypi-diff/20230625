# Comparing `tmp/c4m_flexcell-0.3.3.tar.gz` & `tmp/c4m_flexcell-0.4.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4m_flexcell-0.3.3.tar", last modified: Sun Jun 25 12:40:27 2023, max compression
+gzip compressed data, was "c4m_flexcell-0.4.0.dev3.tar", last modified: Sat Jun 24 19:34:06 2023, max compression
```

## Comparing `c4m_flexcell-0.3.3.tar` & `c4m_flexcell-0.4.0.dev3.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2022-07-12 15:00:24.000000 c4m_flexcell-0.3.3/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1264 2023-06-24 18:59:02.000000 c4m_flexcell-0.3.3/.gitlab-ci.yml
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2020-07-06 13:05:29.000000 c4m_flexcell-0.3.3/COPYRIGHT.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/LICENSE.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.922344 c4m_flexcell-0.3.3/LICENSES/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/LICENSES/agpl-3.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 09:58:12.000000 c4m_flexcell-0.3.3/LICENSES/cern_ohl_s_v2.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/LICENSES/gpl-2.0.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4246 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3774 2023-06-25 11:33:25.000000 c4m_flexcell-0.3.3/README.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.922344 c4m_flexcell-0.3.3/ReleaseNotes/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2021-03-14 14:00:41.000000 c4m_flexcell-0.3.3/ReleaseNotes/v0.0.4.md
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-08-22 13:25:11.000000 c4m_flexcell-0.3.3/ReleaseNotes/v0.1.0.md
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.922344 c4m_flexcell-0.3.3/c4m/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/c4m/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2021-05-15 12:46:28.000000 c4m_flexcell-0.3.3/c4m/cell_canvas.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.922344 c4m_flexcell-0.3.3/c4m/flexcell/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      129 2023-05-26 12:28:32.000000 c4m_flexcell-0.3.3/c4m/flexcell/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   622096 2023-06-25 10:03:10.000000 c4m_flexcell-0.3.3/c4m/flexcell/_cells.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    10483 2023-06-25 10:03:10.000000 c4m_flexcell-0.3.3/c4m/flexcell/canvas.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3272 2023-06-25 11:29:03.000000 c4m_flexcell-0.3.3/c4m/flexcell/cell.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    94698 2023-06-25 11:28:53.000000 c4m_flexcell-0.3.3/c4m/flexcell/factory.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-05-09 10:49:53.000000 c4m_flexcell-0.3.3/c4m/flexcell/stdcell.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4246 2023-06-25 12:40:27.000000 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/PKG-INFO
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      730 2023-06-25 12:40:27.000000 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/SOURCES.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-25 12:40:27.000000 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/dependency_links.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-06-25 12:40:27.000000 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/requires.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-06-25 12:40:27.000000 c4m_flexcell-0.3.3/c4m_flexcell.egg-info/top_level.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:19:21.000000 c4m_flexcell-0.3.3/ci-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-09-30 12:33:15.000000 c4m_flexcell-0.3.3/dev-requirements.txt
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2161 2023-06-25 09:51:58.000000 c4m_flexcell-0.3.3/dodo.py
--rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/run_unittests.sh
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/setup.cfg
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1394 2023-06-25 10:03:10.000000 c4m_flexcell-0.3.3/setup.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/test/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/test/__init__.py
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/test/interactive/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2020-07-14 09:04:04.000000 c4m_flexcell-0.3.3/test/interactive/.gitignore
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2020-10-06 14:32:17.000000 c4m_flexcell-0.3.3/test/interactive/export.ipynb
-drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-25 12:40:27.926344 c4m_flexcell-0.3.3/test/unit/
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.3.3/test/unit/__init__.py
--rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-03-03 17:44:42.000000 c4m_flexcell-0.3.3/test/unit/test_library.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       96 2022-07-12 15:00:24.000000 c4m_flexcell-0.4.0.dev3/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1264 2023-06-24 18:59:02.000000 c4m_flexcell-0.4.0.dev3/.gitlab-ci.yml
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      484 2020-07-06 13:05:29.000000 c4m_flexcell-0.4.0.dev3/COPYRIGHT.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      782 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSE.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.509446 c4m_flexcell-0.4.0.dev3/LICENSES/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    34523 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSES/agpl-3.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    13419 2020-07-06 09:58:12.000000 c4m_flexcell-0.4.0.dev3/LICENSES/cern_ohl_s_v2.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    18009 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/LICENSES/gpl-2.0.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     3878 2023-06-24 18:59:02.000000 c4m_flexcell-0.4.0.dev3/README.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/ReleaseNotes/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      321 2021-03-14 14:00:41.000000 c4m_flexcell-0.4.0.dev3/ReleaseNotes/v0.0.4.md
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      462 2022-08-22 13:25:11.000000 c4m_flexcell-0.4.0.dev3/ReleaseNotes/v0.1.0.md
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/c4m/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      149 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/c4m/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2247 2021-05-15 12:46:28.000000 c4m_flexcell-0.4.0.dev3/c4m/cell_canvas.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.513446 c4m_flexcell-0.4.0.dev3/c4m/flexcell/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      129 2023-05-26 12:28:32.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   509363 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/_cells.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    89759 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/activecolumnscell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    11848 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/canvas.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4297 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/cell.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)   126383 2023-06-24 19:24:29.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/factory.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)    52730 2023-05-09 10:49:53.000000 c4m_flexcell-0.4.0.dev3/c4m/flexcell/stdcell.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     4355 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/PKG-INFO
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)      764 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/SOURCES.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        1 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/dependency_links.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       28 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/requires.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        4 2023-06-24 19:34:06.000000 c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/top_level.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)        6 2022-11-01 15:19:21.000000 c4m_flexcell-0.4.0.dev3/ci-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       61 2022-09-30 12:33:15.000000 c4m_flexcell-0.4.0.dev3/dev-requirements.txt
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2133 2023-06-24 16:45:30.000000 c4m_flexcell-0.4.0.dev3/dodo.py
+-rwxrwxr-x   0 verhaegs   (500) verhaegs   (500)      165 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/run_unittests.sh
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       38 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/setup.cfg
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     1387 2023-06-24 19:24:22.000000 c4m_flexcell-0.4.0.dev3/setup.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/test/__init__.py
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/interactive/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       16 2020-07-14 09:04:04.000000 c4m_flexcell-0.4.0.dev3/test/interactive/.gitignore
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2683 2020-10-06 14:32:17.000000 c4m_flexcell-0.4.0.dev3/test/interactive/export.ipynb
+drwxrwxr-x   0 verhaegs   (500) verhaegs   (500)        0 2023-06-24 19:34:06.517446 c4m_flexcell-0.4.0.dev3/test/unit/
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)       84 2021-03-14 14:00:40.000000 c4m_flexcell-0.4.0.dev3/test/unit/__init__.py
+-rw-rw-r--   0 verhaegs   (500) verhaegs   (500)     2762 2023-03-03 17:44:42.000000 c4m_flexcell-0.4.0.dev3/test/unit/test_library.py
```

### Comparing `c4m_flexcell-0.3.3/.gitlab-ci.yml` & `c4m_flexcell-0.4.0.dev3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/LICENSE.md` & `c4m_flexcell-0.4.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/LICENSES/agpl-3.0.txt` & `c4m_flexcell-0.4.0.dev3/LICENSES/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/LICENSES/cern_ohl_s_v2.txt` & `c4m_flexcell-0.4.0.dev3/LICENSES/cern_ohl_s_v2.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/LICENSES/gpl-2.0.txt` & `c4m_flexcell-0.4.0.dev3/LICENSES/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/PKG-INFO` & `c4m_flexcell-0.4.0.dev3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m_flexcell
-Version: 0.3.3
+Version: 0.4.0.dev3
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
@@ -15,15 +15,14 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
-* v0.3.3: bug fix; remove public 0.3.2 release
 * v0.3.2: code cleansing, bug fixing, update dependencies
 * v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
@@ -33,9 +32,11 @@
 Alternative implementations try to fully automate the layout generation out of the transistor netlist. Finding a good placement of the transistor for non-trivial logic cells is a hard problem leading often to complex code for finding acceptable solutions. Also the layout code itself often becomes complex to take peculiarities of different design rules into account.  
 The `flexcell` library tries to take a middle road. It will start from a topological layout of the cell but without the layout already fixed to certain design rules; it thus avoid the step where netlist need to be converted to topologies. It will use the design rules from a PDKMaster Technology object to generate an optimized layout for conforming to the cells topology. By baking in independence of the Technology the standard cell library should be easily ported to different technologies with better area efficiency than current [lambda rules](http://www.electronics-tutorial.net/Digital-CMOS-Design/CMOS-Layout-Design/CMOS-lambda-Design-Rules/) based solutions.  
 In future options are planned so libraries can be generated for different targets like ,minimum area, maximum performance or minimum power consumption.
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever.  
+This development is done in a development branch for new layout generation code.
+When this development is done it will be released as version 0.4.0.  
 Current implementation is based on the topology of the Coriolis nsxlib standard cells with some area improvements but not yet with optimal area use. For v0.1 of this library a total replacement of the layout generation is planned fully based on minimized area for the technology design rules.  
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
```

### Comparing `c4m_flexcell-0.3.3/README.md` & `c4m_flexcell-0.4.0.dev3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
-* v0.3.3: bug fix; remove public 0.3.2 release
 * v0.3.2: code cleansing, bug fixing, update dependencies
 * v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
@@ -20,9 +19,11 @@
 Alternative implementations try to fully automate the layout generation out of the transistor netlist. Finding a good placement of the transistor for non-trivial logic cells is a hard problem leading often to complex code for finding acceptable solutions. Also the layout code itself often becomes complex to take peculiarities of different design rules into account.  
 The `flexcell` library tries to take a middle road. It will start from a topological layout of the cell but without the layout already fixed to certain design rules; it thus avoid the step where netlist need to be converted to topologies. It will use the design rules from a PDKMaster Technology object to generate an optimized layout for conforming to the cells topology. By baking in independence of the Technology the standard cell library should be easily ported to different technologies with better area efficiency than current [lambda rules](http://www.electronics-tutorial.net/Digital-CMOS-Design/CMOS-Layout-Design/CMOS-lambda-Design-Rules/) based solutions.  
 In future options are planned so libraries can be generated for different targets like ,minimum area, maximum performance or minimum power consumption.
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever.  
+This development is done in a development branch for new layout generation code.
+When this development is done it will be released as version 0.4.0.  
 Current implementation is based on the topology of the Coriolis nsxlib standard cells with some area improvements but not yet with optimal area use. For v0.1 of this library a total replacement of the layout generation is planned fully based on minimized area for the technology design rules.  
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
```

### Comparing `c4m_flexcell-0.3.3/c4m/cell_canvas.ipynb` & `c4m_flexcell-0.4.0.dev3/c4m/cell_canvas.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/c4m/flexcell/_cells.py` & `c4m_flexcell-0.4.0.dev3/c4m/flexcell/_cells.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,3289 +1,65 @@
 # SPDX-License-Identifier: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 from .stdcell import StdCell, Wire, Via, Device
 
 _cells = [
-    StdCell(
-        name='a2_x2', width=80, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_net0_ndif1",
-                    space={"bottom": "vssrail"}, conn={"right": "n_i0_1"},
-                ),
-                Wire('METAL1', (10, 30), 40, 6, False, name="m1_net0_1"),
-                Wire(
-                    'METAL1', 30, (60, 100), 6, False,
-                    conn={"top": "v_net0_pdif1", "bottom": "m1_net0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 30, 160, 2, name="v_net0_pdif1",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_i0_1", "right": "p_i1_1"},
-                ),
-                Via('POLY', 'METAL1', 32, 80, 2, conn={"right": "pl_net0_1"}),
-                Device(
-                    'nmos', 60, 31, 4, 38, 'vertical', name="n_net0_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 80, 'vertical', name="p_net0_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 60, (60, 100), 4, False, name="pl_net0_1",
-                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
-                ),
-            ],
-            '_net1': [
-                Wire(
-                    'NDIF', 30, (16, 46), 12, False,
-                    conn={"left": "n_i0_1", "right": "n_i1_1"},
-                ),
-            ],
-            'i0': [
-                Device(
-                    'nmos', 20, 50, 4, 38, 'vertical', name="n_i0_1",
-                    source_net='_net0', drain_net='_net1',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='vdd', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 20, (60, 100), False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "pl_i0_1"}),
-                Wire(
-                    'METAL1', 10, (62, 138), 6, True,
-                    space={"top": "vddrail", "bottom": "v_net0_ndif1"},
-                ),
-            ],
-            'i1': [
-                Device(
-                    'nmos', 40, 31, 4, 38, 'vertical', name="n_i1_1",
-                    source_net='_net1', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 48, 60, 2, conn={"left": "n_i1_1"}),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Via('POLY', 'METAL1', 48, 100, 2, conn={"left": "p_i1_1"}),
-                Wire(
-                    'METAL1', 50, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2,
-                    space={"bottom": "vssrail"}, conn={"left": "n_net0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2,
-                    space={"top": "vddrail"}, conn={"left": "p_net0_1"},
-                ),
-                Wire(
-                    'METAL1', 70, (60, 100), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_i0_1"}),
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 50, 182, 2,
-                    conn={"left": "p_i1_1", "right": "p_net0_1", "up": "vddrail"},
-                ),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 50, 18, 2,
-                    conn={"left": "n_i1_1", "right": "n_net0_1", "up": "vssrail"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='a3_x2', width=100, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'NDIF', 30, (40, 50), 3, False,
-                    conn={"left": "n_i0_1", "right": "n_i1_1"},
-                )
-            ],
-            '_net1': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2,
-                    space={"top": "m1_i0_i"}, conn={"right": "n_i0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 160, 2,
-                    space={"bottom": "m1_i0_i"}, conn={"right": "p_i0_1"},
-                ),
-                Wire('METAL1', (10, 70), 40, 3, False, name="m1_net1_1"),
-                Wire('METAL1', (10, 70), 160, 3, False, name="m1_net1_2"),
-                Via(
-                    'PDIF', 'METAL1', 50, 160, 2, space={"bottom": "m1_i2_i"},
-                    conn={"left": "p_i1_1", "right": "p_i2_1"},
-                ),
-                Wire(
-                    'METAL1', 70, (60, 100), 3, False, name="m1_net1_3",
-                    conn={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 72, 80, 2, conn={"right": "pl_net1_1"}),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net1_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net1_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 80, (56, 104), 4, False, name="pl_net1_1",
-                    conn={"top": "p_net1_1", "bottom": "n_net1_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 50, (40, 50), 3, False,
-                    conn={"left": "n_i1_1", "right": "n_i2_1"},
-                )
-            ],
-            'i0': [
-                Wire('METAL1', 10, (50, 150), 6, True, name="m1_i0_i"),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 20, 50, 4, 40, 'vertical', name="n_i0_1",
-                    source_net='_net1', drain_net='_net0',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='_net1', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 20, (76, 124), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (62, 120), 6, True,
-                    space={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 32, 100, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 50, 4, 40, 'vertical', name="n_i1_1",
-                    source_net='_net0', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='vdd', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 40, (76, 122), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire(
-                    'METAL1', 50, (60, 150), 3, True, name="m1_i2_i",
-                    space={"bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 52, 100, 2, conn={"right": "pl_i2_1"}),
-                Device(
-                    'nmos', 60, 50, 4, 40, 'vertical', name="n_i2_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 40, 'vertical', name="p_i2_1",
-                    source_net='_net1', drain_net='vdd',
-                ),
-                Wire('POLY', 60, (60, 100), 4, False, name="pl_i2_1",
-                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net1_1"},
-                ),
-                Wire(
-                    'METAL1', 90, (60, 100), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via(
-                    'PDIF', 'METAL1', 30, 182, 2,
-                    conn={"left": "p_i0_1", "right": "p_i1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 182, 2,
-                    conn={"left": "p_i2_1", "right": "p_net1_1", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 50, 184, 2),
-                Wire('NTIE', 50, (180, 188), 8, False),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 70, 18, 2,
-                    conn={"left": "n_i2_1", "right": "n_net1_1", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 50, 14, 2),
-                Wire('PTIE', 50, (10, 18), 8, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='a4_x2', width=120, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'NDIF', 50, (34, 66), 4, False,
-                    conn={"left": "n_i1_1", "right": "n_i2_1"},
-                ),
-            ],
-            '_net1': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, space={"top": "m1_i0_i"},
-                    conn={"right": "n_i0_1"},
-                ),
-                Wire('METAL1', (10, 90), 40, 6, False, name="m1_net1_1"),
-                Via(
-                    'PDIF', 'METAL1', 30, 160, 2, space={"bottom": "m1_i1_i"},
-                    conn={"left": "p_i0_1", "right": "p_i1_1"},
-                ),
-                Wire('METAL1', (30, 90), 160, 6, False, name="m1_net1_2"),
-                Via(
-                    'PDIF', 'METAL1', 70, 160, 2, space={"bottom": "m1_i3_i"},
-                    conn={"left": "p_i2_1", "right": "p_i3_1"},
-                ),
-                Wire(
-                    'METAL1', 90, (42, 138), 6, False,
-                    conn={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 92, 90, 2, conn={"right": "pl_net1_1"}),
-                Device(
-                    'nmos', 100, 31, 4, 38, 'vertical', name="n_net1_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 80, 'vertical', name="p_net1_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 100, (60, 100), 4, False, name="pl_net1_1",
-                    conn={"top": "p_net1_1", "bottom": "n_net1_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 70, (34, 66), 4, False,
-                    conn={"left": "n_i2_1", "right": "n_i3_1"},
-                ),
-            ],
-            '_net3': [
-                Wire(
-                    'NDIF', 30, (34, 66), 4, False,
-                    conn={"left": "n_i0_1", "right": "n_i1_1"},
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 10, (50, 118), 6, True, name="m1_i0_i",
-                    space={"top": "vddrail"},
-                ),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 20, 50, 4, 40, 'vertical', name="n_i0_1",
-                    source_net='_net1', drain_net='_net3',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='vdd', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 20, (76, 124), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (50, 150), 6, True, name="m1_i1_i",
-                    space={"bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 32, 120, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 50, 4, 40, 'vertical', name="n_i1_1",
-                    source_net='_net3', drain_net='_net0',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='_net1', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 40, (76, 124), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire(
-                    'METAL1', 50, (50, 118), 6, True, name="m1_i2_i",
-                    space={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 52, 100, 2, conn={"right": "pl_i2_1"}),
-                Device(
-                    'nmos', 60, 50, 4, 40, 'vertical', name="n_i2_1",
-                    source_net='_net0', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 40, 'vertical', name="p_i2_1",
-                    source_net='vdd', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 60, (98, 124), 4, False, name="pl_i2_1",
-                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
-                ),
-            ],
-            'i3': [
-                Wire(
-                    'METAL1', 70, (50, 150), 6, True, name="m1_i3_i",
-                    space={"bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 72, 80, 2, conn={"right": "pl_i3_1"}),
-                Device(
-                    'nmos', 80, 50, 4, 40, 'vertical', name="n_i3_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 40, 'vertical', name="p_i3_1",
-                    source_net='_net1', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 80, (80, 124), 4, False, name="pl_i3_1",
-                    conn={"top": "p_i3_1", "bottom": "n_i3_1"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 110, 40, 2, name="v_q_ndif1",
-                    space={"bottom": "vssrail"}, conn={"left": "n_net1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 110, 140, 2, name="v_q_pdif1",
-                    space={"top": "vddrail"}, conn={"left": "p_net1_1"},
-                ),
-                Wire(
-                    'METAL1', 110, (60, 100), 6, True,
-                    space= {"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_i0_1"}),
-                Via(
-                    'PDIF', 'METAL1', 50, 182, 2,
-                    conn={"left": "p_i1_1", "right": "p_i2_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 182, 2,
-                    conn={"left": "p_i3_1", "right": "p_net1_1", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 8, False),
-                Via('NTIE', 'METAL1', 70, 184, 2),
-                Wire('NTIE', 70, (180, 188), 8, False),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 90, 18, 2,
-                    conn={"left": "n_i3_1", "right": "n_net1_1", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 30, 14, 2),
-                Wire('PTIE', 30, (10, 18), 8, False),
-                Via('PTIE', 'METAL1', 70, 14, 2),
-                Wire('PTIE', 70, (10, 18), 8, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='ao22_x2', width=100, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'NDIF', 'METAL1', 30, 60, 2, name="v_net0_ndif1",
-                    space={"top": "m1_i1_1", "bottom": "vssrail"},
-                    conn={"left": "n_i0_1", "right": "n_i1_1"},
-                ),
-                Wire(
-                    'METAL1', (30, 50), 60, 3, False, name="m1_net0_1",
-                    conn={"left": "v_net0_ndif1"},
-                ),
-                Wire(
-                    'METAL1', 50, (60, 100), 3, False,
-                    conn={"top": "v_net0_pdif1", "bottom": "m1_net0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 50, 140, 2, name="v_net0_pdif1",
-                    conn={"left": "p_i1_1", "right": "p_i2_1"},
-                ),
-                Via('POLY', 'METAL1', 52, 80, 2, conn={"right": "pl_net0_1"}),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 80, (56, 104), 4, False, name="pl_net0_1",
-                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
-                ),
-            ],
-            '_net1': [
-                Wire(
-                    'PDIF', 30, (130, 162), 3, False,
-                    conn={"left": "p_i0_1", "right": "p_i1_1"},
-                ),
-            ],
-            '_net2': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_net2_ndif1",
-                    conn={"right": "n_i0_1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2,
-                    conn={"left": "n_i1_1", "right": "n_i2_1"},
-                ),
-                Wire('METAL1', (10, 50), 40, 6, False),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 10, (82, 138), 6, True,
-                    space={"top": "vddrail", "bottom": "v_net2_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='_net2', drain_net='_net0',
-                ),
-                Device(
-                    'pmos', 20, 146, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='vdd', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 20, (56, 124), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (70, 158), 6, True, name="m1_i1_1",
-                    space={"top": "vddrail"},
-                ),
-                Via('POLY', 'METAL1', 32, 100, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i1_1",
-                    source_net='_net0', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 40, 146, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='_net1', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 40, (56, 104), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire(
-                    'METAL1', 70, (62, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"}
-                ),
-                Via('POLY', 'METAL1', 68, 60, 2, conn={"left": "n_i2_1"}),
-                Via('POLY', 'METAL1', 68, 100, 2, conn={"left": "p_i2_1"}),
-                Device(
-                    'nmos', 60, 40, 4, 20, 'vertical', name="n_i2_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 60, 146, 4, 40, 'vertical', name="p_i2_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 90, (42, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net0_1"},
-                ),
-            ],
-            'vdd': [
-                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_i0_1"}),
-                Via(
-                    'PDIF', 'METAL1', 70, 182, 2,
-                    conn={"left": "p_i2_1", "right": "p_net0_1", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 50, 184, 2),
-                Wire('NTIE', 50, (180, 188), 10, False),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 70, 18, 2,
-                    conn={"left": "n_i2_1", "right": "n_net0_1", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 50, 14, 2),
-                Wire('PTIE', 50, (10, 18), 10, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='mx2_x2', width=140, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'NDIF', 90, (35, 45), 4, False,
-                    conn={"left": "n_cmd_2", "right": "n_i1_1"},
-                ),
-            ],
-            '_net1': [
-                Device(
-                    'nmos', 120, 31, 4, 38, 'vertical', name="n_net1_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 120, 150, 4, 80, 'vertical', name="p_net1_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 120, (56, 104), 4, False, name="pl_net1_1",
-                    conn={"top": "p_net1_1", "bottom": "n_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 72, 100, 2, conn={"right": "pl_net1_1"}),
-                Via(
-                    'NDIF', 'METAL1', 70, 60, 2, name="v_net1_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_net5_1", "right": "n_cmd_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2, name="v_net1_pdif1",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_cmd_2", "right": "p_net5_1"},
-                ),
-                Wire(
-                    'METAL1', 70, (80, 120), 6, False,
-                    conn={"top": "v_net1_pdif1", "bottom": "v_net1_ndif1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 50, (15, 25), 4, False,
-                    conn={"left": "n_i0_1", "right": "n_net5_1"},
-                ),
-            ],
-            '_net3': [
-                Wire(
-                    'PDIF', 50, (134, 166), 4, False,
-                    conn={"left": "p_i0_1", "right": "p_cmd_2"},
-                ),
-            ],
-            '_net4': [
-                Wire(
-                    'PDIF', 90, (134, 166), 4, False,
-                    conn={"left": "p_net5_1", "right": "p_i1_1"},
-                ),
-            ],
-            '_net5': [
-                Via('NDIF', 'METAL1', 10, 40, 2, conn={"right": "n_cmd_1"}),
-                Via('PDIF', 'METAL1', 10, 140, 2, conn={"right": "p_cmd_1"}),
-                Wire('METAL1', 10, (40, 140), 6, False, name="m1_net5_1"),
-                Wire(
-                    'METAL1', (10, 80), 40, 6, False, name="m1_net5_2",
-                    conn={"left": "m1_net5_1", "right": "m1_net5_3"},
-                ),
-                Via('POLY', 'METAL1', 58, 40, 2, conn={"right": "n_net5_1"}),
-                Device(
-                    'nmos', 60, 21, 4, 18, 'vertical', name="n_net5_1",
-                    source_net='_net2', drain_net='_net1',
-                ),
-                Via(
-                    'POLY', 'METAL1', 83, 120, 2, name="v_net5_pl1",
-                    conn={"left": "p_net5_1"},
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 40, 'vertical', name="p_net5_1",
-                    source_net='_net1', drain_net='_net4',
-                ),
-                Wire(
-                    'METAL1', 85, (40, 106), 6, False, name="m1_net5_3",
-                    conn={"top": "v_net5_pl1"},
-                ),
-            ],
-            'cmd': [
-                Device(
-                    'nmos', 20, 21, 4, 18, 'vertical', name="n_cmd_1",
-                    source_net='_net5', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_cmd_1",
-                    source_net='_net5', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 20, (52, 124), 4, False, name="pl_cmd_1",
-                    conn={"top": "p_cmd_1", "bottom": "n_cmd_1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 50, 80, 2,
-                    conn={"left": "pl_cmd_1", "right": "n_cmd_2"}
-                ),
-                Wire(
-                    'METAL1', 50, (62, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "m1_net5_2"},
-                ),
-                Wire('POLY', 60, (80, 120), 4, False, conn={"top": "p_cmd_2"}),
-                Device(
-                    'pmos', 60, 150, 4, 40, 'vertical', name="p_cmd_2",
-                    source_net='_net3', drain_net='_net1',
-                ),
-                Device(
-                    'nmos', 80, 41, 4, 18, 'vertical', name="n_cmd_2",
-                    source_net='_net1', drain_net='_net0',
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 30, (62, 138), 6, True,
-                    space={"top": "vddrail", "bottom": "m1_net5_2"},
-                ),
-                Device(
-                    'nmos', 40, 21, 4, 18, 'vertical', name="n_i0_1",
-                    source_net='vss', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='vdd', drain_net='_net3',
-                ),
-                Via('POLY', 'METAL1', 32, 60, 2, conn={"right": "n_i0_1"}),
-                Via('POLY', 'METAL1', 32, 120, 2, conn={"right": "p_i0_1"}),
-            ],
-            'i1': [
-                Device(
-                    'nmos', 100, 41, 4, 18, 'vertical', name="n_i1_1",
-                    source_net='_net0', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='_net4', drain_net='vdd',
-                ),
-                Wire(
-                    'METAL1', 110, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 108, 60, 2, conn={"left": "n_i1_1"}),
-                Wire('METAL1', (100, 110), 120, 3, conn={"left": "v_i1_pl1"}),
-                Via(
-                    'POLY', 'METAL1', 98, 120, 2, name="v_i1_pl1",
-                    conn={"right": "p_i1_1"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 130, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 130, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net1_1"},
-                ),
-                Wire(
-                    'METAL1', 130, (42, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via(
-                    'PDIF', 'METAL1', 30, 182, 2,
-                    conn={"left": "p_cmd_1", "right": "p_i0_1"}
-                ),
-                Via('NTIE', 'METAL1', 90, 184, 2),
-                Wire('NTIE', 90, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 110, 182, 2,
-                    conn={"left": "p_i1_1", "right": "p_net1_1", "up": "vddrail"},
-                ),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 30, 18, 2,
-                    conn={"left": "n_cmd_1", "right": "n_i0_1", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 90, 14, 2),
-                Wire('PTIE', 90, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 110, 18, 2,
-                    conn={"left": "n_i1_1", "right": "n_net1_1", "up": "vssrail"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='mx3_x2', width=220, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'PDIF', 'METAL1', 30, 160, 2, name="v_net0_pdif1",
-                    space={"top": "vddrail"}, conn={"right": "p_i2_1"},
-                ),
-                Wire(
-                    'METAL1', (30, 110), 160, 6, False, name="m1_net0_1",
-                    # conn={"left": "v_net0_pdif1", "right": "v_net0_pdif2"},
-                ),
-                Via('PDIF', 'METAL1', 110, 160, 2, name="v_net0_pdif2",
-                    space={"top": "vddrail", "bottom": "m1_net5_1"},
-                    conn={"left": "p_i1_1", "right": "p_net4_1"},
-                ),
-            ],
-            '_net1': [
-                Via(
-                    'NDIF', 'METAL1', 30, 40, 2, name="v_net1_ndif1",
-                    space={"bottom": "vssrail"}, conn={"right": "n_i2_1"},
-                ),
-                Wire(
-                    'METAL1', (30, 110), 40, 6, False,
-                    conn={"left": "v_net1_ndif1", "right": "v_net1_ndif2"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 110, 40, 2, name="v_net1_ndif2",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_i1_1", "right": "n_cmd0_2"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'PDIF', 150, (154, 186), 4, False,
-                    conn={"left": "p_cmd0_2", "right": "p_i0_1"},
-                ),
-            ],
-            '_net3': [
-                Via(
-                    'NDIF', 'METAL1', 30, 64, 2, name="v_net3_ndif1",
-                    conn={"left": "n_cmd1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 30, 120, 2, name="v_net3_pdif1",
-                    space={"top": "m1_cmd1_1"}, conn={"left": "p_cmd1_1"},
-                ),
-                Wire(
-                    'METAL1', 30, (80, 100), 3, False, name="m1_net3_1",
-                    conn={"top": "v_net3_pdif1", "bottom": "v_net3_ndif1"},
-                ),
-                Wire(
-                    'METAL1', (36, 60), 60, 6, False, name="m1_net3_2",
-                    conn={"left": "v_net3_ndif1", "right": "v_net3_pl1"},
-                ),
-                Wire(
-                    'METAL1', (36, 70), 120, 6, False, name="m1_net3_3",
-                    conn={"left": "v_net3_pdif1", "right": "v_net3_pl2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 58, 60, 2, name="v_net3_pl1",
-                    conn={"right": "n_net3_1"},
-                ),
-                Device(
-                    'nmos', 60, 34, 4, 24, 'vertical', name="n_net3_1",
-                    source_net='_net9', drain_net='_net5',
-                ),
-                Via(
-                    'POLY', 'METAL1', 75, 120, 2, name="v_net3_pl2",
-                    conn={"right": "p_net3_1"},
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 40, 'vertical', name="p_net3_1",
-                    source_net='_net5', drain_net='_net6',
-                ),
-            ],
-            '_net4': [
-                Via(
-                    'NDIF', 'METAL1', 170, 64, 2, name="v_net4_ndif1",
-                    conn={"right": "n_cmd0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 170, 120, 2, name="v_net4_pdif1",
-                    space={"top": "m1_net5_1"}, conn={"right": "p_cmd0_1"},
-                ),
-                Wire(
-                    'METAL1', 170, (80, 100), 6, False,
-                    conn={"top": "v_net4_pdif1", "bottom": "v_net4_ndif1"},
-                ),
-                Device(
-                    'nmos', 140, 26, 4, 24, 'vertical', name="n_net4_1",
-                    source_net='vss', drain_net='_net7',    
-                ),
-                Device(
-                    'pmos', 120, 170, 4, 40, 'vertical', name="p_net4_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Via(
-                    'POLY', 'METAL1', 142, 60, 2, name="v_net4_pl1",
-                    conn={"left": "p_net4_1"},
-                ),
-                Wire(
-                    'METAL1', (140, 170), 60, 6, False, name="m1_net4_1",
-                    conn={"left":"v_net4_pl1", "right": "v_net4_ndif1"},
-                ),
-                Wire(
-                    'POLY', 140, (40, 60), False,
-                    conn={"top": "v_net4_pl1", "bottom": "n_net4_1"},
-                )
-            ],
-            '_net5': [
-                Device(
-                    'nmos', 200, 50, 4, 40, 'vertical', name="n_net5_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 200, 150, 4, 80, 'vertical', name="p_net5_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 200, (76, 104), 4, False, name="pl_net5_1",
-                    conn={"top": "p_net5_1", "bottom": "n_net5_1"},
-                ),
-                Via('POLY', 'METAL1', 192, 80, 2, conn={"right": "pl_net5_1"}),
-                Wire(
-                    'METAL1', 190, (42, 138), 6, False,
-                    conn={"top": "m1_net5_1", "bottom": "m1_net5_2"},
-                ),
-                Wire(
-                    'METAL1', (84, 190), 140, 6, False, name="m1_net5_1",
-                    conn={"left": "v_net5_pdif1"},
-                ),
-                Wire(
-                    'METAL1', (170, 190), 40, 6, False, name="m1_net5_2",
-                    conn={"left": "v_net5_ndif2"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 170, 34, 2, name="v_net5_ndif2",
-                    space={"bottom": "vssrail"}, conn={"left": "n_i0_1"},
-                ),
-                Wire(
-                    'METAL1', 170, (142, 158), 6, False,
-                    conn={"top": "v_net5_pdif2", "bottom": "m1_net5_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 170, 160, 2, name="v_net5_pdif2",
-                    space={"top": "vddrail"}, conn={"left": "p_i0_1"},
-                ),
-                Wire(
-                    'METAL1', 90, (62, 78), 6, False,
-                    conn={"top": "m1_net5_1", "bottom": "m1_net5_3"},
-                ),
-                Wire(
-                    'METAL1', (70, 90), 60, 6, False, name="m1_net5_3",
-                    conn={"left": "v_net5_ndif1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 70, 60, 2, name="v_net5_ndif1",
-                    conn={"left": "n_net3_1", "right": "n_cmd1_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2, name="v_net5_pdif1",
-                    space={"top": "m1_net0_1"},
-                    conn={"left": "p_cmd1_2", "right": "p_net3_1"},
-                ),
-            ],
-            '_net6': [
-                Wire(
-                    'PDIF', 90, (134, 166), 4, False,
-                    conn={"left": "p_net3_1", "right": "p_i1_1"},
-                ),
-            ],
-            '_net7': [
-                Wire(
-                    'NDIF', 150, (26, 36), 8, False,
-                    conn={"left": "n_net4_1", "right": "n_i0_1"},
-                ),
-            ],
-            '_net8': [
-                Wire(
-                    'PDIF', 50, (154, 186), 4, False,
-                    conn={"left": "p_i2_1", "right": "p_cmd1_2"},
-                ),
-            ],
-            '_net9': [
-                Wire(
-                    'NDIF', 50, (26, 42), 8, False,
-                    conn={"left": "n_i2_1", "right": "n_net3_1"},
-                ),
-            ],
-            '_net10': [
-                Wire(
-                    'NDIF', 90, (36, 52), 8, False,
-                    conn={"left": "n_cmd1_2", "right": "n_i1_1"},
-                ),
-            ],
-            'cmd0': [
-                Device(
-                    'nmos', 180, 64, 4, 12, 'vertical', name="n_cmd0_1",
-                    source_net='_net4', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 180, 124, 4, 28, 'vertical', name="p_cmd0_1",
-                    source_net='_net4', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 180, (76, 104), 4, False, name="pl_cmd0_1",
-                    conn={"top": "p_cmd0_1", "bottom": "n_cmd0_1"},
-                ),
-                Device(
-                    'pmos', 140, 170, 4, 40, 'vertical', name="p_cmd0_2",
-                    source_net='vdd', drain_net='_net2',
-                ),
-                Wire(
-                    'POLY', 140, (100, 140), 2, False,
-                    conn={"top": "p_cmd0_2"},
-                ),
-                Wire(
-                    'METAL1', 130, (82, 118), 6, True,
-                    space={"top": "m1_net5_1", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 132, 100, 2, conn={"right": "pl_cmd0_1"}),
-                Via('POLY', 'METAL1', 128, 45, 2, conn={"left": "n_cmd0_2"}),
-                Device(
-                    'nmos', 120, 26, 4, 24, 'vertical', name="n_cmd0_2",
-                    source_net='_net1', drain_net='vss',
-                ),
-            ],
-            'cmd1': [
-                Wire(
-                    'METAL1', 10, (62, 140), 6, True, name="m1_cmd1_i",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "pl_cmd1_1"}),
-                Device(
-                    'nmos', 20, 66, 4, 16, 'vertical', name="n_cmd1_1",
-                    source_net='vss', drain_net='_net3',
-                ),
-                Device(
-                    'pmos', 20, 124, 4, 28, 'vertical', name="p_cmd1_1",
-                    source_net='vdd', drain_net='_net3',
-                ),
-                Wire(
-                    'POLY', 20, (80, 104), 4, False, name="pl_cmd1_1",
-                    conn={"top": "p_cmd1_1", "bottom": "n_cmd1_1"},
-                ),
-                Wire(
-                    'METAL1', (12, 60), 140, 6, False, name="m1_cmd1_1",
-                    conn={"left": "m1_cmd1_i", "right": "v_cmd1_pl1"},
-                ),
-                Via('POLY', 'METAL1', 58, 140, 2, name="v_cmd1_pl1"),
-                Device(
-                    'pmos', 60, 170, 4, 40, 'vertical', name="p_cmd1_2",
-                    source_net='_net8', drain_net='_net5',
-                ),
-                Wire(
-                    'POLY', 60, (80, 140), 4, False,
-                    conn={"top": "p_cmd1_2", "bottom": "pl_cmd1_2"},
-                ),
-                Wire('POLY', (60, 80), 80, 4, False, name="pl_cmd1_2"),
-                Wire(
-                    'POLY', 80, (52, 80), 4, False,
-                    conn={"top": "pl_cmd1_2", "bottom": "n_cmd1_2"},
-                ),
-                Device(
-                    'nmos', 80, 44, 4, 24, 'vertical', name="n_cmd1_2",
-                    source_net='_net5', drain_net='_net10',
-                ),
-            ],
-            'i0': [
-                Device(
-                    'nmos', 160, 26, 4, 24, 'vertical', name="n_i0_1",
-                    source_net='_net7', drain_net='_net5',
-                ),
-                Device(
-                    'pmos', 160, 170, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='_net2', drain_net='_net5',
-                ),
-                Via('POLY', 'METAL1', 152, 82, 2, conn={"right": "n_i0_1"}),
-                Via('POLY', 'METAL1', 152, 120, 2, conn={"right": "p_i0_1"}),
-                Wire(
-                    'METAL1', 150, (80, 120), 6, True,
-                    space={"top": "m1_net5_1", "bottom": "m1_net4_1"},
-                ),
-            ],
-            'i1': [
-                Device(
-                    'nmos', 100, 44, 4, 24, 'vertical', name="n_i1_1",
-                    source_net='_net10', drain_net='_net1',
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 40, 'vertical', name="p_i1_1",
-                    source_net='_net6', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 100, (52, 144), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-                Wire(
-                    'METAL1', 110, (80, 100), 3, True,
-                    space={"top": "m1_net5_1", "bottom": "v_net1_ndif2"},
-                ),
-                Via('POLY', 'METAL1', 108, 100, 2, conn={"left": "pl_i1_1"}),
-            ],
-            'i2': [
-                Device(
-                    'nmos', 40, 34, 4, 24, 'vertical', name="n_i2_1",
-                    source_net='_net1', drain_net='_net9',
-                ),
-                Device(
-                    'pmos', 40, 170, 4, 40, 'vertical', name="p_i2_1",
-                    source_net='_net0', drain_net='_net8',
-                ),
-                Wire(
-                    'POLY', 40, (52, 144), 4, False, name="pl_i2_1",
-                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
-                ),
-                Via('POLY', 'METAL1', 48, 100, 2, conn={"left": "pl_i2_1"}),
-                Wire(
-                    'METAL1', 50, (80, 100), 3, True,
-                    space={"top": "m1_net3_3", "bottom": "m1_net3_2"},
-                ),
-            ],
-            'q': [
-                Via('NDIF', 'METAL1', 210, 60, 2, conn={"left": "n_net5_1"}),
-                Via(
-                    'PDIF', 'METAL1', 210, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net5_1"},
-                ),
-                Wire(
-                    'METAL1', 210, (64, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_cmd1_1"}),
-                Via('NTIE', 'METAL1', 90, 184, 2),
-                Wire('NTIE', 90, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 130, 182, 2,
-                    conn={"left": "p_net4_1", "right": "p_cmd0_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 190, 182, 2, space={"bottom": "m1_net5_1"},
-                    conn={"left": "p_cmd0_1", "right": "p_net5_1"},
-                ),
-            ],
-            'vss': [
-                Via('NDIF', 'METAL1', 10, 18, 2, conn={"right": "n_cmd1_1"}),
-                Via('PTIE', 'METAL1', 90, 14, 2),
-                Wire('PTIE', 90, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 130, 18, 2,
-                    conn={"left": "n_cmd0_2", "right": "n_net4_1", "up": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 190, 18, 2,
-                    conn={"left": "n_cmd0_1", "right": "n_net5_1"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='nsnrlatch_x1', width=100, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'NDIF', 70, (40, 60), 4, False,
-                    conn={"left": "n_q_1", "right": "n_nrst_1"},
-                )
-            ],
-            '_net1': [
-                Wire(
-                    'NDIF', 30, (40, 60), 4, False,
-                    conn={"left": "n_nset_1", "right": "n_nq_1"},
-                )
-            ],
-            'nq': [
-                Device(
-                    'nmos', 40, 50, 4, 40, 'vertical', name="n_nq_1",
-                    source_net='_net1', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_nq_1",
-                    source_net='q', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 40, (76, 130), 2, False, name="pl_nq_1",
-                    space={}, conn={"top": "n_nq_1", "bottom": "p_nq_1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 42, 90, 2, name='v_nq_pl1',
-                    conn={"right": "pl_nq_1"},
-                ),
-                Wire(
-                    'METAL1', (50, 60), 90, 2,
-                    conn={"left": "v_nq_pl1", "right": "m1_nq_1"},
-                ),
-                Wire(
-                    'METAL1', 70, (40, 158), 3, True, name="m1_nq_1",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2,
-                    conn={"left": "p_q_1", "right": "p_nrst_1"},
-                ),
-                Wire('METAL1', (69, 91), 40, 6, False),
-                Via(
-                    'NDIF', 'METAL1', 90, 40, 2,
-                    space={"bottom": "vssrail"}, conn={"left": "n_nrst_1"},
-                ),
-            ],
-            'nrst': [
-                Device(
-                    'nmos', 80, 50, 4, 40, 'vertical', name="n_nrst_1",
-                    source_net='_net0', drain_net='nq',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 40, 'vertical', name="p_nrst_1",
-                    source_net='nq', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 80, (80, 124), 4, False, name="pl_nrst_1",
-                    space={}, conn={"top": "p_nrst_1", "bottom": "n_nrst_1"},
-                ),
-                Wire('METAL1', 90, (80, 138), 6, True, space={"top": "vddrail"}),
-                Via('POLY', 'METAL1', 88, 100, 2, conn={"left": "pl_nrst_1"}),
-            ],
-            'nset': [
-                Device(
-                    'nmos', 20, 50, 4, 40, 'vertical', name="n_nset_1",
-                    source_net='q', drain_net='_net1',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_nset_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 20, (80, 124), 4, False, name="pl_nset_1",
-                    space={}, conn={"top": "p_nset_1", "bottom": "n_nset_1"},
-                ),
-                Wire('METAL1', 10, (80, 138), 6, True, space={"top": "vddrail"}),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "pl_nset_1"}),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 30, (40, 158), 3, True, name="m1_q_1",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 30, 140, 2,
-                    conn={"left": "p_nset_1", "right": "p_nq_1"},
-                ),
-                Wire('METAL1', (9, 31), 40, 6, False),
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2,
-                    space={"bottom": "vssrail"}, conn={"right": "n_nset_1"},
-                ),
-                Device(
-                    'nmos', 60, 50, 4, 40, 'vertical', name="n_q_1",
-                    source_net='vss', drain_net='_net0',
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 40, 'vertical', name="p_q_1",
-                    source_net='vdd', drain_net='nq',
-                ),
-                Wire(
-                    'POLY', 60, (76, 130), 2, False, name="pl_q_1",
-                    space={}, conn={"top": "n_q_1", "bottom": "p_q_1"},
-                ),
-                Wire(
-                    'METAL1', (40, 50), 110, 2,
-                    conn={"left": "m1_q_1", "right": "v_q_pl1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 58, 110, 2, name="v_q_pl1",
-                    conn={"right": "pl_q_1"},
-                ),
-            ],
-            'vdd': [
-                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_nset_1"}),
-                Via(
-                    'PDIF', 'METAL1', 50, 160, 2, name="v_vdd_pdif1",
-                     conn={"left": "p_nq_1", "right": "p_q_1"},
-                ),
-                Wire(
-                    'METAL1', 50, (170, 180), 2,
-                    conn={"bottom": "v_vdd_pdif1", "top": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 10, False),
-                Via('NTIE', 'METAL1', 70, 184, 2),
-                Wire('NTIE', 70, (180, 188), 10, False),
-                Via('PDIF', 'METAL1', 90, 182, 2, conn={"left": "p_nrst_1"}),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 30, 14, 2),
-                Wire('PTIE', 30, (10, 18), 10, False),
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2, name="v_vss_ndif1",
-                    conn={"left": "n_nq_1", "right": "n_q_1"},
-                ),
-                Wire(
-                    'METAL1', 50, (20, 30), 2,
-                    conn={"bottom": "vssrail", "top": "v_vss_ndif1"},
-                ),
-                Via('PTIE', 'METAL1', 70, 14, 2),
-                Wire('PTIE', 70, (10, 18), 10, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='nxr2_x1', width=140, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_net0_ndif1",
-                    conn={"right": "n_i0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 140, 2, name="v_net0_pdif1",
-                    conn={"right": "p_i0_1"},
-                ),
-                Wire(
-                    'METAL1', 10, (60, 120), 3, False,
-                    conn={"top": "v_net0_pdif1", "bottom": "v_net0_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_net0_1"}),
-                Wire(
-                    'POLY', 80, (56, 104), 4, False, name="pl_net0_1",
-                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
-                ),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
-                    source_net='nq', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
-                    source_net='nq', drain_net='_net1',
-                ),
-            ],
-            '_net1': [
-                Via(
-                    'PDIF', 'METAL1', 50, 160, 2, name="v_net1_pdif1",
-                    space={"top": "vddrail", "bottom": "m1_nq_o"},
-                    conn={"left": "p_i0_2", "right": "p_i1_1"},
-                ),
-                Wire(
-                    'METAL1', (50, 90), 160, 6, False, name="m1_net1_1",
-                    conn={"left": "v_net1_pdif1", "right": "v_net1_pdif2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, name="v_net1_pdif2",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_net0_1", "right": "p_net3_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 90, (16, 46), 12, False,
-                    conn={"left": "n_net0_1", "right": "n_i1_1"},
-                ),
-            ],
-            '_net3': [
-                Via(
-                    'NDIF', 'METAL1', 130, 40, 2, name="v_net3_ndif1",
-                    conn={"left": "n_i1_2"},
-                ),
-                Via('PDIF', 'METAL1', 130, 140, 2, name="v_net3_pdif1",
-                    conn={"left": "p_i1_2"},
-                ),
-                Wire(
-                    'METAL1', 130, (60, 120), 3, False,
-                    conn={"top": "v_net3_pdif1", "bottom": "v_net3_ndif1"}
-                ),
-                Via(
-                    'POLY', 'METAL1', 128, 80, 2, name="v_net3_pl3",
-                    conn={"left": "p_net3_1"},
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 80, 'vertical', name="p_net3_1",
-                    source_net='_net1', drain_net='vdd',
-                ),
-                Via(
-                    'POLY', 'METAL1', 92, 80, 2, name="v_net3_pl1",
-                    conn={"right": "v_net3_pl3"},
-                ),
-                Wire(
-                    'METAL1', 90, (60, 80), 6, False, name="m1_net3_1",
-                    conn={"top": "v_net3_pl1"},
-                ),
-                Wire(
-                    'METAL1', (70, 90), 60, 6, False,
-                    conn={"left": "v_net3_pl2", "right": "m1_net3_1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 62, 60, 2, name="v_net3_pl2",
-                    conn={"left": "n_net3_1"}
-                ),
-                Device(
-                    'nmos', 60, 31, 4, 38, 'vertical', name="n_net3_1",
-                    source_net='_net4', drain_net='nq',
-                ),
-            ],
-            '_net4': [
-                Wire(
-                    'NDIF', 50, (16, 46), 4, False,
-                    conn={"left": "n_i0_2", "right": "n_net3_1"},
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 30, (60, 140), 3, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 30, 60, 2,
-                    conn={"left": "n_i0_1", "right": "n_i0_2"},
-                ),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='_net0', drain_net='vss',
-                ),
-                Device(
-                    'nmos', 40, 31, 4, 38, 'vertical', name="n_i0_2",
-                    source_net='vss', drain_net='_net4',
-                ),
-                Via(
-                    'POLY', 'METAL1', 30, 100, 2,
-                    conn={"left": "p_i0_1", "right": "p_i0_2"},
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 80, 'vertical', name="p_i0_2",
-                    source_net='vdd', drain_net='_net1',
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 110, (40, 140), 4, True, name="m1_i1_i",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 110, 60, 2,
-                    conn={"left": "n_i1_1", "right": "n_i1_2"},
-                ),
-                Device(
-                    'nmos', 100, 31, 4, 38, 'vertical', name="n_i1_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'nmos', 120, 40, 4, 20, 'vertical', name="n_i1_2",
-                    source_net='vss', drain_net='_net3',
-                ),
-                Wire(
-                    'METAL1', (70, 110), 100, 6, False,
-                    conn={"left": "v_i1_pl1", "right": "m1_i1_i"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 62, 100, 2, name="v_i1_pl1",
-                    conn={"left": "p_i1_1"},
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 80, 'vertical', name="p_i1_1",
-                    source_net='_net1', drain_net='nq',
-                ),
-                Via('POLY', 'METAL1', 112, 100, 2, conn={"right": "p_i1_2"}),
-                Device(
-                    'pmos', 120, 150, 4, 40, 'vertical', name="p_i1_2",
-                    source_net='vdd', drain_net='_net3',
-                ),
-            ],
-            'nq': [
-                Wire(
-                    'METAL1', 50, (40, 150), 6, True, name="m1_nq_o",
-                    space={"bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (50, 72), 40, 6, False,
-                    conn={"left": "m1_nq_o", "right": "v_nq_ndif1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, name="v_nq_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_net3_1", "right": "n_net0_1"},
-                ),
-                Wire(
-                    'METAL1', (50, 72), 140, 6, False,
-                    conn={"left": "m1_nq_o", "right": "v_nq_pdif1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2, name="v_nq_pdif1",
-                    space={"top": "m1_net1_1"},
-                    conn={"left": "p_i1_1", "right": "p_net0_1"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 10, 184, 2),
-                Wire('NTIE', 10, (180, 190), 6, False),
-                Via(
-                    'PDIF', 'METAL1', 30, 182, 2,
-                    conn={"left": "p_i0_1", "right": "p_i0_2", "up": "vddrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 110, 182, 2,
-                    conn={"left": "p_net3_1", "right": "p_i1_2", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 130, 184, 2),
-                Wire('NTIE', 130, (180, 190), 6, False),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 30, 18, 2,
-                    conn={"left": "n_i0_1", "right": "n_i0_2", "up": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 110, 18, 2,
-                    conn={"left": "n_i1_1", "right": "n_i1_2", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 130, 14, 2),
-                Wire('PTIE', 130, (8, 18), 6, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='o2_x2', width=80, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'PDIF', 30, (140, 160), 4, False,
-                    conn={"left": "p_i1_1", "right": "p_i0_1"},
-                )
-            ],
-            '_net1': [
-                Via(
-                    'PDIF', 'METAL1', 10, 160, 2, space={"bottom": "m1_i1_i"},
-                    conn={"right": "p_i1_1"},
-                ),
-                Wire('METAL1', (10, 30), 160, 6, False, name="m1_net1_1"),
-                Via(
-                    'NDIF', 'METAL1', 30, 40, 2, name="v_net1_ndif1",
-                    conn={"left": "n_i1_1", "right": "n_i0_1"},
-                ),
-                Wire(
-                    'METAL1', 30, (60, 160), 4, False,
-                    conn={"top": "m1_net1_1", "bottom": "v_net1_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 32, 80, 2, conn={"right": "pl_net1_1"}),
-                Device(
-                    'nmos', 60, 31, 4, 38, 'vertical', name="n_net1_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 80, 'vertical', name="p_net1_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 60, (56, 104), 4, False, name="pl_net1_1",
-                    conn={"top": "p_net1_1", "bottom": "n_net1_1"},
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 50, (42, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='_net1', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 48, 60, 2, conn={"left": "n_i0_1"}),
-                Device(
-                    'pmos', 40, 140, 4, 60, 'vertical', name="p_i0_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Via('POLY', 'METAL1', 48, 100, 2, conn={"left": "p_i0_1"}),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 10, (60, 150), 6, True, name="m1_i1_i",
-                    space={"bottom": "vssrail"}),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i1_1",
-                    source_net='vss', drain_net='_net1',
-                ),
-                Device(
-                    'pmos', 20, 140, 4, 60, 'vertical', name="p_i1_1",
-                    source_net='_net1', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 20, (56, 104), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 70, (40, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net1_1"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 50, 182, 2,
-                    conn={"left": "p_i0_1", "right": "p_net1_1", "up": "vddrail"},
-                ),
-            ],
-            'vss': [
-                Via('NDIF', 'METAL1', 10, 18, 2, conn={"right": "n_i1_1"}),
-                Via('PTIE', 'METAL1', 30, 14, 2),
-                Wire('PTIE', 30, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 50, 18, 2,
-                    conn={"left": "n_i0_1", "right": "n_net1_1", "up": "vssrail"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='o3_x2', width=100, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'PDIF', 30, (140, 160), 4, False,
-                    conn={"left": "p_i2_1", "right": "p_i1_1"},
-                )
-            ],
-            '_net1': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, space={"top": "m1_i2_i"},
-                    conn={"right": "n_i2_1"},
-                ),
-                Wire('METAL1', (10, 70), 40, 6, False, name="m1_net1_1"),
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2, space={"top": "m1_i0_i"},
-                    conn={"left": "n_i1_1", "right": "n_i0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 160, 2, space={"bottom": "m1_i2_i"},
-                    conn={"right": "p_i2_1"},
-                ),
-                Wire('METAL1', (10, 70), 160, 6, False, name="m1_net1_2"),
-                Wire(
-                    'METAL1', 70, (62, 158), 6, False,
-                    conn={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 72, 80, 2, conn={"right": "pl_net1_1"}),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net1_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net1_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 80, (56, 104), 4, False, name="pl_net1_1",
-                    conn={"top": "p_net1_1", "bottom": "n_net1_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'PDIF', 50, (140, 160), 4, False,
-                    conn={"left": "p_i1_1", "right": "p_i0_1"},
-                )
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 50, (50, 140), 6, True, name="m1_i0_i",
-                    space={"top": "m1_net1_2"},
-                ),
-                Via('POLY', 'METAL1', 52, 100, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 60, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='_net1', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 60, 140, 4, 60, 'vertical', name="p_i0_1",
-                    source_net='_net2', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 60, (56, 98), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (80, 140), 6, True, name="m1_i1_i",
-                    space={"top": "m1_net1_2", "bottom": "m1_net1_1"},
-                ),
-                Via('POLY', 'METAL1', 30, 60, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i1_1",
-                    source_net='vss', drain_net='_net1',
-                ),
-                Device(
-                    'pmos', 40, 140, 4, 60, 'vertical', name="p_i1_1",
-                    source_net='_net0', drain_net='_net2',
-                ),
-                Wire(
-                    'POLY', 40, (56, 104), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire('METAL1', 10, (50, 150), 6, True, name="m1_i2_i"),
-                Via('POLY', 'METAL1', 10, 80, 2, conn={"right": "pl_i2_1"}),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i2_1",
-                    source_net='_net1', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 20, 140, 4, 60, 'vertical', name="p_i2_1",
-                    source_net='_net1', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 20, (56, 104), 4, False, name="pl_i2_1",
-                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net1_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net1_1"},
-                ),
-                Wire(
-                    'METAL1', 90, (40, 160), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 10, 184, 2),
-                Wire('NTIE', 10, (180, 190), 6, False),
-                Via('NTIE', 'METAL1', 50, 184, 2),
-                Wire('NTIE', 50, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 70, 184, 2, space={"bottom": "m1_net1_2"},
-                    conn={"left": "p_i0_1", "right": "p_net1_1"},
-                ),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 30, 18, 2, space={"top": "m1_net1_1"},
-                    conn={"left": "n_i2_1", "right": "n_i1_1"},
-                ),
-                Via('PTIE', 'METAL1', 50, 14, 2),
-                Wire('PTIE', 50, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 70, 18, 2, space={"top": "m1_net1_1"},
-                    conn={"left": "n_i0_1", "right": "n_net1_1"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='o4_x2', width=120, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'PDIF', 70, (140, 160), 4, False,
-                    conn={"left": "p_i0_1", "right": "p_i2_1"},
-                )
-            ],
-            '_net1': [
-                Wire(
-                    'PDIF', 30, (140, 160), 4, False,
-                    conn={"left": "p_i3_1", "right": "p_i1_1"},
-                )
-            ],
-            '_net2': [
-                Via(
-                    'NDIF', 'METAL1', 30, 40, 2, name="v_net2_ndif1",
-                    space={"top": "m1_i1_i"},
-                    conn={"left": "n_i3_1", "right": "n_i1_1"},
-                ),
-                Wire('METAL1', (30, 90), 40, 3, False, name="m1_net2_1"),
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, name="v_net2_ndif2",
-                    space={"top": "m1_i2_i"},
-                    conn={"left": "n_i0_1", "right": "n_i2_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 160, 2, name="v_net2_pdif1",
-                    space={"bottom": "m1_i3_i"},
-                    conn={"right": "p_i3_1"},
-                ),
-                Wire('METAL1', (10, 90), 160, 6, False, name="m1_net2_2"),
-                Wire(
-                    'METAL1', 90, (60, 100), 3, False,
-                    conn={"top": "m1_net2_2", "bottom": "m1_net2_1"},
-                ),
-                Via('POLY', 'METAL1', 92, 80, 2, conn={"right": "pl_net2_1"}),
-                Device(
-                    'nmos', 100, 31, 4, 38, 'vertical', name="n_net2_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 80, 'vertical', name="p_net2_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 100, (60, 100), 4, False, name="pl_net2_1",
-                    conn={"top": "p_net2_1", "bottom": "n_net2_1"},
-                ),
-            ],
-            '_net3': [
-                Wire(
-                    'PDIF', 50, (140, 160), 4, False,
-                    conn={"left": "p_i1_1", "right": "p_i0_1"},
-                )
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 50, (82, 138), 6, True, name="m1_i0_i",
-                    space={"top": "m1_net2_2", "bottom": "m1_net2_1"},
-                ),
-                Via('POLY', 'METAL1', 52, 80, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 60, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='vss', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 60, 140, 4, 60, 'vertical', name="p_i0_1",
-                    source_net='_net3', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 60, (60, 100), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (50, 138), 3, True, name="m1_i1_i",
-                    space={"top": "m1_net2_2"},
-                ),
-                Via('POLY', 'METAL1', 32, 80, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i1_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 40, 140, 4, 60, 'vertical', name="p_i1_1",
-                    source_net='_net1', drain_net='_net3',
-                ),
-                Wire(
-                    'POLY', 40, (60, 100), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire(
-                    'METAL1', 70, (50, 138), 3, True, name="m1_i2_i",
-                    space={"top": "m1_net2_2"},
-                ),
-                Via('POLY', 'METAL1', 72, 80, 2, conn={"right": "pl_i2_1"}),
-                Device(
-                    'nmos', 80, 40, 4, 20, 'vertical', name="n_i2_1",
-                    source_net='_net2', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 80, 140, 4, 60, 'vertical', name="p_i2_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 80, (60, 100), 4, False, name="pl_i2_1",
-                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
-                ),
-            ],
-            'i3': [
-                Wire(
-                    'METAL1', 10, (62, 150), 3, True, name="m1_i3_i",
-                    space={"bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i3_1"}),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i3_1",
-                    source_net='vss', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 20, 140, 4, 60, 'vertical', name="p_i3_1",
-                    source_net='_net2', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 20, (60, 100), 4, False, name="pl_i3_1",
-                    conn={"top": "p_i3_1", "bottom": "n_i3_1"},
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 110, 40, 2,
-                    space={"bottom": "vssrail"}, conn={"left": "n_net2_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 110, 140, 2,
-                    space={"top": "vddrail"}, conn={"left": "p_net2_1"},
-                ),
-                Wire(
-                    'METAL1', 110, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 8, False),
-                Via('NTIE', 'METAL1', 70, 184, 2),
-                Wire('NTIE', 70, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 90, 184, 2, space={"bottom": "m1_net2_2"},
-                    conn={"left": "p_i2_1", "right": "p_net2_1"},
-                ),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 10, 18, 2,
-                    conn={"right": "n_i3_1"},
-                ),
-                Via('PTIE', 'METAL1', 30, 14, 2),
-                Wire('PTIE', 30, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 50, 18, 2,
-                    conn={"left": "n_i1_1", "right": "n_i0_1"},
-                ),
-                Via('PTIE', 'METAL1', 70, 14, 2),
-                Wire('PTIE', 70, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 90, 18, 2, space={"top": "m1_net2_1"},
-                    conn={"left": "n_i2_1", "right": "n_net2_1"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='oa22_x2', width=100, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'PDIF', 'METAL1', 30, 140, 2, name="v_net0_pdif1",
-                    space={"top": "m1_net1_1"},
-                    conn={"left": "p_i0_1", "right": "p_i1_1"},
-                ),
-                Wire(
-                    'METAL1', (30, 50), 140, 3, False, name="m1_net0_1",
-                    conn={"left": "v_net0_pdif1"},
-                ),
-                Wire(
-                    'METAL1', 50, (60, 100), 3, False,
-                    conn={"top": "m1_net0_1", "bottom": "v_net0_ndif1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2, name="v_net0_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_i1_1", "right": "n_i2_1"},
-                ),
-                Via('POLY', 'METAL1', 52, 80, 2, conn={"right": "pl_net0_1"}),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
-                   source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
-                   source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 80, (56, 104), 4, False, name="pl_net0_1",
-                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
-                ),
-            ],
-            '_net1': [
-                Via(
-                    'PDIF', 'METAL1', 10, 160, 2, name="v_net1_pdif1",
-                    space={"bottom": "m1_i0_i"}, conn={"right": "p_i0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 50, 160, 2, name="v_net1_pdif2",
-                    space={"bottom": "m1_net0_1"},
-                    conn={"left": "p_i1_1", "right": "p_i2_1"},
-                ),
-                Wire(
-                    'METAL1', (10, 50), 160, 6, False, name="m1_net1_1",
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 30, (36, 66), 8, False,
-                    conn={"left": "n_i0_1", "right": "n_i1_1"},
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 10, (42, 150), 6, True, name="m1_i0_i",
-                    space={"bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i0_1"}),
-                Device(
-                    'nmos', 20, 51, 4, 38, 'vertical', name="n_i0_1",
-                   source_net='vss', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                   source_net='_net1', drain_net='_net0',
-                ),
-                Wire(
-                    'POLY', 20, (60, 100), 4, False, name="pl_i0_1",
-                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 30, (42, 118), 6, True,
-                    space={"top": "v_net0_pdif1", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 32, 100, 2, conn={"right": "pl_i1_1"}),
-                Device(
-                    'nmos', 40, 51, 4, 38, 'vertical', name="n_i1_1",
-                   source_net='_net2', drain_net='_net0',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_i1_1",
-                   source_net='_net0', drain_net='_net1',
-                ),
-                Wire(
-                    'POLY', 40, (60, 100), 4, False, name="pl_i1_1",
-                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
-                ),
-            ],
-            'i2': [
-                Wire(
-                    'METAL1', 70, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 68, 60, 2, conn={"left": "n_i2_1"}),
-                Device(
-                    'nmos', 60, 31, 4, 38, 'vertical', name="n_i2_1",
-                   source_net='_net0', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 68, 100, 2, conn={"left": "p_i2_1"}),
-                Device(
-                    'pmos', 60, 150, 4, 40, 'vertical', name="p_i2_1",
-                   source_net='_net1', drain_net='vdd',
-                ),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 90, (60, 100), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_net0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_net0_1"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 30, 184, 2),
-                Wire('NTIE', 30, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 70, 182, 2,
-                    conn={"left": "p_i2_1", "right": "p_net0_1", "up": "vddrail"},
-                ),
-            ],
-            'vss': [
-                Via(
-                    'NDIF', 'METAL1', 10, 18, 2,
-                    conn={"right": "n_i0_1", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 30, 14, 2),
-                Wire('PTIE', 30, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 70, 18, 2,
-                    conn={"left": "n_i2_1", "right": "n_net0_1", "up": "vssrail"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='powmid_x0', width=140, height=200,
-        nets={
-            'vdd': [
-                Wire('METAL3', 40, (0, 200), 48, True),
-                # TODO VIA1 via
-                Wire('METAL2', (20, 60), 190, 6, True),
-                *(
-                    Via('METAL1', 'METAL2', x, 190, 2)
-                    for x in (25, 35, 45, 55)
-                ),
-                *(
-                    Via('METAL2', 'METAL3', x, 190, 2)
-                    for x in (25, 35, 45, 55)
-                ),
-                *(
-                    Via('NTIE', 'METAL1', x, 182, 2)
-                    for x in (10, 30, 50, 70, 90, 110, 130)
-                ),
-                Wire('NTIE', (10, 130), 182, 6, False),
-            ],
-            'vss': [
-                Wire('METAL3', 100, (0, 200), 48, True),
-                *(
-                    Via('PTIE', 'METAL1', x, 18, 2)
-                    for x in (10, 30, 50, 70, 90, 110, 130)
-                ),
-                # TODO VIA1 via
-                Wire('METAL2', (80, 120), 10, 6, True),
-                *(
-                    Via('METAL1', 'METAL2', x, 10, 2)
-                    for x in (85, 95, 105, 115)
-                ),
-                *(
-                    Via('METAL2', 'METAL3', x, 10, 2)
-                    for x in (85, 95, 105, 115)
-                ),
-                Wire('PTIE', (10, 130), 18, 6, False),
-                *(
-                    Via('POLY', 'METAL1', x, 40, 2, name=f"v_vss_top{i}")
-                    for i, x in enumerate((10, 30, 50, 70, 90, 110, 130))
-                ),
-                *(
-                    Wire(
-                        'METAL1', x, (18, 54), 6, False,
-                        conn={"top": f"v_vss_top{i}", "bottom": "vssrail"},
-                    )
-                    for i, x in enumerate((10, 30, 50, 70, 90, 110, 130))
-                ),
-                Wire('POLY', 70, (30, 170), 130, False),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='sff1_x4', width=300, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'PDIF', 230, (154, 186), 4, False,
-                    conn={"left": "p_ckr_2", "right": "p_q_1"},
-                ),
-            ],
-            '_net1': [
-                Wire(
-                    'PDIF', 110, (154, 186), 4, False,
-                    conn={"left": "p_u", "right": "p_ckr_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'NDIF', 110, (34, 46), 4, False,
-                    conn={"left": "n_u", "right": "n_nckr_2"},
-                ),
-            ],
-            '_net4': [
-                Wire(
-                    'NDIF', 150, (16, 46), 4, False,
-                    conn={"left": "n_ckr_1", "right": "n_y_1"},
-                ),
-            ],
-            '_net5': [
-                Wire(
-                    'PDIF', 150, (134, 186), 4, False,
-                    conn={"left": "p_nckr_2", "right": "p_y_1"},
-                ),
-            ],
-            '_net6': [
-                Wire(
-                    'NDIF', 230, (34, 46), 4, False,
-                    conn={"left": "n_nckr_3", "right": "n_q_1"},
-                ),
-            ],
-            'ck': [
-                Wire(
-                    'METAL1', 30, (42, 158), 3, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_ck",
-                    source_net='nckr', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_ck",
-                    source_net='nckr', drain_net='vdd',
-                ),
-                Via('POLY', 'METAL1', 28, 60, 2, conn={"left": "n_ck"}),
-                Via('POLY', 'METAL1', 28, 120, 2, conn={"left": "p_ck"}),
-            ],
-            'ckr': [
-                Device(
-                    'pmos', 120, 150, 4, 40, 'vertical', name="p_ckr_1",
-                    source_net='_net1', drain_net='sff_m',
-                ),
-                Device(
-                    'nmos', 140, 40, 4, 20, 'vertical', name="n_ckr_1",
-                    source_net='sff_m', drain_net='_net4',
-                ),
-                Device(
-                    'nmos', 200, 40, 4, 20, 'vertical', name="n_ckr_2",
-                    source_net='y', drain_net='sff_s',
-                ),
-                Device(
-                    'pmos', 220, 150, 4, 40, 'vertical', name="p_ckr_2",
-                    source_net='sff_s', drain_net='_net0',
-                ),
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2,
-                    conn={"left": "n_nckr_1"}, space={"bottom": "vssrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 50, 140, 2,
-                    conn={"left": "p_nckr_1"}, space={"top": "vddrail"},
-                ),
-                Wire('METAL1', 50, (42, 138), 6, False, space={}),
-                Via(
-                    'POLY', 'METAL1', 52, 80, 2, name="v_ckr_p2",
-                    conn={"right": "n_ckr_2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 124, 120, 2, name="v_ckr_p1",
-                    conn={"left": "p_ckr_1"},
-                ),
-                Wire(
-                    'METAL1', (125, 136), 120, 3, False, name="m1_ckr_v1",
-                    conn={"left": "v_ckr_p1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 136, 80, 2, name="v_ckr_n1",
-                    conn={"right": "n_ckr_1"},
-                ),
-                Wire(
-                    'METAL1', 135, (82, 121), 3, False,
-                #     conn={"top": "m1_ckr_v1", "bottom": "v_ckr_n1"},
-                    conn={"bottom": "v_ckr_n1"},
-                ),
-                Via('POLY', 'METAL1', 208, 80, 2, conn={"left": "v_ckr_p2"}),
-                Via('POLY', 'METAL1', 212, 120, 2, conn={"right": "p_ckr_2"}),
-                Wire('METAL1', 210, (79, 121), 6, False, space={}),
-            ],
-            'i': [
-                Device(
-                    'nmos', 80, 40, 4, 20, 'vertical', name="n_i",
-                    source_net='u', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 80, 170, 4, 40, 'vertical', name="p_i",
-                    source_net='u', drain_net='vdd',
-                ),
-                Wire(
-                    'METAL1', 90, (42, 158), 3, True, name="m1_i",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via('POLY', 'METAL1', 88, 60, 2, conn={"left": "n_i"}),
-                Via('POLY', 'METAL1', 88, 140, 2, conn={"left": "p_i"}),
-            ],
-            'nckr': [
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_nckr_1",
-                    source_net='vss', drain_net='ckr',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_nckr_1",
-                    source_net='vdd', drain_net='ckr',
-                ),
-                Device(
-                    'nmos', 120, 40, 4, 20, 'vertical', name="n_nckr_2",
-                    source_net='_net2', drain_net='sff_m',
-                ),
-                Device(
-                    'pmos', 140, 150, 4, 40, 'vertical', name="p_nckr_2",
-                    source_net='sff_m', drain_net='_net5',
-                ),
-                Device(
-                    'pmos', 200, 150, 4, 40, 'vertical', name="p_nckr_3",
-                    source_net='y', drain_net='sff_s',
-                ),
-                Device(
-                    'nmos', 220, 40, 4, 20, 'vertical', name="n_nckr_3",
-                    source_net='sff_s', drain_net='_net6',
-                ),
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_ndif_nckr",
-                    conn={"right": "n_ck"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 140, 2, name="v_pdif_nckr",
-                    conn={"right": "p_ck"},
-                ),
-                Wire(
-                    'METAL1', 10, (42, 138), 6, False,
-                    conn={"top": "v_pdif_nckr", "bottom": "v_ndif_nckr"},
-                ),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "n_nckr_3"}),
-                Wire(
-                    'POLY', 40, (56, 124), 4, False,
-                    conn={"bottom": "n_nckr_1", "top": "p_nckr_1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 122, 60, 2, name="v_poly_nckr",
-                    conn={"left": "n_nckr_2"},
-                ),
-                Via('POLY', 'METAL1', 120, 100, 2),
-                Wire(
-                    'METAL1', 120, (60, 100), 3, False, space={},
-                    conn={"bottom": "v_poly_nckr"},
-                ),
-                Wire('POLY', 140, (100, 124), 4, False, conn={"top": "p_nckr_2"}),
-                Wire('POLY', 200, (100, 144), 4, False, conn={"top": "p_nckr_3"}),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 270, (42, 158), 6, True, name="m1_q_o",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 270, 40, 2, space={"bottom": "vssrail"},
-                    conn={"left": "n_sffs_1", "right": "n_sffs_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 270, 140, 2, space={"top": "vddrail"},
-                    conn={"left": "p_sffs_1", "right": "p_sffs_2"},
-                ),
-                Device(
-                    'nmos', 240, 40, 4, 20, 'vertical', name="n_q_1",
-                    source_net='_net6', drain_net='vss',
-                ),
-                Via(
-                    'POLY', 'METAL1', 245, 60, 2, name="v_q_n1",
-                    # conn={"left": "n_q_1", "right": "m1_q_o"}, space={},
-                    conn={"left": "n_q_1"},
-                ),
-                Wire(
-                    'METAL1', (244, 270), 60, 6, False,
-                    conn={"left": "v_q_n1", "right": "m1_q_o"},
-                ),
-                Device(
-                    'pmos', 240, 170, 4, 40, 'vertical', name="p_q_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Via(
-                    'POLY', 'METAL1', 245, 100, 2, name="v_q_p1",
-                    # conn={"left": "p_q_1", "right": "m1_q_o"}, space={},
-                    conn={"left": "p_q_1"},
-                ),
-                Wire(
-                    'METAL1', (244, 270), 100, 6, False,
-                    conn={"left": "v_q_p1", "right": "m1_q_o"}
-                ),
-            ],
-            'sff_m': [
-                Via(
-                    'NDIF', 'METAL1', 130, 40, 4, name="v_sffm_ndif1",
-                    conn={"left": "n_nckr_2", "right": "n_ckr_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 130, 150, 2, name="v_sffm_pdif1",
-                    conn={"left": "p_ckr_1", "right": "p_nckr_2"},
-                ),
-                Wire(
-                    'METAL1', (130, 151), 40, 6, False,
-                    conn={"left": "v_sffm_ndif1"},
-                ),
-                Wire(
-                    'METAL1', (130, 151), 150, 6, False,
-                    conn={"left": "v_sffm_pdif1"},
-                ),
-                Wire('METAL1', 150, (39, 151), 6, False, space={}),
-                Via(
-                    'POLY', 'METAL1', 175, 60, 2, name="v_sffm_n1",
-                    conn={"right": "n_sffm_1"},
-                ),
-                Wire(
-                    'METAL1', (149, 176), 60, 6, False,
-                    conn={"right": "v_sffm_n1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 175, 120, 2, name="v_sffm_p1",
-                    conn={"right": "p_sffm_1"},
-                ),
-                Wire(
-                    'METAL1', (149, 176), 120, 6, False,
-                    conn={"right": "v_sffm_p1"},
-                ),
-                Device(
-                    'nmos', 180, 21, 4, 18, 'vertical', name="n_sffm_1",
-                    source_net='vss', drain_net='y',
-                ),
-                Device(
-                    'pmos', 180, 170, 4, 40, 'vertical', name="p_sffm_1",
-                    source_net='vdd', drain_net='y',
-                ),
-            ],
-            'sff_s': [
-                Device(
-                    'nmos', 260, 31, 4, 38, 'vertical', name="n_sffs_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 260, 150, 4, 80, 'vertical', name="p_sffs_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 260, (56, 104), 4, False,
-                    conn={"top": "p_sffs_1", "bottom": "n_sffs_1"},
-                ),
-                Device(
-                    'nmos', 280, 31, 4, 38, 'vertical', name="n_sffs_2",
-                    source_net='q', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 280, 150, 4, 80, 'vertical', name="p_sffs_2",
-                    source_net='q', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 280, (56, 104), 4, False, name="pl_sffs_2",
-                    conn={"top": "p_sffs_2", "bottom": "n_sffs_2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 255, 80, 2, name="v_sffs_pl",
-                    conn={"right": "pl_sffs_2"},
-                ),
-                Wire(
-                    'METAL1', 230, (39, 161), 6, False, name="m1_sffs_1",
-                ),
-                Wire(
-                    'METAL1', (229, 256), 80, 6, False,
-                    conn={"left": "m1_sffs_1","right": "v_sffs_pl"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 210, 40, 2, name="v_sffs_ndif1",
-                    conn={"left": "n_ckr_2", "right": "n_nckr_3"},
-                    space={"bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (209, 231), 40, 3, False,
-                    # conn={"left": "v_sffs_ndif1", "right": "m1_sffs_1"},
-                    conn={"left": "v_sffs_ndif1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 210, 140, 2, name="v_sffs_pdif1",
-                    conn={"left": "p_nckr_3", "right": "p_ckr_2"},
-                    space={"top": "vddrail"},
-                ),
-                Wire(
-                    'METAL1', (209, 231), 160, 3, False,
-                    # conn={"left": "v_sffs_pdif1", "right": "m1_sffs_1"},
-                    conn={"left": "v_sffs_pdif1"},
-                ),
-            ],
-            'u': [
-                Device(
-                    'nmos', 100, 40, 4, 20, 'vertical', name="n_u",
-                    source_net='vss', drain_net='_net2',
-                ),
-                Device(
-                    'pmos', 100, 170, 4, 40, 'vertical', name="p_u",
-                    source_net='vdd', drain_net='_net1',
-                ),
-                Via(
-                    'POLY', 'METAL1', 72, 120, 2, name="v_u_p2",
-                    conn={"right": "p_u"},
-                ),
-                Wire(
-                    'METAL1', 70, (42, 158), 6, False,
-                    conn={"bottom": "v_u_ndif", "top": "v_u_pdif"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, name="v_u_ndif",
-                    conn={"right": "n_i"}, space={"bottom": "vssrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 160, 2, name="v_u_pdif",
-                    conn={"right": "p_i"}, space={"top": "vddrail"},
-                ),
-                Wire(
-                    'METAL1', 104, (62, 118), 3, False,
-                    conn={"top": "v_u_p", "bottom": "v_u_n"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 104, 60, 2, name="v_u_n",
-                    conn={"left": "n_u"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 104, 120, 2, name="v_u_p",
-                    conn={"left": "v_u_p2"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 10, 184, 2),
-                Wire('NTIE', 10, (180, 190), 6, False),
-                Via(
-                    'PDIF', 'METAL1', 30, 184, 2,
-                    conn={"left": "p_ck", "right": "p_nckr_1"},
-                ),
-                Via('NTIE', 'METAL1', 50, 184, 2),
-                Wire('NTIE', 50, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 90, 184, 2,
-                    conn={"left": "p_i", "right": "p_u", "up": "vddrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 170, 184, 2,
-                    conn={"left": "p_y_1", "right": "p_sffm_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 250, 140, 2,
-                    conn={"left": "p_q_1", "right": "p_sffs_1"},
-                ),
-                Via('PDIF', 'METAL1', 290, 160, 2, conn={"left": "p_sffs_2"}),
-                Via('NTIE', 'METAL1', 130, 184, 2),
-                Wire('NTIE', 130, (180, 188), 10, False),
-                Via('NTIE', 'METAL1', 210, 184, 2),
-                Wire('NTIE', 210, (180, 188), 10, False),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 30, 16, 2,
-                    conn={"left": "n_ck", "right": "n_nckr_1"}, 
-                ),
-                Via('PTIE', 'METAL1', 50, 14, 2),
-                Wire('PTIE', 50, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 90, 16, 2,
-                    conn={"left": "n_i", "right": "n_u"},
-                ),
-                Via(
-                    'NDIF', "METAL1", 170, 20, 4,
-                    conn={"left": "n_y_1", "right": "n_sffm_1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 250, 40, 2,
-                    conn={"left": "n_q_1", "right": "n_sffs_1"},
-                ),
-                Via('NDIF', 'METAL1', 290, 40, 2, conn={"left": "n_sffs_2"}),
-                Via('PTIE', 'METAL1', 130, 14, 2),
-                Wire('PTIE', 130, (10, 18), 10, False),
-                Via('PTIE', 'METAL1', 230, 14, 2),
-                Wire('PTIE', 230, (10, 18), 10, False),
-            ],
-            'y': [
-                Device(
-                    'nmos', 160, 21, 4, 18, 'vertical', name="n_y_1",
-                    source_net='_net4', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 160, 170, 4, 40, 'vertical', name="p_y_1",
-                    source_net='_net5', drain_net='vdd',
-                ),
-                Via(
-                    'POLY', 'METAL1', 164, 40, 2, name="v_y_n1",
-                    conn={"left": "n_y_1"},
-                ),
-                Wire('METAL1', (164, 191), 40, 6, False, conn={"left": "v_y_n1"}),
-                Via(
-                    'POLY', 'METAL1', 164, 140, 2, name="v_y_p1",
-                    conn={"left": "p_y_1"},
-                ),
-                Wire('METAL1', (164, 191), 140, 6, False, conn={"left": "v_y_p1"}),
-                Via(
-                    'NDIF', 'METAL1', 190, 40, 2, name="v_y_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_sffm_1", "right": "n_ckr_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 190, 160, 2, name="v_y_pdif1",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_sffm_1", "right": "p_nckr_3"},
-                ),
-                Wire(
-                    'METAL1', 190, (42, 158), 3, False,
-                    conn={"top": "v_y_pdif1", "bottom": "v_y_ndif1"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='sff1r_x4', width=360, height=200,
-        nets={
-            '_net0': [
-                Wire(
-                    'PDIF', 110, (140, 170), 4, False,
-                    conn={"left": "p_u_1", "right": "p_ckr_1"},
-                ),
-            ],
-            '_net2': [
-                Wire(
-                    'PDIF', 150, (134, 186), 4, False,
-                    conn={"left": "p_nckr_2", "right": "p_y_1"},
-                ),
-            ],
-            '_net3': [
-                Via(
-                    'PDIF', 'METAL1', 230, 160, 2, name="v_net3_pdif1",
-                    space={"top": "vddrail"}, conn={"left": "p_nrst_2"},
-                ),
-                Wire(
-                    'METAL1', (230, 290), 160, 6, False, name="m1_net3_1",
-                    conn={"left": "v_net3_pdif1", "right": "v_net3_pdif2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 290, 160, 2, name="v_net3_pdif2",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_ckr_2", "right": "p_q_1"}
-                ),
-            ],
-            '_net4': [
-                Wire(
-                    'NDIF', 190, (16, 26), 4, False,
-                    conn={"left": "n_sffm_1", "right": "n_nrst_1"},
-                ),
-            ],
-            '_net5': [
-                Wire(
-                    'NDIF', 290, (34, 46), 8, False,
-                    conn={"left": "n_nrst_2", "right": "n_q_1"},
-                ),
-            ],
-            '_net6': [
-                Wire(
-                    'NDIF', 150, (16, 46), 4, False,
-                    conn={"left": "n_ckr_1", "right": "n_y_1"},
-                ),
-            ],
-            '_net7': [
-                Wire(
-                    'NDIF', 110, (35, 45), 4, False,
-                    conn={"left": "n_u_1", "right": "n_nckr_2"},
-                ),
-            ],
-            '_net8': [
-                Wire(
-                    'NDIF', 270, (34, 46), 8, False,
-                    conn={"left": "n_nckr_3", "right": "n_nrst_2"},
-                ),
-            ],
-            'ck': [
-                Wire(
-                    'METAL1', 30, (40, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"}
-                ),
-                Via('POLY', 'METAL1', 30, 60, 2, conn={"left": "n_ck_1"}),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_ck_1",
-                    source_net='nckr', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 30, 120, 2, conn={"left": "p_ck_1"}),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_ck_1",
-                    source_net='nckr', drain_net='vdd',
-                ),
-            ],
-            'ckr': [
-                Via(
-                    'NDIF', 'METAL1', 50, 40, 2, name="v_ckr_ndif1",
-                    conn={"left": "n_nckr_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 50, 140, 2, name="v_ckr_pdif1",
-                    conn={"left": "p_nckr_1"},
-                ),
-                Wire(
-                    'METAL1', 50, (60, 100), 6, False,
-                    conn={"top": "v_ckr_pdif1", "bottom": "v_ckr_ndif1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 52, 80, 2, name="v_ckr_pl5",
-                    conn={"right": "n_ckr_2"},
-                ),
-                Via('POLY', 'METAL1', 135, 80, 2, name="v_ckr_pl1"),
-                Wire(
-                    'METAL1', 135, (82, 120), 3, False, name="m1_ckr_1",
-                    conn={"top": "v_ckr_pl2", "bottom": "v_ckr_pl1"},
-                ),
-                Wire('METAL1', (122, 135), 120, 3, False, conn={"right": "m1_ckr_1"}),
-                Via(
-                    'POLY', 'METAL1', 122, 120, 2, name="v_ckr_pl2",
-                    conn={"left": "p_ckr_1"},
-                ),
-                Device(
-                    'pmos', 120, 150, 4, 40, 'vertical', name="p_ckr_1",
-                    source_net='_net0', drain_net='sff_m',
-                ),
-                Wire(
-                    'POLY', 140, (60, 80), 4, False,
-                    conn={"bottom": "n_ckr_1"},
-                ),
-                Device(
-                    'nmos', 140, 40, 4, 20, 'vertical', name="n_ckr_1",
-                    source_net='sff_m', drain_net='_net6',
-                ),
-
-                Device(
-                    'nmos', 240, 40, 4, 20, 'vertical', name="n_ckr_2",
-                    source_net='y', drain_net='sff_s',
-                ),
-                Via(
-                    'POLY', 'METAL1', 245, 80, 2, name="v_ckr_pl3",
-                    conn={"left": "v_ckr_pl5"},
-                ),
-                Wire(
-                    'METAL1', (245, 270), 80, 6, False,
-                    conn={"left": "v_ckr_pl3", "right": "m1_ckr_2"},
-                ),
-                Wire(
-                    'METAL1', 270, (80, 100), 6, False, name="m1_ckr_2",
-                    conn={"top": "v_ckr_pl4"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 272, 100, 2, name="v_ckr_pl4",
-                    conn={"right": "p_ckr_2"},
-                ),
-                Device(
-                    'pmos', 280, 150, 4, 40, 'vertical', name="p_ckr_2",
-                    source_net='sff_s', drain_net='_net3',
-                ),
-            ],
-            'i': [
-                Wire(
-                    'METAL1', 90, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"}
-                ),
-                Via('POLY', 'METAL1', 88, 60, 2, conn={"left": "n_i_1"}),
-                Device(
-                    'nmos', 80, 40, 4, 20, 'vertical', name="n_i_1",
-                    source_net='u', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 88, 140, 2, conn={"left": "p_i_1"}),
-                Device(
-                    'pmos', 80, 170, 4, 40, 'vertical', name="p_i_1",
-                    source_net='u', drain_net='vdd',
-                ),
-            ],
-            'nckr': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_nckr_ndif1",
-                    conn={"right": "n_ck_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 140, 2, name="v_nckr_pdif1",
-                    conn={"right": "p_ck_1"},
-                ),
-                Wire(
-                    'METAL1', 10, (60, 100), 6, False,
-                    conn={"top": "v_nckr_pdif1", "bottom": "v_nckr_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "n_nckr_3"}),
-                Device(
-                    'nmos', 40, 40, 4, 20, 'vertical', name="n_nckr_1",
-                    source_net='vss', drain_net='ckr',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 40, 'vertical', name="p_nckr_1",
-                    source_net='vdd', drain_net='ckr',
-                ),
-                Wire(
-                    'POLY', 40, (56, 124), 4, False,
-                    conn={"top": "p_nckr_1", "bottom": "n_nckr_1"},
-                ),
-                Via('POLY', 'METAL1', 120, 100, 2, name="v_nckr_pl1"),
-                Wire(
-                    'METAL1', 120, (60, 100), 6, False,
-                    conn={"top": "v_nckr_pl1", "bottom": "v_nckr_pl2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 122, 60, 2, name="v_nckr_pl2",
-                    conn={"left": "n_nckr_2"},
-                ),
-                Device(
-                    'nmos', 120, 40, 4, 20, 'vertical', name="n_nckr_2",
-                    source_net='_net7', drain_net='sff_m',
-                ),
-                Wire('POLY', 140, (100, 120), 4, False, conn={"top": "p_nckr_2"}),
-                Device(
-                    'pmos', 140, 150, 4, 40, 'vertical', name="p_nckr_2",
-                    source_net='sff_m', drain_net='_net2',
-                ),
-                Device(
-                    'nmos', 260, 40, 4, 20, 'vertical', name="n_nckr_3",
-                    source_net='sff_s', drain_net='_net8',
-                ),
-                Wire('POLY', 260, (98, 120), 4, False, conn={"top": "p_nckr_3"}),
-                Device(
-                    'pmos', 260, 150, 4, 40, 'vertical', name="p_nckr_3",
-                    source_net='y', drain_net='sff_s',
-                ),
-            ],
-            'nrst': [
-                Device(
-                    'nmos', 200, 21, 4, 18, 'vertical', name="n_nrst_1",
-                    source_net='_net4', drain_net='y',
-                ),
-                Via('POLY', 'METAL1', 228, 60, 2, conn={"left": "n_nrst_1"}),
-                Device(
-                    'pmos', 200, 170, 4, 40, 'vertical', name="p_nrst_1",
-                    source_net='y', drain_net='vdd',
-                ),
-                Device(
-                    'pmos', 220, 170, 4, 40, 'vertical', name="p_nrst_2",
-                    source_net='vdd', drain_net='_net3',
-                ),
-                Via('POLY', 'METAL1', 228, 120, 2, conn={"left": "p_nrst_1"}),
-                Wire('POLY', 220, (120, 140), 8, False, conn={"top": "p_nrst_2"}),
-                Wire(
-                    'METAL1', 230, (40, 60), 6, True, name="m1_nrst_1",
-                    space={"top": "m1_y_2", "bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (230, 278), 60, 6, False,
-                    conn={"left": "m1_nrst_1", "right": "v_nrst_pl2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 278, 60, 2, name="v_nrst_pl2",
-                    conn={"right": "n_nrst_2"},
-                ),
-                Device(
-                    'nmos', 280, 40, 4, 20, 'vertical', name="n_nrst_2",
-                    source_net='_net8', drain_net='_net5',
-                ),
-            ],
-            'q': [
-                Via(
-                    'NDIF', 'METAL1', 330, 40, 2, name="v_q_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_sffs_1", "right": "n_sffs_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 330, 140, 2, name="v_q_pdif1",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_sffs_1", "right": "p_sffs_2"},
-                ),
-                Wire(
-                    'METAL1', 330, (60, 100), 6, True, name="m1_q_i",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (310, 330), 60, 6, False,
-                    conn={"left": "v_q_pl1", "right": "m1_q_i"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 302, 60, 2, name="v_q_pl1",
-                    conn={"left": "n_q_1"},
-                ),
-                Device(
-                    'nmos', 300, 40, 4, 20, 'vertical', name="n_q_1",
-                    source_net='_net5', drain_net='vss',
-                ),
-                Wire(
-                    'METAL1', (310, 330), 100, 6, False,
-                    conn={"left": "v_q_pl2", "right": "m1_q_i"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 302, 100, 2, name="v_q_pl2",
-                    conn={"left": "p_q_1"},
-                ),
-                Device(
-                    'pmos', 300, 170, 4, 40, 'vertical', name="p_q_1",
-                    source_net='_net3', drain_net='vdd',
-                ),
-            ],
-            'sff_m': [
-                Via(
-                    'NDIF', 'METAL1', 130, 40, 2, name="v_sffm_ndif1",
-                    conn={"left": "n_nckr_2", "right": "n_ckr_1"},
-                ),
-                Wire(
-                    'METAL1', (130, 150), 40, 6, False,
-                    conn={"left": "v_sffm_ndif1", "right": "m1_sffm_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 130, 140, 2, name="v_sffm_pdif1",
-                    conn={"left": "p_ckr_1", "right": "p_nckr_2"},
-                ),
-                Wire(
-                    'METAL1', (130, 150), 140, 6, False,
-                    conn={"left": "v_sffm_pdif1", "right": "m1_sffm_1"},
-                ),
-                Wire('METAL1', 150, (40, 140), 6, False, name="m1_sffm_1"),
-                Wire(
-                    'METAL1', (150, 170), 60, 6, False,
-                    conn={"left": "m1_sffm_1", "right": "v_sffm_pl1"}
-                ),
-                Via(
-                    'POLY', 'METAL1', 178, 60, 2, name="v_sffm_pl1",
-                    conn={"right": "n_sffm_1"},
-                ),
-                Device(
-                    'nmos', 180, 21, 4, 18, 'vertical', name="n_sffm_1",
-                    source_net='vss', drain_net='_net4',
-                ),
-                Wire(
-                    'METAL1', (150, 170), 120, 6, False,
-                    conn={"left": "m1_sffm_1", "right": "v_sffm_pl2"}
-                ),
-                Via(
-                    'POLY', 'METAL1', 178, 120, 2, name="v_sffm_pl2",
-                    conn={"right": "p_sffm_1"},
-                ),
-                Device(
-                    'pmos', 180, 170, 4, 40, 'vertical', name="p_sffm_1",
-                    source_net='vdd', drain_net='y',
-                ),
-            ],
-            'sff_s': [
-                Device(
-                    'nmos', 320, 31, 4, 38, 'vertical', name="n_sffs_1",
-                    source_net='vss', drain_net='q',
-                ),
-                Device(
-                    'pmos', 320, 150, 4, 80, 'vertical', name="p_sffs_1",
-                    source_net='vdd', drain_net='q',
-                ),
-                Wire(
-                    'POLY', 320, (60, 100), 4, False,
-                    conn={"top": "p_sffs_1", "bottom": "n_sffs_1"},
-                ),
-                Device(
-                    'nmos', 340, 31, 4, 38, 'vertical', name="n_sffs_2",
-                    source_net='q', drain_net='vss',
-                ),
-                Device(
-                    'pmos', 340, 150, 4, 80, 'vertical', name="p_sffs_2",
-                    source_net='q', drain_net='vdd',
-                ),
-                Wire(
-                    'POLY', 340, (60, 100), 4, False, name="pl_sffs_1",
-                    conn={"top": "p_sffs_2", "bottom": "n_sffs_2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 312, 80, 2, name='v_sffs_pl1',
-                    conn={"right": "pl_sffs_1"},
-                ),
-                Wire(
-                    'METAL1', (290, 310), 80, 6, False,
-                    conn={"left": "m1_sffs_1", "right": "v_sffs_pl1"},
-                ),
-                Wire('METAL1', 290, (40, 120), 6, False, name="m1_sffs_1"),
-                Wire(
-                    'METAL1', (250, 290), 40, 6, False,
-                    conn={"left": "v_sffs_ndif1", "right": "m1_sffs_1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 250, 40, 2, name="v_sffs_ndif1",
-                    conn={"left": "n_ckr_2", "right": "n_nckr_3"},
-                ),
-                Wire(
-                    'METAL1', (270, 290), 120, 6, False,
-                    conn={"left": "v_sffs_pdif1", "right": "m1_sffs_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 270, 140, 2, name="v_sffs_pdif1",
-                    conn={"left": "p_nckr_3", "right": "p_ckr_2"},
-                    space={"top": "m1_net3_1"},
-                ),
-            ],
-            'u': [
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, name="v_u_ndif1",
-                    conn={"right": "n_i_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 70, 160, 2, name="v_u_pdif1",
-                    space={"top": "vddrail"}, conn={"right": "p_i_1"},
-                ),
-                Wire(
-                    'METAL1', 70, (60, 100), 3, False,
-                    conn={"top": "v_u_pdif1", "bottom": "v_u_ndif1"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 72, 120, 2, name="v_u_pl3",
-                    conn={"right": "p_u_1"},
-                ),
-                Device(
-                    'pmos', 100, 170, 4, 40, 'vertical', name="p_u_1",
-                    source_net='vdd', drain_net='_net0',
-                ),
-                Via(
-                    'POLY', 'METAL1', 103, 120, 2, name="v_u_pl1",
-                    conn={"left": "v_u_pl3"},
-                ),
-                Wire(
-                    'METAL1', 105, (60, 100), 6, False,
-                    conn={"top": "v_u_pl1", "bottom": "v_u_pl2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 103, 60, 2, name="v_u_pl2",
-                    conn={"left": "n_u_1"},
-                ),
-                Device(
-                    'nmos', 100, 40, 4, 20, 'vertical', name="n_u_1",
-                    source_net='vss', drain_net='_net7',
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 10, 184, 2),
-                Wire('NTIE', 10, (180, 190), 6, False),
-                Via(
-                    'PDIF', 'METAL1', 30, 182, 2,
-                    conn={"left": "p_ck_1", "right": "p_nckr_1"},
-                ),
-                Via('NTIE', 'METAL1', 50, 184, 2),
-                Wire('NTIE', 50, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 90, 182, 2,
-                    conn={"left": "p_i_1", "right": "p_u_1", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 130, 184, 2),
-                Wire('NTIE', 130, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 170, 182, 2,
-                    conn={"left": "p_y_1", "right": "p_sffm_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 210, 182, 2,
-                    conn={"left": "p_nrst_1", "right": "p_nrst_2"},
-                ),
-                Via('NTIE', 'METAL1', 270, 184, 2),
-                Wire('NTIE', 270, (180, 188), 8, False),
-                Via(
-                    'PDIF', 'METAL1', 310, 182, 2,
-                    conn={"left": "p_q_1", "right": "p_sffs_1"},
-                ),
-                Via('PDIF', 'METAL1', 350, 182, 2, conn={"left": "p_sffs_2"}),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 30, 18, 2,
-                    conn={"left": "n_ck_1", "right": "n_nckr_1"},
-                ),
-                Via('PTIE', 'METAL1', 50, 14, 2),
-                Wire('PTIE', 50, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 90, 18, 2,
-                    conn={"left": "n_i_1", "right": "n_u_1"},
-                ),
-                Via('PTIE', 'METAL1', 130, 14, 2),
-                Wire('PTIE', 130, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 170, 18, 2,
-                    conn={"left": "n_y_1", "right": "n_sffm_1"},
-                ),
-                Via('PTIE', 'METAL1', 290, 14, 2),
-                Wire('PTIE', 290, (10, 18), 8, False),
-                Via(
-                    'NDIF', 'METAL1', 310, 18, 2,
-                    conn={"left": "n_q_1", "right": "n_sffs_1"},
-                ),
-                Via('NDIF', 'METAL1', 350, 18, 2, conn={"left": "n_sffs_2"}),
-            ],
-            'y': [
-                Device(
-                    'nmos', 160, 21, 4, 18, 'vertical', name="n_y_1",
-                    source_net='_net6', drain_net='vss',
-                ),
-                Via('POLY', 'METAL1', 162, 40, 2, conn={"left": "n_y_1"}),
-                Device(
-                    'pmos', 160, 170, 4, 40, 'vertical', name="p_y_1",
-                    source_net='_net2', drain_net='vdd',
-                ),
-                Via('POLY', 'METAL1', 162, 140, 2, conn={"left": "p_y_1"}),
-                Via(
-                    'PDIF', 'METAL1', 190, 160, 2, name="v_y_pdif1",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_sffm_1", "right": "p_nrst_1"},
-                ),
-                Wire('METAL1', 190, (42, 158), 6, False, name="m1_y_1"),
-                Wire(
-                    'METAL1', (162, 210), 40, 6, False,
-                    conn={"left": "m1_y_1", "right": "v_y_ndif1"}
-                ),
-                Via(
-                    'NDIF', 'METAL1', 210, 40, 2, name="v_y_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_nrst_1", "right": "n_ckr_2"},
-                ),
-                Wire(
-                    'METAL1', (162, 240), 140, 6, False, name="m1_y_2",
-                    conn={"left": "m1_y_1", "right": "v_y_pdif2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 250, 140, 2, name="v_y_pdif2",
-                    conn={"right": "p_nckr_3"}, space={"top": "m1_net3_1"},
-                ),
-            ],
-        },
-        finalize=True,
-    ),
-    StdCell(
-        name='xr2_x1', width=140, height=200,
-        nets={
-            '_net0': [
-                Via(
-                    'NDIF', 'METAL1', 10, 40, 2, name="v_net0_ndif1",
-                    conn={"right": "n_i0_1"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 10, 140, 2, name="v_net0_pdif1",
-                    conn={"right": "p_i0_1"},
-                ),
-                Wire(
-                    'METAL1', 10, (60, 120), 3, False,
-                    conn={"top": "v_net0_pdif1", "bottom": "v_net0_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_net0_1"}),
-                Wire(
-                    'POLY', 80, (60, 100), 4, False, name="pl_net0_1",
-                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
-                ),
-                Device(
-                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
-                    source_net='q', drain_net='_net4',
-                ),
-                Device(
-                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
-                    source_net='q', drain_net='_net2',
-                ),
-            ],
-            '_net1': [
-                Wire(
-                    'NDIF', 50, (16, 46), 4, False,
-                    conn={"left": "n_i0_2", "right": "n_i1_1"},
-                ),
-            ],
-            '_net2': [
-                Via(
-                    'PDIF', 'METAL1', 50, 160, 2, name="v_net2_pdif1",
-                    space={"top": "vddrail", "bottom": "m1_q_o"},
-                    conn={"left": "p_i0_2", "right": "p_net3_1"},
-                ),
-                Wire(
-                    'METAL1', (50, 90), 160, 6, False, name="m1_net2_1",
-                    conn={"left": "v_net2_pdif1", "right": "v_net2_pdif2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 90, 140, 2, name="v_net2_pdif2",
-                    space={"top": "vddrail"},
-                    conn={"left": "p_net0_1", "right": "p_i1_1"},
-                ),
-            ],
-            '_net3': [
-                Via(
-                    'NDIF', 'METAL1', 130, 40, 2, name="v_net3_ndif1",
-                    conn={"left": "n_i1_2"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 130, 140, 2, name="v_net3_pdif1",
-                    conn={"left": "p_i1_2"},
-                ),
-                Wire(
-                    'METAL1', 130, (42, 138), 6, False,
-                    conn={"top": "v_net3_pdif1", "bottom": "v_net3_ndif1"},
-                ),
-                Via('POLY', 'METAL1', 128, 80, 2, conn={"left": "n_net3_1"}),
-                Device(
-                    'nmos', 100, 31, 4, 38, 'vertical', name="n_net3_1",
-                    source_net='_net4', drain_net='vss',
-                ),
-                Via(
-                    'POLY', 'METAL1', 98, 80, 2, name="v_net3_pl1",
-                    conn={"right": "n_net3_1"},
-                ),
-                Wire(
-                    'METAL1', (70, 98), 80, 6, False,
-                    conn={"left": "m1_net3_1", "right": "v_net3_pl1"},
-                ),
-                Wire(
-                    'METAL1', 70, (80, 98), 6, False, name="m1_net3_1",
-                    conn={"top": "v_net3_pl2"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 68, 100, 2, name="v_net3_pl2",
-                    conn={"left": "p_net3_1"},
-                ),
-                Device(
-                    'pmos', 60, 150, 4, 80, 'vertical', name="p_net3_1",
-                    source_net='_net2', drain_net='q',
-                ),
-            ],
-            '_net4': [
-                Wire(
-                    'NDIF', 90, (16, 46), 4, False,
-                    conn={"left": "n_net0_1", "right": "n_net3_1"},
-                ),
-            ],
-            'i0': [
-                Wire(
-                    'METAL1', 30, (42, 158), 6, True,
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 30, 60, 2,
-                    conn={"left": "n_i0_1", "right": "n_i0_2"},
-                ),
-                Device(
-                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i0_1",
-                    source_net='_net0', drain_net='vss',
-                ),
-                Device(
-                    'nmos', 40, 31, 4, 38, 'vertical', name="n_i0_2",
-                    source_net='vss', drain_net='_net1',
-                ),
-                Via(
-                    'POLY', 'METAL1', 30, 100, 2,
-                    conn={"left": "p_i0_1", "right": "p_i0_2"},
-                ),
-                Device(
-                    'pmos', 20, 150, 4, 40, 'vertical', name="p_i0_1",
-                    source_net='_net0', drain_net='vdd',
-                ),
-                Device(
-                    'pmos', 40, 150, 4, 80, 'vertical', name="p_i0_2",
-                    source_net='vdd', drain_net='_net2',
-                ),
-            ],
-            'i1': [
-                Wire(
-                    'METAL1', 110, (42, 158), 6, True, name="m1_i1_i",
-                    space={"top": "vddrail", "bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (62, 110), 60, 6, False,
-                    conn={"left": "v_i1_pl1", "right": "m1_i1_i"},
-                ),
-                Via(
-                    'POLY', 'METAL1', 62, 60, 2, name="v_i1_pl1",
-                    conn={"left": "n_i1_1"},
-                ),
-                Device(
-                    'nmos', 60, 31, 4, 38, 'vertical', name="n_i1_1",
-                    source_net='_net1', drain_net='q',
-                ),
-                Via('POLY', 'METAL1', 110, 60, 2, conn={"right": "n_i1_2"}),
-                Device(
-                    'nmos', 120, 40, 4, 20, 'vertical', name="n_i1_2",
-                    source_net='vss', drain_net='_net3',
-                ),
-                Via(
-                    'POLY', 'METAL1', 110, 100, 2,
-                    conn={"left": "p_i1_1", "right": "p_i1_2"},
-                ),
-                Device(
-                    'pmos', 100, 150, 4, 80, 'vertical', name="p_i1_1",
-                    source_net='_net2', drain_net='vdd',
-                ),
-                Device(
-                    'pmos', 120, 150, 4, 40, 'vertical', name="p_i1_2",
-                    source_net='vdd', drain_net='_net3',
-                ),
-            ],
-            'q': [
-                Wire(
-                    'METAL1', 50, (40, 130), 3, True, name="m1_q_o",
-                    space={"bottom": "vssrail"},
-                ),
-                Wire(
-                    'METAL1', (50, 70), 40, 6, False,
-                    conn={"left": "m1_q_o", "right": "v_q_ndif1"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 70, 40, 2, name="v_q_ndif1",
-                    space={"bottom": "vssrail"},
-                    conn={"left": "n_i1_1", "right": "n_net0_1"},
-                ),
-                Wire('METAL1', (50, 70), 120, 6, False),
-                Via(
-                    'PDIF', 'METAL1', 70, 140, 2, name="v_q_pdif1",
-                    space={"top": "m1_net2_1"},
-                    conn={"left": "p_net3_1", "right": "p_net0_1"},
-                ),
-            ],
-            'vdd': [
-                Via('NTIE', 'METAL1', 10, 184, 2),
-                Wire('NTIE', 10, (180, 190), 6, False),
-                Via(
-                    'PDIF', 'METAL1', 30, 184, 2,
-                    conn={"left": "p_i0_1", "right": "p_i0_2", "up": "vddrail"},
-                ),
-                Via(
-                    'PDIF', 'METAL1', 110, 184, 2,
-                    conn={"left": "p_i1_1", "right": "p_i1_2", "up": "vddrail"},
-                ),
-                Via('NTIE', 'METAL1', 130, 184, 2),
-                Wire('NTIE', 130, (180, 190), 6, False),
-            ],
-            'vss': [
-                Via('PTIE', 'METAL1', 10, 14, 2),
-                Wire('PTIE', 10, (8, 18), 6, False),
-                Via(
-                    'NDIF', 'METAL1', 30, 18, 2,
-                    conn={"left": "n_i0_1", "right": "n_i0_2", "up": "vssrail"},
-                ),
-                Via(
-                    'NDIF', 'METAL1', 110, 18, 2,
-                    conn={"left": "n_net3_1", "right": "n_i1_2", "up": "vssrail"},
-                ),
-                Via('PTIE', 'METAL1', 130, 14, 2),
-                Wire('PTIE', 130, (8, 18), 6, False),
-            ],
-        },
-        finalize=True,
-    ),
+    # StdCell(
+    #     name='powmid_x0', width=140, height=200,
+    #     nets={
+    #         'vdd': [
+    #             Wire('METAL3', 40, (0, 200), 48, True),
+    #             # TODO VIA1 via
+    #             Wire('METAL2', (20, 60), 190, 6, True),
+    #             *(
+    #                 Via('METAL1', 'METAL2', x, 190, 2)
+    #                 for x in (25, 35, 45, 55)
+    #             ),
+    #             *(
+    #                 Via('METAL2', 'METAL3', x, 190, 2)
+    #                 for x in (25, 35, 45, 55)
+    #             ),
+    #             *(
+    #                 Via('NTIE', 'METAL1', x, 182, 2)
+    #                 for x in (10, 30, 50, 70, 90, 110, 130)
+    #             ),
+    #             Wire('NTIE', (10, 130), 182, 6, False),
+    #         ],
+    #         'vss': [
+    #             Wire('METAL3', 100, (0, 200), 48, True),
+    #             *(
+    #                 Via('PTIE', 'METAL1', x, 18, 2)
+    #                 for x in (10, 30, 50, 70, 90, 110, 130)
+    #             ),
+    #             # TODO VIA1 via
+    #             Wire('METAL2', (80, 120), 10, 6, True),
+    #             *(
+    #                 Via('METAL1', 'METAL2', x, 10, 2)
+    #                 for x in (85, 95, 105, 115)
+    #             ),
+    #             *(
+    #                 Via('METAL2', 'METAL3', x, 10, 2)
+    #                 for x in (85, 95, 105, 115)
+    #             ),
+    #             Wire('PTIE', (10, 130), 18, 6, False),
+    #             *(
+    #                 Via('POLY', 'METAL1', x, 40, 2, name=f"v_vss_top{i}")
+    #                 for i, x in enumerate((10, 30, 50, 70, 90, 110, 130))
+    #             ),
+    #             *(
+    #                 Wire(
+    #                     'METAL1', x, (18, 54), 6, False,
+    #                     conn={"top": f"v_vss_top{i}", "bottom": "vssrail"},
+    #                 )
+    #                 for i, x in enumerate((10, 30, 50, 70, 90, 110, 130))
+    #             ),
+    #             Wire('POLY', 70, (30, 170), 130, False),
+    #         ],
+    #     },
+    #     finalize=True,
+    # ),
 ]
 
 
 _oldcells = [
     StdCell(
         name='a2_x2', width=100, height=200,
         nets={
@@ -3948,92 +724,149 @@
                 Via('NDIF', 'METAL1', 140, 40, 2),
                 Wire('NDIF', 144, (16, 46), 8, False),
             ],
         },
         finalize=True,
     ),
     StdCell(
-        name='ao22_x2', width=120, height=200,
+        name='ao22_x2', width=100, height=200,
         nets={
             '_net0': [
-                Wire('NDIF', 38, (34, 60), 12, False),
-                Via('NDIF', 'METAL1', 38, 62, 2),
-                Wire('METAL1', (38, 58), 64, 6, False),
-                Via('POLY', 'METAL1', 60, 88, 2),
-                Wire('METAL1', 60, (62, 158), 6, False),
-                Via('PDIF', 'METAL1', 60, 136, 2),
-                Wire('PDIF', 60, (130, 162), 12, False),
-                Via('PDIF', 'METAL1', 60, 156, 2),
-                Wire('POLY', (58, 92), 88, 4, False),
-                Device('nmos', 92, 31, 4, 38, 'vertical', source_net='vss', drain_net='q'),
-                Wire('POLY', 92, (56, 104), 4, False),
-                Device('pmos', 92, 150, 4, 80, 'vertical', source_net='vdd', drain_net='q'),
+                Via(
+                    'NDIF', 'METAL1', 30, 60, 2, name="v_net0_ndif1",
+                    space={"top": "m1_i1_1", "bottom": "vssrail"},
+                    conn={"left": "n_i0_1", "right": "n_i1_1"},
+                ),
+                Wire(
+                    'METAL1', (30, 50), 60, 3, False, name="m1_net0_1",
+                    conn={"left": "v_net0_ndif1"},
+                ),
+                Wire(
+                    'METAL1', 50, (60, 100), 3, False,
+                    conn={"top": "v_net0_pdif1", "bottom": "m1_net0_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 50, 140, 2, name="v_net0_pdif1",
+                    conn={"left": "p_i1_1", "right": "p_i2_1"},
+                ),
+                Via('POLY', 'METAL1', 52, 80, 2, conn={"right": "pl_net0_1"}),
+                Device(
+                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
+                    source_net='vss', drain_net='q',
+                ),
+                Device(
+                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
+                    source_net='vdd', drain_net='q',
+                ),
+                Wire(
+                    'POLY', 80, (56, 104), 4, False, name="pl_net0_1",
+                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
+                ),
             ],
             '_net1': [
-                Wire('PDIF', 36, (130, 162), 12, False),
+                Wire(
+                    'PDIF', 30, (130, 162), 3, False,
+                    conn={"left": "p_i0_1", "right": "p_i1_1"},
+                ),
             ],
             '_net2': [
-                Wire('NDIF', 14, (34, 46), 8, False),
-                Via('NDIF', 'METAL1', 16, 40, 2),
-                Wire('METAL1', (18, 58), 40, 6, False),
-                Via('NDIF', 'METAL1', 60, 40, 2),
-                Wire('NDIF', 60, (34, 46), 12, False),
+                Via(
+                    'NDIF', 'METAL1', 10, 40, 2, name="v_net2_ndif1",
+                    conn={"right": "n_i0_1"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 50, 40, 2,
+                    conn={"left": "n_i1_1", "right": "n_i2_1"},
+                ),
+                Wire('METAL1', (10, 50), 40, 6, False),
             ],
             'i0': [
-                Via('POLY', 'METAL1', 20, 80, 2),
-                Wire('METAL1', 20, (82, 138), 6, True),
-                Device('nmos', 24, 40, 4, 20, 'vertical', source_net='_net2', drain_net='_net0'),
-                Wire('POLY', 24, (56, 124), 4, False),
-                Device('pmos', 24, 146, 4, 40, 'vertical', source_net='vdd', drain_net='_net1'),
+                Wire(
+                    'METAL1', 10, (82, 138), 6, True,
+                    space={"top": "vddrail", "bottom": "v_net2_ndif1"},
+                ),
+                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i0_1"}),
+                Device(
+                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i0_1",
+                    source_net='_net2', drain_net='_net0',
+                ),
+                Device(
+                    'pmos', 20, 146, 4, 40, 'vertical', name="p_i0_1",
+                    source_net='vdd', drain_net='_net1',
+                ),
+                Wire(
+                    'POLY', 20, (56, 124), 4, False, name="pl_i0_1",
+                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
+                ),
             ],
             'i1': [
-                Via('POLY', 'METAL1', 40, 80, 2),
-                Via('POLY', 'METAL1', 40, 100, 2),
-                Wire('METAL1', 40, (82, 158), 6, True),
-                Wire('POLY', (40, 48), 104, 4, False),
-                Wire('POLY', (40, 52), 76, 4, False),
-                Wire('POLY', 48, (104, 122), 4, False),
-                Device('pmos', 48, 146, 4, 40, 'vertical', source_net='_net1', drain_net='_net0'),
-                Device('nmos', 52, 40, 4, 20, 'vertical', source_net='_net0', drain_net='_net2'),
-                Wire('POLY', 52, (56, 72), 4, False),
+                Wire(
+                    'METAL1', 30, (70, 158), 6, True, name="m1_i1_1",
+                    space={"top": "vddrail"},
+                ),
+                Via('POLY', 'METAL1', 32, 100, 2, conn={"right": "pl_i1_1"}),
+                Device(
+                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i1_1",
+                    source_net='_net0', drain_net='_net2',
+                ),
+                Device(
+                    'pmos', 40, 146, 4, 40, 'vertical', name="p_i1_1",
+                    source_net='_net1', drain_net='_net0',
+                ),
+                Wire(
+                    'POLY', 40, (56, 104), 4, False, name="pl_i1_1",
+                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
+                ),
             ],
             'i2': [
-                Device('nmos', 70, 40, 4, 20, 'vertical', source_net='_net2', drain_net='vss'),
-                Wire('POLY', 70, (52, 56), 4, False),
-                Wire('POLY', 70, (104, 124), 4, False),
-                Device('pmos', 70, 146, 4, 40, 'vertical', source_net='_net0', drain_net='vdd'),
-                Wire('POLY', (70, 80), 56, 4, False),
-                Wire('POLY', (70, 80), 104, 4, False),
-                Via('POLY', 'METAL1', 80, 60, 2),
-                Via('POLY', 'METAL1', 80, 100, 2),
-                Wire('METAL1', 80, (62, 158), 6, True),
+                Wire(
+                    'METAL1', 70, (62, 158), 6, True,
+                    space={"top": "vddrail", "bottom": "vssrail"}
+                ),
+                Via('POLY', 'METAL1', 68, 60, 2, conn={"left": "n_i2_1"}),
+                Via('POLY', 'METAL1', 68, 100, 2, conn={"left": "p_i2_1"}),
+                Device(
+                    'nmos', 60, 40, 4, 20, 'vertical', name="n_i2_1",
+                    source_net='_net2', drain_net='vss',
+                ),
+                Device(
+                    'pmos', 60, 146, 4, 40, 'vertical', name="p_i2_1",
+                    source_net='_net0', drain_net='vdd',
+                ),
             ],
             'q': [
-                Via('NDIF', 'METAL1', 100, 40, 2),
-                Wire('METAL1', 100, (42, 160), 6, True),
-                Via('PDIF', 'METAL1', 100, 120, 2),
-                Via('PDIF', 'METAL1', 100, 140, 2),
-                Via('PDIF', 'METAL1', 100, 160, 2),
-                Wire('NDIF', 104, (16, 46), 8, False),
-                Wire('PDIF', 104, (114, 186), 8, False),
+                Wire(
+                    'METAL1', 90, (42, 160), 6, True,
+                    space={"top": "vddrail", "bottom": "vssrail"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
+                    conn={"left": "n_net0_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
+                    conn={"left": "p_net0_1"},
+                ),
             ],
             'vdd': [
-                Wire('PDIF', 14, (130, 162), 8, False),
-                Via('PDIF', 'METAL1', 16, 160, 2),
-                Wire('METAL1', 16, (160, 176), 8, False),
-                Via('NTIE', 'METAL1', 36, 182, 2),
-                Wire('NTIE', (30, 66), 184, 8, False),
-                Via('NTIE', 'METAL1', 60, 182, 2),
-                Wire('PDIF', 82, (114, 186), 8, False),
-                Via('PDIF', 'METAL1', 84, 184, 2),
+                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_i0_1"}),
+                Via(
+                    'PDIF', 'METAL1', 70, 182, 2,
+                    conn={"left": "p_i2_1", "right": "p_net0_1", "up": "vddrail"},
+                ),
+                Via('NTIE', 'METAL1', 50, 184, 2),
+                Wire('NTIE', 50, (180, 188), 10, False),
             ],
             'vss': [
-                Wire('NDIF', 82, (16, 46), 8, False),
-                Via('NDIF', 'METAL1', 82, 40, 2),
-                Wire('METAL1', 84, (22, 40), 6, False),
+                Via(
+                    'NDIF', 'METAL1', 70, 18, 2,
+                    conn={"left": "n_i2_1", "right": "n_net0_1", "up": "vssrail"},
+                ),
+                Via('PTIE', 'METAL1', 50, 14, 2),
+                Wire('PTIE', 50, (10, 18), 10, False),
             ],
         },
         finalize=True,
     ),
     StdCell(
         name='ao22_x4', width=160, height=200,
         nets={
@@ -4984,14 +1817,377 @@
                 Wire('METAL1', 140, (22, 38), 6, False),
                 Via('NDIF', 'METAL1', 140, 40, 2),
             ],
         },
         finalize=True,
     ),
     StdCell(
+        name='mx3_x2', width=220, height=200,
+        nets={
+            '_net0': [
+                Via(
+                    'PDIF', 'METAL1', 30, 160, 2, name="v_net0_pdif1",
+                    space={"top": "vddrail"}, conn={"right": "p_i2_1"},
+                ),
+                Wire(
+                    'METAL1', (30, 110), 160, 6, False, name="m1_net0_1",
+                    # conn={"left": "v_net0_pdif1", "right": "v_net0_pdif2"},
+                ),
+                Via('PDIF', 'METAL1', 110, 160, 2, name="v_net0_pdif2",
+                    space={"top": "vddrail", "bottom": "m1_net5_1"},
+                    conn={"left": "p_i1_1", "right": "p_net4_1"},
+                ),
+            ],
+            '_net1': [
+                Via(
+                    'NDIF', 'METAL1', 30, 40, 2, name="v_net1_ndif1",
+                    space={"bottom": "vssrail"}, conn={"right": "n_i2_1"},
+                ),
+                Wire(
+                    'METAL1', (30, 110), 40, 6, False,
+                    conn={"left": "v_net1_ndif1", "right": "v_net1_ndif2"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 110, 40, 2, name="v_net1_ndif2",
+                    space={"bottom": "vssrail"},
+                    conn={"left": "n_i1_1", "right": "n_cmd0_2"},
+                ),
+            ],
+            '_net2': [
+                Wire(
+                    'PDIF', 150, (154, 186), 4, False,
+                    conn={"left": "p_cmd0_2", "right": "p_i0_1"},
+                ),
+            ],
+            '_net3': [
+                Via(
+                    'NDIF', 'METAL1', 30, 64, 2, name="v_net3_ndif1",
+                    conn={"left": "n_cmd1_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 30, 120, 2, name="v_net3_pdif1",
+                    space={"top": "m1_cmd1_1"}, conn={"left": "p_cmd1_1"},
+                ),
+                Wire(
+                    'METAL1', 30, (80, 100), 3, False, name="m1_net3_1",
+                    conn={"top": "v_net3_pdif1", "bottom": "v_net3_ndif1"},
+                ),
+                Wire(
+                    'METAL1', (36, 60), 60, 6, False, name="m1_net3_2",
+                    conn={"left": "v_net3_ndif1", "right": "v_net3_pl1"},
+                ),
+                Wire(
+                    'METAL1', (36, 70), 120, 6, False, name="m1_net3_3",
+                    conn={"left": "v_net3_pdif1", "right": "v_net3_pl2"},
+                ),
+                Via(
+                    'POLY', 'METAL1', 58, 60, 2, name="v_net3_pl1",
+                    conn={"right": "n_net3_1"},
+                ),
+                Device(
+                    'nmos', 60, 34, 4, 24, 'vertical', name="n_net3_1",
+                    source_net='_net9', drain_net='_net5',
+                ),
+                Via(
+                    'POLY', 'METAL1', 75, 120, 2, name="v_net3_pl2",
+                    conn={"right": "p_net3_1"},
+                ),
+                Device(
+                    'pmos', 80, 150, 4, 40, 'vertical', name="p_net3_1",
+                    source_net='_net5', drain_net='_net6',
+                ),
+            ],
+            '_net4': [
+                Via(
+                    'NDIF', 'METAL1', 170, 64, 2, name="v_net4_ndif1",
+                    conn={"right": "n_cmd0_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 170, 120, 2, name="v_net4_pdif1",
+                    space={"top": "m1_net5_1"}, conn={"right": "p_cmd0_1"},
+                ),
+                Wire(
+                    'METAL1', 170, (80, 100), 6, False,
+                    conn={"top": "v_net4_pdif1", "bottom": "v_net4_ndif1"},
+                ),
+                Device(
+                    'nmos', 140, 26, 4, 24, 'vertical', name="n_net4_1",
+                    source_net='vss', drain_net='_net7',    
+                ),
+                Device(
+                    'pmos', 120, 170, 4, 40, 'vertical', name="p_net4_1",
+                    source_net='_net0', drain_net='vdd',
+                ),
+                Via(
+                    'POLY', 'METAL1', 142, 60, 2, name="v_net4_pl1",
+                    conn={"left": "p_net4_1"},
+                ),
+                Wire(
+                    'METAL1', (140, 170), 60, 6, False, name="m1_net4_1",
+                    conn={"left":"v_net4_pl1", "right": "v_net4_ndif1"},
+                ),
+                Wire(
+                    'POLY', 140, (40, 60), False,
+                    conn={"top": "v_net4_pl1", "bottom": "n_net4_1"},
+                )
+            ],
+            '_net5': [
+                Device(
+                    'nmos', 200, 50, 4, 40, 'vertical', name="n_net5_1",
+                    source_net='vss', drain_net='q',
+                ),
+                Device(
+                    'pmos', 200, 150, 4, 80, 'vertical', name="p_net5_1",
+                    source_net='vdd', drain_net='q',
+                ),
+                Wire(
+                    'POLY', 200, (76, 104), 4, False, name="pl_net5_1",
+                    conn={"top": "p_net5_1", "bottom": "n_net5_1"},
+                ),
+                Via('POLY', 'METAL1', 192, 80, 2, conn={"right": "pl_net5_1"}),
+                Wire(
+                    'METAL1', 190, (42, 138), 6, False,
+                    conn={"top": "m1_net5_1", "bottom": "m1_net5_2"},
+                ),
+                Wire(
+                    'METAL1', (84, 190), 140, 6, False, name="m1_net5_1",
+                    conn={"left": "v_net5_pdif1"},
+                ),
+                Wire(
+                    'METAL1', (170, 190), 40, 6, False, name="m1_net5_2",
+                    conn={"left": "v_net5_ndif2"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 170, 34, 2, name="v_net5_ndif2",
+                    space={"bottom": "vssrail"}, conn={"left": "n_i0_1"},
+                ),
+                Wire(
+                    'METAL1', 170, (142, 158), 6, False,
+                    conn={"top": "v_net5_pdif2", "bottom": "m1_net5_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 170, 160, 2, name="v_net5_pdif2",
+                    space={"top": "vddrail"}, conn={"left": "p_i0_1"},
+                ),
+                Wire(
+                    'METAL1', 90, (62, 78), 6, False,
+                    conn={"top": "m1_net5_1", "bottom": "m1_net5_3"},
+                ),
+                Wire(
+                    'METAL1', (70, 90), 60, 6, False, name="m1_net5_3",
+                    conn={"left": "v_net5_ndif1"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 70, 60, 2, name="v_net5_ndif1",
+                    conn={"left": "n_net3_1", "right": "n_cmd1_2"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 70, 140, 2, name="v_net5_pdif1",
+                    space={"top": "m1_net0_1"},
+                    conn={"left": "p_cmd1_2", "right": "p_net3_1"},
+                ),
+            ],
+            '_net6': [
+                Wire(
+                    'PDIF', 90, (134, 166), 4, False,
+                    conn={"left": "p_net3_1", "right": "p_i1_1"},
+                ),
+            ],
+            '_net7': [
+                Wire(
+                    'NDIF', 150, (26, 36), 8, False,
+                    conn={"left": "n_net4_1", "right": "n_i0_1"},
+                ),
+            ],
+            '_net8': [
+                Wire(
+                    'PDIF', 50, (154, 186), 4, False,
+                    conn={"left": "p_i2_1", "right": "p_cmd1_2"},
+                ),
+            ],
+            '_net9': [
+                Wire(
+                    'NDIF', 50, (26, 42), 8, False,
+                    conn={"left": "n_i2_1", "right": "n_net3_1"},
+                ),
+            ],
+            '_net10': [
+                Wire(
+                    'NDIF', 90, (36, 52), 8, False,
+                    conn={"left": "n_cmd1_2", "right": "n_i1_1"},
+                ),
+            ],
+            'cmd0': [
+                Device(
+                    'nmos', 180, 64, 4, 12, 'vertical', name="n_cmd0_1",
+                    source_net='_net4', drain_net='vss',
+                ),
+                Device(
+                    'pmos', 180, 124, 4, 28, 'vertical', name="p_cmd0_1",
+                    source_net='_net4', drain_net='vdd',
+                ),
+                Wire(
+                    'POLY', 180, (76, 104), 4, False, name="pl_cmd0_1",
+                    conn={"top": "p_cmd0_1", "bottom": "n_cmd0_1"},
+                ),
+                Device(
+                    'pmos', 140, 170, 4, 40, 'vertical', name="p_cmd0_2",
+                    source_net='vdd', drain_net='_net2',
+                ),
+                Wire(
+                    'POLY', 140, (100, 140), 2, False,
+                    conn={"top": "p_cmd0_2"},
+                ),
+                Wire(
+                    'METAL1', 130, (82, 118), 6, True,
+                    space={"top": "m1_net5_1", "bottom": "vssrail"},
+                ),
+                Via('POLY', 'METAL1', 132, 100, 2, conn={"right": "pl_cmd0_1"}),
+                Via('POLY', 'METAL1', 128, 45, 2, conn={"left": "n_cmd0_2"}),
+                Device(
+                    'nmos', 120, 26, 4, 24, 'vertical', name="n_cmd0_2",
+                    source_net='_net1', drain_net='vss',
+                ),
+            ],
+            'cmd1': [
+                Wire(
+                    'METAL1', 10, (62, 140), 6, True, name="m1_cmd1_i",
+                    space={"top": "vddrail", "bottom": "vssrail"},
+                ),
+                Via('POLY', 'METAL1', 12, 100, 2, conn={"right": "pl_cmd1_1"}),
+                Device(
+                    'nmos', 20, 66, 4, 16, 'vertical', name="n_cmd1_1",
+                    source_net='vss', drain_net='_net3',
+                ),
+                Device(
+                    'pmos', 20, 124, 4, 28, 'vertical', name="p_cmd1_1",
+                    source_net='vdd', drain_net='_net3',
+                ),
+                Wire(
+                    'POLY', 20, (80, 104), 4, False, name="pl_cmd1_1",
+                    conn={"top": "p_cmd1_1", "bottom": "n_cmd1_1"},
+                ),
+                Wire(
+                    'METAL1', (12, 60), 140, 6, False, name="m1_cmd1_1",
+                    conn={"left": "m1_cmd1_i", "right": "v_cmd1_pl1"},
+                ),
+                Via('POLY', 'METAL1', 58, 140, 2, name="v_cmd1_pl1"),
+                Device(
+                    'pmos', 60, 170, 4, 40, 'vertical', name="p_cmd1_2",
+                    source_net='_net8', drain_net='_net5',
+                ),
+                Wire(
+                    'POLY', 60, (80, 140), 4, False,
+                    conn={"top": "p_cmd1_2", "bottom": "pl_cmd1_2"},
+                ),
+                Wire('POLY', (60, 80), 80, 4, False, name="pl_cmd1_2"),
+                Wire(
+                    'POLY', 80, (52, 80), 4, False,
+                    conn={"top": "pl_cmd1_2", "bottom": "n_cmd1_2"},
+                ),
+                Device(
+                    'nmos', 80, 44, 4, 24, 'vertical', name="n_cmd1_2",
+                    source_net='_net5', drain_net='_net10',
+                ),
+            ],
+            'i0': [
+                Device(
+                    'nmos', 160, 26, 4, 24, 'vertical', name="n_i0_1",
+                    source_net='_net7', drain_net='_net5',
+                ),
+                Device(
+                    'pmos', 160, 170, 4, 40, 'vertical', name="p_i0_1",
+                    source_net='_net2', drain_net='_net5',
+                ),
+                Via('POLY', 'METAL1', 152, 82, 2, conn={"right": "n_i0_1"}),
+                Via('POLY', 'METAL1', 152, 120, 2, conn={"right": "p_i0_1"}),
+                Wire(
+                    'METAL1', 150, (80, 120), 6, True,
+                    space={"top": "m1_net5_1", "bottom": "m1_net4_1"},
+                ),
+            ],
+            'i1': [
+                Device(
+                    'nmos', 100, 44, 4, 24, 'vertical', name="n_i1_1",
+                    source_net='_net10', drain_net='_net1',
+                ),
+                Device(
+                    'pmos', 100, 150, 4, 40, 'vertical', name="p_i1_1",
+                    source_net='_net6', drain_net='_net0',
+                ),
+                Wire(
+                    'POLY', 100, (52, 144), 4, False, name="pl_i1_1",
+                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
+                ),
+                Wire(
+                    'METAL1', 110, (80, 100), 3, True,
+                    space={"top": "m1_net5_1", "bottom": "v_net1_ndif2"},
+                ),
+                Via('POLY', 'METAL1', 108, 100, 2, conn={"left": "pl_i1_1"}),
+            ],
+            'i2': [
+                Device(
+                    'nmos', 40, 34, 4, 24, 'vertical', name="n_i2_1",
+                    source_net='_net1', drain_net='_net9',
+                ),
+                Device(
+                    'pmos', 40, 170, 4, 40, 'vertical', name="p_i2_1",
+                    source_net='_net0', drain_net='_net8',
+                ),
+                Wire(
+                    'POLY', 40, (52, 144), 4, False, name="pl_i2_1",
+                    conn={"top": "p_i2_1", "bottom": "n_i2_1"},
+                ),
+                Via('POLY', 'METAL1', 48, 100, 2, conn={"left": "pl_i2_1"}),
+                Wire(
+                    'METAL1', 50, (80, 100), 3, True,
+                    space={"top": "m1_net3_3", "bottom": "m1_net3_2"},
+                ),
+            ],
+            'q': [
+                Via('NDIF', 'METAL1', 210, 60, 2, conn={"left": "n_net5_1"}),
+                Via(
+                    'PDIF', 'METAL1', 210, 140, 2, space={"top": "vddrail"},
+                    conn={"left": "p_net5_1"},
+                ),
+                Wire(
+                    'METAL1', 210, (64, 160), 6, True,
+                    space={"top": "vddrail", "bottom": "vssrail"},
+                ),
+            ],
+            'vdd': [
+                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_cmd1_1"}),
+                Via('NTIE', 'METAL1', 90, 184, 2),
+                Wire('NTIE', 90, (180, 188), 8, False),
+                Via(
+                    'PDIF', 'METAL1', 130, 182, 2,
+                    conn={"left": "p_net4_1", "right": "p_cmd0_2"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 190, 182, 2, space={"bottom": "m1_net5_1"},
+                    conn={"left": "p_cmd0_1", "right": "p_net5_1"},
+                ),
+            ],
+            'vss': [
+                Via('NDIF', 'METAL1', 10, 18, 2, conn={"right": "n_cmd1_1"}),
+                Via('PTIE', 'METAL1', 90, 14, 2),
+                Wire('PTIE', 90, (10, 18), 8, False),
+                Via(
+                    'NDIF', 'METAL1', 130, 18, 2,
+                    conn={"left": "n_cmd0_2", "right": "n_net4_1", "up": "vssrail"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 190, 18, 2,
+                    conn={"left": "n_cmd0_1", "right": "n_net5_1"},
+                ),
+            ],
+        },
+        finalize=True,
+    ),
+    StdCell(
         name='mx3_x2', width=260, height=200,
         nets={
             '_net0': [
                 Wire('PDIF', 48, (154, 186), 8, False),
                 Via('PDIF', 'METAL1', 50, 160, 2),
                 Wire('METAL1', (52, 130), 160, 6, False),
                 Via('PDIF', 'METAL1', 132, 160, 2),
@@ -9726,88 +6922,149 @@
                 Via('NDIF', 'METAL1', 144, 18, 2),
                 Wire('NDIF', 146, (16, 46), 8, False),
             ],
         },
         finalize=True,
     ),
     StdCell(
-        name='oa22_x2', width=120, height=200,
+        name='ao22_x2', width=100, height=200,
         nets={
             '_net0': [
-                Wire('PDIF', 36, (134, 166), 8, False),
-                Via('PDIF', 'METAL1', 38, 140, 2),
-                Wire('METAL1', (38, 58), 140, 6, False),
-                Via('NDIF', 'METAL1', 60, 40, 2),
-                Wire('NDIF', 60, (34, 46), 8, False),
-                Via('POLY', 'METAL1', 60, 80, 2),
-                Wire('METAL1', 60, (42, 138), 6, False),
-                Wire('POLY', (60, 92), 80, 4, False),
-                Device('nmos', 92, 31, 4, 38, 'vertical', source_net='vss', drain_net='q'),
-                Wire('POLY', 92, (56, 104), 4, False),
-                Device('pmos', 92, 150, 4, 80, 'vertical', source_net='vdd', drain_net='q'),
+                Via(
+                    'NDIF', 'METAL1', 30, 60, 2, name="v_net0_ndif1",
+                    space={"top": "m1_i1_1", "bottom": "vssrail"},
+                    conn={"left": "n_i0_1", "right": "n_i1_1"},
+                ),
+                Wire(
+                    'METAL1', (30, 50), 60, 3, False, name="m1_net0_1",
+                    conn={"left": "v_net0_ndif1"},
+                ),
+                Wire(
+                    'METAL1', 50, (60, 100), 3, False,
+                    conn={"top": "v_net0_pdif1", "bottom": "m1_net0_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 50, 140, 2, name="v_net0_pdif1",
+                    conn={"left": "p_i1_1", "right": "p_i2_1"},
+                ),
+                Via('POLY', 'METAL1', 52, 80, 2, conn={"right": "pl_net0_1"}),
+                Device(
+                    'nmos', 80, 31, 4, 38, 'vertical', name="n_net0_1",
+                    source_net='vss', drain_net='q',
+                ),
+                Device(
+                    'pmos', 80, 150, 4, 80, 'vertical', name="p_net0_1",
+                    source_net='vdd', drain_net='q',
+                ),
+                Wire(
+                    'POLY', 80, (56, 104), 4, False, name="pl_net0_1",
+                    conn={"top": "p_net0_1", "bottom": "n_net0_1"},
+                ),
             ],
             '_net1': [
-                Wire('PDIF', 18, (134, 166), 12, False),
-                Via('PDIF', 'METAL1', 20, 140, 2),
-                Wire('METAL1', 20, (142, 158), 6, False),
-                Via('PDIF', 'METAL1', 20, 160, 2),
-                Wire('METAL1', (14, 58), 160, 6, False),
-                Wire('PDIF', 60, (134, 166), 8, False),
-                Via('PDIF', 'METAL1', 60, 160, 2),
+                Wire(
+                    'PDIF', 30, (130, 162), 3, False,
+                    conn={"left": "p_i0_1", "right": "p_i1_1"},
+                ),
             ],
             '_net2': [
-                Wire('NDIF', 36, (16, 46), 8, False),
+                Via(
+                    'NDIF', 'METAL1', 10, 40, 2, name="v_net2_ndif1",
+                    conn={"right": "n_i0_1"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 50, 40, 2,
+                    conn={"left": "n_i1_1", "right": "n_i2_1"},
+                ),
+                Wire('METAL1', (10, 50), 40, 6, False),
             ],
             'i0': [
-                Wire('METAL1', 20, (42, 118), 6, True),
-                Via('POLY', 'METAL1', 20, 80, 2),
-                Wire('POLY', 20, (56, 124), 4, False),
-                Wire('POLY', (20, 28), 56, 4, False),
-                Wire('POLY', (20, 28), 124, 4, False),
-                Device('nmos', 28, 31, 4, 38, 'vertical', source_net='vss', drain_net='_net2'),
-                Device('pmos', 28, 150, 4, 40, 'vertical', source_net='_net1', drain_net='_net0'),
+                Wire(
+                    'METAL1', 10, (82, 138), 6, True,
+                    space={"top": "vddrail", "bottom": "v_net2_ndif1"},
+                ),
+                Via('POLY', 'METAL1', 12, 80, 2, conn={"right": "pl_i0_1"}),
+                Device(
+                    'nmos', 20, 40, 4, 20, 'vertical', name="n_i0_1",
+                    source_net='_net2', drain_net='_net0',
+                ),
+                Device(
+                    'pmos', 20, 146, 4, 40, 'vertical', name="p_i0_1",
+                    source_net='vdd', drain_net='_net1',
+                ),
+                Wire(
+                    'POLY', 20, (56, 124), 4, False, name="pl_i0_1",
+                    conn={"top": "p_i0_1", "bottom": "n_i0_1"},
+                ),
             ],
             'i1': [
-                Via('POLY', 'METAL1', 40, 60, 2),
-                Wire('METAL1', 40, (42, 118), 6, True),
-                Via('POLY', 'METAL1', 40, 120, 2),
-                Wire('POLY', (40, 48), 124, 4, False),
-                Wire('POLY', (40, 50), 56, 4, False),
-                Device('pmos', 48, 150, 4, 40, 'vertical', source_net='_net0', drain_net='_net1'),
-                Device('nmos', 50, 31, 4, 38, 'vertical', source_net='_net2', drain_net='_net0'),
+                Wire(
+                    'METAL1', 30, (70, 158), 6, True, name="m1_i1_1",
+                    space={"top": "vddrail"},
+                ),
+                Via('POLY', 'METAL1', 32, 100, 2, conn={"right": "pl_i1_1"}),
+                Device(
+                    'nmos', 40, 40, 4, 20, 'vertical', name="n_i1_1",
+                    source_net='_net0', drain_net='_net2',
+                ),
+                Device(
+                    'pmos', 40, 146, 4, 40, 'vertical', name="p_i1_1",
+                    source_net='_net1', drain_net='_net0',
+                ),
+                Wire(
+                    'POLY', 40, (56, 104), 4, False, name="pl_i1_1",
+                    conn={"top": "p_i1_1", "bottom": "n_i1_1"},
+                ),
             ],
             'i2': [
-                Device('nmos', 68, 31, 4, 38, 'vertical', source_net='_net0', drain_net='vss'),
-                Wire('POLY', 68, (54, 58), 4, False),
-                Wire('POLY', 68, (100, 124), 4, False),
-                Device('pmos', 68, 150, 4, 40, 'vertical', source_net='_net1', drain_net='vdd'),
-                Wire('POLY', (68, 76), 60, 8, False),
-                Wire('POLY', (72, 80), 100, 8, False),
-                Via('POLY', 'METAL1', 80, 60, 2),
-                Wire('METAL1', 80, (42, 158), 6, True),
-                Via('POLY', 'METAL1', 80, 100, 2),
+                Wire(
+                    'METAL1', 70, (62, 158), 6, True,
+                    space={"top": "vddrail", "bottom": "vssrail"}
+                ),
+                Via('POLY', 'METAL1', 68, 60, 2, conn={"left": "n_i2_1"}),
+                Via('POLY', 'METAL1', 68, 100, 2, conn={"left": "p_i2_1"}),
+                Device(
+                    'nmos', 60, 40, 4, 20, 'vertical', name="n_i2_1",
+                    source_net='_net2', drain_net='vss',
+                ),
+                Device(
+                    'pmos', 60, 146, 4, 40, 'vertical', name="p_i2_1",
+                    source_net='_net0', drain_net='vdd',
+                ),
             ],
             'q': [
-                Via('NDIF', 'METAL1', 100, 40, 2),
-                Wire('METAL1', 100, (42, 158), 6, True),
-                Via('PDIF', 'METAL1', 100, 120, 2),
-                Via('PDIF', 'METAL1', 100, 140, 2),
-                Via('PDIF', 'METAL1', 100, 160, 2),
-                Wire('NDIF', 104, (16, 46), 12, False),
-                Wire('PDIF', 104, (114, 186), 12, False),
+                Wire(
+                    'METAL1', 90, (42, 160), 6, True,
+                    space={"top": "vddrail", "bottom": "vssrail"},
+                ),
+                Via(
+                    'NDIF', 'METAL1', 90, 40, 2, space={"bottom": "vssrail"},
+                    conn={"left": "n_net0_1"},
+                ),
+                Via(
+                    'PDIF', 'METAL1', 90, 140, 2, space={"top": "vddrail"},
+                    conn={"left": "p_net0_1"},
+                ),
             ],
             'vdd': [
-                Wire('PDIF', 82, (114, 186), 8, False),
-                Via('PDIF', 'METAL1', 84, 184, 2),
+                Via('PDIF', 'METAL1', 10, 182, 2, conn={"right": "p_i0_1"}),
+                Via(
+                    'PDIF', 'METAL1', 70, 182, 2,
+                    conn={"left": "p_i2_1", "right": "p_net0_1", "up": "vddrail"},
+                ),
+                Via('NTIE', 'METAL1', 50, 184, 2),
+                Wire('NTIE', 50, (180, 188), 10, False),
             ],
             'vss': [
-                Wire('NDIF', 14, (16, 46), 8, False),
-                Via('NDIF', 'METAL1', 18, 18, 2),
-                Via('NDIF', 'METAL1', 84, 18, 2),
-                Wire('NDIF', 84, (16, 46), 12, False),
+                Via(
+                    'NDIF', 'METAL1', 70, 18, 2,
+                    conn={"left": "n_i2_1", "right": "n_net0_1", "up": "vssrail"},
+                ),
+                Via('PTIE', 'METAL1', 50, 14, 2),
+                Wire('PTIE', 50, (10, 18), 10, False),
             ],
         },
         finalize=True,
     ),
     StdCell(
         name='oa22_x4', width=160, height=200,
         nets={
@@ -11494,20 +8751,14 @@
             '_net1': [
                 Wire('PDIF', 132, (154, 186), 4, False),
                 Wire('PDIF', 136, (134, 186), 8, False),
             ],
             '_net2': [
                 Wire('NDIF', 132, (34, 46), 8, False),
             ],
-            '_net3': [
-                Device('nmos', 284, 40, 4, 20, 'vertical', source_net='_net6', drain_net='vss'),
-                Wire('POLY', 284, (54, 58), 4, False),
-                Wire('POLY', (284, 290), 58, 4, False),
-                Via('POLY', 'METAL1', 290, 60, 2),
-            ],
             '_net4': [
                 Wire('NDIF', 180, (16, 46), 12, False),
             ],
             '_net5': [
                 Wire('PDIF', 182, (134, 186), 8, False),
             ],
             '_net6': [
```

### Comparing `c4m_flexcell-0.3.3/c4m/flexcell/canvas.py` & `c4m_flexcell-0.4.0.dev3/c4m/flexcell/canvas.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
-from typing import Optional
+from typing import Optional, Any
 
 from pdkmaster.typing import OptMultiT, cast_OptMultiT, cast_OptMultiT_n
 from pdkmaster.technology import (
     property_ as _prp, geometry as _geo, primitive as _prm, technology_ as _tch,
 )
 from pdkmaster.design import routinggauge as _rg
 
@@ -96,14 +96,18 @@
                     f"l {l}um smaller than min. nmos transistor l {nmos.computed.min_l}um",
                 )
             if l//_geo.epsilon < pmos.computed.min_l//_geo.epsilon:
                 raise ValueError(
                     f"l {l}um smaller than min. pmos transistor l {nmos.computed.min_l}um",
                 )
 
+        self._balancedmos_w_ratio = r = 2.0
+        self._nmos_min_w = 20*lambda_
+        self._pmos_min_w = r*20*lambda_
+
         inside = cast_OptMultiT(inside)
         if inside is None:
             if inside_enclosure is not None:
                 raise ValueError("inside_enclosure provided with inside")
         else:
             if inside_enclosure is None:
                 inside_enclosure = _prp.Enclosure(0.0)
@@ -135,14 +139,34 @@
         self._min_active_well_enclosure = active.min_well_enclosure[idx].max()
         self._poly = poly = nmos.gate.poly
         if poly != pmos.gate.poly:
             raise NotImplementedError(
                 "Different poly wire for nmos and pmos transistor"
             )
 
+        self._min_active_poly_space = tech.computed.min_space(active, poly)
+
+        # Draw SD regions with vertical implant enclosure the same as the
+        # gate implant enclosure
+        gate_enc = nmos.min_gateimplant_enclosure[0]
+        idx = active.implant.index(nimplant)
+        act_enc = active.min_implant_enclosure[idx]
+        self._min_active_nimplant_enc = act_enc
+        self._min_nsd_enc = _prp.Enclosure((
+            act_enc.first, max(act_enc.min(), gate_enc.second),
+        ))
+
+        gate_enc = nmos.min_gateimplant_enclosure[0]
+        idx = active.implant.index(pimplant)
+        act_enc = active.min_implant_enclosure[idx]
+        self._min_active_pimplant_enc = act_enc
+        self._min_psd_enc = _prp.Enclosure((
+            act_enc.first, max(act_enc.min(), gate_enc.second),
+        ))
+
         self._vias = vias = tuple(tech.primitives.__iter_type__(_prm.Via))
         self._contact = cont = vias[0]
         min_contact_active_space = None
         try:
             min_contact_active_space = tech.computed.min_space(
                 primitive1=cont, primitive2=active,
             )
@@ -171,14 +195,18 @@
                         min_contact_active_space = enc + s + polyenc
                     else:
                         min_contact_active_space = max(
                             min_contact_active_space,
                             enc + s + polyenc,
                         )
         self._min_contact_active_space = min_contact_active_space
+        idx = cont.bottom.index(active)
+        self._min_contact_active_enclosure = cont.min_bottom_enclosure[idx]
+        idx = cont.bottom.index(poly)
+        self._min_contact_poly_enclosure = cont.min_bottom_enclosure[idx]
         self._via1 = via1 = vias[1]
         self._via2 = via2 = vias[2]
         for v in (cont, via1, via2):
             if len(v.top) != 1:
                 raise NotImplementedError(
                     f"Number of top layers for contact/via '{v.name}' not 1"
                 )
@@ -191,14 +219,15 @@
         if not isinstance(metal1, _prm.MetalWire):
             raise ValueError(
                 "top contact layer is not of type 'MetalWire' but of type "
                 f"'{type(metal1)}'"
             )
         self._metal1 = metal1
         self._metal1pin = metal1.pin
+        self._min_contact_metal1_enclosure = cont.min_top_enclosure[0]
         metal2 = via1.top[0]
         if not isinstance(metal2, _prm.MetalWire):
             raise ValueError(
                 "top via1 layer is not of type 'MetalWire' but of type "
                 f"'{type(metal2)}'"
             )
         self._metal2 = metal2
@@ -209,25 +238,29 @@
                 "top via2 layer is not of type 'MetalWire' but of type "
                 f"'{type(metal3)}'"
             )
         self._metal3 = metal3
         self._metal3pin = metal3.pin
 
         enc = via1.min_bottom_enclosure[0].min()
-        self._pin_width = via1.width + 2*enc
+        self._pin_width = tech.computed.min_width(
+            metal1, up=True, down=True, min_enclosure=True,
+        )
 
         self._cell_height = 200*lambda_
         self._cell_horplacement_grid = 20*lambda_
         self._m1_vssrail_width = 24*lambda_
         self._m1_vddrail_width = 24*lambda_
         self._well_edge_height = 96*lambda_
-        self._balancedmos_w_ratio = 2.0
 
         self._min_tap_chs = 2 # Should be high enough for min. diffusion area
 
+        # ActiveColumsCell specific values
+        self._ac_canvas: Any = None
+
     @property
     def tech(self) -> _tch.Technology:
         return self._tech
     @property
     def lambda_(self) -> float:
         return self._lambda
     @property
```

### Comparing `c4m_flexcell-0.3.3/c4m/flexcell/stdcell.py` & `c4m_flexcell-0.4.0.dev3/c4m/flexcell/stdcell.py`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/c4m_flexcell.egg-info/PKG-INFO` & `c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4m-flexcell
-Version: 0.3.3
+Version: 0.4.0.dev3
 Summary: PDKMaster based scalable standard cell library
 Author: Staf Verhaegen
 Author-email: staf@fibraservi.eu
 License: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 Project-URL: Source Code, https://gitlab.com/Chips4Makers/c4m-flexcell
 Project-URL: Bug Tracker, https://gitlab.com/Chips4Makers/c4m-flexcell/issues
 Requires-Python: ~=3.6
@@ -15,15 +15,14 @@
 
 A standard cell library is a collection of cells that perform certain digital functions. It consists of so-called combinatorial cells which perform a binary logic function and sequential cells sync internal signal with a clock signal.
 
 Standard cells are introduced into an [ASIC](https://en.wikipedia.org/wiki/Application-specific_integrated_circuit) [EDA](https://en.wikipedia.org/wiki/Electronic_design_automation) flow during the synthesis step. This is the step where a (RTL) logic design into a netlist consisting only of the cells from your standard cell library. Later on these cells are then placed next to each and the inputs and outputs of each cell connected to each other. The former is called placement and the latter routing.
 
 ## Release History
 
-* v0.3.3: bug fix; remove public 0.3.2 release
 * v0.3.2: code cleansing, bug fixing, update dependencies
 * v0.3.1: small update for Coriolis export
 * v0.3.0: Update for [release v0.9.0 of PDKMaster](https://gitlab.com/Chips4Makers/PDKMaster/-/blob/v0.9.0/ReleaseNotes/v0.9.0.md); replace Library-> StdCellFactory to follow common usage of a factory to generate cells.
 * v0.2.0: Small updates for changing PDKMaster API
 * [v0.1.0](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.1.0.md)
 * [v0.0.4](https://gitlab.com/Chips4Makers/c4m-flexcell/-/blob/v0.1.0/ReleaseNotes/v0.0.4.md)
 
@@ -33,9 +32,11 @@
 Alternative implementations try to fully automate the layout generation out of the transistor netlist. Finding a good placement of the transistor for non-trivial logic cells is a hard problem leading often to complex code for finding acceptable solutions. Also the layout code itself often becomes complex to take peculiarities of different design rules into account.  
 The `flexcell` library tries to take a middle road. It will start from a topological layout of the cell but without the layout already fixed to certain design rules; it thus avoid the step where netlist need to be converted to topologies. It will use the design rules from a PDKMaster Technology object to generate an optimized layout for conforming to the cells topology. By baking in independence of the Technology the standard cell library should be easily ported to different technologies with better area efficiency than current [lambda rules](http://www.electronics-tutorial.net/Digital-CMOS-Design/CMOS-Layout-Design/CMOS-lambda-Design-Rules/) based solutions.  
 In future options are planned so libraries can be generated for different targets like ,minimum area, maximum performance or minimum power consumption.
 
 ## Status
 
 This repository is currently considered experimental code with no backwards compatibility guarantees whatsoever.  
+This development is done in a development branch for new layout generation code.
+When this development is done it will be released as version 0.4.0.  
 Current implementation is based on the topology of the Coriolis nsxlib standard cells with some area improvements but not yet with optimal area use. For v0.1 of this library a total replacement of the layout generation is planned fully based on minimized area for the technology design rules.  
 If interested head over to [gitter](https://gitter.im/Chips4Makers/community) for further discussion.
```

### Comparing `c4m_flexcell-0.3.3/c4m_flexcell.egg-info/SOURCES.txt` & `c4m_flexcell-0.4.0.dev3/c4m_flexcell.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 LICENSES/gpl-2.0.txt
 ReleaseNotes/v0.0.4.md
 ReleaseNotes/v0.1.0.md
 c4m/__init__.py
 c4m/cell_canvas.ipynb
 c4m/flexcell/__init__.py
 c4m/flexcell/_cells.py
+c4m/flexcell/activecolumnscell.py
 c4m/flexcell/canvas.py
 c4m/flexcell/cell.py
 c4m/flexcell/factory.py
 c4m/flexcell/stdcell.py
 c4m_flexcell.egg-info/PKG-INFO
 c4m_flexcell.egg-info/SOURCES.txt
 c4m_flexcell.egg-info/dependency_links.txt
```

### Comparing `c4m_flexcell-0.3.3/dodo.py` & `c4m_flexcell-0.4.0.dev3/dodo.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,10 +86,9 @@
 
     return {
         "title": lambda _: "Installing python module",
         "file_dep": c4m_py_files,
         "targets": (flexcell_inst_dir,),
         "actions": (
             f"{pip} install --no-deps {top_dir}",
-            f"{pip} check",
         ),
     }
```

### Comparing `c4m_flexcell-0.3.3/setup.py` & `c4m_flexcell-0.4.0.dev3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-License-Identifier: GPL-2.0-or-later OR AGPL-3.0-or-later OR CERN-OHL-S-2.0+
 from setuptools import setup, find_packages
 
 def local_scheme(version):
     if version.tag and not version.distance:
         return version.format_with("")
     else:
-        return version.format_choice("+{node}", "+{node}.dirty")
+        return version.format_choice("", "+{node}.dirty")
 
 # Don't seem to have much success with exclude parameter of find_packages()
 _packages = list(filter(lambda pkg: pkg[:4] != "test", find_packages()))
 
 with open("README.md", "r") as f:
     long_description = f.read()
```

### Comparing `c4m_flexcell-0.3.3/test/interactive/export.ipynb` & `c4m_flexcell-0.4.0.dev3/test/interactive/export.ipynb`

 * *Files identical despite different names*

### Comparing `c4m_flexcell-0.3.3/test/unit/test_library.py` & `c4m_flexcell-0.4.0.dev3/test/unit/test_library.py`

 * *Files identical despite different names*

