# Comparing `tmp/vollseg-napari-mtrack-1.3.3.tar.gz` & `tmp/vollseg-napari-mtrack-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-mtrack/dist/.tmp-x14qv95x/vollseg-napari-mtrack-1.3.3.tar", last modified: Fri Jan 27 15:52:59 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/vollseg-napari-mtrack/dist/.tmp-uhqqnw0q/vollseg-napari-mtrack-1.3.5.tar", last modified: Sun Jun 25 12:47:09 2023, max compression
```

## Comparing `vollseg-napari-mtrack-1.3.3.tar` & `vollseg-napari-mtrack-1.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:59.505247 vollseg-napari-mtrack-1.3.3/
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:58.382366 vollseg-napari-mtrack-1.3.3/.github/
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:58.589856 vollseg-napari-mtrack-1.3.3/.github/workflows/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     2814 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/.github/workflows/test_and_deploy.yml
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      992 2022-11-17 16:36:37.000000 vollseg-napari-mtrack-1.3.3/.gitignore
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:58.645424 vollseg-napari-mtrack-1.3.3/.napari-hub/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      463 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/.napari-hub/DESCRIPTION.md
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      542 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/.napari-hub/config.yml
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1211 2022-10-28 15:57:24.000000 vollseg-napari-mtrack-1.3.3/.pre-commit-config.yaml
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1487 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.3/LICENSE
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       96 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.3/MANIFEST.in
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     4385 2023-01-27 15:52:59.506499 vollseg-napari-mtrack-1.3.3/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     2927 2022-10-28 20:45:44.000000 vollseg-napari-mtrack-1.3.3/README.md
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      271 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.3/pyproject.toml
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1919 2023-01-27 15:52:59.515618 vollseg-napari-mtrack-1.3.3/setup.cfg
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:58.671815 vollseg-napari-mtrack-1.3.3/src/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      217 2022-12-22 18:14:03.000000 vollseg-napari-mtrack-1.3.3/src/launch.py
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:58.950709 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      518 2023-01-27 10:34:59.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/__init__.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     2442 2022-12-24 10:29:19.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_reader.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      644 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_sample_data.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     2128 2023-01-27 15:48:38.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_temporal_plots.py
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:59.424200 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/__init__.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      107 2023-01-07 18:41:12.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/test_reader.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      112 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/test_sample_data.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      488 2023-01-07 18:42:26.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/test_widget.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      130 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/test_writer.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      605 2022-12-29 12:49:22.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/utils.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      160 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_version.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    63006 2023-01-27 15:50:43.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_widget.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      923 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_writer.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1538 2022-12-21 12:24:27.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/napari.yaml
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:59.467164 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/resources/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/resources/kapoorlogo.png
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2023-01-27 15:52:59.163022 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     4385 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1142 2023-01-27 15:52:58.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/SOURCES.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        1 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/dependency_links.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       76 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/entry_points.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       85 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/requires.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       22 2023-01-27 15:52:57.000000 vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/top_level.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      616 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.3/tox.ini
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:09.537707 vollseg-napari-mtrack-1.3.5/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:08.230841 vollseg-napari-mtrack-1.3.5/.github/
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:08.484889 vollseg-napari-mtrack-1.3.5/.github/workflows/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2814 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/.github/workflows/test_and_deploy.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      992 2022-11-17 16:36:37.000000 vollseg-napari-mtrack-1.3.5/.gitignore
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:08.548429 vollseg-napari-mtrack-1.3.5/.napari-hub/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      463 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/.napari-hub/DESCRIPTION.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      542 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/.napari-hub/config.yml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1211 2022-10-28 15:57:24.000000 vollseg-napari-mtrack-1.3.5/.pre-commit-config.yaml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1487 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.5/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       96 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.5/MANIFEST.in
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 12:47:09.539707 vollseg-napari-mtrack-1.3.5/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2927 2022-10-28 20:45:44.000000 vollseg-napari-mtrack-1.3.5/README.md
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      271 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.5/pyproject.toml
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1919 2023-06-25 12:47:09.549716 vollseg-napari-mtrack-1.3.5/setup.cfg
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:08.578242 vollseg-napari-mtrack-1.3.5/src/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      217 2022-12-22 18:14:03.000000 vollseg-napari-mtrack-1.3.5/src/launch.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:08.867687 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      518 2023-01-27 10:34:59.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2442 2022-12-24 10:29:19.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      644 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2128 2023-01-27 15:48:38.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_temporal_plots.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:09.429844 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        0 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      107 2023-01-07 18:41:12.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/test_reader.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      112 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/test_sample_data.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      488 2023-01-07 18:42:26.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/test_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      130 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/test_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      605 2022-12-29 12:49:22.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/utils.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      160 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    62783 2023-06-25 12:46:15.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_widget.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      923 2022-10-28 14:14:01.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_writer.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1538 2022-12-21 12:24:27.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/napari.yaml
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:09.492709 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/resources/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6153 2022-03-22 02:26:26.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/resources/kapoorlogo.png
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:47:09.084458 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4385 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1142 2023-06-25 12:47:08.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       76 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       85 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       22 2023-06-25 12:47:06.000000 vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      616 2022-10-28 14:14:00.000000 vollseg-napari-mtrack-1.3.5/tox.ini
```

### Comparing `vollseg-napari-mtrack-1.3.3/.github/workflows/test_and_deploy.yml` & `vollseg-napari-mtrack-1.3.5/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/.gitignore` & `vollseg-napari-mtrack-1.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/.napari-hub/config.yml` & `vollseg-napari-mtrack-1.3.5/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/.pre-commit-config.yaml` & `vollseg-napari-mtrack-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/LICENSE` & `vollseg-napari-mtrack-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/PKG-INFO` & `vollseg-napari-mtrack-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-mtrack
-Version: 1.3.3
+Version: 1.3.5
 Summary: Segment kymographs of microtubules, actin filaments and perform Ransac based fits to compute dynamic instability parameters for individual kymographs and also in batch
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack#README.md
```

### Comparing `vollseg-napari-mtrack-1.3.3/README.md` & `vollseg-napari-mtrack-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/setup.cfg` & `vollseg-napari-mtrack-1.3.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/__init__.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/__init__.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_reader.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_reader.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_sample_data.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_sample_data.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_temporal_plots.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_tests/utils.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_tests/utils.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_widget.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,31 +419,27 @@
                         _x,
                         unet_model=model_unet,
                         n_tiles=plugin.n_tiles.value,
                         axes=axes_reorder,
                     )
                 )
 
