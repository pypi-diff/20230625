# Comparing `tmp/gridworks-0.2.6.tar.gz` & `tmp/gridworks-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks-0.2.6.tar", max compression
+gzip compressed data, was "gridworks-0.2.7.tar", max compression
```

## Comparing `gridworks-0.2.6.tar` & `gridworks-0.2.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1065 2023-06-07 14:24:50.545067 gridworks-0.2.6/LICENSE
--rw-r--r--   0        0        0     5778 2023-06-07 14:24:50.545067 gridworks-0.2.6/README.md
--rw-r--r--   0        0        0     2552 2023-06-07 14:25:03.549213 gridworks-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      249 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/__init__.py
--rw-r--r--   0        0        0      208 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/__main__.py
--rw-r--r--   0        0        0    47777 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/actor_base.py
--rw-r--r--   0        0        0    18028 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/algo_utils.py
--rw-r--r--   0        0        0    12872 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/api_utils.py
--rw-r--r--   0        0        0     2016 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/base_api_types.py
--rw-r--r--   0        0        0      251 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/conversion_factors.py
--rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/__init__.py
--rw-r--r--   0        0        0    23522 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/base_g_node.py
--rw-r--r--   0        0        0     6726 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node.py
--rw-r--r--   0        0        0     6405 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node_instance.py
--rw-r--r--   0        0        0     5011 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/g_node_strategy.py
--rw-r--r--   0        0        0      694 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/gps_point.py
--rw-r--r--   0        0        0     2498 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/market_type.py
--rw-r--r--   0        0        0     1214 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/data_classes/supervisor_container.py
--rw-r--r--   0        0        0      131 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/dev_utils/__init__.py
--rw-r--r--   0        0        0     3391 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/dev_utils/algo_setup.py
--rw-r--r--   0        0        0     1238 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/algo_cert_type.py
--rw-r--r--   0        0        0      990 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/core_g_node_role.py
--rw-r--r--   0        0        0     2547 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/message_category_symbol.py
--rw-r--r--   0        0        0      626 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0     2734 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/supervisor_container_status.py
--rw-r--r--   0        0        0      795 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/enums/universe_type.py
--rw-r--r--   0        0        0      336 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/errors.py
--rw-r--r--   0        0        0     4187 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/gw_config.py
--rw-r--r--   0        0        0     2813 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/message.py
--rw-r--r--   0        0        0    17029 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/property_format.py
--rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/py.typed
--rw-r--r--   0        0        0     9199 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/rest_api.py
--rw-r--r--   0        0        0     1476 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/__init__.py
--rw-r--r--   0        0        0    20321 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/base_g_node_gt.py
--rw-r--r--   0        0        0    24525 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/g_node_gt.py
--rw-r--r--   0        0        0    15787 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     6719 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/gw_cert_id.py
--rw-r--r--   0        0        0     3502 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/heartbeat_a.py
--rw-r--r--   0        0        0        0 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/old_versions/__init__.py
--rw-r--r--   0        0        0     1838 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/old_versions/heartbeat_a_001.py
--rw-r--r--   0        0        0     5581 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/ready.py
--rw-r--r--   0        0        0     8098 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/sim_timestep.py
--rw-r--r--   0        0        0     6096 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/super_starter.py
--rw-r--r--   0        0        0    12069 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     5788 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks/utils.py
--rw-r--r--   0        0        0      543 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/__init__.py
--rw-r--r--   0        0        0     2634 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/stub_actors.py
--rw-r--r--   0        0        0     2936 2023-06-07 14:24:50.613068 gridworks-0.2.6/src/gridworks_test/wait.py
--rw-r--r--   0        0        0     7269 1970-01-01 00:00:00.000000 gridworks-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-25 19:40:25.796958 gridworks-0.2.7/LICENSE
+-rw-r--r--   0        0        0     5587 2023-06-25 19:40:42.877121 gridworks-0.2.7/README.md
+-rw-r--r--   0        0        0     2579 2023-06-25 19:40:42.877121 gridworks-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      249 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/__main__.py
+-rw-r--r--   0        0        0    51618 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks/actor_base.py
+-rw-r--r--   0        0        0    18028 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/algo_utils.py
+-rw-r--r--   0        0        0    12872 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/api_utils.py
+-rw-r--r--   0        0        0     2016 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/base_api_types.py
+-rw-r--r--   0        0        0      251 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/conversion_factors.py
+-rw-r--r--   0        0        0        0 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/__init__.py
+-rw-r--r--   0        0        0    23522 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/base_g_node.py
+-rw-r--r--   0        0        0     6726 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node.py
+-rw-r--r--   0        0        0     6405 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node_instance.py
+-rw-r--r--   0        0        0     5011 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/g_node_strategy.py
+-rw-r--r--   0        0        0      694 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/gps_point.py
+-rw-r--r--   0        0        0     2498 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/market_type.py
+-rw-r--r--   0        0        0     1214 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/data_classes/supervisor_container.py
+-rw-r--r--   0        0        0      131 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/dev_utils/__init__.py
+-rw-r--r--   0        0        0     3391 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/dev_utils/algo_setup.py
+-rw-r--r--   0        0        0     1238 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/algo_cert_type.py
+-rw-r--r--   0        0        0      990 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/core_g_node_role.py
+-rw-r--r--   0        0        0     2547 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/g_node_role.py
+-rw-r--r--   0        0        0      992 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/g_node_status.py
+-rw-r--r--   0        0        0      933 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/gni_status.py
+-rw-r--r--   0        0        0      563 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_price_unit.py
+-rw-r--r--   0        0        0      590 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_quantity_unit.py
+-rw-r--r--   0        0        0     1394 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/market_type_name.py
+-rw-r--r--   0        0        0     1326 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/message_category.py
+-rw-r--r--   0        0        0     1189 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/message_category_symbol.py
+-rw-r--r--   0        0        0      626 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/recognized_currency_unit.py
+-rw-r--r--   0        0        0     2734 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/strategy_name.py
+-rw-r--r--   0        0        0     1081 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/supervisor_container_status.py
+-rw-r--r--   0        0        0      795 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/enums/universe_type.py
+-rw-r--r--   0        0        0      336 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/errors.py
+-rw-r--r--   0        0        0     8749 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks/gw_config.py
+-rw-r--r--   0        0        0     2813 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/message.py
+-rw-r--r--   0        0        0    17029 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/property_format.py
+-rw-r--r--   0        0        0        0 2023-06-25 19:40:25.884959 gridworks-0.2.7/src/gridworks/py.typed
+-rw-r--r--   0        0        0     9199 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/rest_api.py
+-rw-r--r--   0        0        0     1476 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/__init__.py
+-rw-r--r--   0        0        0    20321 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/base_g_node_gt.py
+-rw-r--r--   0        0        0    24525 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/g_node_gt.py
+-rw-r--r--   0        0        0    15787 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/g_node_instance_gt.py
+-rw-r--r--   0        0        0     6719 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/gw_cert_id.py
+-rw-r--r--   0        0        0     3502 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/heartbeat_a.py
+-rw-r--r--   0        0        0        0 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/old_versions/__init__.py
+-rw-r--r--   0        0        0     1838 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/old_versions/heartbeat_a_001.py
+-rw-r--r--   0        0        0     5581 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/ready.py
+-rw-r--r--   0        0        0     8098 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/sim_timestep.py
+-rw-r--r--   0        0        0     6096 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/super_starter.py
+-rw-r--r--   0        0        0    12069 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/types/supervisor_container_gt.py
+-rw-r--r--   0        0        0     5788 2023-06-25 19:40:25.888959 gridworks-0.2.7/src/gridworks/utils.py
+-rw-r--r--   0        0        0      788 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/__init__.py
+-rw-r--r--   0        0        0     6947 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/stub_actors.py
+-rw-r--r--   0        0        0     4047 2023-06-25 19:40:42.877121 gridworks-0.2.7/src/gridworks_test/wait.py
+-rw-r--r--   0        0        0     7078 1970-01-01 00:00:00.000000 gridworks-0.2.7/PKG-INFO
```

### Comparing `gridworks-0.2.6/LICENSE` & `gridworks-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/README.md` & `gridworks-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,20 +30,14 @@
 
 To learn how using and contributing to GridWorks can support a cost-effective and rapid transition to a sustainable future:
 
 - Try some simple [Hello World](https://gridworks.readthedocs.io/en/latest/hello-gridworks.html) examples;
 - Read the [Millinocket Story](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html) to learn how to exploit the synergy between wind power and space heating;
 - Go through the partner [Millinocket Tutorial](https://gridworks.readthedocs.io/en/latest/millinocket-tutorial.html).
 
-## Blockchain Mechanics
-
-Gridworks runs markets between distributed actors acting as avatars for physical devices on the grid. It needs a
-foundation of trustless, secure, scalable validation and authentication. It heavily uses the Algorand blockchain. If
-you want to undestand more about how and why this is, go [here](blockchain.html).
-
 ## GridWorks SDKs
 
 - **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for communication and GNode structure. It is used as a package in all of our other repos.
 
 - **gridworks-atn**: [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html) SDK. AtomicTNodes are the GridWorks actors that make electrical devices _transactive_. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.
 
 - **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/) for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK. GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
@@ -55,14 +49,19 @@
 and does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
 is a distributed simulation, it needs a method of handling time. That's done by a [TimeCoordinator](https://github.com/thegridelectric/gridworks-timecoordinator) GNode.
 
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
+## RabbitMQ Infrastructure
+
+GridWorks uses the  `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers. 
+
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

### Comparing `gridworks-0.2.6/pyproject.toml` & `gridworks-0.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks"
-version = "0.2.6"
+version = "0.2.7"
 description = "Gridworks"
 authors = ["GridWorks <gridworks@gridworks-consulting.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks"
 repository = "https://github.com/thegridelectric/gridworks"
 documentation = "https://gridworks.readthedocs.io"
@@ -39,14 +39,15 @@
 aiocache = {version = "^0.11.1", extras = ["redis,memcached"]}
 aioredis = "1.3.1"
 sphinx-rtd-theme = "^1.1.1" # move to dev dependencies. Look to cookie cutter online help.
 
 
 [tool.poetry.dev-dependencies]
 ipython = ">=8.7.0"
+pytest-asyncio = "^0.20.3"
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 flake8 = ">=4.0.1"
 flake8-bandit = ">=2.1.2"
 flake8-bugbear = ">=21.9.2"
```

### Comparing `gridworks-0.2.6/src/gridworks/actor_base.py` & `gridworks-0.2.7/src/gridworks/actor_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import enum
 import functools
 import logging
+import random
 import threading
 import time
 import uuid
 from abc import ABC
 from abc import abstractmethod
 from enum import auto
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import no_type_check
 
 import pendulum
 import pika
 from fastapi_utils.enums import StrEnum
+from pika.channel import Channel as PikaChannel
+from pika.spec import Basic
+from pika.spec import BasicProperties
 
 import gridworks.base_api_types as base_api_types
 import gridworks.property_format as property_format
 import gridworks.utils as utils
 from gridworks.enums import GNodeRole
 from gridworks.enums import MessageCategory
 from gridworks.enums import MessageCategorySymbol
@@ -95,23 +99,26 @@
 LOGGER = logging.getLogger(__name__)
 
 LOGGER.setLevel(logging.INFO)
 
 
 class ActorBase(ABC):
     "This is the base class for GNodes, used to communicate via RabbitMQ"
-    SHUTDOWN_INTERVAL = 0.1
+    _url: str
+
+    SHUTDOWN_INTERVAL: float = 0.1
 
     def __init__(
         self,
         settings: GNodeSettings,
         api_type_maker_by_name: Dict[
             str, HeartbeatA_Maker
         ] = base_api_types.TypeMakerByName,
     ):
+        self.settings: GNodeSettings = settings
         self.api_type_maker_by_name = api_type_maker_by_name
         self.latest_routing_key: Optional[str] = None
         self.shutting_down: bool = False
         self.alias: str = settings.g_node_alias
         self.g_node_instance_id: str = settings.g_node_instance_id
         self.g_node_role: GNodeRole = GNodeRole(settings.g_node_role_value)
         self.rabbit_role: RabbitRole = RabbitRolebyRole[self.g_node_role]
@@ -148,15 +155,15 @@
         )
         self.publishing_thread: threading.Thread = threading.Thread(
             target=self.run_publisher
         )
         self._publish_connection: Optional[
             pika.adapters.select_connection.SelectConnection
         ] = None
-        self._publish_channel: Optional[pika.channel.Channel] = None
+        self._publish_channel: Optional[PikaChannel] = None
         self._stopping: bool = False
         self._stopped: bool = True
         self._latest_on_message_diagnostic: Optional[OnReceiveMessageDiagnostic] = None
 
     def start(self) -> None:
         self.local_start()
         self._stopped = False
@@ -317,19 +324,23 @@
         command. When RabbitMQ responds that the channel is open, the
         on_channel_open callback will be invoked by pika.
         """
         LOGGER.info("Creating a new channel")
         self._consume_connection.channel(on_open_callback=self.on_consumer_channel_open)  # type: ignore
 
     @no_type_check
-    def on_consumer_channel_open(self, channel) -> None:
-        """This method is invoked by pika when the channel has been opened.
-        The channel object is passed in so we can make use of it.
-        Since the channel is now open, we'll declare the exchange to use.
-        :param pika.channel.Channel channel: The channel object
+    def on_consumer_channel_open(self, channel: PikaChannel) -> None:
+        """Invoked by pika when the channel has been successfully opened.
+
+        This callback is triggered when the channel is opened, and it provides
+        the channel object that can be used for further operations. In this case,
+        we'll proceed to declare the exchange to be used.
+
+        :param channel: The opened channel object.
+        :type channel: PikaChannel
         """
         LOGGER.info("Channel opened")
         self._consume_channel = channel
         self.add_on_consume_channel_close_callback()
         self.setup_exchange()
 
     @no_type_check
@@ -337,22 +348,28 @@
         """This method tells pika to call the on_consumer_channel_closed method if
         RabbitMQ unexpectedly closes the channel.
         """
         LOGGER.info("Adding consumer channel close callback")
         self._consume_channel.add_on_close_callback(self.on_consumer_channel_closed)
 
     @no_type_check
-    def on_consumer_channel_closed(self, channel, reason) -> None:
-        """Invoked by pika when RabbitMQ unexpectedly closes the channel.
-        Channels are usually closed if you attempt to do something that
-        violates the protocol, such as re-declare an exchange or queue with
-        different parameters. In this case, we'll close the connection
-        to shutdown the object.
-        :param pika.channel.Channel: The closed channel
-        :param Exception reason: why the channel was closed
+    def on_consumer_channel_closed(
+        self, channel: PikaChannel, reason: Exception
+    ) -> None:
+        """Invoked by pika when the RabbitMQ channel is unexpectedly closed.
+
+        This callback is triggered when a channel is closed, usually due to
+        violating the protocol by attempting to re-declare an exchange or queue
+        with different parameters. In this case, the connection is closed to
+        gracefully shutdown the object.
+
+        :param channel: The closed channel object.
+        :type channel: PikaChannel
+        :param reason: why the channel was closed
+        :type reason: Exception
         """
         LOGGER.warning("Consume channel %i was closed: %s", channel, reason)
         self.close_consumer_connection()
 
     @no_type_check
     def setup_exchange(self) -> None:
         """Setup the exchange on RabbitMQ by invoking the Exchange.Declare RPC
@@ -630,40 +647,50 @@
         by sending the Channel.OpenOK RPC reply, the on_channel_open method
         will be invoked.
         """
         LOGGER.info("Creating a new publish channel")
         self._publish_connection.channel(on_open_callback=self.on_publish_channel_open)  # type: ignore
 
     @no_type_check
-    def on_publish_channel_open(self, channel) -> None:
-        """This method is invoked by pika when the channel has been opened.
-        The channel object is passed in so we can make use of it.
-        Since the channel is now open, we'll declare the exchange to use.
-        :param pika.channel.Channel channel: The channel object
+    def on_publish_channel_open(self, channel: PikaChannel) -> None:
+        """Invoked by pika when the channel has been successfully opened.
+
+        This callback is triggered when the channel is opened, and it provides
+        the channel object that can be used for further operations. In this case,
+        we'll proceed to declare the exchange to be used.
+
+        :param channel: The opened channel object.
+        :type channel: PikaChannel
         """
         LOGGER.info("Publish channel opened")
         self._publish_channel = channel
         self.add_on_publish_channel_close_callback()
 
     def add_on_publish_channel_close_callback(self) -> None:
         """This method tells pika to call the on_channel_closed method if
         RabbitMQ unexpectedly closes the channel.
         """
         LOGGER.info("Adding channel close callback")
         self._publish_channel.add_on_close_callback(self.on_publish_channel_closed)  # type: ignore
 
     @no_type_check
-    def on_publish_channel_closed(self, channel, reason) -> None:
-        """Invoked by pika when RabbitMQ unexpectedly closes the channel.
-        Channels are usually closed if you attempt to do something that
-        violates the protocol, such as re-declare an exchange or queue with
-        different parameters. In this case, we'll close the connection
-        to shutdown the object.
-        :param pika.channel.Channel channel: The closed channel
-        :param Exception reason: why the channel was closed
+    def on_publish_channel_closed(
+        self, channel: PikaChannel, reason: Exception
+    ) -> None:
+        """Invoked by pika when the RabbitMQ channel is unexpectedly closed.
+
+        This callback is triggered when a channel is closed, usually due to
+        violating the protocol by attempting to re-declare an exchange or queue
+        with different parameters. In this case, the connection is closed to
+        gracefully shutdown the object.
+
+        :param channel: The closed channel object.
+        :type channel: PikaChannel
+        :param reason: The reason why the channel was closed.
+        :type reason: Exception
         """
         LOGGER.warning(f"Publish channel {channel} was closed: {reason}")
         self._publish_channel = None
         if not self._stopping:
             self._publish_connection.close()
 
     def run_publisher(self) -> None:
@@ -1021,33 +1048,40 @@
             return OnSendMessageDiagnostic.UNKNOWN_ERROR
 
     #################################################
     # Receiving messages
     #################################################
 
     @no_type_check
-    def on_message(self, _unused_channel, basic_deliver, properties, body) -> None:
-        """Invoked by pika when a message is delivered from RabbitMQ. If a message
+    def on_message(
+        self,
+        _unused_channel: PikaChannel,
+        basic_deliver: Basic.Deliver,
+        properties: BasicProperties,
+        body: bytes,
+    ) -> None:
+        """
+        Invoked by pika when a message is delivered from RabbitMQ. If a message
         does not get here that you expect should get here, check the routing key
         of the outbound message and the rabbitmq bindings.
 
         Parses the TypeName of the message payload and the GNodeAlias of the sender.
-        If it recognizes the GNode and the TypeName then it sends the message on to
+        If it recognizes the GNode and the TypeName, then it sends the message on to
         the check_routing function, which will be defined in a child class (e.g., the
         GNodeFactoryActorBase if the actor is a GNodeFactory).
 
-        From RabbitMQ:  The
-        channel is passed for your convenience. The basic_deliver object that
-        is passed in carries the exchange, routing key, delivery tag and
-        a redelivered flag for the message. The properties passed in is an
-        instance of BasicProperties with the message properties and the body
-        is the message that was sent.
+        From RabbitMQ: The channel is passed for your convenience. The basic_deliver
+        object that is passed in carries the exchange, delivery tag, and a redelivered
+        flag for the message. The properties passed in is an instance of BasicProperties
+        with the message properties including the routing key. The body is the message
+        that was sent.
+
         :param pika.channel.Channel _unused_channel: The channel object
-        :param pika.Spec.Basic.Deliver: basic_deliver method
-        :param pika.Spec.BasicProperties: properties
+        :param pika.spec.Basic.Deliver basic_deliver: The basic.deliver method
+        :param pika.spec.BasicProperties properties: The message properties including the routing key
         :param bytes body: The message body
         """
         self.latest_routing_key = basic_deliver.routing_key
 
         LOGGER.debug(
             f"{self.alias}: Got {basic_deliver.routing_key} with delivery tag {basic_deliver.delivery_tag}"
         )
@@ -1112,26 +1146,99 @@
     ########################
     ## Receives
     ########################
 
     def route_message(
         self, from_alias: str, from_role: GNodeRole, payload: SimTimestep
     ) -> None:
-        """This router should be overwritten by derived class based on the
-        messages received by that GNodeRole"""
-        if payload.TypeName == SimTimestep_Maker.type_name:
+        """
+        Base class for message routing in GNode Actors, handling interactions
+        with the Supervisor and TimeCoordinator.
+
+        Derived classes are expected to implement their own `route_message` method.
+        It is recommended to call `super().route_message(from_alias, from_role, payload)`
+        at the end of the method if the message has not been routed yet.
+        """
+
+        if payload.TypeName == HeartbeatA_Maker.type_name:
+            if from_role != GNodeRole.Supervisor:
+                LOGGER.info(
+                    f"Ignoring HeartbeatA from GNode {from_alias} with GNodeRole {from_role}; expects"
+                    f"Supervisor as the GNodeRole"
+                )
+                return
+            elif from_alias != self.settings.my_super_alias:
+                LOGGER.info(
+                    f"Ignoring HeartbeatA from supervisor {from_alias}; "
+                    f"my supervisor is {self.settings.my_super_alias}"
+                )
+                return
+
+            try:
+                self.heartbeat_from_super(from_alias, payload)
+            except:
+                LOGGER.exception("Error in heartbeat_received")
+        elif payload.TypeName == SimTimestep_Maker.type_name:
             try:
                 self.timestep_from_timecoordinator(payload)
             except:
                 LOGGER.exception("Error in timestep_from_timecoordinator")
 
     def route_mqtt_message(self, from_alias: str, payload: HeartbeatA) -> None:
-        """This router should be overwritten by derived class"""
+        """
+        Base class for message routing from SCADA actors, which use
+        MessageCategory.MqttJsonBroadcast
+
+        This is only intended to be used for AtomicTNodes and Ears.
+        """
         ...
 
+    def heartbeat_from_super(self, from_alias: str, ping: HeartbeatA) -> None:
+        """
+        Subordinate GNode responds to its supervisor's heartbeat with a "pong" message.
+
+        Both the received heartbeat (ping) and the response (pong) have the type HeartbeatA
+        (see: https://gridworks.readthedocs.io/en/latest/apis/types.html#heartbeata).
+
+        The subordinate GNode generates its own unique identifier (hex) and includes it
+        in the pong message along with the heartbeat it received from the supervisor.
+
+        Note that the subordinate GNode does not have the responsibility of verifying
+        the authenticity of the last heartbeat received from the supervisor - although typically,
+        the supervisor does send the last heartbeat from this GNode (except during the initial
+        heartbeat exchange).
+
+        Args:
+            from_alias (str): the alias of the GNode that sent the ping.
+            ping (HeartbeatA): the heartbeat sent.
+
+        Raises:
+        ValueError: If `from_alias` is not this GNode's Supervisor alias.
+
+        """
+        if from_alias != self.settings.my_super_alias:
+            raise ValueError(
+                f"from_alias {from_alias} does not match my supervisor"
+                f" {self.settings.my_super_alias}. This message should"
+                f"have been filtered out in the route_message method."
+            )
+        pong = HeartbeatA_Maker(
+            my_hex=str(random.choice("0123456789abcdef")), your_last_hex=ping.MyHex
+        ).tuple
+
+        self.send_message(
+            payload=pong,
+            to_role=GNodeRole.Supervisor,
+            to_g_node_alias=self.settings.my_super_alias,
+        )
+
+        LOGGER.debug(
+            f"[{self.alias}] Sent HB: SuHex {pong.YourLastHex}, AtnHex {pong.MyHex}"
+        )
+
     ########################
     ## Time related (simulated time)
     ########################
 
     def timestep_from_timecoordinator(self, payload: SimTimestep) -> None:
         if self._time < payload.TimeUnixS:
             self._time = payload.TimeUnixS
```

### Comparing `gridworks-0.2.6/src/gridworks/algo_utils.py` & `gridworks-0.2.7/src/gridworks/algo_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/api_utils.py` & `gridworks-0.2.7/src/gridworks/api_utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/base_api_types.py` & `gridworks-0.2.7/src/gridworks/base_api_types.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/base_g_node.py` & `gridworks-0.2.7/src/gridworks/data_classes/base_g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/g_node.py` & `gridworks-0.2.7/src/gridworks/data_classes/g_node.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/g_node_instance.py` & `gridworks-0.2.7/src/gridworks/data_classes/g_node_instance.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/g_node_strategy.py` & `gridworks-0.2.7/src/gridworks/data_classes/g_node_strategy.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/gps_point.py` & `gridworks-0.2.7/src/gridworks/data_classes/gps_point.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/market_type.py` & `gridworks-0.2.7/src/gridworks/data_classes/market_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/data_classes/supervisor_container.py` & `gridworks-0.2.7/src/gridworks/data_classes/supervisor_container.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/dev_utils/algo_setup.py` & `gridworks-0.2.7/src/gridworks/dev_utils/algo_setup.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/__init__.py` & `gridworks-0.2.7/src/gridworks/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/algo_cert_type.py` & `gridworks-0.2.7/src/gridworks/enums/algo_cert_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/core_g_node_role.py` & `gridworks-0.2.7/src/gridworks/enums/core_g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/g_node_role.py` & `gridworks-0.2.7/src/gridworks/enums/g_node_role.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/g_node_status.py` & `gridworks-0.2.7/src/gridworks/enums/g_node_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/gni_status.py` & `gridworks-0.2.7/src/gridworks/enums/gni_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/market_price_unit.py` & `gridworks-0.2.7/src/gridworks/enums/market_price_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/market_quantity_unit.py` & `gridworks-0.2.7/src/gridworks/enums/market_quantity_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/market_type_name.py` & `gridworks-0.2.7/src/gridworks/enums/market_type_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/message_category.py` & `gridworks-0.2.7/src/gridworks/enums/message_category.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/message_category_symbol.py` & `gridworks-0.2.7/src/gridworks/enums/message_category_symbol.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/recognized_currency_unit.py` & `gridworks-0.2.7/src/gridworks/enums/recognized_currency_unit.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/strategy_name.py` & `gridworks-0.2.7/src/gridworks/enums/strategy_name.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/supervisor_container_status.py` & `gridworks-0.2.7/src/gridworks/enums/supervisor_container_status.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/enums/universe_type.py` & `gridworks-0.2.7/src/gridworks/enums/universe_type.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/message.py` & `gridworks-0.2.7/src/gridworks/message.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/property_format.py` & `gridworks-0.2.7/src/gridworks/property_format.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/rest_api.py` & `gridworks-0.2.7/src/gridworks/rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/__init__.py` & `gridworks-0.2.7/src/gridworks/types/__init__.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/base_g_node_gt.py` & `gridworks-0.2.7/src/gridworks/types/base_g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/g_node_gt.py` & `gridworks-0.2.7/src/gridworks/types/g_node_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/g_node_instance_gt.py` & `gridworks-0.2.7/src/gridworks/types/g_node_instance_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/gw_cert_id.py` & `gridworks-0.2.7/src/gridworks/types/gw_cert_id.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/heartbeat_a.py` & `gridworks-0.2.7/src/gridworks/types/heartbeat_a.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/old_versions/heartbeat_a_001.py` & `gridworks-0.2.7/src/gridworks/types/old_versions/heartbeat_a_001.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/ready.py` & `gridworks-0.2.7/src/gridworks/types/ready.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/sim_timestep.py` & `gridworks-0.2.7/src/gridworks/types/sim_timestep.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/super_starter.py` & `gridworks-0.2.7/src/gridworks/types/super_starter.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/types/supervisor_container_gt.py` & `gridworks-0.2.7/src/gridworks/types/supervisor_container_gt.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks/utils.py` & `gridworks-0.2.7/src/gridworks/utils.py`

 * *Files identical despite different names*

### Comparing `gridworks-0.2.6/src/gridworks_test/wait.py` & `gridworks-0.2.7/src/gridworks_test/wait.py`

 * *Files 17% similar despite different names*

```diff
@@ -101,7 +101,39 @@
             )
         if logger is not None:
             logger.error(err_str)
         if raise_timeout:
             raise ValueError(err_str)
         else:
             return False
