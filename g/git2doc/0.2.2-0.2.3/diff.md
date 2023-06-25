# Comparing `tmp/git2doc-0.2.2.tar.gz` & `tmp/git2doc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git2doc-0.2.2.tar", last modified: Sat Jun 24 21:15:37 2023, max compression
+gzip compressed data, was "git2doc-0.2.3.tar", last modified: Sun Jun 25 20:19:16 2023, max compression
```

## Comparing `git2doc-0.2.2.tar` & `git2doc-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.174569 git2doc-0.2.2/
--rw-rw-rw-   0        0        0     2588 2023-06-24 21:15:37.172570 git2doc-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1919 2023-06-19 20:38:01.000000 git2doc-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.159569 git2doc-0.2.2/git2doc/
--rw-rw-rw-   0        0        0        0 2023-06-19 20:38:01.000000 git2doc-0.2.2/git2doc/__init__.py
--rw-rw-rw-   0        0        0    12158 2023-06-24 21:15:09.000000 git2doc-0.2.2/git2doc/loader.py
-drwxrwxrwx   0        0        0        0 2023-06-24 21:15:37.169574 git2doc-0.2.2/git2doc.egg-info/
--rw-rw-rw-   0        0        0     2588 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-24 21:15:37.000000 git2doc-0.2.2/git2doc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-24 21:15:37.175569 git2doc-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-06-24 21:15:30.000000 git2doc-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.913595 git2doc-0.2.3/
+-rw-rw-rw-   0        0        0     2942 2023-06-25 20:19:16.912599 git2doc-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2273 2023-06-25 20:06:36.000000 git2doc-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.898362 git2doc-0.2.3/git2doc/
+-rw-rw-rw-   0        0        0        0 2023-06-19 20:38:01.000000 git2doc-0.2.3/git2doc/__init__.py
+-rw-rw-rw-   0        0        0    12271 2023-06-25 19:48:30.000000 git2doc-0.2.3/git2doc/loader.py
+drwxrwxrwx   0        0        0        0 2023-06-25 20:19:16.908600 git2doc-0.2.3/git2doc.egg-info/
+-rw-rw-rw-   0        0        0     2942 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-25 20:19:16.000000 git2doc-0.2.3/git2doc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-25 20:19:16.914599 git2doc-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1043 2023-06-25 20:18:56.000000 git2doc-0.2.3/setup.py
```

### Comparing `git2doc-0.2.2/PKG-INFO` & `git2doc-0.2.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Doc 📚
+# git2doc 📚
 
