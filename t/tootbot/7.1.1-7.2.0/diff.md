# Comparing `tmp/tootbot-7.1.1.tar.gz` & `tmp/tootbot-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootbot-7.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tootbot-7.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tootbot-7.1.1.tar` & `tootbot-7.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4489 2023-05-21 07:37:02.157318 tootbot-7.1.1/README.rst
--rw-r--r--   0        0        0     3833 2023-05-21 07:37:02.161318 tootbot-7.1.1/pyproject.toml
--rw-r--r--   0        0        0      752 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/__init__.py
--rw-r--r--   0        0        0     7645 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/app.py
--rw-r--r--   0        0        0    31019 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/collect.py
--rw-r--r--   0        0        0    18239 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/control.py
--rw-r--r--   0        0        0     4766 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/create_config.py
--rw-r--r--   0        0        0     4466 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/debug.py
--rw-r--r--   0        0        0     2472 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/monitoring.py
--rw-r--r--   0        0        0    16491 2023-05-21 07:37:02.161318 tootbot-7.1.1/src/tootbot/publish.py
--rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4489 2023-06-25 09:00:25.116817 tootbot-7.2.0/README.rst
+-rw-r--r--   0        0        0     3833 2023-06-25 09:00:25.120817 tootbot-7.2.0/pyproject.toml
+-rw-r--r--   0        0        0      752 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/__init__.py
+-rw-r--r--   0        0        0     7645 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/app.py
+-rw-r--r--   0        0        0    31346 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/collect.py
+-rw-r--r--   0        0        0    18390 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/control.py
+-rw-r--r--   0        0        0     4877 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/create_config.py
+-rw-r--r--   0        0        0     4466 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/debug.py
+-rw-r--r--   0        0        0     2472 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/monitoring.py
+-rw-r--r--   0        0        0    16491 2023-06-25 09:00:25.120817 tootbot-7.2.0/src/tootbot/publish.py
+-rw-r--r--   0        0        0     6316 1970-01-01 00:00:00.000000 tootbot-7.2.0/PKG-INFO
```

### Comparing `tootbot-7.1.1/README.rst` & `tootbot-7.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.1/pyproject.toml` & `tootbot-7.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,19 +20,19 @@
   "Intended Audience :: End Users/Desktop"
 ]
 
 dependencies = [
     "imgurpython>=1.1.7",
     "arrow>=1.2.3",
     "python-magic>=0.4.27",
-    "asyncpraw>=7.6.1",
+    "asyncpraw>=7.7.0",
     "outdated>=0.2.2",
-    "tqdm>=4.64.1",
+    "tqdm>=4.65.0",
     "aiosqlite>=0.17.0",
-    "yt-dlp>=2023.2.17",
+    "yt-dlp>=2023.6.22",
     "minimal-activitypub>=0.5.5",
 ]
 [project.optional-dependencies]
 doc = [
     "Sphinx>=6.1.3",
     "python-docs-theme>=2022.1",
     "sphinx-rtd-theme>=1.2.0",
```

### Comparing `tootbot-7.1.1/src/tootbot/__init__.py` & `tootbot-7.2.0/src/tootbot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Package 'tootbot' level definitions."""
 import sys
 from typing import Final
 
-__version__: Final[str] = "7.1.1"
+__version__: Final[str] = "7.2.0"
 __display_name__: Final[str] = "Tootbot"
 __package_name__: Final[str] = __display_name__.lower()
 
 # Package level Static Variables
 POST_RECORDER_SQLITE_DB: Final[str] = "history.db"
 POST_RECORDER_HISTORY_RETENTION_DAYS: Final[int] = 31
 USER_AGENT: Final[str] = __display_name__
```

### Comparing `tootbot-7.1.1/src/tootbot/app.py` & `tootbot-7.2.0/src/tootbot/app.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.1/src/tootbot/collect.py` & `tootbot-7.2.0/src/tootbot/collect.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import aiofiles
 import aiohttp
 import arrow
 import asyncpraw.exceptions
 import asyncprawcore
 import magic
 import yt_dlp.utils
+from asyncpraw.models import Redditor
 from asyncpraw.models import Submission
 from imgurpython import ImgurClient
 from imgurpython.helpers.error import ImgurClientError
 from imgurpython.helpers.error import ImgurClientRateLimitError
 from tqdm import tqdm
 from tqdm.asyncio import tqdm as aiotqdm
 
@@ -285,15 +286,15 @@
                     continue
 
                 if await recorder.duplicate_check(posts[post_id].url):
                     logger.debug("Skipping %s, it has already been tooted", post_id)
                     del posts[post_id]
                     continue
 
-    def get_caption(
+    def get_caption(  # noqa C901
         self: RH,
         submission: Submission,
         max_len: int,
         add_hash_tags: Optional[str] = None,
         promo_message: Optional[str] = None,
     ) -> str:
         """get_caption returns the text to be posted to mastodon. This is
@@ -315,51 +316,65 @@
             "RedditHelper.get_caption("
             "submission='%s', max_len=%s, add_hash_tags='%s', promo_message='%s')",
             submission.id,
             max_len,
             add_hash_tags,
             promo_message,
         )
