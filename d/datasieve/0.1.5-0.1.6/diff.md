# Comparing `tmp/datasieve-0.1.5.tar.gz` & `tmp/datasieve-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.1.5.tar", max compression
+gzip compressed data, was "datasieve-0.1.6.tar", max compression
```

## Comparing `datasieve-0.1.5.tar` & `datasieve-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1059 2023-06-17 14:14:28.752287 datasieve-0.1.5/LICENSE
--rw-r--r--   0        0        0    11780 2023-06-17 14:14:28.752287 datasieve-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/__init__.py
--rw-r--r--   0        0        0     8644 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/pipeline.py
--rw-r--r--   0        0        0      567 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     3228 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/base_transform.py
--rw-r--r--   0        0        0     5683 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     2748 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1357 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/noise.py
--rw-r--r--   0        0        0     1334 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1491 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/sklearn_wrapper.py
--rw-r--r--   0        0        0     1589 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1585 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3275 2023-06-17 14:14:28.752287 datasieve-0.1.5/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-06-17 14:14:28.752287 datasieve-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    12406 1970-01-01 00:00:00.000000 datasieve-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-06-25 13:43:39.659777 datasieve-0.1.6/LICENSE
+-rw-r--r--   0        0        0     9244 2023-06-25 13:43:39.659777 datasieve-0.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 13:43:39.659777 datasieve-0.1.6/datasieve/__init__.py
+-rw-r--r--   0        0        0     8702 2023-06-25 13:43:39.659777 datasieve-0.1.6/datasieve/pipeline.py
+-rw-r--r--   0        0        0      567 2023-06-25 13:43:39.659777 datasieve-0.1.6/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     3228 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/base_transform.py
+-rw-r--r--   0        0        0     5683 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     2748 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1357 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/noise.py
+-rw-r--r--   0        0        0     1334 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1491 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/sklearn_wrapper.py
+-rw-r--r--   0        0        0     1589 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1585 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3275 2023-06-25 13:43:39.663777 datasieve-0.1.6/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-06-25 13:43:39.663777 datasieve-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9870 1970-01-01 00:00:00.000000 datasieve-0.1.6/PKG-INFO
```

### Comparing `datasieve-0.1.5/LICENSE` & `datasieve-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/README.md` & `datasieve-0.1.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: datasieve
+Version: 0.1.6
+Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
+License: MIT
+Author: Robert Caulk
+Requires-Python: >=3.8.1,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pandas (==2.0.2)
+Requires-Dist: scikit-learn (>=1.1.3)
+Description-Content-Type: text/markdown
+
+![datasieve-logo](assets/datasieve_logo.png)
+
 # DataSieve
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
 
 - fits an arbitrary series of transformations to an array X
 - transforms subsequent arrays of the same dimension according to the fit from the original X
 - inverse transforms arrays by inverting the series of transformations
@@ -115,78 +133,14 @@
 
 The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `MinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `Pipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
 Another feature is demonstrated in the `PCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `Pipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `VarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `VarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
 
-## Adding a custom step
-
-Each step of the `Pipeline` *must* contain the following methods:
-
-```python
-class MyTransformer(BaseTransform):
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        This method is defined by default by the BaseTransform class. But users can override
-        to do something unique (see DBSCAN where this is particularly useful.)
-        """
-        X, y, sample_weight = self.fit(X, y, sample_weight)
-        return self.transform(X, y, sample_weight)
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Some fun fitting method
-        """
-        return X, y, sample_weight, feature_list
-
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Transformation of X or y or sample_weight or all three, anything the user
-        wants.
-        """
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        The inverse transform - it is defined like this by default in BaseTransform class
-        """
-        return X, y, sample_weight, feature_list
-```
-
-This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
-
-```python
-class DataSieveMinMaxScaler(MinMaxScaler):
-    """
-    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
-    inverse_transform all take the full set of params X, y, sample_weight (even if they
-    are unused) to follow the FlowdaptPipeline API.
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        X = super().transform(X)
-        return X, y, sample_weight, feature_list
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        return X, y, sample_weight, feature_list
-
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        X = super().transform(X)
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        return super().inverse_transform(X), y, sample_weight, feature_list
-```
-
 
 ## Outlier checking
 
 DataSieve also allows users to fit a pipeline that can be used to flag outliers in data *without* removing them from the dataset. This may be handy in a variety of cases where keeping the data point is important but having some indication of which points are outliers is also important. In order to use this functionality, you can take an already `fit` pipeline and call `transform(X, outlier_check=True)` which will return X as well as a vector of 1s and 0s indicating which points are outliers. This is demonstrated in the following example:
 
 ```python
 pipeline = Pipeline([
@@ -235,8 +189,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `datasieve-0.1.5/datasieve/pipeline.py` & `datasieve-0.1.6/datasieve/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 y,
                 sample_weight=sample_weight,
                 feature_list=feature_list,
                 outlier_check=outlier_check,
                 **self.fitparams[name]
             )
 
-        X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list)
+        X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list, outlier_check)
 
         return X, y, sample_weight
 
     def fit(self, X, y=None, sample_weight=None):
         X, y, sample_weight = self._validate_arguments(X, y, sample_weight, fit=True)
         feature_list = copy.deepcopy(self.feature_list)
 
@@ -191,23 +191,23 @@
 
         if fit and outlier_check:
             raise Exception("Asking for outlier_check with fit() is not possible."
                             "outlier_check functionality only works with transform.")
 
         return X, y, sample_weight
 