-[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://pypi.org/project/git2doc/)
+A powerful Python library for converting git repositories into documents. git2doc allows you to extract and analyze code from GitHub repositories, making it easier to understand and work with large codebases.
 
-Git2Doc is a Python package that allows you to convert git repositories into documents. It is designed to help developers analyze and understand codebases by providing an easy way to extract and process text content from git repositories.
+## Why git2doc? 🚀
 
-## Table of Contents
+Working with large repositories can be overwhelming, especially when trying to understand the structure and content of the code. git2doc simplifies this process by converting repositories into documents, allowing you to easily search, analyze, and understand the codebase.
+
+## Table of Contents 📖
 
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Example: Fetch and Load Repositories](#example-fetch-and-load-repositories)
-  - [Example: Get Top Repositories](#example-get-top-repositories)
+  - [Fetching Repositories](#fetching-repositories)
+  - [Loading Repository Data](#loading-repository-data)
+  - [Writing Data to Parquet Files](#writing-data-to-parquet-files)
+- [Badges](#badges)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Installation
-
-To install Git2Doc, simply run:
+## Installation 💻
 
 ```bash
 pip install git2doc
 ```
 
-## Usage
+## Usage 🛠️
 
-### Example: Fetch and Load Repositories
+### Fetching Repositories
 
 ```python
-from git2doc.loader import pipeline_fetch_and_load
-
-# Fetch and load the top 5 repositories created in the last 7 days
-github_data = pipeline_fetch_and_load(n_repos=5, last_n_days=7)
+from git2doc import get_repos_orchestrator
 
-# Print the metadata and documents for each repository
-for repo_key, repo_data in github_data.items():
-    print(f"Repository: {repo_key}")
-    print("Metadata:")
-    for key, value in repo_data["metadata"].items():
-        print(f"  {key}: {value}")
-    print("Documents:")
-    for doc in repo_data["docs"]:
-        print(f"  {doc.metadata['file_path']}: {doc.page_content[:50]}...")
+repos = get_repos_orchestrator(
+    n_repos=10,
+    last_n_days=30,
+    language="Python"
+)
 ```
 
-### Example: Get Top Repositories
+### Loading Repository Data
 
 ```python
-from git2doc.loader import get_top_repos
+from git2doc import pull_code_from_repo
+
+repo_data = pull_code_from_repo(
+    repo="https://github.com/voynow/git2doc",
+    branch="main"
+)
+```
 
-# Get the top 5 Python repositories created in the last 7 days
-top_repos = get_top_repos(n_repos=5, last_n_days=7, language="Python")
+### Writing Data to Parquet Files
 
-# Print the repository URLs
-for repo in top_repos:
-    print(repo["html_url"])
+```python
+from git2doc import pipeline_fetch_and_load
+
+pipeline_fetch_and_load(
+    n_repos=1000,
+    last_n_days=365,
+    language="Python",
+    write_batch_size=100,
+    delete=True,
+)
 ```
 
-## Contributing
+## Badges 🏅
+
+[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://badge.fury.io/py/git2doc)
+[![GitHub stars](https://img.shields.io/github/stars/voynow/git2doc)](https://github.com/voynow/git2doc/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/voynow/git2doc)](https://github.com/voynow/git2doc/network)
+[![GitHub issues](https://img.shields.io/github/issues/voynow/git2doc)](https://github.com/voynow/git2doc/issues)
+
+## Contributing 🤝
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue on GitHub.
 
-## License
+## License 📄
 
-Git2Doc is released under the [MIT License](https://opensource.org/licenses/MIT).
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `git2doc-0.2.2/git2doc/loader.py` & `git2doc-0.2.3/git2doc/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,23 @@
     ".sense",
     ".log",
     ".bvh",
     ".onnx",
     ".gltf",
     ".cif",
     ".geojson",
-    "pkl",
+    ".pkl",
+    ".bin",
+    ".pdb",
+    ".sdf",
+    ".xmi",
+    ".out",
+    ".train",
+    ".stl",
+    ".kicad_pcb",
 ]
 REPODATA_FOLDER = "./repodata/"
 
 
 def load_file(item, output_path) -> Optional[dict]:
     """
     Loads a single file from the repository.
```

### Comparing `git2doc-0.2.2/git2doc.egg-info/PKG-INFO` & `git2doc-0.2.3/git2doc.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,81 +1,95 @@
 Metadata-Version: 2.1
 Name: git2doc
-Version: 0.2.2
+Version: 0.2.3
 Summary: A tool for converting git repositories into documents
 Home-page: https://github.com/voynow/git2doc
 Author: Jamie Voynow
 Author-email: voynow99@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
-# Git2Doc 📚
+# git2doc 📚
 
-[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://pypi.org/project/git2doc/)
+A powerful Python library for converting git repositories into documents. git2doc allows you to extract and analyze code from GitHub repositories, making it easier to understand and work with large codebases.
 
-Git2Doc is a Python package that allows you to convert git repositories into documents. It is designed to help developers analyze and understand codebases by providing an easy way to extract and process text content from git repositories.
+## Why git2doc? 🚀
 
-## Table of Contents
+Working with large repositories can be overwhelming, especially when trying to understand the structure and content of the code. git2doc simplifies this process by converting repositories into documents, allowing you to easily search, analyze, and understand the codebase.
+
+## Table of Contents 📖
 
 - [Installation](#installation)
 - [Usage](#usage)
-  - [Example: Fetch and Load Repositories](#example-fetch-and-load-repositories)
-  - [Example: Get Top Repositories](#example-get-top-repositories)
+  - [Fetching Repositories](#fetching-repositories)
+  - [Loading Repository Data](#loading-repository-data)
+  - [Writing Data to Parquet Files](#writing-data-to-parquet-files)
+- [Badges](#badges)
 - [Contributing](#contributing)
 - [License](#license)
 
-## Installation
-
-To install Git2Doc, simply run:
+## Installation 💻
 
 ```bash
 pip install git2doc
 ```
 
-## Usage
+## Usage 🛠️
 
-### Example: Fetch and Load Repositories
+### Fetching Repositories
 
 ```python
-from git2doc.loader import pipeline_fetch_and_load
-
-# Fetch and load the top 5 repositories created in the last 7 days
-github_data = pipeline_fetch_and_load(n_repos=5, last_n_days=7)
+from git2doc import get_repos_orchestrator
 
-# Print the metadata and documents for each repository
-for repo_key, repo_data in github_data.items():
-    print(f"Repository: {repo_key}")
-    print("Metadata:")
-    for key, value in repo_data["metadata"].items():
-        print(f"  {key}: {value}")
-    print("Documents:")
-    for doc in repo_data["docs"]:
-        print(f"  {doc.metadata['file_path']}: {doc.page_content[:50]}...")
+repos = get_repos_orchestrator(
+    n_repos=10,
+    last_n_days=30,
+    language="Python"
+)
 ```
 
-### Example: Get Top Repositories
+### Loading Repository Data
 
 ```python
-from git2doc.loader import get_top_repos
+from git2doc import pull_code_from_repo
+
+repo_data = pull_code_from_repo(
+    repo="https://github.com/voynow/git2doc",
+    branch="main"
+)
+```
 
-# Get the top 5 Python repositories created in the last 7 days
-top_repos = get_top_repos(n_repos=5, last_n_days=7, language="Python")
+### Writing Data to Parquet Files
 
-# Print the repository URLs
-for repo in top_repos:
-    print(repo["html_url"])
+```python
+from git2doc import pipeline_fetch_and_load
+
+pipeline_fetch_and_load(
+    n_repos=1000,
+    last_n_days=365,
+    language="Python",
+    write_batch_size=100,
+    delete=True,
+)
 ```
 
-## Contributing
+## Badges 🏅
+
+[![PyPI version](https://badge.fury.io/py/git2doc.svg)](https://badge.fury.io/py/git2doc)
+[![GitHub stars](https://img.shields.io/github/stars/voynow/git2doc)](https://github.com/voynow/git2doc/stargazers)
+[![GitHub forks](https://img.shields.io/github/forks/voynow/git2doc)](https://github.com/voynow/git2doc/network)
+[![GitHub issues](https://img.shields.io/github/issues/voynow/git2doc)](https://github.com/voynow/git2doc/issues)
+
+## Contributing 🤝
 
 Contributions are welcome! Please feel free to submit a pull request or open an issue on GitHub.
 
-## License
+## License 📄
 
-Git2Doc is released under the [MIT License](https://opensource.org/licenses/MIT).
+This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `git2doc-0.2.2/setup.py` & `git2doc-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='git2doc',
-    version='0.2.2',
+    version='0.2.3',
     description='A tool for converting git repositories into documents',
     author='Jamie Voynow',
     author_email='voynow99@gmail.com',
     url='https://github.com/voynow/git2doc',
     packages=find_packages(),
     install_requires=[
         'langchain',
```

