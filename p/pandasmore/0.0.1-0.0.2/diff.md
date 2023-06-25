# Comparing `tmp/pandasmore-0.0.1.tar.gz` & `tmp/pandasmore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasmore-0.0.1.tar", last modified: Sun Jun 25 12:28:22 2023, max compression
+gzip compressed data, was "pandasmore-0.0.2.tar", last modified: Sun Jun 25 13:05:24 2023, max compression
```

## Comparing `pandasmore-0.0.1.tar` & `pandasmore-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.284997 pandasmore-0.0.1/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.280999 pandasmore-0.0.1/.github/
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.280999 pandasmore-0.0.1/.github/workflows/
--rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.1/.github/workflows/deploy.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-04-27 10:12:58.000000 pandasmore-0.0.1/.gitignore
--rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.1/LICENSE
--rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.1/MANIFEST.in
--rw-rw-r--   0 imb       (1000) imb       (1000)     3113 2023-06-25 12:28:22.284997 pandasmore-0.0.1/PKG-INFO
--rw-rw-r--   0 imb       (1000) imb       (1000)     2292 2023-06-24 18:52:42.000000 pandasmore-0.0.1/README.md
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.284997 pandasmore-0.0.1/nbs/
--rw-r--r--   0 imb       (1000) imb       (1000)    62177 2023-06-25 12:25:24.000000 pandasmore-0.0.1/nbs/00_core.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.1/nbs/_quarto.yml
--rw-r--r--   0 imb       (1000) imb       (1000)     6968 2023-06-24 18:52:26.000000 pandasmore-0.0.1/nbs/index.ipynb
--rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-06-24 21:58:12.000000 pandasmore-0.0.1/nbs/nbdev.yml
--rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.1/nbs/sidebar.yml
--rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.1/nbs/styles.css
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.284997 pandasmore-0.0.1/pandasmore/
--rw-r--r--   0 imb       (1000) imb       (1000)       22 2023-06-24 21:58:11.000000 pandasmore-0.0.1/pandasmore/__init__.py
--rw-rw-r--   0 imb       (1000) imb       (1000)     1576 2023-06-24 21:58:11.000000 pandasmore-0.0.1/pandasmore/_modidx.py
--rw-r--r--   0 imb       (1000) imb       (1000)    12535 2023-06-24 21:58:11.000000 pandasmore-0.0.1/pandasmore/core.py
-drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 12:28:22.284997 pandasmore-0.0.1/pandasmore.egg-info/
--rw-r--r--   0 imb       (1000) imb       (1000)     3113 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/PKG-INFO
--rw-r--r--   0 imb       (1000) imb       (1000)      518 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/SOURCES.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/dependency_links.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/entry_points.txt
--rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.1/pandasmore.egg-info/not-zip-safe
--rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/requires.txt
--rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-06-25 12:28:22.000000 pandasmore-0.0.1/pandasmore.egg-info/top_level.txt
--rw-r--r--   0 imb       (1000) imb       (1000)     1025 2023-06-23 19:24:51.000000 pandasmore-0.0.1/settings.ini
--rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-25 12:28:22.284997 pandasmore-0.0.1/setup.cfg
--rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.1/setup.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:23.996715 pandasmore-0.0.2/.github/
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/.github/workflows/
+-rw-r--r--   0 imb       (1000) imb       (1000)      242 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.github/workflows/deploy.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)      148 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0 imb       (1000) imb       (1000)     1608 2023-04-27 10:12:58.000000 pandasmore-0.0.2/.gitignore
+-rw-r--r--   0 imb       (1000) imb       (1000)    11337 2023-04-27 10:12:58.000000 pandasmore-0.0.2/LICENSE
+-rw-r--r--   0 imb       (1000) imb       (1000)      111 2023-04-27 10:12:58.000000 pandasmore-0.0.2/MANIFEST.in
+-rw-rw-r--   0 imb       (1000) imb       (1000)     4772 2023-06-25 13:05:24.000715 pandasmore-0.0.2/PKG-INFO
+-rw-rw-r--   0 imb       (1000) imb       (1000)     3951 2023-06-25 12:55:28.000000 pandasmore-0.0.2/README.md
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/nbs/
+-rw-r--r--   0 imb       (1000) imb       (1000)    61779 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/00_core.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      345 2023-06-23 19:18:59.000000 pandasmore-0.0.2/nbs/_quarto.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)    14674 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/index.ipynb
+-rw-r--r--   0 imb       (1000) imb       (1000)      279 2023-06-25 12:55:13.000000 pandasmore-0.0.2/nbs/nbdev.yml
+-rw-rw-r--   0 imb       (1000) imb       (1000)       76 2023-06-24 20:54:34.000000 pandasmore-0.0.2/nbs/sidebar.yml
+-rw-r--r--   0 imb       (1000) imb       (1000)      600 2023-04-27 10:12:58.000000 pandasmore-0.0.2/nbs/styles.css
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/pandasmore/
+-rw-r--r--   0 imb       (1000) imb       (1000)       41 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/__init__.py
+-rw-rw-r--   0 imb       (1000) imb       (1000)     1576 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/_modidx.py
+-rw-r--r--   0 imb       (1000) imb       (1000)    12540 2023-06-25 12:55:13.000000 pandasmore-0.0.2/pandasmore/core.py
+drwxrwxr-x   0 imb       (1000) imb       (1000)        0 2023-06-25 13:05:24.000715 pandasmore-0.0.2/pandasmore.egg-info/
+-rw-r--r--   0 imb       (1000) imb       (1000)     4772 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/PKG-INFO
+-rw-r--r--   0 imb       (1000) imb       (1000)      518 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/SOURCES.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/dependency_links.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       42 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/entry_points.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)        1 2023-06-23 19:24:31.000000 pandasmore-0.0.2/pandasmore.egg-info/not-zip-safe
+-rw-r--r--   0 imb       (1000) imb       (1000)       23 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/requires.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)       11 2023-06-25 13:05:23.000000 pandasmore-0.0.2/pandasmore.egg-info/top_level.txt
+-rw-r--r--   0 imb       (1000) imb       (1000)      898 2023-06-25 12:55:00.000000 pandasmore-0.0.2/settings.ini
+-rw-rw-r--   0 imb       (1000) imb       (1000)       38 2023-06-25 13:05:24.000715 pandasmore-0.0.2/setup.cfg
+-rw-r--r--   0 imb       (1000) imb       (1000)     2596 2023-04-27 10:12:58.000000 pandasmore-0.0.2/setup.py
```

### Comparing `pandasmore-0.0.1/.gitignore` & `pandasmore-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.1/LICENSE` & `pandasmore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.1/nbs/00_core.ipynb` & `pandasmore-0.0.2/nbs/00_core.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9296440972222222%*

 * *Differences: {"'cells'": "{8: {'source': {insert: [(3, '    \\n')]}}, delete: [46, 45, 43]}",*

 * * "'metadata'": "{delete: ['language_info']}"}*

