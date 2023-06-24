# Comparing `tmp/seaborn-analyzer-0.3.2.tar.gz` & `tmp/seaborn-analyzer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaborn-analyzer-0.3.2.tar", last modified: Wed Jun 21 06:34:36 2023, max compression
+gzip compressed data, was "seaborn-analyzer-0.3.3.tar", last modified: Sat Jun 24 22:37:57 2023, max compression
```

## Comparing `seaborn-analyzer-0.3.2.tar` & `seaborn-analyzer-0.3.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.784345 seaborn-analyzer-0.3.2/
--rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.2/LICENSE
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-21 06:34:36.783991 seaborn-analyzer-0.3.2/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-21 06:25:30.000000 seaborn-analyzer-0.3.2/README.rst
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.782839 seaborn-analyzer-0.3.2/seaborn_analyzer/
--rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-21 06:25:22.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/__init__.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53230 2023-06-21 06:06:04.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set.py
--rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set_old.py
--rw-r--r--   0 knakamura   (501) staff       (20)    82445 2023-06-21 06:21:22.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_class_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_hist_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_pair_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)    97799 2023-06-21 06:18:38.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/custom_reg_plot.py
--rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.2/seaborn_analyzer/multiclass_fitparams.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.783408 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/
--rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/PKG-INFO
--rw-r--r--   0 knakamura   (501) staff       (20)      531 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/SOURCES.txt
--rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/dependency_links.txt
--rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/requires.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-21 06:34:36.000000 seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/top_level.txt
--rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-21 06:34:36.784394 seaborn-analyzer-0.3.2/setup.cfg
--rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.2/setup.py
-drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-21 06:34:36.783545 seaborn-analyzer-0.3.2/tests/
--rw-r--r--   0 knakamura   (501) staff       (20)     3356 2023-06-21 06:33:42.000000 seaborn-analyzer-0.3.2/tests/test_cv.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.817271 seaborn-analyzer-0.3.3/
+-rw-r--r--   0 knakamura   (501) staff       (20)     1522 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.3/LICENSE
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-24 22:37:57.817079 seaborn-analyzer-0.3.3/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)    14461 2023-06-24 22:35:23.000000 seaborn-analyzer-0.3.3/README.rst
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.815336 seaborn-analyzer-0.3.3/seaborn_analyzer/
+-rw-r--r--   0 knakamura   (501) staff       (20)      178 2023-06-24 22:35:28.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/__init__.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53228 2023-06-22 08:57:33.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    53653 2023-06-20 05:30:27.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set_old.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    83193 2023-06-22 09:00:50.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    22202 2021-10-26 17:55:27.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_hist_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    12128 2021-11-01 17:19:31.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_pair_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)    98854 2023-06-24 07:21:33.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/custom_reg_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     1620 2023-06-20 06:33:07.000000 seaborn-analyzer-0.3.3/seaborn_analyzer/multiclass_fitparams.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.816118 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/
+-rw-r--r--   0 knakamura   (501) staff       (20)    15891 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/PKG-INFO
+-rw-r--r--   0 knakamura   (501) staff       (20)      579 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/SOURCES.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)        1 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/dependency_links.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)      155 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/requires.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       17 2023-06-24 22:37:57.000000 seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/top_level.txt
+-rw-r--r--   0 knakamura   (501) staff       (20)       38 2023-06-24 22:37:57.817317 seaborn-analyzer-0.3.3/setup.cfg
+-rw-r--r--   0 knakamura   (501) staff       (20)     2163 2023-06-19 08:02:59.000000 seaborn-analyzer-0.3.3/setup.py
+drwxr-xr-x   0 knakamura   (501) staff       (20)        0 2023-06-24 22:37:57.816738 seaborn-analyzer-0.3.3/tests/
+-rw-r--r--   0 knakamura   (501) staff       (20)     8536 2023-06-24 22:25:10.000000 seaborn-analyzer-0.3.3/tests/test_class_plot.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     3376 2023-06-22 05:49:24.000000 seaborn-analyzer-0.3.3/tests/test_cv.py
+-rw-r--r--   0 knakamura   (501) staff       (20)     8488 2023-06-24 22:18:27.000000 seaborn-analyzer-0.3.3/tests/test_reg_plot.py
```

### Comparing `seaborn-analyzer-0.3.2/LICENSE` & `seaborn-analyzer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/PKG-INFO` & `seaborn-analyzer-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.2
+Version: 0.3.3
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.2 requires
+seaborn-analyzer 0.3.3 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.2/README.rst` & `seaborn-analyzer-0.3.3/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.2 requires
+seaborn-analyzer 0.3.3 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,33 +26,32 @@
 def _eval_set_selection(validation_fraction, 
                         transformer, 
                         X, 
                         y,
                         fit_params, 
                         train, 
                         test, 
-                        random_state,
-                        stratify
+                        random_state
                         ):
     """eval_setの中から学習データ or テストデータのみを抽出"""
     fit_params_modified = copy.deepcopy(fit_params)
     # eval_setが存在しない or Noneなら、そのままfit_paramsを返す
     eval_sets = [v for v in fit_params.keys() if 'eval_set' in v]
     if len(eval_sets) == 0 or fit_params[eval_sets[0]] is None:
