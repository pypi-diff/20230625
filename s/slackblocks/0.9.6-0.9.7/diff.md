# Comparing `tmp/slackblocks-0.9.6.tar.gz` & `tmp/slackblocks-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slackblocks-0.9.6.tar", max compression
+gzip compressed data, was "slackblocks-0.9.7.tar", max compression
```

## Comparing `slackblocks-0.9.6.tar` & `slackblocks-0.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1526 2023-06-12 15:43:52.399738 slackblocks-0.9.6/LICENSE
--rw-r--r--   0        0        0     2400 2023-06-12 15:43:52.399738 slackblocks-0.9.6/README.md
--rw-r--r--   0        0        0     1384 2023-06-12 15:43:52.399738 slackblocks-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     1115 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/__init__.py
--rw-r--r--   0        0        0     2743 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/attachments.py
--rw-r--r--   0        0        0     6922 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/blocks.py
--rw-r--r--   0        0        0    40245 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/elements.py
--rw-r--r--   0        0        0      131 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/errors.py
--rw-r--r--   0        0        0     3456 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/messages.py
--rw-r--r--   0        0        0      671 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/modals.py
--rw-r--r--   0        0        0    11977 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/objects.py
--rw-r--r--   0        0        0     2815 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/utils.py
--rw-r--r--   0        0        0     3886 2023-06-12 15:43:52.399738 slackblocks-0.9.6/slackblocks/views.py
--rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 slackblocks-0.9.6/setup.py
--rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 slackblocks-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1526 2023-06-25 13:44:58.537805 slackblocks-0.9.7/LICENSE
+-rw-r--r--   0        0        0     2400 2023-06-25 13:44:58.537805 slackblocks-0.9.7/README.md
+-rw-r--r--   0        0        0     1384 2023-06-25 13:44:58.537805 slackblocks-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     1115 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/__init__.py
+-rw-r--r--   0        0        0     2743 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/attachments.py
+-rw-r--r--   0        0        0     7479 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/blocks.py
+-rw-r--r--   0        0        0    40245 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/elements.py
+-rw-r--r--   0        0        0      131 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/errors.py
+-rw-r--r--   0        0        0     3456 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/messages.py
+-rw-r--r--   0        0        0      671 2023-06-25 13:44:58.537805 slackblocks-0.9.7/slackblocks/modals.py
+-rw-r--r--   0        0        0    11977 2023-06-25 13:44:58.541805 slackblocks-0.9.7/slackblocks/objects.py
+-rw-r--r--   0        0        0     2815 2023-06-25 13:44:58.541805 slackblocks-0.9.7/slackblocks/utils.py
+-rw-r--r--   0        0        0     3886 2023-06-25 13:44:58.541805 slackblocks-0.9.7/slackblocks/views.py
+-rw-r--r--   0        0        0     3076 1970-01-01 00:00:00.000000 slackblocks-0.9.7/setup.py
+-rw-r--r--   0        0        0     3630 1970-01-01 00:00:00.000000 slackblocks-0.9.7/PKG-INFO
```

### Comparing `slackblocks-0.9.6/LICENSE` & `slackblocks-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/README.md` & `slackblocks-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/pyproject.toml` & `slackblocks-0.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slackblocks"
-version = "0.9.6"
+version = "0.9.7"
 description = "Python wrapper for the Slack Blocks API"
 authors = [
     "Nicholas Lambourne <dev@ndl.im>",
 ]
 maintainers = [
     "Nicholas Lambourne <dev@ndl.im>",
 ]
