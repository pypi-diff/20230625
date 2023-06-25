# Comparing `tmp/miko_analyzer-0.3.0.tar.gz` & `tmp/miko_analyzer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miko_analyzer-0.3.0.tar", max compression
+gzip compressed data, was "miko_analyzer-0.3.1.tar", max compression
```

## Comparing `miko_analyzer-0.3.0.tar` & `miko_analyzer-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    11357 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/LICENSE
--rw-r--r--   0        0        0      841 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/__init__.py
--rw-r--r--   0        0        0       97 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/__main__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/cmdline/__init__.py
--rw-r--r--   0        0        0      280 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/cmdline/base.py
--rw-r--r--   0        0        0        0 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/graph/__init__.py
--rw-r--r--   0        0        0     2473 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/graph/plotting.py
--rw-r--r--   0        0        0        0 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/structure/__init__.py
--rw-r--r--   0        0        0     6812 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/structure/cluster.py
--rw-r--r--   0        0        0       62 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/tesla/__init__.py
--rw-r--r--   0        0        0       25 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/tesla/dpgen/__init__.py
--rw-r--r--   0        0        0     3194 2023-03-14 08:49:32.084764 miko_analyzer-0.3.0/miko/tesla/dpgen/base.py
--rw-r--r--   0        0        0    21511 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/tesla/dpgen/exploration.py
--rw-r--r--   0        0        0     3168 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/tesla/dpgen/labeling.py
--rw-r--r--   0        0        0     3676 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/tesla/dpgen/training.py
--rw-r--r--   0        0        0       54 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/utils/__init__.py
--rw-r--r--   0        0        0     1050 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/utils/log_factory.py
--rw-r--r--   0        0        0       45 2023-03-14 08:49:32.088764 miko_analyzer-0.3.0/miko/utils/output.py
--rw-r--r--   0        0        0     1170 2023-03-14 08:56:13.259113 miko_analyzer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 miko_analyzer-0.3.0/setup.py
--rw-r--r--   0        0        0     1988 1970-01-01 00:00:00.000000 miko_analyzer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/LICENSE
+-rw-r--r--   0        0        0      841 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/__main__.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/cmdline/__init__.py
+-rw-r--r--   0        0        0      280 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/cmdline/base.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/graph/__init__.py
+-rw-r--r--   0        0        0     2472 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/graph/plotting.py
+-rw-r--r--   0        0        0        0 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/structure/__init__.py
+-rw-r--r--   0        0        0     6812 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/structure/cluster.py
+-rw-r--r--   0        0        0       62 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/__init__.py
+-rw-r--r--   0        0        0       25 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/__init__.py
+-rw-r--r--   0        0        0     3127 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/base.py
+-rw-r--r--   0        0        0    26841 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/exploration.py
+-rw-r--r--   0        0        0     4261 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/labeling.py
+-rw-r--r--   0        0        0     2930 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/tesla/dpgen/training.py
+-rw-r--r--   0        0        0       54 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/__init__.py
+-rw-r--r--   0        0        0       57 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/files.py
+-rw-r--r--   0        0        0     1050 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/log_factory.py
+-rw-r--r--   0        0        0       45 2023-06-25 10:04:44.323831 miko_analyzer-0.3.1/miko/utils/output.py
+-rw-r--r--   0        0        0     1130 2023-06-25 10:10:57.927889 miko_analyzer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1955 1970-01-01 00:00:00.000000 miko_analyzer-0.3.1/setup.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 miko_analyzer-0.3.1/PKG-INFO
```

### Comparing `miko_analyzer-0.3.0/LICENSE` & `miko_analyzer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.0/README.md` & `miko_analyzer-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.0/miko/graph/plotting.py` & `miko_analyzer-0.3.1/miko/graph/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
         "fontsize": 24
     }
     return theme_dict
 
 
 def canvas_style(
         context='notebook',
-        style='darkgrid',
+        style='ticks',
         palette='deep',
         font='sans-serif',
-        font_scale=1,
+        font_scale=1.5,
         color_codes=True,
         rc=None,
         **kwargs
 ):
     """set basic properties for canvas
 
     :param context: select context of the plot. Please refer to seaborn contexts.
```

### Comparing `miko_analyzer-0.3.0/miko/structure/cluster.py` & `miko_analyzer-0.3.1/miko/structure/cluster.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.0/miko/tesla/dpgen/base.py` & `miko_analyzer-0.3.1/miko/tesla/dpgen/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,23 +77,21 @@
 
 
 class DPAnalyzer(ABC):
     """Base class to be implemented as analyzer for `DPTask`
     """
     def __init__(self, dp_task: DPTask) -> None:
         self.dp_task = dp_task
-        for key in dp_task.__dict__:
-            setattr(self, key, dp_task.__dict__[key])
 
     def _iteration_control_code(self, control_step, iteration=None):
         if iteration is None:
-            if self.step_code < control_step:
-                iteration = self.iteration - 1
+            if self.dp_task.step_code < control_step:
+                iteration = self.dp_task.iteration - 1
             else:
-                iteration = self.iteration
+                iteration = self.dp_task.iteration
         return iteration
 
     def _iteration_dir(self, **kwargs):
         iteration = self._iteration_control_code(**kwargs)
         return 'iter.' + str(iteration).zfill(6)
 
     @classmethod
```

### Comparing `miko_analyzer-0.3.0/miko/tesla/dpgen/exploration.py` & `miko_analyzer-0.3.1/miko/tesla/dpgen/exploration.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import json
 import os
 from re import A
 import shutil
-from collections.abc import Iterable, Sized
+from collections.abc import Iterable, Collection, Sized
 from glob import glob
 from pathlib import Path
 
-from typing import Union, List
+from typing import Optional, Union, List, Tuple, Dict
 from matplotlib.figure import Figure
 
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from ase.io import read, write
 from matplotlib import pyplot as plt
 
-from miko.utils import logger
+from miko.utils.log_factory import logger
+from miko.utils.files import count_lines
 from miko.graph.plotting import canvas_style, AxesInit, square_grid
 from miko.tesla.dpgen.base import DPAnalyzer
 
 
 def read_model_deviation(model_devi_path: Path):
     model_devi_path = model_devi_path.resolve()
     try:
@@ -32,26 +33,26 @@
     return steps, max_devi_f, max_devi_e
 
 
 class DPExplorationAnalyzer(DPAnalyzer):
     """Analyzer for exploration tasks.
     """
 
-    def make_set(self, iteration: int = None) -> dict:
+    def make_set(self, iteration: Optional[int] = None) -> List[dict]:
         """Dump dataset for easy analysis as list of dict
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             List[dict]: all model deviation results
         """
         n_iter = self._iteration_dir(control_step=2, iteration=iteration)
         all_data = []
-        for task in (self.path / n_iter).glob('01.model_devi/task*'):
+        for task in (self.dp_task.path / n_iter).glob('01.model_devi/task*'):
             # read model_devi.out
             steps, max_devi_f, max_devi_e = \
                 read_model_deviation(task / 'model_devi.out')
 
             # load job config
             try:
                 with open(task / 'job.json', 'r') as f:
@@ -68,57 +69,61 @@
                 'task_path': task,
                 'steps': steps
             }
             all_dict = {**result_dict, **job_dict}
             all_data.append(all_dict)
         return all_data
 
-    def get_cur_job(self, iteration: int) -> dict:
+    def get_cur_job(self, iteration: Optional[int]) -> dict:
         """Get `cur_job.json` for the selected iteration
 
         Args:
-            iteration (int): the iteration to get
+            iteration (int, optional): the iteration to get
 
         Returns:
             dict: current job parameters
         """
         n_iter = self._iteration_dir(control_step=2, iteration=iteration)
         try:
-            with open(self.path / n_iter / '01.model_devi' / 'cur_job.json', 'r') as f:
+            with open(
+                self.dp_task.path / n_iter / '01.model_devi' / 'cur_job.json', 'r'
+            ) as f:
                 job_dict = json.load(f)
         except Exception as err:
             logger.warning(err)
             job_dict = {}
         return job_dict
 
-    def make_set_dataframe(self, iteration: int = None) -> pd.DataFrame:
+    def make_set_dataframe(
+            self, iteration: Optional[int] = None) -> pd.DataFrame:
         """Dump dataset for easy analysis as `pandas.Dataframe`
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             pd.DataFrame: Dataframe containing all model deviation logs.
         """
         all_data = self.make_set(iteration=iteration)
         df = pd.DataFrame(all_data)
+        df = df.explode(["max_devi_e", "max_devi_f", "steps"])
         return df
 
-    def make_set_pickle(self, iteration: int = None) -> pd.DataFrame:
+    def make_set_pickle(self, iteration: Optional[int] = None) -> pd.DataFrame:
         """Dump pickle from `self.make_set_dataframe` for quick load.
            Default to `<dpgen_task_path>/model_devi_each_iter/data_<iter>.pkl`
 
         Args:
             iteration (int, optional): iteration to be dumped. Defaults to None, dumping the latest iteration.
 
         Returns:
             pd.DataFrame: DataFrame containing all model deviation logs.
         """
         df = self.make_set_dataframe(iteration=iteration)
-        save_path = self.path / 'model_devi_each_iter'
+        save_path = self.dp_task.path / 'model_devi_each_iter'
         os.makedirs(name=save_path, exist_ok=True)
         if iteration is None:
             iteration = self._iteration_control_code(
                 control_step=2, iteration=iteration)
         df.to_pickle(save_path / f'data_{str(iteration).zfill(6)}.pkl')
         return df
 
@@ -127,38 +132,44 @@
 
         Args:
             iteration (int): the iteration to get
 
         Returns:
             pd.DataFrame: DataFrame containing all model deviation logs.
         """