-        return fit_params_modified
+        return fit_params_modified, train
     # eval_setの列名(pipelineでは列名が変わるため)
     eval_set_name = eval_sets[0]
     # 元のeval_setからX, yを取得
     X_fit = fit_params[eval_set_name][0][0]
     y_fit = fit_params[eval_set_name][0][1]
     # Training dataの一部をeval_setとして使用する場合
     if isinstance(validation_fraction, float):
         # Select training data from source training data
         rng = np.random.default_rng(seed=random_state)
-        size = int(train.shape[0]*validation_fraction)
+        size = int(train.shape[0]*(1.0 - validation_fraction))
         train_divided = rng.choice(train, size=size, replace=False)
         train_divided.sort()
         # Select validation data from difference set of the selected training data and the source training data
         val_divided = np.setdiff1d(train, train_divided)
         fit_params_modified[eval_set_name] = [(_transform_except_last_estimator(transformer, X[val_divided], X[train_divided])\
                                               , y[val_divided])]
     # Cross validationのテストデータをeval_setとして使用する場合
@@ -88,25 +87,23 @@
     split_progress=None,
     candidate_progress=None,
     error_score=np.nan,
     ):
     """Fit estimator and compute scores for a given dataset split."""
     
     # fit_params内のデータをvalidation_fractionに合わせて整形 (validation_fraction='')
