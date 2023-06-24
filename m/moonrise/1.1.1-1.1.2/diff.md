# Comparing `tmp/moonrise-1.1.1.tar.gz` & `tmp/moonrise-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonrise-1.1.1.tar", last modified: Sat Jun  3 21:47:22 2023, max compression
+gzip compressed data, was "moonrise-1.1.2.tar", last modified: Sat Jun 24 21:54:38 2023, max compression
```

## Comparing `moonrise-1.1.1.tar` & `moonrise-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.516444 moonrise-1.1.1/
--rw-rw-rw-   0        0        0     1103 2023-05-01 03:19:38.000000 moonrise-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6448 2023-06-03 21:47:22.517445 moonrise-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     5878 2023-05-15 20:49:18.000000 moonrise-1.1.1/README.md
--rw-rw-rw-   0        0        0      104 2023-05-01 03:19:38.000000 moonrise-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      846 2023-06-03 21:47:22.529445 moonrise-1.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.441448 moonrise-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.470447 moonrise-1.1.1/src/moonrise/
--rw-rw-rw-   0        0        0     6864 2023-05-23 21:39:47.000000 moonrise-1.1.1/src/moonrise/Base_Test.py
--rw-rw-rw-   0        0        0     6040 2023-06-02 13:56:46.000000 moonrise-1.1.1/src/moonrise/Moon_Browser.py
--rw-rw-rw-   0        0        0     6562 2023-05-15 15:31:11.000000 moonrise-1.1.1/src/moonrise/Moon_Methods.py
--rw-rw-rw-   0        0        0     2126 2023-06-02 13:56:46.000000 moonrise-1.1.1/src/moonrise/Moon_Movie.py
--rw-rw-rw-   0        0        0     1876 2023-05-15 20:38:47.000000 moonrise-1.1.1/src/moonrise/__init__.py
--rw-rw-rw-   0        0        0     2363 2023-05-11 19:30:47.000000 moonrise-1.1.1/src/moonrise/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-03 21:47:22.514443 moonrise-1.1.1/src/moonrise.egg-info/
--rw-rw-rw-   0        0        0     6448 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 21:47:22.000000 moonrise-1.1.1/src/moonrise.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-24 21:54:38.595596 moonrise-1.1.2/
+-rw-rw-rw-   0        0        0     1103 2023-06-07 21:03:48.000000 moonrise-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     6448 2023-06-24 21:54:38.595596 moonrise-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     5878 2023-06-07 21:03:48.000000 moonrise-1.1.2/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-07 21:03:48.000000 moonrise-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      846 2023-06-24 21:54:38.604595 moonrise-1.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-24 21:54:38.536241 moonrise-1.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-24 21:54:38.561241 moonrise-1.1.2/src/moonrise/
+-rw-rw-rw-   0        0        0     6864 2023-06-24 18:32:03.000000 moonrise-1.1.2/src/moonrise/Base_Test.py
+-rw-rw-rw-   0        0        0     6040 2023-06-24 18:32:03.000000 moonrise-1.1.2/src/moonrise/Moon_Browser.py
+-rw-rw-rw-   0        0        0     9659 2023-06-24 21:52:24.000000 moonrise-1.1.2/src/moonrise/Moon_Methods.py
+-rw-rw-rw-   0        0        0     2126 2023-06-07 21:03:48.000000 moonrise-1.1.2/src/moonrise/Moon_Movie.py
+-rw-rw-rw-   0        0        0     1876 2023-06-13 16:19:06.000000 moonrise-1.1.2/src/moonrise/__init__.py
+-rw-rw-rw-   0        0        0     2363 2023-06-07 21:03:48.000000 moonrise-1.1.2/src/moonrise/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-24 21:54:38.594080 moonrise-1.1.2/src/moonrise.egg-info/
+-rw-rw-rw-   0        0        0     6448 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-24 21:54:38.000000 moonrise-1.1.2/src/moonrise.egg-info/top_level.txt
```

### Comparing `moonrise-1.1.1/LICENSE` & `moonrise-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/PKG-INFO` & `moonrise-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.1
+Version: 1.1.2
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `moonrise-1.1.1/README.md` & `moonrise-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/setup.cfg` & `moonrise-1.1.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6f6f 6e72 6973 650d 0a76 6572   = moonrise..ver
-00000020: 7369 6f6e 203d 2031 2e31 2e31 0d0a 6175  sion = 1.1.1..au
+00000020: 7369 6f6e 203d 2031 2e31 2e32 0d0a 6175  sion = 1.1.2..au
 00000030: 7468 6f72 203d 2043 6872 6973 746f 7068  thor = Christoph
 00000040: 6572 2044 6961 6d6f 6e64 2d4a 6f6e 6573  er Diamond-Jones
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2063 6872 6973 746f 7068 6572 2e6a 6f6e   christopher.jon
 00000070: 6573 3131 3338 4067 6d61 696c 2e63 6f6d  es1138@gmail.com
 00000080: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000090: 5465 7374 2073 7569 7465 2063 7265 6174  Test suite creat
```

### Comparing `moonrise-1.1.1/src/moonrise/Base_Test.py` & `moonrise-1.1.2/src/moonrise/Base_Test.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/src/moonrise/Moon_Browser.py` & `moonrise-1.1.2/src/moonrise/Moon_Browser.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/src/moonrise/Moon_Methods.py` & `moonrise-1.1.2/src/moonrise/Moon_Methods.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
+from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.support.ui import Select
 from selenium.common.exceptions import TimeoutException
 
 class MoonMethods:
     """Common-use methods when locating and interacting with web elements
     """
     
