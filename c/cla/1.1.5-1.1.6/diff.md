# Comparing `tmp/cla-1.1.5.tar.gz` & `tmp/cla-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cla-1.1.5.tar", last modified: Wed Mar 22 06:28:02 2023, max compression
+gzip compressed data, was "cla-1.1.6.tar", last modified: Sun Jun 25 05:39:42 2023, max compression
```

## Comparing `cla-1.1.5.tar` & `cla-1.1.6.tar`

### file list

```diff
@@ -1,47 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.385465 cla-1.1.5/
--rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.1.5/LICENCE
--rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4563 2023-03-22 06:28:02.385465 cla-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.087175 cla-1.1.5/cla/
--rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.1.5/cla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.150242 cla-1.1.5/cla/gui/
--rw-rw-rw-   0        0        0      651 2023-03-15 01:21:18.000000 cla-1.1.5/cla/gui/1ef4b15e-ddd2-4c12-8dc7-bc3320c2ebb1.csv
--rw-rw-rw-   0        0        0      656 2023-03-15 01:33:38.000000 cla-1.1.5/cla/gui/4f6f3342-be14-4643-b3d6-01d74cae7d67.csv
--rw-rw-rw-   0        0        0      655 2023-03-15 01:33:50.000000 cla-1.1.5/cla/gui/8693335f-2967-4fbb-9115-1be62ee417ed.csv
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.5/cla/gui/__init__.py
--rw-rw-rw-   0        0        0      657 2023-03-15 01:35:54.000000 cla-1.1.5/cla/gui/c675011b-501a-4869-8644-93530784649e.csv
--rw-rw-rw-   0        0        0      657 2023-03-15 01:24:32.000000 cla-1.1.5/cla/gui/cad00a83-0e66-4c6a-8760-4aa76caea54b.csv
--rw-rw-rw-   0        0        0     3497 2023-03-16 03:12:35.000000 cla-1.1.5/cla/gui/run.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.291310 cla-1.1.5/cla/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.5/cla/gui/static/__init__.py
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.1.5/cla/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.1.5/cla/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.1.5/cla/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.1.5/cla/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.1.5/cla/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.1.5/cla/gui/static/sample.csv
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.322520 cla-1.1.5/cla/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.1.5/cla/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.1.5/cla/gui/templates/home.html
--rw-rw-rw-   0        0        0    71952 2023-03-21 10:38:31.000000 cla-1.1.5/cla/metrics.py
--rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.1.5/cla/unify.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.385465 cla-1.1.5/cla/vis/
--rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.1.5/cla/vis/__init__.py
--rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.1.5/cla/vis/feature_importance.py
--rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.1.5/cla/vis/plotComponents1D.py
--rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.1.5/cla/vis/plotComponents2D.py
--rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.1.5/cla/vis/plotComponents3D.py
--rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.1.5/cla/vis/plt2base64.py
--rw-rw-rw-   0        0        0     4959 2023-03-15 01:20:08.000000 cla-1.1.5/cla/vis/unsupervised_dimension_reductions.py
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.102829 cla-1.1.5/cla.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-03-22 06:28:01.000000 cla-1.1.5/cla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-03-22 06:28:02.000000 cla-1.1.5/cla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 06:28:01.000000 cla-1.1.5/cla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-03-22 06:28:01.000000 cla-1.1.5/cla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-03-22 06:28:01.000000 cla-1.1.5/cla.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 06:28:02.385465 cla-1.1.5/data/
--rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.1.5/data/sample.csv
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-22 06:28:02.385465 cla-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-03-21 10:38:47.000000 cla-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.659752 cla-1.1.6/
+-rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.1.6/LICENCE
+-rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4563 2023-06-25 05:39:42.659752 cla-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.399722 cla-1.1.6/cla/
+-rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.1.6/cla/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.607727 cla-1.1.6/cla/gui/
+-rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-1.1.6/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.6/cla/gui/__init__.py
+-rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-1.1.6/cla/gui/run.py
+-rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-1.1.6/cla/gui/sample.csv
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.635755 cla-1.1.6/cla/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.1.6/cla/gui/static/__init__.py
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.1.6/cla/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.1.6/cla/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.1.6/cla/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.1.6/cla/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.1.6/cla/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.1.6/cla/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.639748 cla-1.1.6/cla/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.1.6/cla/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.1.6/cla/gui/templates/home.html
+-rw-rw-rw-   0        0        0    72189 2023-06-25 05:38:43.000000 cla-1.1.6/cla/metrics.py
+-rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.1.6/cla/unify.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.655760 cla-1.1.6/cla/vis/
+-rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.1.6/cla/vis/__init__.py
+-rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.1.6/cla/vis/feature_importance.py
+-rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.1.6/cla/vis/plotComponents1D.py
+-rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.1.6/cla/vis/plotComponents2D.py
+-rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.1.6/cla/vis/plotComponents3D.py
+-rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.1.6/cla/vis/plt2base64.py
+-rw-rw-rw-   0        0        0     4959 2023-03-15 01:20:08.000000 cla-1.1.6/cla/vis/unsupervised_dimension_reductions.py
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.588156 cla-1.1.6/cla.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      821 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-25 05:39:42.000000 cla-1.1.6/cla.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 05:39:42.655760 cla-1.1.6/data/
+-rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.1.6/data/sample.csv
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-25 05:39:42.663747 cla-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-06-25 04:59:20.000000 cla-1.1.6/setup.py
```

### Comparing `cla-1.1.5/PKG-INFO` & `cla-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.1.5
+Version: 1.1.6
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.1.5 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.1.6 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.1.5/README.md` & `cla-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/1ef4b15e-ddd2-4c12-8dc7-bc3320c2ebb1.csv` & `cla-1.1.6/cla/gui/sample.csv`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,81 @@
-# X1,X2,...,Y
--1.953,-1.657,0
--1.715,0.159,0
-0.015,0.286,0
--2.258,0.488,0
--1.372,-1.235,0
--0.999,-0.405,0
--0.493,-1.251,0
-0.297,1.164,0
--0.120,0.719,0
--0.917,0.393,0
-0.536,-0.268,0
--0.399,1.519,0
--0.348,-1.122,0
-0.139,-1.932,0
--3.241,0.415,0
--1.691,0.864,0
--0.401,-0.770,0
--1.817,0.484,0
--1.295,-0.863,0
--1.016,-0.639,0
-0.966,2.039,1
-2.696,0.317,1
-1.643,0.552,1
-0.796,1.727,1
-3.097,-1.363,1
-1.214,1.847,1
--0.008,-0.612,1
-0.724,-0.599,1
-1.913,0.569,1
--0.150,0.607,1
-1.310,1.201,1
-1.934,-0.033,1
-2.062,0.590,1
--1.071,-0.418,1
-1.443,0.186,1
-0.972,0.656,1
--0.422,1.000,1
-1.923,-0.369,1
-0.412,0.846,1
-2.110,1.664,1
+# X1,X2,Y
+-0.735,-0.79,0
+-1.963,-1.243,0
+-1.562,-0.075,0
+-0.382,-0.585,0
+-1.472,0.193,0
+-2.202,-1.223,0
+-0.682,0.894,0
+-1.78,-0.247,0
+-1.093,0.603,0
+0.18,-0.858,0
+-0.845,-1.225,0
+-1.668,-0.24,0
+-1.273,-1.538,0
+0.194,2.662,0
+-0.758,0.32,0
+-1.828,-1.346,0
+-2.337,1.093,0
+-1.023,-0.713,0
+-1.089,-0.006,0
+0.18,0.246,0
+-2.276,-0.769,0
+0.611,0.767,0
+-1.185,-0.641,0
+0.439,1.042,0
+-0.796,0.417,0
+-2.171,0.475,0
+0.884,0.246,0
+-1.287,0.84,0
+0.404,-0.144,0
+1.319,0.313,0
+-1.864,0.833,0
+-0.544,1.942,0
+-0.528,-0.343,0
+-2.213,-1.168,0
+0.274,-0.445,0
+-1.363,-0.917,0
+-2.972,-1.057,0
+-1.251,0.309,0
+-1,-1.041,0
+-1.18,1.629,0
+1.134,0.006,1
+1.77,1.139,1
+0.097,1.104,1
+0.222,-1.089,1
+1.344,-0.279,1
+2.71,-2.368,1
+1.081,1.026,1
+0.622,0.462,1
+0.617,-0.319,1
+0.488,-0.256,1
+1.733,-1.708,1
+1.051,-0.118,1
+1.865,-0.418,1
+-1.585,0.579,1
+1.324,-0.301,1
+1.3,0.427,1
+-0.914,-2.845,1
+0.616,1.664,1
+1.129,0.255,1
+0.792,0.413,1
+-0.021,-2.532,1
+2.133,-1.244,1
+-0.208,-0.95,1
+0.6,-2.238,1
+0.905,-0.113,1
+-0.173,2.099,1
+1.365,-2.494,1
+2.429,-1.071,1
+1.127,-0.272,1
+-0.481,-1.185,1
+0.829,-1.084,1
+1.019,0.537,1
+0.697,0.843,1
+1.773,-0.417,1
+0.603,-0.627,1
+1.528,-0.092,1
+0.756,0.693,1
+2.592,0.876,1
+0.277,1.361,1
+1.235,1.248,1
```