-    stratify = y if is_classifier(estimator) else None
     fit_params_modified, train_divided = _eval_set_selection(
         validation_fraction, 
         transformer, 
         X, 
         y,
         fit_params, 
         train, 
         test,
-        estimator.random_state,
-        stratify
+        estimator.steps[-1][1].random_state if isinstance(estimator, Pipeline) else estimator.random_state
         )
 
     # 学習してスコア計算
     result = _fit_and_score(estimator, X, y, scorer, train_divided, test, verbose, parameters,
                             fit_params_modified,
                             return_train_score=return_train_score,
                             return_parameters=return_parameters, return_n_test_samples=return_n_test_samples,
@@ -152,15 +149,15 @@
     X : array-like of shape (n_samples, n_features)
         The data to fit. Can be for example a list, or an array.
 
     y : array-like of shape (n_samples,) or (n_samples, n_outputs), default=None
         The target variable to try to predict in the case of
         supervised learning.
 
-    validation_fraction : {float, 'cv', 'transformed', or None}
+    validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
         Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
         If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
         
         If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
         If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
```

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/_cv_eval_set_old.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/_cv_eval_set_old.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_class_plot.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_class_plot.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import numbers
 import numpy as np
 import pandas as pd
 from scipy import stats
 from sklearn.metrics import auc, roc_curve, RocCurveDisplay
 from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
 from sklearn.preprocessing import label_binarize
+from sklearn.pipeline import Pipeline
+from sklearn.base import is_classifier
 from matplotlib import colors
 import copy
 import decimal
 
 from .multiclass_fitparams import OneVsRestClassifierPatched
-from ._cv_eval_set_old import init_eval_set, _make_transformer, _eval_set_selection
+from ._cv_eval_set import _make_transformer, _eval_set_selection
 
 class classplot():
     # 散布図カラーリスト
     _SCATTER_COLORS = ['green', 'red', 'mediumblue', 'brown', 'darkmagenta', 'darkorange', 'gold', 'grey']
     # クラス確率図カラーマップ
     _PROB_CMAP = ['Greens', 'Reds', 'Blues', 'YlOrBr', 'Purples', 'OrRd', 'Wistia', 'Greys']
     # デフォルトでの決定境界図の透明度(alpha)
@@ -415,15 +417,15 @@
     @classmethod
     def class_separator_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
                              x_colnames: List[str] = None, x_chart: List[str] = None,
                              pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
                              plot_scatter = 'class_error', rounddigit_x3 = 2,
                              scatter_colors = None, true_marker = 'o', false_marker = 'x',
                              cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                             clf_params=None, fit_params=None, eval_set_selection=None,
+                             clf_params=None, fit_params=None, validation_fraction=None,
                              subplot_kws=None, contourf_kws=None, scatter_kws=None, legend_kws=None):
         """
         Plot class separation lines of any scikit-learn classifier with 2 to 4D explanatory variables.
 
         Parameters
         ----------
         clf: classifier object implementing ``fit``
@@ -485,26 +487,24 @@
 
         clf_params: dict, optional
             Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params: dict, optional
             Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
         
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         subplot_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize.`` See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
         contourf_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.contourf(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html
 
@@ -606,20 +606,18 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
+            transformer = _make_transformer(validation_fraction, clf)
 
             # クロスバリデーション
             for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
                 # 表示対象以外のCVなら飛ばす
                 if i not in display_cv_indices:
                     continue
                 print(f'cv_number={i}/{cv_num}')
@@ -631,19 +629,27 @@
                 # 表示用にテストデータと学習データ分割
                 X_train = X[train]
                 y_train = y_true[train]
                 X_test = X[test]
                 y_test = y_true[test]
 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    clf.steps[-1][1].random_state if isinstance(clf, Pipeline) else clf.random_state
+                    )
 
                 # 学習と推論
-                clf.fit(X_train, y_train, **fit_params_modified)
+                clf.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 y_pred = clf.predict(X_test)
                 # 決定境界図をプロット
                 cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
                                    pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
                                    proba_pred = None, proba_class_indices = None, plot_border = True, plot_scatter = plot_scatter,
                                    scatter_color_dict=scatter_color_dict, scatter_marker_dict=scatter_marker_dict, proba_cmap_dict=None, proba_type=None,
                                    rounddigit_x3=rounddigit_x3, cv_index=cv_index,
@@ -653,15 +659,15 @@
     def class_proba_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
                          x_colnames: List[str] = None, x_chart: List[str] = None,
                          pair_sigmarange = 1.0, pair_sigmainterval = 0.5, chart_extendsigma = 0.5, chart_scale = 1,
                          plot_border = True, plot_scatter = 'class', rounddigit_x3 = 2,
                          proba_class = None, proba_cmap_dict = None, proba_type = 'contourf',
                          scatter_colors = None, true_marker = 'o', false_marker = 'x',
                          cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                         clf_params=None, fit_params=None, eval_set_selection=None,
+                         clf_params=None, fit_params=None, validation_fraction=None,
                          subplot_kws=None, contourf_kws=None, imshow_kws=None, scatter_kws=None, legend_kws=None):
         """
         Plot class prediction probability of any scikit-learn classifier with 2 to 4D explanatory variables.
 
         Parameters
         ----------
         clf: classifier object implementing ``fit``
@@ -735,26 +741,24 @@
 
         clf_params: dict, optional
             Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params: dict, optional
             Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         subplot_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
         contourf_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.contourf() if proba_type is set to 'contourf', or additional parameters passed to matplotlib.pyplot.contour() if proba_type is set to 'contour'. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contourf.html or https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.contour.html
 
@@ -893,20 +897,18 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
+            transformer = _make_transformer(validation_fraction, clf)
 
             # クロスバリデーション
             for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
                 # 表示対象以外のCVなら飛ばす
                 if i not in display_cv_indices:
                     continue
                 print(f'cv_number={i}/{cv_num}')
@@ -927,19 +929,27 @@
                 if len(proba_class_indices) == 0:
                     print(f'there is no assigned "proba_class" in the train data')
                     continue
                 # proba_cmap_dictも学習データから再取得
                 proba_cmap_dict = {k: v for k, v in proba_cmap_dict.items() if k in class_list_train}
 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    clf.steps[-1][1].random_state if isinstance(clf, Pipeline) else clf.random_state
+                    )
 
                 # 学習と推論
-                clf.fit(X_train, y_train, **fit_params_modified)
+                clf.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 y_pred = clf.predict(X_test)
                 # クラス確率を推定
                 proba_pred = clf.predict_proba(X_test)[:, proba_class_indices]
                 # クラス確率図をプロット
                 cls._class_chart_plot(clf, X_test, y_pred, y_test, x_chart, x_not_chart, x_chart_indices,
                                     pair_sigmarange = pair_sigmarange, pair_sigmainterval = pair_sigmainterval, chart_extendsigma=chart_extendsigma, chart_scale=chart_scale,
                                     proba_pred = proba_pred, proba_class_indices = proba_class_indices, plot_border = plot_border, plot_scatter = plot_scatter,
@@ -1157,15 +1167,15 @@
     @classmethod
     def roc_plot(cls, clf, x: List[str], y: str, data: pd.DataFrame = None,
                  x_colnames: List[str] = None, 
                  cv=None, cv_seed=42, cv_group=None,
                  ax=None,
                  sample_weight=None, drop_intermediate=True,
                  response_method="predict_proba", pos_label=None, average='macro',
-                 clf_params=None, fit_params=None, eval_set_selection=None,
+                 clf_params=None, fit_params=None, validation_fraction=None,
                  draw_grid=True, grid_kws=None, subplot_kws=None, legend_kws=None,
                  plot_roc_kws=None, class_average_kws=None, cv_mean_kws=None, chance_plot_kws=None):
         """Plot Receiver operating characteristic (ROC) curve with cross validation.
 
         Available both binary and multiclass classifiction.
 
         Extra keyword arguments will be passed to matplotlib's ``plot``.
@@ -1221,26 +1231,24 @@
 
         clf_params: dict, default=None
             Parameters passed to the classifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params : dict, default=None
             Parameters passed to the fit() method of the classifier, e.g. ``early_stopping_round`` and ``eval_set`` of XGBClassifier. If the classifier is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
         
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "train", select train data from `X` and `y` using cv.split().
-
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         draw_grid: bool, default=True
             If True, grid lines are drawn.
 
         grid_kws: dict, default=None
             Additional parameters passed to matplotlib.pyplot.grid() that draws grid lines, e.g. ``color``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.grid.html
 
@@ -1334,20 +1342,18 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'test'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, clf)
+            transformer = _make_transformer(validation_fraction, clf)
 
             # 表示用のax作成
             if ax is None:
                 if 'figsize' not in subplot_kws.keys():
                     subplot_kws['figsize'] = (6, (cv_num + 1) * 6)
                 fig, ax = plt.subplots(cv_num + 1, 1, **subplot_kws)
 
@@ -1370,19 +1376,27 @@
                 if 'lw' not in class_average_kws.keys():
                     class_average_kws['lw'] = 2
                 if 'linestyle' not in class_average_kws.keys():
                     class_average_kws['linestyle'] = ':'
                 class_average_kws['color'] = color_list[i]
 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    clf.steps[-1][1].random_state if isinstance(clf, Pipeline) else clf.random_state
+                    )
                 
                 # CVごとのROC曲線をプロット
-                viz = cls.plot_roc_curve_multiclass(clf, X[train], y_true[train], 
+                viz = cls.plot_roc_curve_multiclass(clf, X[train_divided], y_true[train_divided], 
                                                     X_test=X[test], y_test=y_true[test],
                                                     sample_weight=sample_weight, drop_intermediate=drop_intermediate,
                                                     response_method=response_method,
                                                     name=name, ax=ax[i],
                                                     pos_label=pos_label, average=average, fit_params=fit_params_modified,
                                                     plot_roc_kws=plot_roc_kws,
                                                     class_average_kws=class_average_kws
```

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_hist_plot.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_hist_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_pair_plot.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_pair_plot.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/custom_reg_plot.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/custom_reg_plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import numbers
 import numpy as np
 import pandas as pd
 from scipy import stats
 from sklearn.linear_model import LinearRegression
 from sklearn.metrics import r2_score, mean_absolute_error, mean_squared_error, mean_squared_log_error, mean_absolute_percentage_error
 from sklearn.model_selection import KFold, LeaveOneOut, GroupKFold, LeaveOneGroupOut
+from sklearn.pipeline import Pipeline
+from sklearn.base import is_classifier
 import decimal
 
-from ._cv_eval_set_old import init_eval_set, _make_transformer, _eval_set_selection, cross_val_score_eval_set
+from ._cv_eval_set import _make_transformer, _eval_set_selection, cross_val_score_eval_set
 
 class regplot():
     # regression_heat_plotメソッド (回帰モデルヒートマップ表示)における、散布図カラーマップ
     _HEAT_SCATTER_HUECOLORS = ['red', 'mediumblue', 'darkorange', 'darkmagenta', 'cyan',  'pink', 'brown', 'gold', 'grey']
 
     def _round_digits(src: float, rounddigit: int = None, method='decimal'):
         """
@@ -245,15 +247,15 @@
         ax.text(true_max, np.amin(y_pred), score_text, verticalalignment='bottom', horizontalalignment='right')
     
     @classmethod
     def regression_pred_true(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
                              x_colnames: List[str] = None, hue=None, linecolor='red', rounddigit=3,
                              rank_number=None, rank_col=None, scores='mae', 
                              cv_stats='mean', cv=None, cv_seed=42, cv_group=None, ax=None,
-                             estimator_params=None, fit_params=None, eval_set_selection=None,
+                             estimator_params=None, fit_params=None, validation_fraction=None,
                              subplot_kws=None, scatter_kws=None, legend_kws=None):
 
         """
         Plot prediction vs. true scatter plots of any scikit-learn regression estimator
 
         Parameters
         ----------
@@ -307,26 +309,24 @@
 
         estimator_params : dict, optional
             Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params : dict, optional
             Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         subplot_kws : dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. figsize. Available only if ``axes`` is None. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
         scatter_kws: dict, optional
             Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
 
@@ -411,56 +411,54 @@
                 cv_num = len(set(data[cv_group_colname].values))
             elif isLeaveOneOut:
                 cv_num = 1
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
+            transformer = _make_transformer(validation_fraction, estimator)
 
             # スコア種類ごとにクロスバリデーションスコアの算出
             score_all_dict = {}
             for scoring in scores:
                 # cross_val_scoreでクロスバリデーション
                 if scoring == 'r2':
-                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    score_all_dict['r2'] = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='r2',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                 elif scoring == 'mae':
-                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_mae = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_absolute_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'mse':
-                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_mse = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_squared_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'rmse':
-                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_rmse = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_root_mean_squared_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'rmsle':
-                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                    neg_msle = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_squared_log_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
                 elif scoring == 'mape':
-                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_mape = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_absolute_percentage_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'max_error':
-                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_max_error = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='max_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
             
             # 表示用のax作成
             if ax is None:
                 # LeaveOneOutのとき、クロスバリデーションごとの図は作成せず
@@ -499,23 +497,31 @@
                         rank_col_test = data.index.values[test]
                     else:  # 表示フィールド指定あるとき
                         rank_col_test = data[rank_col].values[test]
                 else:
                     rank_col_test = np.array([])
 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    estimator.steps[-1][1].random_state if isinstance(estimator, Pipeline) else estimator.random_state
+                    )
 
                 # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