-    def _convert_back_to_df(self, X, y, sample_weight, feature_list):
+    def _convert_back_to_df(self, X, y, sample_weight, feature_list, outlier_check=False):
         if not self.pandas_types:
             return X, y, sample_weight
 
         assert X.shape[1] == len(feature_list)
 
         X = pd.DataFrame(X, columns=feature_list)
 
-        if y is not None:
+        if y is not None and not outlier_check:
             y = pd.DataFrame(y, columns=self.label_list)
 
         return X, y, sample_weight
 
     def _validate_step(cls, trans: BaseTransform):
         """
         Raise exception if `trans` is not a BaseTransform
```

### Comparing `datasieve-0.1.5/datasieve/transforms/__init__.py` & `datasieve-0.1.6/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/base_transform.py` & `datasieve-0.1.6/datasieve/transforms/base_transform.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/dbscan.py` & `datasieve-0.1.6/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.6/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/noise.py` & `datasieve-0.1.6/datasieve/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/pca.py` & `datasieve-0.1.6/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/sklearn_wrapper.py` & `datasieve-0.1.6/datasieve/transforms/sklearn_wrapper.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.1.6/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.6/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/datasieve/utils.py` & `datasieve-0.1.6/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.1.5/pyproject.toml` & `datasieve-0.1.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.1.5"
+version = "0.1.6"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.1.5/PKG-INFO` & `datasieve-0.1.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1
-Name: datasieve
-Version: 0.1.5
-Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
-License: MIT
-Author: Robert Caulk
-Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (==2.0.2)
-Requires-Dist: scikit-learn (>=1.1.3)
-Description-Content-Type: text/markdown
+![datasieve-logo](assets/datasieve_logo.png)
 
 # DataSieve
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
 
 - fits an arbitrary series of transformations to an array X
 - transforms subsequent arrays of the same dimension according to the fit from the original X
@@ -131,78 +117,14 @@
 
 The command `feature_pipeline.fit_transform(X, y, sample_weight)` fits each pipeline step to `X`, and transforms `X` according to each step's `transform()` method. In some cases, this will not affect `y` or `sample_weight`. For example, `MinMaxScaler` simply scales `X` and saves the normalization information.  Meanwhile, in the `SVMOutlierExtractor`, `.fit()` will fit an SVM to `X` and `.transform()` will remove any detected outliers from `X`. Typical `Scikit-Learn` pipelines do not remove those data points from `y` and `sample_weight`. Luckily, the `Pipeline` takes care of the "associated removal" of the same outlier data points from `y` and `sample_weight`. 
 
 ## Feature modification
 
 Another feature is demonstrated in the `PCA`, which fits a PCA transform to `X` and then transforms `X` to principal components. This dimensionality reduction means that the features are no longer the same, instead they are now `PC1`, `PC2` ... `PCX`. `Pipeline` handles the feature renaming at that step (which is not a feature available in the `Scikit-Learn` pipeline). Similar to `FlowdaptPCA`, the `VarianceThreshold` subclasses the `Scikit-Learn` `VarianceThreshold` which is geared toward removing features that have a low variance. `VarianceThreshold` ensures that the removed features are properly handled when `X` passes through this part of the pipeline.
 
-## Adding a custom step
-
-Each step of the `Pipeline` *must* contain the following methods:
-
-```python
-class MyTransformer(BaseTransform):
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        This method is defined by default by the BaseTransform class. But users can override
-        to do something unique (see DBSCAN where this is particularly useful.)
-        """
-        X, y, sample_weight = self.fit(X, y, sample_weight)
-        return self.transform(X, y, sample_weight)
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Some fun fitting method
-        """
-        return X, y, sample_weight, feature_list
-
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        Transformation of X or y or sample_weight or all three, anything the user
-        wants.
-        """
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        """
-        The inverse transform - it is defined like this by default in BaseTransform class
-        """
-        return X, y, sample_weight, feature_list
-```
-
-This is because these four methods are called automatically by the `Pipeline` object. In most cases, the goal is to add functionality for an existing transformer from the `Scikit-Learn` library. Here is an example of subclassing the `MinMaxScaler` to work with the `FlowdaptPipeline`:
-
-```python
-class DataSieveMinMaxScaler(MinMaxScaler):
-    """
-    A subclass of the SKLearn MinMaxScaler that ensures fit, transform, fit_transform and
-    inverse_transform all take the full set of params X, y, sample_weight (even if they
-    are unused) to follow the FlowdaptPipeline API.
-    """
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-
-    def fit_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        X = super().transform(X)
-        return X, y, sample_weight, feature_list
-
-    def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        super().fit(X)
-        return X, y, sample_weight, feature_list
-
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        X = super().transform(X)
-        return X, y, sample_weight, feature_list
-
-    def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
-        return super().inverse_transform(X), y, sample_weight, feature_list
-```
-
 
 ## Outlier checking
 
 DataSieve also allows users to fit a pipeline that can be used to flag outliers in data *without* removing them from the dataset. This may be handy in a variety of cases where keeping the data point is important but having some indication of which points are outliers is also important. In order to use this functionality, you can take an already `fit` pipeline and call `transform(X, outlier_check=True)` which will return X as well as a vector of 1s and 0s indicating which points are outliers. This is demonstrated in the following example:
 
 ```python
 pipeline = Pipeline([
@@ -251,8 +173,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

