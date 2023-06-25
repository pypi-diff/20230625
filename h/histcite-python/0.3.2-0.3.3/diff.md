# Comparing `tmp/histcite-python-0.3.2.tar.gz` & `tmp/histcite-python-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.3.2.tar", last modified: Fri May 19 16:49:22 2023, max compression
+gzip compressed data, was "histcite-python-0.3.3.tar", last modified: Sun Jun 25 01:55:19 2023, max compression
```

## Comparing `histcite-python-0.3.2.tar` & `histcite-python-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 16:49:10.000000 histcite-python-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-19 16:49:22.769626 histcite-python-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7729 2023-05-19 16:49:10.000000 histcite-python-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/parse_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-19 16:49:10.000000 histcite-python-0.3.2/histcite/recognize_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-19 16:49:22.000000 histcite-python-0.3.2/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 16:49:22.769626 histcite-python-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-19 16:49:10.000000 histcite-python-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 16:49:22.769626 histcite-python-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-19 16:49:10.000000 histcite-python-0.3.2/tests/test_parse_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-25 01:55:10.000000 histcite-python-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-25 01:55:19.889989 histcite-python-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8284 2023-06-25 01:55:10.000000 histcite-python-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/parse_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-25 01:55:10.000000 histcite-python-0.3.3/histcite/recognize_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-25 01:55:19.000000 histcite-python-0.3.3/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-25 01:55:10.000000 histcite-python-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 01:55:19.889989 histcite-python-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 01:55:19.889989 histcite-python-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-25 01:55:10.000000 histcite-python-0.3.3/tests/test_parse_reference.py
```

### Comparing `histcite-python-0.3.2/LICENSE` & `histcite-python-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/PKG-INFO` & `histcite-python-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.3.2
-Summary: A Python interface to histcite.
-Home-page: https://github.com/doublessay/histcite-python
-Author: WangK2
-Author-email: kw221225@gmail.com
+Version: 0.3.3
+Summary: A Python interface for histcite
+Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
-Keywords: histcite,web of science,citation network
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
+Project-URL: Homepage, https://github.com/doublessay/histcite-python
+Keywords: histcite,citation network,web of science,scopus,cssci
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
-- 发现不在本地文献集中、但被本地文献集引用较多的文献；
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
-- `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
-- `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
-- `Recs`， 记录数；
+- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
+- `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
+- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
+- `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
 | :-: | :-: | :-: |
 | 是否开源 | 是 | 否 |
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
+
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 或者是
+$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
 ```
 >注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
@@ -132,18 +133,23 @@
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 >注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## Q&A
 1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2、每次必须指定一种数据库来源吗？  
+答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+
+3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
-- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.3.2/README.md` & `histcite-python-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
-- 发现不在本地文献集中、但被本地文献集引用较多的文献；
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
-- `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
-- `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
-- `Recs`， 记录数；
+- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
+- `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
+- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
+- `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
 | :-: | :-: | :-: |
 | 是否开源 | 是 | 否 |
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
+
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 或者是
+$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
 ```
 >注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
@@ -109,18 +112,23 @@
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 >注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## Q&A
 1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2、每次必须指定一种数据库来源吗？  
+答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+
+3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
-- [x] 支持 `Scopus` 题录数据
-- [ ] 支持 `PubMed` 题录数据
+- [x] 支持 `Scopus` 题录数据
```

### Comparing `histcite-python-0.3.2/histcite/cli.py` & `histcite-python-0.3.3/histcite/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import argparse
 from histcite.compute_metrics import ComputeMetrics
 from histcite.process_file import ProcessFile
 from histcite.network_graph import GraphViz
     
 def main():
-    parser = argparse.ArgumentParser(description='A Python interface to histcite.')
+    parser = argparse.ArgumentParser(description='A Python interface for histcite.')
     parser.add_argument('-f','--folder_path', type=str, required=True, help='folder path of the downloaded files')
     parser.add_argument('-t','--source_type', type=str, required=True, choices=['wos','cssci','scopus'], help='source type of the downloaded files')
     parser.add_argument('-n','--node_num', type=int, default=50, help='node number in the citation network graph')
     parser.add_argument('-g','--graph', action="store_true", help='generate graph file only')
     args = parser.parse_args()
 
     # 将结果存放在用户指定的folder_path下的result文件夹中