```diff
@@ -247,14 +247,15 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "#|export\n",
                 "def order_columns(df: pd.DataFrame, these_first: List[str]) -> pd.DataFrame:\n",
                 "    \"\"\"Returns `df` with reordered columns. Use as `df = order_columns(df,_)`\"\"\"\n",
+                "    \n",
                 "    remaining = [x for x in df.columns if x not in these_first]\n",
                 "    return df[these_first + remaining]"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -1874,21 +1875,14 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
                 "#|export\n",
                 "def norm(df: pd.Series|pd.DataFrame, \n",
                 "         divide_by_mean = False\n",
                 "         ) -> pd.DataFrame:\n",
                 "    \"\"\"Subtract means from all columns of `df` and divide by their std. deviations, unless `divide_by_mean` is True\"\"\"\n",
                 "\n",
@@ -1900,41 +1894,23 @@
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
             "source": [
                 "#| hide\n",
                 "import nbdev; nbdev.nbdev_export()"
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "python3",
             "language": "python",
             "name": "python3"
-        },
-        "language_info": {
-            "name": "python",
-            "version": "3.9.16"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `pandasmore-0.0.1/nbs/styles.css` & `pandasmore-0.0.2/nbs/styles.css`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.1/pandasmore/_modidx.py` & `pandasmore-0.0.2/pandasmore/_modidx.py`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.1/pandasmore/core.py` & `pandasmore-0.0.2/pandasmore/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # %% auto 0
 __all__ = ['order_columns', 'process_dates', 'setup_tseries', 'setup_panel', 'fast_lag', 'lag', 'add_lags', 'rpct_change',
            'rdiff', 'rrolling', 'wins', 'norm']
 
 # %% ../nbs/00_core.ipynb 8
 def order_columns(df: pd.DataFrame, these_first: List[str]) -> pd.DataFrame:
     """Returns `df` with reordered columns. Use as `df = order_columns(df,_)`"""
