# Comparing `tmp/Scrapset-3.1.0.tar.gz` & `tmp/Scrapset-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Scrapset-3.1.0.tar", last modified: Sat Jun 24 08:13:04 2023, max compression
+gzip compressed data, was "Scrapset-3.4.0.tar", last modified: Sun Jun 25 18:38:20 2023, max compression
```

## Comparing `Scrapset-3.1.0.tar` & `Scrapset-3.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:04.470395 Scrapset-3.1.0/
--rw-rw-rw-   0        0        0     4280 2023-06-24 08:13:04.470395 Scrapset-3.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-3.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:04.470395 Scrapset-3.1.0/Scrapset/
--rw-rw-rw-   0        0        0     6578 2023-06-24 08:02:19.000000 Scrapset-3.1.0/Scrapset/Scrapset.py
--rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-3.1.0/Scrapset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-24 08:13:04.470395 Scrapset-3.1.0/Scrapset.egg-info/
--rw-rw-rw-   0        0        0     4280 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-24 08:13:04.000000 Scrapset-3.1.0/Scrapset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-3.1.0/licence.txt
--rw-rw-rw-   0        0        0      158 2023-06-24 08:13:04.470395 Scrapset-3.1.0/setup.cfg
--rw-rw-rw-   0        0        0      499 2023-06-24 08:10:23.000000 Scrapset-3.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.479450 Scrapset-3.4.0/
+-rw-rw-rw-   0        0        0     4280 2023-06-25 18:38:20.479450 Scrapset-3.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4049 2023-06-05 16:18:22.000000 Scrapset-3.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.471162 Scrapset-3.4.0/Scrapset/
+-rw-rw-rw-   0        0        0     6576 2023-06-25 18:37:56.000000 Scrapset-3.4.0/Scrapset/Scrapset.py
+-rw-rw-rw-   0        0        0       49 2023-06-06 18:47:28.000000 Scrapset-3.4.0/Scrapset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-25 18:38:20.478184 Scrapset-3.4.0/Scrapset.egg-info/
+-rw-rw-rw-   0        0        0     4280 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-25 18:38:20.000000 Scrapset-3.4.0/Scrapset.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      632 2023-06-05 15:50:58.000000 Scrapset-3.4.0/licence.txt
+-rw-rw-rw-   0        0        0      158 2023-06-25 18:38:20.480501 Scrapset-3.4.0/setup.cfg
+-rw-rw-rw-   0        0        0      499 2023-06-25 18:38:10.000000 Scrapset-3.4.0/setup.py
```

### Comparing `Scrapset-3.1.0/PKG-INFO` & `Scrapset-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 3.1.0
+Version: 3.4.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-3.1.0/README.md` & `Scrapset-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `Scrapset-3.1.0/Scrapset/Scrapset.py` & `Scrapset-3.4.0/Scrapset/Scrapset.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
             self.url=url
             driver=webdriver.Chrome()
             time.sleep(1)
             list_of_dic = {'title': [],'all_details':[],'up_vote':[],'comments':[]}  # Initialize the dictionary
             while initial_page <= last_page:
                 driver.get(url+f'/discussions?page={initial_page}')
                 initial_page=initial_page+1
-                time.sleep(1.4)
+                time.sleep(3)
                 threads=driver.find_elements(By.XPATH,'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li/div[1]')
                 c=0
                 for thread in threads:
                     c=c+1
                     try:
                         title=thread.find_element(By.XPATH,f'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li[{c}]/div[1]/a/div/div/div').text
                         all_details=thread.find_element(By.XPATH,f'//*[@id="site-content"]/section[2]/div[2]/div/div/div/div/div[4]/ul/li[{c}]/div[1]/a/div/span').text
```

### Comparing `Scrapset-3.1.0/Scrapset.egg-info/PKG-INFO` & `Scrapset-3.4.0/Scrapset.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Scrapset
-Version: 3.1.0
+Version: 3.4.0
 Summary: DataScraper: Effortless Dataset Extraction
 Author: Ibrahim
 Author-email: string2025@gmail.com
 Description-Content-Type: text/markdown
 License-File: licence.txt
 
 # Dataset Scraper (Scrapset)
```

### Comparing `Scrapset-3.1.0/licence.txt` & `Scrapset-3.4.0/licence.txt`

 * *Files identical despite different names*

