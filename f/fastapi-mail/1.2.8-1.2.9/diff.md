# Comparing `tmp/fastapi_mail-1.2.8.tar.gz` & `tmp/fastapi_mail-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_mail-1.2.8.tar", max compression
+gzip compressed data, was "fastapi_mail-1.2.9.tar", max compression
```

## Comparing `fastapi_mail-1.2.8.tar` & `fastapi_mail-1.2.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1072 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/LICENSE
--rwxr-xr-x   0        0        0     3407 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/README.md
--rwxr-xr-x   0        0        0      385 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/__init__.py
--rw-r--r--   0        0        0     1127 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/config.py
--rw-r--r--   0        0        0     1848 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/connection.py
--rw-r--r--   0        0        0      122 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/email_utils/__init__.py
--rw-r--r--   0        0        0    16451 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/email_utils/email_check.py
--rwxr-xr-x   0        0        0      530 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/errors.py
--rwxr-xr-x   0        0        0     4004 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/fastmail.py
--rw-r--r--   0        0        0     4784 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/msg.py
--rw-r--r--   0        0        0     3133 2023-04-26 07:48:59.443228 fastapi_mail-1.2.8/fastapi_mail/schemas.py
--rw-r--r--   0        0        0     1871 2023-04-26 07:49:16.068640 fastapi_mail-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 fastapi_mail-1.2.8/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/LICENSE
+-rwxr-xr-x   0        0        0     3407 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/README.md
+-rwxr-xr-x   0        0        0      385 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/__init__.py
+-rw-r--r--   0        0        0     1127 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/config.py
+-rw-r--r--   0        0        0     1848 2023-06-25 12:16:26.079044 fastapi_mail-1.2.9/fastapi_mail/connection.py
+-rw-r--r--   0        0        0      122 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/email_utils/__init__.py
+-rw-r--r--   0        0        0    16451 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/email_utils/email_check.py
+-rwxr-xr-x   0        0        0      530 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/errors.py
+-rwxr-xr-x   0        0        0     4004 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/fastmail.py
+-rw-r--r--   0        0        0     5731 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/msg.py
+-rw-r--r--   0        0        0     3590 2023-06-25 12:16:26.083044 fastapi_mail-1.2.9/fastapi_mail/schemas.py
+-rw-r--r--   0        0        0     1871 2023-06-25 12:16:39.586939 fastapi_mail-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4670 1970-01-01 00:00:00.000000 fastapi_mail-1.2.9/PKG-INFO
```

### Comparing `fastapi_mail-1.2.8/LICENSE` & `fastapi_mail-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/README.md` & `fastapi_mail-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/config.py` & `fastapi_mail-1.2.9/fastapi_mail/config.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/connection.py` & `fastapi_mail-1.2.9/fastapi_mail/connection.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/email_utils/email_check.py` & `fastapi_mail-1.2.9/fastapi_mail/email_utils/email_check.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/errors.py` & `fastapi_mail-1.2.9/fastapi_mail/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/fastmail.py` & `fastapi_mail-1.2.9/fastapi_mail/fastmail.py`

 * *Files identical despite different names*

### Comparing `fastapi_mail-1.2.8/fastapi_mail/msg.py` & `fastapi_mail-1.2.9/fastapi_mail/msg.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,24 +4,27 @@
 from email.message import EmailMessage, Message
 from email.mime.base import MIMEBase
 from email.mime.multipart import MIMEMultipart
 from email.mime.text import MIMEText
 from email.utils import formatdate, make_msgid
 from typing import Any, Union
 
+from .schemas import MessageType, MultipartSubtypeEnum
+
 PY3 = sys.version_info[0] == 3
 
 
 class MailMsg:
     """
     Mail message parameters
 
     :param: subject: Email subject header
     :param: recipients: List of email addresses
     :param: body: Plain text message or HTML message
+    :param: alternative_body: Plain text message or HTML message
     :param: template_body: Data to pass into chosen Jinja2 template
     :param: subtype: MessageType class. Type of body parameter, either "plain" or "html"
     :param: sender: Email sender address
     :param: cc: CC list
     :param: bcc: BCC list
     :param: reply_to: Reply-To list
     :param: attachments: List of attachment instances
@@ -32,14 +35,15 @@
     """
 
     def __init__(self, entries) -> None:
         self.recipients = entries.recipients
         self.attachments = entries.attachments
         self.subject = entries.subject
         self.body = entries.body
+        self.alternative_body = entries.alternative_body
         self.template_body = entries.template_body
         self.cc = entries.cc
         self.bcc = entries.bcc
         self.reply_to = entries.reply_to
         self.charset = entries.charset
         self.subtype = entries.subtype
         self.multipart_subtype = entries.multipart_subtype
@@ -84,21 +88,48 @@
                         filename = filename.encode("utf8")
 
                 filename = ("UTF8", "", filename)
                 part.add_header("Content-Disposition", "attachment", filename=filename)
 
             self.message.attach(part)
 