-        # Create string of hashtags
-        hashtag_string = ""
-        promo_string = ""
+
+        author_tag = ""
+        if self.config.mastodon_config.use_redditor_tag:
+            redditor: Redditor = submission.author
+            reddit_user = redditor.name
+            author_tag = f"posted by #u{reddit_user} "
+
         hashtags_for_post = self.config.bot.hash_tags
 
         # Workout hashtags for post
+        hashtag_string = ""
         if add_hash_tags:
             hashtags_for_subreddit = [x.strip() for x in add_hash_tags.split(",")]
             hashtags_for_post = hashtags_for_subreddit + self.config.bot.hash_tags
         if hashtags_for_post:
             for tag in hashtags_for_post:
                 # Add hashtag to string, followed by a space for the next one
-                hashtag_string += "#" + tag + " "
+                hashtag_string += f"#{tag} "
 
+        promo_string = ""
         if promo_message:
             promo_string = f" \n \n{self.config.promo.message}"
+
         caption_max_length = max_len
         caption_max_length -= (
-            len(submission.shortlink) - len(hashtag_string) - len(promo_string)
+            len(submission.shortlink)
+            + len(author_tag)
+            + len(hashtag_string)
+            + len(promo_string)
         )
 
         caption: str = ""
         # Create contents of the Mastodon post
         if len(submission.title) < caption_max_length:
             temp_caption = submission.title + " "
         else:
             temp_caption = submission.title[caption_max_length - 2] + "... "
         if self.config.mastodon_config.use_caption:
             caption += temp_caption
+        caption += author_tag
+
         if self.config.mastodon_config.use_tags:
             caption += hashtag_string
+
         if self.config.mastodon_config.use_backlink:
             if self.config.mastodon_config.link_to_media:
                 caption += submission.url
             else:
                 caption += submission.shortlink
         caption += promo_string