-        pkl_path = self.path / \
+        pkl_path = self.dp_task.path / \
             f'model_devi_each_iter/data_{str(iteration).zfill(6)}.pkl'
         df = pd.read_pickle(pkl_path)
         return df
 
     @staticmethod
-    def _convert_group_by(group_by: str, **kwargs):
-        plot_items = kwargs.get(group_by)
-        if isinstance(plot_items, str):
-            num_item = 1
-            plot_items = [int(plot_items)]
-        elif isinstance(plot_items, (int, float)):
+    def _convert_group_by(
+        group_by: Optional[str] = None, 
+        **kwargs
+    ) -> Tuple[int, Union[List, Collection]]:
+        if group_by is None:
             num_item = 1
-            plot_items = [plot_items]
-        elif isinstance(plot_items, Sized):
-            num_item = len(plot_items)
+            plot_items = [None]
         else:
-            logger.error('The values chosen for plotting not exists.')
-            raise TypeError(
-                'Please pass values to be plotted with `group_by` value as variable name')
+            plot_items = kwargs.get(group_by)
+            if isinstance(plot_items, str):
+                num_item = 1
+                plot_items = [int(plot_items)]
+            elif isinstance(plot_items, (int, float)):
+                num_item = 1
+                plot_items = [plot_items]
+            elif isinstance(plot_items, Collection):
+                num_item = len(plot_items)
+            else:
+                num_item = 1
+                plot_items = [plot_items]
         return num_item, plot_items
 
     @staticmethod
-    def select_dataset(dataset, select, select_value):
+    def select_dataset(dataset, select, select_value=None):
         try:
             df = dataset[dataset[select] == select_value]
         except KeyError as err:
             logger.error(f'Please choose existing parameter for `select`')
             raise err
         return df
 
@@ -177,55 +188,90 @@
         try:
             parts = dataset[dataset['iteration'] == iteration_dir]
         except KeyError as err:
             logger.error(f'Please choose existing iteration as input.')
             raise err
         return parts
 
-    def _data_prepareation(self, plot_item, iteration=None, group_by="temps", select=None, select_value=None, **kwargs):
+    def _load_model_devi_dataframe(
+            self,
+            plot_item,
+            iteration=None,
+            group_by=None,
+            select=None,
+            select_value=None,
+            **kwargs
+    ) -> pd.DataFrame:
         iteration_code = self._iteration_control_code(
             control_step=2, iteration=iteration)
         try:
             df = self.load_from_pickle(iteration=iteration_code)
         except FileNotFoundError:
             df = self.make_set_pickle(iteration=iteration_code)
 
-        label_unit = kwargs.get('label_unit')
-
+        # select data frame of given select
         if all([select, select_value]):
             df = self.select_dataset(df, select, select_value)
-        partdata = self.extract_group_dataset(df, plot_item, group_by)
+
+        # extract data frame of given group
+        if group_by:
+            partdata = self.extract_group_dataset(df, plot_item, group_by)
+        else:
+            partdata = df
+
+        # export data frame of given iteration
         parts = self.extract_iteration_dataset(
-            partdata, self._iteration_dir(control_step=2, iteration=iteration)
+            partdata, self._iteration_dir(
+                control_step=2, iteration=iteration
+            )
         )
-        steps = np.array(list(parts['steps'])).flatten()
-        mdf = np.array(list(parts['max_devi_f'])).flatten()
+        return parts
+
+    def _data_prepareation(
+            self,
+            plot_item,
+            iteration=None,
+            group_by=None,
+            select=None,
+            select_value=None,
+            **kwargs
+    ):
+        iteration_code = self._iteration_control_code(
+            control_step=2, iteration=iteration)
+        parts = self._load_model_devi_dataframe(
+            plot_item, iteration, group_by, select, select_value, **kwargs
+        )
+
+        steps = parts['steps']
+        mdf = parts['max_devi_f']
+        label_unit = kwargs.get('label_unit')
         logger.info(
             f"f_max = {mdf.max()} ev/Å at {group_by}={plot_item} {label_unit} at iter {iteration_code}.")
         return steps, mdf
 
     def _read_model_devi_trust_level(self, trust_level_key, iteration=None):
         cur_job = self.get_cur_job(iteration)
         trust_level = cur_job.get(trust_level_key)
         if trust_level is None:
