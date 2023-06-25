# Comparing `tmp/blackboardsync-0.9.0a1.tar.gz` & `tmp/blackboardsync-0.9.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blackboardsync-0.9.0a1.tar", last modified: Wed Jun 21 09:08:54 2023, max compression
+gzip compressed data, was "blackboardsync-0.9.2rc1.tar", last modified: Sun Jun 25 17:20:55 2023, max compression
```

## Comparing `blackboardsync-0.9.0a1.tar` & `blackboardsync-0.9.2rc1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/ISSUE_TEMPLATE/unisupport.yml
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.567335 blackboardsync-0.9.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/UNIVERSITIES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/alert.png
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/alert.svg
--rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/assets/watermark.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/blackboard/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/blackboard/blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/institutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.571336 blackboardsync-0.9.0a1/blackboard_sync/qt/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/LoginWebView.ui
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/PersistenceWarning.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/SettingsWindow.ui
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/SetupWizard.ui
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/UniNotSupportedDialog.ui
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/qt/qt_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/sync_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/universities.json
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/blackboard_sync/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/blackboardsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 09:08:54.000000 blackboardsync-0.9.0a1/blackboardsync.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/bb_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/qt_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/dev/sync_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.575336 blackboardsync-0.9.0a1/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pkg_macos.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pkg_win.nsi
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/packaging/pyinst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:54.579336 blackboardsync-0.9.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_blackboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-21 09:08:08.000000 blackboardsync-0.9.0a1/tests/test_sync_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/.github/ISSUE_TEMPLATE/unisupport.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   107308 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/UNIVERSITIES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/blackboard_sync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/blackboard_sync/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/assets/alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/assets/alert.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   110234 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    31742 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36877 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/assets/watermark.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.921773 blackboardsync-0.9.2rc1/blackboard_sync/blackboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/blackboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/blackboard/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/blackboard/blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10082 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/institutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/blackboard_sync/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/LoginWebView.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/PersistenceWarning.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/SettingsWindow.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/SetupWizard.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/UniNotSupportedDialog.ui
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20342 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/qt/qt_elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10269 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/sync_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13794 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/universities.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/blackboard_sync/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/blackboardsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-25 17:20:55.000000 blackboardsync-0.9.2rc1/blackboardsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-25 17:20:55.000000 blackboardsync-0.9.2rc1/blackboardsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 17:20:55.000000 blackboardsync-0.9.2rc1/blackboardsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-25 17:20:55.000000 blackboardsync-0.9.2rc1/blackboardsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 17:20:55.000000 blackboardsync-0.9.2rc1/blackboardsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/dev/bb_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/dev/qt_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/dev/sync_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/packaging/pkg_macos.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/packaging/pkg_win.nsi
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/packaging/pyinst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:55.925773 blackboardsync-0.9.2rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/test_blackboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/test_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-25 17:20:12.000000 blackboardsync-0.9.2rc1/tests/test_sync_config.py
```

### Comparing `blackboardsync-0.9.0a1/.github/ISSUE_TEMPLATE/unisupport.yml` & `blackboardsync-0.9.2rc1/.github/ISSUE_TEMPLATE/unisupport.yml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/.github/workflows/build.yml` & `blackboardsync-0.9.2rc1/.github/workflows/build.yml`

 * *Files 2% similar despite different names*

```diff
@@ -130,10 +130,11 @@
           packaging/pkg_macos.sh "blackboard_sync-$GITHUB_REF_NAME"
 
       # Save Packages
 
       - name: Upload as release - only tagged commits
         uses: softprops/action-gh-release@v1
         with:
