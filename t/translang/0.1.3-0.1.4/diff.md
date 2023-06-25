# Comparing `tmp/translang-0.1.3.tar.gz` & `tmp/translang-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translang-0.1.3.tar", last modified: Sat Jun 24 13:50:07 2023, max compression
+gzip compressed data, was "translang-0.1.4.tar", last modified: Sun Jun 25 17:07:31 2023, max compression
```

## Comparing `translang-0.1.3.tar` & `translang-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.715774 translang-0.1.3/
--rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     4288 2023-06-24 13:50:07.714773 translang-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-06-24 09:24:07.000000 translang-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 13:50:07.715774 translang-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1843 2023-06-24 13:49:05.000000 translang-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.699080 translang-0.1.3/translang/
--rw-rw-rw-   0        0        0      203 2023-06-24 13:49:10.000000 translang-0.1.3/translang/__init__.py
--rw-rw-rw-   0        0        0     5106 2023-06-24 13:48:19.000000 translang-0.1.3/translang/core.py
-drwxrwxrwx   0        0        0        0 2023-06-24 13:50:07.712777 translang-0.1.3/translang.egg-info/
--rw-rw-rw-   0        0        0     4288 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-24 13:50:07.000000 translang-0.1.3/translang.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-25 17:07:31.225835 translang-0.1.4/
+-rw-rw-rw-   0        0        0     1089 2023-06-24 08:01:00.000000 translang-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     5533 2023-06-25 17:07:31.224361 translang-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4628 2023-06-25 17:06:34.000000 translang-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-25 17:07:31.226865 translang-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1885 2023-06-25 17:06:42.000000 translang-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:07:31.207169 translang-0.1.4/translang/
+-rw-rw-rw-   0        0        0      203 2023-06-25 17:06:46.000000 translang-0.1.4/translang/__init__.py
+-rw-rw-rw-   0        0        0     5533 2023-06-25 17:04:37.000000 translang-0.1.4/translang/core.py
+drwxrwxrwx   0        0        0        0 2023-06-25 17:07:31.223353 translang-0.1.4/translang.egg-info/
+-rw-rw-rw-   0        0        0     5533 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-25 17:07:31.000000 translang-0.1.4/translang.egg-info/top_level.txt
```

### Comparing `translang-0.1.3/LICENSE` & `translang-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `translang-0.1.3/PKG-INFO` & `translang-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.3
+Version: 0.1.4
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -17,66 +17,97 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # translang
-Translation Service Module for other projects. Refer to the [hf-transllm](https://github.com/dsdanielpark/hf-transllm) Project for Reference.
-
-
+Translation Service Module for other projects. 
 
 ## Install
 ```
 pip install translang
 ```
 
-
-
 ## Usage
 ### Seamless Integration of Translation APIs through Inheritance
 You can easily extend the `TranslationService` class to integrate with popular translation API services.
+Refer to the [`inference` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L75) and [`generate` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L93) in [hf-transllm](https://github.com/dsdanielpark/hf-transllm) project.
 
 ```python
 from translang import TranslationService
 
 class CustomTranslationService(TranslationService):
     def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo'):
         super().__init__(translator, deepl_api_key, bard_api_key, openai_api_key, openai_model)
 
-    def custom_process_with_translation(self, text: str, dest_lang: str) -> str:
-        translated_text = self.translate(text, dest_lang)
+    def custom_process_with_translation(self, text: str, target_lang: str) -> str:
+        translated_text = self.translate(text, target_lang)
         # Perform additional customization or processing if needed
         return translated_text
 ```
 
+Commercial use or official use of the Google Translate service is chargeable. Please provide the google_official argument and google_api_key. Refer to the following notebook file and official link for more information. Use the google argument only for some basic functionality testing.
 ```python
 translator = CustomTranslationService(translator="google")
 
 translated_text = translator.custom_process_with_translation("Hello", "ko")
 print(translated_text)
 ```
 
+<br>
 
-### Static Methods
-
-Google Translator
+### `TranslationService.translate` Method
+Google Translator, DeepL, OpenAI, Bard
 ```python
 fomr translang import TranslationService
 
 translator = TranslationService(translator="google")                                                                         # Google
 # translator = TranslationService(translator="deepl", deepl_api_key="YOUR_DEEPL_API_KEY")                                    # DeepL
 # translator = TranslationService(translator="bard", bard_api_key="YOUR_BARD_API_KEY")                                       # Bard
 # translator = TranslationService(translator="openai", openai_api_key="YOUR_OPENAI_API_KEY", openai_model="gpt-3.5-trubo")   # Open AI
 
 translated_text = translator.translate("Hello", "ko")
 print(translated_text)
 ```
 
 
+<br>
+
+### `TranslationService.translate_parallel` Method
+
+```python
+from translang import TranslationService
+
+# Create an instance of TranslationService
+translator = TranslationService(translator="google", use_cache=True)
+
+# List of texts to translate
+texts = [
+    "Hello",
+    "Nice to meet you",
+    "Testing the translation service"
+]
+
+# Destination language code
+target_lang = "ko"
+
+# Call the translate_parallel method
+translated_texts = translator.translate_parallel(texts, target_lang)
+
+# Print the translated texts
+for text, translated_text in zip(texts, translated_texts):
+    print(f"Original: {text}")
+    print(f"Translated: {translated_text}")
+    print("-----")
+
+```
+
+<br><br>
+
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; 
 ```
 The MIT License (MIT)
 
 Copyright (c) 2023 Minwoo Park