### Comparing `cla-1.1.5/cla/gui/run.py` & `cla-1.1.6/cla/gui/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 else:
     ROOT_DIR = os.path.dirname (os.path.dirname(__file__))
     if ROOT_DIR not in sys.path:
         sys.path.append(ROOT_DIR)
     import metrics
 
 app = Flask(__name__)
-app.config['MAX_CONTENT_LENGTH'] = 5 * 1024 * 1024  # limit to 5MB
+app.config['MAX_CONTENT_LENGTH'] = 50 * 1024 * 1024  # limit to 50MB to avoid 413 error
 
 def generate(d, n):
 
     d = int(d)
     n = int(n)
 
     X, y = metrics.mvg(nobs=n, md=d)
@@ -76,26 +76,29 @@
 @app.route("/submit", methods=['GET', 'POST'])
 def run_cla():
     if request.method == 'POST':
 
         r = ''
         use_sample = request.form["use_sample"]
 
-        if (use_sample):
+        if (use_sample == 'true' or use_sample is True):
             # distance between means, respect to std, i.e. (mu2 - mu1) / std, or how many stds is the difference.
             d = request.form["d"]
             n = request.form["nobs"]  # number of observations / samples
             csv = generate(d, n)
         else:
             f = request.files['dataFile']
             csv = os.path.dirname(os.path.realpath(
                 __file__)) + "/" + str(uuid.uuid4()) + ".csv"
             f.save(csv)
 
