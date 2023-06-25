# Comparing `tmp/openfractal_client-0.1.1.tar.gz` & `tmp/openfractal_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfractal_client-0.1.1.tar", last modified: Sun Jun 25 19:56:14 2023, max compression
+gzip compressed data, was "openfractal_client-0.1.2.tar", last modified: Sun Jun 25 21:23:34 2023, max compression
```

## Comparing `openfractal_client-0.1.1.tar` & `openfractal_client-0.1.2.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/code-check.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/doc.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/CHANGELOGS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/auto_install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/configs/manager_local.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/configs/manager_slurm.yml
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/construct.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/license.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.729010 openfractal_client-0.1.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/01_submit_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/02_execute_manager.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    32553 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/docs/tutorials/03_export_dataset.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/env.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/openfractal_client/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/openfractal_client/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/openfractal_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 19:56:14.000000 openfractal_client-0.1.1/openfractal_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 19:56:14.733011 openfractal_client-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 19:52:17.000000 openfractal_client-0.1.1/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.245152 openfractal_client-0.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/workflows/code-check.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/workflows/doc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/workflows/docker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/CHANGELOGS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11315 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/configs/manager_local.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/configs/manager_slurm.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/construct.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/license.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)    50050 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/tutorials/01_submit_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    40864 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/tutorials/02_execute_manager.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    32553 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/docs/tutorials/03_export_dataset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/env.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/openfractal_client/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/openfractal_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/openfractal_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/openfractal_client/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/openfractal_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-25 21:23:34.000000 openfractal_client-0.1.2/openfractal_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-25 21:23:34.000000 openfractal_client-0.1.2/openfractal_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 21:23:34.000000 openfractal_client-0.1.2/openfractal_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-25 21:23:34.000000 openfractal_client-0.1.2/openfractal_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 21:23:34.000000 openfractal_client-0.1.2/openfractal_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/scripts/auto_install.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/scripts/build_installer.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 21:23:34.249152 openfractal_client-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 21:20:53.000000 openfractal_client-0.1.2/tests/test_import.py
```

### Comparing `openfractal_client-0.1.1/.github/CODE_OF_CONDUCT.md` & `openfractal_client-0.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/.github/workflows/code-check.yml` & `openfractal_client-0.1.2/.github/workflows/code-check.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/.github/workflows/doc.yml` & `openfractal_client-0.1.2/.github/workflows/doc.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/.github/workflows/docker.yml` & `openfractal_client-0.1.2/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/.github/workflows/release.yml` & `openfractal_client-0.1.2/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -30,19 +30,14 @@
       - name: Setup mamba
         uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: env.yml
           environment-name: openfractal
           cache-environment: true
           cache-downloads: true
