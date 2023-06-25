# Comparing `tmp/IMDBTraktSyncer-1.5.1.tar.gz` & `tmp/IMDBTraktSyncer-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDBTraktSyncer-1.5.1.tar", last modified: Mon Jun 19 16:13:11 2023, max compression
+gzip compressed data, was "IMDBTraktSyncer-1.5.2.tar", last modified: Sun Jun 25 00:18:13 2023, max compression
```

## Comparing `IMDBTraktSyncer-1.5.1.tar` & `IMDBTraktSyncer-1.5.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.126736 IMDBTraktSyncer-1.5.1/
-drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.093737 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/
--rw-rw-rw-   0        0        0    35208 2023-06-19 16:10:38.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/IMDBTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     6693 2023-06-19 09:47:56.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorHandling.py
--rw-rw-rw-   0        0        0     1797 2023-06-19 16:10:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorLogger.py
--rw-rw-rw-   0        0        0    10221 2023-06-19 09:48:14.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/imdbData.py
--rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/traktData.py
--rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-06-19 16:13:11.123746 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0    12155 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      549 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-06-19 16:13:10.000000 IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.1/LICENSE
--rw-rw-rw-   0        0        0    12155 2023-06-19 16:13:11.125747 IMDBTraktSyncer-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    11409 2023-06-19 09:51:38.000000 IMDBTraktSyncer-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 16:13:11.126736 IMDBTraktSyncer-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1377 2023-06-19 16:12:51.000000 IMDBTraktSyncer-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.452952 IMDBTraktSyncer-1.5.2/
+drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.419464 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/
+-rw-rw-rw-   0        0        0    35244 2023-06-24 23:28:03.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/IMDBTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     4624 2023-06-19 09:47:47.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4317 2023-06-19 09:47:23.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     6941 2023-06-24 23:42:02.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorHandling.py
+-rw-rw-rw-   0        0        0     1669 2023-06-25 00:09:11.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorLogger.py
+-rw-rw-rw-   0        0        0    10647 2023-06-25 00:08:47.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/imdbData.py
+-rw-rw-rw-   0        0        0    10353 2023-06-19 09:48:23.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/traktData.py
+-rw-rw-rw-   0        0        0    12192 2023-06-19 15:47:42.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-06-25 00:18:13.449956 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0    12155 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      549 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-25 00:18:13.000000 IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDBTraktSyncer-1.5.2/LICENSE
+-rw-rw-rw-   0        0        0    12155 2023-06-25 00:18:13.451940 IMDBTraktSyncer-1.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11409 2023-06-25 00:16:59.000000 IMDBTraktSyncer-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 00:18:13.452952 IMDBTraktSyncer-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1377 2023-06-25 00:17:18.000000 IMDBTraktSyncer-1.5.2/setup.py
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/IMDBTraktSyncer.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/IMDBTraktSyncer.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                 raise SystemExit
             else:
                 raise
 
         wait = WebDriverWait(driver, 10)
         
         # Load sign in page
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/registration/signin', driver)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/registration/signin', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         # wait for sign in link to appear and then click it
         sign_in_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, 'a.list-group-item > .auth-provider-text')))
         if 'IMDb' in sign_in_link.text:
@@ -91,15 +91,15 @@
         password_input.send_keys(imdb_password)
         submit_button = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, "input[type='submit']")))
         submit_button.click()
 
         time.sleep(2)
 
         # go to IMDB homepage
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/', driver)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         time.sleep(2)
 
         # Check if signed in
@@ -222,15 +222,15 @@
                 for item in imdb_watchlist_to_set:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                         print(f" - Adding item ({item_count} of {num_items}): {item['Title']}{year_str} to IMDB Watchlist")
                         
                         # Load page
-                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
                         # Wait until the loader has disappeared, indicating the watchlist button has loaded
                         wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
                         
@@ -339,15 +339,15 @@
                 for i, item in enumerate(imdb_ratings_to_set, 1):
 
                     year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                     print(f' - Rating {item["Type"]}: ({i} of {len(imdb_ratings_to_set)}) {item["Title"]}{year_str}: {item["Rating"]}/10 on IMDB')
                     
                     try:
                         # Load page