+    def attach_alternative(self, message: MIMEMultipart) -> MIMEMultipart:
+        """
+        Attaches an alternative body to a given message
+        """
+        tmpmsg = message
+        if self.subtype == MessageType.plain:
+            flipped_subtype = "html"
+        else:
+            flipped_subtype = "plain"
+        tmpmsg.attach(self._mimetext(self.alternative_body, flipped_subtype))
+        message = MIMEMultipart(MultipartSubtypeEnum.related.value)
+        message.set_charset(self.charset)
+        message.attach(tmpmsg)
+        return message
+
     async def _message(self, sender: str = None) -> Union[EmailMessage, Message]:
         """
         Creates the email message
         """
 
         self.message = MIMEMultipart(self.multipart_subtype.value)
         self.message.set_charset(self.charset)
+
+        if self.template_body:
+            self.message.attach(self._mimetext(self.template_body, self.subtype.value))
+        elif self.body:
+            self.message.attach(self._mimetext(self.body, self.subtype.value))
+
+        if (
+            self.alternative_body is not None
+            and self.multipart_subtype == MultipartSubtypeEnum.alternative
+        ):
+            self.message = self.attach_alternative(self.message)
+
         self.message["Date"] = formatdate(time.time(), localtime=True)
         self.message["Message-ID"] = self.msgId
         self.message["To"] = ", ".join(self.recipients)
         self.message["From"] = sender
 
         if self.subject:
             self.message["Subject"] = self.subject
@@ -108,20 +139,14 @@
 
         if self.bcc:
             self.message["Bcc"] = ", ".join(self.bcc)
 
         if self.reply_to:
             self.message["Reply-To"] = ", ".join(self.reply_to)
 
-        if self.template_body:
-            self.message.attach(self._mimetext(self.template_body, self.subtype.value))
-
-        elif self.body:
-            self.message.attach(self._mimetext(self.body, self.subtype.value))
-
         if self.attachments:
             await self.attach_file(self.message, self.attachments)
 
         if self.headers:
             for header_name, header_content in self.headers.items():
                 self.message.add_header(header_name, header_content)
```

### Comparing `fastapi_mail-1.2.8/fastapi_mail/schemas.py` & `fastapi_mail-1.2.9/fastapi_mail/schemas.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from enum import Enum
 from io import BytesIO
 from mimetypes import MimeTypes
 from typing import Dict, List, Optional, Union
 
-from pydantic import BaseModel, EmailStr, validator
+from pydantic import BaseModel, EmailStr, root_validator, validator
 from starlette.datastructures import Headers, UploadFile
 
 from fastapi_mail.errors import WrongFile
 
 
 class MultipartSubtypeEnum(Enum):
     """
@@ -34,14 +34,15 @@
 
 
 class MessageSchema(BaseModel):
     recipients: List[EmailStr]
     attachments: List[Union[UploadFile, Dict, str]] = []
     subject: str = ""
     body: Optional[Union[str, list]] = None
+    alternative_body: Optional[str] = None
     template_body: Optional[Union[list, dict, str]] = None
     cc: List[EmailStr] = []
     bcc: List[EmailStr] = []
     reply_to: List[EmailStr] = []
     charset: str = "utf-8"
     subtype: MessageType
     multipart_subtype: MultipartSubtypeEnum = MultipartSubtypeEnum.mixed
@@ -67,15 +68,17 @@
                     with open(file, mode="rb") as f:
                         _, file_name = os.path.split(f.name)
                         content_type = mime_type[0]
                         headers = None
                         if content_type:
                             headers = Headers({"content-type": content_type})
                         file_content = BytesIO(f.read())
-                        u = UploadFile(filename=file_name, file=file_content, headers=headers)
+                        u = UploadFile(
+                            filename=file_name, file=file_content, headers=headers
+                        )
                         temp.append((u, file_meta))
                 else:
                     raise WrongFile(
                         "incorrect file path for attachment or not readable"
                     )
             elif isinstance(file, UploadFile):
                 temp.append((file, file_meta))
@@ -90,9 +93,21 @@
         """
         Validate subtype field
         """
         if values["template_body"]:
             return MessageType.html
         return value
 
+    @root_validator
+    def validate_alternative_body(cls, values):
+        """
+        Validate alternative_body field
+        """
+        if (
+            values["multipart_subtype"] != MultipartSubtypeEnum.alternative
+            and values["alternative_body"]
+        ):
+            values["alternative_body"] = None
+        return values
+
     class Config:
         arbitrary_types_allowed = True
```

### Comparing `fastapi_mail-1.2.8/pyproject.toml` & `fastapi_mail-1.2.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-mail"
-version = "1.2.8"
+version = "1.2.9"
 description = "Simple lightweight mail library for FastApi"
 authors = ["Sabuhi Shukurov <sabuhi.shukurov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/sabuhish/fastapi-mail"
 repository = "https://github.com/sabuhish/fastapi-mail"
 classifiers = [
```

### Comparing `fastapi_mail-1.2.8/PKG-INFO` & `fastapi_mail-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: fastapi-mail
-Version: 1.2.8
+Version: 1.2.9
 Summary: Simple lightweight mail library for FastApi
 Home-page: https://github.com/sabuhish/fastapi-mail
 License: MIT
 Author: Sabuhi Shukurov
 Author-email: sabuhi.shukurov@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Provides-Extra: httpx
 Provides-Extra: redis
 Requires-Dist: Jinja2 (>=3.0,<4.0)
 Requires-Dist: aiosmtplib (>=2.0,<3.0)
 Requires-Dist: blinker (>=1.5,<2.0)
```

