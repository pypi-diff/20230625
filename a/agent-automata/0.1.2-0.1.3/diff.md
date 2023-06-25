# Comparing `tmp/agent_automata-0.1.2.tar.gz` & `tmp/agent_automata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_automata-0.1.2.tar", max compression
+gzip compressed data, was "agent_automata-0.1.3.tar", max compression
```

## Comparing `agent_automata-0.1.2.tar` & `agent_automata-0.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-05-19 19:20:54.929118 agent_automata-0.1.2/LICENSE
--rw-r--r--   0        0        0     1814 2023-06-25 01:11:39.711901 agent_automata-0.1.2/README.md
--rw-r--r--   0        0        0       65 2023-06-19 04:29:05.701184 agent_automata-0.1.2/agent_automata/__init__.py
--rw-r--r--   0        0        0     5193 2023-06-25 00:46:46.593183 agent_automata-0.1.2/agent_automata/automaton.py
--rw-r--r--   0        0        0     1064 2023-06-20 01:10:38.682715 agent_automata-0.1.2/agent_automata/automaton_loading.py
--rw-r--r--   0        0        0       98 2023-06-19 16:49:13.050651 agent_automata-0.1.2/agent_automata/builtin_toolkit/__init__.py
--rw-r--r--   0        0        0     3147 2023-06-24 23:25:10.297036 agent_automata-0.1.2/agent_automata/builtin_toolkit/automaton_functions.py
--rw-r--r--   0        0        0      817 2023-06-24 23:25:20.497386 agent_automata-0.1.2/agent_automata/builtin_toolkit/engines.py
--rw-r--r--   0        0        0      417 2023-06-24 23:25:28.723909 agent_automata-0.1.2/agent_automata/builtin_toolkit/knowledge.py
--rw-r--r--   0        0        0     1252 2023-06-24 23:25:58.690557 agent_automata-0.1.2/agent_automata/builtin_toolkit/planners/__init__.py
--rw-r--r--   0        0        0       14 2023-06-19 23:50:26.240064 agent_automata-0.1.2/agent_automata/builtin_toolkit/planners/prompts.yml
--rw-r--r--   0        0        0     6384 2023-06-24 23:26:06.944833 agent_automata-0.1.2/agent_automata/builtin_toolkit/planners/react.py
--rw-r--r--   0        0        0      310 2023-06-24 23:25:36.095857 agent_automata-0.1.2/agent_automata/builtin_toolkit/reflectors.py
--rw-r--r--   0        0        0      420 2023-06-24 23:25:43.974894 agent_automata-0.1.2/agent_automata/builtin_toolkit/validators.py
--rw-r--r--   0        0        0      794 2023-06-19 15:55:56.006183 agent_automata-0.1.2/agent_automata/engines.py
--rw-r--r--   0        0        0     1067 2023-06-19 23:03:22.118975 agent_automata-0.1.2/agent_automata/knowledge.py
--rw-r--r--   0        0        0      921 2023-06-20 01:03:53.810061 agent_automata-0.1.2/agent_automata/planners.py
--rw-r--r--   0        0        0     1069 2023-06-19 23:04:30.926263 agent_automata-0.1.2/agent_automata/reflectors.py
--rw-r--r--   0        0        0     1836 2023-06-19 18:55:42.980689 agent_automata-0.1.2/agent_automata/sessions.py
--rw-r--r--   0        0        0     3361 2023-06-23 14:36:48.701074 agent_automata-0.1.2/agent_automata/types.py
--rw-r--r--   0        0        0      500 2023-06-19 04:31:28.381518 agent_automata-0.1.2/agent_automata/utilities/__init__.py
--rw-r--r--   0        0        0     1793 2023-06-20 12:37:49.606444 agent_automata-0.1.2/agent_automata/validators.py
--rw-r--r--   0        0        0      583 2023-06-25 00:02:13.934331 agent_automata-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2428 1970-01-01 00:00:00.000000 agent_automata-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 19:20:54.929118 agent_automata-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1816 2023-06-25 01:33:32.357891 agent_automata-0.1.3/README.md
+-rw-r--r--   0        0        0       65 2023-06-19 04:29:05.701184 agent_automata-0.1.3/agent_automata/__init__.py
+-rw-r--r--   0        0        0     5193 2023-06-25 00:46:46.593183 agent_automata-0.1.3/agent_automata/automaton.py
+-rw-r--r--   0        0        0     1064 2023-06-20 01:10:38.682715 agent_automata-0.1.3/agent_automata/automaton_loading.py
+-rw-r--r--   0        0        0       98 2023-06-19 16:49:13.050651 agent_automata-0.1.3/agent_automata/builtin_toolkit/__init__.py
+-rw-r--r--   0        0        0     3147 2023-06-24 23:25:10.297036 agent_automata-0.1.3/agent_automata/builtin_toolkit/automaton_functions.py
+-rw-r--r--   0        0        0      817 2023-06-24 23:25:20.497386 agent_automata-0.1.3/agent_automata/builtin_toolkit/engines.py
+-rw-r--r--   0        0        0      417 2023-06-24 23:25:28.723909 agent_automata-0.1.3/agent_automata/builtin_toolkit/knowledge.py
+-rw-r--r--   0        0        0     1252 2023-06-24 23:25:58.690557 agent_automata-0.1.3/agent_automata/builtin_toolkit/planners/__init__.py
+-rw-r--r--   0        0        0       14 2023-06-19 23:50:26.240064 agent_automata-0.1.3/agent_automata/builtin_toolkit/planners/prompts.yml
+-rw-r--r--   0        0        0     6384 2023-06-24 23:26:06.944833 agent_automata-0.1.3/agent_automata/builtin_toolkit/planners/react.py
+-rw-r--r--   0        0        0      310 2023-06-24 23:25:36.095857 agent_automata-0.1.3/agent_automata/builtin_toolkit/reflectors.py
+-rw-r--r--   0        0        0      420 2023-06-24 23:25:43.974894 agent_automata-0.1.3/agent_automata/builtin_toolkit/validators.py
+-rw-r--r--   0        0        0      794 2023-06-19 15:55:56.006183 agent_automata-0.1.3/agent_automata/engines.py
+-rw-r--r--   0        0        0     1067 2023-06-19 23:03:22.118975 agent_automata-0.1.3/agent_automata/knowledge.py
+-rw-r--r--   0        0        0      921 2023-06-20 01:03:53.810061 agent_automata-0.1.3/agent_automata/planners.py
+-rw-r--r--   0        0        0     1069 2023-06-19 23:04:30.926263 agent_automata-0.1.3/agent_automata/reflectors.py
+-rw-r--r--   0        0        0     1836 2023-06-19 18:55:42.980689 agent_automata-0.1.3/agent_automata/sessions.py
+-rw-r--r--   0        0        0     3361 2023-06-23 14:36:48.701074 agent_automata-0.1.3/agent_automata/types.py
+-rw-r--r--   0        0        0      500 2023-06-19 04:31:28.381518 agent_automata-0.1.3/agent_automata/utilities/__init__.py
+-rw-r--r--   0        0        0     1793 2023-06-20 12:37:49.606444 agent_automata-0.1.3/agent_automata/validators.py
+-rw-r--r--   0        0        0      579 2023-06-25 01:44:09.264997 agent_automata-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2426 1970-01-01 00:00:00.000000 agent_automata-0.1.3/PKG-INFO
```

### Comparing `agent_automata-0.1.2/LICENSE` & `agent_automata-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/README.md` & `agent_automata-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Agent Automata
 
 ## Introduction