-            trust_level = self.param_data[trust_level_key]
+            trust_level = self.dp_task.param_data[trust_level_key]
         # Is average OK for different systems?
         if isinstance(trust_level, Iterable):
-            trust_level = np.mean(trust_level)
+            trust_level = np.mean(trust_level)  # type: ignore
         return trust_level
 
     def plot_single_iteration(
             self,
-            iteration: int = None,
-            x_limit: Union[float, List[float]] = None,
-            y_limit: Union[float, List[float]] = None,
+            iteration: Optional[int] = None,
+            *,
+            x_limit: Optional[Union[float, List[float]]] = None,
+            y_limit: Optional[Union[float, List[float]]] = None,
             use_log: bool = False,
-            group_by: str = 'temps',
-            select: str = None,
-            select_value: str = None,
+            group_by: Optional[str] = None,
+            select: Optional[str] = None,
+            select_value: Optional[str] = None,
             **kwargs
     ) -> Figure:
         """Generate a plot of model deviation in each iteration.
 
         Args:
             iteration (int, optional): The iteration. Defaults to current iteration.
             x_limit (float, List[float], optional): Choose the limit of x axis. Defaults to None.
@@ -253,15 +299,15 @@
         gs = fig.add_gridspec(num_item, 3)
 
         for i, plot_item in enumerate(plot_items):
             steps, mdf = self._data_prepareation(
                 plot_item, iteration, group_by, select, select_value, **kwargs)
 
             # left part
-            fig_left = fig.add_subplot(gs[i, :-1])
+            fig_left = fig.add_subplot(gs[i, :-1]) # type: ignore
             fig_left_args = {
                 'x': steps,
                 'y': mdf,
                 'plot_item': plot_item,
                 'label_unit': kwargs.get('label_unit'),
                 'x_limit': x_limit,
                 'y_limit': y_limit,
@@ -271,40 +317,42 @@
                 'color': 'red',
                 'iteration': iteration,
             }
             PlottingExploartion.plot_mdf_time_curve(fig_left, fig_left_args)
             global_ylim = fig_left.get_ylim()
 
             # right part
-            fig_right = fig.add_subplot(gs[i, -1])
+            fig_right = fig.add_subplot(gs[i, -1]) # type: ignore
             fig_right_args = {
                 'data': mdf,
                 'plot_item': plot_item,
                 'label_unit': kwargs.get('label_unit'),
                 'y_limit': global_ylim,
                 'use_log': use_log,
                 'f_trust_lo': self._read_model_devi_trust_level("model_devi_f_trust_lo", iteration),
                 'f_trust_hi': self._read_model_devi_trust_level("model_devi_f_trust_hi", iteration),
                 'color': 'red',
                 'iteration': iteration,
             }
             PlottingExploartion.plot_mdf_distribution(
                 fig_right, fig_right_args, orientation='horizontal')
+            fig_right.set_xticklabels([])
+            fig_right.set_yticklabels([])
         return fig
 
     def plot_multiple_iterations(
             self,
             iterations: Iterable,
-            group_by: str = 'temps',
+            group_by: Optional[str] = None,
             f_trust_lo: float = 0.10,
             f_trust_hi: float = 0.30,
-            x_limit: Union[float, List[float]] = None,
-            y_limit: Union[float, List[float]] = None,
-            select: str = None,
-            select_value: str = None,
+            x_limit: Optional[Union[float, List[float]]] = None,
+            y_limit: Optional[Union[float, List[float]]] = None,
+            select: Optional[str] = None,
+            select_value: Optional[str] = None,
             **kwargs
     ):
         """Analyse trajectories for different temperatures.
 
         Args:
             iterations (Iterabke): Iterations selected, which should be iterable.
             group_by (str, optional): Choose which the plots are grouped by, which should be included.
