# Comparing `tmp/action-graph-1.3.0.tar.gz` & `tmp/action-graph-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "action-graph-1.3.0.tar", last modified: Fri Jun 23 21:32:13 2023, max compression
+gzip compressed data, was "action-graph-1.3.1.tar", last modified: Sun Jun 25 00:50:09 2023, max compression
```

## Comparing `action-graph-1.3.0.tar` & `action-graph-1.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.0/LICENSE
--rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.0/README.md
--rw-r--r--   0        0        0      684 2023-06-23 21:25:46.349305 action-graph-1.3.0/action_graph/__init__.py
--rw-r--r--   0        0        0     3181 2023-06-05 00:52:07.725399 action-graph-1.3.0/action_graph/action.py
--rw-r--r--   0        0        0    10818 2023-06-23 21:27:59.160761 action-graph-1.3.0/action_graph/agent.py
--rw-r--r--   0        0        0     4708 2023-06-23 20:12:13.999379 action-graph-1.3.0/action_graph/planner.py
--rw-r--r--   0        0        0      832 2023-06-23 21:26:03.705234 action-graph-1.3.0/pyproject.toml
--rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.0/tests/01-redundant_precon_test.py
--rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.0/tests/02-multi_feasible_test.py
--rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.0/tests/03-references_test.py
--rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.0/tests/04-loop_test.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-03-10 21:00:20.184864 action-graph-1.3.1/LICENSE
+-rw-r--r--   0        0        0     1450 2023-03-10 21:03:34.335982 action-graph-1.3.1/README.md
+-rw-r--r--   0        0        0      684 2023-06-25 00:49:06.146086 action-graph-1.3.1/action_graph/__init__.py
+-rw-r--r--   0        0        0     3181 2023-06-24 22:19:40.196028 action-graph-1.3.1/action_graph/action.py
+-rw-r--r--   0        0        0    10818 2023-06-23 21:27:59.160761 action-graph-1.3.1/action_graph/agent.py
+-rw-r--r--   0        0        0     4664 2023-06-25 00:33:36.780557 action-graph-1.3.1/action_graph/planner.py
+-rw-r--r--   0        0        0      832 2023-06-25 00:49:10.266264 action-graph-1.3.1/pyproject.toml
+-rwxr-xr-x   0        0        0     1103 2023-06-16 14:34:49.765956 action-graph-1.3.1/tests/01-redundant_precon_test.py
+-rwxr-xr-x   0        0        0     1039 2023-06-23 21:15:35.619807 action-graph-1.3.1/tests/02-multi_feasible_test.py
+-rwxr-xr-x   0        0        0     1284 2023-06-16 14:37:32.454361 action-graph-1.3.1/tests/03-references_test.py
+-rwxr-xr-x   0        0        0      909 2023-06-23 20:50:11.922048 action-graph-1.3.1/tests/04-loop_test.py
+-rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 action-graph-1.3.1/PKG-INFO
```

### Comparing `action-graph-1.3.0/LICENSE` & `action-graph-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/README.md` & `action-graph-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/action_graph/__init__.py` & `action-graph-1.3.1/action_graph/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python3
 
 from action_graph.action import Action, ActionStatus, State
 from action_graph.agent import Agent
 
 name = 'action_graph'
-__version__ = '1.3.0'
+__version__ = '1.3.1'
 __all__ = [
     'State',
     'Action',
     'ActionStatus',
     'ActionFailedException',
     'ActionAbortedException',
     'ActionTimedOutException',
```

### Comparing `action-graph-1.3.0/action_graph/action.py` & `action-graph-1.3.1/action_graph/action.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/action_graph/agent.py` & `action-graph-1.3.1/action_graph/agent.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/action_graph/planner.py` & `action-graph-1.3.1/action_graph/planner.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
         :return:List[Action]: List of actions updated with their expected outcomes (effects)
         """
 
         if len(target_state.items()) > 1:
             raise PlanningFailedException(f'target_state [{target_state}] should be a single state')
         tk, tv = list(target_state.items())[0]
         # in case target state value is a reference to another state variable
-        if isinstance(tv, str) and tv[0] == '@':
-            tv = self.__parse_references(tv, start_state)
+        tv = self.__parse_references(tv, start_state, '@')
         # check if the target state is already satisfied
         if (tk, tv) in list(start_state.items()):
             return []   # goal already met, move on
         #
         # find action(s) that satisfy the state current effect-item
         probable_actions: List[Action] = self._action_lookup[(tk, tv)]
         if not probable_actions:  # if no actions are found, try with templated actions
@@ -60,17 +59,16 @@
             action = p_action.__copy__()
             if action.effects[tk] is Ellipsis:
                 action.effects[tk] = tv  # apply variable effects
             #
             action_path: List[Action] = []
             for pk, pv in action.preconditions.items():  # for each pre-condition ...
                 try:  # choose the shortest feasible path
-                    if isinstance(pv, str) and pv[0] == '$':
-                        pv = self.__parse_references(pv, action.effects)
-                    action_path += self.generate_plan({pk: pv}, start_state, avoid_actions)  # merge the actions
+                    pv = self.__parse_references(pv, action.effects, '$')
+                    action_path.extend(self.generate_plan({pk: pv}, start_state, avoid_actions))  # merge the actions
                 except RecursionError:  # watch out for cyclic references
                     raise PlanningFailedException(f'Found cyclic references! {pk}:{pv}')
             # include the current action;  remove duplicates; keep the order intact
             action_path = self.__make_unique(action_path + [action])
             #
             if not chosen_path:  # if no other path is available...
                 chosen_path = action_path  # use the current path
@@ -88,15 +86,15 @@
     def __create_action_lookup(self, actions: List[Action]) -> Dict[Tuple[Any, Any], List[Action]]:
         action_lookup: Dict[Tuple[Any, Any], List[Action]] = defaultdict(list)
         for action in actions:
             for k, v in action.effects.items():
                 action_lookup[(k, v)].append(action)
         return action_lookup
 
-    def __parse_references(self, ref: Any, state: State) -> Any:
-        while ref[1:] in state:
+    def __parse_references(self, ref: Any, state: State, prefix: str) -> Any:
+        while isinstance(ref, str) and ref[0] == prefix and ref[1:] in state:
             ref = state[ref[1:]]
         return ref
 
     def __make_unique(self, path):
         unique = set()
         return [x for x in path if x not in unique and not unique.add(x)]
```

### Comparing `action-graph-1.3.0/pyproject.toml` & `action-graph-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
     { name = "Bharath Achyutha Rao", email = "bharath.rao@hotmail.com" },
 ]
 name = "action_graph"
-version = "1.3.0"
+version = "1.3.1"
 description = "Autonomous agent for task/action planning and execution"
 readme = "README.md"
 requires-python = ">=3.7,<4.0"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `action-graph-1.3.0/tests/01-redundant_precon_test.py` & `action-graph-1.3.1/tests/01-redundant_precon_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/tests/02-multi_feasible_test.py` & `action-graph-1.3.1/tests/02-multi_feasible_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/tests/03-references_test.py` & `action-graph-1.3.1/tests/03-references_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/tests/04-loop_test.py` & `action-graph-1.3.1/tests/04-loop_test.py`

 * *Files identical despite different names*

### Comparing `action-graph-1.3.0/PKG-INFO` & `action-graph-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action_graph
-Version: 1.3.0
+Version: 1.3.1
 Summary: Autonomous agent for task/action planning and execution
 Author-email: Bharath Achyutha Rao <bharath.rao@hotmail.com>
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Bug Tracker, https://github.com/bharathra/action_graph/issues
```