+                estimator.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 y_pred = estimator.predict(X_test)
                 # 学習データスコア算出
-                y_pred_train = estimator.predict(X_train)
-                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
+                y_pred_train = estimator.predict(X[train_divided])
+                score_dict = cls._make_score_dict(y[train_divided], y_pred_train, scores)
                 for score in scores:
                     if f'{score}_train' not in score_train_dict:
                         score_train_dict[f'{score}_train'] = []
                     score_train_dict[f'{score}_train'].append(score_dict[score])
                 # CV内結果をプロット(LeaveOneOutのときはプロットしない)
                 if not isLeaveOneOut:
                     score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
@@ -604,15 +610,15 @@
 
 
     @classmethod
     def average_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
                      x_colnames: List[str] = None, hue=None,
                      aggregate='mean',
                      cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                     estimator_params=None, fit_params=None, eval_set_selection=None,
+                     estimator_params=None, fit_params=None, validation_fraction=None,
                      subplot_kws=None, plot_kws=None, scatter_kws=None, legend_kws=None):
         """
         Plot relationship between one explanatory variable and predicted value by line graph.
 
         Other explanatory variables are fixed to aggregated values such as mean values or median values.
 
         Parameters
@@ -651,26 +657,24 @@
 
         estimator_params : dict, optional
             Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params : dict, optional
             Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
         
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if `estimator` is LightGBM or XGBoost and `cv` is not None.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         subplot_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
         plot_kws: dict, optional
             Additional parameters passed to matplotlib.axes.Axes.plot(), e.g. ``alpha``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.plot.html
 
@@ -739,38 +743,44 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
+            transformer = _make_transformer(validation_fraction, estimator)
 
             # クロスバリデーション
             for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
                 # 表示対象以外のCVなら飛ばす
                 if i not in display_cv_indices:
                     continue
                 print(f'cv_number={i}/{cv_num}')
                 # 表示用にテストデータと学習データ分割
                 X_train = X[train]
                 y_train = y_true[train]
                 data_test = data.iloc[test]
                 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    estimator.steps[-1][1].random_state if isinstance(estimator, Pipeline) else estimator.random_state
+                    )
 
                 # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
+                estimator.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 # ヒートマップをプロット
                 cls._average_plot(estimator, data_test, x_colnames, y_colname, hue,
                                   aggregate=aggregate,
                                   subplot_kws=subplot_kws, plot_kws=plot_kws,
                                   scatter_kws=scatter_kws, legend_kws=legend_kws,
                                   cv_index=i)
 
@@ -947,15 +957,15 @@
         ax.text(xmax, np.amin(y_true), score_text, verticalalignment='bottom', horizontalalignment='right')
 
     @classmethod
     def regression_plot_1d(cls, estimator, x: str, y: str, data: pd.DataFrame = None, x_colname: str = None,
                            hue=None, linecolor='red', rounddigit=3,
                            rank_number=None, rank_col=None, scores='mae',
                            cv_stats='mean', cv=None, cv_seed=42, cv_group=None,
-                           estimator_params=None, fit_params=None, eval_set_selection=None,
+                           estimator_params=None, fit_params=None, validation_fraction=None,
                            subplot_kws=None, scatter_kws=None, legend_kws=None):
         """
         Plot regression lines of any scikit-learn regressor with 1D explanatory variable.
 
         Parameters
         ----------
         estimator : estimator object implementing ``fit``
