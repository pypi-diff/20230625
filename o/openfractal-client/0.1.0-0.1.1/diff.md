# Comparing `tmp/openfractal_client-0.1.0.tar.gz` & `tmp/openfractal_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.1.0.tar", last modified: Sat Jun 24 14:25:46 2023, max compression
+gzip compressed data, was "openfractal_client-0.1.1.tar", last modified: Sun Jun 25 19:56:14 2023, max compression
```

## Comparing `openfractal_client-0.1.0.tar` & `openfractal_client-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/CHANGELOGS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/configs/manager_local.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/configs/manager_slurm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.505146 openfractal_client-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/01_submit_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    36862 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/02_execute_manager.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31799 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/docs/tutorials/03_export_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/openfractal_client/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/openfractal_client/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/openfractal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-24 14:25:46.000000 openfractal_client-0.1.0/openfractal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 14:25:46.509147 openfractal_client-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-24 14:22:35.000000 openfractal_client-0.1.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/auto_install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/configs/manager_local.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/configs/manager_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/construct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/01_submit_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/02_execute_manager.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32553 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/03_export_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/tests/test_import.py
```

### Comparing `openfractal_client-0.1.0/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.1.1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/.github/workflows/code-check.yml` & `openfractal_client-0.1.1/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/.github/workflows/doc.yml` & `openfractal_client-0.1.1/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/.github/workflows/docker.yml` & `openfractal_client-0.1.1/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/.github/workflows/release.yml` & `openfractal_client-0.1.1/.github/workflows/release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -103,19 +103,25 @@
 
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
+      - name: Build standalone installer
+        run: |
+          export OPENFRACTAL_CLIENT_CONSTRUCTOR_VERSION="${{ inputs.release-version }}"
+          CONDA_SOLVER=libmamba constructor --platform=linux-64 .
+
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
           body: ${{steps.github_release.outputs.changelog}}
+          files: OpenFractalClient-*.sh
 
       - name: Deploy the doc
         run: |
           echo "Get the gh-pages branch"
           git fetch origin gh-pages
 
           echo "Build and deploy the doc on ${{ inputs.release-version }}"
```

### Comparing `openfractal_client-0.1.0/.github/workflows/test.yml` & `openfractal_client-0.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/Dockerfile` & `openfractal_client-0.1.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/LICENSE` & `openfractal_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/PKG-INFO` & `openfractal_client-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.1.0/README.md` & `openfractal_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/configs/manager_local.yml` & `openfractal_client-0.1.1/configs/manager_local.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/configs/manager_slurm.yml` & `openfractal_client-0.1.1/configs/manager_slurm.yml`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     worker_init: []
     scratch_directory: null
     bind_address: 127.0.0.1
     cores_per_worker: 16
     memory_per_worker: 16 # GB
     extra_executor_options: {}
 
-    # Specific options for the local executor.
+    # Specific options for the SLURM executor.
     walltime: "1:00:00"
     exclusive: false
     partition: null
     account: null
     workers_per_node: 7
     max_nodes: 1
     scheduler_options: []
```

### Comparing `openfractal_client-0.1.0/docker-compose.yml` & `openfractal_client-0.1.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/docs/tutorials/01_submit_dataset.ipynb` & `openfractal_client-0.1.1/docs/tutorials/01_submit_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/docs/tutorials/02_execute_manager.ipynb` & `openfractal_client-0.1.1/docs/tutorials/02_execute_manager.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9768075989550455%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(0, '### Local\\n')], delete: [23, 16, 0]}}, 4: {'source': "*

 * *            "{insert: [(0, '### SLURM\\n'), (40, '    # Specific options for the SLURM "*

 * *            "executor.\\n')], delete: [42, 23, 16, 0]}}, 11: {'source': {insert: [(3, '\\n'), (4, "*

 * *            "'ds.dict()')], delete: [3]}}, 14: {'source': {insert: [(0, 'progress = True\\n'), (1, "*

 * *            "'status = None\\n'), (2, 'fetch_error = True\\n'), (3, 'fetch_wfn = True\\n'), (4, "*

 * *            "'\\n'), (5,  […]*

