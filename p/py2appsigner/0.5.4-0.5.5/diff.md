# Comparing `tmp/py2appsigner-0.5.4.tar.gz` & `tmp/py2appsigner-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py2appsigner-0.5.4.tar", last modified: Fri Jun 23 20:15:50 2023, max compression
+gzip compressed data, was "py2appsigner-0.5.5.tar", last modified: Sun Jun 25 20:41:32 2023, max compression
```

## Comparing `py2appsigner-0.5.4.tar` & `py2appsigner-0.5.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-23 20:15:50.036314 py2appsigner-0.5.4/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.4/LICENSE
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-23 20:15:50.036185 py2appsigner-0.5.4/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.4/README.md
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-23 20:15:50.034170 py2appsigner-0.5.4/py2appsigner/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.4/py2appsigner/ApplicationNotarize.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6794 2023-06-21 20:24:26.000000 py2appsigner-0.5.4/py2appsigner/ApplicationSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.4/py2appsigner/ApplicationStaple.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.4/py2appsigner/ApplicationVerify.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1222 2023-06-20 13:59:01.000000 py2appsigner-0.5.4/py2appsigner/BaseCommand.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.4/py2appsigner/CommandBasic.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      826 2023-06-20 03:50:35.000000 py2appsigner-0.5.4/py2appsigner/CommandExtended.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10146 2023-06-21 20:49:22.000000 py2appsigner-0.5.4/py2appsigner/Commands.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.4/py2appsigner/Common.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.4/py2appsigner/Notary.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6233 2023-06-20 03:49:22.000000 py2appsigner-0.5.4/py2appsigner/ZipSign.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.4/py2appsigner/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-06-21 19:37:48.000000 py2appsigner-0.5.4/py2appsigner/_version.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-23 20:15:50.035761 py2appsigner-0.5.4/py2appsigner/environment/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.4/py2appsigner/environment/BasicEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.4/py2appsigner/environment/Environment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.4/py2appsigner/environment/NotaryEnvironment.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.4/py2appsigner/environment/__init__.py
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-23 20:15:50.035962 py2appsigner-0.5.4/py2appsigner/resources/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.4/py2appsigner/resources/__init__.py
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.4/py2appsigner/resources/loggingConfiguration.json
-drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-23 20:15:50.034939 py2appsigner-0.5.4/py2appsigner.egg-info/
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/PKG-INFO
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/SOURCES.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/dependency_links.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/entry_points.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/requires.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-23 20:15:50.000000 py2appsigner-0.5.4/py2appsigner.egg-info/top_level.txt
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-23 20:15:50.036344 py2appsigner-0.5.4/setup.cfg
--rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.4/setup.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-25 20:41:32.127972 py2appsigner-0.5.5/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    34523 2023-05-17 20:07:47.000000 py2appsigner-0.5.5/LICENSE
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-25 20:41:32.127838 py2appsigner-0.5.5/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     4408 2023-06-19 21:06:01.000000 py2appsigner-0.5.5/README.md
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-25 20:41:32.125577 py2appsigner-0.5.5/py2appsigner/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2595 2023-06-03 20:42:54.000000 py2appsigner-0.5.5/py2appsigner/ApplicationNotarize.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     7363 2023-06-24 23:58:12.000000 py2appsigner-0.5.5/py2appsigner/ApplicationSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      711 2023-06-02 20:02:20.000000 py2appsigner-0.5.5/py2appsigner/ApplicationStaple.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      505 2023-06-02 20:02:20.000000 py2appsigner-0.5.5/py2appsigner/ApplicationVerify.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1222 2023-06-20 13:59:01.000000 py2appsigner-0.5.5/py2appsigner/BaseCommand.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1758 2023-06-03 17:59:25.000000 py2appsigner-0.5.5/py2appsigner/CommandBasic.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      826 2023-06-20 03:50:35.000000 py2appsigner-0.5.5/py2appsigner/CommandExtended.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    10557 2023-06-24 23:55:05.000000 py2appsigner-0.5.5/py2appsigner/Commands.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      113 2023-06-03 20:21:23.000000 py2appsigner-0.5.5/py2appsigner/Common.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2316 2023-06-19 20:48:07.000000 py2appsigner-0.5.5/py2appsigner/Notary.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     6233 2023-06-20 03:49:22.000000 py2appsigner-0.5.5/py2appsigner/ZipSign.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       46 2023-05-17 20:18:22.000000 py2appsigner-0.5.5/py2appsigner/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       22 2023-06-25 20:40:13.000000 py2appsigner-0.5.5/py2appsigner/_version.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-25 20:41:32.127399 py2appsigner-0.5.5/py2appsigner/environment/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     2094 2023-05-31 01:40:56.000000 py2appsigner-0.5.5/py2appsigner/environment/BasicEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1519 2023-06-03 20:04:40.000000 py2appsigner-0.5.5/py2appsigner/environment/Environment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      219 2023-06-04 22:46:26.000000 py2appsigner-0.5.5/py2appsigner/environment/NotaryEnvironment.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-02 19:06:14.000000 py2appsigner-0.5.5/py2appsigner/environment/__init__.py
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-25 20:41:32.127603 py2appsigner-0.5.5/py2appsigner/resources/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-05-17 20:20:16.000000 py2appsigner-0.5.5/py2appsigner/resources/__init__.py
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      854 2023-05-19 16:43:35.000000 py2appsigner-0.5.5/py2appsigner/resources/loggingConfiguration.json
+drwxr-xr-x   0 humberto.a.sanchez.ii   (501) staff       (20)        0 2023-06-25 20:41:32.126314 py2appsigner-0.5.5/py2appsigner.egg-info/
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)    44603 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/PKG-INFO
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      866 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/SOURCES.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)        1 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/dependency_links.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)      246 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/entry_points.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       26 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/requires.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       13 2023-06-25 20:41:32.000000 py2appsigner-0.5.5/py2appsigner.egg-info/top_level.txt
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)       38 2023-06-25 20:41:32.128008 py2appsigner-0.5.5/setup.cfg
+-rw-r--r--   0 humberto.a.sanchez.ii   (501) staff       (20)     1363 2023-06-04 22:36:05.000000 py2appsigner-0.5.5/setup.py
```

### Comparing `py2appsigner-0.5.4/LICENSE` & `py2appsigner-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/PKG-INFO` & `py2appsigner-0.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.4
+Version: 0.5.5
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.4/README.md` & `py2appsigner-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/ApplicationNotarize.py` & `py2appsigner-0.5.5/py2appsigner/ApplicationNotarize.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/ApplicationSign.py` & `py2appsigner-0.5.5/py2appsigner/ApplicationSign.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,40 +45,50 @@
 MACH_OBJECT_DYNAMIC_LIBRARY_WILDCARD: str = '*.dylib'
 
 PRE_FRAMEWORK_PATH: str = '/Contents/Frameworks/Python.framework/Versions'
 
 
 class ApplicationSign(CommandExtended):
 