@@ -1008,26 +1018,24 @@
 
         fit_params : dict, optional
             Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         subplot_kws : dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         scatter_kws: dict, optional
             Additional parameters passed to sns.scatterplot(), e.g. ``alpha``. See https://seaborn.pydata.org/generated/seaborn.scatterplot.html
 
         legend_kws : dict
             Additional parameters passed to ax.legend(), e.g. ``loc``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.legend.html
 
@@ -1108,56 +1116,54 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
+            transformer = _make_transformer(validation_fraction, estimator)
 
             # スコア種類ごとにクロスバリデーションスコアの算出
             score_all_dict = {}
             for scoring in scores:
                 # cross_val_scoreでクロスバリデーション
                 if scoring == 'r2':
-                    score_all_dict['r2'] = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                    score_all_dict['r2'] = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='r2',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                 elif scoring == 'mae':
-                    neg_mae = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true, 
+                    neg_mae = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_absolute_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mae'] = -neg_mae  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'mse':
-                    neg_mse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_mse = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_squared_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mse'] = -neg_mse  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'rmse':
-                    neg_rmse = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_rmse = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_root_mean_squared_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['rmse'] = -neg_rmse  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'rmsle':
-                    neg_msle = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_msle = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_squared_log_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['rmsle'] = np.sqrt(-neg_msle)  # 正負を逆にしてルートをとる
                 elif scoring == 'mape':