+
         return caption
 
 
 class LinkedMediaHelper:
     """Helper class providing methods to get media attachments."""
 
     def __init__(
```

### Comparing `tootbot-7.1.1/src/tootbot/control.py` & `tootbot-7.2.0/src/tootbot/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -336,14 +336,15 @@
     throttling_enabled: bool
     throttling_max_delay: int
     number_of_errors: int
     use_caption: bool
     use_tags: bool
     use_backlink: bool
     link_to_media: bool
+    use_redditor_tag: bool
 
 
 @dataclass
 class SubredditConfig:
     """Dataclass to hold configuration settings about the subreddits to be monitored."""
 
     name: str
@@ -431,14 +432,17 @@
             throttling_enabled=str_to_bool(config["Mastodon"]["ThrottlingEnabled"]),
             throttling_max_delay=int(config["Mastodon"]["ThrottlingMaxDelay"]),
             number_of_errors=0,
             use_caption=config["Mastodon"].getboolean("UseCaption", fallback=True),
             use_tags=config["Mastodon"].getboolean("UseTags", fallback=True),
             use_backlink=config["Mastodon"].getboolean("UseBacklink", fallback=True),
             link_to_media=config["Mastodon"].getboolean("MediaLink", fallback=False),
+            use_redditor_tag=config["Mastodon"].getboolean(
+                "UseRedditorTag", fallback=False
+            ),
         )
         subreddits = await Configuration._load_subreddits_settings(config)
 
         configuration = cls(
             bot=bot,
             subreddits=subreddits,
             promo=promo,
```

### Comparing `tootbot-7.1.1/src/tootbot/create_config.py` & `tootbot-7.2.0/src/tootbot/create_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # This is the config file for Tootbot! You must restart the bot for any changes to take
 # effect.
 
 # General settings
 [BotSettings]
 # Minimum delay between social media posts, in seconds (default is '600')
 DelayBetweenPosts: 300
-# Run only once (for example when using cron to run tootbot on shedule)
+# Run only once (for example when using cron to run tootbot on schedule)
 RunOnceOnly : false
 # Minimum position of post on subreddit front page that the bot will look at
 # (default is '10')
 PostLimit : 10
 # Allow NSFW Reddit posts to be posted by the bot
 NSFWPostsAllowed : false
 # NSFW media will be marked as sensitive
@@ -35,19 +35,19 @@
 # Log level for messages printed to stdout
 # Possible values are CRITICAL, ERROR, WARNING, INFO, DEBUG
 # If not set the default is INFO
 LogLevel : INFO
 
 # Name of subreddits to take posts from (example: 'gaming')
 # Multireddits can be used like this: 'gaming+funny+news'
-# lines in the Subbreddits section are formated as:
+# lines in the Subbreddits section are formatted as:
 # subreddit: hashtags
 # Subreddit can also be a multireddit as per above
-# hashtags can be one or multiple hashtags sepeareted by commas without the "#" symbol
-# (e.g. hastag1, hashtag2)
+# hashtags can be one or multiple hashtags separated by commas without the "#" symbol
+# (e.g. hashtag1, hashtag2)
 [Subreddits]
 cats: cats
 kittens+bodegacats: cats, kittens, bodegcats
 dogs: dogs
 puppies+goodboy: dogs, puppies, goodboy
 
 # Settings related to promotional messages
@@ -88,16 +88,16 @@
 # Name of instance to log into (example: mastodon.social). This is mandatory
 InstanceDomain :
 # Sets all media attachments as sensitive media, this should be left on 'true'
 # in most cases (note: images from NSFW Reddit posts will always be marked as sensitive)
 # More info:
 # https://gist.github.com/joyeusenoelle/74f6e6c0f349651349a0df9ae4582969#what-does-cw-mean
 SensitiveMedia : true
-# Visibilty setting to use for posts. If left empy defaults to "public"
-# Possiible values are "public", "unlisted", "private"
+# Visibility setting to use for posts. If left empy defaults to "public"
+# Possible values are "public", "unlisted", "private"
 PostVisibility : unlisted
 # With throttling enabled, tootbot will slow down posting toots more and more while
 # the Mastodon API is returning errors
 ThrottlingEnabled : true
 # Maximum delay in seconds between attempts to post a toot when throttling.
 ThrottlingMaxDelay : 86400
 # Should tootbot add a caption to the toot? This defaults to true and will use the title
@@ -107,14 +107,16 @@
 # hash tags defined in this config file.
 UseTags : true
 # Include a link back to the reddit post being tooted. This defaults to true
 UseBacklink : true
 # Make back link go directly to url reddit post links to. For this to take effect,
 # UseBacklink needs to be set to true as well.
 MediaLink : false
+# Add "posted by #u<reddit username>" to the end of the post but before any hash tags.
+UseRedditorTag: false
 """
 
 
 def create() -> None:
     """Creates a sample config.ini configuration file."""
     with open(file="config.ini", mode="w+", encoding="UTF-8") as config_file:
         config_file.writelines(CONFIG_TEMPLATE)
```

### Comparing `tootbot-7.1.1/src/tootbot/debug.py` & `tootbot-7.2.0/src/tootbot/debug.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.1/src/tootbot/monitoring.py` & `tootbot-7.2.0/src/tootbot/monitoring.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.1/src/tootbot/publish.py` & `tootbot-7.2.0/src/tootbot/publish.py`

 * *Files identical despite different names*

### Comparing `tootbot-7.1.1/PKG-INFO` & `tootbot-7.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tootbot
-Version: 7.1.1
+Version: 7.2.0
 Summary: A Python bot that looks up posts from specified subreddits and automatically posts them on Mastodon
 Author-email: marvin8 <marvin8@tuta.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Requires-Dist: imgurpython>=1.1.7
 Requires-Dist: arrow>=1.2.3
 Requires-Dist: python-magic>=0.4.27
-Requires-Dist: asyncpraw>=7.6.1
+Requires-Dist: asyncpraw>=7.7.0
 Requires-Dist: outdated>=0.2.2
-Requires-Dist: tqdm>=4.64.1
+Requires-Dist: tqdm>=4.65.0
 Requires-Dist: aiosqlite>=0.17.0
-Requires-Dist: yt-dlp>=2023.2.17
+Requires-Dist: yt-dlp>=2023.6.22
 Requires-Dist: minimal-activitypub>=0.5.5
 Requires-Dist: pre-commit>=3.0.4 ; extra == "dev"
 Requires-Dist: black>=23.1.0 ; extra == "dev"
 Requires-Dist: mypy>=1.0.0 ; extra == "dev"
 Requires-Dist: safety>=2.3.4 ; extra == "dev"
 Requires-Dist: pip-audit>=2.4.14 ; extra == "dev"
 Requires-Dist: types-aiofiles>=22.1.0.8 ; extra == "dev"
```