+          prerelease: ${{ contains(github.ref_name, '-') }}
           files: |
             dist/*.exe
             dist/*.dmg
```

### Comparing `blackboardsync-0.9.0a1/.gitignore` & `blackboardsync-0.9.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/CHANGELOG.md` & `blackboardsync-0.9.2rc1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/CONTRIBUTING.md` & `blackboardsync-0.9.2rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/LICENSE` & `blackboardsync-0.9.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/PKG-INFO` & `blackboardsync-0.9.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.0a1
+Version: 0.9.2rc1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.0a1/Pipfile` & `blackboardsync-0.9.2rc1/Pipfile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/Pipfile.lock` & `blackboardsync-0.9.2rc1/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9980994152046784%*

 * *Differences: {"'develop'": "{'hypothesis': {'hashes': "*

 * *              "['sha256:51fb2259489dc446d3edc04cbc8ebd5848d7d3f238121183bee5449b91f7a8d8', "*

 * *              "'sha256:564d9860ed5e09b0434b7bafea392b0da8f67131190202c6002e58c2c96b7596'], "*

 * *              "'version': '==6.79.2'}, 'keyring': {'hashes': "*

 * *              "['sha256:ade5e1e7710a7579d7c01e64a712926270239aba48055b1cdc6c022dd6d789b5', "*

 * *              "'sha256:bd48a36612ef55505bf70e563528e3e66ba93267e344b6780cf6151f9c1eda6d'], "*

 * *              "'version': '==24.1. […]*

```diff
@@ -789,19 +789,19 @@
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "version": "==6.0.0"
         },
         "hypothesis": {
             "hashes": [
-                "sha256:7a0b8ca178f16720e96f11e96b71b6139db0e30727e9cf8bd8e3059710393fc7",
-                "sha256:de8fb599fc855d3006236ab58cd0edafd099d63837225aad848dac22e239475b"
+                "sha256:51fb2259489dc446d3edc04cbc8ebd5848d7d3f238121183bee5449b91f7a8d8",
+                "sha256:564d9860ed5e09b0434b7bafea392b0da8f67131190202c6002e58c2c96b7596"
             ],
             "index": "pypi",
-            "version": "==6.79.1"
+            "version": "==6.79.2"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -872,19 +872,19 @@
                 "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==3.1.2"
         },
         "keyring": {
             "hashes": [
-                "sha256:4e87665a19c514c7edada8b15015cf89bd99b8d7edabc5c43cca77166fa8dfad",
-                "sha256:770f609eed2a16c65a6349f3ba1545d00c73f9fed4254c13766c674fe6d0d22b"
+                "sha256:ade5e1e7710a7579d7c01e64a712926270239aba48055b1cdc6c022dd6d789b5",
+                "sha256:bd48a36612ef55505bf70e563528e3e66ba93267e344b6780cf6151f9c1eda6d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==24.0.0"
+            "version": "==24.1.0"
         },
         "lazy-object-proxy": {
             "hashes": [
                 "sha256:09763491ce220c0299688940f8dc2c5d05fd1f45af1e42e636b2e8b2303e4382",
                 "sha256:0a891e4e41b54fd5b8313b96399f8b0e173bbbfc03c7631f01efbe29bb0bcf82",
                 "sha256:189bbd5d41ae7a498397287c408617fe5c48633e7755287b21d741f7db2706a9",
                 "sha256:18b78ec83edbbeb69efdc0e9c1cb41a3b1b1ed11ddd8ded602464c3fc6020494",
@@ -1009,43 +1009,43 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "mypy": {
             "hashes": [
-                "sha256:1c4c42c60a8103ead4c1c060ac3cdd3ff01e18fddce6f1016e08939647a0e703",
-                "sha256:44797d031a41516fcf5cbfa652265bb994e53e51994c1bd649ffcd0c3a7eccbf",
-                "sha256:473117e310febe632ddf10e745a355714e771ffe534f06db40702775056614c4",
-                "sha256:4c99c3ecf223cf2952638da9cd82793d8f3c0c5fa8b6ae2b2d9ed1e1ff51ba85",
-                "sha256:550a8b3a19bb6589679a7c3c31f64312e7ff482a816c96e0cecec9ad3a7564dd",
-                "sha256:658fe7b674769a0770d4b26cb4d6f005e88a442fe82446f020be8e5f5efb2fae",
-                "sha256:6e33bb8b2613614a33dff70565f4c803f889ebd2f859466e42b46e1df76018dd",
-                "sha256:6e42d29e324cdda61daaec2336c42512e59c7c375340bd202efa1fe0f7b8f8ca",
-                "sha256:74bc9b6e0e79808bf8678d7678b2ae3736ea72d56eede3820bd3849823e7f305",
-                "sha256:76ec771e2342f1b558c36d49900dfe81d140361dd0d2df6cd71b3db1be155409",
-                "sha256:7d23370d2a6b7a71dc65d1266f9a34e4cde9e8e21511322415db4b26f46f6b8c",
-                "sha256:87df44954c31d86df96c8bd6e80dfcd773473e877ac6176a8e29898bfb3501cb",
-                "sha256:8c5979d0deb27e0f4479bee18ea0f83732a893e81b78e62e2dda3e7e518c92ee",
-                "sha256:95d8d31a7713510685b05fbb18d6ac287a56c8f6554d88c19e73f724a445448a",
-                "sha256:a22435632710a4fcf8acf86cbd0d69f68ac389a3892cb23fbad176d1cddaf228",
-                "sha256:a8763e72d5d9574d45ce5881962bc8e9046bf7b375b0abf031f3e6811732a897",
-                "sha256:c1eb485cea53f4f5284e5baf92902cd0088b24984f4209e25981cc359d64448d",
-                "sha256:c5d2cc54175bab47011b09688b418db71403aefad07cbcd62d44010543fc143f",
-                "sha256:cbc07246253b9e3d7d74c9ff948cd0fd7a71afcc2b77c7f0a59c26e9395cb152",
-                "sha256:d0b6c62206e04061e27009481cb0ec966f7d6172b5b936f3ead3d74f29fe3dcf",
-                "sha256:ddae0f39ca146972ff6bb4399f3b2943884a774b8771ea0a8f50e971f5ea5ba8",
-                "sha256:e1f4d16e296f5135624b34e8fb741eb0eadedca90862405b1f1fde2040b9bd11",
-                "sha256:e86c2c6852f62f8f2b24cb7a613ebe8e0c7dc1402c61d36a609174f63e0ff017",
-                "sha256:ebc95f8386314272bbc817026f8ce8f4f0d2ef7ae44f947c4664efac9adec929",
-                "sha256:f9dca1e257d4cc129517779226753dbefb4f2266c4eaad610fc15c6a7e14283e",
-                "sha256:faff86aa10c1aa4a10e1a301de160f3d8fc8703b88c7e98de46b531ff1276a9a"
+                "sha256:0cf0ca95e4b8adeaf07815a78b4096b65adf64ea7871b39a2116c19497fcd0dd",
+                "sha256:0f98973e39e4a98709546a9afd82e1ffcc50c6ec9ce6f7870f33ebbf0bd4f26d",
+                "sha256:19d42b08c7532d736a7e0fb29525855e355fa51fd6aef4f9bbc80749ff64b1a2",
+                "sha256:210fe0f39ec5be45dd9d0de253cb79245f0a6f27631d62e0c9c7988be7152965",
+                "sha256:3b1b5c875fcf3e7217a3de7f708166f641ca154b589664c44a6fd6d9f17d9e7e",
+                "sha256:3f2b353eebef669529d9bd5ae3566905a685ae98b3af3aad7476d0d519714758",
+                "sha256:50f65f0e9985f1e50040e603baebab83efed9eb37e15a22a4246fa7cd660f981",
+                "sha256:53c2a1fed81e05ded10a4557fe12bae05b9ecf9153f162c662a71d924d504135",
+                "sha256:5a0ee54c2cb0f957f8a6f41794d68f1a7e32b9968675ade5846f538504856d42",
+                "sha256:62bf18d97c6b089f77f0067b4e321db089d8520cdeefc6ae3ec0f873621c22e5",
+                "sha256:653863c75f0dbb687d92eb0d4bd9fe7047d096987ecac93bb7b1bc336de48ebd",
+                "sha256:67242d5b28ed0fa88edd8f880aed24da481929467fdbca6487167cb5e3fd31ff",
+                "sha256:6ba9a69172abaa73910643744d3848877d6aac4a20c41742027dcfd8d78f05d9",
+                "sha256:6c34d43e3d54ad05024576aef28081d9d0580f6fa7f131255f54020eb12f5352",
+                "sha256:7461469e163f87a087a5e7aa224102a30f037c11a096a0ceeb721cb0dce274c8",
+                "sha256:94a81b9354545123feb1a99b960faeff9e1fa204fce47e0042335b473d71530d",
+                "sha256:a0b2e0da7ff9dd8d2066d093d35a169305fc4e38db378281fce096768a3dbdbf",
+                "sha256:a34eed094c16cad0f6b0d889811592c7a9b7acf10d10a7356349e325d8704b4f",
+                "sha256:a3af348e0925a59213244f28c7c0c3a2c2088b4ba2fe9d6c8d4fbb0aba0b7d05",
+                "sha256:b4c734d947e761c7ceb1f09a98359dd5666460acbc39f7d0a6b6beec373c5840",
+                "sha256:bba57b4d2328740749f676807fcf3036e9de723530781405cc5a5e41fc6e20de",
+                "sha256:ca33ab70a4aaa75bb01086a0b04f0ba8441e51e06fc57e28585176b08cad533b",
+                "sha256:de1e7e68148a213036276d1f5303b3836ad9a774188961eb2684eddff593b042",
+                "sha256:f051ca656be0c179c735a4c3193f307d34c92fdc4908d44fd4516fbe8b10567d",
+                "sha256:f5984a8d13d35624e3b235a793c814433d810acba9eeefe665cdfed3d08bc3af",
+                "sha256:f7a5971490fd4a5a436e143105a1f78fa8b3fe95b30fff2a77542b4f3227a01f"
             ],
             "index": "pypi",
-            "version": "==1.3.0"
+            "version": "==1.4.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -1161,27 +1161,27 @@
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:57e28820ca8094678b807ff529196506d7a21e17156cb1cddb3e74cebce54640",
-                "sha256:ffa199e3fbab8365778c4a10e1fbf1b9cd50707de826eb304b50e57ec0cc8d38"
+                "sha256:b0cabcb11063d21a0b261d557acb0a9d2126350e63b70cdf7db6347baea456dc",
+                "sha256:ca9ed98ce73076ba72e092b23d3c93ea6c4e186b3f1c3dad6edd98ff6ffcca2e"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.6.0"
+            "version": "==3.8.0"
         },
         "pluggy": {
             "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
+                "sha256:c2fd55a7d7a3863cba1a013e4e2414658b1d07b6bc57b3919e0c63c9abb99849",
+                "sha256:d12f0c4b579b15f5e054301bb226ee85eeeba08ffec228092f8defbaa3a4c4b3"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==1.2.0"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "version": "==2.10.0"
@@ -1254,19 +1254,19 @@
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:cdcbd012c9312258922f8cd3f1b62a6580fdced17db6014896053d47cddf9295",
-                "sha256:ee990a3cc55ba808b80795a79944756f315c67c12b56abd3ac993a7b8c17030b"
+                "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
+                "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
-            "version": "==7.3.2"
+            "version": "==7.4.0"
         },
         "pytest-mock": {
             "hashes": [
                 "sha256:21c279fff83d70763b05f8874cc9cfb3fcacd6d354247a976f9529d19f9acf39",
                 "sha256:7f6b125602ac6d743e523ae0bfa71e1a697a2f5534064528c6ff84c2f7c2fc7f"
             ],
             "index": "pypi",
```

### Comparing `blackboardsync-0.9.0a1/README.md` & `blackboardsync-0.9.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/__about__.py` & `blackboardsync-0.9.2rc1/blackboard_sync/__about__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     "__copyright__",
 ]
 
 __title__ = "BlackboardSync"
 __summary__ = "Automatic Syncing Of Your Blackboard Content"
 __uri__ = "https://github.com/jacobszpz/BlackboardSync"
 
-__version__ = "0.9.0-alpha.1"
+__version__ = "0.9.2-rc.1"
 
 __author__ = "Jacob Sánchez"
 __email__ = "jacobszpz@protonmail.com"
 
 __license__ = "GNU General Public License v2"
 __copyright__ = f"2023, {__author__}"
```

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/__init__.py` & `blackboardsync-0.9.2rc1/blackboard_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/__main__.py` & `blackboardsync-0.9.2rc1/blackboard_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/assets/alert.png` & `blackboardsync-0.9.2rc1/blackboard_sync/assets/alert.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/assets/alert.svg` & `blackboardsync-0.9.2rc1/blackboard_sync/assets/alert.svg`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/assets/logo.ico` & `blackboardsync-0.9.2rc1/blackboard_sync/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/assets/logo.png` & `blackboardsync-0.9.2rc1/blackboard_sync/assets/logo.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/assets/watermark.png` & `blackboardsync-0.9.2rc1/blackboard_sync/assets/watermark.png`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/blackboard/__init__.py` & `blackboardsync-0.9.2rc1/blackboard_sync/blackboard/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/blackboard/api.py` & `blackboardsync-0.9.2rc1/blackboard_sync/blackboard/api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/blackboard/blackboard.py` & `blackboardsync-0.9.2rc1/blackboard_sync/blackboard/blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/config.py` & `blackboardsync-0.9.2rc1/blackboard_sync/config.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/download.py` & `blackboardsync-0.9.2rc1/blackboard_sync/download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/institutions.py` & `blackboardsync-0.9.2rc1/blackboard_sync/institutions.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/LoginWebView.ui` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/LoginWebView.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/PersistenceWarning.ui` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/PersistenceWarning.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/SettingsWindow.ui` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/SettingsWindow.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/SetupWizard.ui` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/SetupWizard.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/UniNotSupportedDialog.ui` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/UniNotSupportedDialog.ui`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/__init__.py` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/qt/qt_elements.py` & `blackboardsync-0.9.2rc1/blackboard_sync/qt/qt_elements.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/sync.py` & `blackboardsync-0.9.2rc1/blackboard_sync/sync.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/sync_controller.py` & `blackboardsync-0.9.2rc1/blackboard_sync/sync_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         self.app.setOverrideCursor(Qt.WaitCursor)
         # Call login function on sync
         auth = self.model.auth(self.login_window.cookie_jar)
         self.tray.set_logged_in(auth)
         self.login_window.setVisible(False)
         self.app.restoreOverrideCursor()
         self._check_for_updates()
-        self.tray.show_msg('BlackboardSync is running', 'You can always find it in the system tray')
+        self.tray.show_msg('The download has started', 'BlackboardSync is running in the background. Find it in the system tray.')
 
     def _check_for_updates(self) -> None:
         if (html_url := check_for_updates()) is not None:
             if UpdateFoundDialog().update:
                 webbrowser.open(html_url)
 
     def _show_login_window(self) -> None:
```

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/updates.py` & `blackboardsync-0.9.2rc1/blackboard_sync/updates.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboard_sync/webdav.py` & `blackboardsync-0.9.2rc1/blackboard_sync/webdav.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/blackboardsync.egg-info/PKG-INFO` & `blackboardsync-0.9.2rc1/blackboardsync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blackboardsync
-Version: 0.9.0a1
+Version: 0.9.2rc1
 Summary: Sync your blackboard content to your device
 Author-email: Jacob Sánchez <jacobszpz@protonmail.com>
 Project-URL: Homepage, https://bbsync.app
 Project-URL: Repository, https://github.com/jacobszpz/BlackboardSync
 Project-URL: Bug Tracker, https://github.com/jacobszpz/BlackboardSync/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `blackboardsync-0.9.0a1/blackboardsync.egg-info/SOURCES.txt` & `blackboardsync-0.9.2rc1/blackboardsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/docs/Makefile` & `blackboardsync-0.9.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/docs/conf.py` & `blackboardsync-0.9.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/docs/index.rst` & `blackboardsync-0.9.2rc1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/docs/make.bat` & `blackboardsync-0.9.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/main.py` & `blackboardsync-0.9.2rc1/main.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/packaging/pkg_macos.sh` & `blackboardsync-0.9.2rc1/packaging/pkg_macos.sh`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/packaging/pkg_win.nsi` & `blackboardsync-0.9.2rc1/packaging/pkg_win.nsi`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/packaging/pyinst.py` & `blackboardsync-0.9.2rc1/packaging/pyinst.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/pyproject.toml` & `blackboardsync-0.9.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/strategies.py` & `blackboardsync-0.9.2rc1/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/test_api.py` & `blackboardsync-0.9.2rc1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/test_blackboard.py` & `blackboardsync-0.9.2rc1/tests/test_blackboard.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/test_download.py` & `blackboardsync-0.9.2rc1/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/test_qt.py` & `blackboardsync-0.9.2rc1/tests/test_qt.py`

 * *Files identical despite different names*

### Comparing `blackboardsync-0.9.0a1/tests/test_sync_config.py` & `blackboardsync-0.9.2rc1/tests/test_sync_config.py`

 * *Files identical despite different names*

