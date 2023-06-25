# Comparing `tmp/text2text-1.1.3.tar.gz` & `tmp/text2text-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.1.3.tar", last modified: Sun Jun 25 05:05:30 2023, max compression
+gzip compressed data, was "text2text-1.1.4.tar", last modified: Sun Jun 25 05:23:45 2023, max compression
```

## Comparing `text2text-1.1.3.tar` & `text2text-1.1.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.660236 text2text-1.1.3/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-25 04:04:30.000000 text2text-1.1.3/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:05:30.660236 text2text-1.1.3/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    56554 2023-06-25 04:57:45.000000 text2text-1.1.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 05:05:30.660236 text2text-1.1.3/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-25 04:04:43.000000 text2text-1.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.656235 text2text-1.1.3/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      606 2023-06-25 04:37:26.000000 text2text-1.1.3/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-25 04:29:02.000000 text2text-1.1.3/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 04:30:23.000000 text2text-1.1.3/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-06-25 04:35:45.000000 text2text-1.1.3/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.658235 text2text-1.1.3/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-06-25 04:40:01.000000 text2text-1.1.3/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-06-25 04:46:04.000000 text2text-1.1.3/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.659236 text2text-1.1.3/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-06-25 04:56:07.000000 text2text-1.1.3/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12577 2023-06-25 04:45:49.000000 text2text-1.1.3/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.657235 text2text-1.1.3/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:23:45.241565 text2text-1.1.4/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-25 04:04:30.000000 text2text-1.1.4/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:23:45.241565 text2text-1.1.4/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    56554 2023-06-25 04:57:45.000000 text2text-1.1.4/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 05:23:45.241565 text2text-1.1.4/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-25 05:22:04.000000 text2text-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:23:45.237564 text2text-1.1.4/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      606 2023-06-25 04:37:26.000000 text2text-1.1.4/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-25 04:29:02.000000 text2text-1.1.4/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 04:30:23.000000 text2text-1.1.4/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-06-25 04:35:45.000000 text2text-1.1.4/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:23:45.239565 text2text-1.1.4/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-25 04:40:01.000000 text2text-1.1.4/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2023-06-25 05:15:40.000000 text2text-1.1.4/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:23:45.240565 text2text-1.1.4/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-06-25 04:56:07.000000 text2text-1.1.4/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      797 2023-06-25 05:21:35.000000 text2text-1.1.4/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-06-25 04:45:49.000000 text2text-1.1.4/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-25 04:04:30.000000 text2text-1.1.4/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:23:45.238565 text2text-1.1.4/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:23:45.000000 text2text-1.1.4/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-25 05:23:45.000000 text2text-1.1.4/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:23:45.000000 text2text-1.1.4/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-25 05:23:45.000000 text2text-1.1.4/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-25 05:23:45.000000 text2text-1.1.4/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.1.3/LICENSE.txt` & `text2text-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/PKG-INFO` & `text2text-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.3
+Version: 1.1.4
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.1.3/README.md` & `text2text-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/setup.py` & `text2text-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.1.3",
+  version="1.1.4",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.1.3/text2text/__init__.py` & `text2text-1.1.4/text2text/__init__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/abstractor.py` & `text2text-1.1.4/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/answerer.py` & `text2text-1.1.4/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/assistant.py` & `text2text-1.1.4/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/biunilm/loader_utils.py` & `text2text-1.1.4/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/biunilm/seq2seq_loader.py` & `text2text-1.1.4/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/bm25er.py` & `text2text-1.1.4/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/counter.py` & `text2text-1.1.4/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/fitter.py` & `text2text-1.1.4/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/handler.py` & `text2text-1.1.4/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/identifier.py` & `text2text-1.1.4/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/indexer.py` & `text2text-1.1.4/text2text/indexer.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   def add(self, input_lines, src_lang='en', faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     starting_id = np.amax(faiss.vector_to_array(self.index.id_map), initial=0)
     ids = list(range(starting_id, starting_id+len(input_lines)))
     v = self.get_formatted_matrix(input_lines, src_lang=src_lang, **kwargs)
     self.index.add_with_ids(v, np.array(ids))
-    self.corpus.append(input_lines)
+    self.corpus.append(list(input_lines))
     return self
 
   def remove(self, ids, faiss_index=None, **kwargs):
     if faiss_index is not None:
       self.index = faiss_index
     self.index.remove_ids(np.array(ids))
     for i in ids:
@@ -48,11 +48,11 @@
     distances, pred_ids = self.search(input_lines, k=k)
     return [[self.corpus[i] for i in line_ids] for line_ids in pred_ids]
 
   def transform(self, input_lines, src_lang='en', encoders=[t2t.Tfidfer], **kwargs):
     self.encoders = encoders
     d = self.get_formatted_matrix(["DUMMY"], src_lang=src_lang, **kwargs).shape[-1]
     self.index = faiss.IndexIDMap2(faiss.IndexFlatL2(d))
-    self.corpus = input_lines
+    self.corpus = []
     if not input_lines:
       return self
     return self.add(input_lines, src_lang=src_lang, **kwargs)
```

### Comparing `text2text-1.1.3/text2text/measurer.py` & `text2text-1.1.4/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.1.4/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.1.4/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.1.4/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.1.4/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.1.4/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/questioner.py` & `text2text-1.1.4/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/responder.py` & `text2text-1.1.4/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/server.py` & `text2text-1.1.4/text2text/server.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/summarizer.py` & `text2text-1.1.4/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/tfidfer.py` & `text2text-1.1.4/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/tokenizer.py` & `text2text-1.1.4/text2text/tokenizer.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     pretrained_translator = self.__class__.PRETRAINED_TRANSLATOR
     self.__class__.tokenizer = AutoTokenizer.from_pretrained(pretrained_translator)
 
   def transform(self, input_lines, src_lang='en', output='tokens', **kwargs):
     input_lines = t2t.Transformer.transform(self, input_lines, src_lang=src_lang, **kwargs)
     tokenizer = self.__class__.tokenizer
     tokenizer.src_lang = src_lang
-    encoded_inputs = tokenizer(input_lines, add_special_tokens=False)
+    encoded_inputs = tokenizer(input_lines, add_special_tokens=False, truncation=True)
     if output == 'ids':
       return encoded_inputs["input_ids"]
     return [
       tokenizer.convert_ids_to_tokens(input_ids) 
       for input_ids in encoded_inputs["input_ids"]
     ]
```

### Comparing `text2text-1.1.3/text2text/transformer.py` & `text2text-1.1.4/text2text/transformer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/translator.py` & `text2text-1.1.4/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text/vectorizer.py` & `text2text-1.1.4/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.3/text2text.egg-info/PKG-INFO` & `text2text-1.1.4/text2text.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.3
+Version: 1.1.4
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `text2text-1.1.3/text2text.egg-info/SOURCES.txt` & `text2text-1.1.4/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

