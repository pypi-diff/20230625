# Comparing `tmp/property-lister-2.1.tar.gz` & `tmp/property-lister-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "property-lister-2.1.tar", last modified: Fri May  5 18:54:26 2023, max compression
+gzip compressed data, was "property-lister-2.2.tar", last modified: Sun Jun 25 18:05:13 2023, max compression
```

## Comparing `property-lister-2.1.tar` & `property-lister-2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:54:26.833056 property-lister-2.1/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-05-05 18:51:11.000000 property-lister-2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2999 2023-05-05 18:54:26.833056 property-lister-2.1/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     2600 2023-05-05 18:53:22.000000 property-lister-2.1/README.md
--rwxrwx---   0 root         (0) root         (0)      760 2023-05-05 18:51:37.000000 property-lister-2.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 18:54:26.833056 property-lister-2.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:54:26.833056 property-lister-2.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:54:26.833056 property-lister-2.1/src/property_lister/
--rwxrwx---   0 root         (0) root         (0)        0 2023-05-05 18:51:11.000000 property-lister-2.1/src/property_lister/__init__.py
--rwxrwx---   0 root         (0) root         (0)     9486 2023-05-05 18:51:30.000000 property-lister-2.1/src/property_lister/property_lister.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 18:54:26.833056 property-lister-2.1/src/property_lister.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2999 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-05 18:54:26.000000 property-lister-2.1/src/property_lister.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:05:13.674762 property-lister-2.2/
+-rw-r--r--   0 root         (0) root         (0)     1090 2023-06-25 14:51:57.000000 property-lister-2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-06-25 18:05:13.674762 property-lister-2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-25 16:43:02.000000 property-lister-2.2/README.md
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-25 16:43:19.000000 property-lister-2.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 18:05:13.674762 property-lister-2.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:05:13.674762 property-lister-2.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:05:13.674762 property-lister-2.2/src/property_lister/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-25 14:51:57.000000 property-lister-2.2/src/property_lister/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9478 2023-06-25 15:06:18.000000 property-lister-2.2/src/property_lister/property_lister.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 18:05:13.674762 property-lister-2.2/src/property_lister.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2999 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-25 18:05:13.000000 property-lister-2.2/src/property_lister.egg-info/top_level.txt
```

### Comparing `property-lister-2.1/LICENSE` & `property-lister-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `property-lister-2.1/PKG-INFO` & `property-lister-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 2.1
+Version: 2.2
 Summary: Extract and convert property list files from SQLite database files and from other property list files
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
@@ -43,15 +43,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-2.1-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.2-py3-none-any.whl
 
 apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
@@ -75,15 +75,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v2.1 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.2 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-2.1/README.md` & `property-lister-2.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-2.1-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.2-py3-none-any.whl
 
 apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
@@ -62,15 +62,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v2.1 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.2 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

### Comparing `property-lister-2.1/pyproject.toml` & `property-lister-2.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "property-lister"
-version = "2.1"
+version = "2.2"
 authors = [{ name = "Ivan Sincek" }]
 description = "Extract and convert property list files from SQLite database files and from other property list files"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `property-lister-2.1/src/property_lister/property_lister.py` & `property-lister-2.2/src/property_lister/property_lister.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 start = datetime.datetime.now()
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Property Lister v2.1 ( github.com/ivan-sincek/property-lister )")
+	print("Property Lister v2.2 ( github.com/ivan-sincek/property-lister )")
 	print("")
 	print("--- Extract from an SQLite database file ---")
 	print("Usage:   property-lister -db database -o out")
 	print("Example: property-lister -db Cache.db -o results")
 	print("")
 	print("--- Extract from a property list file ---")
 	print("Usage:   property-lister -pl property-list -o out")
@@ -42,40 +42,40 @@
 	print("    Output directory")
 	print("    All extracted propery list files will be saved in this directory")
 	print("    -o <out> - results | etc.")
 
 # ------------------- MISCELENIOUS BEGIN -------------------
 
 def remove_directory(directory):
-	removed = True
+	success = True
 	try:
 		if os.path.exists(directory):
 			shutil.rmtree(directory)
 	except Exception:
-		removed = False
+		success = False
 		print_error(("Cannot remove '{0}' related directories/subdirectories and/or files").format(directory))
-	return removed
+	return success
 
 def create_directory(directory):
-	created = True
+	success = True
 	try:
 		if not os.path.exists(directory):
 			os.mkdir(directory)
 	except Exception:
-		created = False
-		print_error(("Cannot create '{0}' related directories/subdirectories and/or files").format(directory))
-	return created
+		success = False
+		print_error(("Cannot create '{0}' directory").format(directory))
+	return success
 
 def check_directory(directory):
 	success = False
 	overwrite = "yes"
 	if os.path.exists(directory):
 		print(("'{0}' directory already exists").format(directory))
-		overwrite = input("Overwrite the output directory (yes): ").lower()
-	if overwrite == "yes" and remove_directory(directory):
+		overwrite = input("Overwrite the output directory (yes): ")
+	if overwrite.lower() == "yes" and remove_directory(directory):
 		success = create_directory(directory)
 	return success
 
 def check_directory_files(directory):
 	tmp = []
 	for path, dirs, files in os.walk(directory):
 		for file in files:
@@ -200,26 +200,26 @@
 def dump(database, out):
 	for db in database:
 		count = 0
 		data = read_database(db)
 		if data:
 			db = build(out, db, ext["txt"])
 			open(db, "w").write(data)
-			blobs = re.findall(r"(?<=,X')[\w\d]+", data, re.IGNORECASE)
+			blobs = re.findall(r"(?<=,X')[\w\d]+", data, re.MULTILINE | re.IGNORECASE)
 			if blobs:
 				for blob in blobs:
 					count += 1
 					new = build(out, db, ext["blob"], True, count)
 					open(new, "wb").write(binascii.unhexlify(blob))
 					extract(new, out, True)
 
 # file --> full path (external/internal)
 def extract(file, out, internal):
 	data = run(["plistutil", "-f", "xml", "-i", ("'{0}'").format(file)])
-	if re.search(rb"\<plist[\s\S]+\<\/plist\>", data, re.IGNORECASE):
+	if re.search(rb"\<plist[\s\S]+\<\/plist\>", data, re.MULTILINE | re.IGNORECASE):
 		open(build(out, file, ext["xml"], True) if internal else build(out, build(out, file, ext["plist"]), ext["xml"], True), "wb").write(data)
 		try:
 			data = biplist.readPlist(file)
 			if isinstance(data, dict):
 				count = 0
 				for key in data:
 					if isinstance(data[key], biplist.Data):
@@ -254,15 +254,15 @@
 			error("Missing a mandatory option (-pl, -o)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed and check_directory(args["out"]):
 		print("##########################################################################")
 		print("#                                                                        #")
-		print("#                          Property Lister v2.1                          #")
+		print("#                          Property Lister v2.2                          #")
 		print("#                                     by Ivan Sincek                     #")
 		print("#                                                                        #")
 		print("# Extract and convert property list files.                               #")
 		print("# GitHub repository at github.com/ivan-sincek/property-lister.           #")
 		print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 		print("#                                                                        #")
 		print("##########################################################################")
```

