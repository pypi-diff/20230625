# Comparing `tmp/eFatura-1.0.9.tar.gz` & `tmp/eFatura-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eFatura-1.0.9.tar", last modified: Sun Jun 25 09:35:04 2023, max compression
+gzip compressed data, was "eFatura-1.1.0.tar", last modified: Sun Jun 25 09:42:38 2023, max compression
```

## Comparing `eFatura-1.0.9.tar` & `eFatura-1.1.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 09:34:31.000000 eFatura-1.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:35:04.117894 eFatura-1.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-25 09:34:31.000000 eFatura-1.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.113893 eFatura-1.0.9/Shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-25 09:34:31.000000 eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.appdata.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 09:34:31.000000 eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.desktop
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 09:34:31.000000 eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.113893 eFatura-1.0.9/eFatura/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/eFatura/Assets/
--rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/Assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/eFatura/Core/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/eFatura/GUI/
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/GUI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/eFatura/Libs/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/Libs/Oturum.py
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/Libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/arayuz.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 09:34:31.000000 eFatura-1.0.9/eFatura/konsol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:35:04.117894 eFatura-1.0.9/eFatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:35:04.000000 eFatura-1.0.9/eFatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:35:04.121894 eFatura-1.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-25 09:34:31.000000 eFatura-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-25 09:42:10.000000 eFatura-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:42:38.022216 eFatura-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6358 2023-06-25 09:42:10.000000 eFatura-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.018216 eFatura-1.1.0/Shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.desktop
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-25 09:42:10.000000 eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.018216 eFatura-1.1.0/eFatura/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    25470 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/GUI/
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/GUI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura/Libs/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Libs/Oturum.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/Libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/arayuz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-25 09:42:10.000000 eFatura-1.1.0/eFatura/konsol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 09:42:38.022216 eFatura-1.1.0/eFatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-25 09:42:38.000000 eFatura-1.1.0/eFatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 09:42:38.022216 eFatura-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-25 09:42:10.000000 eFatura-1.1.0/setup.py
```

### Comparing `eFatura-1.0.9/PKG-INFO` & `eFatura-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.9
+Version: 1.1.0
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.9 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.1.0 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.0.9/README.md` & `eFatura-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml`

 * *Files 1% similar despite different names*

#### Comparing `eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.appdata.xml` & `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.appdata.xml`

```diff
@@ -28,15 +28,15 @@
       <image>https://raw.githubusercontent.com/keyiflerolsun/eFatura/main/.github/icons/SS.png</image>
     </screenshot>
   </screenshots>
   <categories>
     <category>Education</category>
   </categories>
   <releases>
-    <release version="1.0.9" date="2023-6-25">
+    <release version="1.1.0" date="2023-6-25">
       <description>
         <p>Çeşitli iyileştirmeler yapıldı..</p>
       </description>
     </release>
     <release version="1.0.5" date="2023-5-23"/>
     <release version="0.0.1" date="2022-8-13"/>
   </releases>
```

### Comparing `eFatura-1.0.9/Shared/org.KekikAkademi.eFatura.svg` & `eFatura-1.1.0/Shared/org.KekikAkademi.eFatura.svg`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/eFatura/Assets/logo.png` & `eFatura-1.1.0/eFatura/Assets/logo.png`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/eFatura/Core/__init__.py` & `eFatura-1.1.0/eFatura/Core/__init__.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/eFatura/GUI/__init__.py` & `eFatura-1.1.0/eFatura/GUI/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -105,24 +105,21 @@
     def ara_butonuna_tiklandiginda(self, widget):
         self.ara_butonu.grab_focus()
         arama_sorgusu = self.arama_metni.get_text()
         self.arama_metni.set_text("")
 
         self.cikti_alani.foreach(Gtk.Widget.destroy)
 
-        bekleme_etiketi = Gtk.Label(
-            label           = "Lütfen Bekleyiniz...",
-            markup          = "<span foreground='#EF7F1A' font_desc='12'>Lütfen Bekleyiniz...</span>",
-            use_markup      = True,
-            margin_top      = 10,
-            halign          = Gtk.Align.CENTER,
-            justify         = Gtk.Justification.CENTER,
-            line_wrap       = True,
-            max_width_chars = 30
-        )
+        bekleme_etiketi = Gtk.Label()
+        bekleme_etiketi.set_markup("<span foreground='#EF7F1A' font_desc='12'>Lütfen Bekleyiniz...</span>")
+        bekleme_etiketi.set_margin_top(10)
+        bekleme_etiketi.set_halign(Gtk.Align.CENTER)
+        bekleme_etiketi.set_justify(Gtk.Justification.CENTER)
+        bekleme_etiketi.set_line_wrap(True)
+        bekleme_etiketi.set_max_width_chars(30)
         self.cikti_alani.pack_start(bekleme_etiketi, False, False, 0)
         self.parent.show_all()
 
         def arama_tamamlandi():
             sonuc = e_fatura(arama_sorgusu)
             if sonuc:
                 bekleme_etiketi.set_markup(f"<span foreground='#17a2b8' font_desc='12'>{arama_sorgusu} Numarası\nE-Fatura Mükellefidir..</span>")
```

### Comparing `eFatura-1.0.9/eFatura/Libs/Oturum.py` & `eFatura-1.1.0/eFatura/Libs/Oturum.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/eFatura/konsol.py` & `eFatura-1.1.0/eFatura/konsol.py`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/eFatura.egg-info/PKG-INFO` & `eFatura-1.1.0/eFatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eFatura
-Version: 1.0.9
+Version: 1.1.0
 Summary: Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu
 Home-page: https://github.com/keyiflerolsun/eFatura
 Author: keyiflerolsun
 Author-email: keyiflerolsun@gmail.com
 License: GPLv3+
 Keywords: eFatura,KekikAkademi,keyiflerolsun
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: eFatura Version: 1.0.9 Summary: Vergi veya TC
+Metadata-Version: 2.1 Name: eFatura Version: 1.1.0 Summary: Vergi veya TC
 Kimlik NumarasÄ±ndan E-Fatura MÃ¼kellefiyet Sorgusu Home-page: https://
 github.com/keyiflerolsun/eFatura Author: keyiflerolsun Author-email:
 keyiflerolsun@gmail.com License: GPLv3+ Keywords:
 eFatura,KekikAkademi,keyiflerolsun Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10 Description-Content-Type: text/markdown # [https://
```

### Comparing `eFatura-1.0.9/eFatura.egg-info/SOURCES.txt` & `eFatura-1.1.0/eFatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eFatura-1.0.9/setup.py` & `eFatura-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from io         import open
 
 setup(
     # ? Genel Bilgiler
     name         = "eFatura",
-    version      = "1.0.9",
+    version      = "1.1.0",
     url          = "https://github.com/keyiflerolsun/eFatura",
     description  = "Vergi veya TC Kimlik Numarasından E-Fatura Mükellefiyet Sorgusu",
     keywords     = ["eFatura", "KekikAkademi", "keyiflerolsun"],
 
     author       = "keyiflerolsun",
     author_email = "keyiflerolsun@gmail.com",
```