-Agent automata is a lightweight orchestration architecture for a hierarchical group of modular, autonomous agents, with the goal of composing actions from simple autonomous agents into complex collective behavior.
+`agent-automata` is a lightweight orchestration architecture for a hierarchical group of modular, autonomous agents, with the goal of composing actions from simple autonomous agents into complex collective behavior.
 
 The core idea behind this architecture is that instead of having a complex central agent managing many commands and sub-agents, or a fixed set of agents with specific roles in a task loop, we modify Langchain agents to be able to call each other as tools, and then establish a hierarchical, rank-based structure to control the direction of the calls:
 ```
 Agent A (Rank 3):
   - Agent B (Rank 2)
     - Tool 1
     - Tool 2
```

### Comparing `agent_automata-0.1.2/agent_automata/automaton.py` & `agent_automata-0.1.3/agent_automata/automaton.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/automaton_loading.py` & `agent_automata-0.1.3/agent_automata/automaton_loading.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/builtin_toolkit/automaton_functions.py` & `agent_automata-0.1.3/agent_automata/builtin_toolkit/automaton_functions.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/builtin_toolkit/engines.py` & `agent_automata-0.1.3/agent_automata/builtin_toolkit/engines.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/builtin_toolkit/planners/__init__.py` & `agent_automata-0.1.3/agent_automata/builtin_toolkit/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/builtin_toolkit/planners/react.py` & `agent_automata-0.1.3/agent_automata/builtin_toolkit/planners/react.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/engines.py` & `agent_automata-0.1.3/agent_automata/engines.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/knowledge.py` & `agent_automata-0.1.3/agent_automata/knowledge.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/planners.py` & `agent_automata-0.1.3/agent_automata/planners.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/reflectors.py` & `agent_automata-0.1.3/agent_automata/reflectors.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/sessions.py` & `agent_automata-0.1.3/agent_automata/sessions.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/types.py` & `agent_automata-0.1.3/agent_automata/types.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/agent_automata/validators.py` & `agent_automata-0.1.3/agent_automata/validators.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.2/pyproject.toml` & `agent_automata-0.1.3/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "agent_automata"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
-authors = ["Mengyang (John) Cha <15233508+solarapparition@users.noreply.github.com>"]
+authors = ["solarapparition <15233508+solarapparition@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 PyYAML = ">=6.0"
 langchain = { version = ">=0.0.203", optional = true }
```

### Comparing `agent_automata-0.1.2/PKG-INFO` & `agent_automata-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agent-automata
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 License: MIT
-Author: Mengyang (John) Cha
+Author: solarapparition
 Author-email: 15233508+solarapparition@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: builtins
@@ -15,15 +15,15 @@
 Requires-Dist: langchain (>=0.0.203) ; extra == "builtins"
 Requires-Dist: openai (>=0.27.4) ; extra == "builtins"
 Description-Content-Type: text/markdown
 
 # Agent Automata
 
 ## Introduction
-Agent automata is a lightweight orchestration architecture for a hierarchical group of modular, autonomous agents, with the goal of composing actions from simple autonomous agents into complex collective behavior.
+`agent-automata` is a lightweight orchestration architecture for a hierarchical group of modular, autonomous agents, with the goal of composing actions from simple autonomous agents into complex collective behavior.
 
 The core idea behind this architecture is that instead of having a complex central agent managing many commands and sub-agents, or a fixed set of agents with specific roles in a task loop, we modify Langchain agents to be able to call each other as tools, and then establish a hierarchical, rank-based structure to control the direction of the calls:
 ```
 Agent A (Rank 3):
   - Agent B (Rank 2)
     - Tool 1
     - Tool 2
```

