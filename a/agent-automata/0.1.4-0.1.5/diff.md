# Comparing `tmp/agent_automata-0.1.4.tar.gz` & `tmp/agent_automata-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agent_automata-0.1.4.tar", max compression
+gzip compressed data, was "agent_automata-0.1.5.tar", max compression
```

## Comparing `agent_automata-0.1.4.tar` & `agent_automata-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,74 @@
--rw-r--r--   0        0        0     1067 2023-05-19 19:20:54.929118 agent_automata-0.1.4/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-25 01:46:36.090001 agent_automata-0.1.4/README.md
--rw-r--r--   0        0        0       65 2023-06-19 04:29:05.701184 agent_automata-0.1.4/agent_automata/__init__.py
--rw-r--r--   0        0        0     5193 2023-06-25 00:46:46.593183 agent_automata-0.1.4/agent_automata/automaton.py
--rw-r--r--   0        0        0     1064 2023-06-20 01:10:38.682715 agent_automata-0.1.4/agent_automata/automaton_loading.py
--rw-r--r--   0        0        0       98 2023-06-19 16:49:13.050651 agent_automata-0.1.4/agent_automata/builtin_toolkit/__init__.py
--rw-r--r--   0        0        0     3147 2023-06-24 23:25:10.297036 agent_automata-0.1.4/agent_automata/builtin_toolkit/automaton_functions.py
--rw-r--r--   0        0        0      817 2023-06-24 23:25:20.497386 agent_automata-0.1.4/agent_automata/builtin_toolkit/engines.py
--rw-r--r--   0        0        0      417 2023-06-24 23:25:28.723909 agent_automata-0.1.4/agent_automata/builtin_toolkit/knowledge.py
--rw-r--r--   0        0        0     1252 2023-06-24 23:25:58.690557 agent_automata-0.1.4/agent_automata/builtin_toolkit/planners/__init__.py
--rw-r--r--   0        0        0       14 2023-06-19 23:50:26.240064 agent_automata-0.1.4/agent_automata/builtin_toolkit/planners/prompts.yml
--rw-r--r--   0        0        0     6384 2023-06-24 23:26:06.944833 agent_automata-0.1.4/agent_automata/builtin_toolkit/planners/react.py
--rw-r--r--   0        0        0      310 2023-06-24 23:25:36.095857 agent_automata-0.1.4/agent_automata/builtin_toolkit/reflectors.py
--rw-r--r--   0        0        0      420 2023-06-24 23:25:43.974894 agent_automata-0.1.4/agent_automata/builtin_toolkit/validators.py
--rw-r--r--   0        0        0      794 2023-06-19 15:55:56.006183 agent_automata-0.1.4/agent_automata/engines.py
--rw-r--r--   0        0        0     1067 2023-06-19 23:03:22.118975 agent_automata-0.1.4/agent_automata/knowledge.py
--rw-r--r--   0        0        0      921 2023-06-20 01:03:53.810061 agent_automata-0.1.4/agent_automata/planners.py
--rw-r--r--   0        0        0     1069 2023-06-19 23:04:30.926263 agent_automata-0.1.4/agent_automata/reflectors.py
--rw-r--r--   0        0        0     1836 2023-06-19 18:55:42.980689 agent_automata-0.1.4/agent_automata/sessions.py
--rw-r--r--   0        0        0     3361 2023-06-23 14:36:48.701074 agent_automata-0.1.4/agent_automata/types.py
--rw-r--r--   0        0        0      500 2023-06-19 04:31:28.381518 agent_automata-0.1.4/agent_automata/utilities/__init__.py
--rw-r--r--   0        0        0     1793 2023-06-20 12:37:49.606444 agent_automata-0.1.4/agent_automata/validators.py
--rw-r--r--   0        0        0      579 2023-06-25 01:47:14.386767 agent_automata-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 agent_automata-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-19 19:20:54.929118 agent_automata-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-25 01:46:36.090001 agent_automata-0.1.5/README.md
+-rw-r--r--   0        0        0       65 2023-06-19 04:29:05.701184 agent_automata-0.1.5/agent_automata/__init__.py
+-rw-r--r--   0        0        0     5248 2023-06-25 03:37:14.286630 agent_automata-0.1.5/agent_automata/automaton.py
+-rw-r--r--   0        0        0     1064 2023-06-20 01:10:38.682715 agent_automata-0.1.5/agent_automata/automaton_loading.py
+-rw-r--r--   0        0        0       98 2023-06-19 16:49:13.050651 agent_automata-0.1.5/agent_automata/builtin_toolkit/__init__.py
+-rw-r--r--   0        0        0      300 2023-06-19 18:10:20.737110 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4688 2023-06-24 23:27:00.081671 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/automaton_functions.cpython-311.pyc
+-rw-r--r--   0        0        0     1783 2023-06-24 23:27:00.108941 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/engines.cpython-311.pyc
+-rw-r--r--   0        0        0     1024 2023-06-24 23:27:00.118250 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/knowledge.cpython-311.pyc
+-rw-r--r--   0        0        0     1780 2023-06-19 23:23:50.665222 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/planners.cpython-311.pyc
+-rw-r--r--   0        0        0      876 2023-06-24 23:27:00.132105 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/reflectors.cpython-311.pyc
+-rw-r--r--   0        0        0     1030 2023-06-24 23:27:00.136532 agent_automata-0.1.5/agent_automata/builtin_toolkit/__pycache__/validators.cpython-311.pyc
+-rw-r--r--   0        0        0     3242 2023-06-25 03:44:50.656917 agent_automata-0.1.5/agent_automata/builtin_toolkit/automaton_functions.py
+-rw-r--r--   0        0        0      817 2023-06-24 23:25:20.497386 agent_automata-0.1.5/agent_automata/builtin_toolkit/engines.py
+-rw-r--r--   0        0        0      417 2023-06-24 23:25:28.723909 agent_automata-0.1.5/agent_automata/builtin_toolkit/knowledge.py
+-rw-r--r--   0        0        0     1252 2023-06-24 23:25:58.690557 agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-24 23:27:00.123160 agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     9786 2023-06-25 03:40:32.860793 agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/__pycache__/react.cpython-311.pyc
+-rw-r--r--   0        0        0       14 2023-06-19 23:50:26.240064 agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/prompts.yml
+-rw-r--r--   0        0        0     6829 2023-06-25 03:38:43.571864 agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/react.py
+-rw-r--r--   0        0        0      310 2023-06-24 23:25:36.095857 agent_automata-0.1.5/agent_automata/builtin_toolkit/reflectors.py
+-rw-r--r--   0        0        0      420 2023-06-24 23:25:43.974894 agent_automata-0.1.5/agent_automata/builtin_toolkit/validators.py
+-rw-r--r--   0        0        0      794 2023-06-19 15:55:56.006183 agent_automata-0.1.5/agent_automata/engines.py
+-rw-r--r--   0        0        0     1067 2023-06-19 23:03:22.118975 agent_automata-0.1.5/agent_automata/knowledge.py
+-rw-r--r--   0        0        0      921 2023-06-20 01:03:53.810061 agent_automata-0.1.5/agent_automata/planners.py
+-rw-r--r--   0        0        0     1069 2023-06-19 23:04:30.926263 agent_automata-0.1.5/agent_automata/reflectors.py
+-rw-r--r--   0        0        0     1844 2023-06-25 03:42:59.388230 agent_automata-0.1.5/agent_automata/sessions.py
+-rw-r--r--   0        0        0     3361 2023-06-23 14:36:48.701074 agent_automata-0.1.5/agent_automata/types.py
+-rw-r--r--   0        0        0     2929 2023-06-19 15:37:20.514074 agent_automata-0.1.5/agent_automata/uncommitted/llm_function.py
+-rw-r--r--   0        0        0       65 2023-05-07 19:34:46.145109 agent_automata-0.1.5/agent_automata/uncommitted/old/__init__.py
+-rw-r--r--   0        0        0     5331 2023-06-18 14:50:35.671182 agent_automata-0.1.5/agent_automata/uncommitted/old/builtin_functions.py
+-rw-r--r--   0        0        0     6989 2023-06-19 18:55:42.969336 agent_automata-0.1.5/agent_automata/uncommitted/old/core.py
+-rw-r--r--   0        0        0    12288 2023-06-18 15:04:30.154360 agent_automata-0.1.5/agent_automata/uncommitted/old/db/resource_metadata.db
+-rw-r--r--   0        0        0      418 2023-06-19 01:19:58.497268 agent_automata-0.1.5/agent_automata/uncommitted/old/engines.py
+-rw-r--r--   0        0        0     2728 2023-06-09 12:31:01.805547 agent_automata-0.1.5/agent_automata/uncommitted/old/indexing.py
+-rw-r--r--   0        0        0      500 2023-06-03 17:46:00.149172 agent_automata-0.1.5/agent_automata/uncommitted/old/knowledge.py
+-rw-r--r--   0        0        0     2929 2023-06-19 00:55:42.726334 agent_automata-0.1.5/agent_automata/uncommitted/old/llm_function.py
+-rw-r--r--   0        0        0      902 2023-06-11 03:09:50.221747 agent_automata-0.1.5/agent_automata/uncommitted/old/loaders.py
+-rw-r--r--   0        0        0     1088 2023-06-19 01:19:58.498915 agent_automata-0.1.5/agent_automata/uncommitted/old/planners.py
+-rw-r--r--   0        0        0      758 2023-05-31 00:04:19.006782 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/automaton.yml
+-rw-r--r--   0        0        0     1247 2023-05-04 13:40:58.013110 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/uncommitted/bot.yml
+-rw-r--r--   0        0        0     2571 2023-04-25 13:42:03.481828 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/uncommitted/orchestrator.yml
+-rw-r--r--   0        0        0     1950 2023-05-31 00:04:24.370934 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/uncommitted/researcher.yml
+-rw-r--r--   0        0        0        0 2023-04-20 05:12:16.202565 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/uncommitted/strategist.yml
+-rw-r--r--   0        0        0     1857 2023-05-06 14:19:27.141807 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/uncommitted/visionary.yml
+-rw-r--r--   0        0        0     2010 2023-06-09 12:37:36.865647 agent_automata-0.1.5/agent_automata/uncommitted/old/prompts/roles/worker.yml
+-rw-r--r--   0        0        0     7155 2023-06-19 15:07:14.494892 agent_automata-0.1.5/agent_automata/uncommitted/old/reasoning.py
+-rw-r--r--   0        0        0      568 2023-06-03 17:39:42.679866 agent_automata-0.1.5/agent_automata/uncommitted/old/reflection.py
+-rw-r--r--   0        0        0     3182 2023-06-09 12:31:01.806028 agent_automata-0.1.5/agent_automata/uncommitted/old/resource_metadata.py
+-rw-r--r--   0        0        0     2034 2023-06-11 03:10:26.824531 agent_automata-0.1.5/agent_automata/uncommitted/old/sessions.py
+-rw-r--r--   0        0        0     1119 2023-06-19 01:19:58.499729 agent_automata-0.1.5/agent_automata/uncommitted/old/types.py
+-rw-r--r--   0        0        0      219 2023-05-31 00:04:19.008336 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-18 13:27:24.770441 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13007 2023-04-15 01:38:51.244913 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0      518 2023-05-31 13:52:41.000000 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3137 2023-04-15 01:38:51.246280 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/analyze_package.cpython-38.pyc
+-rw-r--r--   0        0        0     4843 2023-05-07 19:43:30.068683 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/analyze_package.cpython-39.pyc
+-rw-r--r--   0        0        0      958 2023-06-18 13:27:47.320347 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/importing.cpython-311.pyc
+-rw-r--r--   0        0        0      647 2023-05-07 20:53:31.491356 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/importing.cpython-39.pyc
+-rw-r--r--   0        0        0     3271 2023-06-09 12:33:26.922855 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/__pycache__/module_processing.cpython-39.pyc
+-rw-r--r--   0        0        0     5780 2023-06-09 12:31:01.816388 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/analyze_package.py
+-rw-r--r--   0        0        0      319 2023-05-07 20:53:19.426804 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/importing.py
+-rw-r--r--   0        0        0     4411 2023-06-09 12:31:01.823667 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/module_processing.py
+-rw-r--r--   0        0        0    12463 2023-05-07 20:43:56.425427 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/uncommitted/__init__.py
+-rw-r--r--   0        0        0     2192 2023-04-15 01:38:51.249072 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/uncommitted/json_schema_inference.py
+-rw-r--r--   0        0        0     3993 2023-04-15 01:38:51.250548 agent_automata-0.1.5/agent_automata/uncommitted/old/utilities/uncommitted/simple_cache.py
+-rw-r--r--   0        0        0     5804 2023-06-19 01:19:58.506224 agent_automata-0.1.5/agent_automata/uncommitted/old/validation.py
+-rw-r--r--   0        0        0      500 2023-06-19 04:31:28.381518 agent_automata-0.1.5/agent_automata/utilities/__init__.py
+-rw-r--r--   0        0        0     1335 2023-06-19 04:51:07.300118 agent_automata-0.1.5/agent_automata/utilities/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4594 2023-06-19 16:18:36.613791 agent_automata-0.1.5/agent_automata/utilities/__pycache__/llm_function.cpython-311.pyc
+-rw-r--r--   0        0        0     1793 2023-06-20 12:37:49.606444 agent_automata-0.1.5/agent_automata/validators.py
+-rw-r--r--   0        0        0      579 2023-06-25 03:46:38.500785 agent_automata-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 agent_automata-0.1.5/PKG-INFO
```

### Comparing `agent_automata-0.1.4/LICENSE` & `agent_automata-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/README.md` & `agent_automata-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/automaton.py` & `agent_automata-0.1.5/agent_automata/automaton.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,37 +49,38 @@
     objectives = input_info["objectives"]
     validate_input = load_validator(
         automaton_path, input_validator_data, input_requirements, objectives
     )
 
     output_info = automaton_data["output"]
     output_format: str = output_info["format"]
