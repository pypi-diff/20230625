# Comparing `tmp/mciplayer-2.0.1.tar.gz` & `tmp/mciplayer-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mciplayer-2.0.1.tar", last modified: Tue Jun 13 10:09:52 2023, max compression
+gzip compressed data, was "mciplayer-2.0.2.tar", last modified: Sun Jun 25 09:04:21 2023, max compression
```

## Comparing `mciplayer-2.0.1.tar` & `mciplayer-2.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.376503 mciplayer-2.0.1/
--rw-rw-rw-   0        0        0      930 2023-06-13 10:09:52.375021 mciplayer-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      778 2023-06-13 08:49:45.000000 mciplayer-2.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.368810 mciplayer-2.0.1/mciplayer/
--rw-rw-rw-   0        0        0     8256 2023-06-13 08:47:19.000000 mciplayer-2.0.1/mciplayer/__init__.py
--rw-rw-rw-   0        0        0      856 2023-06-13 08:44:46.000000 mciplayer-2.0.1/mciplayer/tool.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:09:52.375021 mciplayer-2.0.1/mciplayer.egg-info/
--rw-rw-rw-   0        0        0      930 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 10:09:52.000000 mciplayer-2.0.1/mciplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5112 2023-06-13 10:07:23.000000 mciplayer-2.0.1/py_mciwnd.cpp
--rw-rw-rw-   0        0        0     5676 2023-06-13 10:07:42.000000 mciplayer-2.0.1/py_mciwnd_unicode.cpp
--rw-rw-rw-   0        0        0       42 2023-06-13 10:09:52.377506 mciplayer-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1025 2023-06-13 10:08:38.000000 mciplayer-2.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:04:21.264797 mciplayer-2.0.2/
+-rw-rw-rw-   0        0        0      930 2023-06-25 09:04:21.264797 mciplayer-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-06-13 08:49:45.000000 mciplayer-2.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-25 09:04:21.259363 mciplayer-2.0.2/mciplayer/
+-rw-rw-rw-   0        0        0     9348 2023-06-25 08:54:32.000000 mciplayer-2.0.2/mciplayer/__init__.py
+-rw-rw-rw-   0        0        0      856 2023-06-13 08:44:46.000000 mciplayer-2.0.2/mciplayer/tool.py
+drwxrwxrwx   0        0        0        0 2023-06-25 09:04:21.263791 mciplayer-2.0.2/mciplayer.egg-info/
+-rw-rw-rw-   0        0        0      930 2023-06-25 09:04:21.000000 mciplayer-2.0.2/mciplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-06-25 09:04:21.000000 mciplayer-2.0.2/mciplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 09:04:21.000000 mciplayer-2.0.2/mciplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-06-25 09:04:21.000000 mciplayer-2.0.2/mciplayer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 09:04:21.000000 mciplayer-2.0.2/mciplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5681 2023-06-25 08:23:44.000000 mciplayer-2.0.2/py_mciwnd.cpp
+-rw-rw-rw-   0        0        0     6495 2023-06-25 08:43:08.000000 mciplayer-2.0.2/py_mciwnd_unicode.cpp
+-rw-rw-rw-   0        0        0       42 2023-06-25 09:04:21.264797 mciplayer-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1025 2023-06-25 09:02:39.000000 mciplayer-2.0.2/setup.py
```

### Comparing `mciplayer-2.0.1/PKG-INFO` & `mciplayer-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-2.0.1/README.md` & `mciplayer-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mciplayer-2.0.1/mciplayer/__init__.py` & `mciplayer-2.0.2/mciplayer/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -99,43 +99,55 @@
     def length(self):
         """
         Returns the length of the audio (in milliseconds).
         It is also possible to use self.start()-self.end() to get the same thing.
         """
         return MCIWndGetLength(self.wnd) if not self.use_utf8 else uMCIWndGetLength(self.wnd)
     @mciplayermethod
-    def save(self,filename):
+    def save(self,filename=None):
         """
         Saves the audio in the player.
         """
-        if not MCIWndCanSave(self.wnd):
-            raise SupportError('Save is unsupported for this MCI Window')
-        if not filename.endswith('.wav'):
-            raise SupportError('save() supports only wave audio.')
-        cwd=os.getcwd()
-        os.chdir(os.environ['TMP'])
-        dn=str(uuid4())
-        os.mkdir(dn)
-        os.chdir(dn)
-        if self.use_utf8:
-            uMCIWndSave(self.wnd,b'a')
-        else:
-            MCIWndSave(self.wnd,b'a')
-        self._audios.append(dn)
-        os.chdir(cwd)
-        self._names.append(os.path.abspath(filename))
+        if filename is not None:
+            if not MCIWndCanSave(self.wnd):
+                raise SupportError('Save is unsupported for this MCI Window')
+            if not filename.endswith('.wav'):
+                raise SupportError('save() supports only wave audio.')
+            cwd=os.getcwd()
+            os.chdir(os.environ['TMP'])
+            dn=str(uuid4())
+            os.mkdir(dn)
+            os.chdir(dn)
+            if self.use_utf8:
+                uMCIWndSave(self.wnd,b'a')
+            else:
+                MCIWndSave(self.wnd,b'a')
+            self._audios.append(dn)
+            os.chdir(cwd)
+            self._names.append(os.path.abspath(filename))
+        else:
+            if self.use_utf8:
+                uMCIWndSaveDialog(self.wnd)
+            else:
+                MCIWndSaveDialog(self.wnd)
     @mciplayermethod
