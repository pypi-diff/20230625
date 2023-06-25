# Comparing `tmp/alphawave-0.2.7.tar.gz` & `tmp/alphawave-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.2.7.tar", last modified: Fri Jun 23 17:56:51 2023, max compression
+gzip compressed data, was "alphawave-0.2.8.tar", last modified: Sun Jun 25 03:56:26 2023, max compression
```

## Comparing `alphawave-0.2.7.tar` & `alphawave-0.2.8.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.7/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-23 17:56:51.298537 alphawave-0.2.7/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.7/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-23 17:56:44.000000 alphawave-0.2.7/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-23 17:56:51.298537 alphawave-0.2.7/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9267 2023-06-20 23:20:58.000000 alphawave-0.2.7/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.7/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.7/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.7/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.7/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.7/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.7/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.7/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.7/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.7/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.7/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.7/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.7/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.7/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.7/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1676 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-23 17:56:51.000000 alphawave-0.2.7/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.7/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.7/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.7/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.7/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.7/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.7/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.2.7/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.7/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.7/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.2.7/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.7/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.7/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.7/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.7/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6944 2023-06-23 17:13:40.000000 alphawave-0.2.7/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.7/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.2.7/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    21329 2023-06-23 16:43:17.000000 alphawave-0.2.7/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      813 2023-06-21 16:08:15.000000 alphawave-0.2.7/src/alphawave_pyexts/falcon.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      850 2023-06-21 22:46:07.000000 alphawave-0.2.7/src/alphawave_pyexts/falcon40.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.7/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6039 2023-06-22 03:24:44.000000 alphawave-0.2.7/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.2.7/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-23 17:56:51.298537 alphawave-0.2.7/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.7/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.7/tests/testOpenAiClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.7/tests/testSchema.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.2.8/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-25 03:56:26.108699 alphawave-0.2.8/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.2.8/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      945 2023-06-25 03:56:16.000000 alphawave-0.2.8/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-06-25 03:56:26.108699 alphawave-0.2.8/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9267 2023-06-20 23:20:58.000000 alphawave-0.2.8/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.2.8/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.2.8/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6405 2023-06-19 15:45:37.000000 alphawave-0.2.8/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.2.8/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8905 2023-06-19 15:46:26.000000 alphawave-0.2.8/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8916 2023-06-19 16:39:38.000000 alphawave-0.2.8/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-06-15 04:11:41.000000 alphawave-0.2.8/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.2.8/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.2.8/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.2.8/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.2.8/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1359 2023-06-15 04:10:27.000000 alphawave-0.2.8/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.2.8/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.2.8/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9441 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1758 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      155 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-06-25 03:56:26.000000 alphawave-0.2.8/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.104699 alphawave-0.2.8/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    16612 2023-06-19 22:45:42.000000 alphawave-0.2.8/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1332 2023-06-11 16:22:40.000000 alphawave-0.2.8/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2956 2023-06-19 02:42:43.000000 alphawave-0.2.8/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-06-11 19:07:37.000000 alphawave-0.2.8/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.2.8/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.2.8/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1425 2023-06-22 21:06:20.000000 alphawave-0.2.8/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1509 2023-06-07 03:15:08.000000 alphawave-0.2.8/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3130 2023-06-18 18:54:41.000000 alphawave-0.2.8/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3874 2023-06-23 16:34:08.000000 alphawave-0.2.8/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.2.8/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.2.8/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.2.8/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2134 2023-06-19 01:22:49.000000 alphawave-0.2.8/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.2.8/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7080 2023-06-25 00:20:00.000000 alphawave-0.2.8/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2687 2023-06-19 22:44:59.000000 alphawave-0.2.8/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.2.8/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.2.8/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    21511 2023-06-24 16:19:30.000000 alphawave-0.2.8/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.2.8/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13725 2023-06-19 22:24:29.000000 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-06-19 22:47:56.000000 alphawave-0.2.8/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.2.8/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12058 2023-06-25 03:39:18.000000 alphawave-0.2.8/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6684 2023-06-23 16:42:51.000000 alphawave-0.2.8/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-06-25 03:56:26.108699 alphawave-0.2.8/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.2.8/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.2.8/tests/testOpenAiClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      948 2023-06-06 20:59:59.000000 alphawave-0.2.8/tests/testSchema.py
```

### Comparing `alphawave-0.2.7/LICENSE` & `alphawave-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/PKG-INFO` & `alphawave-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.7
+Version: 0.2.8
 Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.7/README.md` & `alphawave-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/pyproject.toml` & `alphawave-0.2.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.2.7"
