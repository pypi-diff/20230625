# Comparing `tmp/tweeterpy-0.0.3.tar.gz` & `tmp/tweeterpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.3.tar", last modified: Thu Jun 22 07:59:27 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.4.tar", last modified: Sun Jun 25 07:48:12 2023, max compression
```

## Comparing `tweeterpy-0.0.3.tar` & `tweeterpy-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.596127 tweeterpy-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     3389 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 07:59:27.596127 tweeterpy-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-06-22 07:57:46.000000 tweeterpy-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.3/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.3/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      481 2023-06-22 07:37:42.000000 tweeterpy-0.0.3/tweeterpy/config.py
--rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.3/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-20 11:23:57.000000 tweeterpy-0.0.3/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.3/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0    20755 2023-06-21 13:16:47.000000 tweeterpy-0.0.3/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3259 2023-06-22 07:37:42.000000 tweeterpy-0.0.3/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:59:27.580491 tweeterpy-0.0.3/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      221 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 07:59:27.000000 tweeterpy-0.0.3/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 07:48:12.553864 tweeterpy-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-06-25 07:48:12.553864 tweeterpy-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 07:48:12.553864 tweeterpy-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-06-25 07:47:41.000000 tweeterpy-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:48:12.553864 tweeterpy-0.0.4/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.4/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     2581 2023-06-20 09:49:11.000000 tweeterpy-0.0.4/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.4/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     1980 2023-06-20 14:19:17.000000 tweeterpy-0.0.4/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.4/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.4/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.4/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    22817 2023-06-25 07:23:32.000000 tweeterpy-0.0.4/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     3526 2023-06-25 07:16:42.000000 tweeterpy-0.0.4/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-06-25 07:48:12.553864 tweeterpy-0.0.4/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-06-25 07:48:12.000000 tweeterpy-0.0.4/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-06-25 07:48:12.000000 tweeterpy-0.0.4/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 07:48:12.000000 tweeterpy-0.0.4/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      221 2023-06-25 07:48:12.000000 tweeterpy-0.0.4/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 07:48:12.000000 tweeterpy-0.0.4/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.3/LICENSE` & `tweeterpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/PKG-INFO` & `tweeterpy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.3 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.4 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-0.0.3/README.md` & `tweeterpy-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/setup.py` & `tweeterpy-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-0.0.3/tweeterpy/api_util.py` & `tweeterpy-0.0.4/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/tweeterpy/constants.py` & `tweeterpy-0.0.4/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/tweeterpy/login_util.py` & `tweeterpy-0.0.4/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/tweeterpy/request_util.py` & `tweeterpy-0.0.4/tweeterpy/request_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.3/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.4/tweeterpy/tweeterpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import getpass
 from functools import reduce
 
 from .api_util import ApiUpdater
 from .constants import Path
 from .login_util import TaskHandler
 from .request_util import make_request
+from .session_util import load_session, save_session
 from . import util
 from . import config
 
 
 class TweeterPy:
 
     def __init__(self):
@@ -65,50 +66,99 @@
                     data_container['cursor_endpoint'] = end_cursor
 
                 if ((top_cursor and end_cursor) and len(data) == 2) or ((top_cursor or end_cursor) and len(data) == 1) or (not end_cursor):
                     data_container["has_next_page"] = False
 
                 if not data_container["has_next_page"] or (total is not None and len(data_container['data']) >= total):
                     return data_container
-
+            # fmt: on 
             except ConnectionError as error:
                 print(error)
                 continue
 
             except Exception as error:
                 print(error)
                 return data_container
 
-    def generate_session(self):
+    @property
+    def session(self):
+        return self._session
+
+    @session.setter
+    def session(self, session):
+        self._session = session
+        config._DEFAULT_SESSION = session
+
+    @property
+    def me(self):
+        """Returns logged in user information.
+
+        Returns:
+            dict: Currently logged in user's data.
+        """
+        url = util.generate_url(url_path=Path.VIEWER_ENDPOINT)
+        query = {"variables": json.dumps({"withCommunitiesMemberships": True,
+                                          "withSubscribedTab": True, "withCommunitiesCreation": True}),
+                 "features": json.dumps(util.generate_features())}
+        response = self.session.get(url, params=query).json()
+        return response
+
+    def generate_session(self, auth_token=None):
+        """Generate a twitter session. With/Without Login.
+
+        Args:
+            auth_token (str, optional): Generate session with an auth-token. If auth_token is None (Default Behaviour), generates a guest session without login. Defaults to None.
+
+        Returns:
+            requests.Session: requests.Session Object.
+        """
         self.session = requests.Session()
         if config.PROXY is not None:
             self.session.proxies = config.PROXY
             self.session.verify = False
         self.session.headers.update(util.generate_headers())
         make_request(Path.BASE_URL, session=self.session)
         guest_token = make_request(
             Path.GUEST_TOKEN_URL, method="POST", session=self.session)['guest_token']
         self.session.headers.update({'X-Guest-Token': guest_token})
         self.session.cookies.update({'gt': guest_token})