-    def open(self,fn):
+    def open(self,fn=None):
         """
         Open a new audio file
         """
-        if self.use_utf8:
-            uMCIWndOpen(self.wnd,fn.encode('utf-8'),0)
-        else:
-            MCIWndOpen(self.wnd,fn.encode('ansi'),0)
+        if fn is not None:
+            if self.use_utf8:
+                uMCIWndOpen(self.wnd,fn.encode('utf-8'),0)
+            else:
+                MCIWndOpen(self.wnd,fn.encode('ansi'),0)
+        else:
+            if self.use_utf8:
+                uMCIWndOpenDialog(self.wnd)
+            else:
+                MCIWndOpenDialog(self.wnd)
     @mciplayermethod
     def enable_record(self):
         """
         Enables recording.
         """
         if self.use_utf8:
             uMCIWndNew(self.wnd,b'waveaudio')
@@ -218,14 +230,34 @@
     @mciplayermethod
     def wait(self):
         """
         Waits until the player finishes playing current audio.
         """
         while self.position()<self.end():
             pass
+    @property
+    @mciplayermethod
+    def filename(self):
+        """
+        The file name which the player is playing currently
+        """
+        if self.use_utf8:
+            return uMCIWndGetFileName(self.wnd)
+        else:
+            return MCIWndGetFileName(self.wnd)
+    @property
+    @mciplayermethod
+    def status(self):
+        """
+        The status of the player, can be one of 'not ready', 'opened', 'paused', 'playing', 'recording', 'seeking', 'stopped'
+        """
+        if self.use_utf8:
+            return uMCIWndGetMode(self.wnd)
+        else:
+            return MCIWndGetMode(self.wnd)
     def __del__(self):
         """
         Close the player before deletion.
         """
         self.close()
 def _play_demo():
     """
```

### Comparing `mciplayer-2.0.1/mciplayer/tool.py` & `mciplayer-2.0.2/mciplayer/tool.py`

 * *Files identical despite different names*

### Comparing `mciplayer-2.0.1/mciplayer.egg-info/PKG-INFO` & `mciplayer-2.0.2/mciplayer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mciplayer
-Version: 2.0.1
+Version: 2.0.2
 Summary: A simple audio player/recorder using MCI
 Description-Content-Type: text/markdown
 
 <p><span><span style="font-family:Verdana, Arial, Helvetica, sans-serif;line-height:19px;text-indent:26px;"><span style="font-size:14px;"><span style="font-family:Arial;line-height:26px;"><br></span></span></span></span></p>
 
 ### This package should be built AND installed in Windows
```

### Comparing `mciplayer-2.0.1/py_mciwnd.cpp` & `mciplayer-2.0.2/py_mciwnd.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -104,14 +104,30 @@
     unsigned dwStyle
 ) {
     return (int)MCIWndCreate((HWND)hwndParent, (HINSTANCE)hInstance, dwStyle, 0);
 }
 int mwt(int hwnd) {
     return MCIWndStop((HWND)hwnd);
 }
+int mwod(int hwnd) {
+    return MCIWndOpenDialog((HWND)hwnd);
+}
+int mwsd(int hwnd) {
+    return MCIWndSaveDialog((HWND)hwnd);
+}
+py::bytes mwgfn(int hwnd) {
+    char *c = new char[1024];
+    MCIWndGetFileName((HWND)hwnd, c, 1024);
+    return py::bytes(c);
+}
+py::bytes mwgm(int hwnd) {
+    char* c = new char[1024];
+    MCIWndGetMode((HWND)hwnd, c, 1024);
+    return py::bytes(c[0]?c:"not ready");
+}
 PYBIND11_MODULE(_mciwnd, m) {
     m.def("MCIWndCreate", &mwc);
     m.def("MCIWndCreateNull", &mwcn);
     m.def("MCIWndPlay", &mwp);
     m.def("MCIWndPause", &mwp_);
     m.def("MCIWndResume", &mwr);
     m.def("MCIWndGetStart", &mwgs);
@@ -131,14 +147,18 @@
     m.def("MCIWndCanSave", &mwcs);
     m.def("MCIWndSeek", &mwsk);
     m.def("MCIWndOpen", &mwo);
     m.def("MCIWndGetError", &mwer);
     m.def("MCIWndClose", &mwcl);
     m.def("MCIWndNew", &mwn);
     m.def("MCIWndStop", &mwt);
+    m.def("MCIWndGetMode", &mwgm);
+    m.def("MCIWndOpenDialog", &mwod);
+    m.def("MCIWndSaveDialog", &mwsd);
+    m.def("MCIWndGetFileName", &mwgfn);
     m.attr("WS_OVERLAPPED") = 0x00000000L;
     m.attr("WS_POPUP") = 0x80000000L;
     m.attr("WS_CHILD") = 0x40000000L;
     m.attr("WS_MINIMIZE") = 0x20000000L;
     m.attr("WS_VISIBLE") = 0x10000000L;
     m.attr("WS_DISABLED") = 0x08000000L;
     m.attr("WS_CLIPSIBLINGS") = 0x04000000L;
```

### Comparing `mciplayer-2.0.1/py_mciwnd_unicode.cpp` & `mciplayer-2.0.2/py_mciwnd_unicode.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -115,14 +115,36 @@
     unsigned dwStyle
 ) {
     return (int)MCIWndCreate((HWND)hwndParent, (HINSTANCE)hInstance, dwStyle, 0);
 }
 int mwt(int hwnd) {
     return MCIWndStop((HWND)hwnd);
 }
+py::bytes mwgfn(int hwnd) {
+    wchar_t* c = new wchar_t[1024];
+    char* tmp = new char[1024];
+    MCIWndGetFileName((HWND)hwnd, c, 1024);
+    WideCharToMultiByte(CP_UTF8, 0, c, 1024, tmp, 1024, 0, 0);
+    delete[] c;
+    return py::bytes(tmp);
+}
+py::bytes mwgm(int hwnd) {
+    wchar_t* c = new wchar_t[1024];
+    char* tmp = new char[1024];
+    MCIWndGetMode((HWND)hwnd, c, 1024);
+    WideCharToMultiByte(CP_UTF8, 0, c, 1024, tmp, 1024, 0, 0);
+    delete[] c;
+    return py::bytes(tmp[0]?tmp:"not ready");
+}
+int mwod(int hwnd) {
+    return MCIWndOpenDialog((HWND)hwnd);
+}
+int mwsd(int hwnd) {
+    return MCIWndSaveDialog((HWND)hwnd);
+}
 PYBIND11_MODULE(_mciwnd_unicode, m) {
     m.def("uMCIWndCreate", &mwc);
     m.def("uMCIWndCreateNull", &mwcn);
     m.def("uMCIWndPlay", &mwp);
     m.def("uMCIWndPause", &mwp_);
     m.def("uMCIWndResume", &mwr);
     m.def("uMCIWndGetStart", &mwgs);
@@ -142,14 +164,18 @@
     m.def("uMCIWndCanSave", &mwcs);
     m.def("uMCIWndSeek", &mwsk);
     m.def("uMCIWndOpen", &mwo);
     m.def("uMCIWndGetError", &mwer);
     m.def("uMCIWndClose", &mwcl);
     m.def("uMCIWndNew", &mwn);
     m.def("uMCIWndStop", &mwt);
+    m.def("uMCIWndGetFileName", &mwgfn);
+    m.def("uMCIWndGetMode", &mwgm);
+    m.def("uMCIWndOpenDialog", &mwod);
+    m.def("uMCIWndSaveDialog", &mwsd);
     m.attr("WS_OVERLAPPED") = 0x00000000L;
     m.attr("WS_POPUP") = 0x80000000L;
     m.attr("WS_CHILD") = 0x40000000L;
     m.attr("WS_MINIMIZE") = 0x20000000L;
     m.attr("WS_VISIBLE") = 0x10000000L;
     m.attr("WS_DISABLED") = 0x08000000L;
     m.attr("WS_CLIPSIBLINGS") = 0x04000000L;
```

### Comparing `mciplayer-2.0.1/setup.py` & `mciplayer-2.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md','r') as file:
         return file.read()
 if platform.system()!='Windows': # Must be a Windows operating system.
     raise OSError("Please build in Windows!")
 else:
     setup(
         name='mciplayer',
-        version='2.0.1',
+        version='2.0.2',
         description='A simple audio player/recorder using MCI',
         long_description_content_type='text/markdown',
         ext_modules=[
             Extension('mciplayer._mciwnd',sources=['py_mciwnd.cpp'],include_dirs=[get_include()],language='c++'),
             Extension('mciplayer._mciwnd_unicode',sources=['py_mciwnd_unicode.cpp'],include_dirs=[get_include()],language='c++')
         ],
         packages=['mciplayer'],long_description=readme(),
```