+version = "0.2.8"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave - a client for interfacing with Large Language Models (LLM)"
```

### Comparing `alphawave-0.2.7/src/alphawave/AlphaWave.py` & `alphawave-0.2.8/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/Colorize.py` & `alphawave-0.2.8/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.2.8/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/JSONResponseValidator.py` & `alphawave-0.2.8/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/MemoryFork.py` & `alphawave-0.2.8/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/OSClient.py` & `alphawave-0.2.8/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/OpenAIClient.py` & `alphawave-0.2.8/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/RepairTestClient.py` & `alphawave-0.2.8/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/Response.py` & `alphawave-0.2.8/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/TestClient.py` & `alphawave-0.2.8/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/TestClientTest.py` & `alphawave-0.2.8/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/alphawaveTypes.py` & `alphawave-0.2.8/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/internalTypes.py` & `alphawave-0.2.8/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave/jsonParser.py` & `alphawave-0.2.8/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.2.8/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.2.7
+Version: 0.2.8
 Summary: AlphaWave - a client for interfacing with Large Language Models (LLM)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.2.7/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.2.8/src/alphawave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,22 @@
 src/alphawave_agents/MathCommand.py
 src/alphawave_agents/PromptCommand.py
 src/alphawave_agents/SchemaBasedCommand.py
 src/alphawave_agents/SentimentAnalysis.py
 src/alphawave_agents/SetPropertyCommand.py
 src/alphawave_agents/__init__.py
 src/alphawave_agents/agentTypes.py
+src/alphawave_pyexts/FsInference.py
 src/alphawave_pyexts/LLMClient.py
 src/alphawave_pyexts/SearchCommand.py
 src/alphawave_pyexts/chat.py
+src/alphawave_pyexts/configuration_RW.py
 src/alphawave_pyexts/conversation.py
-src/alphawave_pyexts/falcon.py
-src/alphawave_pyexts/falcon40.py
+src/alphawave_pyexts/handler.py
+src/alphawave_pyexts/modelling_RW.py
 src/alphawave_pyexts/serverUtils.py
 src/alphawave_pyexts/utilityV2.py
 src/alphawave_pyexts/llmsearch/google_search_concurrent.py
 src/alphawave_pyexts/llmsearch/search_service.py
 tests/testOSClient.py
 tests/testOpenAiClient.py
 tests/testSchema.py
```

### Comparing `alphawave-0.2.7/src/alphawave_agents/Agent.py` & `alphawave-0.2.8/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.2.8/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.2.8/src/alphawave_agents/AgentCommandValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/AskCommand.py` & `alphawave-0.2.8/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.2.8/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.2.8/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.2.8/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/MathCommand.py` & `alphawave-0.2.8/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/PromptCommand.py` & `alphawave-0.2.8/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.2.8/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.2.8/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.2.8/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_agents/agentTypes.py` & `alphawave-0.2.8/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.2.8/src/alphawave_pyexts/LLMClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,46 +12,39 @@
 MODEL_NAME = None; WORKER_ADDR=None; CONTROLLER_ADDRESS = "http://localhost:21001"
 USER_PREFIX = 'user'
 ASSISTANT_PREFIX = 'assistant'
 SYSTEM_PREFIX = 'system'
 
 host='192.168.1.195'
 port = 5004
