# Comparing `tmp/neuroneq-0.0.5.tar.gz` & `tmp/neuroneq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\neuroneq-0.0.5.tar", last modified: Sun Aug  1 19:24:57 2021, max compression
+gzip compressed data, was "neuroneq-0.0.6.tar", last modified: Sun Jun 25 18:35:04 2023, max compression
```

## Comparing `neuroneq-0.0.5.tar` & `neuroneq-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:57.980285 neuroneq-0.0.5/
--rw-rw-rw-   0        0        0     1089 2021-08-01 13:59:30.000000 neuroneq-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      843 2021-08-01 19:24:57.978654 neuroneq-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       87 2021-08-01 13:59:30.000000 neuroneq-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:57.877473 neuroneq-0.0.5/neuroneq/
--rw-rw-rw-   0        0        0        0 2021-08-01 13:59:30.000000 neuroneq-0.0.5/neuroneq/__init__.py
--rw-rw-rw-   0        0        0     1759 2021-08-01 13:59:30.000000 neuroneq-0.0.5/neuroneq/cli.py
--rw-rw-rw-   0        0        0    31061 2021-08-01 19:19:51.000000 neuroneq-0.0.5/neuroneq/main.py
-drwxrwxrwx   0        0        0        0 2021-08-01 19:24:57.973453 neuroneq-0.0.5/neuroneq.egg-info/
--rw-rw-rw-   0        0        0      843 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2021-08-01 19:24:57.000000 neuroneq-0.0.5/neuroneq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-08-01 19:24:57.981444 neuroneq-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1252 2021-08-01 19:24:13.000000 neuroneq-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:35:04.830836 neuroneq-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-06-25 17:55:23.000000 neuroneq-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1486 2023-06-25 18:35:04.828835 neuroneq-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      735 2023-06-25 18:33:55.000000 neuroneq-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 18:35:04.802835 neuroneq-0.0.6/neuroneq/
+-rw-rw-rw-   0        0        0       38 2023-06-25 18:20:13.000000 neuroneq-0.0.6/neuroneq/__init__.py
+-rw-rw-rw-   0        0        0     1759 2023-06-25 17:55:23.000000 neuroneq-0.0.6/neuroneq/cli.py
+-rw-rw-rw-   0        0        0    31170 2023-06-25 17:55:23.000000 neuroneq-0.0.6/neuroneq/main.py
+-rw-rw-rw-   0        0        0     1576 2023-06-25 18:32:11.000000 neuroneq-0.0.6/neuroneq/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:35:04.826836 neuroneq-0.0.6/neuroneq.egg-info/
+-rw-rw-rw-   0        0        0     1486 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 18:35:03.000000 neuroneq-0.0.6/neuroneq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 18:35:04.830836 neuroneq-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1252 2023-06-25 18:34:28.000000 neuroneq-0.0.6/setup.py
```

### Comparing `neuroneq-0.0.5/LICENSE` & `neuroneq-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroneq-0.0.5/neuroneq/cli.py` & `neuroneq-0.0.6/neuroneq/cli.py`

 * *Files identical despite different names*

### Comparing `neuroneq-0.0.5/neuroneq/main.py` & `neuroneq-0.0.6/neuroneq/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,28 +263,30 @@
 
         try:
             self.distanceplot.quiver(src_pos[0],src_pos[1],src_pos[2],(trg_pos[0]-src_pos[0]),(trg_pos[1]-src_pos[1]),(trg_pos[2]-src_pos[2]),
             pivot='tail',length=true_dist,label="euclid: {:.4f}".format(true_dist),color='blue',normalize=True)
         except Exception as e:
             print(e)
 
+        src_vec_dist = np.linalg.norm(vec_pos-src_pos)
         try:
             self.distanceplot.quiver(src_pos[0],src_pos[1],src_pos[2],(vec_pos[0]-src_pos[0]),(vec_pos[1]-src_pos[1]),(vec_pos[2]-src_pos[2]),
-            pivot='tail',length=np.linalg.norm(vec_pos-src_pos)/10,color='green',normalize=True)
+            pivot='tail',length=src_vec_dist*1000,color='green',normalize=True)
         except Exception as e:
             print(e)
 
+        #vec_trg_dist = np.linalg.norm(trg_pos-vec_pos)
         #try:
         #    self.distanceplot.quiver(vec_pos[0],vec_pos[1],vec_pos[2],(trg_pos[0]-vec_pos[0]),(trg_pos[1]-vec_pos[1]),(trg_pos[2]-vec_pos[2]),
-        #    pivot='tail',length=np.linalg.norm(trg_pos-vec_pos),label="{:.4f}".format(dist),color='green',normalize=True)
+        #    pivot='tail',length=vec_trg_dist,label="{:.4f}".format(vec_trg_dist),color='green',normalize=True)
         #except Exception as e:
         #    print(e)
 
         try:
-            self.distanceplot.quiver(src_pos[0],src_pos[1],src_pos[2],(trg_pos[0]-src_pos[0]),(trg_pos[1]-src_pos[1]),(trg_pos[2]-src_pos[2]),
+            self.distanceplot.quiver(vec_pos[0],vec_pos[1],vec_pos[2],(trg_pos[0]-vec_pos[0]),(trg_pos[1]-vec_pos[1]),(trg_pos[2]-vec_pos[2]),
             pivot='tail',length=dist,label="{:.4f}".format(dist),color='orange',normalize=True)
         except Exception as e:
             print(e)
 
         self.distanceplot.legend()
         self.distancecanvas.draw()
         #v = self.v
@@ -349,28 +351,28 @@
 
         equation = "np.linalg.norm(np.cross((trg_pos - src_pos), (trg_pos - vec_pos))) / np.linalg.norm((vec_pos - src_pos))"
         self.equation_row = Row(general_frame).config("Distance Equation", equation , "Use src_pos,trg_pos,vec_pos", True,entry_width=100)
         self.equation_row.pack(padx=10)
 
         def euclid():
             self.equation_row.set_value("np.linalg.norm(trg_pos - src_pos)")
-            self.plot_distance_page()
+            self.plot_distance_page(disable_vec_trg=True)
         
         def angle():
             self.equation_row.set_value(equation)
             self.plot_distance_page()
 
 
         plotButton = tk.Button(general_frame, text="Plot", command=self.plot_distance_page)
-        euclidButton = tk.Button(general_frame, text="Euclidian Distance", command=euclid)
-        angleButton = tk.Button(general_frame, text="Angle Based Distance", command=angle)
+        #euclidButton = tk.Button(general_frame, text="Euclidian Distance", command=euclid)
+        #angleButton = tk.Button(general_frame, text="Angle Based Distance", command=angle)
         #plotButton.grid(column=0, row =99, padx=5, pady=5, sticky='W')
         plotButton.pack()
-        euclidButton.pack(side=tk.RIGHT)
-        angleButton.pack(side=tk.RIGHT)
+        #euclidButton.pack(side=tk.RIGHT)
+        #angleButton.pack(side=tk.RIGHT)
         plotButton.config(state=tk.ACTIVE)
 
 
     def parameters_page(self,root):
         '''
         Reads the parameters hoc file
         Lines should be formatted like:
```

### Comparing `neuroneq-0.0.5/setup.py` & `neuroneq-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="neuroneq",
-    version="0.0.5",
+    version="0.0.6",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="NeuronEQ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/neuroneq",
     download_url='',
```