@@ -323,118 +371,196 @@
 
         """
         num_item, plot_items = self._convert_group_by(group_by, **kwargs)
         label_unit = kwargs.get('label_unit', 'K')
 
         canvas_style(**kwargs)
         nrows = square_grid(num_item)
-        fig, axs = plt.subplots(nrows, nrows, figsize=[12, 12], constrained_layout=True)
+        fig, axs = plt.subplots(nrows, nrows, figsize=[
+                                12, 12], constrained_layout=True)
         for i, plot_item in enumerate(plot_items):
             try:
                 ax = axs.flatten()[i]
             except AttributeError:
                 ax = axs
             for iteration in iterations:
                 step, mdf = self._data_prepareation(
                     plot_item, iteration, group_by, select, select_value, **kwargs)
-                ax.scatter(step, mdf, s=80, alpha=0.3,
+                ax.scatter(step, mdf, s=80, alpha=0.3, # type: ignore
                            label=f'iter {int(iteration)}', marker='o')
-            ax.axhline(f_trust_lo, linestyle='dashed')
-            ax.axhline(f_trust_hi, linestyle='dashed')
-            ax.set_ylabel(r'$\sigma_{f}^{max}$ (ev/Å)')
-            ax.set_xlabel('Simulation time (fs)')
-            ax.set_title(f'{plot_item} {label_unit}')
-            ax.legend()
+            ax.axhline(f_trust_lo, linestyle='dashed') # type: ignore
+            ax.axhline(f_trust_hi, linestyle='dashed') # type: ignore
+            ax.set_ylabel(r"$\sigma_{f}^{max}$ (ev/Å)") # type: ignore
+            ax.set_xlabel('Simulation time (fs)') # type: ignore
+            ax.legend() # type: ignore
             if x_limit is not None:
-                PlottingExploartion._plot_set_axis_limits(ax, x_limit, 'x_limit')
+                PlottingExploartion._plot_set_axis_limits(
+                    ax, x_limit, 'x_limit') # type: ignore
             if kwargs.get('use_log', False) == True:
-                ax.set_yscale('log')
+                ax.set_yscale('log') # type: ignore
             else:
                 if y_limit is not None:
-                    PlottingExploartion._plot_set_axis_limits(ax, y_limit, 'y_limit')
+                    PlottingExploartion._plot_set_axis_limits(
+                        ax, y_limit, 'y_limit') # type: ignore
         for i in range(num_item, nrows * nrows):
             try:
                 fig.delaxes(axs.flatten()[i])
             except AttributeError:
                 pass
-        try:
-            plot_title = f'Iteration {",".join(iterations)}'
-        except TypeError:
-            plot_title = f'Iteration {iterations}'
-        fig.suptitle(plot_title)
         return fig
 
     def plot_multi_iter_distribution(
             self,
             iterations: Iterable,
-            group_by: str ='temps',
-            select: str = None,
-            select_value: str = None,
-            x_limit: Union[float, List[float]] = None,
-            y_limit: Union[float, List[float]] = None,
+            group_by: Optional[str] = None,
+            select: Optional[str] = None,
+            select_value: Optional[str] = None,
+            f_trust_lo: Optional[float] = None,
+            f_trust_hi: Optional[float] = None,
+            x_limit: Optional[Union[float, List[float]]] = None,
+            y_limit: Optional[Union[float, List[float]]] = None,
             **kwargs
     ) -> Figure:
         """Draw distribution in histogram of model deviation for multiple iterations.
 
         Args:
             iterations (Iterable): _description_
-            group_by (str, optional): _description_. Defaults to 'temps'.
+            group_by (str, optional): _description_. Defaults to None.
             select (str, optional): _description_. Defaults to None.
             select_value (str, optional): _description_. Defaults to None.
