# Comparing `tmp/MLandPattern-0.2.1.tar.gz` & `tmp/MLandPattern-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.2.1.tar", last modified: Mon Jun 12 15:36:54 2023, max compression
+gzip compressed data, was "MLandPattern-0.2.2.tar", last modified: Sun Jun 25 15:30:44 2023, max compression
```

## Comparing `MLandPattern-0.2.1.tar` & `MLandPattern-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.969108 MLandPattern-0.2.1/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.963367 MLandPattern-0.2.1/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    21914 2023-06-12 15:34:46.000000 MLandPattern-0.2.1/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.1/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-12 15:36:54.967072 MLandPattern-0.2.1/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-12 15:36:54.000000 MLandPattern-0.2.1/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-12 15:36:54.968780 MLandPattern-0.2.1/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.1/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-12 15:36:54.969255 MLandPattern-0.2.1/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-12 15:34:54.000000 MLandPattern-0.2.1/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.651630 MLandPattern-0.2.2/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.644349 MLandPattern-0.2.2/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    21938 2023-06-13 15:17:56.000000 MLandPattern-0.2.2/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.2.2/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-06-25 15:30:44.650589 MLandPattern-0.2.2/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-06-25 15:30:44.000000 MLandPattern-0.2.2/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-06-25 15:30:44.651290 MLandPattern-0.2.2/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.2.2/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-06-25 15:30:44.651772 MLandPattern-0.2.2/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-06-25 15:30:07.000000 MLandPattern-0.2.2/setup.py
```

### Comparing `MLandPattern-0.2.1/MLandPattern/MLandPattern.py` & `MLandPattern-0.2.2/MLandPattern/MLandPattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,16 +319,16 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}%')
-        print(f'Error: {(100 - acc)}%')
+        # print(f'Accuracy: {acc}%')
+        # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
 def MVG_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the MultiVariate Gaussian classifier on the logarithm dimension for a set of data, and applyes it to a test dataset
@@ -359,16 +359,16 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}%')
-        print(f'Error: {(100 - acc)}%')
+        # print(f'Accuracy: {acc}%')
+        # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
 def Naive_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier for a set of data, and applyes it to a test dataset
@@ -400,16 +400,16 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}%')
-        print(f'Error: {(100 - acc)}%')
+        # print(f'Accuracy: {acc}%')
+        # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
 def Naive_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier on the logarithm realm for a set of data, and applyes it to a test dataset
@@ -442,16 +442,16 @@
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
         acc = round(acc*100, 2)
-        print(f'Accuracy: {acc}%')
-        print(f'Error: {(100 - acc)}%')
+        # print(f'Accuracy: {acc}%')
+        # print(f'Error: {(100 - acc)}%')
 
     return S, predictions, acc
 
 
 def TiedGaussian(train_data, train_labels, test_data, prior_probability, test_label=[]):
     '''
     Calculates the model of the Tied Gaussian classifier for a set of data, and applyes it to a test dataset
@@ -481,16 +481,16 @@
 
     if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc /= len(test_label)
-        print(f"Accuracy: {acc}")
-        print(f"Error: {1 - acc}")
+        # print(f"Accuracy: {acc}")
+        # print(f"Error: {1 - acc}")
 
     return S, predictions, acc
 
 def Tied_Naive_classifier(
     train_data, train_labels, test_data, prior_probability, test_label=[]
 ):
     '''
@@ -522,16 +522,16 @@
 
     if len(test_label) != 0:
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc /= len(test_label)
-        print(f"Accuracy: {acc*100}%")
-        print(f"Error: {(1 - acc)*100}%")
+        # print(f"Accuracy: {acc*100}%")
+        # print(f"Error: {(1 - acc)*100}%")
 
     return S, predictions, acc
 
 
 
 def split_db(D, L, ratio, seed=0):
     '''
```

