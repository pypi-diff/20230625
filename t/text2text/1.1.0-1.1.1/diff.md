# Comparing `tmp/text2text-1.1.0.tar.gz` & `tmp/text2text-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.1.0.tar", last modified: Fri Jun 23 14:33:45 2023, max compression
+gzip compressed data, was "text2text-1.1.1.tar", last modified: Sat Jun 24 21:54:16 2023, max compression
```

## Comparing `text2text-1.1.0.tar` & `text2text-1.1.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.973021 text2text-1.1.0/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-23 14:21:46.000000 text2text-1.1.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    60408 2023-06-23 14:33:45.973021 text2text-1.1.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    59594 2023-06-23 14:27:03.000000 text2text-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 14:33:45.973021 text2text-1.1.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-23 14:25:29.000000 text2text-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.970021 text2text-1.1.0/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-06-23 14:22:43.000000 text2text-1.1.0/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.971021 text2text-1.1.0/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1451 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2010 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.973021 text2text-1.1.0/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2605 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)      984 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/searcher.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-23 14:21:46.000000 text2text-1.1.0/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 14:33:45.971021 text2text-1.1.0/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    60408 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1064 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-23 14:33:45.000000 text2text-1.1.0/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:54:16.674018 text2text-1.1.1/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-24 20:00:33.000000 text2text-1.1.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    59869 2023-06-24 21:54:16.673018 text2text-1.1.1/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    59055 2023-06-24 21:53:13.000000 text2text-1.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 21:54:16.674018 text2text-1.1.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-24 21:51:40.000000 text2text-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:54:16.670018 text2text-1.1.1/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-06-24 21:49:10.000000 text2text-1.1.1/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:54:16.671018 text2text-1.1.1/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-06-24 21:46:37.000000 text2text-1.1.1/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:54:16.673018 text2text-1.1.1/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-06-24 21:49:27.000000 text2text-1.1.1/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/searcher.py
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-24 20:16:12.000000 text2text-1.1.1/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12572 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-24 20:00:33.000000 text2text-1.1.1/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 21:54:16.671018 text2text-1.1.1/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    59869 2023-06-24 21:54:16.000000 text2text-1.1.1/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-06-24 21:54:16.000000 text2text-1.1.1/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 21:54:16.000000 text2text-1.1.1/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-24 21:54:16.000000 text2text-1.1.1/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-24 21:54:16.000000 text2text-1.1.1/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.1.0/LICENSE.txt` & `text2text-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/PKG-INFO` & `text2text-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: text2text
-Version: 1.1.0
-Summary: Text2Text: Crosslingual NLP/G toolkit
-Home-page: https://github.com/artitw/text2text
-Author: Artit Wangperawong
-Author-email: artitw@gmail.com
-Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # Text2Text: Crosslingual NLP/G toolkit
 Transform texts in a hundred different [languages](https://github.com/artitw/text2text#languages-available)!
 
 <details>
   <summary>Overview</summary>
 
 * [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
@@ -84,29 +70,14 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
-
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.1.0/README.md` & `text2text-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: text2text
+Version: 1.1.1
+Summary: Text2Text: Crosslingual NLP/G toolkit
+Home-page: https://github.com/artitw/text2text
+Author: Artit Wangperawong
+Author-email: artitw@gmail.com
+Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Text2Text: Crosslingual NLP/G toolkit
 Transform texts in a hundred different [languages](https://github.com/artitw/text2text#languages-available)!
 
 <details>
   <summary>Overview</summary>
 
 * [Colab Notebooks](https://github.com/artitw/text2text#colab-notebooks)
@@ -70,29 +84,14 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
-
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.1.0/setup.py` & `text2text-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.1.0",
+  version="1.1.1",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.1.0/text2text/__init__.py` & `text2text-1.1.1/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/abstractor.py` & `text2text-1.1.1/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/answerer.py` & `text2text-1.1.1/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/assistant.py` & `text2text-1.1.1/text2text/assistant.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,23 @@
       use_safetensors=True,
       trust_remote_code=False,
       device="cuda:0",
       use_triton=False,
       quantize_config=None
     )
 
-  def transform(self, input_lines, src_lang='en', knowledge_base=None, **kwargs):
+  def transform(self, input_lines, src_lang='en', retriever=None, **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang, **kwargs)
     df = pd.DataFrame({"input_line": input_lines})
     if src_lang != 'en':
       df["input_line"] = self._translate_lines(df["input_line"].tolist(), src_lang, 'en')
-    if knowledge_base:
-      corpus, index = knowledge_base
-      article_ids = index.search(df["input_line"].str.lower().tolist(), k=1)[1]
-      df["knowledge"] = [corpus[i[0]] for i in article_ids]
-      df["input_line"] = df["knowledge"] + " - " + df["input_line"]
+    if retriever:
+      k = kwargs.get('k', 1)
+      df["knowledge"] = retriever.retrieve(df["input_line"].str.lower().tolist(), k=k)
+      df["input_line"] = df["knowledge"].apply(' '.join) + " - " + df["input_line"]
     df["input_line"] = "USER: " + df["input_line"] + "\nASSISTANT:"
     temperature = kwargs.get('temperature', 0.7)
     top_p = kwargs.get('top_p', 0.9)
     top_k = kwargs.get('top_k', 0)
     repetition_penalty = kwargs.get('repetition_penalty', 1.1)
     max_new_tokens = kwargs.get('max_new_tokens', 512)
     tok = self.__class__.tokenizer
```

### Comparing `text2text-1.1.0/text2text/biunilm/loader_utils.py` & `text2text-1.1.1/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/biunilm/seq2seq_loader.py` & `text2text-1.1.1/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/bm25er.py` & `text2text-1.1.1/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/counter.py` & `text2text-1.1.1/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/fitter.py` & `text2text-1.1.1/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/handler.py` & `text2text-1.1.1/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/identifier.py` & `text2text-1.1.1/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/indexer.py` & `text2text-1.1.1/text2text/indexer.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,34 +18,42 @@
   def size(self, **kwargs):
     return self.index.ntotal
 
   def add(self, input_lines, src_lang='en', ids=[], faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     if not ids:
-      starting_id = 1+np.amax(faiss.vector_to_array(self.index.id_map), initial=0)
+      starting_id = np.amax(faiss.vector_to_array(self.index.id_map), initial=0)
       ids = list(range(starting_id, starting_id+len(input_lines)))
     v = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
     self.index.add_with_ids(v, np.array(ids))
+    self.corpus.append(input_lines)
     return self
 
   def remove(self, ids, faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     self.index.remove_ids(np.array(ids))
+    for i in ids:
+      del self.corpus[i]
 
   def search(self, input_lines, src_lang='en', k=3, faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     if not self.index or not self.index.ntotal:
       warnings.warn('Empty results because no index found. Make sure to build your index before searching.')
       return []
     xq = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
     return self.index.search(xq, k)
 
+  def retrieve(self, input_lines, k=3):
+    dist, pred_ids = self.search(input_lines, k=k)
+    return [[self.corpus[i] for i in line_ids] for line_ids in pred_ids]
+
   def transform(self, input_lines, src_lang='en', ids=[], encoders=[t2t.Tfidfer], **kwargs):
     self.encoders = encoders
     d = self.get_formatted_matrix(["DUMMY"], src_lang=src_lang, **kwargs).shape[-1]
     self.index = faiss.IndexIDMap2(faiss.IndexFlatL2(d))
+    self.corpus = input_lines
     if not input_lines:
       return self
     return self.add(input_lines, src_lang=src_lang, ids=ids, **kwargs)
```

### Comparing `text2text-1.1.0/text2text/measurer.py` & `text2text-1.1.1/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.1.1/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.1.1/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.1.1/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.1.1/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.1.1/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/questioner.py` & `text2text-1.1.1/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/responder.py` & `text2text-1.1.1/text2text/responder.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,33 +22,33 @@
         input_ids=inputs['input_ids'].to(model.device),
         attention_mask=inputs['attention_mask'],
         max_length=128, min_length=8,
     )
 
     return [tokenizer.decode(out, skip_special_tokens=True) for out in outputs]
 
-  def transform(self, input_lines, src_lang='en', knowledge_base=None, **kwargs):
+  def transform(self, input_lines, src_lang='en', retriever=None, **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang, **kwargs)
     df = pd.DataFrame({"input_line": input_lines})
     df.loc[len(df)] = "[CONTEXT][KNOWLEDGE]"
     cols = ["instruction", "context", "knowledge"]
     df[cols] = df["input_line"].str.split(r"\[CONTEXT\]|\[KNOWLEDGE\]", expand=True)
     df.drop(df.tail(1).index, inplace=True)
     df.fillna("", inplace=True)
     df[cols] = df[cols].apply(lambda x: x.str.strip())
 
     if src_lang != 'en':
       df["instruction"] = self._translate_lines(df["instruction"].tolist(), src_lang, 'en')
       df["context"] = self._translate_lines(df["context"].tolist(), src_lang, 'en')
       df["knowledge"] = self._translate_lines(df["knowledge"].tolist(), src_lang, 'en')
 
-    if knowledge_base:
-      corpus, index = knowledge_base
-      article_ids = index.search(df["context"].str.lower().tolist(), k=1)[1]
-      df["article"] = [corpus[i[0]] for i in article_ids]
+    if retriever:
+      k = kwargs.get('k', 1)
+      df["article"] = retriever.retrieve(df["input_line"].str.lower().tolist(), k=k)
+      df["article"] = df["article"].apply(' '.join)
       df["knowledge"] = df.apply(lambda row: row["article"] if not row["knowledge"] else row["knowledge"], axis=1)
 
     df["input_line"] = df["instruction"] + " [CONTEXT] " + df["context"]
     df["input_line"] = df.apply(lambda row: row["input_line"] + " [KNOWLEDGE] " + row["knowledge"] if row["knowledge"] else row["input_line"], axis=1)
     
     output_lines = self._get_responses(df["input_line"].tolist())
```

### Comparing `text2text-1.1.0/text2text/searcher.py` & `text2text-1.1.1/text2text/searcher.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/server.py` & `text2text-1.1.1/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/summarizer.py` & `text2text-1.1.1/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/tfidfer.py` & `text2text-1.1.1/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/tokenizer.py` & `text2text-1.1.1/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/transformer.py` & `text2text-1.1.1/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/translator.py` & `text2text-1.1.1/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text/vectorizer.py` & `text2text-1.1.1/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.0/text2text.egg-info/PKG-INFO` & `text2text-1.1.1/text2text.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.0
+Version: 1.1.1
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -84,29 +84,14 @@
 [Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
 [Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
 [Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
 [Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
 [Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
 [Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
 
-## Class Diagram
-```
-      Indexer    Measurer   Counter -- Tfidfer
-           \          \     /             \
-        Searcher     Tokenizer           Bm25er
-             \_______    |      ________________ Assistant
-              _______Transformer______________
-             /           |                    \
-        Answerer     Translator              Abstractor
-           /         /    |     \              /       \
-  Responder  Vectorizer  Fitter  Variator  Questioner  Summarizer
-                  /
-          Identifier
-```
-
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
```

### Comparing `text2text-1.1.0/text2text.egg-info/SOURCES.txt` & `text2text-1.1.1/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

