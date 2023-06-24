# Comparing `tmp/mapdata-2.6.2.tar.gz` & `tmp/mapdata-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-2.6.2.tar", last modified: Fri Jun 23 20:38:37 2023, max compression
+gzip compressed data, was "mapdata-2.6.3.tar", last modified: Sat Jun 24 22:29:17 2023, max compression
```

## Comparing `mapdata-2.6.2.tar` & `mapdata-2.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.6.2/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.6.2/MANIFEST.in
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-23 20:38:37.462579 mapdata-2.6.2/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     2821 2023-06-23 20:29:24.000000 mapdata-2.6.2/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/mapdata/
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   328306 2023-06-23 20:04:35.000000 mapdata-2.6.2/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-23 20:38:37.462579 mapdata-2.6.2/mapdata.egg-info/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-23 20:38:37.000000 mapdata-2.6.2/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-23 20:38:37.462579 mapdata-2.6.2/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-23 20:19:05.000000 mapdata-2.6.2/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.748690 mapdata-2.6.3/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-2.6.3/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-2.6.3/MANIFEST.in
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-24 22:29:17.748690 mapdata-2.6.3/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     2821 2023-06-23 20:29:24.000000 mapdata-2.6.3/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.744690 mapdata-2.6.3/mapdata/
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   328878 2023-06-24 21:57:48.000000 mapdata-2.6.3/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2023-06-24 22:29:17.748690 mapdata-2.6.3/mapdata.egg-info/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     4019 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      185 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2023-06-24 22:29:17.000000 mapdata-2.6.3/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2023-06-24 22:29:17.748690 mapdata-2.6.3/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1313 2023-06-24 22:15:50.000000 mapdata-2.6.3/setup.py
```

### Comparing `mapdata-2.6.2/LICENSE.txt` & `mapdata-2.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-2.6.2/PKG-INFO` & `mapdata-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.6.2
+Version: 2.6.3
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.6.2/README.md` & `mapdata-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-2.6.2/mapdata/mapdata.py` & `mapdata-2.6.3/mapdata/mapdata.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "2.6.2"
-vdate = "2023-06-23"
+version = "2.6.3"
+vdate = "2023-06-24"
 
 copyright = "2023"
 
 
 import sys
 import os.path
 import io
@@ -531,54 +531,73 @@
 	# an alphabetic.
 	colnames = []
 	for hdr in tbl_hdrs:
 		colnames.append(dquote(hdr))
 	return colnames
 
 def isint(v):
+	# Missing values match and will be handled by 'conv_int()'
 	if v is None or (type(v) is str and v.strip() == ''):
-		return None
+		return True
 	if type(v) == int:
 		return True
 	if type(v) == float:
 		return False
 	try:
 		int(v)
 		return True
 	except ValueError:
 		return False
 	except TypeError:
 		return False
 
-def isfloat(v):
+def conv_int(v):
 	if v is None or (type(v) is str and v.strip() == ''):
 		return None
 	try:
+		rv = int(v)
+		return rv
+	except:
+		return None
+
+def isfloat(v):
+	# Missing values match and will be handled by 'conv_float()'
+	if v is None or (type(v) is str and v.strip() == ''):
+		return True
+	try:
 		float(v)
 		return True
 	except ValueError:
 		return False
 	except TypeError:
 		return False
 
+def conv_float(v):
+	if v is None or (type(v) is str and v.strip() == ''):
+		return None
+	try:
+		rv = float(v)
+		return rv
+	except:
+		return None
+
 def isboolean(v):
 	return parse_boolean(v) is not None
 
 
 def dt_type(v):
 	# Type of date/time: timestamp, date, or None
-	if v is None or (type(v) is str and v.strip() == ''):
-		return None
-	t = None
-	if parse_datetimetz(v):
-		return "timestamptz"
-	if parse_datetime(v):
-		return "timestamp"
+	if type(v) is str and v.strip() == '':
+		v = None
 	if parse_date(v):
 		return "date"
+	if parse_datetime(v):
+		return "timestamp"
+	if parse_datetimetz(v):
+		return "timestamptz"
 	return None
 
 def data_type(v):
 	# Characterizes the value v as one of a simple set of data types.
 	# Returns "timestamp", "date", "int", "float", or "string"
 	if v is None or (type(v) is str and v == ''):
 		return None
@@ -599,31 +618,38 @@
 	elif data_type_str == "date":
 		return datetime.date
 	elif data_type_str == "timestamp":
 		return parse_datetime
 	elif data_type_str == "timestamptz":
 		return parse_datetimetz
 	elif data_type_str == "int":
-		return int
+		return conv_int
 	elif data_type_str == "float":
-		return float
+		return conv_float
 	elif data_type_str == "boolean":
-		return bool
+		return parse_boolean
 
 def common_data_type(values):
 	# Returns a data type common to all the values in the list.
 	# This is "string" unlees all types are the same.
 	# Null (None) values are ignored.  If all values are null, return "string".
 	val2 = [v for v in values if v is not None and not (type(v) is str and v.strip() == '')]
 	if len(val2) == 0:
 		return "string"
 	else:
 		types = [data_type(v) for v in val2]
-		if len(set(types)) == 1:
+		typeset = set(types)
+		if len(typeset) == 1:
 			return types[0]
+		elif len(typeset) == 2:
+			uq_types = list(typeset)
+			if 'int' in uq_types and 'float' in uq_types:
+				return 'float'
+			else:
+				return "string"
 		else:
 			return "string"
 
 def set_data_types(headers, rows, data_type_list):
 	return_queue = queue.Queue()
 	def eval_columns(headers, rows, return_queue):
 		coltypes = []
```

### Comparing `mapdata-2.6.2/mapdata.egg-info/PKG-INFO` & `mapdata-2.6.3/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 2.6.2
+Version: 2.6.3
 Summary: An interactive map and table explorer for geographic coordinates in a CSV file
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: dreas.nielsen@gmail.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,PNG,JPG,Postscript
 Platform: UNKNOWN
```

### Comparing `mapdata-2.6.2/setup.py` & `mapdata-2.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 import io
 
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 setuptools.setup(name='mapdata',
-	version='2.6.2',
+	version='2.6.3',
 	description="An interactive map and table explorer for geographic coordinates in a CSV file",
 	author='Dreas Nielsen',
 	author_email='dreas.nielsen@gmail.com',
     url='https://osdn.net/project/mapdata/',
 	scripts=['mapdata/mapdata.py'],
     license='GPL',
 	requires=['tkintermapview', 'pyproj', 'odfpy', 'openpyxl', 'xlrd', 'matplotlib'],
```