+    
     remaining = [x for x in df.columns if x not in these_first]
     return df[these_first + remaining]
 
 # %% ../nbs/00_core.ipynb 10
 def process_dates(df: pd.DataFrame, # Function returns copy of this df with `dtdate_var` and `f'{freq}date'` cols added
                 time_var: str='date', # This will be the date variable used to generate datetime var `dtdate_var`
                 time_var_format: str='%Y-%m-%d', # Format of `time_var`; must be valid pandas `strftime`
@@ -218,15 +219,15 @@
         return (df.groupby(byvars)
                     .apply(lambda x: df[x].clip(df[x].quantile(low), df[x].quantile(high), axis=1))
                     .reset_index()
                     .set_index(df.index))
     else:
         return df.clip(df.quantile(low), df.quantile(high), axis=1).squeeze()
 
-# %% ../nbs/00_core.ipynb 44
+# %% ../nbs/00_core.ipynb 43
 def norm(df: pd.Series|pd.DataFrame, 
          divide_by_mean = False
          ) -> pd.DataFrame:
     """Subtract means from all columns of `df` and divide by their std. deviations, unless `divide_by_mean` is True"""
 
     if isinstance(df,pd.Series): df = df.to_frame()
     if divide_by_mean:
```

### Comparing `pandasmore-0.0.1/pandasmore.egg-info/SOURCES.txt` & `pandasmore-0.0.2/pandasmore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pandasmore-0.0.1/settings.ini` & `pandasmore-0.0.2/settings.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 [DEFAULT]
-# All sections below are required unless otherwise specified.
-# See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
-
-### Python library ###
 repo = pandasmore
-lib_name = %(repo)s
-version = 0.0.1
+lib_name = pandasmore
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
-
-### nbdev ###
 doc_path = _docs
 lib_path = pandasmore
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
-
-### Docs ###
 branch = main
 custom_sidebar = False
 custom_quarto_yml = True
-doc_host = https://%(user)s.github.io
-doc_baseurl = /%(repo)s
-git_url = https://github.com/%(user)s/%(repo)s
-title = %(lib_name)s
-
-### PyPI ###
+doc_host = https://ionmihai.github.io
+doc_baseurl = /pandasmore
+git_url = https://github.com/ionmihai/pandasmore
+title = pandasmore
 audience = Developers
 author = ionmihai
 author_email = mihaiion@email.arizona.edu
-copyright = 2023 onwards, %(author)s
+copyright = 2023 onwards, ionmihai
 description = Extends pandas with common functions used in finance and economics research
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = ionmihai
-
-### Optional ###
 requirements = fastcore pandas
-# dev_requirements = 
-# console_scripts =
+readme_nb = index.ipynb
+allowed_metadata_keys = 
+allowed_cell_metadata_keys = 
+jupyter_hooks = True
+clean_ids = True
+clear_all = False
+
```

### Comparing `pandasmore-0.0.1/setup.py` & `pandasmore-0.0.2/setup.py`

 * *Files identical despite different names*