```

### Comparing `histcite-python-0.3.2/histcite/compute_metrics.py` & `histcite-python-0.3.3/histcite/compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/histcite/network_graph.py` & `histcite-python-0.3.3/histcite/network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/histcite/parse_reference.py` & `histcite-python-0.3.3/histcite/parse_reference.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/histcite/process_file.py` & `histcite-python-0.3.3/histcite/process_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             raise ValueError(f'File {file_name} is not a valid csv file')
         
 class ProcessFile:
 
     def __init__(self,folder_path:str,source_type:str):
         """
         folder_path: 文件夹路径\n
-        source_type: 数据来源 wos|cssci|scopus|pubmed
+        source_type: 数据来源 wos|cssci|scopus
         """
         self.folder_path = folder_path
         self.source_type = source_type
         if source_type=='wos':
             self.file_name_list = [i.split('.')[0] for i in os.listdir(folder_path) if i[:9]=='savedrecs']
         elif source_type=='cssci':
             self.file_name_list = [i for i in os.listdir(folder_path) if i[:3]=='LY_']
```

### Comparing `histcite-python-0.3.2/histcite/recognize_reference.py` & `histcite-python-0.3.3/histcite/recognize_reference.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.3.3/histcite_python.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.3.2
-Summary: A Python interface to histcite.
-Home-page: https://github.com/doublessay/histcite-python
-Author: WangK2
-Author-email: kw221225@gmail.com
+Version: 0.3.3
+Summary: A Python interface for histcite
+Author-email: WangK2 <kw221225@gmail.com>
 License: MIT
-Keywords: histcite,web of science,citation network
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Education
+Project-URL: Homepage, https://github.com/doublessay/histcite-python
+Keywords: histcite,citation network,web of science,scopus,cssci
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # HistCite工具的Python实现
 