-        config._DEFAULT_SESSION = self.session
+        if auth_token:
+            self.session.cookies.update({'auth_token': auth_token})
+            util.generate_headers(self.session)
         return self.session
 
-    @property
-    def me(self):
-        """Returns logged in user information.
+    def save_session(self, session=None, session_name=None):
+        """Save a logged in session to avoid frequent logins in future.
+
+        Args:
+            session (requests.Session, optional): requests.Session object you want to save. If None, saves current session by default. Defaults to None. 
+            session_name (str, optional): Session name. If None, uses currently logged in username. Defaults to None.
 
         Returns:
-            dict: Currently logged in user's data.
+            path: Saved session file path.
         """
-        url = util.generate_url(url_path=Path.VIEWER_ENDPOINT)
-        query = {"variables": json.dumps({"withCommunitiesMemberships": True,
-                                          "withSubscribedTab": True, "withCommunitiesCreation": True}),
-                 "features": json.dumps(util.generate_features())}
-        response = self.session.get(url, params=query).json()
-        return response
+        if session is None:
+            session = self.session
+        if session_name is None:
+            session_name = self.me['data']['viewer']['user_results']['result']['legacy']['screen_name']
+        return save_session(filename=session_name, session=session)
+
+    def load_session(self, session_file_path=None, session=None):
+        """Load a saved session.
+
+        Args:
+            session_file_path (path, optional): File path to load session from. If None, shows a list of all saved session to choose from. Defaults to None.
+            session (request.Session, optional): requests.Session object to load a saved session into. Defaults to None.
+
+        Returns:
+            requests.Session: Restored session.
+        """
+        self.session = load_session(
+            file_path=session_file_path, session=session)
+        return self.session
 
     def logged_in(self):
         """Check if the user is logged in.
 
         Returns:
             bool: Returns True if the user is logged in.
         """
@@ -124,17 +174,15 @@
             password (str, optional): Password. Defaults to None.
         """
         if username is None:
             username = str(input("Enter Your Username or Email : ")).strip()
         if password is None:
             password = getpass.getpass()
         TaskHandler().login(username, password)
-        self.me
-        self.session.headers.update(
-            {"X-Csrf-Token": self.session.cookies["ct0"]})
+        util.generate_headers(session=self.session)
 
     def get_user_id(self, username):
         """Get user ID of a twitter user.
 
         Args:
             username (str): Twitter username.
 
@@ -416,8 +464,8 @@
         url, query_params = self._generate_request_data(
             Path.RETWEETED_BY_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'retweeters_timeline', 'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
 
 if __name__ == "__main__":
-    pass
+    pass
```

### Comparing `tweeterpy-0.0.3/tweeterpy/util.py` & `tweeterpy-0.0.4/tweeterpy/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 class DotDict(dict):
     """dot.notation access to dictionary attributes"""
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
     __delattr__ = dict.__delitem__
 
 
-def generate_headers():
+def generate_headers(session=None):
     headers = {"Authority": Path.DOMAIN,
                "Accept-Encoding": "gzip, deflate, br",
                "Accept-Language": "en-US,en;q=0.9",
                "Authorization": PUBLIC_TOKEN,
                "Cache-Control": "no-cache",
                "Referer": Path.BASE_URL,
                "User-Agent": config._USER_AGENT,
                "X-Twitter-Active-User": "yes",
                "X-Twitter-Client-Language": "en"
                }
+    if session:
+        if "auth_token" in session.cookies.keys():
+            session.get(Path.BASE_URL)
+            session.headers.update(
+                {"X-Csrf-Token": session.cookies.get("ct0", None), "X-Twitter-Auth-Type": "OAuth2Session"})
     return headers
 
 
 def generate_features(default_features=True, user_data_features=False, user_info_feautres=False, additional_features=False):
     features = {}
     if default_features:
         default_features = {"responsive_web_graphql_exclude_directive_enabled": True, "verified_phone_label_enabled": True,
```

### Comparing `tweeterpy-0.0.3/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.4/tweeterpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.3
+Version: 0.0.4
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.3 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.4 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

