# Comparing `tmp/chat-box-streamlit-0.0.4.tar.gz` & `tmp/chat-box-streamlit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.4.tar", last modified: Sun Jun 18 09:37:08 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.5.tar", last modified: Sun Jun 25 03:16:09 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.4.tar` & `chat-box-streamlit-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-18 09:36:57.000000 chat-box-streamlit-0.0.4/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 09:37:08.000000 chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 09:37:08.407075 chat-box-streamlit-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-18 09:36:59.000000 chat-box-streamlit-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/chat_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-25 03:15:54.000000 chat-box-streamlit-0.0.5/chat_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 03:16:09.000000 chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 03:16:09.520041 chat-box-streamlit-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 03:15:57.000000 chat-box-streamlit-0.0.5/setup.py
```

### Comparing `chat-box-streamlit-0.0.4/LICENSE` & `chat-box-streamlit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.4/PKG-INFO` & `chat-box-streamlit-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.4/README.md` & `chat-box-streamlit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.4/chat_box/__init__.py` & `chat-box-streamlit-0.0.5/chat_box/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 
 def input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None):
     return _chat_box(component="input", placeholder=placeholder, rows=rows, loading=loading, loadingText=loadingText, key=key)
 
 def display_chat(leftMessages = [], rightMessages=[], height=500, rows=1, key=None):
     return _chat_box(component="", leftMessages=leftMessages, rightMessages=rightMessages, rows=rows, height=height, key=key)
 
-def initialise():
-    if 'leftMessages' not in st.session_state:
-        st.session_state['leftMessages'] = []
+# def initialise():
+#     if 'leftMessages' not in st.session_state:
+#         st.session_state['leftMessages'] = []
     
-    if 'rightMessages' not in st.session_state:
-        st.session_state['rightMessages'] = []
+#     if 'rightMessages' not in st.session_state:
+#         st.session_state['rightMessages'] = []
 
-    if 'input' not in st.session_state:
-        st.session_state['input'] = ""
+#     if 'input' not in st.session_state:
+#         st.session_state['input'] = ""
 
 
-def main():
-    initialise()
-    st.header('🗃️ Demo Chat')
+# def main():
+#     initialise()
+#     st.header('🗃️ Demo Chat')
 
-    st.session_state.input = input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1)
-    if st.session_state.input != "" and st.session_state.input is not None:
-        st.session_state['leftMessages'].append(st.session_state.input)
-        st.session_state['rightMessages'].append("(Response) : " + st.session_state.input)
+#     st.session_state.input = input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1)
+#     if st.session_state.input != "" and st.session_state.input is not None:
+#         st.session_state['leftMessages'].append(st.session_state.input)
+#         st.session_state['rightMessages'].append("(Response) : " + st.session_state.input)
 
 
-    display_chat(leftMessages=st.session_state['leftMessages'], rightMessages=st.session_state['rightMessages'], height=600)
+#     display_chat(leftMessages=st.session_state['leftMessages'], rightMessages=st.session_state['rightMessages'], height=600)
 
-if not _RELEASE:
-    st.set_page_config(page_title="ChatBox Demo", page_icon=":speech_balloon:")
-    st.markdown("## Streamlit ChatBox Demo 💬")
-    main()
+# if not _RELEASE:
+#     st.set_page_config(page_title="ChatBox Demo", page_icon=":speech_balloon:")
+#     st.markdown("## Streamlit ChatBox Demo 💬")
+#     main()
```

### Comparing `chat-box-streamlit-0.0.4/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.5/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.4/setup.py` & `chat-box-streamlit-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.4",
+    version="0.0.5",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

