# Comparing `tmp/caped-ai-augmentations-1.0.5.tar.gz` & `tmp/caped-ai-augmentations-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/caped-ai-augmentations/dist/.tmp-ghv26k6k/caped-ai-augmentations-1.0.5.tar", last modified: Fri Dec 23 18:23:28 2022, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/caped-ai-augmentations/dist/.tmp-ibbtoh4a/caped-ai-augmentations-1.0.6.tar", last modified: Sun Jun 25 12:38:41 2023, max compression
```

## Comparing `caped-ai-augmentations-1.0.5.tar` & `caped-ai-augmentations-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-12-23 18:23:28.261172 caped-ai-augmentations-1.0.5/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1512 2022-09-07 10:32:19.000000 caped-ai-augmentations-1.0.5/LICENSE
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      738 2022-12-23 18:23:28.259171 caped-ai-augmentations-1.0.5/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       75 2022-09-07 10:16:18.000000 caped-ai-augmentations-1.0.5/README.md
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-12-23 18:23:28.180650 caped-ai-augmentations-1.0.5/caped_ai_augmentations/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    11274 2022-10-03 15:24:38.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentTYXCsv.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    11983 2022-10-03 15:24:27.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentTZYXCsv.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    11396 2022-12-23 18:22:21.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentYX.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    12485 2022-12-23 15:45:33.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentYXC.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)    13152 2022-10-03 15:25:00.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentZYX.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      315 2022-10-12 12:10:32.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/__init__.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      105 2022-12-23 18:22:53.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/_version.py
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     4537 2022-09-07 10:31:25.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations/utils.py
-drwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        0 2022-12-23 18:23:28.244170 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      738 2022-12-23 18:23:27.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/PKG-INFO
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)      548 2022-12-23 18:23:28.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/SOURCES.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)        1 2022-12-23 18:23:27.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/dependency_links.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       71 2022-12-23 18:23:27.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/requires.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       23 2022-12-23 18:23:27.000000 caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/top_level.txt
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)       38 2022-12-23 18:23:28.262170 caped-ai-augmentations-1.0.5/setup.cfg
--rwxrwxrwx   0 varunkapoor  (1000) varunkapoor  (1000)     1294 2022-12-01 18:01:12.000000 caped-ai-augmentations-1.0.5/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.582453 caped-ai-augmentations-1.0.6/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1512 2022-09-07 10:32:19.000000 caped-ai-augmentations-1.0.6/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-06-25 12:38:41.578451 caped-ai-augmentations-1.0.6/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       75 2022-09-07 10:16:18.000000 caped-ai-augmentations-1.0.6/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.395400 caped-ai-augmentations-1.0.6/caped_ai_augmentations/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11274 2022-10-03 15:24:38.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTYXCsv.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11983 2022-10-03 15:24:27.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTZYXCsv.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    11894 2022-12-23 20:19:23.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYX.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    12485 2022-12-23 15:45:33.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYXC.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13152 2022-10-03 15:25:00.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentZYX.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      315 2022-10-12 12:10:32.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      105 2023-06-25 12:38:07.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/_version.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     4537 2022-12-23 19:35:26.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations/utils.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-25 12:38:41.540733 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      738 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      548 2023-06-25 12:38:41.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       66 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       23 2023-06-25 12:38:40.000000 caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-25 12:38:41.599793 caped-ai-augmentations-1.0.6/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1289 2023-06-25 12:37:58.000000 caped-ai-augmentations-1.0.6/setup.py
```

### Comparing `caped-ai-augmentations-1.0.5/LICENSE` & `caped-ai-augmentations-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/PKG-INFO` & `caped-ai-augmentations-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.5
+Version: 1.0.6
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentTYXCsv.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentTZYXCsv.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentTZYXCsv.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentYX.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYX.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,32 +110,37 @@
        
 
         parse_dict = {}
         callback_geometric = None
         callback_intensity = None
 
 
-       
+        #flipud
+        if (self.vertical_flip is not None):
+            callback_geometric = self._flipud_image
+          
+        if (self.horizontal_flip is not None):
+            callback_geometric = self._fliplr_image    
    
 
         # elastic deformation
         if (self.alpha_affine is not None):
              callback_geometric = self._elastic_deform_image
              parse_dict['alpha'] = self.alpha       
              parse_dict['sigma'] = self.sigma
              parse_dict['alpha_affine'] = self.alpha_affine
 
         # rotate
         if  (self.rotate_angle is not None):
             callback_geometric = self._rotate_image
 
             if self.rotate_angle == 'random':
-                parse_dict['rotate_angle'] = np.radians(int(np.random.uniform(-180, 180)))
+                parse_dict['rotate_angle'] = int(np.random.uniform(-180, 180))
             elif type(self.rotate_angle) == int:
-                parse_dict['rotate_angle'] = np.radians(self.rotate_angle)
+                parse_dict['rotate_angle'] = self.rotate_angle
             else:
                 raise ValueError('Rotate angle should be int or random')
 
         # add additive noise
         if (self.distribution is not None):
 
             callback_intensity = self._noise_image  
@@ -200,16 +205,25 @@
         ret_image = callback(target_image,  parse_dict) 
         ret_labelimage =  callback(target_labelimage,  parse_dict) 
 
         return ret_image, ret_labelimage
 
 
    
+    def _flipud_image(self, image, parse_dict):
+        
+        aug_image = np.flipud(image)
+        
+        return aug_image 
          
-  
+    def _fliplr_image(self, image, parse_dict):
+        
+        aug_image = np.fliplr(image)
+        
+        return aug_image
 
     def _elastic_deform_image(self, image, parse_dict):
         """ Elastically deform the image """
         alpha = parse_dict['alpha']
         alpha_affine = parse_dict['alpha_affine']
         sigma = parse_dict['sigma']
         elastic_transform = ElasticTransform(alpha = alpha, alpha_affine = alpha_affine, sigma = sigma)
@@ -279,14 +293,16 @@
           return aug_image
 
     def _rotate_image(self, image, parse_dict):
         """rotate array usiong affine transformation and also if the csv file of coordinates is supplied"""
         rotate_angle = parse_dict['rotate_angle']
        
         aug_image = rotate(image, rotate_angle)
+         
+        aug_image = aug_image + image 
                
         return aug_image   
 
 
     
 def matrix_transform_block(image, matrix):
```

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentYXC.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentYXC.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/AugmentZYX.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/AugmentZYX.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations/utils.py` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations/utils.py`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/PKG-INFO` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caped-ai-augmentations
-Version: 1.0.5
+Version: 1.0.6
 Summary: Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.
 Home-page: https://github.com/Kapoorlabs-CAPED/Augmentations/
 Author: Varun Kapoor
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `caped-ai-augmentations-1.0.5/caped_ai_augmentations.egg-info/SOURCES.txt` & `caped-ai-augmentations-1.0.6/caped_ai_augmentations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caped-ai-augmentations-1.0.5/setup.py` & `caped-ai-augmentations-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     description='Augmentations for volume, planar segmentation, classification image segmentation and associated csv file of oneat clicks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         "albumentations",
         "scipy",
         "opencv-python",
-        "scikit-learn",
+        "sklearn",
         "dask",
         "natsort",
         "photutils",
        
     ],
     packages=setuptools.find_packages(),
     classifiers=[
```