### Comparing `property-lister-2.1/src/property_lister.egg-info/PKG-INFO` & `property-lister-2.2/src/property_lister.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: property-lister
-Version: 2.1
+Version: 2.2
 Summary: Extract and convert property list files from SQLite database files and from other property list files
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/property-lister
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.6
@@ -43,15 +43,15 @@
 ```bash
 git clone https://github.com/ivan-sincek/property-lister && cd property-lister
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/property_lister-2.1-py3-none-any.whl
+python3 -m pip install dist/property_lister-2.2-py3-none-any.whl
 
 apt-get -y install plistutil
 ```
 
 ## Extracting and Converting
 
 Extract and convert property list files inside Cache.db unencrypted SQLite database file:
@@ -75,15 +75,15 @@
 Repeat the same for the app specific directories.
 
 Check my other project on how to [search for files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#3-search-for-files-and-directories) and on how to [extract sensitive data from the files](https://github.com/ivan-sincek/ios-penetration-testing-cheat-sheet#4-inspect-files).
 
 ## Usage
 
 ```fundamental
-Property Lister v2.1 ( github.com/ivan-sincek/property-lister )
+Property Lister v2.2 ( github.com/ivan-sincek/property-lister )
 
 --- Extract from an SQLite database file ---
 Usage:   property-lister -db database -o out
 Example: property-lister -db Cache.db -o results
 
 --- Extract from a property list file ---
 Usage:   property-lister -pl property-list -o out
```