-cv.register_conv_template(Conversation(
-        name="dolly",
-        system="### Instruction",
-        roles=("### Input", "### Response"),
-        messages=(),
-        offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_TWO,
-        sep="\n",
-        sep2="### Response",
-    )
-)
-cv.register_conv_template(Conversation(
+
+cv.register_conv_template(
+    Conversation(
         name="falcon_instruct",
-        system="",
+        system="You are helpful, creative, clever, and very friendly.",
         roles=("User", "Assistant"),
         messages=(),
         offset=0,
-        sep_style=SeparatorStyle.ADD_COLON_TWO,
+        sep_style=SeparatorStyle.ADD_COLON_SINGLE,
+        stop_str=["User:"],
+        stop_token_ids=[11],
         sep="\n",
-        sep2="\nAssistant:\n",
+        sep2="<|endoftext|>",
+        first_msg_no_role=False,
     )
 )
-
 cv.register_conv_template(Conversation(
         name="guanaco",
         system="",
         roles=("Human", "Assistant"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_TWO,
         sep="\n",
-        sep2="Assistant:\n",
+        sep2="",
     )
 )
 cv.register_conv_template(Conversation(
         name="wizardLM",
         system="### Instruction",
         roles=("### Input", "### Response"),
         messages=(),
@@ -76,31 +69,36 @@
     USER_PREFIX = conv.roles[0]
     ASSISTANT_PREFIX = conv.roles[1]
     SYSTEM_PREFIX = conv.system
     
     # set this so client can check for run-on, although this test should pbly be here!
     if format:
         conv.system='' # no default prompt
-        for msg in messages:
-            #print(f'***** llm input msf {msg}')
+        for msg_idx, msg in enumerate(messages):
+            #if conv.first_msg_no_role and msg_idx ==0:
+            #    continue
             role = msg['role']
             ### conv.system is a prompt msg, and will be inserted as the first entry by conv.get_prompt()
-            if role.lower() == 'system':
-                conv.system = msg['content']
+            if role.lower() == 'system' and msg_idx==0:
+                if len(conv.roles)>2:
+                    conv.system=conv.roles[2]+msg['content']
+                else:
+                    conv.system = msg['content']
                 continue
-            elif role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
+            if role.lower() == 'user' or role.lower() == 'system' or role == conv.roles[0]:
                 role_index = 0
             else:
                 role_index = 1
             conv.append_message(conv.roles[role_index], msg['content'])
 
             #priming prompt
-            conv.append_message(conv.roles[1], '')
+        conv.append_message(conv.roles[1], '')
         prompt = conv.get_prompt()
-
+        if conv.first_msg_no_role:
+            prompt = messages[0]['content']+conv.sep+prompt
     else:
         prompt = messages
     prompt = re.sub('\n{3,}', '\n\n', prompt)
     #print(f'***** llm output prompt string {prompt}')
     server_message = {'prompt':prompt, 'temp': temp, 'top_p':top_p, 'max_tokens':max_tokens, 'user_prompt':USER_PREFIX}
     smj = json.dumps(server_message)
     try:
```

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.2.8/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/chat.py` & `alphawave-0.2.8/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/conversation.py` & `alphawave-0.2.8/src/alphawave_pyexts/conversation.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     sep_style: SeparatorStyle
     sep: str
     sep2: str = None
     # Stop criteria (the default one is EOS token)
     stop_str: str = None
     # Stops generation if meeting any token in this list
     stop_token_ids: List[int] = None
+    # prepends first msg text to front of prompt
+    first_msg_no_role:bool = False
 
     def get_prompt(self) -> str:
         """Get the prompt for generation."""
         if self.sep_style == SeparatorStyle.ADD_COLON_SINGLE:
             ret = self.system + self.sep
             for role, message in self.messages:
                 if message:
@@ -172,14 +174,15 @@
             messages=[[x, y] for x, y in self.messages],
             offset=self.offset,
             sep_style=self.sep_style,
             sep=self.sep,
             sep2=self.sep2,
             stop_str=self.stop_str,
             stop_token_ids=self.stop_token_ids,
+            first_msg_no_role=self.first_msg_no_role,
         )
 
     def dict(self):
         return {
             "template_name": self.name,
             "system": self.system,
             "roles": self.roles,
@@ -445,15 +448,15 @@
         name="mpt",
         system="""<|im_start|>system
 - You are a helpful assistant chatbot trained by MosaicML.
 - You answer questions.
 - You are excited to be able to help the user, but will refuse to do anything that could be considered harmful to the user.
 - You are more than just an information source, you are also able to write poetry, short stories, and make jokes.
 """,
-        roles=("<|im_start|>user", "<|im_start|>assistant"),
+        roles=("<|im_start|>user", "<|im_start|>assistant", "<|im_start|>system"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_NEW_LINE_SINGLE,
         sep="<|im_end|>",
         stop_token_ids=[50278, 0],
     )
 )
@@ -531,15 +534,15 @@
 
 # Snoozy default template
 # Reference: https://github.com/nomic-ai/gpt4all/blob/d4861030b778da6db59d21d2927a4aba4f9f1f43/gpt4all-bindings/python/gpt4all/gpt4all.py#L232
 register_conv_template(
     Conversation(
         name="snoozy",
         system="### Instruction:\nThe prompt below is a question to answer, a task to complete, or a conversation to respond to; decide which and write an appropriate response.",
-        roles=("### Prompt", "### Response"),
+        roles=("### Prompt", "### Response", "### Instruction:\n"),
         messages=(),
         offset=0,
         sep_style=SeparatorStyle.ADD_COLON_SINGLE,
         sep="\n",
         stop_str="###",
     )
 )
```

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.2.8/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.2.8/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.2.8/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/tests/testOSClient.py` & `alphawave-0.2.8/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/tests/testOpenAiClient.py` & `alphawave-0.2.8/tests/testOpenAiClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.2.7/tests/testSchema.py` & `alphawave-0.2.8/tests/testSchema.py`

 * *Files identical despite different names*