-                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
                         # Wait until the rating bar has loaded
                         wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="hero-rating-bar__loading"]')))
                         
@@ -444,15 +444,15 @@
                         
                         for review in imdb_reviews_to_set:
                             item_count += 1
                             try:
                                 print(f" - Submitting review ({item_count} of {num_items}): {review['Title']} ({review['Year']}) on IMDB")
                                 
                                 # Load page
-                                success, status_code, url = EH.get_page_with_retries(f'https://contribute.imdb.com/review/{review["IMDB_ID"]}/add?bus=imdb', driver)
+                                success, status_code, url = EH.get_page_with_retries(f'https://contribute.imdb.com/review/{review["IMDB_ID"]}/add?bus=imdb', driver, wait)
                                 if not success:
                                     # Page failed to load, raise an exception
                                     raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                                 
                                 review_title_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "input.klondike-input")))
                                 review_input = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, "textarea.klondike-textarea")))
                                 
@@ -557,15 +557,15 @@
                 for item in imdb_watchlist_items_to_remove:
                     try:
                         item_count += 1
                         year_str = f' ({item["Year"]})' if item["Year"] is not None else '' # sometimes year is None for episodes from trakt so remove it from the print string
                         print(f" - Removing item ({item_count} of {num_items}): {item['Title']}{year_str} from IMDB Watchlist")
                         
                         # Load page
-                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver)
+                        success, status_code, url = EH.get_page_with_retries(f'https://www.imdb.com/title/{item["IMDB_ID"]}/', driver, wait)
                         if not success:
                             # Page failed to load, raise an exception
                             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
                         
                         # Wait until the loader has disappeared, indicating the watchlist button has loaded
                         wait.until(EC.invisibility_of_element_located((By.CSS_SELECTOR, '[data-testid="tm-box-wl-loader"]')))
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/authTrakt.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/checkChromedriver.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorHandling.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorHandling.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import traceback
 import requests
 import time
-from selenium.common.exceptions import WebDriverException
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+from selenium.webdriver.common.by import By
+from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
+from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.common.by import By
+from selenium.common.exceptions import SessionNotCreatedException
 try:
     from IMDBTraktSyncer import verifyCredentials as VC
     from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import verifyCredentials as VC
     import errorLogger as EL
 
@@ -102,26 +106,26 @@
         521: "Service Unavailable - Cloudflare error",
         522: "Service Unavailable - Cloudflare error"
     }
 
     return error_messages.get(status_code, "Unknown error")
 
 # Function to get page with retries and adjusted wait time
-def get_page_with_retries(url, driver, total_wait_time=180, initial_wait_time=5):
+def get_page_with_retries(url, driver, wait, total_wait_time=180, initial_wait_time=5):
     num_retries = total_wait_time // initial_wait_time
     wait_time = total_wait_time / num_retries
     max_retries = num_retries
     status_code = None
 
     for retry in range(max_retries):
         try:
             driver.get(url)
             
             # Wait until the page has finished loading