```

### Comparing `slackblocks-0.9.6/slackblocks/__init__.py` & `slackblocks-0.9.7/slackblocks/__init__.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/attachments.py` & `slackblocks-0.9.7/slackblocks/attachments.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/blocks.py` & `slackblocks-0.9.7/slackblocks/blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -206,20 +206,35 @@
     or side-by-side with any of the available block elements.
     """
 
     def __init__(
         self,
         text: Optional[TextLike] = None,
         block_id: Optional[str] = None,
-        fields: Optional[List[Text]] = None,
+        fields: Optional[Union[TextLike, List[TextLike]]] = None,
         accessory: Optional[Element] = None,
     ):
         super().__init__(type_=BlockType.SECTION, block_id=block_id)
-        self.text = Text.to_text(text)
-        self.fields = fields
+        if not text and not fields:
+            raise InvalidUsageError(
+                "Must supply either `text` or `fields` or `both` to SectionBlock."
+            )
+        self.text = Text.to_text(text, max_length=3000, allow_none=True)
+        self.fields = coerce_to_list(
+            [
+                Text.to_text(field, max_length=2000, allow_none=False)
+                for field in coerce_to_list(fields, class_=(str, Text), allow_none=True)
+            ]
+            if fields
+            else None,
+            class_=Text,
+            allow_none=True,
+            max_size=10,
+        )
+
         self.accessory = accessory
 
     def _resolve(self) -> Dict[str, Any]:
         section = self._attributes()
         if self.text:
             section["text"] = self.text._resolve()
         if self.fields:
```

### Comparing `slackblocks-0.9.6/slackblocks/elements.py` & `slackblocks-0.9.7/slackblocks/elements.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/messages.py` & `slackblocks-0.9.7/slackblocks/messages.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/modals.py` & `slackblocks-0.9.7/slackblocks/modals.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/objects.py` & `slackblocks-0.9.7/slackblocks/objects.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/utils.py` & `slackblocks-0.9.7/slackblocks/utils.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/slackblocks/views.py` & `slackblocks-0.9.7/slackblocks/views.py`

 * *Files identical despite different names*

### Comparing `slackblocks-0.9.6/setup.py` & `slackblocks-0.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['slackblocks']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'slackblocks',
-    'version': '0.9.6',
+    'version': '0.9.7',
     'description': 'Python wrapper for the Slack Blocks API',
     'long_description': '# slackblocks <img src="https://github.com/nicklambourne/slackblocks/raw/master/docs/img/sb.png" align="right" width="250px"/>\n\n![PyPI - License](https://img.shields.io/pypi/l/slackblocks)\n![Python Versions](https://img.shields.io/pypi/pyversions/slackblocks)\n![PyPI](https://img.shields.io/pypi/v/slackblocks?color=yellow&label=PyPI&logo=python&logoColor=white)\n[![Downloads](https://pepy.tech/badge/slackblocks)](https://pepy.tech/project/slackblocks)\n[![Build Status](https://github.com/nicklambourne/slackblocks/actions/workflows/unit-tests.yml/badge.svg?branch=master)](https://github.com/nicklambourne/slackblocks/actions)\n\n## What is it?\n\n`slackblocks` is a Python API for building messages in the fancy Slack Block Kit API.\n\nIt was created by [Nicholas Lambourne](https://github.com/nicklambourne) for the [UQCS Slack Bot](https://github.com/UQComputingSociety/uqcsbot) because he hates writing JSON, naturally this project has subsequently involved writing more JSON than if he\'d done the original task by hand.\n\n## Requirements\n`slackblocks` requires Python >= 3.7.\n\nAs of version 0.1.0 it has no dependencies outside the Python standard library.\n\n## Installation\n\n```bash\npip install slackblocks\n```\n\n## Usage\n\n```python\nfrom slackblocks import Message, SectionBlock\n\n\nblock = SectionBlock("Hello, world!")\nmessage = Message(channel="#general", blocks=block)\nmessage.json()\n\n```\n\nWill produce the following JSON string:\n```json\n{\n    "channel": "#general",\n    "mrkdwn": true,\n    "blocks": [\n        {\n            "type": "section",\n            "block_id": "992ceb6b-9ad4-496b-b8e6-1bd8a632e8b3",\n            "text": {\n                "type": "mrkdwn",\n                "text": "Hello, world!"\n            }\n        }\n    ]\n}\n```\nWhich can be sent as payload to the Slack message API HTTP endpoints.\n\nOf more practical uses is the ability to unpack the objects directly into \nthe Python Slack Client in order to send messages:\n```python\nfrom os import environ\nfrom slack import WebClient\nfrom slackblocks import Message, SectionBlock\n\n\nclient = WebClient(token=environ["SLACK_API_TOKEN"])\nblock = SectionBlock("Hello, world!")\nmessage = Message(channel="#general", blocks=block)\n\nresponse = client.chat_postMessage(**message)\n```\n\nNote the `**` operator in front of the `message` object.\n\n## Can I use this in my project?\n\nYes, please do! The code is all open source and BSD-3.0 licensed.\n',
     'author': 'Nicholas Lambourne',
     'author_email': 'dev@ndl.im',
     'maintainer': 'Nicholas Lambourne',
     'maintainer_email': 'dev@ndl.im',
     'url': 'https://github.com/nicklambourne/slackblocks',
```

### Comparing `slackblocks-0.9.6/PKG-INFO` & `slackblocks-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slackblocks
-Version: 0.9.6
+Version: 0.9.7
 Summary: Python wrapper for the Slack Blocks API
 Home-page: https://github.com/nicklambourne/slackblocks
 License: BSD-3-Clause
 Keywords: slackblocks,slack,messaging,message generation,slack blocks,blocks
 Author: Nicholas Lambourne
 Author-email: dev@ndl.im
 Maintainer: Nicholas Lambourne
```