-            unet_mask, skeleton, denoised_image = zip(*pre_res)
+            unet_mask, skeleton = zip(*pre_res)
 
             unet_mask = np.asarray(unet_mask)
 
             unet_mask = unet_mask > 0
             unet_mask = np.moveaxis(unet_mask, 0, t)
             unet_mask = np.reshape(unet_mask, x.shape)
 
             skeleton = np.asarray(skeleton)
             skeleton = skeleton > 0
             skeleton = np.moveaxis(skeleton, 0, t)
             skeleton = np.reshape(skeleton, x.shape)
 
-            denoised_image = np.asarray(denoised_image)
-            denoised_image = np.moveaxis(denoised_image, 0, t)
-            denoised_image = np.reshape(denoised_image, x.shape)
-
             layer_data = np.zeros_like(unet_mask)
             for i in range(unet_mask.shape[0]):
                 layer_data[i] = thin(unet_mask[i])
 
         else:
             for layer in list(plugin.viewer.value.layers):
                 if (
@@ -581,15 +577,15 @@
             res = VollSeg(
                 x,
                 unet_model=model_unet,
                 n_tiles=plugin.n_tiles.value,
                 axes=axes,
             )
 
-            unet_mask, skeleton, denoised_image = res
+            unet_mask, skeleton = res
 
             layer_data = thin(unet_mask)
 
         else:
             for layer in list(plugin.viewer.value.layers):
                 if (
                     isinstance(layer, napari.layers.Labels)
@@ -1529,26 +1525,26 @@
                                         None,
                                         None,
                                     ]
                                 )
 
                         if s == len(all_shape_layer_data) - 1:
                             cat_frequ = cat_frequ / total_time
-                            cat_frequ = (
-                                cat_frequ
-                                / plugin.microscope_calibration_time.value
+                            cat_frequ = cat_frequ / (
+                                plugin.microscope_calibration_time.value
+                                + 1.0e-10
                             )
 
                             total_depol_time = total_depol_time + abs(
                                 end_time - start_time
                             )
                             res_frequ = res_frequ / total_depol_time
-                            res_frequ = (
-                                res_frequ
-                                / plugin.microscope_calibration_time.value
+                            res_frequ = res_frequ / (
+                                plugin.microscope_calibration_time.value
+                                + 1.0e-10
                             )
                             cat_events.append(
                                 [
                                     index,
                                     None,
                                     None,
                                     None,
@@ -1576,15 +1572,14 @@
                                     cat_events,
                                     res_events,
                                 )
                             )
 
         # Polish the data here
         polish_data = _polish_data(data)
-        print(data.shape)
 
         df = pd.DataFrame(
             polish_data,
             columns=[
                 "File_Index",
                 "Growth_Rate",
                 "Shrink_Rate",
```

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/_writer.py` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/_writer.py`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/napari.yaml` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack/resources/kapoorlogo.png` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/PKG-INFO` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-mtrack
-Version: 1.3.3
+Version: 1.3.5
 Summary: Segment kymographs of microtubules, actin filaments and perform Ransac based fits to compute dynamic instability parameters for individual kymographs and also in batch
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-mtrack#README.md
```

### Comparing `vollseg-napari-mtrack-1.3.3/src/vollseg_napari_mtrack.egg-info/SOURCES.txt` & `vollseg-napari-mtrack-1.3.5/src/vollseg_napari_mtrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg-napari-mtrack-1.3.3/tox.ini` & `vollseg-napari-mtrack-1.3.5/tox.ini`

 * *Files identical despite different names*