-            WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.TAG_NAME, 'body')))
+            wait.until(EC.presence_of_element_located((By.TAG_NAME, 'body')))
             
             # Get the HTTP status code of the page using JavaScript
             status_code = driver.execute_script(
                 """
                 var xhr = new XMLHttpRequest();
                 xhr.open('GET', window.location.href, false);
                 xhr.send(null);
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/errorLogger.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/errorLogger.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,11 +39,8 @@
 
 # Set the log format
 formatter = CustomFormatter('%(asctime)s - %(levelname)s - %(message)s')
 handler.setFormatter(formatter)
 
 # Get the root logger and add the handler
 logger = logging.getLogger('')
-logger.addHandler(handler)
-
-# Set the logging level for selenium.webdriver to WARNING
-logging.getLogger('selenium.webdriver').setLevel(logging.WARNING)
+logger.addHandler(handler)
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/imdbData.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/imdbData.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 from selenium.webdriver.common.by import By
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, StaleElementReferenceException
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
+from selenium.common.exceptions import SessionNotCreatedException
 from chromedriver_py import binary_path
 try:
     from IMDBTraktSyncer import errorHandling as EH
     from IMDBTraktSyncer import errorLogger as EL
 except ImportError:
     import errorHandling as EH
     import errorLogger as EL
@@ -23,15 +24,15 @@
 def getImdbData(imdb_username, imdb_password, driver, directory, wait):
     # Process IMDB Ratings Reviews & Watchlist
     print('Processing IMDB Data')
     
     #Get IMDB Watchlist Items
     try:
         # Load page
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/watchlist', driver)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/watchlist', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         csv_link = wait.until(EC.presence_of_element_located((By.CSS_SELECTOR, ".export a")))
         driver.execute_script("arguments[0].scrollIntoView(true);", csv_link)
         csv_link.click()
@@ -75,15 +76,15 @@
         # No IMDB Watchlist Items
         imdb_watchlist = []
         pass
     
     # Get IMDB Ratings
     try:
         # Load page
-        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/ratings', driver)
+        success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/list/ratings', driver, wait)
         if not success:
             # Page failed to load, raise an exception
             raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
 
         dropdown = wait.until(EC.element_to_be_clickable((By.CSS_SELECTOR, ".circle")))
         dropdown.click()
 
@@ -139,15 +140,15 @@
                 media_type = results[0].get('type')
                 return media_type
         return None
 
     #Get IMDB Reviews
     
     # Load page
-    success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/profile', driver)
+    success, status_code, url = EH.get_page_with_retries('https://www.imdb.com/profile', driver, wait)
     if not success:
         # Page failed to load, raise an exception
         raise PageLoadException(f"Failed to load page. Status code: {status_code}. URL: {url}")
     
     reviews = []
     errors_found_getting_imdb_reviews = False
     try:
@@ -193,17 +194,22 @@
 
                     # Wait until the URL changes
                     wait.until(EC.url_changes(current_url))
                     
                     # Refresh review_elements
                     review_elements = wait.until(EC.presence_of_all_elements_located((By.CSS_SELECTOR, ".imdb-user-review")))
 
-                except (NoSuchElementException, TimeoutException):
-                    # "Next" link not found or timed out waiting for the "Next" link, exit the loop without error.
-                    error_message = '"Next" link not found or timed out waiting for the "Next" link, exit the loop without error.'
+                except NoSuchElementException:
+                    # "Next" link not found on IMDB reviews page, exit the loop without error
+                    error_message = '"Next" link not found on IMDB reviews page. Exiting the loop without error.'
+                    EL.logger.warning(error_message, exc_info=True)
+                    break
+                except TimeoutException:
+                    # Timed out waiting for URL change or next page review elements on IMDB reviews page
+                    error_message = 'Timed out waiting for URL change or next page review elements on IMDB reviews page. Exiting the loop without error.'
                     EL.logger.error(error_message, exc_info=True)
                     break
             except Exception as e:
                 errors_found_getting_imdb_reviews = True
                 error_message = f"Exception occurred while getting IMDB reviews: {type(e)}"
                 print(f"{error_message}")
                 EL.logger.error(error_message, exc_info=True)
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/traktData.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/traktData.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer/verifyCredentials.py` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/PKG-INFO` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.1/IMDBTraktSyncer.egg-info/SOURCES.txt` & `IMDBTraktSyncer-1.5.2/IMDBTraktSyncer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/LICENSE` & `IMDBTraktSyncer-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/PKG-INFO` & `IMDBTraktSyncer-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDBTraktSyncer
-Version: 1.5.1
+Version: 1.5.2
 Summary: A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.
 Home-page: https://github.com/RileyXX/IMDB-Trakt-Syncer
 Author: RileyXX
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IMDBTraktSyncer-1.5.1/README.md` & `IMDBTraktSyncer-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `IMDBTraktSyncer-1.5.1/setup.py` & `IMDBTraktSyncer-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), 'r', encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 DESCRIPTION = 'A python script that syncs user watchlist, ratings and comments for Movies, TV Shows and Episodes both ways between Trakt and IMDB.'
 
 # Setting up
 setup(
     name="IMDBTraktSyncer",
     version=VERSION,
     author="RileyXX",
```