-        r = analyze(csv)
+        try:
+            r = analyze(csv)
+        except Exception as e:
+            r = str(e)
 
     # render_template("home.html", use_sample = use_sample, d = d, nobs = n, cla_result = r)
     return {'message': 'success', 'html': r}
 
 
 if __name__ == '__main__':
     # # use netstat -ano|findstr 5005 to check port use
```

### Comparing `cla-1.1.5/cla/gui/static/bootstrap.css` & `cla-1.1.6/cla/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/static/bootstrap.js` & `cla-1.1.6/cla/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/static/jquery-3.3.1.min.js` & `cla-1.1.6/cla/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/static/jquery.blockUI.js` & `cla-1.1.6/cla/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/static/jquery.form.min.js` & `cla-1.1.6/cla/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/static/sample.csv` & `cla-1.1.6/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/gui/templates/home.html` & `cla-1.1.6/cla/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/metrics.py` & `cla-1.1.6/cla/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -484,15 +484,18 @@
     X0, X1 = X[:, 0], X[:, 1]
     xx, yy = make_meshgrid(X0, X1)
 
     cmap = matplotlib.colors.ListedColormap(
         ['0.8', '0.1', 'red', 'blue', 'black', 'orange', 'green', 'cyan', 'purple', 'gray'])
 
     plt.figure()
