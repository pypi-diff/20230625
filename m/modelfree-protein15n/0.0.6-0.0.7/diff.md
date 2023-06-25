# Comparing `tmp/modelfree-protein15n-0.0.6.tar.gz` & `tmp/modelfree-protein15n-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelfree-protein15n-0.0.6.tar", last modified: Sun May 28 16:06:51 2023, max compression
+gzip compressed data, was "modelfree-protein15n-0.0.7.tar", last modified: Sun Jun 25 14:26:54 2023, max compression
```

## Comparing `modelfree-protein15n-0.0.6.tar` & `modelfree-protein15n-0.0.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/LICENSE
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/MANIFEST.in
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/PKG-INFO
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2698 2023-05-17 21:05:22.000000 modelfree-protein15n-0.0.6/README.md
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.639547 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/PKG-INFO
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      546 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/SOURCES.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/dependency_links.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/entry_points.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/requires.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/top_level.txt
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.661398 modelfree-protein15n-0.0.6/modfree/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/__init__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/__main__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1372 2023-05-28 15:54:27.000000 modelfree-protein15n-0.0.6/modfree/analysis.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      699 2023-05-28 15:39:24.000000 modelfree-protein15n-0.0.6/modfree/constants_functions.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/data_format.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6438 2023-05-28 15:44:13.000000 modelfree-protein15n-0.0.6/modfree/generator.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1901 2023-05-28 15:34:09.000000 modelfree-protein15n-0.0.6/modfree/inputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14226 2023-05-28 15:39:13.000000 modelfree-protein15n-0.0.6/modfree/mf.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5613 2023-05-28 15:53:09.000000 modelfree-protein15n-0.0.6/modfree/modfree.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3538 2023-05-28 15:30:20.000000 modelfree-protein15n-0.0.6/modfree/outputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     4472 2023-05-28 15:30:09.000000 modelfree-protein15n-0.0.6/modfree/ploter.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2961 2023-05-28 15:43:26.000000 modelfree-protein15n-0.0.6/modfree/run_fit.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/setup.cfg
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/setup.py
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-06-25 14:26:54.302009 modelfree-protein15n-0.0.7/
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/LICENSE
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/MANIFEST.in
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-06-25 14:26:54.302009 modelfree-protein15n-0.0.7/PKG-INFO
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2698 2023-05-17 21:05:22.000000 modelfree-protein15n-0.0.7/README.md
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-06-25 14:26:54.223934 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/PKG-INFO
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      546 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/SOURCES.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/dependency_links.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/entry_points.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/requires.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-06-25 14:26:53.000000 modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/top_level.txt
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-06-25 14:26:54.297923 modelfree-protein15n-0.0.7/modfree/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/modfree/__init__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/modfree/__main__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1372 2023-05-28 15:54:27.000000 modelfree-protein15n-0.0.7/modfree/analysis.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      699 2023-05-28 15:39:24.000000 modelfree-protein15n-0.0.7/modfree/constants_functions.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/modfree/data_format.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6438 2023-05-28 15:44:13.000000 modelfree-protein15n-0.0.7/modfree/generator.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1901 2023-05-28 15:34:09.000000 modelfree-protein15n-0.0.7/modfree/inputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14226 2023-05-28 15:39:13.000000 modelfree-protein15n-0.0.7/modfree/mf.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5531 2023-06-25 14:26:31.000000 modelfree-protein15n-0.0.7/modfree/modfree.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3538 2023-05-28 15:30:20.000000 modelfree-protein15n-0.0.7/modfree/outputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     4548 2023-06-25 14:23:10.000000 modelfree-protein15n-0.0.7/modfree/ploter.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2961 2023-05-28 15:43:26.000000 modelfree-protein15n-0.0.7/modfree/run_fit.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-06-25 14:26:54.302009 modelfree-protein15n-0.0.7/setup.cfg
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.7/setup.py
```

### Comparing `modelfree-protein15n-0.0.6/LICENSE` & `modelfree-protein15n-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/PKG-INFO` & `modelfree-protein15n-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.6
+Version: 0.0.7
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
```

### Comparing `modelfree-protein15n-0.0.6/README.md` & `modelfree-protein15n-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/PKG-INFO` & `modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.6
+Version: 0.0.7
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
```

### Comparing `modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/SOURCES.txt` & `modelfree-protein15n-0.0.7/modelfree_protein15n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/analysis.py` & `modelfree-protein15n-0.0.7/modfree/analysis.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/constants_functions.py` & `modelfree-protein15n-0.0.7/modfree/constants_functions.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/data_format.py` & `modelfree-protein15n-0.0.7/modfree/data_format.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/generator.py` & `modelfree-protein15n-0.0.7/modfree/generator.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/inputs.py` & `modelfree-protein15n-0.0.7/modfree/inputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/mf.py` & `modelfree-protein15n-0.0.7/modfree/mf.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/modfree.py` & `modelfree-protein15n-0.0.7/modfree/modfree.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import modfree.inputs as inputs
 import modfree.outputs as outputs
 import modfree.run_fit as run_fit
 import modfree.ploter as ploter
 import modfree.generator as generator
 
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 
 console = Console()
 
 
 header = "\n".join(
 [
@@ -43,29 +43,29 @@
 
 def plot(args: Namespace):
     data_file = args.o
     what_to_plot = args.p
     if what_to_plot == "relaxation" or what_to_plot == "all":
         ploter.plot_rates(output_dir=data_file, file_format=args.format, dpi=args.dpi)
     if what_to_plot == "parameters" or what_to_plot == "all":
-        ploter.plot_params(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_params(output_dir=data_file, file_format=args.format, dpi=args.dpi)
     if what_to_plot == "statistics" or what_to_plot == "all":
         ploter.plot_statistics(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
     if what_to_plot == "correlation" or what_to_plot == "all":
         ploter.plot_rates_corr(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
 
 
 def fit(args: Namespace):
     data_files = inputs.read_directory_file(args.d)
     input_parameters = inputs.read_parameter_file(args.p)
     result = run_fit.launch_fits(input_parameters, args.r, data_files)
     outputs.save_params(result, directory=args.o)
     df.Save(result, args.o+"/rawoutput.txt")
     if args.plot:
-        ploter.plot_params(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_params(output_dir=data_file, file_format=args.format, dpi=args.dpi)
         ploter.plot_statistics(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
         ploter.plot_rates_corr(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
         ploter.plot_rates(output_dir=data_file, file_format=args.format, dpi=args.dpi)
 
 
 def generate(args: Namespace):
     generator.generate(args.n, args.o, fields=args.fields, rates=args.rates, modes=args.modes, noise_proportion=args.noise)
```

### Comparing `modelfree-protein15n-0.0.6/modfree/outputs.py` & `modelfree-protein15n-0.0.7/modfree/outputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/modfree/ploter.py` & `modelfree-protein15n-0.0.7/modfree/ploter.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 sns.set_context("poster")
 sns.set_palette('dark')
 colors = ['blue', 'orange', 'red', 'darkred', 'black', 'darkblue', 'darkorange', 'maroon', 'purple', 'pink']
 
 
 def check_output_dir(output_dir):
     if not os.path.isdir(output_dir+"/Plots"):
+        os.mkdir(output_dir)
+    if not os.path.isdir(output_dir+"/Plots"):
         os.mkdir(output_dir+"/Plots")
 
 
 def plot_param(filename, color="darkblue", ax=None, log=False):
     with open(filename, "r") as f:
         dat = [el.rstrip("\n").split() for el in f.readlines()]
     x = [int(el[0]) for el in dat]
```

### Comparing `modelfree-protein15n-0.0.6/modfree/run_fit.py` & `modelfree-protein15n-0.0.7/modfree/run_fit.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.6/setup.py` & `modelfree-protein15n-0.0.7/setup.py`

 * *Files identical despite different names*