```diff
@@ -27,20 +27,31 @@
                 "\n",
                 "_ = dotenv.load_dotenv(\"../../openfractal_test_secrets.env\")"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
+            "id": "58df69fe",
+            "metadata": {},
+            "source": [
+                "## Launch a Manager\n",
+                "\n",
+                "A manager or a worker is responisble to receive jobs from a backend QCFractal server, execute those jobs and report the results to the backend server."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
             "id": "26b21668-89e4-4ddb-8721-635e246d2c58",
             "metadata": {
                 "jp-MarkdownHeadingCollapsed": true
             },
             "source": [
-                "## Launch a manager: local\n",
+                "### Local\n",
                 "\n",
                 "A manager is a QM worker that will perform any QM calculations provided by an Openfractal instance.\n",
                 "\n",
                 "You first need to create a YAML config file `manager_local.yml`:\n",
                 "\n",
                 "```yaml\n",
                 "base_folder: /tmp/qcf_compute\n",
@@ -48,22 +59,20 @@
                 "cluster: manager_demo_local_1\n",
                 "\n",
                 "loglevel: INFO\n",
                 "logfile: null\n",
                 "\n",
                 "update_frequency: 30\n",
                 "\n",
-                "# Settings to connect to the Fractal Server.\n",
                 "server:\n",
                 "  fractal_uri: https://openfractal-test-pgzbs3yryq-uc.a.run.app\n",
                 "  username: YOUR_USERNAME\n",
                 "  password: YOUR_PASSWORD\n",
                 "  verify: false\n",
                 "\n",
-                "# How and where to detect the QM softwares.\n",
                 "environments:\n",
                 "  use_manager_environment: true\n",
                 "  conda: []\n",
                 "  apptainer: []\n",
                 "\n",
                 "executors:\n",
                 "  local:\n",