-          create-args: >-
-            pip
-            semver
-            python-build
-            setuptools_scm
 
       - name: Check the version is valid semver
         run: |
           RELEASE_VERSION="${{ inputs.release-version }}"
 
           {
             pysemver check $RELEASE_VERSION
@@ -103,27 +98,61 @@
 
       - name: Publish package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           packages-dir: dist/
 
-      - name: Build standalone installer
-        run: |
-          export OPENFRACTAL_CLIENT_CONSTRUCTOR_VERSION="${{ inputs.release-version }}"
-          CONDA_SOLVER=libmamba constructor --platform=linux-64 .
-
       - name: Create GitHub Release
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           tag_name: ${{ inputs.release-version }}
           body: ${{steps.github_release.outputs.changelog}}
-          files: OpenFractalClient-*.sh
 
       - name: Deploy the doc
         run: |
           echo "Get the gh-pages branch"
           git fetch origin gh-pages
 
           echo "Build and deploy the doc on ${{ inputs.release-version }}"
           mike deploy --push --force stable
           mike deploy --push --force ${{ inputs.release-version }}
+
+  build-installer-linux:
+    needs: [release]
+
+    runs-on: ubuntu-latest
+    timeout-minutes: 30
+
+    defaults:
+      run:
+        shell: bash -l {0}
+
+    steps:
+      - name: Checkout the code
+        uses: actions/checkout@v3
+        with:
+          ref: ${{ inputs.release-version }}
+
+      - name: Setup mamba
+        uses: mamba-org/setup-micromamba@v1
+        with:
+          environment-file: env.yml
+          environment-name: openfractal
+          cache-environment: true
+          cache-downloads: true
+
+      - name: Build the wheel and sdist
+        run: python -m build --no-isolation
+
+      - name: Build standalone installer
+        run: |
+          export OPENFRACTAL_CLIENT_CONSTRUCTOR_VERSION="${{ inputs.release-version }}"
+          bash ./scripts/build_installer.sh
+
+      - name: Create GitHub Release
+        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        with:
+          tag_name: ${{ inputs.release-version }}
+          files: |
+            ./build/*.sh
+            ./build/*.sha256
```

### Comparing `openfractal_client-0.1.1/.github/workflows/test.yml` & `openfractal_client-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/Dockerfile` & `openfractal_client-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/LICENSE` & `openfractal_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/PKG-INFO` & `openfractal_client-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal_client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.1.1/README.md` & `openfractal_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/configs/manager_local.yml` & `openfractal_client-0.1.2/configs/manager_local.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/configs/manager_slurm.yml` & `openfractal_client-0.1.2/configs/manager_slurm.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/construct.yaml` & `openfractal_client-0.1.2/construct.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -32,7 +32,8 @@
   - datamol
   - openff-toolkit
   - zarr
 
 installer_type: sh
 initialize_by_default: false
 register_python: False
+batch_mode: true
```

### Comparing `openfractal_client-0.1.1/docker-compose.yml` & `openfractal_client-0.1.2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/docs/index.md` & `openfractal_client-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/docs/installation.md` & `openfractal_client-0.1.2/docs/installation.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Installation
 
 ## Automatic Installation
 
 For participating to the data generation effort only. If you want to interact with the datasets or submit datasets yourself, you must use one of the other installation methods.
 
 ```bash
-curl https://raw.githubusercontent.com/OpenDrugDiscovery/openfractal-client/main/auto_install.sh | bash
+curl https://raw.githubusercontent.com/OpenDrugDiscovery/openfractal-client/main/scripts/auto_install.sh | bash
 ```
 
 ## Docker
 
 Public docker images are available at <https://github.com/OpenDrugDiscovery/openfractal-client/pkgs/container/openfractal-client>.
 
 ```bash
```

### Comparing `openfractal_client-0.1.1/docs/tutorials/01_submit_dataset.ipynb` & `openfractal_client-0.1.2/docs/tutorials/01_submit_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/docs/tutorials/02_execute_manager.ipynb` & `openfractal_client-0.1.2/docs/tutorials/02_execute_manager.ipynb`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/docs/tutorials/03_export_dataset.ipynb` & `openfractal_client-0.1.2/docs/tutorials/03_export_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/env.yml` & `openfractal_client-0.1.2/env.yml`

 * *Files 19% similar despite different names*

```diff
@@ -22,18 +22,14 @@
   - openmmforcefields
 
   # Optional
   - datamol
   - openff-toolkit
   - zarr
 
-  # Packaging
-  - constructor
-  - conda-libmamba-solver
-
   # Dev
   - pytest >=6.0
   - black >=23
   - jupyterlab
   - ipywidgets
   - nglview
   - ipytree
@@ -45,7 +41,14 @@
   - mkdocs-material-extensions
   - mkdocstrings
   - mkdocstrings-python
   - mkdocs-jupyter
   - markdown-include
   - mdx_truly_sane_lists
   - mike >=1.0.0
+
+  # Packaging
+  - constructor
+  - conda-libmamba-solver
+  - python-build
+  - setuptools_scm
+  - semver
```

### Comparing `openfractal_client-0.1.1/mkdocs.yml` & `openfractal_client-0.1.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/openfractal_client/cli.py` & `openfractal_client-0.1.2/openfractal_client/cli.py`

 * *Files identical despite different names*

### Comparing `openfractal_client-0.1.1/openfractal_client.egg-info/PKG-INFO` & `openfractal_client-0.1.2/openfractal_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfractal-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python client based on QCPortal for Open Drug Discovery (ODD) QM large scale data generation.
 Author-email: Hadrien Mary <hadrien@valencediscovery.com>
 License: Apache
 Project-URL: Source Code, https://github.com/OpenDrugDiscovery/openfractal-client
 Project-URL: Bug Tracker, https://github.com/OpenDrugDiscovery/openfractal-client/issues
 Project-URL: Documentation, https://github.com/OpenDrugDiscovery/openfractal-client
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `openfractal_client-0.1.1/pyproject.toml` & `openfractal_client-0.1.2/pyproject.toml`

 * *Files identical despite different names*