-    def __init__(self, environment: Environment, fixLib: bool):
+    def __init__(self, environment: Environment, fixLib: bool, fixSymLink: bool):
 
         super().__init__(environment=environment)
         self.logger: Logger = getLogger(__name__)
 
-        self._fixLib: bool = fixLib
+        self._fixLib:     bool = fixLib
+        self._fixSymLink: bool = fixSymLink
 
         self._codeSignCommand: str = self._constructCodeSignCommand()
 
     def execute(self):
 
         self._fixLibrary()
+        self._fixSymbolicLink()
         self._cleanupCrud()
         self._signFrameworks()
         self._signLibraries()
         self._signPythonApp()
         self._signApplication()
 
     def _fixLibrary(self):
 
         if self._fixLib is True:
             directoryToOverWrite: str = f'{self._applicationName}/Contents/Frameworks'
             options: str = self._getToolOptions(verboseOptions=COPY_OPTIONS_VERBOSE, quietOptions=COPY_OPTIONS_QUIET)
             overwrite: str = f'cp {options} {GOOD_LIB} {directoryToOverWrite}'
             self._runCommand(overwrite)
 
+    def _fixSymbolicLink(self):
+        if self._fixSymLink is True:
+            linkToRemove: str = f'{self._applicationName}/Contents/Resources/lib/python{self._pythonVersion}/site.pyo '
+            options:      str = self._getToolOptions(verboseOptions=REMOVE_OPTIONS_VERBOSE,
+                                                     quietOptions=REMOVE_OPTIONS_QUIET)
+            remove:       str  = f'rm {options} {linkToRemove}'
+            self._runCommand(remove)
+
     def _cleanupCrud(self):
         """
         Ugh code signing will be the death of me
         Either invalid links or something code signing or verifying complains about
         """
         removeOptions: str = self._getToolOptions(verboseOptions=REMOVE_OPTIONS_VERBOSE, quietOptions=REMOVE_OPTIONS_QUIET)
         for partialCrud in CLEAN_UP_CRUD:
```

### Comparing `py2appsigner-0.5.4/py2appsigner/ApplicationStaple.py` & `py2appsigner-0.5.5/py2appsigner/ApplicationStaple.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/BaseCommand.py` & `py2appsigner-0.5.5/py2appsigner/BaseCommand.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/CommandBasic.py` & `py2appsigner-0.5.5/py2appsigner/CommandBasic.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/CommandExtended.py` & `py2appsigner-0.5.5/py2appsigner/CommandExtended.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/Commands.py` & `py2appsigner-0.5.5/py2appsigner/Commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,34 +94,42 @@
 def zipSign(environment: Environment):
 
     zipsign: ZipSign = ZipSign(environment=environment)
     zipsign.execute()
 
 
 @py2appSign.command()
-@option('--fix-lib', '-f', required=False, is_flag=True, help='Fix broken library ')
+@option('--fix-lib',      '-l', required=False, is_flag=True, help='Fix broken library')
+@option('--fix-sym-link', '-s', required=False, is_flag=True, help='Fix invalid symbolic link')
 @pass_obj
-def appSign(environment: Environment, fix_lib: bool = False):
-    # noinspection SpellCheckingInspection
+def appSign(environment: Environment, fix_lib: bool = False, fix_sym_link: bool = False):
     """
     fix-lib gets the following dynamic library from Homebrew;  And copies it into the
     Python virtual environment;  Works only on Apple Silicon OS X
     and with Homebrew installed
 
     See: https://stackoverflow.com/questions/62095338/py2app-fails-macos-signing-on-liblzma-5-dylib
 
     On Intel OS X
 
     /usr/local/Cellar/xz/5.2.5/lib/liblzma.5.dylib
 
     Apple Silicon
 
     /opt/homebrew/opt/xz/lib/liblzma.5.dylib
+
+    -fix-sym-link remove the following symbolic link from the application binary before signing
+
+     <application>.app/Contents/Resources/lib/python<python version>/site.pyo
+
+     Leaving this file in place with a signed and notarized application causes it to
+     fail the appVerify phase and renders the binary unusable
+
     """
-    applicationSign: ApplicationSign = ApplicationSign(environment=environment, fixLib=fix_lib)
+    applicationSign: ApplicationSign = ApplicationSign(environment=environment, fixLib=fix_lib, fixSymLink=fix_sym_link)
     applicationSign.execute()
 
 
 @command
 @version_option(version=f'{version}', message='%(prog)s version %(version)s')
 @option('--application-name',  '-a', required=True,  help='The application name that py2app built')
 @option('--projects-base',     '-b', required=False, help='Projects base, overrides environment variable')
@@ -228,8 +236,8 @@
     py2appSign(['--python-version', '3.10', '-d', 'pyut', '--application-name', 'pyut', 'zipsign'])
     py2appSign(['--python-version', '3.10', '-d', 'pyut', '--application-name', 'pyut', 'appsign'])
     appNotarize(['-d', 'pyut', '--application-name', 'pyut', '--verbose'])
     appStaple(['-d', 'pyut', '--application-name', 'pyut', '--verbose'])
     notaryTool(['information', '-i', '5f57fc1e-23d3-42ab-b0ad-ec1d2635c4ad'])
     notaryTool(['--keychain-profile', 'NOTARY_TOOL_APP_ID', 'history'])
     """
-    py2appSign(['--python-version', '3.11', '-d', 'pyut', '--application-name', 'pyut', '--verbose', 'appsign'])
+    py2appSign(['-p', '3.11', '-d', 'pyut', '-a', 'pyut', '--verbose', 'appsign', '-s'])
```

### Comparing `py2appsigner-0.5.4/py2appsigner/Notary.py` & `py2appsigner-0.5.5/py2appsigner/Notary.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/ZipSign.py` & `py2appsigner-0.5.5/py2appsigner/ZipSign.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/environment/BasicEnvironment.py` & `py2appsigner-0.5.5/py2appsigner/environment/BasicEnvironment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/environment/Environment.py` & `py2appsigner-0.5.5/py2appsigner/environment/Environment.py`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner/resources/loggingConfiguration.json` & `py2appsigner-0.5.5/py2appsigner/resources/loggingConfiguration.json`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/py2appsigner.egg-info/PKG-INFO` & `py2appsigner-0.5.5/py2appsigner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py2appsigner
-Version: 0.5.4
+Version: 0.5.5
 Summary: Scripts to Code Sign py2app applications
 Home-page: https://github.com/py2appsigner
 Author: Humberto A. Sanchez II
 Author-email: humberto.a.sanchez.ii@gmail.com
 Maintainer: Humberto A. Sanchez II
 Maintainer-email: humberto.a.sanchez.ii@gmail.com
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
```

### Comparing `py2appsigner-0.5.4/py2appsigner.egg-info/SOURCES.txt` & `py2appsigner-0.5.5/py2appsigner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py2appsigner-0.5.4/setup.py` & `py2appsigner-0.5.5/setup.py`

 * *Files identical despite different names*