@@ -93,15 +102,15 @@
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "a7b8d866",
             "metadata": {},
             "source": [
-                "## Launch a manager: SLURM\n",
+                "### SLURM\n",
                 "\n",
                 "A manager is a QM worker that will perform any QM calculations provided by an Openfractal instance.\n",
                 "\n",
                 "You first need to create a YAML config file `manager_slurm.yml`:\n",
                 "\n",
                 "```yaml\n",
                 "base_folder: /tmp/qcf_compute\n",
@@ -109,22 +118,20 @@
                 "cluster: manager_demo_slurm_1\n",
                 "\n",
                 "loglevel: INFO\n",
                 "logfile: null\n",
                 "\n",
                 "update_frequency: 30\n",
                 "\n",
-                "# Settings to connect to the Fractal Server.\n",
                 "server:\n",
                 "  fractal_uri: https://openfractal-test-pgzbs3yryq-uc.a.run.app\n",
                 "  username: YOUR_USERNAME\n",
                 "  password: YOUR_PASSWORD\n",
                 "  verify: false\n",
                 "\n",
-                "# How and where to detect the QM softwares.\n",
                 "environments:\n",
                 "  use_manager_environment: true\n",
                 "  conda: []\n",
                 "  apptainer: []\n",
                 "\n",
                 "executors:\n",
                 "  slurm:\n",
@@ -135,15 +142,15 @@
                 "    worker_init: []\n",
                 "    scratch_directory: null\n",
                 "    bind_address: 127.0.0.1\n",
                 "    cores_per_worker: 16\n",
                 "    memory_per_worker: 16 # GB\n",
                 "    extra_executor_options: {}\n",
                 "\n",
-                "    # Specific options for the local executor.\n",
+                "    # Specific options for the SLURM executor.\n",
                 "    walltime: \"1:00:00\"\n",
                 "    exclusive: false\n",
                 "    partition: null\n",
                 "    account: null\n",
                 "    workers_per_node: 7\n",
                 "    max_nodes: 1\n",
                 "    scheduler_options: []\n",
@@ -155,14 +162,99 @@
                 "qcfractal-compute-manager --config manager_slurm.yml\n",
                 "```"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
+            "id": "f408c10b",
+            "metadata": {},
+            "source": [
+                "### Docker\n",
+                "\n",
+                "#### With `docker-compose`\n",
+                "\n",
+                "You can use the following docker-compose configuration:\n",
+                "\n",
+                "```yaml\n",
+                "version: \"3\"\n",
+                "services:\n",
+                "  opf_manager:\n",
+                "    image: ghcr.io/opendrugdiscovery/openfractal-client:main\n",
+                "    command: qcfractal-compute-manager\n",
+                "    environment:\n",
+                "      # General\n",
+                "      QCF_COMPUTE_BASE_FOLDER: /tmp/\n",
+                "      QCF_COMPUTE_CLUSTER: manager_demo_1\n",
+                "      QCF_COMPUTE_LOGLEVEL: INFO\n",
+                "      QCF_COMPUTE_UPDATE_FREQUENCY: 30\n",
+                "      # Server\n",
+                "      QCF_COMPUTE_SERVER: \"{}\" # somehow this is needed....\n",
+                "      QCF_COMPUTE_SERVER_FRACTAL_URI: https://openfractal-test-pgzbs3yryq-uc.a.run.app\n",
+                "      QCF_COMPUTE_SERVER_USERNAME: YOUR_USERNAME\n",
+                "      QCF_COMPUTE_SERVER_PASSWORD: YOUR_PASSWORD\n",
+                "      QCF_COMPUTE_SERVER_VERIFY: false\n",
+                "      # Environment\n",
+                "      QCF_COMPUTE_ENVIRONMENTS_USE_MANAGER_ENVIRONMENT: true\n",
+                "      QCF_COMPUTE_ENVIRONMENTS_CONDA: \"[]\"\n",
+                "      QCF_COMPUTE_ENVIRONMENTS_APPTAINER: \"[]\"\n",
+                "      # Executors\n",
+                "      QCF_COMPUTE_EXECUTORS: '{\"local\": {\"type\": \"local\", \"queue_tags\": [\"demo_tutorial\"], \"cores_per_worker\": 16, \"memory_per_worker\": 16, \"max_workers\": 4}}'\n",
+                "```\n",
+                "\n",
+                "Then execute the container with:\n",
+                "\n",
+                "```bash\n",
+                " # Execute in the background\n",
+                "docker-compose up -d\n",
+                "\n",
+                " # Check logs\n",
+                "docker-compose logs -f\n",
+                "\n",
+                " # Shutdown the manager\n",
+                "docker-compose down\n",
+                "```\n",
+                "\n",
+                "#### With `docker`\n",
+                "\n",
+                "It is recommended and often more convenient to use `docker-compose`. If you prefer to use `docker`:\n",
+                "\n",
+                "```bash\n",
+                "docker run --rm -ti \\\n",
+                "  -e QCF_COMPUTE_BASE_FOLDER=\"/tmp/\" \\\n",
+                "  -e QCF_COMPUTE_CLUSTER=\"manager_demo_1\" \\\n",
+                "  -e QCF_COMPUTE_LOGLEVEL=\"INFO\" \\\n",
+                "  -e QCF_COMPUTE_UPDATE_FREQUENCY=\"30\" \\\n",
+                "  -e QCF_COMPUTE_SERVER=\"{}\"  \\\n",
+                "  -e QCF_COMPUTE_SERVER_FRACTAL_URI=\"https://openfractal-test-pgzbs3yryq-uc.a.run.app\" \\\n",
+                "  -e QCF_COMPUTE_SERVER_USERNAME=\"YOUR_USERNAME\" \\\n",
+                "  -e QCF_COMPUTE_SERVER_PASSWORD=\"YOUR_PASSWORD\" \\\n",
+                "  -e QCF_COMPUTE_SERVER_VERIFY=\"false\" \\\n",
+                "  -e QCF_COMPUTE_ENVIRONMENTS_USE_MANAGER_ENVIRONMENT=\"true\" \\\n",
+                "  -e QCF_COMPUTE_ENVIRONMENTS_CONDA=\"[]\" \\\n",
+                "  -e QCF_COMPUTE_ENVIRONMENTS_APPTAINER=\"[]\" \\\n",
+                "  -e QCF_COMPUTE_EXECUTORS='{\"local\": {\"type\": \"local\", \"queue_tags\": [\"demo_tutorial\"], \"cores_per_worker\": 16, \"memory_per_worker\": 16, \"max_workers\": 4}}' \\\n",
+                "  ghcr.io/opendrugdiscovery/openfractal-client:main qcfractal-compute-manager\n",
+                "```\n"
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
+            "id": "3b389c00",
+            "metadata": {},
+            "source": [
+                "### HuggingFace Space\n",
+                "\n",
+                "Follow the instructions at <https://huggingface.co/spaces/hadim/openfractal-client-space/blob/main/README.md>."
+            ]
+        },
+        {
+            "attachments": {},
+            "cell_type": "markdown",
             "id": "bab80522-4c82-484d-a85b-5474a62fe06d",
             "metadata": {},
             "source": [
                 "## Monitor the managers"
             ]
         },
         {
@@ -428,15 +520,16 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "dataset_name = \"dataset_demo_4321690179\"\n",
                 "\n",
                 "ds = client.get_dataset(\"singlepoint\", dataset_name)\n",
-                "ds"
+                "\n",
+                "ds.dict()"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "id": "87912998-a88b-4301-9dfc-e7aa7cee6880",
             "metadata": {},
@@ -874,20 +967,37 @@
                     },
                     "execution_count": 6,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "progress = True\n",
+                "status = None\n",
+                "fetch_error = True\n",
+                "fetch_wfn = True\n",
+                "\n",
+                "\n",
                 "records_list = []\n",
-                "for r in tqdm(client.query_records(dataset_id=ds.id)):\n",
-                "    # Access those objects to fetch them locally\n",
-                "    r.error\n",
-                "    r.wavefunction\n",
-                "    records_list.append(r.dict())\n",
+                "for spec_name in tqdm(ds.specification_names, disable=not progress):\n",
+                "    record_iterator = ds.iterate_records(\n",
+                "        specification_names=spec_name,\n",
+                "        force_refetch=True,\n",
+                "        fetch_updated=True,\n",
+                "        status=status,\n",
+                "    )\n",
+                "\n",
+                "    for _, _, record in tqdm(record_iterator, disable=not progress, leave=False):\n",
+                "        if fetch_error:\n",
+                "            record.error\n",
+                "        if fetch_wfn:\n",
+                "            record.wavefunction  # type: ignore\n",
+                "        record_dict = record.dict()\n",
+                "        record_dict[\"specification_name\"] = spec_name\n",
+                "        records_list.append(record_dict)\n",
                 "\n",
                 "records = pd.DataFrame(records_list)\n",
                 "records = records.sort_values(\"id\")\n",
                 "records = records.reset_index(drop=True)\n",
                 "\n",
                 "records"
             ]