@@ -56,24 +57,33 @@
             False: EC.visibility_of_element_located,
             True: EC.visibility_of_all_elements_located
         }
 
         wait = WebDriverWait(self.moon_driver, time_to_wait)
 
         try:
-            if type(locator) is WebElement:
-                return locator
-            if locator.startswith("/"):
-                return wait.until(multi_element_return.get(get_multiples)((By.XPATH, locator)))
+            if type(locator) is WebElement or type(locator) is MoonElement:
+                results = locator
+            elif locator.startswith("/"):
+                results = wait.until(multi_element_return.get(get_multiples)((By.XPATH, locator)))
             elif locator.split(":")[0] in location_methods:
-                return wait.until(multi_element_return.get(get_multiples)((location_methods[locator.split(":")[0]], locator.split(":")[1])))
+                results = wait.until(multi_element_return.get(get_multiples)((location_methods[locator.split(":")[0]], locator.split(":")[1])))
             else:
-                return wait.until(multi_element_return.get(get_multiples)((By.CSS_SELECTOR, locator)))
+                results = wait.until(multi_element_return.get(get_multiples)((By.CSS_SELECTOR, locator)))
         except TimeoutException:
             raise TimeoutException(f"Could not find '{locator}' after {time_to_wait} seconds.")
+        
+        # Convert WebElement(s) to MoonElement(s)
+        if type(results) is list:
+            elements = []
+            for e in results:
+                elements.append(MoonElement(e))
+            return elements
+        else:
+            return MoonElement(results)
 
     def click_element(self, locator, timeout=None):
         """Click the element identified by ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
@@ -132,8 +142,59 @@
     def get_text(self, locator, timeout=None):
         """Returns the text value of the element identified by ``locator``.
 
            Arguments:
            - ``locator``: The method by which to locate a web element.
            - ``timeout``: How long to search for the element before throwing a TimeoutException.
         """
-        return self.get_web_element(locator=locator, timeout=timeout).text
+        return self.get_web_element(locator=locator, timeout=timeout).text
+    
+    def drag_element_to_element(self, dragged_locator: str, target_locator: str, timeout: int = None):
+        """Clicks and drags one element to another element.
+
+           Arguments:
+           - ``dragged_locator`` (str): Locator for the element to be clicked and dragged.
+           - ``target_locator`` (str): Locator for the element that the dragged element will be dragged to.
+           - ``timeout`` (int, optional): Maximum time (in seconds) to search for both the dragged and target elements before throwing a TimeoutException.
+        """
+        dragged_element = self.get_web_element(locator=dragged_locator, timeout=timeout)
+        target_element = self.get_web_element(locator=target_locator, timeout=timeout)
+
+        ActionChains(self.moon_driver).drag_and_drop(dragged_element, target_element).perform()
+
+    def drag_element_to_offset(self, dragged_locator: str, x_offset: int, y_offset: int, timeout: int = None):
+        """Clicks and drags one element to another element.
+
+           Arguments:
+           - ``dragged_locator`` (str): Locator for the element to be clicked and dragged.
+           - ``x_offset`` (int): The number of pixels to drag the element along the x axis.
+           - ``y_offset`` (int): The number of pixels to drag the element along the y axis.
+           - ``timeout`` (int, optional): Maximum time (in seconds) to search for the dragged element before throwing a TimeoutException.
+        """
+        dragged_element = self.get_web_element(locator=dragged_locator, timeout=timeout)
+
+        ActionChains(self.moon_driver).drag_and_drop_by_offset(dragged_element, xoffset=x_offset, yoffset=y_offset).perform()
+
+class MoonElement(WebElement):
+    """Replacement object for standard WebElements.
+       Inherits all attributes and methods of Selenium WebElements with additional methods. 
+    """
+
+    def __init__(self, element: WebElement):
+        self.element = element
+        self.driver = element.parent
+        super().__init__(self.driver, element.id)
+
+    def get_parent(self):
+        """Return the parent element of a WebElement.
+        """
+        return MoonElement(self.driver.execute_script("return arguments[0].parentNode", self.element))
+    
+    def get_children(self, locator: str = "*"):
+        """Returns all child elements of a WebElement.
+           Arguments:
+           - ``locator``: The method by which to locate children of the given WebElement.
+        """
+        elements = []
+        for e in self.driver.execute_script(f"return arguments[0].querySelectorAll('{locator}')", self.element):
+            elements.append(MoonElement(e))
+        return elements
```

### Comparing `moonrise-1.1.1/src/moonrise/Moon_Movie.py` & `moonrise-1.1.2/src/moonrise/Moon_Movie.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/src/moonrise/__init__.py` & `moonrise-1.1.2/src/moonrise/__init__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/src/moonrise/__main__.py` & `moonrise-1.1.2/src/moonrise/__main__.py`

 * *Files identical despite different names*

### Comparing `moonrise-1.1.1/src/moonrise.egg-info/PKG-INFO` & `moonrise-1.1.2/src/moonrise.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonrise
-Version: 1.1.1
+Version: 1.1.2
 Summary: Test suite creation toolset with additional quality of life upgrades for using the selenium test framework.
 Home-page: https://github.com/Worakow1138/Moonrise
 Author: Christopher Diamond-Jones
 Author-email: christopher.jones1138@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

