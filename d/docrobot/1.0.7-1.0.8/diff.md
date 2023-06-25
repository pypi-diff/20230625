# Comparing `tmp/docrobot-1.0.7.tar.gz` & `tmp/docrobot-1.0.8.tar.gz`

## Comparing `docrobot-1.0.7.tar` & `docrobot-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.7/convert.ps1
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.7/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.7/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/__init__.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/form.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/form.ui
--rw-r--r--   0        0        0    21618 2020-02-02 00:00:00.000000 docrobot-1.0.7/src/docrobot/guimain.pyw
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.7/LICENSE
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.0.7/README.md
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.7/pyproject.toml
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 docrobot-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 docrobot-1.0.8/convert.ps1
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 docrobot-1.0.8/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 docrobot-1.0.8/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/__init__.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/form.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/form.ui
+-rw-r--r--   0        0        0    21677 2020-02-02 00:00:00.000000 docrobot-1.0.8/src/docrobot/guimain.pyw
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 docrobot-1.0.8/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 docrobot-1.0.8/LICENSE
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 docrobot-1.0.8/README.md
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 docrobot-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 docrobot-1.0.8/PKG-INFO
```

### Comparing `docrobot-1.0.7/.github/workflows/python-publish.yml` & `docrobot-1.0.8/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.7/src/docrobot/form.py` & `docrobot-1.0.8/src/docrobot/form.py`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.7/src/docrobot/form.ui` & `docrobot-1.0.8/src/docrobot/form.ui`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.7/src/docrobot/guimain.pyw` & `docrobot-1.0.8/src/docrobot/guimain.pyw`

 * *Files 1% similar despite different names*

```diff
@@ -176,16 +176,17 @@
                     changed |= True
                     unmatch = unmatch + 1
                 else:
                     match = match + 1
 
             # 检查和替换项目人数
             rnd_name = str(r[8].value).strip()
-            if not rnd_name.endswith('等'):
+            if rnd_name != '' and not rnd_name.endswith('等'):
                 real_num = len(rnd_name.split('、'))
+                real_num = real_num + 1
                 if real_num != int(r[6].value):
                     self.textEdit.append(self.arr_prj[i].p_order + ' 项目: ' + '研发人员名字数量不匹配:' + rnd_name)
                     self.textEdit.append('研发人数: ' + str(r[6].value) + ' ===> ' + str(real_num))
                     r[6].value = real_num
                     changed |= True
                     unmatch = unmatch + 1
                 else:
```

### Comparing `docrobot-1.0.7/LICENSE` & `docrobot-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `docrobot-1.0.7/pyproject.toml` & `docrobot-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "docrobot"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="Xu Hong", email="icehong@gmail.com" },
 ]
 description = "一个文档自动化处理工具"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `docrobot-1.0.7/PKG-INFO` & `docrobot-1.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docrobot
-Version: 1.0.7
+Version: 1.0.8
 Summary: 一个文档自动化处理工具
 Project-URL: Homepage, https://github.com/icehong/docrobot
 Project-URL: Bug Tracker, https://github.com/icehong/docrobot/issues
 Author-email: Xu Hong <icehong@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