-由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为国科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
+由于原引文分析工具 [HistCite](https://support.clarivate.com/ScientificandAcademicResearch/s/article/HistCite-No-longer-in-active-development-or-officially-supported) 已停止维护，目前国内普遍使用的为中科大某位同学在原程序基础上进行修复的版本 [HistCite Pro](https://zhuanlan.zhihu.com/p/20902898)，仅能在 `Windows` 平台上运行，存在诸多限制。借助 [pandas 2.0](https://pandas.pydata.org/docs/dev/whatsnew/v2.0.0.html) 和可视化工具 [Graphviz](https://graphviz.org)，本工具复刻了原 `HistCite` 的大部分功能，同时拓展了对其他数据源的支持，可以跨平台使用。
 
 最近更新：
 - `v0.3.0` 增加了对 `Scopus` 数据库题录数据的支持；
 - `v0.2.0` 增加了对 `CSSCI` 数据库题录数据的支持；
 
 核心功能：
 - 生成引文网络图；
-- 生成统计数据，其中包括文献、作者、机构、文献来源、作者关键词等；  
-- 发现不在本地文献集中、但被本地文献集引用较多的文献；
+- 生成统计数据，包括文献、作者、机构、文献来源、作者关键词等分析对象；  
+- 发现不在本地文献集中、但被本地文献集引用较多的文献，即本次文献获取过程忽略的重要文献；
 
 术语说明：
-- `GCS`, Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
-- `LCS`, Local Citation Score，表示一篇文献在本地论文集中的被引次数；
-- `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
-- `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
-- `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
-- `Recs`， 记录数；
+- `GCS`，Global Citation Score， 表示一篇文献在 Web of Science核心合集中的总被引次数；
+- `LCS`，Local Citation Score，表示一篇文献在本地论文集中的被引次数；
+- `GCR`，Global Cited References，表示一篇文献所有参考文献的数量；
+- `LCR`， Local Cited References，表示一篇文献所有本地参考文献的数量；
+- `T*`，Total，表示给定作者、机构、期刊等相应分数之和。例如 `TLCS` = 总本地引文数；
+- `Recs`，记录数；
 - `Web of Science` 题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 - 其他来源的题录数据会沿用 `Web of Science` 的字段命名格式；
 
 工具对比：
 | 对比项 | histcite-python | histcite pro |
 | :-: | :-: | :-: |
 | 是否开源 | 是 | 否 |
 | 是否跨平台 | 是 | 否，仅限 Windows |
 | 是否支持其他数据源 | 是 | 否，仅限 Web of Science |
 | 是否提供前端界面 | 否 | 是 |
-| 引文网络图 | 矢量图，比较清晰 | 位图，比较粗糙 |
+| 引文网络图 | 矢量图，比较清晰 | 位图，比较模糊 |
 
 ## 快速开始
 ```console
 # 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 数据准备
 | 数据来源 | 下载说明 |
 | :---: | --- |
 | `Web of Science` | `核心合集`，格式选择 `Tab delimited file/制表符分隔文件`，导出内容选择 `Full Record and Cited References/全记录与引用的参考文献` 或者是 `Custome selection/自定义选择项`，全选字段。 |
 | `CSSCI` | 从 `CSSCI数据库` 正常导出即可。 |
 | `Scopus` | 格式选择 `CSV` 文件，导出字段需要额外勾选 `Author keywords` 和 `Include references`，或者直接全选字段。 |
+
 >⚠️ 文件下载之后不要改名(会根据文件名识别有效的题录数据文件)，下载完成后放在一个单独的文件夹内。
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
 |  | 参数 | 说明 |
 | :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -t | --source_type | 题录数据来源，可选 `wos`、`cssci`、`scopus`，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`，无需传值 |
 
 ```console
 $ 假设文件夹路径为/Users/.../downloads/dataset，来源为web of science, 引文网络图节点数设置为100
 $ histcite -f /Users/.../downloads/dataset -t wos -n 100
+$ 或者是
+$ histcite --folder_path /Users/.../downloads/dataset --source_type wos --node_num 100
 ```
 >注：结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 statistics.xlsx, graph.node.xlsx, graph.dot 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
@@ -132,18 +133,23 @@
 graph_node_file.to_excel(os.path.join(folder_path,'result','graph.node.xlsx'),index=False)
 ```
 >注：`generate_dot_file` 函数的 `allow_external_node` 参数表示引文网络节点中是否允许出现 `doc_indices` 之外的节点文献，`doc_indices` 一般为 `LCS` 比较高的文献，这些文献同样会参考低 `LCS` 的文献，或被低 `LCS` 的文献引用，因此如果将 `allow_external_node` 设置为 `True`，引文网络图中将会出现这些低 `LCS` 的文献节点，默认为 `False`。
 
 ## 实现细节
 |  | Web of Science | CSSCI | Scopus|
 | --- | --- | --- | --- |
-| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作 `和 `题名` 进行判断 | 通过 `一作 `和 `题名` 进行判断 |
+| 如何识别引文关系 | 如果存在 `DOI`，则优先使用 `DOI` 进行匹配；否则通过 `一作`、`发表年份`、`文献来源`、`开始页` 进行判断  | 通过 `一作` 和 `题名` 进行判断 | 通过 `一作` 和 `题名` 进行判断 |
 | 如何去重 | 根据 `UT` 入藏号进行去重 | 根据 `一作` 和 `题名` 字段进行去重 | 根据 `EID` 字段进行去重 |
 
 ## Q&A
 1、为什么选取 `LSC` 最高的100篇文献，但是引文网络图及图节点文件中的节点数量少于100？  
-答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。
+答：考虑到实用性和美观性，程序会自动忽略没有边的节点。即这些选中的文献没有引用其他选中的文献，或被这些文献引用。  
+
+2、每次必须指定一种数据库来源吗？  
+答：是的。不同来源数据库的参考文献字段包含的内容不同，解析方式不同，引文识别方式也不同，需要单独处理。
+
+3、为什么不支持 `CNKI`、`PubMed` 等数据库的题录数据？  
+答：无法导出参考文献或引文字段信息，也就无法识别引文关系。如果需要支持其他数据库，欢迎提交issue。
 
 ## TODO
 - [x] 支持 `CSSCI` 题录数据
 - [x] 支持 `Scopus` 题录数据
-- [ ] 支持 `PubMed` 题录数据
```

### Comparing `histcite-python-0.3.2/histcite_python.egg-info/SOURCES.txt` & `histcite-python-0.3.3/histcite_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 README.md
-setup.py
+pyproject.toml
 histcite/__init__.py
 histcite/cli.py
 histcite/compute_metrics.py
 histcite/network_graph.py
 histcite/parse_reference.py
 histcite/process_file.py
 histcite/recognize_reference.py
```

### Comparing `histcite-python-0.3.2/tests/test_compute_metrics.py` & `histcite-python-0.3.3/tests/test_compute_metrics.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/tests/test_network_graph.py` & `histcite-python-0.3.3/tests/test_network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.3.2/tests/test_parse_reference.py` & `histcite-python-0.3.3/tests/test_parse_reference.py`

 * *Files identical despite different names*