```

### Comparing `translang-0.1.3/README.md` & `translang-0.1.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,91 @@
 # translang
-Translation Service Module for other projects. Refer to the [hf-transllm](https://github.com/dsdanielpark/hf-transllm) Project for Reference.
-
-
+Translation Service Module for other projects. 
 
 ## Install
 ```
 pip install translang
 ```
 
-
-
 ## Usage
 ### Seamless Integration of Translation APIs through Inheritance
 You can easily extend the `TranslationService` class to integrate with popular translation API services.
+Refer to the [`inference` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L75) and [`generate` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L93) in [hf-transllm](https://github.com/dsdanielpark/hf-transllm) project.
 
 ```python
 from translang import TranslationService
 
 class CustomTranslationService(TranslationService):
     def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo'):
         super().__init__(translator, deepl_api_key, bard_api_key, openai_api_key, openai_model)
 
-    def custom_process_with_translation(self, text: str, dest_lang: str) -> str:
-        translated_text = self.translate(text, dest_lang)
+    def custom_process_with_translation(self, text: str, target_lang: str) -> str:
+        translated_text = self.translate(text, target_lang)
         # Perform additional customization or processing if needed
         return translated_text
 ```
 
+Commercial use or official use of the Google Translate service is chargeable. Please provide the google_official argument and google_api_key. Refer to the following notebook file and official link for more information. Use the google argument only for some basic functionality testing.
 ```python
 translator = CustomTranslationService(translator="google")
 
 translated_text = translator.custom_process_with_translation("Hello", "ko")
 print(translated_text)
 ```
 
+<br>
 
-### Static Methods
-
-Google Translator
+### `TranslationService.translate` Method
+Google Translator, DeepL, OpenAI, Bard
 ```python
 fomr translang import TranslationService
 
 translator = TranslationService(translator="google")                                                                         # Google
 # translator = TranslationService(translator="deepl", deepl_api_key="YOUR_DEEPL_API_KEY")                                    # DeepL
 # translator = TranslationService(translator="bard", bard_api_key="YOUR_BARD_API_KEY")                                       # Bard
 # translator = TranslationService(translator="openai", openai_api_key="YOUR_OPENAI_API_KEY", openai_model="gpt-3.5-trubo")   # Open AI
 
 translated_text = translator.translate("Hello", "ko")
 print(translated_text)
 ```
 
 
+<br>
+
+### `TranslationService.translate_parallel` Method
+
+```python
+from translang import TranslationService
+
+# Create an instance of TranslationService
+translator = TranslationService(translator="google", use_cache=True)
+
+# List of texts to translate
+texts = [
+    "Hello",
+    "Nice to meet you",
+    "Testing the translation service"
+]
+
+# Destination language code
+target_lang = "ko"
+
+# Call the translate_parallel method
+translated_texts = translator.translate_parallel(texts, target_lang)
+
+# Print the translated texts
+for text, translated_text in zip(texts, translated_texts):
+    print(f"Original: {text}")
+    print(f"Translated: {translated_text}")
+    print("-----")
+
+```
+
+<br><br>
+
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; 
 ```
 The MIT License (MIT)
 
 Copyright (c) 2023 Minwoo Park
```

### Comparing `translang-0.1.3/setup.py` & `translang-0.1.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,29 +21,30 @@
 
 
 version = get_version()
 
 
 setup(
     name="translang",
-    version="0.1.3",
+    version="0.1.4",
     author="daniel park",
     author_email="parkminwoo1991@gmail.com",
     description="Translation Service API Module.",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/dsdanielpark/hf-transllm",
     packages=find_packages(exclude=[]),
     python_requires=">=3.6",
     install_requires=[
         "requests",
         "deepl",
         "deep_translator",
         "bardapi",
         "openai",
+        "google-cloud-translate==2.0.1",
     ],
     keywords="Python, API, Bard, Google Bard, Large Language Model, Chatbot API, Google API, Chatbot",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "Programming Language :: Python",
```

### Comparing `translang-0.1.3/translang/core.py` & `translang-0.1.4/translang/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 import deepl
 import openai
 import concurrent.futures
 from deep_translator import GoogleTranslator
 from bardapi import Bard
 from typing import List
+from google.cloud import translate_v2 as translate
 
 
 class TranslationService:
     """
     A service for translating text using different translation engines.
 
     Args:
@@ -27,26 +28,29 @@
         openai_model (str): The OpenAI model being used.
         use_cache (bool): Whether to use a translation cache.
         translation_cache (dict): Cache for storing translated texts.
         translator_engine: The translation engine object.
 
     """
 
-    def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo', use_cache=False):
+    def __init__(self, translator="google", google_api_key=None, deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo', use_cache=False):
         self.translator = translator
+        self.google_api_key = google_api_key
         self.deepl_api_key = deepl_api_key
         self.bard_api_key = bard_api_key
         self.openai_api_key = openai_api_key
         self.openai_model = openai_model
         self.use_cache = use_cache
 
         self.translation_cache = {}
         self.translator_engine = None
-
-        if self.translator == "google":
+        
+        if self.translator=='google_official':
+            self.translator_engine = translate.Client(api_key=google_api_key)
+        elif self.translator == "google":
             pass
         elif self.translator == "deepl":
             self.translator_engine = deepl.Translator(auth_key=self.deepl_api_key)
         elif self.translator == "bard":
             self.translator_engine = Bard(token=self.bard_api_key)
         elif self.translator == "openai":
             openai.api_key = self.openai_api_key
@@ -66,59 +70,60 @@
         
         if extracted_text:
             return extracted_text.group(1) or extracted_text.group(2) 
         
         return text
 
 
-    def translate(self, text: str, dest_lang: str) -> str:
+    def translate(self, text: str, target_lang: str) -> str:
         """
         Translate the given text to the specified destination language.
 
         Args:
             text (str): The text to be translated.
-            dest_lang (str): The destination language code.
+            target_lang (str): The destination language code.
 
         Returns:
             str: The translated text.
 
         """
         if self.use_cache:
-            cache_key = (text, dest_lang)
+            cache_key = (text, target_lang)
             translated_text = self.translation_cache.get(cache_key)
             if translated_text is not None:
                 return translated_text
-
-        if self.translator == "google":
-            self.translator_engine = GoogleTranslator(source="auto", target=dest_lang)
+        if self.translator == "google_official":
+            translated_text = self.translator_engine.translate(text, target_language=target_lang)
+        elif self.translator == "google":
+            self.translator_engine = GoogleTranslator(source="auto", target=target_lang)
             translated_text = self.translator_engine.translate(text)
         elif self.translator == "deepl":
-            translated_text = self.translator_engine.translate_text(text, target_lang=dest_lang).text
+            translated_text = self.translator_engine.translate_text(text, target_lang=target_lang).text
         elif self.translator == "bard":
-            translated = self.translator_engine.get_answer(f"Translate the following text to {dest_lang}: {text}")['content']
+            translated = self.translator_engine.get_answer(f"Translate the following text to {target_lang}: {text}")['content']
             translated_text = self._refine_bard_answer(translated)
         elif self.translator == "openai":
-            prompt = f"Translate the following text to {dest_lang}: {text}"
+            prompt = f"Translate the following text to {target_lang}: {text}"
             response = openai.Completion.create(engine=self.openai_model, prompt=prompt, max_tokens=100)
             translated_text = response.choices[0].text.strip()
 
         if self.use_cache:
-            cache_key = (text, dest_lang)
+            cache_key = (text, target_lang)
             self.translation_cache[cache_key] = translated_text
 
         return translated_text
 
-    def translate_parallel(self, texts: List[str], dest_lang: str) -> List[str]:
+    def translate_parallel(self, texts: List[str], target_lang: str) -> List[str]:
         """
         Translate a list of texts to the specified destination language in parallel.
 
         Args:
             texts (List[str]): The list of texts to be translated.
-            dest_lang (str): The destination language code.
+            target_lang (str): The destination language code.
 
         Returns:
             List[str]: The list of translated texts.
 
         """
         with concurrent.futures.ThreadPoolExecutor() as executor:
-            translated_texts = list(executor.map(self.translate, texts, [dest_lang] * len(texts)))
+            translated_texts = list(executor.map(self.translate, texts, [target_lang] * len(texts)))
         return translated_texts
```

### Comparing `translang-0.1.3/translang.egg-info/PKG-INFO` & `translang-0.1.4/translang.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translang
-Version: 0.1.3
+Version: 0.1.4
 Summary: Translation Service API Module.
 Home-page: https://github.com/dsdanielpark/hf-transllm
 Author: daniel park
 Author-email: parkminwoo1991@gmail.com
 Keywords: Python,API,Bard,Google Bard,Large Language Model,Chatbot API,Google API,Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -17,66 +17,97 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # translang
-Translation Service Module for other projects. Refer to the [hf-transllm](https://github.com/dsdanielpark/hf-transllm) Project for Reference.
-
-
+Translation Service Module for other projects. 
 
 ## Install
 ```
 pip install translang
 ```
 
-
-
 ## Usage
 ### Seamless Integration of Translation APIs through Inheritance
 You can easily extend the `TranslationService` class to integrate with popular translation API services.
+Refer to the [`inference` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L75) and [`generate` method](https://github.com/dsdanielpark/hf-transllm/blob/main/transllm/core.py#L93) in [hf-transllm](https://github.com/dsdanielpark/hf-transllm) project.
 
 ```python
 from translang import TranslationService
 
 class CustomTranslationService(TranslationService):
     def __init__(self, translator="google", deepl_api_key=None, bard_api_key=None, openai_api_key=None, openai_model='gpt-3.5-turbo'):
         super().__init__(translator, deepl_api_key, bard_api_key, openai_api_key, openai_model)
 
-    def custom_process_with_translation(self, text: str, dest_lang: str) -> str:
-        translated_text = self.translate(text, dest_lang)
+    def custom_process_with_translation(self, text: str, target_lang: str) -> str:
+        translated_text = self.translate(text, target_lang)
         # Perform additional customization or processing if needed
         return translated_text
 ```
 
+Commercial use or official use of the Google Translate service is chargeable. Please provide the google_official argument and google_api_key. Refer to the following notebook file and official link for more information. Use the google argument only for some basic functionality testing.
 ```python
 translator = CustomTranslationService(translator="google")
 
 translated_text = translator.custom_process_with_translation("Hello", "ko")
 print(translated_text)
 ```
 
+<br>
 
-### Static Methods
-
-Google Translator
+### `TranslationService.translate` Method
+Google Translator, DeepL, OpenAI, Bard
 ```python
 fomr translang import TranslationService
 
 translator = TranslationService(translator="google")                                                                         # Google
 # translator = TranslationService(translator="deepl", deepl_api_key="YOUR_DEEPL_API_KEY")                                    # DeepL
 # translator = TranslationService(translator="bard", bard_api_key="YOUR_BARD_API_KEY")                                       # Bard
 # translator = TranslationService(translator="openai", openai_api_key="YOUR_OPENAI_API_KEY", openai_model="gpt-3.5-trubo")   # Open AI
 
 translated_text = translator.translate("Hello", "ko")
 print(translated_text)
 ```
 
 
+<br>
+
+### `TranslationService.translate_parallel` Method
+
+```python
+from translang import TranslationService
+
+# Create an instance of TranslationService
+translator = TranslationService(translator="google", use_cache=True)
+
+# List of texts to translate
+texts = [
+    "Hello",
+    "Nice to meet you",
+    "Testing the translation service"
+]
+
+# Destination language code
+target_lang = "ko"
+
+# Call the translate_parallel method
+translated_texts = translator.translate_parallel(texts, target_lang)
+
+# Print the translated texts
+for text, translated_text in zip(texts, translated_texts):
+    print(f"Original: {text}")
+    print(f"Translated: {translated_text}")
+    print("-----")
+
+```
+
+<br><br>
+
 ## License
 [MIT](https://opensource.org/license/mit/) <br>
 I hold no legal responsibility; 
 ```
 The MIT License (MIT)
 
 Copyright (c) 2023 Minwoo Park
```