-    plot_contours(plt, clf, xx, yy, cmap=plt.cm.coolwarm, alpha=0.1)
+
+    if X.shape[1] == 2:
+        plot_contours(plt, clf, xx, yy, cmap=plt.cm.coolwarm, alpha=0.1)
+    
     plt.scatter(X0, X1, c=y, s=70, facecolors=cmap,
                 edgecolors='gray', alpha=.4)  # cmap='gray'
     plt.xlim(xx.min(), xx.max())
     plt.ylim(yy.min(), yy.max())
     plt.xlabel('X1')
     plt.ylabel('X2')
     plt.xticks(())
@@ -518,31 +521,29 @@
     if Xn is not None:
         Xn0, Xn1 = Xn[:, 0], Xn[:, 1]
         plt.scatter(Xn0, Xn1, c='r', s=120, facecolors=cmap,
                     edgecolors='k', alpha=1, label='Sample')  # cmap='gray'
 
     plt.legend()
     plt.show()
-    print("SVC({})".format(clf.get_params()))
-
 
 def classify_with_svm(X, y):
     """Train SVM classifiers
 
     Parameters
     ----------
     X: feature matrix of with 2 columns 
     y: label    
     """
 
     # we create an instance of SVM and fit out data. We do not scale our
     # data since we want to plot the support vectors
     C = 1.0  # SVM regularization parameter