-                    neg_mape = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_mape = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='neg_mean_absolute_percentage_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['mape'] = -neg_mape  # scikit-learnの仕様に合わせ正負を逆に
                 elif scoring == 'max_error':
-                    neg_max_error = cross_val_score_eval_set(eval_set_selection, estimator, X, y_true,
+                    neg_max_error = cross_val_score_eval_set(estimator, X, y_true, validation_fraction,
                                                     cv=cv, scoring='max_error',
                                                     fit_params=fit_params, n_jobs=-1, **split_kws)
                     score_all_dict['max_error'] = - neg_max_error  # scikit-learnの仕様に合わせ正負を逆に
             
             # 表示用のaxes作成
             # クロスバリデーションごとに図作成
             if 'figsize' not in subplot_kws.keys():
@@ -1183,22 +1189,30 @@
                 if rank_number is not None:
                     if rank_col is None:  # 表示フィールド指定ないとき、Index使用
                         rank_col_test = data.index.values[test]
                     else:  # 表示フィールド指定あるとき
                         rank_col_test = data[rank_col].values[test]
                 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    estimator.steps[-1][1].random_state if isinstance(estimator, Pipeline) else estimator.random_state
+                    )
 
                 # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
+                estimator.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 # 学習データスコア算出
-                y_pred_train = estimator.predict(X_train)
-                score_dict = cls._make_score_dict(y_train, y_pred_train, scores)
+                y_pred_train = estimator.predict(X[train_divided])
+                score_dict = cls._make_score_dict(y[train_divided], y_pred_train, scores)
                 for score in scores:
                     if f'{score}_train' not in score_train_dict:
                         score_train_dict[f'{score}_train'] = []
                     score_train_dict[f'{score}_train'].append(score_dict[score])
                 # CV内結果をプロット
                 score_cv_dict = {k: v[i] for k, v in score_all_dict.items()}
                 score_cv_dict.update({f'{k}_train': v for k, v in score_dict.items()})