+
+
+def wait_for(
+    f: Callable[[], bool],
+    timeout: float,
+    tag: str = "",
+    raise_timeout: bool = True,
+    retry_duration: float = 0.1,
+) -> bool:
+    """Call function f() until it returns True or a timeout is reached. For async tests use await await_for() instead.
+    retry_duration specified the sleep time between calls. If the timeout is reached before f return True, the function
+    will either raise a ValueError (the default), or, if raise_timeout==False, it will return False. Function f is
+    guaranteed to be called at least once. If an exception is raised the tag string will be attached to its message.
+    """
+    now = time.time()
+    until = now + timeout
+    if now >= until:
+        if f():
+            return True
+    while now < until:
+        if f():
+            return True
+        now = time.time()
+        if now < until:
+            time.sleep(min(retry_duration, until - now))
+            now = time.time()
+    if raise_timeout:
+        raise ValueError(
+            f"ERROR. Function {f} timed out after {timeout} seconds. {tag}"
+        )
+    else:
+        return False
```

### Comparing `gridworks-0.2.6/PKG-INFO` & `gridworks-0.2.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridworks
-Version: 0.2.6
+Version: 0.2.7
 Summary: Gridworks
 Home-page: https://github.com/thegridelectric/gridworks
 License: MIT
 Author: GridWorks
 Author-email: gridworks@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -66,20 +66,14 @@
 
 To learn how using and contributing to GridWorks can support a cost-effective and rapid transition to a sustainable future:
 
 - Try some simple [Hello World](https://gridworks.readthedocs.io/en/latest/hello-gridworks.html) examples;
 - Read the [Millinocket Story](https://gridworks.readthedocs.io/en/latest/millinocket-demo.html) to learn how to exploit the synergy between wind power and space heating;
 - Go through the partner [Millinocket Tutorial](https://gridworks.readthedocs.io/en/latest/millinocket-tutorial.html).
 
-## Blockchain Mechanics
-
-Gridworks runs markets between distributed actors acting as avatars for physical devices on the grid. It needs a
-foundation of trustless, secure, scalable validation and authentication. It heavily uses the Algorand blockchain. If
-you want to undestand more about how and why this is, go [here](blockchain.html).
-
 ## GridWorks SDKs
 
 - **gridworks**: [package](https://pypi.org/project/gridworks/) provides basic shared mechanics for communication and GNode structure. It is used as a package in all of our other repos.
 
 - **gridworks-atn**: [package](https://pypi.org/project/gridworks-atn/) and associated [documentation](https://gridworks-atn.readthedocs.io/en/latest/) for the GridWorks Python [AtomicTNodes](https://gridworks.readthedocs.io/en/latest/atomic-t-node.html) SDK. AtomicTNodes are the GridWorks actors that make electrical devices _transactive_. This SDK is a great place to learn about blockchain mechanics, as it introduces some of the simpler structures (NFTs, stateless contracts, and then some simple stateful smart contracts constructed using [beaker](https://github.com/algorand-devrel/beaker) ) required for establishing the link between physical reality on the electric grid and the actors that play their avatars in GridWorks.
 
 - **gridworks-marketmaker**: [package](https://pypi.org/project/gridworks-marketmaker/) and associated [documentation](https://gridworks-marketmaker.readthedocs.io/en/latest/) for our Python [MarketMaker](https://gridworks.readthedocs.io/en/latest/market-maker.html) SDK. GridWorks uses distributed actors to balance the electric grid, and MarketMakers are the actors brokering this grid balancing via the markets they run for energy and balancing services.
@@ -91,14 +85,19 @@
 and does most of the heavy lifting in terms of identity management and authentication in GridWorks. Finally, since the demo
 is a distributed simulation, it needs a method of handling time. That's done by a [TimeCoordinator](https://github.com/thegridelectric/gridworks-timecoordinator) GNode.
 
 ## Usage
 
 `pip install gridworks` to install the foundational package.
 
+## RabbitMQ Infrastructure
+
+GridWorks uses the  `rabbit` subfolder for maintaining dev rabbit brokers as well as their own live rabbit brokers. 
+
+
 ## Contributing
 
 Contributions are very welcome.
 To learn more, see the [Contributor Guide].
 
 ## License
```

