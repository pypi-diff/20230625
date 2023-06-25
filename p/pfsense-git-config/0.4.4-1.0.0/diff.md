# Comparing `tmp/pfsense_git_config-0.4.4.tar.gz` & `tmp/pfsense_git_config-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfsense_git_config-0.4.4.tar", max compression
+gzip compressed data, was "pfsense_git_config-1.0.0.tar", max compression
```

## Comparing `pfsense_git_config-0.4.4.tar` & `pfsense_git_config-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2607 2023-06-24 18:45:03.779583 pfsense_git_config-0.4.4/README.md
--rw-r--r--   0        0        0       90 2023-06-24 18:45:03.779583 pfsense_git_config-0.4.4/pfsense_git_config/__init__.py
--rw-r--r--   0        0        0     3999 2023-06-24 18:44:58.147073 pfsense_git_config-0.4.4/pfsense_git_config/git_repo.py
--rw-r--r--   0        0        0     4165 2023-06-24 18:44:58.147073 pfsense_git_config-0.4.4/pfsense_git_config/main.py
--rw-r--r--   0        0        0     1973 2023-06-24 18:44:58.147073 pfsense_git_config-0.4.4/pfsense_git_config/pfsense_configs.py
--rw-r--r--   0        0        0     1323 2023-06-24 18:45:03.791584 pfsense_git_config-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     3340 1970-01-01 00:00:00.000000 pfsense_git_config-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     2958 2023-06-25 13:02:02.384325 pfsense_git_config-1.0.0/README.md
+-rw-r--r--   0        0        0       90 2023-06-25 13:02:02.384325 pfsense_git_config-1.0.0/pfsense_git_config/__init__.py
+-rw-r--r--   0        0        0     3999 2023-06-25 13:01:57.880126 pfsense_git_config-1.0.0/pfsense_git_config/git_repo.py
+-rw-r--r--   0        0        0     4165 2023-06-25 13:01:57.880126 pfsense_git_config-1.0.0/pfsense_git_config/main.py
+-rw-r--r--   0        0        0     1973 2023-06-25 13:01:57.880126 pfsense_git_config-1.0.0/pfsense_git_config/pfsense_configs.py
+-rw-r--r--   0        0        0     1323 2023-06-25 13:02:02.396325 pfsense_git_config-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3691 1970-01-01 00:00:00.000000 pfsense_git_config-1.0.0/PKG-INFO
```

### Comparing `pfsense_git_config-0.4.4/README.md` & `pfsense_git_config-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # pfSense Git Config
 
 Import pfSense config changes into a git repo.
 
+This gives you a record of individual config updates, and allows you to browse
+the changes easily.
+
+> **_NOTE:_** Your pfSense config data is sensitive - it will contain hashed
+> passwords and information about the networks served by your firewall. I would
+> only keep this on a private git server and with access restrictions on the
+> repo as well.
+
 ## Current Version
 
-Version: `0.4.4`
+Version: `1.0.0`
 
 ## Usage
 
 Usage: `pfsense_git_config` [OPTIONS]
 
 Read pfSense configation changes, add them to a Git repo of config changes
```

### Comparing `pfsense_git_config-0.4.4/pfsense_git_config/git_repo.py` & `pfsense_git_config-1.0.0/pfsense_git_config/git_repo.py`

 * *Files identical despite different names*

### Comparing `pfsense_git_config-0.4.4/pfsense_git_config/main.py` & `pfsense_git_config-1.0.0/pfsense_git_config/main.py`

 * *Files identical despite different names*

### Comparing `pfsense_git_config-0.4.4/pfsense_git_config/pfsense_configs.py` & `pfsense_git_config-1.0.0/pfsense_git_config/pfsense_configs.py`

 * *Files identical despite different names*

### Comparing `pfsense_git_config-0.4.4/pyproject.toml` & `pfsense_git_config-1.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pfsense-git-config"
-version = "0.4.4"
+version = "1.0.0"
 description = "pfSense Git Config"
 authors = ["Nigel Metheringham <nigel.metheringham@gmail.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/pfsense-git-config/"
 repository = "https://github.com/nigelm/pfsense_git_config"
 packages = [{include = "pfsense_git_config"}]
```

### Comparing `pfsense_git_config-0.4.4/PKG-INFO` & `pfsense_git_config-1.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfsense-git-config
-Version: 0.4.4
+Version: 1.0.0
 Summary: pfSense Git Config
 Home-page: https://pypi.org/project/pfsense-git-config/
 Author: Nigel Metheringham
 Author-email: nigel.metheringham@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -18,17 +18,25 @@
 Project-URL: Repository, https://github.com/nigelm/pfsense_git_config
 Description-Content-Type: text/markdown
 
 # pfSense Git Config
 
 Import pfSense config changes into a git repo.
 
+This gives you a record of individual config updates, and allows you to browse
+the changes easily.
+
+> **_NOTE:_** Your pfSense config data is sensitive - it will contain hashed
+> passwords and information about the networks served by your firewall. I would
+> only keep this on a private git server and with access restrictions on the
+> repo as well.
+
 ## Current Version
 
-Version: `0.4.4`
+Version: `1.0.0`
 
 ## Usage
 
 Usage: `pfsense_git_config` [OPTIONS]
 
 Read pfSense configation changes, add them to a Git repo of config changes
```

