# Comparing `tmp/gns3fy-1.0.0rc2.tar.gz` & `tmp/gns3fy-1.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gns3fy-1.0.0rc2.tar", max compression
+gzip compressed data, was "gns3fy-1.0.0rc3.tar", max compression
```

## Comparing `gns3fy-1.0.0rc2.tar` & `gns3fy-1.0.0rc3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10395 2021-01-04 20:09:47.702729 gns3fy-1.0.0rc2/README.md
--rw-r--r--   0        0        0      157 2021-01-11 03:22:01.034261 gns3fy-1.0.0rc2/gns3fy/__init__.py
--rw-r--r--   0        0        0     1159 2021-01-11 05:24:31.143853 gns3fy-1.0.0rc2/gns3fy/base.py
--rw-r--r--   0        0        0     4780 2022-05-28 08:40:43.049676 gns3fy-1.0.0rc2/gns3fy/connector.py
--rw-r--r--   0        0        0     7078 2021-01-11 05:24:54.302011 gns3fy-1.0.0rc2/gns3fy/drawings.py
--rw-r--r--   0        0        0     3809 2021-01-11 05:26:47.511201 gns3fy-1.0.0rc2/gns3fy/helpers.py
--rw-r--r--   0        0        0    11087 2021-01-11 05:25:10.908041 gns3fy-1.0.0rc2/gns3fy/links.py
--rw-r--r--   0        0        0    16158 2021-01-11 05:25:31.843147 gns3fy-1.0.0rc2/gns3fy/nodes.py
--rw-r--r--   0        0        0     1286 2021-01-11 04:01:53.775029 gns3fy-1.0.0rc2/gns3fy/ports.py
--rw-r--r--   0        0        0    27469 2021-05-09 10:45:29.599868 gns3fy-1.0.0rc2/gns3fy/projects.py
--rw-r--r--   0        0        0     8598 2021-01-11 04:41:06.693948 gns3fy-1.0.0rc2/gns3fy/server.py
--rw-r--r--   0        0        0     4783 2021-01-11 05:26:09.172882 gns3fy-1.0.0rc2/gns3fy/snapshots.py
--rw-r--r--   0        0        0     6181 2021-01-11 05:27:23.526814 gns3fy-1.0.0rc2/gns3fy/templates.py
--rw-r--r--   0        0        0     1038 2022-05-28 08:43:13.650977 gns3fy-1.0.0rc2/pyproject.toml
--rw-r--r--   0        0        0    11341 2022-05-28 08:45:15.349823 gns3fy-1.0.0rc2/setup.py
--rw-r--r--   0        0        0    11221 2022-05-28 08:45:15.350852 gns3fy-1.0.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    10395 2021-01-04 20:09:47.702729 gns3fy-1.0.0rc3/README.md
+-rw-r--r--   0        0        0      157 2021-01-11 03:22:01.034261 gns3fy-1.0.0rc3/gns3fy/__init__.py
+-rw-r--r--   0        0        0     1159 2021-01-11 05:24:31.143853 gns3fy-1.0.0rc3/gns3fy/base.py
+-rw-r--r--   0        0        0     4780 2022-05-28 08:40:43.049676 gns3fy-1.0.0rc3/gns3fy/connector.py
+-rw-r--r--   0        0        0     7078 2021-01-11 05:24:54.302011 gns3fy-1.0.0rc3/gns3fy/drawings.py
+-rw-r--r--   0        0        0     3809 2021-01-11 05:26:47.511201 gns3fy-1.0.0rc3/gns3fy/helpers.py
+-rw-r--r--   0        0        0    11190 2022-05-30 16:24:49.555205 gns3fy-1.0.0rc3/gns3fy/links.py
+-rw-r--r--   0        0        0    16158 2021-01-11 05:25:31.843147 gns3fy-1.0.0rc3/gns3fy/nodes.py
+-rw-r--r--   0        0        0     1286 2021-01-11 04:01:53.775029 gns3fy-1.0.0rc3/gns3fy/ports.py
+-rw-r--r--   0        0        0    27469 2021-05-09 10:45:29.599868 gns3fy-1.0.0rc3/gns3fy/projects.py
+-rw-r--r--   0        0        0     8598 2021-01-11 04:41:06.693948 gns3fy-1.0.0rc3/gns3fy/server.py
+-rw-r--r--   0        0        0     4783 2021-01-11 05:26:09.172882 gns3fy-1.0.0rc3/gns3fy/snapshots.py
+-rw-r--r--   0        0        0     6181 2021-01-11 05:27:23.526814 gns3fy-1.0.0rc3/gns3fy/templates.py
+-rw-r--r--   0        0        0     1038 2022-05-30 16:45:55.262102 gns3fy-1.0.0rc3/pyproject.toml
+-rw-r--r--   0        0        0    11341 2022-05-30 16:46:56.735044 gns3fy-1.0.0rc3/setup.py
+-rw-r--r--   0        0        0    11221 2022-05-30 16:46:56.735962 gns3fy-1.0.0rc3/PKG-INFO
```

### Comparing `gns3fy-1.0.0rc2/README.md` & `gns3fy-1.0.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/base.py` & `gns3fy-1.0.0rc3/gns3fy/base.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/connector.py` & `gns3fy-1.0.0rc3/gns3fy/connector.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/drawings.py` & `gns3fy-1.0.0rc3/gns3fy/drawings.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/helpers.py` & `gns3fy-1.0.0rc3/gns3fy/helpers.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/links.py` & `gns3fy-1.0.0rc3/gns3fy/links.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     GNS3 Link API object. For more information visit: [Links Endpoint API information](
     https://gns3-server.readthedocs.io/en/2.2/api/v2/controller/link.html)
 
     **Attributes:**
 
     - `link_id` (str): Link UUID (**required** to be set when using `get` method)
     - `link_type` (enum): Possible values: ethernet, serial
+    - `link_style` (dict): Describes the visual style of the link
     - `project_id` (str): Project UUID (**required**)
     - `connector` (object): `Connector` instance used for interaction (**required**)
     - `suspend` (bool): Suspend the link
     - `nodes` (list): List of the Nodes and ports (**required** when using `create`
     method, see Features/Link creation on the docs)
     - `filters` (dict): Packet filter. This allow to simulate latency and errors
     - `capturing` (bool): Read only property. True if a capture running on the link
@@ -46,14 +47,15 @@
     ```
     """
 
     project_id: str
     link_id: str
     _connector: Connector = PrivateAttr()
     link_type: Optional[str] = None
+    link_style: Optional[Any] = None
     suspend: Optional[bool] = None
     filters: Optional[Any] = None
     capturing: Optional[bool] = None
     capture_file_path: Optional[str] = None
     capture_file_name: Optional[str] = None
     capture_compute_id: Optional[str] = None
     nodes: List[Port] = Field(default_factory=list)
```

### Comparing `gns3fy-1.0.0rc2/gns3fy/nodes.py` & `gns3fy-1.0.0rc3/gns3fy/nodes.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/ports.py` & `gns3fy-1.0.0rc3/gns3fy/ports.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/projects.py` & `gns3fy-1.0.0rc3/gns3fy/projects.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/server.py` & `gns3fy-1.0.0rc3/gns3fy/server.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/snapshots.py` & `gns3fy-1.0.0rc3/gns3fy/snapshots.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/gns3fy/templates.py` & `gns3fy-1.0.0rc3/gns3fy/templates.py`

 * *Files identical despite different names*

### Comparing `gns3fy-1.0.0rc2/pyproject.toml` & `gns3fy-1.0.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gns3fy"
-version = "1.0.0-rc.2"
+version = "1.0.0-rc.3"
 description = "Python SDK around GNS3 Server REST API"
 authors = ["David Flores <davidflores7_8@hotmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/davidban77/gns3fy"
 homepage = "https://github.com/davidban77/gns3fy"
 keywords = ["network", "gns3", "python", "restapi", "netdev"]
```

### Comparing `gns3fy-1.0.0rc2/setup.py` & `gns3fy-1.0.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.0,<2.0', 'requests>=2.22,<3.0']
 
 setup_kwargs = {
     'name': 'gns3fy',
-    'version': '1.0.0rc2',
+    'version': '1.0.0rc3',
     'description': 'Python SDK around GNS3 Server REST API',
     'long_description': '# gns3fy\n\n[![Circle CI](https://circleci.com/gh/davidban77/gns3fy/tree/develop.svg?style=shield&circle-token=:circle-token)](https://circleci.com/gh/davidban77/gns3fy/tree/develop)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![codecov](https://codecov.io/gh/davidban77/gns3fy/branch/develop/graph/badge.svg)](https://codecov.io/gh/davidban77/gns3fy)\n[![Total alerts](https://img.shields.io/lgtm/alerts/g/davidban77/gns3fy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/davidban77/gns3fy/alerts/)\n[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/davidban77/gns3fy.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/davidban77/gns3fy/context:python)\n[![pypi](https://img.shields.io/pypi/v/gns3fy.svg)](https://pypi.python.org/pypi/gns3fy)\n[![versions](https://img.shields.io/pypi/pyversions/gns3fy.svg)](https://github.com/davidban77/gns3fy)\n\nPython wrapper around [GNS3 Server API](http://api.gns3.net/en/2.2/index.html). Minimal GNS3 version is 2.2.\n\nIts main objective is to interact with the GNS3 server in a programatic way, so it can be integrated with the likes of Ansible, docker and scripts. Ideal for network CI/CD pipeline tooling.\n\n## Documentation\n\nCheck out the [Documentation](https://davidban77.github.io/gns3fy/) to explore use cases and the API Reference\n\n## Use cases\n\nHere are some examples where gns3fy is used in a programmatic way:\n\n- [Ansible-collection-gns3](https://galaxy.ansible.com/davidban77/gns3): Useful for CI/CD pipelines to interact with GNS3 server using Ansible. It can create/delete projects, nodes and links in an ansible playbook.\n- Terraform: Coming soon... (although it might be a Go version of it)\n- [Migrate templates between GNS3 servers](https://davidban77.github.io/gns3fy/user-guide/#migrate-templates-between-gns3-servers)\n- [Check server usage](https://davidban77.github.io/gns3fy/user-guide/#check-server-cpu-and-memory-usage) before turning up resource-hungry nodes\n- [Manipulate project snapshots](https://davidban77.github.io/gns3fy/user-guide/#create-and-list-project-snapshots) like create, delete or list the snapshots configured for the project.\n\n## Install\n\n```shell\npip install gns3fy\n```\n\n### Development version\n\nUse [poetry](https://github.com/sdispater/poetry) to install the package when cloning it.\n\n## How it works\n\nYou can start the library and use the `Gns3Connector` object and the `Project` object.\n\nFor example:\n\n```python\nimport gns3fy.services as gns3\n\n# For a pretty output\nfrom rich.table import Table\nfrom rich import print as rprint\n\n# Create GNS3 connector object\nserver = gns3.create_connector("http://gns3-server:80")\n\n# Create Rich table for pretty printing\ntable = Table("Project Name", "Total Nodes", "Total Links", "Status", "Project ID", title="GNS3 Projectes")\n\nfor prj in gns3.get_projects(server):\n    # Retrieve all attributes (nodes, links, snapshots, drawings) from a project\n    prj.get()\n    # Add a row per project\n    table.add_row(prj.name, str(len(prj.nodes)), str(len(prj.links)), prj.status, prj.project_id)\n\n\nrprint(table)\n"""\n                                       GNS3 Projectes\n┏━━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━━━━━━┳━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Project Name ┃ Total Nodes ┃ Total Links ┃ Status ┃ Project ID                           ┃\n┡━━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━━━━━━╇━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ labby_test   │ 5           │ 7           │ closed │ 944ee3f1-977f-4794-bbbb-b52d993b502a │\n│ oob_site2    │ 4           │ 3           │ opened │ d000bbc4-6540-4039-b366-cf873cdebc53 │\n│ mpls_v2      │ 7           │ 8           │ closed │ 6ba8cf63-8441-42e1-8d67-8798651a97a9 │\n│ netmon       │ 7           │ 12          │ opened │ 01e7f910-7ed6-407d-a0a3-cb1e1c0cc6f6 │\n│ test2        │ 0           │ 0           │ closed │ 5f250655-5ebf-4475-b296-9093b422c735 │\n└──────────────┴─────────────┴─────────────┴────────┴──────────────────────────────────────┘\n"""\n\n# Define the lab you want to load and assign the server connector\nlab = gns3.search_project(server, name="labby_test")\nrepr(lab)\n"""\nProject(name=\'labby_test\', project_id=\'944ee3f1-977f-4794-bbbb-b52d993b502a\', status=\'closed\', ...)\n"""\n\n# Access the project attributes\nprint(f"Name: {lab.name} -- Status: {lab.status} -- Is auto_closed?: {lab.auto_close}")\n"""\nName: labby_test -- Status: closed -- Is auto_closed?: True\n"""\n\n# Open the project\nlab.open()\nlab.status\n"""\nopened\n"""\n\n# Verify the general stats of the project (these were retrieved with gns3.refresh_project)\nstats_table = Table("Nodes", "Links", "Snapshots", "Drawings", title=f"Project: {lab.name}")\nstats_table.add_row(\n    str(len(lab.nodes)), str(len(lab.links)), str(len(lab.snapshots)), str(len(lab.drawings))\n)\nrprint(stats_table)\n"""\n          Project: labby_test\n┏━━━━━━━┳━━━━━━━┳━━━━━━━━━━━┳━━━━━━━━━━┓\n┃ Nodes ┃ Links ┃ Snapshots ┃ Drawings ┃\n┡━━━━━━━╇━━━━━━━╇━━━━━━━━━━━╇━━━━━━━━━━┩\n│ 5     │ 7     │ 0         │ 0        │\n└───────┴───────┴───────────┴──────────┘\n"""\n\n# List the names and status of all the nodes in the project\nnode_table = Table("Node Name", "Type", "Status", title="Projects Nodes")\nfor node in lab.nodes:\n    node_table.add_row(node.name, node.node_type, node.status)\n\n"""\n             Projects Nodes\n┏━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━┳━━━━━━━━━┓\n┃ Node Name ┃ Type            ┃ Status  ┃\n┡━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━╇━━━━━━━━━┩\n│ r3        │ qemu            │ stopped │\n│ cloud1    │ cloud           │ started │\n│ r1        │ qemu            │ stopped │\n│ r2        │ qemu            │ stopped │\n│ sw1       │ ethernet_switch │ started │\n└───────────┴─────────────────┴─────────┘\n"""\n```\n\nTake a look at the API documentation for complete information about the attributes retrieved.\n\n### Usage of Node and Link objects\n\nYou have access to the `Node` and `Link` objects as well, this gives you the ability to start, stop, suspend the individual element in a GNS3 project.\n\n```python\n# Search for a specific node in the lab project\nr3 = gns3.search_node(project=lab, name="r3")\nrepr(r3)\n"""\nNode(name=\'r3\', node_type=\'qemu\', template=\'Cisco IOSv\' ...)\n"""\n\n# You can access useful node information\nprint(f"Name: {r3.name} -- Status: {r3.status} -- Console: {r3.console}")\n"""\nName: r3 -- Status: stopped -- Console: 5006\n"""\n\n# Start the node\nr3.start()\nr3.status\n"""\nstarted\n"""\n\n# See links information\nrepr(r3.links)\n"""\n{Link(link_id=\'4d9f1235-7fd1-466b-ad26-0b4b08beb778\', link_type=\'ethernet\', ...)}\n"""\n\n# Information of the links information\n\n\n>>> from gns3fy import Node, Link, Gns3Connector\n\n>>> PROJECT_ID = "<some project id>"\n>>> server = Gns3Connector("http://<server address>:3080")\n\n>>> alpine1 = Node(project_id=PROJECT_ID, name="alpine-1", connector=server)\n\n>>> alpine1.get()\n>>> print(alpine1)\n"Node(name=\'alpine-1\', node_type=\'docker\', node_directory= ...)"\n\n# And you can access the attributes the same way as the project\n>>> print(f"Name: {alpine1.name} -- Status: {alpine1.status} -- Console: {alpine1.console}")\n"Name: alpine-1 -- Status: started -- Console: 5005"\n\n# Stop the node and start (you can just restart it as well)\n>>> alpine1.stop()\n>>> alpine1.status\nstopped\n\n>>> alpine1.start()\n>>> alpine1.status\nstarted\n\n# You can also see the Link objects assigned to this node\n>>> alpine1.links\n[Link(link_id=\'4d9f1235-7fd1-466b-ad26-0b4b08beb778\', link_type=\'ethernet\', ...)]\n\n# And in the same way you can interact with a Link object\n>>> link1 = alpine1.links[0]\n>>> print(f"Link Type: {link1.link_type} -- Capturing?: {link1.capturing} -- Endpoints: {link1.nodes}")\n"Link Type: ethernet -- Capturing?: False -- Endpoints: [{\'adapter_number\': 2, ...}]"\n```\n\n### Useful functions\n\nYou also have some commodity methods like the `nodes_summary` and `links_summary`, that if used with a library like `tabulate` you can see the following:\n\n```python\n\n>>> from tabulate import tabulate\n\n>>> nodes_summary = lab.nodes_summary(is_print=False)\n\n>>> print(\n...     tabulate(nodes_summary, headers=["Node", "Status", "Console Port", "ID"])\n... )\n"""\nNode              Status      Console Port  ID\n----------------  --------  --------------  ------------------------------------\nEthernetswitch-1  started             5000  da28e1c0-9465-4f7c-b42c-49b2f4e1c64d\nIOU1              started             5001  de23a89a-aa1f-446a-a950-31d4bf98653c\nIOU2              started             5002  0d10d697-ef8d-40af-a4f3-fafe71f5458b\nvEOS-4.21.5F-1    started             5003  8283b923-df0e-4bc1-8199-be6fea40f500\nalpine-1          started             5005  ef503c45-e998-499d-88fc-2765614b313e\nCloud-1           started                   cde85a31-c97f-4551-9596-a3ed12c08498\n"""\n>>> links_summary = lab.links_summary(is_print=False)\n>>> print(\n...     tabulate(links_summary, headers=["Node A", "Port A", "Node B", "Port B"])\n... )\n"""\nNode A          Port A       Node B            Port B\n--------------  -----------  ----------------  -----------\nIOU1            Ethernet1/0  IOU2              Ethernet1/0\nvEOS-4.21.5F-1  Management1  Ethernetswitch-1  Ethernet0\nvEOS-4.21.5F-1  Ethernet1    alpine-1          eth0\nCloud-1         eth1         Ethernetswitch-1  Ethernet7\n"""\n```\n',
     'author': 'David Flores',
     'author_email': 'davidflores7_8@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/davidban77/gns3fy',
```

### Comparing `gns3fy-1.0.0rc2/PKG-INFO` & `gns3fy-1.0.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gns3fy
-Version: 1.0.0rc2
+Version: 1.0.0rc3
 Summary: Python SDK around GNS3 Server REST API
 Home-page: https://github.com/davidban77/gns3fy
 License: MIT
 Keywords: network,gns3,python,restapi,netdev
 Author: David Flores
 Author-email: davidflores7_8@hotmail.com
 Requires-Python: >=3.6,<4.0
```

