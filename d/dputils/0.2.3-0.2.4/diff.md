# Comparing `tmp/dputils-0.2.3.tar.gz` & `tmp/dputils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dputils-0.2.3.tar", max compression
+gzip compressed data, was "dputils-0.2.4.tar", max compression
```

## Comparing `dputils-0.2.3.tar` & `dputils-0.2.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6148 2022-06-13 14:27:14.044961 dputils-0.2.3/dputils/.DS_Store
--rw-r--r--   0        0        0       57 2023-01-23 12:30:33.427985 dputils-0.2.3/dputils/__init__.py
--rw-r--r--   0        0        0     4233 2023-01-11 08:01:06.463851 dputils-0.2.3/dputils/files.py
--rw-r--r--   0        0        0     7988 2023-01-23 12:38:16.785170 dputils-0.2.3/dputils/scrape.py
--rw-r--r--   0        0        0     1088 2022-06-11 05:17:23.834462 dputils-0.2.3/LICENSE
--rw-r--r--   0        0        0     1035 2023-01-23 12:40:39.067393 dputils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2302 2023-01-23 12:08:08.523476 dputils-0.2.3/readme.md
--rw-r--r--   0        0        0     3137 2023-01-23 12:40:47.575344 dputils-0.2.3/setup.py
--rw-r--r--   0        0        0     3227 2023-01-23 12:40:47.576344 dputils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     6148 2022-06-13 14:27:14.044961 dputils-0.2.4/dputils/.DS_Store
+-rw-r--r--   0        0        0       57 2023-01-23 12:30:33.427985 dputils-0.2.4/dputils/__init__.py
+-rw-r--r--   0        0        0     4233 2023-01-11 08:01:06.463851 dputils-0.2.4/dputils/files.py
+-rw-r--r--   0        0        0     7988 2023-01-23 12:38:16.785170 dputils-0.2.4/dputils/scrape.py
+-rw-r--r--   0        0        0     1088 2022-06-11 05:17:23.834462 dputils-0.2.4/LICENSE
+-rw-r--r--   0        0        0     1035 2023-06-25 11:42:55.326649 dputils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2302 2023-01-23 12:08:08.523476 dputils-0.2.4/readme.md
+-rw-r--r--   0        0        0     3137 2023-06-25 11:46:53.425579 dputils-0.2.4/setup.py
+-rw-r--r--   0        0        0     3227 2023-06-25 11:46:53.426717 dputils-0.2.4/PKG-INFO
```

### Comparing `dputils-0.2.3/dputils/.DS_Store` & `dputils-0.2.4/dputils/.DS_Store`

 * *Files identical despite different names*

### Comparing `dputils-0.2.3/dputils/files.py` & `dputils-0.2.4/dputils/files.py`

 * *Files identical despite different names*

### Comparing `dputils-0.2.3/dputils/scrape.py` & `dputils-0.2.4/dputils/scrape.py`

 * *Files identical despite different names*

### Comparing `dputils-0.2.3/LICENSE` & `dputils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dputils-0.2.3/pyproject.toml` & `dputils-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dputils"
-version = "0.2.3"
+version = "0.2.4"
 description = "This library is utility library from digipodium"
 authors = ["AkulS1008 <akulsingh0708@gmail.com>", "Team Digipodium"]
 maintainers = ["Zaid Kamil <xaidmetamorphos@gmail.com>"]
 readme = "readme.md"
 license = "MIT"
 
 homepage = "https://digipodium.github.io/dputils/"
```

### Comparing `dputils-0.2.3/readme.md` & `dputils-0.2.4/readme.md`

 * *Files identical despite different names*

### Comparing `dputils-0.2.3/setup.py` & `dputils-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'fpdf2>=2.5.4,<3.0.0',
  'pdfminer.six>=20220524,<20220525',
  'python-docx>=0.8.11,<0.9.0',
  'requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'dputils',
-    'version': '0.2.3',
+    'version': '0.2.4',
     'description': 'This library is utility library from digipodium',
     'long_description': 'A python library which can be used to extraxct data from files, pdfs, doc(x) files, as well as save data into these\nfiles. This library can be used to scrape and extract webpage data from websites as well.\n\n### Installation Requirements and Instructions\n\nPython versions 3.8 or above should be installed. After that open your terminal:\nFor Windows users:\n\n```shell\npip install dputils\n```\n\nFor Mac/Linux users:\n\n```shell\npip3 install dputils\n```\n\n### Files Modules\n\nFunctions from dputils.files:\n\n1. get_data:\n    - To import, use statement:\n        ```python3\n\nfrom dputils.files import get_data\n\n```\n- Obtains data from files of any extension given as args(supports text files, binary files, pdf, doc for now, more\ncoming!)\n- sample call:\n```python3\ncontent = get_data(r"sample.docx")\nprint(content)\n```\n\n- Returns a string or binary data depending on the output arg\n- images will not be extracted\n\n2. save_data:\n- save_data can be used to write and save data into a file of valid extension.\n- sample call:\n```python3\nfrom dputils.files import save_data\n\npdfContent = save_data("sample.pdf", "Sample text to insert")\nprint(pdfContent)\n```\n- Returns True if file is successfully accessed and modified. Otherwise, False.\n\n### Scrape Modules\n\nThe Scraper class is a web scraping tool that uses the BeautifulSoup library to extract data from a specified URL. The\nclass has several methods including init, validate_url, clean_url, soup, get, and get_all. The init method takes in a\nURL, a user agent, cookies, and a clean flag. The validate_url method checks if the URL is valid and the clean_url\nmethod removes any query parameters from the URL. The soup method makes a request to the URL and returns a BeautifulSoup\nobject of the webpage. The get method takes in a list of Tag objects and returns a dictionary of the extracted data. The\nget_all method takes in a target tag, an items tag, and a list of tags and returns a list of dictionaries of the\nextracted data for each item. The class also has the ability to handle errors and provide information about the\nextraction process.\n\nThese functions can used on python versions 3.8 or greater.\n\nReferences for more help: https://github.com/digipodium/dputils\n\nThank you for using dputils!',
     'author': 'AkulS1008',
     'author_email': 'akulsingh0708@gmail.com',
     'maintainer': 'Zaid Kamil',
     'maintainer_email': 'xaidmetamorphos@gmail.com',
     'url': 'https://digipodium.github.io/dputils/',
```

### Comparing `dputils-0.2.3/PKG-INFO` & `dputils-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dputils
-Version: 0.2.3
+Version: 0.2.4
 Summary: This library is utility library from digipodium
 Home-page: https://digipodium.github.io/dputils/
 License: MIT
 Author: AkulS1008
 Author-email: akulsingh0708@gmail.com
 Maintainer: Zaid Kamil
 Maintainer-email: xaidmetamorphos@gmail.com
```

