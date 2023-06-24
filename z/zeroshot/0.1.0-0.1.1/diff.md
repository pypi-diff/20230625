# Comparing `tmp/zeroshot-0.1.0.tar.gz` & `tmp/zeroshot-0.1.1.tar.gz`

## Comparing `zeroshot-0.1.0.tar` & `zeroshot-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,26 @@
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.0/.git
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zeroshot-0.1.0/zeroshot/__init__.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 zeroshot-0.1.0/zeroshot/classifier.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.0/.gitignore
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 zeroshot-0.1.0/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 zeroshot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 zeroshot-0.1.1/.git
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 zeroshot-0.1.1/requirements.txt
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 zeroshot-0.1.1/requirements_dev.txt
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 zeroshot-0.1.1/.github/workflows/integration_python.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.1/.github/workflows/lint_python.yml
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 zeroshot-0.1.1/.github/workflows/test_python.yml
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 zeroshot-0.1.1/examples/run_classification.ipynb
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 zeroshot-0.1.1/scripts/integration_test.py
+-rw-r--r--   0        0        0   101818 2020-02-02 00:00:00.000000 zeroshot-0.1.1/scripts/test_files/bus.png
+-rw-r--r--   0        0        0   120385 2020-02-02 00:00:00.000000 zeroshot-0.1.1/scripts/test_files/dog.png
+-rw-r--r--   0        0        0    33248 2020-02-02 00:00:00.000000 zeroshot-0.1.1/scripts/test_files/test_model.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/__init__.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/classifier.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/classifier_test.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/downloader.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/downloader_test.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/feature_extractor.py
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/feature_extractor_test.py
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/logistic_regression.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/logistic_regression_test.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/preprocessing.py
+-rw-r--r--   0        0        0    40312 2020-02-02 00:00:00.000000 zeroshot-0.1.1/zeroshot/test_files/test_model.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zeroshot-0.1.1/.gitignore
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 zeroshot-0.1.1/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 zeroshot-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zeroshot-0.1.1/PKG-INFO
```

### Comparing `zeroshot-0.1.0/.gitignore` & `zeroshot-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `zeroshot-0.1.0/pyproject.toml` & `zeroshot-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zeroshot"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Zeroshot Maintainers", email = "hello@usezeroshot.com"},
 ]
 description = "Image classifier with zero-shot learning."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

