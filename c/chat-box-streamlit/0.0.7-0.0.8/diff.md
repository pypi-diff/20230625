# Comparing `tmp/chat-box-streamlit-0.0.7.tar.gz` & `tmp/chat-box-streamlit-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.7.tar", last modified: Sun Jun 25 07:05:46 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.8.tar", last modified: Sun Jun 25 07:28:30 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.7.tar` & `chat-box-streamlit-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:05:46.357175 chat-box-streamlit-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 07:05:28.000000 chat-box-streamlit-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-25 07:05:28.000000 chat-box-streamlit-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 07:05:46.357175 chat-box-streamlit-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-25 07:05:28.000000 chat-box-streamlit-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:05:46.357175 chat-box-streamlit-0.0.7/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-25 07:05:28.000000 chat-box-streamlit-0.0.7/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:05:46.357175 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-25 07:05:46.000000 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-25 07:05:46.000000 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 07:05:46.000000 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 07:05:46.000000 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 07:05:46.000000 chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 07:05:46.357175 chat-box-streamlit-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 07:05:30.000000 chat-box-streamlit-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/chat_box_streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/chat_box_streamlit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-25 07:28:30.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-25 07:28:29.000000 chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 07:28:30.051962 chat-box-streamlit-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-25 07:28:21.000000 chat-box-streamlit-0.0.8/setup.py
```

### Comparing `chat-box-streamlit-0.0.7/LICENSE` & `chat-box-streamlit-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chat-box-streamlit-0.0.7/PKG-INFO` & `chat-box-streamlit-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlit Chat Box 📨
 
 Streamlit Chat Box is a custom chat component built for Streamlit using React, TypeScript, and Styled Components. This project allows you to easily integrate a chat box into your Streamlit applications, enabling interactive and engaging user experiences.
 
 ## Features 🌟
+
 - Real-time chat functionality
 - Customizable UI with styled components
 - Easy integration with Streamlit applications
 - Supports sending and receiving messages
 - Loading indicator for real-time feedback [Work in Progress...]
 
 ## Installation ⚙️
+
 To use the Streamlit Chat Box in your Streamlit application, you need to follow these steps:
 
 1. Install the necessary dependencies by running the following command:
+
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
+
 ```
-from chat_box import display_chat
-from chat_box import input
-from chat_box import message
+from chat_box_streamlit import display_chat
+from chat_box_streamlit import input
+from chat_box_streamlit import message
 ```
 
-## How to use 
+## How to use
 
 1. Input Box
-![Input Box](./assets/Input-Box.png)
-To display an input box where users can enter their messages, use the following code:
+   ![Input Box](./assets/Input-Box.png)
+   To display an input box where users can enter their messages, use the following code:
+
 ```python
 response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
+
 To display with loading:
+
 ```python
 response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
-![Left and Right Messages](./assets/Message.png)
-You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+   ![Left and Right Messages](./assets/Message.png)
+   You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+
 ```
 message(isLeft=True, message="Hi, I am the left message component")
 message(isLeft=False, message="Hello, I am the right message component")
 ```
 
 ## Enjoy Conversational UI! 🗣️💬
+
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
+
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
 
 Thank you for your interest in contributing to our project! We welcome contributions from the community and are grateful for any time and effort you are willing to put in.
 
 1. Fork the repository by clicking the "Fork" button in the top right corner of the page. This will create a copy of the repository in your own GitHub account.
```

### Comparing `chat-box-streamlit-0.0.7/README.md` & `chat-box-streamlit-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 # Streamlit Chat Box 📨
 
 Streamlit Chat Box is a custom chat component built for Streamlit using React, TypeScript, and Styled Components. This project allows you to easily integrate a chat box into your Streamlit applications, enabling interactive and engaging user experiences.
 
 ## Features 🌟
+
 - Real-time chat functionality
 - Customizable UI with styled components
 - Easy integration with Streamlit applications
 - Supports sending and receiving messages
 - Loading indicator for real-time feedback [Work in Progress...]
 
 ## Installation ⚙️
+
 To use the Streamlit Chat Box in your Streamlit application, you need to follow these steps:
 
 1. Install the necessary dependencies by running the following command:
+
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
+
 ```
-from chat_box import display_chat
-from chat_box import input
-from chat_box import message
+from chat_box_streamlit import display_chat
+from chat_box_streamlit import input
+from chat_box_streamlit import message
 ```
 
-## How to use 
+## How to use
 
 1. Input Box
-![Input Box](./assets/Input-Box.png)
-To display an input box where users can enter their messages, use the following code:
+   ![Input Box](./assets/Input-Box.png)
+   To display an input box where users can enter their messages, use the following code:
+
 ```python
 response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
+
 To display with loading:
+
 ```python
 response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