-    output_validator_data = output_info["validator"]
-    validate_output = load_validator(
-        automaton_path, output_validator_data, output_format, objectives
-    )
 
     async def run_core_automaton(request: str) -> str:
         """Run a core automaton."""
 
+        sub_automata = automaton_data["sub_automata"]
+        if "think" not in sub_automata:
+            raise ValueError(
+                f"Core automaton runner: `{automaton_id}` must have a `finalize` sub-automaton defined."
+            )
         if validate_input:
             valid, error = await validate_input(request)
             if not valid:
                 return error
 
         reasoning_data = automaton_data["reasoning"]
         knowledge_name = reasoning_data["knowledge"]
         knowledge = load_knowledge(automaton_path, knowledge_name)
         reflector_data = reasoning_data["reflector"]
         reflect = load_reflector(automaton_path, reflector_data)
         planner_data = reasoning_data["planner"]
         plan = load_planner(automaton_path, planner_data)
         sub_automata_data = {
             id: load_automaton_data(automata_location / id)
-            for id in automaton_data["sub_automata"]
+            for id in sub_automata
         }
 
         steps_taken: Sequence[AutomatonStep] = []
         while True:
             reflection = (
                 await reflect(request, steps_taken, knowledge) if reflect else None
             )
```

### Comparing `agent_automata-0.1.4/agent_automata/automaton_loading.py` & `agent_automata-0.1.5/agent_automata/automaton_loading.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/builtin_toolkit/automaton_functions.py` & `agent_automata-0.1.5/agent_automata/builtin_toolkit/automaton_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,18 +71,20 @@
             self_name=automaton_data["name"],
             workspace_name=requester_id,
         )
 
     elif automaton_id == "think":
 
         async def run(request: str) -> str:
