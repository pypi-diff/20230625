# Comparing `tmp/vollseg-napari-mtrack-1.3.6.tar.gz` & `tmp/vollseg-napari-mtrack-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-mtrack/dist/.tmp-ug176kam/vollseg-napari-mtrack-1.3.6.tar", last modified: Sun Jun 25 12:56:50 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-mtrack/dist/.tmp-_kq026gi/vollseg-napari-mtrack-1.4.2.tar", last modified: Sun Jun 25 13:14:53 2023, max compression
```

## Comparing `vollseg-napari-mtrack-1.3.6.tar` & `vollseg-napari-mtrack-1.4.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:50.060501 vollseg-napari-mtrack-1.3.6/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:48.753104 vollseg-napari-mtrack-1.3.6/.github/
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:48.972383 vollseg-napari-mtrack-1.3.6/.github/workflows/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-11-17 16:36:37.000000 vollseg-napari-mtrack-1.3.6/.gitignore
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:49.049710 vollseg-napari-mtrack-1.3.6/.napari-hub/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/.napari-hub/config.yml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-10-28 15:57:24.000000 vollseg-napari-mtrack-1.3.6/.pre-commit-config.yaml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.6/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.6/MANIFEST.in
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 12:56:50.062837 vollseg-napari-mtrack-1.3.6/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2927 2022-10-28 20:45:44.000000 vollseg-napari-mtrack-1.3.6/README.md
--rwxrwxrwx   0 debian    (1000) debian    (1000)      271 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.6/pyproject.toml
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1919 2023-06-25 12:56:50.072903 vollseg-napari-mtrack-1.3.6/setup.cfg
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:49.078300 vollseg-napari-mtrack-1.3.6/src/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      217 2022-12-22 18:14:03.000000 vollseg-napari-mtrack-1.3.6/src/launch.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:49.367102 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/
--rwxrwxrwx   0 debian    (1000) debian    (1000)      518 2023-01-27 10:34:59.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2442 2022-12-24 10:29:19.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2128 2023-01-27 15:48:38.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_temporal_plots.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:49.961308 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/
--rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 18:41:12.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/test_reader.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      112 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/test_sample_data.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      488 2023-01-07 18:42:26.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/test_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      130 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/test_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      605 2022-12-29 12:49:22.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/utils.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_version.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    62812 2023-06-25 12:56:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_widget.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_writer.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1538 2022-12-21 12:24:27.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/napari.yaml
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:50.015977 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/resources/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/resources/kapoorlogo.png
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:56:49.616081 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1142 2023-06-25 12:56:48.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       76 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       22 2023-06-25 12:56:47.000000 vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)      616 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.6/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:53.334034 vollseg-napari-mtrack-1.4.2/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:51.916303 vollseg-napari-mtrack-1.4.2/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:52.171640 vollseg-napari-mtrack-1.4.2/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-11-17 16:36:37.000000 vollseg-napari-mtrack-1.4.2/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:52.236609 vollseg-napari-mtrack-1.4.2/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-10-28 15:57:24.000000 vollseg-napari-mtrack-1.4.2/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.4.2/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.4.2/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 13:14:53.336032 vollseg-napari-mtrack-1.4.2/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2927 2022-10-28 20:45:44.000000 vollseg-napari-mtrack-1.4.2/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      271 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.4.2/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1919 2023-06-25 13:14:53.347906 vollseg-napari-mtrack-1.4.2/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:52.269014 vollseg-napari-mtrack-1.4.2/src/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      217 2022-12-22 18:14:03.000000 vollseg-napari-mtrack-1.4.2/src/launch.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:52.596640 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      518 2023-01-27 10:34:59.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2442 2022-12-24 10:29:19.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2128 2023-01-27 15:48:38.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:53.211340 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 18:41:12.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      112 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      488 2023-01-07 18:42:26.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      130 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      605 2022-12-29 12:49:22.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/utils.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    62772 2023-06-25 13:14:11.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1538 2022-12-21 12:24:27.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:53.276415 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 13:14:52.859477 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1142 2023-06-25 13:14:51.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       76 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       22 2023-06-25 13:14:50.000000 vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      616 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.4.2/tox.ini
```

### Comparing `vollseg-napari-mtrack-1.3.6/.github/workflows/test_and_deploy.yml` & `vollseg-napari-mtrack-1.4.2/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/.gitignore` & `vollseg-napari-mtrack-1.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/.napari-hub/config.yml` & `vollseg-napari-mtrack-1.4.2/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/.pre-commit-config.yaml` & `vollseg-napari-mtrack-1.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/LICENSE` & `vollseg-napari-mtrack-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/PKG-INFO` & `vollseg-napari-mtrack-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-mtrack
-Version: 1.3.6
+Version: 1.4.2
 Summary: Segment kymographs of microtubules, actin filaments and perform Ransac based fits to compute dynamic instability parameters for individual kymographs and also in batch
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack#README.md
```

### Comparing `vollseg-napari-mtrack-1.3.6/README.md` & `vollseg-napari-mtrack-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/setup.cfg` & `vollseg-napari-mtrack-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/__init__.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/__init__.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_reader.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_reader.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_sample_data.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_temporal_plots.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_tests/utils.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_widget.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,26 +168,22 @@
             orientation="horizontal",
             choices=ransac_model_type_choices,
             value=DEFAULTS_MODEL["ransac_model_type"],
         ),
         defaults_params_button=dict(
             widget_type="PushButton", text="Restore Parameter Defaults"
         ),
-        progress_bar=dict(label=" ", min=0, max=0, visible=False),
-        layout="vertical",
-        persist=False,
         call_button=False,
     )
     def plugin_ransac_parameters(
         max_error,
         min_num_time_points,
         time_axis,
         ransac_model_type,
         defaults_params_button,
-        progress_bar: mw.ProgressBar,
     ) -> List[napari.types.LayerDataTuple]:
 
         return plugin_ransac_parameters
 
     kapoorlogo = abspath(__file__, "resources/kapoorlogo.png")
     citation = Path("https://doi.org/10.1038/s41598-018-37767-1")
 
@@ -729,14 +725,16 @@
 
     def _refreshTableData(df: pd.DataFrame):
 
         table_tab.data = pandasModel(df)
         table_tab.viewer = plugin.viewer.value
         table_tab.time_key = "File_Index"
         table_tab._set_model()
+        if plot_class.scroll_layout.count() > 0:
+            plot_class._reset_container(plot_class.scroll_layout)
         _refreshPlotData(df)
 
     def select_model_ransac(key):
         nonlocal model_selected_ransac
         model_selected_ransac = key
 
     def widgets_inactive(*widgets, active):
```

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/_writer.py` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/napari.yaml` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack/resources/kapoorlogo.png` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/PKG-INFO` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-mtrack
-Version: 1.3.6
+Version: 1.4.2
 Summary: Segment kymographs of microtubules, actin filaments and perform Ransac based fits to compute dynamic instability parameters for individual kymographs and also in batch
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack#README.md
```

### Comparing `vollseg-napari-mtrack-1.3.6/src/vollseg_napari_mtrack.egg-info/SOURCES.txt` & `vollseg-napari-mtrack-1.4.2/src/vollseg_napari_mtrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.6/tox.ini` & `vollseg-napari-mtrack-1.4.2/tox.ini`

 * *Files identical despite different names*