-![Left and Right Messages](./assets/Message.png)
-You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+   ![Left and Right Messages](./assets/Message.png)
+   You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+
 ```
 message(isLeft=True, message="Hi, I am the left message component")
 message(isLeft=False, message="Hello, I am the right message component")
 ```
 
 ## Enjoy Conversational UI! 🗣️💬
+
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
+
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
 
 Thank you for your interest in contributing to our project! We welcome contributions from the community and are grateful for any time and effort you are willing to put in.
 
 1. Fork the repository by clicking the "Fork" button in the top right corner of the page. This will create a copy of the repository in your own GitHub account.
```

### Comparing `chat-box-streamlit-0.0.7/chat_box/__init__.py` & `chat-box-streamlit-0.0.8/chat_box_streamlit/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,18 +12,18 @@
     )
 else:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component("chat_box_streamlit", path=build_dir)
 
 
-def message(isLeft=True, message="", loading=False, loadingText="Loading...", placeholder="Enter your input", height=500, key=None):
+def st_message(isLeft=True, message="", loading=False, loadingText="Loading...", placeholder="Enter your input", height=500, key=None):
     component_value =  _component_func(component="message", isLeft=isLeft, message=message, placeholder=placeholder, loading=loading, loadingText=loadingText, height=height, key=key)
     return component_value
 
-def input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None):
+def st_input(placeholder="Enter your input", loading=False, loadingText="Loading...", rows=1, key=None):
     component_value = _component_func(component="input", placeholder=placeholder, rows=rows, loading=loading, loadingText=loadingText, key=key)
     return component_value
 
-def display_chat(leftMessages = [], rightMessages=[], height=500, rows=1, key=None):
+def st_display_chat(leftMessages = [], rightMessages=[], height=500, rows=1, key=None):
     component_value = _component_func(component="", leftMessages=leftMessages, rightMessages=rightMessages, rows=rows, height=height, key=key)
     return component_value
```

### Comparing `chat-box-streamlit-0.0.7/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.8/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.7
+Version: 0.0.8
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: https://github.com/SSK-14/Streamlit-Chatbox
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Streamlit Chat Box 📨
 
 Streamlit Chat Box is a custom chat component built for Streamlit using React, TypeScript, and Styled Components. This project allows you to easily integrate a chat box into your Streamlit applications, enabling interactive and engaging user experiences.
 
 ## Features 🌟
+
 - Real-time chat functionality
 - Customizable UI with styled components
 - Easy integration with Streamlit applications
 - Supports sending and receiving messages
 - Loading indicator for real-time feedback [Work in Progress...]
 
 ## Installation ⚙️
+
 To use the Streamlit Chat Box in your Streamlit application, you need to follow these steps:
 
 1. Install the necessary dependencies by running the following command:
+
 ```
 pip install chat-box-streamlit
 ```
 
 2. Import the ChatBox component in your Streamlit application:
+
 ```
-from chat_box import display_chat
-from chat_box import input
-from chat_box import message
+from chat_box_streamlit import display_chat
+from chat_box_streamlit import input
+from chat_box_streamlit import message
 ```
 
-## How to use 
+## How to use
 
 1. Input Box
-![Input Box](./assets/Input-Box.png)
-To display an input box where users can enter their messages, use the following code:
+   ![Input Box](./assets/Input-Box.png)
+   To display an input box where users can enter their messages, use the following code:
+
 ```python
 response = input(placeholder="This is the input component", rows=1)
 st.write(response)
 ```
+
 To display with loading:
+
 ```python
 response = input(loading=True, loadingText="Fetching the message...", placeholder="This is input component", rows=1)
 st.write(response)
 ```
 
 2. Left and Right Messages
-![Left and Right Messages](./assets/Message.png)
-You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+   ![Left and Right Messages](./assets/Message.png)
+   You can display messages on the left or right side of the chatbox using the message component. Set isLeft parameter to True for a left message and False for a right message.
+
 ```
 message(isLeft=True, message="Hi, I am the left message component")
 message(isLeft=False, message="Hello, I am the right message component")
 ```
 
 ## Enjoy Conversational UI! 🗣️💬
+
 Feel free to experiment with different messages, components, and settings to create your unique chatbox experience. Happy coding! 💻🎉
 
 ## Contributing 🤝
+
 Contributions to the Streamlit Chat Box project are welcome! If you encounter any issues, have suggestions for improvements, or would like to contribute new features, please open an issue or submit a pull request on the GitHub repository.
 
 ## How to Contribute 👨‍💻
 
 Thank you for your interest in contributing to our project! We welcome contributions from the community and are grateful for any time and effort you are willing to put in.
 
 1. Fork the repository by clicking the "Fork" button in the top right corner of the page. This will create a copy of the repository in your own GitHub account.
```

### Comparing `chat-box-streamlit-0.0.7/setup.py` & `chat-box-streamlit-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 from pathlib import Path
 
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.7",
+    version="0.0.8",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/SSK-14/Streamlit-Chatbox",
     packages=setuptools.find_packages(),
```