-    models = (SVC(kernel='linear', C=C),
-              LinearSVC(C=C),
+    models = (SVC(kernel='linear', C=C), #  # SVC defaulty uses the one-vs-one scheme to support multiclass.
+              LinearSVC(C=C, multi_class='crammer_singer'), # crammer_singer optimizes a joint objective over all classes
               SVC(kernel='rbf', gamma=0.7, C=C),
               SVC(kernel='poly', degree=3, C=C))
     models = (clf.fit(X, y) for clf in models)
 
     # title for the plots
     titles = ('SVC - linear kernel',
               'LinearSVC',
@@ -553,15 +554,17 @@
     fig, sub = plt.subplots(2, 2, figsize=(15, 15))
     plt.subplots_adjust(wspace=0.4, hspace=0.4)
 
     X0, X1 = X[:, 0], X[:, 1]
     xx, yy = make_meshgrid(X0, X1)
 
     for clf, title, ax in zip(models, titles, sub.flatten()):
-        plot_contours(ax, clf, xx, yy, cmap=plt.cm.coolwarm, alpha=0.1)
+
+        if X.shape[1] == 2:
+            plot_contours(ax, clf, xx, yy, cmap=plt.cm.coolwarm, alpha=0.1)
         ax.scatter(X0, X1, c=y, cmap=plt.cm.coolwarm, s=20, edgecolors='k')
         ax.set_xlim(xx.min(), xx.max())
         ax.set_ylim(yy.min(), yy.max())
         ax.set_xlabel('X1')
         ax.set_ylabel('X2')
         ax.set_xticks(())
         ax.set_yticks(())
@@ -608,16 +611,16 @@
 
     # min(grp_samples) is the minimum sample size among all categories.
     # CV requires to be not greater than this value.
 
     try:
         clf = LogisticRegressionCV(cv=min(3, min(grp_samples)), max_iter=1000).fit(
             X, y)  # ridge(L2) regularization
-    except:
-        print('Exception in LogisticRegressionCV().')
+    except Exception as e:
+        print('Exception in LogisticRegressionCV().', e)
         return None, None, None
 
     LOG += "regularization strength\t" + str(clf.C_) + "\n\n"
     # l1_ratio: while 1 is equivalent to using penalty='l1'. For 0 < l1_ratio <1, the penalty is a combination of L1 and L2.
 
     IMG = ''
 
@@ -813,16 +816,16 @@
 
     The term “discrete features” is used instead of naming them “categorical”, because it describes the essence more accurately. For example, pixel intensities of an image are discrete features (but hardly categorical) and you will get better results if mark them as such. Also note, that treating a continuous variable as discrete and vice versa will usually give incorrect results, so be attentive about that.
     True mutual information can’t be negative. If its estimate turns out to be negative, it is replaced by zero.
     """
 
     try:
         mi = mutual_info_classif(X, y, discrete_features=False)
-    except:
-        print('Exception in mutual_info_classif().')
+    except Exception as e:
+        print('Exception in mutual_info_classif().', e)
         return None, None
 
     mi_sorted = np.sort(mi)[::-1]  # sort in desceding order
     mi_sorted_idx = np.argsort(mi)[::-1]
 
     if (X.shape[1] > 50):
         plt.figure(figsize=(20, 3))
@@ -1682,16 +1685,16 @@
     dic, _, _ = CLF(X, y)
     if dic is None:
         dic = {}
 
     ber = 1  # set maximum BER
     try:
         ber, _ = BER(X, y)
-    except:
-        print('Exception in GaussianNB.')
+    except Exception as e:
+        print('Exception in GaussianNB.', e)
     dic['classification.BER'] = ber
 
     svm_width, _ = SVM_Margin_Width(X, y)
     dic['classification.SVM.Margin'] = svm_width
 
     ig, _ = IG(X, y)
     if ig is not None:
```

### Comparing `cla-1.1.5/cla/unify.py` & `cla-1.1.6/cla/unify.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/vis/feature_importance.py` & `cla-1.1.6/cla/vis/feature_importance.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/vis/plotComponents1D.py` & `cla-1.1.6/cla/vis/plotComponents1D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/vis/plotComponents2D.py` & `cla-1.1.6/cla/vis/plotComponents2D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/vis/plotComponents3D.py` & `cla-1.1.6/cla/vis/plotComponents3D.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla/vis/unsupervised_dimension_reductions.py` & `cla-1.1.6/cla/vis/unsupervised_dimension_reductions.py`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/cla.egg-info/PKG-INFO` & `cla-1.1.6/cla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.1.5
+Version: 1.1.6
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.1.5 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.1.6 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.1.5/cla.egg-info/SOURCES.txt` & `cla-1.1.6/cla.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,21 +7,18 @@
 cla/metrics.py
 cla/unify.py
 cla.egg-info/PKG-INFO
 cla.egg-info/SOURCES.txt
 cla.egg-info/dependency_links.txt
 cla.egg-info/requires.txt
 cla.egg-info/top_level.txt
-cla/gui/1ef4b15e-ddd2-4c12-8dc7-bc3320c2ebb1.csv
-cla/gui/4f6f3342-be14-4643-b3d6-01d74cae7d67.csv
-cla/gui/8693335f-2967-4fbb-9115-1be62ee417ed.csv
+cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
 cla/gui/__init__.py
-cla/gui/c675011b-501a-4869-8644-93530784649e.csv
-cla/gui/cad00a83-0e66-4c6a-8760-4aa76caea54b.csv
 cla/gui/run.py
+cla/gui/sample.csv
 cla/gui/static/__init__.py
 cla/gui/static/bootstrap.css
 cla/gui/static/bootstrap.js
 cla/gui/static/jquery-3.3.1.min.js
 cla/gui/static/jquery.blockUI.js
 cla/gui/static/jquery.form.min.js
 cla/gui/static/sample.csv
```

### Comparing `cla-1.1.5/data/sample.csv` & `cla-1.1.6/cla/gui/static/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.1.5/setup.py` & `cla-1.1.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 setup(
     # Application name:
     name="cla",
     
     # Version number (initial):
-    version="1.1.5",
+    version="1.1.6",
     
     # Application author details:
     author="Zhang",
     author_email="oo@zju.edu.cn",
     
     # Packages
     packages=["cla", "cla.vis", "cla.gui", "cla.gui.templates", "cla.gui.static"],
```

