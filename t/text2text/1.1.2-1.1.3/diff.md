# Comparing `tmp/text2text-1.1.2.tar.gz` & `tmp/text2text-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "text2text-1.1.2.tar", last modified: Sat Jun 24 22:46:45 2023, max compression
+gzip compressed data, was "text2text-1.1.3.tar", last modified: Sun Jun 25 05:05:30 2023, max compression
```

## Comparing `text2text-1.1.2.tar` & `text2text-1.1.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:46:45.604496 text2text-1.1.2/
--rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-24 22:08:59.000000 text2text-1.1.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    57467 2023-06-24 22:46:45.604496 text2text-1.1.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    56653 2023-06-24 22:45:52.000000 text2text-1.1.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-24 22:46:45.604496 text2text-1.1.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-24 22:15:13.000000 text2text-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:46:45.600496 text2text-1.1.2/text2text/
--rwxr-xr-x   0 root         (0) root         (0)      635 2023-06-24 22:13:25.000000 text2text-1.1.2/text2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7162 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/abstractor.py
--rw-r--r--   0 root         (0) root         (0)     2157 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/answerer.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/assistant.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:46:45.602496 text2text-1.1.2/text2text/biunilm/
--rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/biunilm/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/biunilm/loader_utils.py
--rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/biunilm/seq2seq_loader.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/bm25er.py
--rw-r--r--   0 root         (0) root         (0)      519 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/counter.py
--rw-r--r--   0 root         (0) root         (0)     1177 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/fitter.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-06-24 22:13:39.000000 text2text-1.1.2/text2text/handler.py
--rw-r--r--   0 root         (0) root         (0)     2106 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/identifier.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-06-24 22:35:17.000000 text2text-1.1.2/text2text/indexer.py
--rw-r--r--   0 root         (0) root         (0)     1165 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/measurer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:46:45.603496 text2text-1.1.2/text2text/pytorch_pretrained_bert/
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/__main__.py
--rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/file_utils.py
--rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/loss.py
--rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/modeling.py
--rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/pytorch_pretrained_bert/tokenization.py
--rw-r--r--   0 root         (0) root         (0)     1782 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/questioner.py
--rw-r--r--   0 root         (0) root         (0)     2589 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/responder.py
--rw-r--r--   0 root         (0) root         (0)     1575 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/server.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/summarizer.py
--rw-r--r--   0 root         (0) root         (0)     1766 2023-06-24 22:12:07.000000 text2text-1.1.2/text2text/tfidfer.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)    12572 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/transformer.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/translator.py
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/variator.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-06-24 22:08:59.000000 text2text-1.1.2/text2text/vectorizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-24 22:46:45.601496 text2text-1.1.2/text2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)    57467 2023-06-24 22:46:45.000000 text2text-1.1.2/text2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1042 2023-06-24 22:46:45.000000 text2text-1.1.2/text2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-24 22:46:45.000000 text2text-1.1.2/text2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      134 2023-06-24 22:46:45.000000 text2text-1.1.2/text2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-24 22:46:45.000000 text2text-1.1.2/text2text.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.660236 text2text-1.1.3/
+-rwxr-xr-x   0 root         (0) root         (0)     1418 2023-06-25 04:04:30.000000 text2text-1.1.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:05:30.660236 text2text-1.1.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)    56554 2023-06-25 04:57:45.000000 text2text-1.1.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-25 05:05:30.660236 text2text-1.1.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1246 2023-06-25 04:04:43.000000 text2text-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.656235 text2text-1.1.3/text2text/
+-rwxr-xr-x   0 root         (0) root         (0)      606 2023-06-25 04:37:26.000000 text2text-1.1.3/text2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7162 2023-06-25 04:29:02.000000 text2text-1.1.3/text2text/abstractor.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2023-06-25 04:30:23.000000 text2text-1.1.3/text2text/answerer.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-06-25 04:35:45.000000 text2text-1.1.3/text2text/assistant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.658235 text2text-1.1.3/text2text/biunilm/
+-rwxr-xr-x   0 root         (0) root         (0)      110 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    10937 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/loader_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    17726 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/biunilm/seq2seq_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/bm25er.py
+-rw-r--r--   0 root         (0) root         (0)      519 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/counter.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/fitter.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-06-25 04:40:01.000000 text2text-1.1.3/text2text/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/identifier.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-06-25 04:46:04.000000 text2text-1.1.3/text2text/indexer.py
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/measurer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.659236 text2text-1.1.3/text2text/pytorch_pretrained_bert/
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      932 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/__main__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7964 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/file_utils.py
+-rwxr-xr-x   0 root         (0) root         (0)     1821 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/loss.py
+-rwxr-xr-x   0 root         (0) root         (0)   108506 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/modeling.py
+-rwxr-xr-x   0 root         (0) root         (0)    15035 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/pytorch_pretrained_bert/tokenization.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/questioner.py
+-rw-r--r--   0 root         (0) root         (0)     2589 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/responder.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-06-25 04:56:07.000000 text2text-1.1.3/text2text/server.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/summarizer.py
+-rw-r--r--   0 root         (0) root         (0)     1766 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/tfidfer.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)    12577 2023-06-25 04:45:49.000000 text2text-1.1.3/text2text/transformer.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/translator.py
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/variator.py
+-rw-r--r--   0 root         (0) root         (0)      816 2023-06-25 04:04:30.000000 text2text-1.1.3/text2text/vectorizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:05:30.657235 text2text-1.1.3/text2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    57368 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      134 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-25 05:05:30.000000 text2text-1.1.3/text2text.egg-info/top_level.txt
```

### Comparing `text2text-1.1.2/LICENSE.txt` & `text2text-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/PKG-INFO` & `text2text-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.2
+Version: 1.1.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,32 +63,31 @@
 ```
 * [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Assistant().transform("Describe Text2Text in a few words: ")` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Language Model Setting](https://github.com/artitw/text2text#byot-bring-your-own-translator) | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
-Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
-[Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
-[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
-[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
-[BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
-[Indexer](https://github.com/artitw/text2text#index) | `index = h.index()` | Index object for information retrieval
-[Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
-[Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
-[Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
-[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
-[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
-[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
-[Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
-[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
+[Tokenization](https://github.com/artitw/text2text#tokenization) | `t2t.Tokenizer().transform(["Hello, World!"])` | `[['▁Hello', ',', '▁World', '!']]`
+[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `t2t.Vectorizer().transform(["Hello, World!"])` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
+[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `t2t.Tfidfer().transform(["Hello, World!"])` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
+[BM25](https://github.com/artitw/text2text#bm25) | `t2t.Bm25er().transform(["Hello, World!"])` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
+[Indexer](https://github.com/artitw/text2text#index) | `index = t2t.Indexer().transform(["Hello, World!"])` | Index object for information retrieval
+[Translation](https://github.com/artitw/text2text#translation) | `t2t.Translater().transform(["Hello, World!"], src_lang="en, tgt_lang="zh")` | `['你好,世界!']`
+[Question Generation](https://github.com/artitw/text2text#question-generation) | `t2t.Questioner().transform(["Hello, World!"], src_lang="en)` | `[('What is the name of the world you are in?', 'The world')]`
+[Summarization](https://github.com/artitw/text2text#summarization) | `t2t.Summarizer().transform(["Hello, World!"], src_lang="en)` | `["World ' s largest world"]`
+[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `t2t.Variator().transform(["Hello, World!"], src_lang="en)` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Responder().transform(["[CONTEXT] Hello EOS How are you?"])` | `['I am doing great. How are you?']`
+[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Answerer().transform(["Hello, World! [SEP] Hello, what?"], src_lang="en")` | `['World']`
+[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Measurer().transform(["Hello, World! [SEP] Hello, what?"])` | `[2]`
+[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Fitter().transform(["Hello, World! [TGT] Hello, what?"])` | Finetuned model saved
+[Identification](https://github.com/artitw/text2text#identification) | `t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."])` | `['sk', 'Slovak']`
+[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Serve(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
@@ -203,58 +202,58 @@
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 Not ChatGPT level but it works well.
 To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
+res = t2t.Assistant().transform([instructions])
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tokenize()
+t2t.Tokenizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).vectorize()
+t2t.Vectorizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
          0.05118701,  0.01895813],
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tfidf()
+t2t.Tfidfer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
   'ing': 0.22360679774997894,
   'orrow': 0.22360679774997894,
@@ -275,19 +274,19 @@
   '세요': 0.3535533905932738,
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).bm25()
+t2t.Bm25er().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
   's': 1.2792257271403649,
   '▁Let': 1.2792257271403649,
@@ -304,19 +303,19 @@
   '을': 1.2792257271403649,
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
-index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~",
-         ]).index()
+index = t2t.Indexer().transform([
+  "Let's go hiking tomorrow, let's go!",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~",
+])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
@@ -325,18 +324,18 @@
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
 ```
-t2t.Handler([
-         "Hello, World! [SEP] Hello, what?",
-         "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
-        ]).measure(metric="levenshtein_distance")
+t2t.Measurer().transform([
+  "Hello, World! [SEP] Hello, what?",
+  "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
+], metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
@@ -345,20 +344,20 @@
 
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
-t2t.Handler([
-         article_en,
-         notre_dame_str,
-         bacteria_str,
-         bio_str
-         ], src_lang='en').translate(tgt_lang='zh')
+t2t.Translator().transform([
+  article_en,
+  notre_dame_str,
+  bacteria_str,
+  bio_str
+], src_lang='en', tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
@@ -423,59 +422,61 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."],
-        src_lang="en_XX"
-        ).translate(tgt_lang='zh_CN')
+t2t.Translator().transform(
+  ["I would like to go hiking tomorrow."],
+  src_lang="en_XX",
+  tgt_lang='zh_CN'
+)
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
-t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?",
-         "It works very well. It's awesome! [SEP] How is it?"
-         ]).answer()
-
-t2t.Handler([
-             "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
-             ], src_lang="zh").answer()
+t2t.Answerer().transform([
+  "Hello, this is Text2Text! [SEP] What is this?",
+  "It works very well. It's awesome! [SEP] How is it?"
+])
+
+t2t.Answerer().transform([
+  "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
+], src_lang="zh")
 
 # Answers
 ['Text2Text', 'awesome']
 ['唱歌']
 ```
 
 ### Question Generation
 ```
-t2t.Handler(["很喜欢陈慧琳唱歌。"], src_lang='zh').question()
-t2t.Handler([
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            "I will go to school today to take my math exam.",
-            "I will go to school today to take my math exam.",
-            "Tomorrow is my cousin's birthday. He will turn 24 years old.",
-            notre_dame_str,
-            bacteria_str,
-            bacteria_str,
-            bacteria_str,
-            "I will go to school today to take my math exam. [SEP] school",
-            "I will go to school today to take my math exam. [SEP] exam",
-            "I will go to school today to take my math exam. [SEP] math",
-          ], src_lang='en').question()
+t2t.Questioner().transform(["很喜欢陈慧琳唱歌。"], src_lang='zh')
+t2t.Questioner().transform([
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  "I will go to school today to take my math exam.",
+  "I will go to school today to take my math exam.",
+  "Tomorrow is my cousin's birthday. He will turn 24 years old.",
+  notre_dame_str,
+  bacteria_str,
+  bacteria_str,
+  bacteria_str,
+  "I will go to school today to take my math exam. [SEP] school",
+  "I will go to school today to take my math exam. [SEP] exam",
+  "I will go to school today to take my math exam. [SEP] math",
+], src_lang='en')
 
 ```
 Note that the last three answers were controlled by specifying the `[SEP]` token in the input above.
 ```
 # Questions
 [('我喜欢做什么?', '唱歌')]
 [('What is biology the science that studies?', 'life'),
@@ -493,26 +494,26 @@
  ('Where will I go to to take my math exam?', 'school'),
  ('What will I take after school?', 'exam'),
  ('What exam will I take?', 'math')]
 ```
 
 ### Summarization
 ```
-t2t.Handler([notre_dame_str, bacteria_str, bio_str], src_lang='en').summarize()
+t2t.Summarizer().transform([notre_dame_str, bacteria_str, bio_str], src_lang='en')
 
 # Summaries
 ["Notre Dame's students run nine student - run outlets . [X_SEP] Scholastic magazine claims to be the oldest continuous collegiate publication in the United States . [X_SEP] The Observer is an independent publication .",
  'Bacteria were among the first life forms to appear on Earth .',
  'biology is the science that studies life .']
 ```
 
 ### Data Augmentation / Back-Translation
 Back-translations useful for augmenting training data
 ```
-t2t.Handler([bacteria_str], src_lang='en').variate()
+t2t.Variator().transform([bacteria_str], src_lang='en')
 ```
 
 <details>
   <summary>Show results</summary>
 
 ```
 # Variations
@@ -633,37 +634,37 @@
 ]
 
 if knowledge != '':
     knowledge = '[KNOWLEDGE] ' + knowledge
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
-t2t.Handler([input_state]).respond()
+t2t.Responder().transform([input_state])
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
-            src_lang="en",
-            tgt_lang="zh",
-            num_epochs=10,
-            save_directory="model_dir"
-            ).fit()
+result = t2t.Fitter().transform(["Hello, World! [TGT] 你好,世界!"],
+  src_lang="en",
+  tgt_lang="zh",
+  num_epochs=10,
+  save_directory="model_dir"
+)
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
-t2t.Handler("Hello, World!").translate(tgt_lang="zh")
+t2t.Translator().transform("Hello, World!", src_lang="en", tgt_lang="zh")
 ```
 
 ### Identification
 Identify the language of a text. Not yet accurate for short sequences (<10 tokens)
 ```
-t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",]).identify()
+t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",])
 
 # Prediction
 `['sk', 'Slovak']`
 ```
 
 ### Serving
 We aim to serve all functionality above
```

### Comparing `text2text-1.1.2/README.md` & `text2text-1.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -49,32 +49,31 @@
 ```
 * [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Assistant().transform("Describe Text2Text in a few words: ")` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Language Model Setting](https://github.com/artitw/text2text#byot-bring-your-own-translator) | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
-Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
-[Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
-[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
-[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
-[BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
-[Indexer](https://github.com/artitw/text2text#index) | `index = h.index()` | Index object for information retrieval
-[Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
-[Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
-[Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
-[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
-[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
-[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
-[Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
-[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
+[Tokenization](https://github.com/artitw/text2text#tokenization) | `t2t.Tokenizer().transform(["Hello, World!"])` | `[['▁Hello', ',', '▁World', '!']]`
+[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `t2t.Vectorizer().transform(["Hello, World!"])` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
+[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `t2t.Tfidfer().transform(["Hello, World!"])` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
+[BM25](https://github.com/artitw/text2text#bm25) | `t2t.Bm25er().transform(["Hello, World!"])` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
+[Indexer](https://github.com/artitw/text2text#index) | `index = t2t.Indexer().transform(["Hello, World!"])` | Index object for information retrieval
+[Translation](https://github.com/artitw/text2text#translation) | `t2t.Translater().transform(["Hello, World!"], src_lang="en, tgt_lang="zh")` | `['你好,世界!']`
+[Question Generation](https://github.com/artitw/text2text#question-generation) | `t2t.Questioner().transform(["Hello, World!"], src_lang="en)` | `[('What is the name of the world you are in?', 'The world')]`
+[Summarization](https://github.com/artitw/text2text#summarization) | `t2t.Summarizer().transform(["Hello, World!"], src_lang="en)` | `["World ' s largest world"]`
+[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `t2t.Variator().transform(["Hello, World!"], src_lang="en)` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Responder().transform(["[CONTEXT] Hello EOS How are you?"])` | `['I am doing great. How are you?']`
+[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Answerer().transform(["Hello, World! [SEP] Hello, what?"], src_lang="en")` | `['World']`
+[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Measurer().transform(["Hello, World! [SEP] Hello, what?"])` | `[2]`
+[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Fitter().transform(["Hello, World! [TGT] Hello, what?"])` | Finetuned model saved
+[Identification](https://github.com/artitw/text2text#identification) | `t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."])` | `['sk', 'Slovak']`
+[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Serve(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
@@ -189,58 +188,58 @@
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 Not ChatGPT level but it works well.
 To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
+res = t2t.Assistant().transform([instructions])
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tokenize()
+t2t.Tokenizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).vectorize()
+t2t.Vectorizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
          0.05118701,  0.01895813],
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tfidf()
+t2t.Tfidfer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
   'ing': 0.22360679774997894,
   'orrow': 0.22360679774997894,
@@ -261,19 +260,19 @@
   '세요': 0.3535533905932738,
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).bm25()
+t2t.Bm25er().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
   's': 1.2792257271403649,
   '▁Let': 1.2792257271403649,
@@ -290,19 +289,19 @@
   '을': 1.2792257271403649,
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
-index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~",
-         ]).index()
+index = t2t.Indexer().transform([
+  "Let's go hiking tomorrow, let's go!",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~",
+])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
@@ -311,18 +310,18 @@
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
 ```
-t2t.Handler([
-         "Hello, World! [SEP] Hello, what?",
-         "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
-        ]).measure(metric="levenshtein_distance")
+t2t.Measurer().transform([
+  "Hello, World! [SEP] Hello, what?",
+  "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
+], metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
@@ -331,20 +330,20 @@
 
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
-t2t.Handler([
-         article_en,
-         notre_dame_str,
-         bacteria_str,
-         bio_str
-         ], src_lang='en').translate(tgt_lang='zh')
+t2t.Translator().transform([
+  article_en,
+  notre_dame_str,
+  bacteria_str,
+  bio_str
+], src_lang='en', tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
@@ -409,59 +408,61 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."],
-        src_lang="en_XX"
-        ).translate(tgt_lang='zh_CN')
+t2t.Translator().transform(
+  ["I would like to go hiking tomorrow."],
+  src_lang="en_XX",
+  tgt_lang='zh_CN'
+)
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
-t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?",
-         "It works very well. It's awesome! [SEP] How is it?"
-         ]).answer()
-
-t2t.Handler([
-             "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
-             ], src_lang="zh").answer()
+t2t.Answerer().transform([
+  "Hello, this is Text2Text! [SEP] What is this?",
+  "It works very well. It's awesome! [SEP] How is it?"
+])
+
+t2t.Answerer().transform([
+  "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
+], src_lang="zh")
 
 # Answers
 ['Text2Text', 'awesome']
 ['唱歌']
 ```
 
 ### Question Generation
 ```
-t2t.Handler(["很喜欢陈慧琳唱歌。"], src_lang='zh').question()
-t2t.Handler([
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            "I will go to school today to take my math exam.",
-            "I will go to school today to take my math exam.",
-            "Tomorrow is my cousin's birthday. He will turn 24 years old.",
-            notre_dame_str,
-            bacteria_str,
-            bacteria_str,
-            bacteria_str,
-            "I will go to school today to take my math exam. [SEP] school",
-            "I will go to school today to take my math exam. [SEP] exam",
-            "I will go to school today to take my math exam. [SEP] math",
-          ], src_lang='en').question()
+t2t.Questioner().transform(["很喜欢陈慧琳唱歌。"], src_lang='zh')
+t2t.Questioner().transform([
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  "I will go to school today to take my math exam.",
+  "I will go to school today to take my math exam.",
+  "Tomorrow is my cousin's birthday. He will turn 24 years old.",
+  notre_dame_str,
+  bacteria_str,
+  bacteria_str,
+  bacteria_str,
+  "I will go to school today to take my math exam. [SEP] school",
+  "I will go to school today to take my math exam. [SEP] exam",
+  "I will go to school today to take my math exam. [SEP] math",
+], src_lang='en')
 
 ```
 Note that the last three answers were controlled by specifying the `[SEP]` token in the input above.
 ```
 # Questions
 [('我喜欢做什么?', '唱歌')]
 [('What is biology the science that studies?', 'life'),
@@ -479,26 +480,26 @@
  ('Where will I go to to take my math exam?', 'school'),
  ('What will I take after school?', 'exam'),
  ('What exam will I take?', 'math')]
 ```
 
 ### Summarization
 ```
-t2t.Handler([notre_dame_str, bacteria_str, bio_str], src_lang='en').summarize()
+t2t.Summarizer().transform([notre_dame_str, bacteria_str, bio_str], src_lang='en')
 
 # Summaries
 ["Notre Dame's students run nine student - run outlets . [X_SEP] Scholastic magazine claims to be the oldest continuous collegiate publication in the United States . [X_SEP] The Observer is an independent publication .",
  'Bacteria were among the first life forms to appear on Earth .',
  'biology is the science that studies life .']
 ```
 
 ### Data Augmentation / Back-Translation
 Back-translations useful for augmenting training data
 ```
-t2t.Handler([bacteria_str], src_lang='en').variate()
+t2t.Variator().transform([bacteria_str], src_lang='en')
 ```
 
 <details>
   <summary>Show results</summary>
 
 ```
 # Variations
@@ -619,37 +620,37 @@
 ]
 
 if knowledge != '':
     knowledge = '[KNOWLEDGE] ' + knowledge
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
-t2t.Handler([input_state]).respond()
+t2t.Responder().transform([input_state])
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
-            src_lang="en",
-            tgt_lang="zh",
-            num_epochs=10,
-            save_directory="model_dir"
-            ).fit()
+result = t2t.Fitter().transform(["Hello, World! [TGT] 你好,世界!"],
+  src_lang="en",
+  tgt_lang="zh",
+  num_epochs=10,
+  save_directory="model_dir"
+)
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
-t2t.Handler("Hello, World!").translate(tgt_lang="zh")
+t2t.Translator().transform("Hello, World!", src_lang="en", tgt_lang="zh")
 ```
 
 ### Identification
 Identify the language of a text. Not yet accurate for short sequences (<10 tokens)
 ```
-t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",]).identify()
+t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",])
 
 # Prediction
 `['sk', 'Slovak']`
 ```
 
 ### Serving
 We aim to serve all functionality above
```

### Comparing `text2text-1.1.2/setup.py` & `text2text-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="text2text",
-  version="1.1.2",
+  version="1.1.3",
   author="Artit Wangperawong",
   author_email="artitw@gmail.com",
   description="Text2Text: Crosslingual NLP/G toolkit",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/artitw/text2text",
   packages=setuptools.find_packages(),
```

### Comparing `text2text-1.1.2/text2text/__init__.py` & `text2text-1.1.3/text2text/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 from .variator import Variator
 from .abstractor import Abstractor
 from .questioner import Questioner
 from .summarizer import Summarizer
 from .answerer import Answerer
 from .responder import Responder
 from .identifier import Identifier
-from .handler import Handler
 from .server import Server
```

### Comparing `text2text-1.1.2/text2text/abstractor.py` & `text2text-1.1.3/text2text/abstractor.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/answerer.py` & `text2text-1.1.3/text2text/answerer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/assistant.py` & `text2text-1.1.3/text2text/assistant.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/biunilm/loader_utils.py` & `text2text-1.1.3/text2text/biunilm/loader_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/biunilm/seq2seq_loader.py` & `text2text-1.1.3/text2text/biunilm/seq2seq_loader.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/bm25er.py` & `text2text-1.1.3/text2text/bm25er.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/counter.py` & `text2text-1.1.3/text2text/counter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/fitter.py` & `text2text-1.1.3/text2text/fitter.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/handler.py` & `text2text-1.1.3/text2text/handler.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/identifier.py` & `text2text-1.1.3/text2text/identifier.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/indexer.py` & `text2text-1.1.3/text2text/indexer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/measurer.py` & `text2text-1.1.3/text2text/measurer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/pytorch_pretrained_bert/__main__.py` & `text2text-1.1.3/text2text/pytorch_pretrained_bert/__main__.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/pytorch_pretrained_bert/file_utils.py` & `text2text-1.1.3/text2text/pytorch_pretrained_bert/file_utils.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/pytorch_pretrained_bert/loss.py` & `text2text-1.1.3/text2text/pytorch_pretrained_bert/loss.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/pytorch_pretrained_bert/modeling.py` & `text2text-1.1.3/text2text/pytorch_pretrained_bert/modeling.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/pytorch_pretrained_bert/tokenization.py` & `text2text-1.1.3/text2text/pytorch_pretrained_bert/tokenization.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/questioner.py` & `text2text-1.1.3/text2text/questioner.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/responder.py` & `text2text-1.1.3/text2text/responder.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/server.py` & `text2text-1.1.3/text2text/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,44 +6,44 @@
 
 app = Flask(__name__)
 
 @app.route("/", methods=['GET', 'POST'])
 def hello():
   return {"result": "Hello, this Text2Text at your service."}
 
-@app.route('/index/<action>', methods=['POST'])
-def index(action):
+@app.route('/indexer/<action>', methods=['POST'])
+def indexer(action):
   try:
-    indexer = t2t.Server.indexer
-    assert hasattr(indexer, action)
     data = request.get_json() or {}
     input_lines = data.get("input_lines", [])
     src_lang = data.get("src_lang", "en")
-    res = getattr(indexer, action)(**data)
+    if hasattr(t2t.Server, "index"):
+      index = t2t.Server.index
+    else:
+      t2t.Server.index = t2t.Indexer().add(input_lines)
+    assert hasattr(index, action)
+    res = getattr(index, action)(**data)
     if action in ["search", "size"]:
       return {"result": np.array(res).tolist()}
   except Exception as e:
     return {"result": str(e)}
-  return {"result": f"index/{action} performed"}
+  return {"result": f"indexer/{action} performed"}
 
-@app.route('/<transformation>', methods=['POST'])
-def transform(transformation):
+@app.route('/<transformer>', methods=['POST'])
+def transform(transformer):
   try:
-    assert transformation in t2t.Handler.EXPOSED_TRANSFORMERS
+    assert hasattr(t2t, transformer)
     data = request.get_json() or {}
     input_lines = data.get("input_lines", [])
     src_lang = data.get("src_lang", "en")
-    h = t2t.Handler(input_lines, src_lang)
+    res = getattr(t2t, transformer)(input_lines, src_lang)
     del data["input_lines"]
     del data["src_lang"]
-    res = getattr(h, transformation)(**data)
-    res = getattr(res, "tolist", lambda: res)()
     return {"result": res}
   except Exception as e:
     return {"result": str(e)}
 
 class Server(object):
   def __init__(self, **kwargs):
-    self.__class__.indexer = t2t.Handler().index()
     address = socket.gethostbyname(socket.getfqdn(socket.gethostname()))
     print(f"Serving at http://{address}/")
     threading.Thread(target=app.run, kwargs=kwargs).start()
```

### Comparing `text2text-1.1.2/text2text/summarizer.py` & `text2text-1.1.3/text2text/summarizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/tfidfer.py` & `text2text-1.1.3/text2text/tfidfer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/tokenizer.py` & `text2text-1.1.3/text2text/tokenizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/transformer.py` & `text2text-1.1.3/text2text/transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,14 +107,15 @@
     'zu': 'Zulu'
   }
 
   SEED = 123
 
   def __init__(self):
     pass
+    
   def transform(self, input_lines, src_lang='en', **kwargs):
     if src_lang not in self.__class__.LANGUAGES:
       raise ValueError(f'{src_lang} not found in {self.__class__.LANGUAGES}')
     self.__class__.src_lang = src_lang
     if type(input_lines) == str:
       input_lines = [input_lines]
     elif type(input_lines) != list:
```

### Comparing `text2text-1.1.2/text2text/translator.py` & `text2text-1.1.3/text2text/translator.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text/vectorizer.py` & `text2text-1.1.3/text2text/vectorizer.py`

 * *Files identical despite different names*

### Comparing `text2text-1.1.2/text2text.egg-info/PKG-INFO` & `text2text-1.1.3/text2text.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: text2text
-Version: 1.1.2
+Version: 1.1.3
 Summary: Text2Text: Crosslingual NLP/G toolkit
 Home-page: https://github.com/artitw/text2text
 Author: Artit Wangperawong
 Author-email: artitw@gmail.com
 Keywords: multilingual crosslingual gpt chatgpt bert natural language processing nlp nlg text generation gpt question answer answering information retrieval tfidf tf-idf bm25 search index summary summarizer summarization tokenizer tokenization translation backtranslation data augmentation science machine learning colab embedding levenshtein sub-word edit distance conversational dialog chatbot
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -63,32 +63,31 @@
 ```
 * [Examples](#examples) run with <16 GB RAM on free [Colab GPUs](https://colab.research.google.com/drive/1LE_ifTpOGO5QJCKNQYtZe6c_tjbwnulR).
 
 ## Quick Start Guide
 Functionality | Invocation | Result
 :------------: | :-------------: | :-------------:
 Module Importing | `import text2text as t2t` | Libraries imported
-[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Handler("Describe Text2Text in a few words: ").assist()` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
+[Assistant](https://github.com/artitw/text2text#assistant) | `t2t.Assistant().transform("Describe Text2Text in a few words: ")` | `['Text2Text is an AI-powered text generation tool that creates coherent and continuous text based on prompts.']`
 [Language Model Setting](https://github.com/artitw/text2text#byot-bring-your-own-translator) | `t2t.Transformer.PRETRAINED_TRANSLATOR = "facebook/m2m100_418M"` | Change from default
-Text Handler | `h = t2t.Handler(["Hello, World!"], src_lang="en")` | Initialized handler with some text
-[Tokenization](https://github.com/artitw/text2text#tokenization) | `h.tokenize()` | `[['▁Hello', ',', '▁World', '!']]`
-[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `h.vectorize()` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
-[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `h.tfidf()` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
-[BM25](https://github.com/artitw/text2text#bm25) | `h.bm25()` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
-[Indexer](https://github.com/artitw/text2text#index) | `index = h.index()` | Index object for information retrieval
-[Translation](https://github.com/artitw/text2text#translation) | `h.translate(tgt_lang="zh")` | `['你好,世界!']`
-[Question Generation](https://github.com/artitw/text2text#question-generation) | `h.question()` | `[('What is the name of the world you are in?', 'The world')]`
-[Summarization](https://github.com/artitw/text2text#summarization) | `h.summarize()` | `["World ' s largest world"]`
-[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `h.variate()` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
-[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Handler(["[CONTEXT] Hello EOS How are you?"]).respond()` | `['I am doing great. How are you?']`
-[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).answer()` | `['World']`
-[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Handler(["Hello, World! [SEP] Hello, what?"]).measure()` | `[2]`
-[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Handler(["Hello, World! [TGT] Hello, what?"]).fit()` | Finetuned model saved
-[Identification](https://github.com/artitw/text2text#identification) | `t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."]).identify()` | `['sk', 'Slovak']`
-[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Server(host='0.0.0.0', port=80)` | Web server started on host and port
+[Tokenization](https://github.com/artitw/text2text#tokenization) | `t2t.Tokenizer().transform(["Hello, World!"])` | `[['▁Hello', ',', '▁World', '!']]`
+[Embedding](https://github.com/artitw/text2text#embedding--vectorization) | `t2t.Vectorizer().transform(["Hello, World!"])` | `array([[0.18745188, 0.05658336, ..., 0.6332584 , 0.43805206]], dtype=float32)`
+[TF-IDF](https://github.com/artitw/text2text#tf-idf) | `t2t.Tfidfer().transform(["Hello, World!"])` | `[{'!': 0.5, ',': 0.5, '▁Hello': 0.5, '▁World': 0.5}]`
+[BM25](https://github.com/artitw/text2text#bm25) | `t2t.Bm25er().transform(["Hello, World!"])` | `[{'!': 0.3068528194400547, ',': 0.3068528194400547, '▁Hello': 0.3068528194400547, '▁World': 0.3068528194400547}]`
+[Indexer](https://github.com/artitw/text2text#index) | `index = t2t.Indexer().transform(["Hello, World!"])` | Index object for information retrieval
+[Translation](https://github.com/artitw/text2text#translation) | `t2t.Translater().transform(["Hello, World!"], src_lang="en, tgt_lang="zh")` | `['你好,世界!']`
+[Question Generation](https://github.com/artitw/text2text#question-generation) | `t2t.Questioner().transform(["Hello, World!"], src_lang="en)` | `[('What is the name of the world you are in?', 'The world')]`
+[Summarization](https://github.com/artitw/text2text#summarization) | `t2t.Summarizer().transform(["Hello, World!"], src_lang="en)` | `["World ' s largest world"]`
+[Data Augmentation](https://github.com/artitw/text2text#data-augmentation--back-translation) | `t2t.Variator().transform(["Hello, World!"], src_lang="en)` | `['Hello the world!', 'Welcome to the world.', 'Hello to the world!',...`
+[Dialog Response](https://github.com/artitw/text2text#dialog-responder) | `t2t.Responder().transform(["[CONTEXT] Hello EOS How are you?"])` | `['I am doing great. How are you?']`
+[Question Answering](https://github.com/artitw/text2text#question-answering) | `t2t.Answerer().transform(["Hello, World! [SEP] Hello, what?"], src_lang="en")` | `['World']`
+[Distance](https://github.com/artitw/text2text#levenshtein-sub-word-edit-distance) | `t2t.Measurer().transform(["Hello, World! [SEP] Hello, what?"])` | `[2]`
+[Training/Finetuning](https://github.com/artitw/text2text#training--finetuning) | `t2t.Fitter().transform(["Hello, World! [TGT] Hello, what?"])` | Finetuned model saved
+[Identification](https://github.com/artitw/text2text#identification) | `t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“..."])` | `['sk', 'Slovak']`
+[Web Server](https://github.com/artitw/text2text#serving) | `t2t.Serve(host='0.0.0.0', port=80)` | Web server started on host and port
 
 ## Languages Available
 <details>
   <summary>Show all</summary>
 
 ```
 t2t.Transformer.LANGUAGES
@@ -203,58 +202,58 @@
 
 ### Assistant
 Based on Vicuna 13B, which is based on LLaMA, which is not commercially licensed.
 Not ChatGPT level but it works well.
 To use a dynamic knowledge base, see [![Q&A Assistant Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1hkNgpSmmUA-mzUibqz25xq-E8KYOLuVx?usp=sharing)
 ```
 instructions = "Generate a JSON object that maps English characters as keys and Greek equivalents as values: {"
-res = t2t.Handler([instructions]).assist()
+res = t2t.Assistant().transform([instructions])
 #[
 #  '{\n"a": "α",\n"b": "β",\n"c": "γ",\n"d": "δ",\n"e": "ε",\n"f": "φ",\n"g": "χ",\n"h": "ι",\n"i": "η",\n"j": "κ",\n"k": "λ",\n"l": "μ",\n"m": "ν",\n"n": "ξ",\n"o": "ο",\n"p": "π",\n"q": "ρ",\n"r": "σ",\n"s": "τ",\n"t": "υ",\n"u": "ύ",\n"v": "φ",\n"w": "χ",\n"x": "ψ",\n"y": "ω",\n"z": "ζ"\n}'
 #]
 ```
 
 ### Tokenization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tokenize()
+t2t.Tokenizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Sub-word tokens
 [['▁Let', "'", 's', '▁go', '▁hik', 'ing', '▁tom', 'orrow'],
  ['▁안녕', '하세요', '.'],
  ['▁', '돼', '지', '꿈', '을', '▁꾸', '세요', '~~']]
 ```
 
 ### Embedding / Vectorization
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).vectorize()
+t2t.Vectorizer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # Embeddings
 array([[-0.00352954,  0.0260059 ,  0.00407429, ..., -0.04830331,
         -0.02540749, -0.00924972],
        [ 0.00043362,  0.00249816,  0.01755436, ...,  0.04451273,
          0.05118701,  0.01895813],
        [-0.03563676, -0.04856304,  0.00518898, ..., -0.00311068,
          0.00071953, -0.00216325]])
 ```
 
 ### TF-IDF
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).tfidf()
+t2t.Tfidfer().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # TF-IDF values
 [{'!': 0.22360679774997894,
   "'": 0.44721359549995787,
   ',': 0.22360679774997894,
   'ing': 0.22360679774997894,
   'orrow': 0.22360679774997894,
@@ -275,19 +274,19 @@
   '세요': 0.3535533905932738,
   '을': 0.3535533905932738,
   '지': 0.3535533905932738}]
 ```
 
 ### BM25
 ```
-t2t.Handler([
-         "Let's go hiking tomorrow",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~"
-         ]).bm25()
+t2t.Bm25er().transform([
+  "Let's go hiking tomorrow",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~"
+])
 
 # BM25 values
 [{"'": 1.2792257271403649,
   'ing': 1.2792257271403649,
   'orrow': 1.2792257271403649,
   's': 1.2792257271403649,
   '▁Let': 1.2792257271403649,
@@ -304,19 +303,19 @@
   '을': 1.2792257271403649,
   '지': 1.2792257271403649}]
 ```
 
 ### Index
 [![STF-IDF Demo](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1RaWj5SqWvyC2SsCTGg8IAVcl9G5hOB50?usp=sharing)
 ```
-index = t2t.Handler([
-         "Let's go hiking tomorrow, let's go!",
-         "안녕하세요.",
-         "돼지꿈을 꾸세요~~",
-         ]).index()
+index = t2t.Indexer().transform([
+  "Let's go hiking tomorrow, let's go!",
+  "안녕하세요.",
+  "돼지꿈을 꾸세요~~",
+])
 
 index.retrieve(["돼지"], k=1) #[['"돼지꿈을 꾸세요~~"']]
 
 # Add documents incrementing on ids if none specified
 index.add(["Hello, World! 你好,世界!"])
 
 # Remove by ids
@@ -325,18 +324,18 @@
 # Retrieve k results per query sorted by distance
 index.retrieve(["你好, World"], k=3)
 ```
 To learn more, see [STF-IDF](https://arxiv.org/abs/2209.14281).
 
 ### Levenshtein Sub-word Edit Distance
 ```
-t2t.Handler([
-         "Hello, World! [SEP] Hello, what?",
-         "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
-        ]).measure(metric="levenshtein_distance")
+t2t.Measurer().transform([
+  "Hello, World! [SEP] Hello, what?",
+  "안녕하세요. [SEP] 돼지꿈을 꾸세요~~"
+], metric="levenshtein_distance")
 
 # Distances
  [2, 8]
 ```
 
 ### Translation
 ```
@@ -345,20 +344,20 @@
 
 notre_dame_str = "As at most other universities, Notre Dame's students run a number of news media outlets. The nine student - run outlets include three newspapers, both a radio and television station, and several magazines and journals. Begun as a one - page journal in September 1876, the Scholastic magazine is issued twice monthly and claims to be the oldest continuous collegiate publication in the United States. The other magazine, The Juggler, is released twice a year and focuses on student literature and artwork. The Dome yearbook is published annually. The newspapers have varying publication interests, with The Observer published daily and mainly reporting university and other news, and staffed by students from both Notre Dame and Saint Mary's College. Unlike Scholastic and The Dome, The Observer is an independent publication and does not have a faculty advisor or any editorial oversight from the University. In 1987, when some students believed that The Observer began to show a conservative bias, a liberal newspaper, Common Sense was published. Likewise, in 2003, when other students believed that the paper showed a liberal bias, the conservative paper Irish Rover went into production. Neither paper is published as often as The Observer; however, all three are distributed to all students. Finally, in Spring 2008 an undergraduate journal for political science research, Beyond Politics, made its debut."
 
 bacteria_str = "Bacteria are a type of biological cell. They constitute a large domain of prokaryotic microorganisms. Typically a few micrometres in length, bacteria have a number of shapes, ranging from spheres to rods and spirals. Bacteria were among the first life forms to appear on Earth, and are present in most of its habitats."
 
 bio_str = "Biology is the science that studies life. What exactly is life? This may sound like a silly question with an obvious answer, but it is not easy to define life. For example, a branch of biology called virology studies viruses, which exhibit some of the characteristics of living entities but lack others. It turns out that although viruses can attack living organisms, cause diseases, and even reproduce, they do not meet the criteria that biologists use to define life."
 
-t2t.Handler([
-         article_en,
-         notre_dame_str,
-         bacteria_str,
-         bio_str
-         ], src_lang='en').translate(tgt_lang='zh')
+t2t.Translator().transform([
+  article_en,
+  notre_dame_str,
+  bacteria_str,
+  bio_str
+], src_lang='en', tgt_lang='zh')
 
 # Translations
 ['联合国秘书长说,叙利亚没有军事解决方案。',
  '与大多数其他大学一样,Notre Dame的学生运行的新闻媒体渠道的数量。九个学生 - 运行的渠道包括三份报纸,两台广播电视台,以及几本杂志和杂志。 开始作为一个一页的杂志在1876年9月,该杂志的Schoolistic发行了每月两次,并声称是美国最古老的连续的大学新闻出版物,和其他杂志,TheJuggler,每年发行两次,并专注于学生文学和艺术作品。 多姆年刊每年发行。 报纸有不同的出版利益,与The Observer发表每日,主要报道大学和其他新闻,并由学生从Notre Dame和圣玛丽的学院。 与Scholastic和The Dome不同,The Observer是一个独立的公众作品,但没有教师顾',
  '细菌是生物细胞的一种类型. 它们构成一个大范围的亲生微生物. 通常几微米长,细菌有许多形状,从球到杖和螺旋。 细菌是地球上出现的第一个生命形式之一,并且存在于其大多数栖息地。',
  '生物学是研究生命的科学. 究竟什么是生命? 这可能听起来像一个愚蠢的问题,有一个显而易见的答案,但它并不容易定义生命. 例如,一个名为病毒学的生物学分支研究病毒,这些病毒表现出一些活体的特征,但缺乏其他。']
 ```
@@ -423,59 +422,61 @@
   'tr_TR': 'Turkish',
   'uk_UA': 'Ukrainian',
   'ur_PK': 'Urdu',
   'vi_VN': 'Vietnamese',
   'xh_ZA': 'Xhosa',
   'zh_CN': 'Chinese'
 }
-t2t.Handler(["I would like to go hiking tomorrow."],
-        src_lang="en_XX"
-        ).translate(tgt_lang='zh_CN')
+t2t.Translator().transform(
+  ["I would like to go hiking tomorrow."],
+  src_lang="en_XX",
+  tgt_lang='zh_CN'
+)
 ['我想明天去徒步旅行。']
 ```
 
 </details>
 
 ### Question Answering
 Question must follow context with ` [SEP] ` in between.
 ```
-t2t.Handler([
-         "Hello, this is Text2Text! [SEP] What is this?",
-         "It works very well. It's awesome! [SEP] How is it?"
-         ]).answer()
-
-t2t.Handler([
-             "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
-             ], src_lang="zh").answer()
+t2t.Answerer().transform([
+  "Hello, this is Text2Text! [SEP] What is this?",
+  "It works very well. It's awesome! [SEP] How is it?"
+])
+
+t2t.Answerer().transform([
+  "很喜欢陈慧琳唱歌。[SEP] 喜欢做什么?"
+], src_lang="zh")
 
 # Answers
 ['Text2Text', 'awesome']
 ['唱歌']
 ```
 
 ### Question Generation
 ```
-t2t.Handler(["很喜欢陈慧琳唱歌。"], src_lang='zh').question()
-t2t.Handler([
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            bio_str,
-            "I will go to school today to take my math exam.",
-            "I will go to school today to take my math exam.",
-            "Tomorrow is my cousin's birthday. He will turn 24 years old.",
-            notre_dame_str,
-            bacteria_str,
-            bacteria_str,
-            bacteria_str,
-            "I will go to school today to take my math exam. [SEP] school",
-            "I will go to school today to take my math exam. [SEP] exam",
-            "I will go to school today to take my math exam. [SEP] math",
-          ], src_lang='en').question()
+t2t.Questioner().transform(["很喜欢陈慧琳唱歌。"], src_lang='zh')
+t2t.Questioner().transform([
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  bio_str,
+  "I will go to school today to take my math exam.",
+  "I will go to school today to take my math exam.",
+  "Tomorrow is my cousin's birthday. He will turn 24 years old.",
+  notre_dame_str,
+  bacteria_str,
+  bacteria_str,
+  bacteria_str,
+  "I will go to school today to take my math exam. [SEP] school",
+  "I will go to school today to take my math exam. [SEP] exam",
+  "I will go to school today to take my math exam. [SEP] math",
+], src_lang='en')
 
 ```
 Note that the last three answers were controlled by specifying the `[SEP]` token in the input above.
 ```
 # Questions
 [('我喜欢做什么?', '唱歌')]
 [('What is biology the science that studies?', 'life'),
@@ -493,26 +494,26 @@
  ('Where will I go to to take my math exam?', 'school'),
  ('What will I take after school?', 'exam'),
  ('What exam will I take?', 'math')]
 ```
 
 ### Summarization
 ```
-t2t.Handler([notre_dame_str, bacteria_str, bio_str], src_lang='en').summarize()
+t2t.Summarizer().transform([notre_dame_str, bacteria_str, bio_str], src_lang='en')
 
 # Summaries
 ["Notre Dame's students run nine student - run outlets . [X_SEP] Scholastic magazine claims to be the oldest continuous collegiate publication in the United States . [X_SEP] The Observer is an independent publication .",
  'Bacteria were among the first life forms to appear on Earth .',
  'biology is the science that studies life .']
 ```
 
 ### Data Augmentation / Back-Translation
 Back-translations useful for augmenting training data
 ```
-t2t.Handler([bacteria_str], src_lang='en').variate()
+t2t.Variator().transform([bacteria_str], src_lang='en')
 ```
 
 <details>
   <summary>Show results</summary>
 
 ```
 # Variations
@@ -633,37 +634,37 @@
 ]
 
 if knowledge != '':
     knowledge = '[KNOWLEDGE] ' + knowledge
 dialog = ' EOS '.join(dialog)
 input_state = f"{instruction} [CONTEXT] {dialog} {knowledge}"
 
-t2t.Handler([input_state]).respond()
+t2t.Responder().transform([input_state])
 # ['About 60 different kinds of cats are recognized by various cat registries.']
 ```
 
 ### Training / Finetuning
 Finetune cross-lingual model on your data
 ```
-result = t2t.Handler(["Hello, World! [TGT] 你好,世界!"],
-            src_lang="en",
-            tgt_lang="zh",
-            num_epochs=10,
-            save_directory="model_dir"
-            ).fit()
+result = t2t.Fitter().transform(["Hello, World! [TGT] 你好,世界!"],
+  src_lang="en",
+  tgt_lang="zh",
+  num_epochs=10,
+  save_directory="model_dir"
+)
 
 # load and use model from saved directory
 t2t.Transformer.PRETRAINED_TRANSLATOR = "model_dir"
-t2t.Handler("Hello, World!").translate(tgt_lang="zh")
+t2t.Translator().transform("Hello, World!", src_lang="en", tgt_lang="zh")
 ```
 
 ### Identification
 Identify the language of a text. Not yet accurate for short sequences (<10 tokens)
 ```
-t2t.Handler(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",]).identify()
+t2t.Identifier().transform(["Aj keď sa Buzz Aldrin stal až „druhým človekom“, ktorý otlačil svoju nohu do povrchu Mesiaca...",])
 
 # Prediction
 `['sk', 'Slovak']`
 ```
 
 ### Serving
 We aim to serve all functionality above
```

### Comparing `text2text-1.1.2/text2text.egg-info/SOURCES.txt` & `text2text-1.1.3/text2text.egg-info/SOURCES.txt`

 * *Files identical despite different names*