@@ -957,15 +1067,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.4"
+            "version": "3.11.3"
         },
         "widgets": {
             "application/vnd.jupyter.widget-state+json": {
                 "state": {},
                 "version_major": 2,
                 "version_minor": 0
             }
```

### Comparing `openfractal_client-0.1.0/docs/tutorials/03_export_dataset.ipynb` & `openfractal_client-0.1.1/docs/tutorials/03_export_dataset.ipynb`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9894485294117648%*

 * *Differences: {"'cells'": "{0: {'attachments': OrderedDict()}, 2: {'attachments': OrderedDict()}, 4: "*

 * *            "{'attachments': OrderedDict()}, 6: {'attachments': OrderedDict()}, 8: {'attachments': "*

 * *            "OrderedDict()}, 10: {'source': {insert: [(0, 'progress = True\\n'), (1, 'status = "*

 * *            "None\\n'), (2, 'fetch_error = True\\n'), (3, 'fetch_wfn = True\\n'), (4, '\\n'), (5, "*

 * *            "'\\n'), (7, 'for spec_name in tqdm(ds.specification_names, disable=not "*

 * *            "progress):\\n'), (8, '     […]*

```diff
@@ -1,10 +1,11 @@
 {
     "cells": [
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "1c715d1a-cc69-4eaf-a2fe-b04951fa0ce9",
             "metadata": {},
             "source": [
                 "In this tutorial, you'll learn how to read and export records."
             ]
         },
@@ -34,14 +35,15 @@
                 "import qcelemental as qcel\n",
                 "from qcportal import PortalClient\n",
                 "\n",
                 "_ = dotenv.load_dotenv(\"../../openfractal_test_secrets.env\")"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "1f9cb60b-430f-4705-ac13-3b5d83399915",
             "metadata": {},
             "source": [
                 "## Initialize the client and list the datasets"
             ]
         },
@@ -78,14 +80,15 @@
                 "    password=os.environ[\"OPENFRACTAL_USER_3_PASSWORD\"],\n",
                 ")\n",
                 "\n",
                 "client"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "5347e5da-7d4c-463d-ab83-173fd554c2f3",
             "metadata": {},
             "source": [
                 "Let's list the available dataset."
             ]
         },
@@ -109,14 +112,15 @@
                 }
             ],
             "source": [
                 "client.list_datasets()"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "a8f2c042-49b8-43f4-94f5-b4c0fb38ca6f",
             "metadata": {},
             "source": [
                 "## Load a dataset given its name and fetch its records"
             ]
         },
@@ -141,14 +145,15 @@
                 "dataset_name = \"dataset_demo_4321690179\"\n",
                 "\n",
                 "ds = client.get_dataset(\"singlepoint\", dataset_name)\n",
                 "ds"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "634fe054-1efd-47b1-b930-5c76868e135a",
             "metadata": {},
             "source": [
                 "Refresh the below often."
             ]
         },