+            f_trust_lo (float, optional): The lower limit of max_deviation_force. Defaults to None.
+            f_trust_hi (float, optional): The higher limit of max_deviation_force. Defaults to None.
             x_limit (Union[float, List[float]], optional): _description_. Defaults to None.
             y_limit (Union[float, List[float]], optional): _description_. Defaults to None.
 
         Returns:
             Figure: A figure containing distribution of model deviation for multiple iterations.
         """
         num_item, plot_items = self._convert_group_by(group_by, **kwargs)
         label_unit = kwargs.get('label_unit', 'K')
 
         canvas_style(**kwargs)
-        
+
         nrows = square_grid(num_item)
-        fig, axs = plt.subplots(nrows, nrows, figsize=[12, 12], constrained_layout=True)
+        fig, axs = plt.subplots(nrows, nrows, figsize=[
+                                12, 12], constrained_layout=True)
 
-        colors = plt.cm.viridis(np.linspace(0, 1, len(iterations)))
+        colors = plt.colormaps['viridis_r']( # type: ignore
+            np.linspace(0.15, 0.85, len(iterations)) # type: ignore
+        )
         for i, plot_item in enumerate(plot_items):
             try:
                 ax = axs.flatten()[i]
             except AttributeError:
                 ax = axs
             for j, iteration in enumerate(iterations):
                 step, mdf = self._data_prepareation(
                     plot_item, iteration, group_by, select, select_value, **kwargs)
+                if f_trust_lo is None:
+                    f_trust_lo = self._read_model_devi_trust_level(
+                        "model_devi_f_trust_lo", iteration)
+                if f_trust_hi is None:
+                    f_trust_hi = self._read_model_devi_trust_level(
+                        "model_devi_f_trust_hi", iteration)
                 ax_args = {
                     'data': mdf,
                     'plot_item': plot_item,
                     'label_unit': kwargs.get('label_unit'),
-                    'f_trust_lo': self._read_model_devi_trust_level("model_devi_f_trust_lo", iteration),
-                    'f_trust_hi': self._read_model_devi_trust_level("model_devi_f_trust_hi", iteration),
+                    'f_trust_lo': f_trust_lo,
+                    'f_trust_hi': f_trust_hi,
                     'iteration': iteration,
                     'x_limit': x_limit,
                     'y_limit': y_limit,
                     'color': colors[j],
                     'label': f'Iter {iteration}'
                 }
                 PlottingExploartion.plot_mdf_distribution(
-                    ax, ax_args, orientation='vertical')
-            ax.set_ylabel('Distribution')
-            ax.set_xlabel(r'$\sigma_{f}^{max}$ (ev/Å)')
-            ax.set_title(f'{plot_item} {label_unit}')
-            ax.legend()
+                    ax, ax_args, orientation='vertical') # type: ignore
+            ax.set_ylabel('Distribution') # type: ignore
+            ax.set_xlabel(r'$\sigma_{f}^{max}$ (ev/Å)') # type: ignore
+            ax.legend() # type: ignore
         for i in range(num_item, nrows * nrows):
             try:
                 fig.delaxes(axs.flatten()[i])
             except AttributeError:
                 pass
-        try:
-            plot_title = f'Iteration {",".join(iterations)}'
-        except TypeError:
-            plot_title = f'Iteration {iterations}'
-        fig.suptitle(plot_title)
+        return fig
+
+    def plot_ensemble_ratio_bar(
+            self,
+            iterations: Iterable,
+            group_by: Optional[str] = None,
+            select: Optional[str] = None,
+            select_value: Optional[str] = None,
+            f_trust_lo: Optional[float] = None,
+            f_trust_hi: Optional[float] = None,
+            **kwargs
+    ) -> Figure:
+        """Draw ensemble ratio bar for multiple iterations.
+
+        Args:
+            iterations (Iterable): _description_
+            group_by (Optional[str], optional): _description_. Defaults to None.
+            select (Optional[str], optional): _description_. Defaults to None.
+            select_value (Optional[str], optional): _description_. Defaults to None.
+            f_trust_lo (Optional[float], optional): _description_. Defaults to None.
+            f_trust_hi (Optional[float], optional): _description_. Defaults to None.
+
+        Returns:
+            Figure: _description_
+        """
+
+        num_item, plot_items = self._convert_group_by(group_by, **kwargs)
+        nrows = square_grid(num_item)
+
+        canvas_style(**kwargs)
+
+        fig, axs = plt.subplots(nrows, nrows)
+        for i, plot_item in enumerate(plot_items):
+            if type(axs) is plt.Axes:
+                ax = axs
+            else:
+                ax = axs.flatten()[i] # type: ignore
+
+            ratios = np.zeros((len(iterations), 3)) # type: ignore
+
+            for j, iteration in enumerate(iterations):
+                df = self._load_model_devi_dataframe(
+                    plot_item, iteration, group_by, select, select_value, **kwargs)
+
+                if f_trust_lo is None:
+                    f_trust_lo = self._read_model_devi_trust_level(
+                        "model_devi_f_trust_lo", iteration)
+                if f_trust_hi is None:
+                    f_trust_hi = self._read_model_devi_trust_level(
+                        "model_devi_f_trust_hi", iteration)
+
+                accu_count = (df['max_devi_f'] <= f_trust_lo).sum()
+                failed_count = (df['max_devi_f'] > f_trust_hi).sum()
+                candidate_count = (
+                    (df['max_devi_f'] > f_trust_lo) &
+                    (df['max_devi_f'] <= f_trust_hi)
+                ).sum()
+
+                all_count = accu_count + failed_count + candidate_count
+                count_array = np.array(
+                    [accu_count, candidate_count, failed_count])
+                ratios[j] = count_array / all_count
+
+            ax_args = {
+                'category_names': ['Accurate', 'Candidate', 'Failed'],
+                'ratios': ratios,
+                'iterations': iterations,
+            }
+            PlottingExploartion.plot_ensemble_ratio_bar(ax, ax_args)
+            handles, labels = ax.get_legend_handles_labels()
+        fig.supxlabel('Iteration')
+        fig.supylabel('Ratio')
+        fig.legend(handles, labels, loc='upper center', # type: ignore
+                   ncol=3, bbox_to_anchor=(0.5, 1.0))
         return fig
 
 
 class PlottingExploartion:
     @staticmethod
     def plot_mdf_time_curve(ax: plt.Axes, args):
         plot_item = args.get('plot_item')
@@ -457,78 +583,89 @@
         else:
             PlottingExploartion._plot_set_axis_limits(ax, y_limit, 'y_limit')
 
         if f_trust_lo is not None:
             ax.axhline(f_trust_lo, linestyle='dashed')
         if f_trust_hi is not None:
             ax.axhline(f_trust_hi, linestyle='dashed')
-        if ax.get_subplotspec().is_last_row():
+        if ax.get_subplotspec().is_last_row(): # type: ignore
             ax.set_xlabel('Simulation Steps')
-        if ax.get_subplotspec().is_first_col():
+        if ax.get_subplotspec().is_first_col(): # type: ignore
             ax.set_ylabel(r'$\sigma_{f}^{max}$ (ev/Å)')
         ax.legend()
-        if iteration is None:
-            if ax.get_subplotspec().is_first_row():
-                ax.set_title(f'Iteration {iteration}')
         return ax
 
     @staticmethod
     def plot_mdf_distribution(ax: plt.Axes, args, orientation='vertical'):
         #data = args.get('data')
         x_limit = args.get('x_limit')
         y_limit = args.get('y_limit')
         f_trust_lo = args.get('f_trust_lo')
         f_trust_hi = args.get('f_trust_hi')
         color = args.get('color')
         label = args.get('label')
 
+        # draw the kernel density estimate plot
         if orientation == 'vertical':
-            sns.histplot(
-                data=args, x="data", bins=50, label=label,
-                kde=True, stat='density', color=color, ec=None, alpha=0.5, ax=ax,
+            sns.kdeplot(
+                data=args, x="data", label=label, fill=True,
+                color=color, alpha=0.5, ax=ax,
             )
             ax.axvline(f_trust_lo, linestyle='dashed')
             ax.axvline(f_trust_hi, linestyle='dashed')
         elif orientation == 'horizontal':
-            sns.histplot(
-                data=args, y="data", bins=50, label=label,
-                kde=True, stat='density', color=color, ec=None, alpha=0.5, ax=ax
+            sns.kdeplot(
+                data=args, y="data", label=label, fill=True,
+                color=color, alpha=0.5, ax=ax
             )
             ax.axhline(f_trust_lo, linestyle='dashed')
             ax.axhline(f_trust_hi, linestyle='dashed')
         else:
             raise ValueError('Invalid orientation')
 
-        if ax.get_subplotspec().is_first_row():
-            ax.set_title('Distribution of Deviation')
-
         PlottingExploartion._plot_set_axis_limits(ax, x_limit, 'x_limit')
         if args.get('use_log', False) == True:
             ax.set_yscale('log')
         else:
             PlottingExploartion._plot_set_axis_limits(ax, y_limit, 'y_limit')
+        return ax
 
-        ax.set_xticklabels([])
-        ax.set_yticklabels([])
+    @staticmethod
+    def plot_ensemble_ratio_bar(ax: plt.Axes, args):
+        data = args.get('ratios')
+        labels = args.get('iterations')
+        category_names = args.get('category_names')
+
+        category_colors = plt.colormaps['YlGnBu_r']( # type: ignore
+            np.linspace(0.15, 0.85, data.shape[1])
+        )
+        data_cum = data.cumsum(axis=1)
+        for i, (colname, color) in enumerate(zip(category_names, category_colors)):
+            widths = data[:, i]
+            starts = data_cum[:, i] - widths
+            ax.bar(labels, widths, width=0.5, bottom=starts,
+                   label=colname, color=color)
+        ax.plot(labels, data[:, 0], "o-", c=category_colors[0], mec="white")
+        ax.set_ylim(0.0, 1.0)
         return ax
 
     @staticmethod
     def _plot_set_axis_limits(ax: plt.Axes, limitation, limitation_type):
         limitation_dict = {
             'x_limit': ax.set_xlim,
             'y_limit': ax.set_ylim,
         }
         _func = limitation_dict[limitation_type]
         if limitation is not None:
             if isinstance(limitation, (int, float)):
                 _func(0, limitation)
-            elif isinstance(limitation, Iterable):
+            elif isinstance(limitation, Sized):
                 if len(limitation) > 2:
                     raise ValueError("Limitation should be a value \
                         or a set with no more than 2 elements.")
                 elif len(limitation) == 1:
-                    _func(0, limitation[0])
+                    _func(0, limitation[0]) # type: ignore
                 else:
                     _func(limitation)
             else:
                 raise ValueError("Limitation should be a value \
                     or a set with no more than 2 elements.")
```

### Comparing `miko_analyzer-0.3.0/miko/utils/log_factory.py` & `miko_analyzer-0.3.1/miko/utils/log_factory.py`

 * *Files identical despite different names*

### Comparing `miko_analyzer-0.3.0/pyproject.toml` & `miko_analyzer-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "miko-analyzer"
-version = "0.3.0"
+version = "0.3.1"
 description = "Analyzing tool for deep learning based chemical research."
 authors = ["Cloudac7 <scottryuu@outlook.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cloudac7/miko-analysis"
 packages = [{include = "miko"}]
 
@@ -12,16 +12,14 @@
 enable = true
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 ase = "^3.21.1"
 matplotlib = "^3.7.1"
 numpy = "<1.24,>=1.18"
-llvmlite  = "^0.39.0"
-numba = "^0.56.0"
 pandas = "^1.3.3"
 dpdata = "*"
 dscribe = "*"
 dynaconf = "*"
 mdanalysis = "^2.2"
 scipy = "^1.10.1"
 seaborn = "*"
```

### Comparing `miko_analyzer-0.3.0/setup.py` & `miko_analyzer-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,30 +14,28 @@
 {'': ['*']}
 
 install_requires = \
 ['ase>=3.21.1,<4.0.0',
  'dpdata',
  'dscribe',
  'dynaconf',
- 'llvmlite>=0.39.0,<0.40.0',
  'matplotlib>=3.7.1,<4.0.0',
  'mdanalysis>=2.2,<3.0',
- 'numba>=0.56.0,<0.57.0',
  'numpy>=1.18,<1.24',
  'pandas>=1.3.3,<2.0.0',
  'scipy>=1.10.1,<2.0.0',
  'seaborn',
  'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['miko = miko.cmdline.base:cli']}
 
 setup_kwargs = {
     'name': 'miko-analyzer',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Analyzing tool for deep learning based chemical research.',
     'long_description': '# Miko-Analyzer\n\n[![Python package](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml/badge.svg)](https://github.com/Cloudac7/miko-analyzer/actions/workflows/ci.yml)\n[![Coverage Status](https://coveralls.io/repos/github/Cloudac7/miko-analyzer/badge.svg?branch=master)](https://coveralls.io/github/Cloudac7/miko-analyzer?branch=master)\n\n> コードで占う巫女。\n> Miko using code to perform divinition.\n\nAn analysis plugin for [Deep Potential](https://github.com/deepmodeling/deepmd-kit) based chemical research.\n\nSupporting simple calculation workflow with the help of [DPDispatcher](https://github.com/deepmodeling/dpdispatcher).\n\n## Installation\n\nTo install, clone the repository:\n\n```\ngit clone https://github.com/cloudac7/miko-analyzer.git\n```\n\nand then install with `pip`:\n\n```\ncd miko-analyzer\npip install .\n```\n\n',
     'author': 'Cloudac7',
     'author_email': 'scottryuu@outlook.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/cloudac7/miko-analysis',
```

### Comparing `miko_analyzer-0.3.0/PKG-INFO` & `miko_analyzer-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miko-analyzer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Analyzing tool for deep learning based chemical research.
 Home-page: https://github.com/cloudac7/miko-analysis
 License: Apache-2.0
 Author: Cloudac7
 Author-email: scottryuu@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,18 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ase (>=3.21.1,<4.0.0)
 Requires-Dist: dpdata
 Requires-Dist: dscribe
 Requires-Dist: dynaconf
-Requires-Dist: llvmlite (>=0.39.0,<0.40.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mdanalysis (>=2.2,<3.0)
-Requires-Dist: numba (>=0.56.0,<0.57.0)
 Requires-Dist: numpy (>=1.18,<1.24)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://github.com/cloudac7/miko-analysis
 Description-Content-Type: text/markdown
```