@@ -1495,15 +1509,15 @@
     def regression_heat_plot(cls, estimator, x: List[str], y: str, data: pd.DataFrame = None,
                              x_colnames: List[str] = None, x_heat: List[str] = None, scatter_hue=None,
                              pair_sigmarange = 1.0, pair_sigmainterval = 0.5, heat_extendsigma = 0.5, 
                              heat_division = 30, color_extendsigma = 0.5,
                              plot_scatter = 'true', rounddigit_rank=3, rounddigit_x1=2, rounddigit_x2=2, rounddigit_x3=2,
                              rank_number=None, rank_col=None,
                              cv=None, cv_seed=42, cv_group=None, display_cv_indices = 0,
-                             estimator_params=None, fit_params=None, eval_set_selection=None,
+                             estimator_params=None, fit_params=None, validation_fraction=None,
                              subplot_kws=None, heat_kws=None, scatter_kws=None, legend_kws=None):
         """
         Plot regression heatmaps of any scikit-learn regressor with 2 to 4D explanatory variables.
 
         Parameters
         ----------
         estimator : estimator object implementing ``fit``
@@ -1577,26 +1591,24 @@
 
         estimator_params : dict, optional
             Parameters passed to the regression estimator. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
         fit_params : dict, optional
             Parameters passed to the fit() method of the regression estimator, e.g. ``early_stopping_round`` and ``eval_set`` of XGBRegressor. If the estimator is pipeline, each parameter name must be prefixed such that parameter p for step s has key s__p.
 
-        eval_set_selection: {'all', 'test', 'train', 'original', 'original_transformed'}, optional
-            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LightGBM or XGBoost.
-            
-            If "all", use all data in `X` and `y`.
-
-            If "train", select train data from `X` and `y` using cv.split().
+        validation_fraction : {float, 'cv', 'transformed', or None}, default='cv'
+            Select data passed to `eval_set` in `fit_params`. Available only if "estimator" is LGBMRegressor, LGBMClassifier, XGBRegressor, or XGBClassifier.
 
-            If "test", select test data from `X` and `y` using cv.split().
+            If float, devide source training data into training data and eval_set according to the specified ratio like sklearn.ensemble.GradientBoostingRegressor.
+            
+            If "cv", select test data from `X` and `y` using cv.split() like lightgbm.cv.
 
-            If "original", use raw `eval_set`.
+            If "transformed", use `eval_set` transformed by `fit_transform()` of the pipeline if the `estimater` is sklearn.pipeline.Pipeline object.
 
-            If "original_transformed", use `eval_set` transformed by fit_transform() of pipeline if `estimater` is pipeline.
+            If None, use raw `eval_set`.
 
         subplot_kws: dict, optional
             Additional parameters passed to matplotlib.pyplot.subplots(), e.g. ``figsize``. See https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html
 
         heat_kws: dict, optional
             Additional parameters passed to sns.heatmap(), e.g. ``cmap``. See https://seaborn.pydata.org/generated/seaborn.heatmap.html
 
@@ -1714,39 +1726,45 @@
             # LeaveOneGroupOutのとき、クロスバリデーション分割数をcv_groupの数に指定
             if isinstance(cv, LeaveOneGroupOut):
                 cv_num = len(set(data[cv_group_colname].values))
             else:
                 cv_num = cv.n_splits
 
             # fit_paramsにeval_metricが入力されており、eval_setが入力されていないときの処理(eval_setにテストデータを使用)
-            if eval_set_selection is None:
-                eval_set_selection = 'test'
-            fit_params, eval_set_selection = init_eval_set(
-                    eval_set_selection, fit_params, X, y)
+            if validation_fraction is None:
+                validation_fraction = 'cv'
             # 最終学習器以外の前処理変換器作成
-            transformer = _make_transformer(eval_set_selection, estimator)
+            transformer = _make_transformer(validation_fraction, estimator)
 
             # クロスバリデーション
             for i, (train, test) in enumerate(cv.split(X, y_true, **split_kws)):
                 # 表示対象以外のCVなら飛ばす
                 if i not in display_cv_indices:
                     continue
                 print(f'cv_number={i}/{cv_num}')
                 # 表示用にテストデータと学習データ分割
                 X_train = X[train]
                 y_train = y_true[train]
                 X_test = X[test]
                 y_test = y_true[test]
 
                 # eval_setの中から学習データ or テストデータのみを抽出
-                fit_params_modified = _eval_set_selection(eval_set_selection, transformer,
-                                                        fit_params, train, test)
+                fit_params_modified, train_divided = _eval_set_selection(
+                    validation_fraction, 
+                    transformer, 
+                    X,
+                    y,
+                    fit_params, 
+                    train, 
+                    test,
+                    estimator.steps[-1][1].random_state if isinstance(estimator, Pipeline) else estimator.random_state
+                    )
 
                 # 学習と推論
-                estimator.fit(X_train, y_train, **fit_params_modified)
+                estimator.fit(X[train_divided], y[train_divided], **fit_params_modified)
                 y_pred = estimator.predict(X_test)
                 # 誤差上位表示用データ取得
                 if rank_number is not None:
                     if rank_col is None:  # 表示フィールド指定ないとき、Index使用
                         rank_col_test = data.index.values[test]
                     else:  # 表示フィールド指定あるとき
                         rank_col_test = data[rank_col].values[test]
```

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer/multiclass_fitparams.py` & `seaborn-analyzer-0.3.3/seaborn_analyzer/multiclass_fitparams.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/seaborn_analyzer.egg-info/PKG-INFO` & `seaborn-analyzer-0.3.3/seaborn_analyzer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaborn-analyzer
-Version: 0.3.2
+Version: 0.3.3
 Summary: seaborn-analyzer: data visualization of regression, classification and distribution
 Home-page: https://github.com/c60evaporator/seaborn-analyzer
 Download-URL: https://github.com/c60evaporator/seaborn-analyzer
 Author: Kenta Nakamura
 Author-email: c60evaporator@gmail.com
 Maintainer: Kenta Nakamura
 Maintainer-email: c60evaporator@gmail.com
@@ -65,15 +65,15 @@
 If you want to know the usage of the other classes, see `API Reference
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#api-reference>`__ and `Examples
 <https://github.com/c60evaporator/seaborn-analyzer/blob/master/README.rst#examples>`__
 
 ============
 Requirements
 ============
-seaborn-analyzer 0.3.2 requires
+seaborn-analyzer 0.3.3 requires
 
 * Python >=3.6
 * Numpy >=1.20.3
 * Pandas >=1.2.4
 * Matplotlib >=3.1.3
 * Seaborn >=0.11.1
 * Scipy >=1.6.3
```

### Comparing `seaborn-analyzer-0.3.2/setup.py` & `seaborn-analyzer-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `seaborn-analyzer-0.3.2/tests/test_cv.py` & `seaborn-analyzer-0.3.3/tests/test_cv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 import seaborn as sns
 import numpy as np
 import pandas as pd
 from sklearn.datasets import fetch_california_housing
 from sklearn.model_selection import KFold
-import lightgbm as lgb
+from lightgbm import LGBMClassifier, LGBMRegressor
 
 import os
 import sys
 ROOT = os.path.dirname(os.path.dirname(__file__))
 sys.path.append(ROOT)
 from seaborn_analyzer._cv_eval_set import cross_val_score_eval_set
 
@@ -30,15 +30,15 @@
         'n_estimators': 10000,
         'verbose': -1,
         'early_stopping_round': 10
         }
     lgb_fit_params = {
         'eval_set':[(X, y)]
         }
-    lgbr = lgb.LGBMClassifier(**lgb_params)
+    lgbr = LGBMClassifier(**lgb_params)
 
     def test_cross_val_score_cls_lgbm(self):
         scores = cross_val_score_eval_set(
             validation_fraction='test',
             estimator=self.lgbr,
             X=self.X, y=self.y,  # Data before cross validation division
             scoring='neg_log_loss',  # Negative LogLoss
@@ -68,15 +68,15 @@
         'n_estimators': 10000,
         'verbose': -1,
         'early_stopping_round': 10
         }
     lgb_fit_params = {
         'eval_set':[(X, y)]
         }
-    lgbr = lgb.LGBMRegressor(**lgb_params)
+    lgbr = LGBMRegressor(**lgb_params)
 
     def test_cross_val_score_reg_lgbm_float(self):
         scores = cross_val_score_eval_set(
             validation_fraction=0.3,
             estimator=self.lgbr,
             X=self.X, y=self.y,  # Data before cross validation division
             scoring='neg_root_mean_squared_error',  # Negative RMSE
```

