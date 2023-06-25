# Comparing `tmp/jupyter_pgadmin_proxy-0.0.1.tar.gz` & `tmp/jupyter_pgadmin_proxy-0.0.2.tar.gz`

## Comparing `jupyter_pgadmin_proxy-0.0.1.tar` & `jupyter_pgadmin_proxy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,9 @@
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/.dockerignore
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/docker-compose.yaml
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy/__init__.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy/pgadmin.svg
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy_test/__init__.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy_test/jupyter_config.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy_test/pgadmin.svg
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/LICENSE.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/README.md
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3102 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/.dockerignore
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/docker-compose.yaml
+-rw-r--r--   0        0        0     3293 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/jupyter_pgadmin_proxy/__init__.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/jupyter_pgadmin_proxy/pgadmin.svg
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/README.md
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3373 2020-02-02 00:00:00.000000 jupyter_pgadmin_proxy-0.0.2/PKG-INFO
```

### Comparing `jupyter_pgadmin_proxy-0.0.1/docker-compose.yaml` & `jupyter_pgadmin_proxy-0.0.2/docker-compose.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
       - 8888:8888
     environment:
       PGHOST: postgres
       PGPORT: 5432
       PGDATABASE: postgres
       PGUSER: postgres
       PGPASSWORD: postgres
+      # PGADMIN_ENABLED: 'false'
     volumes:
       - "${PWD}:/home/jovyan/jupyter-pgadmin-proxy"
   postgres:
     image: postgres:15.3-alpine
     hostname: postgres
     container_name: pgadmin-postgres
     restart: always
```

### Comparing `jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy/__init__.py` & `jupyter_pgadmin_proxy-0.0.2/jupyter_pgadmin_proxy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 import site
 
 logging.basicConfig(level="INFO")
 logger = logging.getLogger("pgAdmin4")
 logger.setLevel("INFO")
 
 
+TRUTHY = ("true", "1", "yes", "on", "y")
+
+
+def truthy(val):
+    return str(val).strip('"').strip("'").lower() in TRUTHY
+
+
 def _get_env(port, base_url):
     """
     Returns a dict containing environment settings to launch the Web App.
     Args:
         port (int): Port number on which the Web app will be started. Ex: 8888
         base_url (str): Controls the prefix in the url on which
                         the Web App will be available.
@@ -90,10 +97,11 @@
         "timeout": 300,
         "environment": _get_env,
         "absolute_url": True,
         # "rewrite_response": rewrite_netloc,
         # "request_headers_override": {"X-Script-Name": "{base_url}pgadmin"},
         "launcher_entry": {
             "title": "pgAdmin4",
-            "icon_path": icon_path
+            "icon_path": icon_path,
+            "enabled": truthy(os.getenv("PGADMIN_ENABLED", "true")),
         },
     }
```

### Comparing `jupyter_pgadmin_proxy-0.0.1/jupyter_pgadmin_proxy/pgadmin.svg` & `jupyter_pgadmin_proxy-0.0.2/jupyter_pgadmin_proxy/pgadmin.svg`

 * *Files identical despite different names*

### Comparing `jupyter_pgadmin_proxy-0.0.1/.gitignore` & `jupyter_pgadmin_proxy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_pgadmin_proxy-0.0.1/LICENSE.md` & `jupyter_pgadmin_proxy-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jupyter_pgadmin_proxy-0.0.1/README.md` & `jupyter_pgadmin_proxy-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,43 @@
-# jupyter-pgadmin-proxy
+# Jupyter pgAdmin proxy
 
-jupyter-pgadmin-proxy provides Jupyter extension to run [pgAdmin 4](https://pypi.org/project/pgadmin4/). See also official pages for ([pgAdmin](https://www.pgadmin.org/).
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/jupyter-pgadmin-proxy.svg)](https://pypi.org/project/jupyter-pgadmin-proxy/)
+
+jupyter-pgadmin-proxy provides Jupyter extension to run [pgAdmin 4](https://pypi.org/project/pgadmin4/). See also official pages for [pgAdmin](https://www.pgadmin.org/).
 
 ## Installation
 
 You can install jupyter-pgadmin-proxy inside your environment with Jupyter / Jupyterlab:
 
 ```
-python3 -m pip install git+https://github.com/huntdatacenter/jupyter-pgadmin-proxy.git@main
+python3 -m pip install jupyter-pgadmin-proxy
+```
+
+## Build
+
+```
+python3 -m pip install hatch
+
+hatch build
+
+ls -la dist/*
 ```
 
 ## Development
 
 Try `make help` to see available commands:
 
 ```
 make help
 ```
 
+```
+python3 -m pip install git+https://github.com/huntdatacenter/jupyter-pgadmin-proxy.git@main
+``
+
 ## Testing in docker
 
 Run/rebuild local Jupyterlab service:
 
 ```
 make rebuild
 ```
```

### Comparing `jupyter_pgadmin_proxy-0.0.1/pyproject.toml` & `jupyter_pgadmin_proxy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "jupyter-pgadmin-proxy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Matus Kosut", email="matus.kosut@ntnu.no" },
   { name="Diepiriye Okujagu", email="diepiriye.d.okujagu@ntnu.no" },
 ]
 description = "Jupyter server proxy for pgAdmin"
 readme = "README.md"
 license = { file = "LICENSE.md" }
```

### Comparing `jupyter_pgadmin_proxy-0.0.1/PKG-INFO` & `jupyter_pgadmin_proxy-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-pgadmin-proxy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Jupyter server proxy for pgAdmin
 Project-URL: Homepage, https://github.com/huntdatacenter/jupyter-pgadmin-proxy
 Author-email: Matus Kosut <matus.kosut@ntnu.no>, Diepiriye Okujagu <diepiriye.d.okujagu@ntnu.no>
 License: MIT License
         
         Copyright (c) 2023 HUNT Cloud
         
@@ -45,34 +45,50 @@
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: ruamel-yaml; extra == 'dev'
 Description-Content-Type: text/markdown
 
-# jupyter-pgadmin-proxy
+# Jupyter pgAdmin proxy
 
-jupyter-pgadmin-proxy provides Jupyter extension to run [pgAdmin 4](https://pypi.org/project/pgadmin4/). See also official pages for ([pgAdmin](https://www.pgadmin.org/).
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/jupyter-pgadmin-proxy.svg)](https://pypi.org/project/jupyter-pgadmin-proxy/)
+
+jupyter-pgadmin-proxy provides Jupyter extension to run [pgAdmin 4](https://pypi.org/project/pgadmin4/). See also official pages for [pgAdmin](https://www.pgadmin.org/).
 
 ## Installation
 
 You can install jupyter-pgadmin-proxy inside your environment with Jupyter / Jupyterlab:
 
 ```
-python3 -m pip install git+https://github.com/huntdatacenter/jupyter-pgadmin-proxy.git@main
+python3 -m pip install jupyter-pgadmin-proxy
+```
+
+## Build
+
+```
+python3 -m pip install hatch
+
+hatch build
+
+ls -la dist/*
 ```
 
 ## Development
 
 Try `make help` to see available commands:
 
 ```
 make help
 ```
 
+```
+python3 -m pip install git+https://github.com/huntdatacenter/jupyter-pgadmin-proxy.git@main
+``
+
 ## Testing in docker
 
 Run/rebuild local Jupyterlab service:
 
 ```
 make rebuild
 ```
```