@@ -582,29 +587,47 @@
                     },
                     "execution_count": 8,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
+                "progress = True\n",
+                "status = None\n",
+                "fetch_error = True\n",
+                "fetch_wfn = True\n",
+                "\n",
+                "\n",
                 "records_list = []\n",
-                "for r in tqdm(client.query_records(dataset_id=ds.id)):\n",
-                "    # Access those objects to fetch them locally\n",
-                "    r.error\n",
-                "    r.wavefunction\n",
-                "    records_list.append(r.dict())\n",
+                "for spec_name in tqdm(ds.specification_names, disable=not progress):\n",
+                "    record_iterator = ds.iterate_records(\n",
+                "        specification_names=spec_name,\n",
+                "        force_refetch=True,\n",
+                "        fetch_updated=True,\n",
+                "        status=status,\n",
+                "    )\n",
+                "\n",
+                "    for _, _, record in tqdm(record_iterator, disable=not progress, leave=False):\n",
+                "        if fetch_error:\n",
+                "            record.error\n",
+                "        if fetch_wfn:\n",
+                "            record.wavefunction  # type: ignore\n",
+                "        record_dict = record.dict()\n",
+                "        record_dict[\"specification_name\"] = spec_name\n",
+                "        records_list.append(record_dict)\n",
                 "\n",
                 "records = pd.DataFrame(records_list)\n",
                 "records = records.sort_values(\"id\")\n",
                 "records = records.reset_index(drop=True)\n",
                 "\n",
                 "records"
             ]
         },
         {
+            "attachments": {},
             "cell_type": "markdown",
             "id": "48a834ca-e96e-429a-9b74-d5d5a5cda5f1",
             "metadata": {},
             "source": [
                 "## End-to-end export to Zarr\n",
                 "\n",
                 "The below function is opiniated en-to-end export pipeline. It's very opiniated and probably not optimal since many of the outputs are not stored as array.\n",
```

### Comparing `openfractal_client-0.1.0/env.yml` & `openfractal_client-0.1.1/env.yml`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,18 @@
   - openmmforcefields
 
   # Optional
   - datamol
   - openff-toolkit
   - zarr
 
+  # Packaging
+  - constructor
+  - conda-libmamba-solver
+
   # Dev
   - pytest >=6.0
   - black >=23
   - jupyterlab
   - ipywidgets
   - nglview
   - ipytree
```

### Comparing `openfractal_client-0.1.0/mkdocs.yml` & `openfractal_client-0.1.1/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 docs_dir: "docs"
 
 # Fail on warnings to detect issues with types and docstring
 strict: true
 
 nav:
   - Overview: index.md
+  - Installation: installation.md
   - Tutorials:
       - Submit a Dataset: tutorials/01_submit_dataset.ipynb
       - Execute a Manager: tutorials/02_execute_manager.ipynb
       - Export a Dataset: tutorials/03_export_dataset.ipynb
   - License: license.md
 
 theme:
```

### Comparing `openfractal_client-0.1.0/openfractal_client/cli.py` & `openfractal_client-0.1.1/openfractal_client/cli.py`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.0/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.1.1/openfractal_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.1.0/openfractal_client.egg-info/SOURCES.txt` & `openfractal_client-0.1.1/openfractal_client.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 CHANGELOGS.md
 Dockerfile
 LICENSE
 README.md
+auto_install.sh
+construct.yaml
 docker-compose.yml
 env.yml
 mkdocs.yml
 pyproject.toml
 .github/CODEOWNERS
 .github/CODE_OF_CONDUCT.md
 .github/PULL_REQUEST_TEMPLATE.md
@@ -15,14 +17,15 @@
 .github/workflows/doc.yml
 .github/workflows/docker.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 configs/manager_local.yml
 configs/manager_slurm.yml
 docs/index.md
+docs/installation.md
 docs/license.md
 docs/tutorials/01_submit_dataset.ipynb
 docs/tutorials/02_execute_manager.ipynb
 docs/tutorials/03_export_dataset.ipynb
 openfractal_client/__init__.py
 openfractal_client/_version.py
 openfractal_client/cli.py
```

### Comparing `openfractal_client-0.1.0/pyproject.toml` & `openfractal_client-0.1.1/pyproject.toml`

 * *Files identical despite different names*