+            print(f"Thinking about: {request}")
             return request
 
     elif automaton_id == "finalize":
 
         async def run(request: str) -> str:
+            print(f"Final Result:\n{request}")
             return request
 
     else:
         raise NotImplementedError(f"Unsupported function name: {automaton_id}.")
 
     return run
```

### Comparing `agent_automata-0.1.4/agent_automata/builtin_toolkit/engines.py` & `agent_automata-0.1.5/agent_automata/builtin_toolkit/engines.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/builtin_toolkit/planners/__init__.py` & `agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/builtin_toolkit/planners/react.py` & `agent_automata-0.1.5/agent_automata/builtin_toolkit/planners/react.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,14 +84,19 @@
     reflection: Union[Sequence[str], None],
     automaton_data: Mapping[str, Any],
     sub_automata_data: Mapping[str, Any],
     engine: Engine,
 ) -> Tuple[AutomatonAction, str]:
     """Planner adapted from the ReAct framework."""
 
+    if "think" not in sub_automata_data:
+        raise ValueError(
+            "The ReAct planner requires a sub-automaton named `think` to be defined."
+        )
+
     sub_automata_names = [f'"{data["name"]}"' for data in sub_automata_data.values()]
     sub_automata_descriptions = [
         SUB_AUTOMATON_DESCRIPTION.format(
             sub_automaton_name=sub_automaton["name"],
             description=sub_automaton["description"],
             input_requirements="\n  ".join(
                 f"{letter}. {requirement}"
@@ -140,11 +145,22 @@
     if not steps_taken:
         print(directives)
     print("\n" + step_intro)
     result = (await engine(prompt, stop=["Result:", "---"])).strip()
     print(result)
     delegate_name, delegate_request = parse_result(result)
 
-    delegate_id = next(
-        id for id, data in sub_automata_data.items() if data["name"] == delegate_name
-    )
+    try:
+        delegate_id = next(
+            id
+            for id, data in sub_automata_data.items()
+            if data["name"] == delegate_name
+        )
+    except StopIteration:
+        return (
+            AutomatonAction(
+                "think",
+                f"The Sub-Automaton Name must be one of the following: {sub_automata_names}",
+            ),
+            result,
+        )
     return AutomatonAction(delegate_id, delegate_request), result
```

### Comparing `agent_automata-0.1.4/agent_automata/engines.py` & `agent_automata-0.1.5/agent_automata/engines.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/knowledge.py` & `agent_automata-0.1.5/agent_automata/knowledge.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/planners.py` & `agent_automata-0.1.5/agent_automata/planners.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/reflectors.py` & `agent_automata-0.1.5/agent_automata/reflectors.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/sessions.py` & `agent_automata-0.1.5/agent_automata/sessions.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     automata_location: Path,
     session_id: str,
     automaton_name: str,
     requester_id: str,
     requester_session_id: str,
 ) -> AutomatonRunner:
     """Handle errors and printouts during execution of a query."""
-    preprint = f"\n\n---{automaton_name}: Start---"
-    postprint = f"\n\n---{automaton_name}: End---"
+    preprint = f"\n\n---{automaton_name}: Start---\n\n"
+    postprint = f"\n\n---{automaton_name}: End---\n\n"
 
     @functools.wraps(run)
     async def wrapper(request: str):
         print(preprint)
         try:
             result = await run(request)
         except KeyboardInterrupt:
```

### Comparing `agent_automata-0.1.4/agent_automata/types.py` & `agent_automata-0.1.5/agent_automata/types.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/agent_automata/validators.py` & `agent_automata-0.1.5/agent_automata/validators.py`

 * *Files identical despite different names*

### Comparing `agent_automata-0.1.4/pyproject.toml` & `agent_automata-0.1.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agent_automata"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["solarapparition <15233508+solarapparition@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `agent_automata-0.1.4/PKG-INFO` & `agent_automata-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agent-automata
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: MIT
 Author: solarapparition
 Author-email: 15233508+solarapparition@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

