# Comparing `tmp/spotify_internal-0.1.8.tar.gz` & `tmp/spotify_internal-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_internal-0.1.8.tar", max compression
+gzip compressed data, was "spotify_internal-0.1.9.tar", max compression
```

## Comparing `spotify_internal-0.1.8.tar` & `spotify_internal-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1052 2022-11-13 11:18:11.924164 spotify_internal-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0      531 2022-12-14 19:39:44.867355 spotify_internal-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      115 2022-11-13 11:16:08.243487 spotify_internal-0.1.8/README.md
--rw-r--r--   0        0        0      178 2022-11-13 13:55:50.386629 spotify_internal-0.1.8/spotify_internal/__init__.py
--rw-r--r--   0        0        0    20363 2022-11-21 12:44:25.843780 spotify_internal-0.1.8/spotify_internal/endpoints.py
--rw-r--r--   0        0        0     7879 2022-12-14 19:39:12.868067 spotify_internal-0.1.8/spotify_internal/internal.py
--rw-r--r--   0        0        0     1841 2022-11-13 15:32:14.431762 spotify_internal-0.1.8/spotify_internal/login.py
--rw-r--r--   0        0        0     2212 2022-12-08 08:13:06.182822 spotify_internal-0.1.8/spotify_internal/utils.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 spotify_internal-0.1.8/setup.py
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 spotify_internal-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1052 2022-11-13 11:18:11.924164 spotify_internal-0.1.9/LICENSE.txt
+-rw-r--r--   0        0        0      530 2023-06-25 05:25:10.059263 spotify_internal-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      115 2022-11-13 11:16:08.243487 spotify_internal-0.1.9/README.md
+-rw-r--r--   0        0        0      178 2022-11-13 13:55:50.386629 spotify_internal-0.1.9/spotify_internal/__init__.py
+-rw-r--r--   0        0        0    20363 2022-11-21 12:44:25.843780 spotify_internal-0.1.9/spotify_internal/endpoints.py
+-rw-r--r--   0        0        0     8112 2023-03-26 13:46:50.877977 spotify_internal-0.1.9/spotify_internal/internal.py
+-rw-r--r--   0        0        0     1841 2022-11-13 15:32:14.431762 spotify_internal-0.1.9/spotify_internal/login.py
+-rw-r--r--   0        0        0     2212 2022-12-08 08:13:06.182822 spotify_internal-0.1.9/spotify_internal/utils.py
+-rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 spotify_internal-0.1.9/PKG-INFO
```

### Comparing `spotify_internal-0.1.8/LICENSE.txt` & `spotify_internal-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotify_internal-0.1.8/pyproject.toml` & `spotify_internal-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "spotify-internal"
-version = "0.1.8"
+version = "0.1.9"
 description = "A Python wrapper around the Spotify Internal API which can let users login with their login creds (and not OAuth)"
 authors = ["addyett <g.aditya2048@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "spotify_internal"}]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 requests = "^2.28.1"
-librespot = "^0.0.7"
+librespot = "0.0.9"
 spotipy = "^2.21.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `spotify_internal-0.1.8/spotify_internal/endpoints.py` & `spotify_internal-0.1.9/spotify_internal/endpoints.py`

 * *Files identical despite different names*

### Comparing `spotify_internal-0.1.8/spotify_internal/internal.py` & `spotify_internal-0.1.9/spotify_internal/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -198,7 +198,11 @@
         return self._get(url)['data']
 
     def track_name_from_id(self, track_id: str):
         track_data = self.spotify.track(track_id)
         # track = ytmusic.search(f"{track_data['artists'][0]['name']} - {track_data['name']}").tracks[0]
         # url = track.url
         return f"{track_data['artists'][0]['name']} - {track_data['name']}"
+
+    def get_lyrics(self):
+        url = 'https://spclient.wg.spotify.com/color-lyrics/v2/track/22L7bfCiAkJo5xGSQgmiIO/image/spotify:image:ab67616d0000b273d9194aa18fa4c9362b47464f?clientLanguage=en'
+        return self._get(url)
```

### Comparing `spotify_internal-0.1.8/spotify_internal/login.py` & `spotify_internal-0.1.9/spotify_internal/login.py`

 * *Files identical despite different names*

### Comparing `spotify_internal-0.1.8/spotify_internal/utils.py` & `spotify_internal-0.1.9/spotify_internal/utils.py`

 * *Files identical despite different names*

### Comparing `spotify_internal-0.1.8/PKG-INFO` & `spotify_internal-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: spotify-internal
-Version: 0.1.8
+Version: 0.1.9
 Summary: A Python wrapper around the Spotify Internal API which can let users login with their login creds (and not OAuth)
 License: MIT
 Author: addyett
 Author-email: g.aditya2048@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: librespot (>=0.0.7,<0.0.8)
+Requires-Dist: librespot (==0.0.9)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: spotipy (>=2.21.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 A Python wrapper around the Spotify Internal API which can let users login with their login creds (and not OAuth)
```

