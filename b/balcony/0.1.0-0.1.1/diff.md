# Comparing `tmp/balcony-0.1.0.tar.gz` & `tmp/balcony-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.0.tar", max compression
+gzip compressed data, was "balcony-0.1.1.tar", max compression
```

## Comparing `balcony-0.1.0.tar` & `balcony-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,41 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.0/LICENSE
--rw-r--r--   0        0        0     2250 2023-05-17 18:38:17.580378 balcony-0.1.0/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.0/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.0/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.0/balcony/aws.py
--rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.1.0/balcony/botocore_utils.py
--rw-r--r--   0        0        0    14364 2023-05-09 17:42:32.497330 balcony-0.1.0/balcony/cli.py
--rw-r--r--   0        0        0     2978 2023-04-30 21:07:33.646010 balcony-0.1.0/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.0/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.0/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.0/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.0/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.0/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.0/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.0/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.0/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.0/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.0/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.0/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.0/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.0/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.0/balcony/errors.py
--rw-r--r--   0        0        0    48117 2023-04-29 22:05:26.837497 balcony-0.1.0/balcony/nodes.py
--rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.1.0/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.0/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.0/balcony/relations.py
--rw-r--r--   0        0        0     2533 2023-04-21 19:19:57.046512 balcony-0.1.0/balcony/test.py
--rw-r--r--   0        0        0     5373 2023-05-09 17:56:32.379928 balcony-0.1.0/balcony/utils.py
--rw-r--r--   0        0        0     2739 2023-04-30 21:55:13.504191 balcony-0.1.0/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-04-29 22:16:26.774034 balcony-0.1.0/balcony/yaml_validators.py
--rw-r--r--   0        0        0      663 2023-05-17 18:36:50.877883 balcony-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3344 1970-01-01 00:00:00.000000 balcony-0.1.0/setup.py
--rw-r--r--   0        0        0     3250 1970-01-01 00:00:00.000000 balcony-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1890 2023-06-22 10:24:32.348247 balcony-0.1.1/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.1/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.1/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.1/balcony/aws.py
+-rw-r--r--   0        0        0    11892 2023-04-21 17:50:16.401554 balcony-0.1.1/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    19026 2023-06-25 12:59:49.346224 balcony-0.1.1/balcony/cli.py
+-rw-r--r--   0        0        0     3621 2023-06-18 17:53:12.079460 balcony-0.1.1/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.1/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.1/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.1/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.1/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.1/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.1/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.1/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.1/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.1/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0      647 2023-06-22 14:01:11.797785 balcony-0.1.1/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.1/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.1/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      517 2023-04-06 12:50:36.974851 balcony-0.1.1/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.1/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.1/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.1/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.1/balcony/errors.py
+-rw-r--r--   0        0        0    48206 2023-06-19 13:08:46.777156 balcony-0.1.1/balcony/nodes.py
+-rw-r--r--   0        0        0    17113 2023-05-01 12:20:53.387726 balcony-0.1.1/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.1/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.1/balcony/relations.py
+-rw-r--r--   0        0        0     1407 2023-06-25 08:18:38.934823 balcony-0.1.1/balcony/terraform_import/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.1/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0     6272 2023-06-25 12:23:39.913627 balcony-0.1.1/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.1/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     2276 2023-06-23 11:28:47.429086 balcony-0.1.1/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.1/balcony/test.py
+-rw-r--r--   0        0        0     6108 2023-06-18 17:25:37.430772 balcony-0.1.1/balcony/utils.py
+-rw-r--r--   0        0        0     2130 2023-06-18 18:03:08.298654 balcony-0.1.1/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.1/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-06-25 14:35:22.458376 balcony-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3126 1970-01-01 00:00:00.000000 balcony-0.1.1/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 balcony-0.1.1/PKG-INFO
```

### Comparing `balcony-0.1.0/LICENSE` & `balcony-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/README.md` & `balcony-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -18,22 +18,21 @@
 
 
 ## Installation & Documentation 
 
 **[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/balcony/quickstart)**
 
 Balcony's documentation website contains quickstart guide, usage cookbook and more.
-## Features & GIFs
-> click to play the videos
-### List available AWS Services 
-`balcony aws` to see every AWS service available.
 
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/aws-services-list.gif)
 
 
+
+
+## Features & GIFs
+> click to play the videos
 ### List Resource Nodes of an AWS Service 
 `balcony aws <service-name>` to see every Resource Node of a service.
 
 ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif)
 
 
 ### Reading a Resource Node 
@@ -43,13 +42,7 @@
 
 
 ### Documentation and Input & Output of Operations
 Use the `--list`, `-l` flag to print the given AWS API Operations documentation, input & output structure. 
  
 
 ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)
-
-
-### Enable Debug messages 
-Use the `--debug`, `-d` flag to see what's going on under the hood!
-
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/debug-messages.gif)
```

#### html2text {}

```diff
@@ -5,20 +5,15 @@
 parameters for each operation. By **establishing relations between operations
 over required parameters**, it's **able to auto-fill** them by reading the
 related operation beforehand. By simply entering their name, balcony enables
 developers to easily list their AWS resources. ## Installation & Documentation
 **[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/
 balcony/quickstart)** Balcony's documentation website contains quickstart
 guide, usage cookbook and more. ## Features & GIFs > click to play the videos
-### List available AWS Services `balcony aws` to see every AWS service
-available. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/
-visuals/aws-services-list.gif) ### List Resource Nodes of an AWS Service
-`balcony aws ` to see every Resource Node of a service. ![](https://github.com/
-oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif) ###
-Reading a Resource Node `balcony aws  ` to read operations of a Resource Node.
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-
-resource-node.gif) ### Documentation and Input & Output of Operations Use the
-`--list`, `-l` flag to print the given AWS API Operations documentation, input
-& output structure. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/
-docs/visuals/list-option.gif) ### Enable Debug messages Use the `--debug`, `-d`
-flag to see what's going on under the hood! ![](https://github.com/oguzhan-
-yilmaz/balcony/blob/main/docs/visuals/debug-messages.gif)
+### List Resource Nodes of an AWS Service `balcony aws ` to see every Resource
+Node of a service. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/
+docs/visuals/resource-node-list.gif) ### Reading a Resource Node `balcony aws
+` to read operations of a Resource Node. ![](https://github.com/oguzhan-yilmaz/
+balcony/blob/main/docs/visuals/reading-a-resource-node.gif) ### Documentation
+and Input & Output of Operations Use the `--list`, `-l` flag to print the given
+AWS API Operations documentation, input & output structure. ![](https://
+github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)
```

### Comparing `balcony-0.1.0/balcony/__init__.py` & `balcony-0.1.1/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/aws.py` & `balcony-0.1.1/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/botocore_utils.py` & `balcony-0.1.1/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/cli.py` & `balcony-0.1.1/balcony/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import json
 import textwrap
 from utils import (
     get_all_available_services,
     ifind_similar_names_in_list,
-    _create_boto_session
+    _create_boto_session,
 )
 from config import (
     get_logger,
     get_rich_console,
     set_log_level_at_runtime,
     clear_relations_cache,
 )
+
 # required for loading custom resource nodes into registry
 from custom_nodes import *  # noqa
 from aws import BalconyAWS
 
 import typer
 import jmespath
 from typing import Optional, List, Dict, Generator
 from rich.columns import Columns
 from rich.panel import Panel
 import logging
 import boto3
 from pathlib import Path
-
+from terraform_import.importer import (
+    generate_import_block_for_resource,
+    get_importable_resources,
+)
+from rich.padding import Padding
 
 console = get_rich_console()
 logger = get_logger(__name__)
 session = _create_boto_session()
 balcony_aws = BalconyAWS(session)
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_enable=False)
 
@@ -43,15 +48,16 @@
 def save_dict_to_output_file(output_filepath: str, data: Dict):
     with open(output_filepath, "w") as f:
         json.dump(data, f, indent=2, default=str)
 
 
 def save_str_list_to_output_file(output_filepath: str, lines: List[str]):
     with open(output_filepath, "w") as f:
-        f.writelines([line + "\n" for line in lines])
+        if lines:
+            f.writelines([str(line) + "\n" for line in lines])
 
 
 def _complete_service_name(incomplete: str) -> Generator[str, None, None]:
     """Typer autocompletion function. Finds matching service names.
 
     Args:
         incomplete (str): Service names that're starting with this string.
@@ -65,15 +71,17 @@
             yield name
     else:
         for name in service_names:
             if name.startswith(incomplete):
                 yield name
 
 
-def _complete_resource_node_name(ctx: typer.Context, incomplete: str) -> Generator[str, None, None]:
+def _complete_resource_node_name(
+    ctx: typer.Context, incomplete: str
+) -> Generator[str, None, None]:
     service = ctx.params.get("service", False)
     if not service:
         return []
     service_node = balcony_aws.get_service_node(service)
     if not service_node:
         return []
     resource_nodes = service_node.get_resource_nodes()
@@ -260,26 +268,22 @@
             "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
         )
     service_markup = f"[green]{service}[/]"
     resource_node_markup = f"[green]{service}[/].[blue]{resource_node}[/]"
 
     if not service and not resource_node:
         # print out resource nodes of this service.
-        _list_service_or_resource(
-            service, resource_node, screen_pager=screen
-        )
+        _list_service_or_resource(service, resource_node, screen_pager=screen)
         console.print(
             Panel("[bold]Please pick one of the AWS Services", title="[red][bold]ERROR")
         )
         raise typer.Exit()
 
     if service and not resource_node:
-        _list_service_or_resource(
-            service, resource_node, screen_pager=screen
-        )
+        _list_service_or_resource(service, resource_node, screen_pager=screen)
         console.print(
             Panel(
                 f"[bold]Please pick one of the Resource Nodes from {service_markup} Service",
                 title="[red][bold]ERROR",
             )
         )
         raise typer.Exit()
@@ -358,39 +362,172 @@
             logger.info(f"Saving output to: {output_filepath}")
             save_dict_to_output_file(output_filepath, read_data)
         else:
             console.print_json(data=read_data, default=str)
         raise typer.Exit()
 
 
+@app.command(
+    "terraform-import",
+    no_args_is_help=True,
+    help="Generate Terraform import blocks for a given AWS Service and Resource Node.",
+)
+def terraform_import_command(
+    service: Optional[str] = typer.Argument(
+        None,
+        show_default=False,
+        help="Name of the AWS Service (e.g. ec2, s3, rds)",
+        autocompletion=_complete_service_name,
+    ),
+    resource_node: Optional[str] = typer.Argument(
+        None,
+        show_default=False,
+        help="Name of the AWS Resource Node. (e.g. Instances, Buckets, DBInstances)",
+        autocompletion=_complete_resource_node_name,
+    ),
+    debug: bool = typer.Option(False, "--debug", "-d", help="Enable debug messages."),
+    follow_pagination: bool = typer.Option(
+        False,
+        "--paginate",
+        "-p",
+        help="Paginate through the output if the output is truncated, otherwise will only read one page.",
+    ),
+    list_available_resources: bool = typer.Option(
+        False,
+        "--list",
+        "-l",
+        help="Lists currently available resources for generating Terraform import blocks.",
+    ),
+    output_file: str = typer.Option(
+        None,
+        "--output",
+        "-o",
+        show_default=False,
+        help="Output file name. If not provided, will print to console.",
+    ),
+):
+    # set debug level if enabled
+    if debug:
+        set_log_level_at_runtime(logging.DEBUG)
+
+    # warn user if pagination is not set
+    if not follow_pagination:
+        logger.debug(
+            "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
+        )
+
+    if list_available_resources:
+        service_resource_list = get_importable_resources()
+
+        def render_importable_resources(service_and_resource_tuples: List[Tuple]):
+            header = f"[bold green]{'service':<15} {'resource_name':<45}[/]\n".format()
+            result = header
+
+            for i, (service_name, resource_name) in enumerate(
+                service_and_resource_tuples
+            ):
+
+                cur_line = f"{service_name:<15} {resource_name:<45}"
+                if i % 2:
+                    cur_line = f"[bold]{cur_line}[/]"
+                result += cur_line + "\n"
+            return result
+
+        rendered_service_resource_list = render_importable_resources(
+            service_resource_list
+        )
+        console.print(rendered_service_resource_list)
+        return  # list option is enabled, do not run the actual importing code.
+
+    if (not service) or (not resource_node):
+        screen = False
+        _list_service_or_resource(service, resource_node, screen_pager=screen)
+
+        console.print(f"{service=} {resource_node=}")
+        console.print(f"[red bold]Please pick a Service and Resource Node[/]")
+        return
+
+    import_blocks = generate_import_block_for_resource(
+        balcony_aws,
+        service,
+        resource_node,
+        follow_pagination=follow_pagination,
+    )
+
+    if not import_blocks:
+        logger.debug(f"No import blocks generated for {service}.{resource_node}")
+
+        fail_msg = textwrap.dedent(
+            f"""
+            No terraform import blocks generated for [bold]{service}.{resource_node}[/]. Some checks:
+                
+                - [underline]Run the balcony with [bold]--debug[/] flag to see more info.[/]
+                    Run     [bold]balcony terraform-import --debug {service} {resource_node}[/]
+                    
+                - [underline]Do you have the correct AWS credentials and Region?[/]
+                    Run     [bold]printenv | grep ^AWS_[/]
+                
+                - [underline]Is the resource node name correct?[/]
+                    Run     [bold]balcony aws {service}[/]      to see available resource nodes.
+                
+                - [underline]You may not have any resources in your AWS Account, check it first:[/]
+                    Run     [bold]balcony aws {service} {resource_node} -d[/] 
+            """
+        ).strip()
+        console.print(Padding(fail_msg, (1, 1)))
+        raise typer.Exit(-1)
+
+    if output_file:
+        output_filepath = Path(output_file).resolve()
+        logger.info(f"Saving output to: {output_filepath}")
+        save_str_list_to_output_file(output_filepath, import_blocks)
+        raise typer.Exit()
+
+    else:
+        console.print("\n".join(import_blocks))
+
+    return import_blocks
+
+
 @app.command("clear-cache", help="Clear relations json cache")
 def clear_cache_command(
     # service: Optional[str] = typer.Argument(None, show_default='all',
     # help='Name of the Service to clear relation caches of', autocompletion=_complete_service_name),
 ):
     logger.debug("Deleting relations cache for services:")
     deleted_service_caches = clear_relations_cache()
     for deleted_service in deleted_service_caches:
         logger.info(f"[green]Deleted[/] {deleted_service}")
 
 
-@app.command("info", help="Information about the AWS Profile and Region currently used", )
+@app.command(
+    "info",
+    help="Information about the AWS Profile and Region currently used",
+)
 def info_command():
     created_session = balcony_aws.boto3_session
-    console.print(f"[bold underline]AWS Region:[/] [bold blue]{created_session.region_name}[/]")
-    console.print(f"[bold underline]AWS Profile:[/] [bold blue]{created_session.profile_name}")
+    console.print(
+        f"[bold underline]AWS Region:[/] [bold blue]{created_session.region_name}[/]"
+    )
+    console.print(
+        f"[bold underline]AWS Profile:[/] [bold blue]{created_session.profile_name}"
+    )
     console.print()
     console.print("[bold underline]Available Profiles:[/]")
 
     for available_profile in created_session.available_profiles or []:
         console.print(f"  - [green bold]{available_profile}[/]")
-    console.print(textwrap.dedent("""
+    console.print(
+        textwrap.dedent(
+            """
         [yellow]You can configure the AWS Profile and Region by setting the
         the $[bold]AWS_DEFAULT_REGION[/] and $[bold]AWS_PROFILE[/] environment variables.[/]
-    """))
+    """
+        )
+    )
 
 
 # @app.command('version', help='Show version info' )
 # def version_command():
 #     from importlib.metadata import version
 #     console.print(__package__)
 #     version=version(__package__)
```

### Comparing `balcony-0.1.0/balcony/config.py` & `balcony-0.1.1/balcony/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,41 @@
 import logging
 from rich.logging import RichHandler
 from rich.console import Console
 import os
 from pathlib import Path
 
+
+_console = Console(color_system="auto", markup=True, )
+_balcony_loggers = []
+
+
+def get_logger(name: str) -> logging.Logger:
+    """Logger creation with RichHandler.
+
+    Args:
+        name (str): Logger name. Usually given `__name__`.
+
+    Returns:
+        logging.Logger: Logger obj
+    """
+    supress_other_module_logs()
+    logging.basicConfig(
+        level=LOG_LEVEL,
+        format="%(message)s",
+        datefmt="[%X]",
+        handlers=[RichHandler(markup=True, console=_console)]
+    )
+
+    _logger = logging.getLogger(name)
+    # keep track of the created loggers
+    _balcony_loggers.append(_logger)
+    return _logger
+
+
 HOME_DIR = os.path.expanduser('~')
 
 # Defaults to ~/.balcony/
 BALCONY_CONFIG_DIR = os.getenv('BALCONY_CONFIG_DIR', os.path.join(HOME_DIR, '.balcony'))
 
 # Defaults to ~/.balcony/relations/
 BALCONY_RELATIONS_DIR = os.getenv('BALCONY_RELATIONS_DIR', os.path.join(BALCONY_CONFIG_DIR, 'relations'))
@@ -17,16 +45,23 @@
 
 LOG_LEVEL = 'INFO'
 
 # YamlResourceNode customization parameters
 YAML_IGNORE_PREFIX = "_"
 YAML_SERVICES_DIRECTORY = Path(__file__).parent / "custom_yamls"
 
-_console = Console(color_system="auto", markup=True, )
-_balcony_loggers = []
+# Terraform Import Config customization parameters
+YAML_TF_IMPORT_CONFIGS_DIRECTORY = Path(__file__).parent / "custom_tf_import_configs"
+
+USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY = os.getenv('BALCONY_TERRAFOM_IMPORT_CONFIG_DIR', False)
+if USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY and not Path(USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY).exists():
+    # make sure the given directory exists, or disable the feature
+    get_logger(__name__).warning(f"Given BALCONY_TERRAFOM_IMPORT_CONFIG_DIR: \
+            {USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY} don't exist.")
+    USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY = False
 
 
 def clear_relations_cache() -> None:
     """Removes the cached relations of services in the  `$BALCONY_RELATIONS_DIR/<service>.json` files."""
     relation_files = os.listdir(BALCONY_RELATIONS_DIR)
     deleted_filenames = []
     for rel_file in relation_files:
@@ -64,29 +99,7 @@
     for _logger in _balcony_loggers:
         _logger.setLevel(log_level)
         # for handler in _logger.handlers:
         #     if isinstance(handler, type(logging.StreamHandler())):
         #         handler.setLevel(log_level)
         #         _logger.debug('Debug logging enabled')
 
-
-def get_logger(name: str) -> logging.Logger:
-    """Logger creation with RichHandler.
-
-    Args:
-        name (str): Logger name. Usually given `__name__`.
-
-    Returns:
-        logging.Logger: Logger obj
-    """
-    supress_other_module_logs()
-    logging.basicConfig(
-        level=LOG_LEVEL,
-        format="%(message)s",
-        datefmt="[%X]",
-        handlers=[RichHandler(markup=True, console=_console)]
-    )
-
-    _logger = logging.getLogger(name)
-    # keep track of the created loggers
-    _balcony_loggers.append(_logger)
-    return _logger
```

### Comparing `balcony-0.1.0/balcony/custom_nodes/codebuild.py` & `balcony-0.1.1/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/ecs.py` & `balcony-0.1.1/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/iam.py` & `balcony-0.1.1/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.1/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/s3.py` & `balcony-0.1.1/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/ses.py` & `balcony-0.1.1/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_nodes/ssm.py` & `balcony-0.1.1/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.1/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.1/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/custom_yamls/iam.yaml` & `balcony-0.1.1/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/nodes.py` & `balcony-0.1.1/balcony/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,26 +493,27 @@
         console.print(operation_panel)
 
     def _rich_operation_details_panel(self, operation_name: str) -> Panel:
 
         operation_model = self.get_operation_model(operation_name)
         input_shape = get_input_shape(operation_model)
         output_shape = operation_model.output_shape
-
-        input_shape_tree = Text("[yellow]No Input Shape Found")
+        input_shape_name = 'No Input Shape Found'
+        input_shape_tree = Text("No Input Shape Found")
         if input_shape:
             input_shape_tree = generate_rich_tree_from_shape(input_shape)
+            input_shape_name = input_shape.name
         output_shape_tree = generate_rich_tree_from_shape(output_shape)
 
         operation_docs = cleanhtml(operation_model.documentation)
         panel_group = Group(
             Padding(f"[bold underline]Documentation:[/] {operation_docs}", (1, 2)),
             Panel(
                 input_shape_tree,
-                title=f"Input: [yellow]{input_shape.name}",
+                title=f"Input: [yellow]{input_shape_name}",
                 title_align="left",
                 padding=(1, 1),
             ),
             Panel(
                 output_shape_tree,
                 title=f"Output: [yellow]{output_shape.name}",
                 title_align="left",
```

### Comparing `balcony-0.1.0/balcony/reader.py` & `balcony-0.1.1/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/registries.py` & `balcony-0.1.1/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/relations.py` & `balcony-0.1.1/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/balcony/test.py` & `balcony-0.1.1/balcony/test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 from aws import BalconyAWS
-from utils import is_word_in_a_list_of_words
-from typing import Dict, List, Union
-from nodes import PAGINATION_TOKEN_KEYS
-
-def get_pagination_token_output_to_parameter_name_mapping(
-    self, operation_name: str
-) -> Union[Dict[str, str], bool]:
-    """Some Operations paginate their output using Pagination Token Parameters defined in `PAGINATION_TOKEN_KEYS`.
-
-    Args:
-        resource_node (ResourceNode): _description_
-        operation_name (str): Name of the operation in the resource_node.
-
-    Returns:
-        Union[Dict[str, str], bool]: False or A dictionary with `parameter_name` and `output_key` keys. e.g. `{"parameter_name":"nextToken", "output_key": "NextToken"}`.
-    """
-    resource_node = self
-
-    # find all parameter names that are in `PAGINATION_TOKEN_KEYS`, case insensitive
-    parameter_names = [
-        pn
-        for pn in resource_node.get_all_parameter_names_from_operation_name(
-            operation_name
-        )
-        if is_word_in_a_list_of_words(pn, PAGINATION_TOKEN_KEYS)
-    ]
-
-    #  find all output keys that are in `PAGINATION_TOKEN_KEYS`, case insensitive
-    output_keys = [
-        ok
-        for ok in resource_node.get_all_output_keys_from_operation_name(
-            operation_name
-        )
-        if is_word_in_a_list_of_words(ok, PAGINATION_TOKEN_KEYS)
-    ]
-
-    if output_keys and parameter_names:
-        return {
-            "parameter_name": parameter_names[0],
-            "output_key": output_keys[0],
-        }
-    return False
-
-
-def main():
-    baws = BalconyAWS()
-    aws_services = baws.get_available_service_names()
-    for aws_service_name in aws_services[aws_services.index("lexv2-runtime") :]:
-        print(aws_service_name)
-        service_node = baws.get_service_node(aws_service_name)
-        for resource_node in service_node.get_resource_nodes():
-            for operation_name in resource_node.get_operation_names():
-                a = get_pagination_token_output_to_parameter_name_mapping(
-                    resource_node, operation_name
-                )
-                print(a)
-
-                # "nexttoken, continuationtoken, marker"
-                # rpp = [_ for _ in rp if "token" in _.lower() or "marker" in _.lower()]
-                # opp = [_ for _ in op if "token" in _.lower() or "marker" in _.lower()]
-                # if rpp or opp:
-                #     print(
-                #         f"  {operation_name} :: {','.join(rpp)} --::-- {','.join(opp)}"
-                #     )
+from terraform_import.main import main as terraform_import_main
 
+balcony_aws = BalconyAWS()
+tf_import_blocks = terraform_import_main(balcony_aws, "ec2", "Instances")
+print('\n\n'.join(tf_import_blocks))
+
+tf_import_blocks = terraform_import_main(balcony_aws, "s3", "Buckets")
+print('\n\n'.join(tf_import_blocks))
+tf_import_blocks
+
+
+# from utils import is_word_in_a_list_of_words
+# from typing import Dict, List, Union
+# from nodes import PAGINATION_TOKEN_KEYS
+
+# def get_pagination_token_output_to_parameter_name_mapping(
+#     self, operation_name: str
+# ) -> Union[Dict[str, str], bool]:
+#     """Some Operations paginate their output using Pagination Token Parameters defined in `PAGINATION_TOKEN_KEYS`.
+
+#     Args:
+#         resource_node (ResourceNode): _description_
+#         operation_name (str): Name of the operation in the resource_node.
+
+#     Returns:
+#         Union[Dict[str, str], bool]: False or A dictionary with `parameter_name` and `output_key` keys. e.g. `{"parameter_name":"nextToken", "output_key": "NextToken"}`.
+#     """
+#     resource_node = self
+
+#     # find all parameter names that are in `PAGINATION_TOKEN_KEYS`, case insensitive
+#     parameter_names = [
+#         pn
+#         for pn in resource_node.get_all_parameter_names_from_operation_name(
+#             operation_name
+#         )
+#         if is_word_in_a_list_of_words(pn, PAGINATION_TOKEN_KEYS)
+#     ]
+
+#     #  find all output keys that are in `PAGINATION_TOKEN_KEYS`, case insensitive
+#     output_keys = [
+#         ok
+#         for ok in resource_node.get_all_output_keys_from_operation_name(
+#             operation_name
+#         )
+#         if is_word_in_a_list_of_words(ok, PAGINATION_TOKEN_KEYS)
+#     ]
+
+#     if output_keys and parameter_names
+
+#         return {
+#             "parameter_name": parameter_names[0],
+#             "output_key": output_keys[0],
+#         }
+#     return False
+
+
+# def main():
+#     baws = BalconyAWS()
+#     aws_services = baws.get_available_service_names()
+#     for aws_service_name in aws_services[aws_services.index("lexv2-runtime") :]:
+#         print(aws_service_name)
+#         service_node = baws.get_service_node(aws_service_name)
+#         for resource_node in service_node.get_resource_nodes():
+#             for operation_name in resource_node.get_operation_names():
+#                 a = get_pagination_token_output_to_parameter_name_mapping(
+#                     resource_node, operation_name
+#                 )
+#                 print(a)
+
+#                 # "nexttoken, continuationtoken, marker"
+#                 # rpp = [_ for _ in rp if "token" in _.lower() or "marker" in _.lower()]
+#                 # opp = [_ for _ in op if "token" in _.lower() or "marker" in _.lower()]
+#                 # if rpp or opp:
+#                 #     print(
+#                 #         f"  {operation_name} :: {','.join(rpp)} --::-- {','.join(opp)}"
+#                 #     )
 
-def __():
-    pass
 
+# def __():
+#     pass
 
-main()
+
+# main()
```

### Comparing `balcony-0.1.0/balcony/utils.py` & `balcony-0.1.1/balcony/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,56 @@
 from collections import Counter
 from re import finditer, compile
 import textwrap
 from typing import List
 import inflect
 import os
 import boto3
-from config import get_logger
+from config import get_logger, YAML_IGNORE_PREFIX
 import botocore
+
 # from functools import lru_cache
 
 inflect_engine = inflect.engine()  # used for singular/plural word comparing
 logger = get_logger(__name__)
 
 _camel_case_regex_compiled = compile(
     r".+?(?:(?<=[a-z])(?=[A-Z])|(?<=[A-Z])(?=[A-Z][a-z])|$)"
 )
 
 
+def find_all_yaml_files(directory: str) -> List[str]:
+    """Find all .yaml files in a directory with the exception of files starting with "_".
+
+    Args:
+        directory (str): Directory to search for yaml files
+
+    Returns:
+        List[str]: List of yaml file paths
+    """
+    yaml_files = []
+    for root, _, files in os.walk(directory):
+        for file in files:
+            # support any yaml file with the exception of files starting with "YAML_IGNORE_PREFIX"
+            if file.endswith(".yaml") and not file.startswith(YAML_IGNORE_PREFIX):
+                yaml_files.append(os.path.join(root, file))
+    return yaml_files
+
+
 def _create_boto_session():
     """Tries to create a boto3 session with the given environment variables.
     Handles the exceptions and exits the program if it fails.
 
     Returns:
         boto3.session.Session: created boto3 session
     """
     profile_name = os.environ.get("AWS_PROFILE", False)
-    region_name = os.environ.get("AWS_REGION", False) or os.environ.get("AWS_DEFAULT_REGION", False)
+    region_name = os.environ.get("AWS_REGION", False) or os.environ.get(
+        "AWS_DEFAULT_REGION", False
+    )
     _kwargs_dict = {}
     if profile_name:
         _kwargs_dict["profile_name"] = profile_name
     if region_name:
         _kwargs_dict["region_name"] = region_name
     session = None
 
@@ -65,22 +86,27 @@
             return True
     return False
 
     return word.lower() in []
 
 
 def inform_about_develeoping_custom_resource_nodes():
-    logger.debug(textwrap.dedent("""
+    logger.debug(
+        textwrap.dedent(
+            """
         [bold yellow][FAILURE][/] It seems balcony [red bold]failed[/] to read this operation. 
         
         You can create Custom ResourceNodes to fix the failed operation. 
         Visit [bold][link=https://oguzhan-yilmaz.github.io/balcony/development/developing-custom-resource-nodes/]Custom Resource Development Documentation[/link][/] to learn more.
         
         You can also track the [bold][link=https://github.com/oguzhan-yilmaz/balcony/issues]Github Issues[/link][/] or create a new issue.
-        """.lstrip('\n'))
+        """.lstrip(
+                "\n"
+            )
+        )
     )
 
 
 def ifind_similar_names_in_list(
     search_for: str, search_in_list: List[str]
 ) -> List[str]:
     """Case insensitive find in list"""
```

### Comparing `balcony-0.1.0/balcony/yaml_config.py` & `balcony-0.1.1/balcony/yaml_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from config import get_logger, YAML_IGNORE_PREFIX, YAML_SERVICES_DIRECTORY
 from yaml_validators import YamlService
-
+from utils import find_all_yaml_files
 import yaml
-import os
 from typing import List, Union, Tuple
 from pathlib import Path
 
 
 logger = get_logger(__name__)
 
 
@@ -26,30 +25,14 @@
         with open(yaml_file_path, "r") as f:
             input_data = yaml.load(f, Loader=yaml.FullLoader)
         return YamlService(**input_data), None
     except Exception as e:
         return False, e
 
 
-def find_all_yaml_files(directory: str) -> List[str]:
-    """Find all yaml files in a directory with the exception of files starting with "_".
-
-    Args:
-        directory (str): Directory to search for yaml files
-
-    Returns:
-        List[str]: List of yaml file paths
-    """
-    yaml_files = []
-    for root, _, files in os.walk(directory):
-        for file in files:
-            # support any yaml file with the exception of files starting with "YAML_IGNORE_PREFIX"
-            if file.endswith(".yaml") and not file.startswith(YAML_IGNORE_PREFIX):
-                yaml_files.append(os.path.join(root, file))
-    return yaml_files
 
 
 def find_and_parse_yaml_services() -> List[YamlService]:
     """Searches and finds the defined yaml files in the YAML_SERVICES_DIRECTORY directory that are not starting with '_'
 
     Returns:
         List[YamlService]: List of found YamlServices, created from yaml files
```

### Comparing `balcony-0.1.0/balcony/yaml_validators.py` & `balcony-0.1.1/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.0/pyproject.toml` & `balcony-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.0"
-description = "AWS API for humans"
+version = "0.1.1"
+description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
 
@@ -17,14 +17,15 @@
 jmespath = "^1.0.1"
 inflect = "^6.0.0"
 mkdocstrings = {version = "^0.21.2", extras = ["python"]}
 mkdocs-material = ">=8.5.7,<10.0.0"
 mkdocs-autorefs = "^0.4.1"
 PyYAML = "^6.0"
 pydantic = "^1.10.7"
+Jinja2 = "^3.1.2"
 
 
 [tool.poetry.group.dev.dependencies]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `balcony-0.1.0/setup.py` & `balcony-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['balcony', 'balcony.custom_nodes']
+['balcony', 'balcony.custom_nodes', 'balcony.terraform_import']
 
 package_data = \
-{'': ['*'], 'balcony': ['custom_yamls/*']}
+{'': ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 
 install_requires = \
-['PyYAML>=6.0,<7.0',
+['Jinja2>=3.1.2,<4.0.0',
+ 'PyYAML>=6.0,<7.0',
  'boto3>=1.24.80,<2.0.0',
  'inflect>=6.0.0,<7.0.0',
  'jmespath>=1.0.1,<2.0.0',
  'mkdocs-autorefs>=0.4.1,<0.5.0',
  'mkdocs-material>=8.5.7,<10.0.0',
  'mkdocstrings[python]>=0.21.2,<0.22.0',
  'pydantic>=1.10.7,<2.0.0',
@@ -20,17 +21,17 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.0',
-    'description': 'AWS API for humans',
-    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes required parameters for each operation. \n\nBy **establishing relations between operations over required parameters**, it\'s **able to auto-fill** them by reading the related operation beforehand.\n\nBy simply entering their name, balcony enables developers to easily list their AWS resources.\n\n\n## Installation & Documentation \n\n**[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/balcony/quickstart)**\n\nBalcony\'s documentation website contains quickstart guide, usage cookbook and more.\n## Features & GIFs\n> click to play the videos\n### List available AWS Services \n`balcony aws` to see every AWS service available.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/aws-services-list.gif)\n\n\n### List Resource Nodes of an AWS Service \n`balcony aws <service-name>` to see every Resource Node of a service.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif)\n\n\n### Reading a Resource Node \n`balcony aws <service-name> <resource-node>` to read operations of a Resource Node.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-resource-node.gif)\n\n\n### Documentation and Input & Output of Operations\nUse the `--list`, `-l` flag to print the given AWS API Operations documentation, input & output structure. \n \n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)\n\n\n### Enable Debug messages \nUse the `--debug`, `-d` flag to see what\'s going on under the hood!\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/debug-messages.gif)\n',
+    'version': '0.1.1',
+    'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
+    'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes required parameters for each operation. \n\nBy **establishing relations between operations over required parameters**, it\'s **able to auto-fill** them by reading the related operation beforehand.\n\nBy simply entering their name, balcony enables developers to easily list their AWS resources.\n\n\n## Installation & Documentation \n\n**[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/balcony/quickstart)**\n\nBalcony\'s documentation website contains quickstart guide, usage cookbook and more.\n\n\n\n\n\n## Features & GIFs\n> click to play the videos\n### List Resource Nodes of an AWS Service \n`balcony aws <service-name>` to see every Resource Node of a service.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif)\n\n\n### Reading a Resource Node \n`balcony aws <service-name> <resource-node>` to read operations of a Resource Node.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-resource-node.gif)\n\n\n### Documentation and Input & Output of Operations\nUse the `--list`, `-l` flag to print the given AWS API Operations documentation, input & output structure. \n \n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,38 +1,36 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['balcony',
-'balcony.custom_nodes'] package_data = \ {'': ['*'], 'balcony': ['custom_yamls/
-*']} install_requires = \ ['PyYAML>=6.0,<7.0', 'boto3>=1.24.80,<2.0.0',
-'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0', 'mkdocs-
-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0', 'mkdocstrings
-[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0', 'rich>=13.3.4,<14.0.0',
-'typer>=0.7.0,<0.8.0'] entry_points = \ {'console_scripts': ['balcony =
-balcony.cli:run_app']} setup_kwargs = { 'name': 'balcony', 'version': '0.1.0',
-'description': 'AWS API for humans', 'long_description': '# balcony\n\n\n
+'balcony.custom_nodes', 'balcony.terraform_import'] package_data = \ {'':
+['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
+install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
+'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
+'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
+'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
+'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
+{'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
+'balcony', 'version': '0.1.1', 'description': 'Read any resource in your AWS
+Account. You can generate terraform code for them, too.', 'long_description':
+'# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\n\nbalcony dynamically parses AWS SDK(`boto3` library) and analyzes
 required parameters for each operation. \n\nBy **establishing relations between
 operations over required parameters**, it\'s **able to auto-fill** them by
 reading the related operation beforehand.\n\nBy simply entering their name,
 balcony enables developers to easily list their AWS resources.\n\n\n##
 Installation & Documentation \n\n**[https://oguzhan-yilmaz.github.io/balcony/]
 (https://oguzhan-yilmaz.github.io/balcony/quickstart)**\n\nBalcony\'s
-documentation website contains quickstart guide, usage cookbook and more.\n##
-Features & GIFs\n> click to play the videos\n### List available AWS Services
-\n`balcony aws` to see every AWS service available.\n\n![](https://github.com/
-oguzhan-yilmaz/balcony/blob/main/docs/visuals/aws-services-list.gif)\n\n\n###
-List Resource Nodes of an AWS Service \n`balcony aws ` to see every Resource
-Node of a service.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/
-docs/visuals/resource-node-list.gif)\n\n\n### Reading a Resource Node
-\n`balcony aws  ` to read operations of a Resource Node.\n\n![](https://
-github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-resource-
-node.gif)\n\n\n### Documentation and Input & Output of Operations\nUse the `--
-list`, `-l` flag to print the given AWS API Operations documentation, input &
-output structure. \n \n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/
-main/docs/visuals/list-option.gif)\n\n\n### Enable Debug messages \nUse the `--
-debug`, `-d` flag to see what\'s going on under the hood!\n\n![](https://
-github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/debug-
-messages.gif)\n', 'author': 'Oguzhan Yilmaz', 'author_email':
+documentation website contains quickstart guide, usage cookbook and
+more.\n\n\n\n\n\n## Features & GIFs\n> click to play the videos\n### List
+Resource Nodes of an AWS Service \n`balcony aws ` to see every Resource Node of
+a service.\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/
+visuals/resource-node-list.gif)\n\n\n### Reading a Resource Node \n`balcony aws
+` to read operations of a Resource Node.\n\n![](https://github.com/oguzhan-
+yilmaz/balcony/blob/main/docs/visuals/reading-a-resource-node.gif)\n\n\n###
+Documentation and Input & Output of Operations\nUse the `--list`, `-l` flag to
+print the given AWS API Operations documentation, input & output structure. \n
+\n\n![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-
+option.gif)\n', 'author': 'Oguzhan Yilmaz', 'author_email':
 'oguzhanylmz271@gmail.com', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'None', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'entry_points': entry_points,
 'python_requires': '>=3.7,<4.0', } setup(**setup_kwargs)
```

### Comparing `balcony-0.1.0/PKG-INFO` & `balcony-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.0
-Summary: AWS API for humans
+Version: 0.1.1
+Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
 License: GPL-3.0-or-later
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: boto3 (>=1.24.80,<2.0.0)
 Requires-Dist: inflect (>=6.0.0,<7.0.0)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0)
 Requires-Dist: mkdocs-material (>=8.5.7,<10.0.0)
 Requires-Dist: mkdocstrings[python] (>=0.21.2,<0.22.0)
@@ -44,22 +45,21 @@
 
 
 ## Installation & Documentation 
 
 **[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/balcony/quickstart)**
 
 Balcony's documentation website contains quickstart guide, usage cookbook and more.
-## Features & GIFs
-> click to play the videos
-### List available AWS Services 
-`balcony aws` to see every AWS service available.
 
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/aws-services-list.gif)
 
 
+
+
+## Features & GIFs
+> click to play the videos
 ### List Resource Nodes of an AWS Service 
 `balcony aws <service-name>` to see every Resource Node of a service.
 
 ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif)
 
 
 ### Reading a Resource Node 
@@ -70,13 +70,7 @@
 
 ### Documentation and Input & Output of Operations
 Use the `--list`, `-l` flag to print the given AWS API Operations documentation, input & output structure. 
  
 
 ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)
 
-
-### Enable Debug messages 
-Use the `--debug`, `-d` flag to see what's going on under the hood!
-
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/debug-messages.gif)
-
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.0 Summary: AWS API for humans
-License: GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email:
-oguzhanylmz271@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License :: OSI
-Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: boto3
+Metadata-Version: 2.1 Name: balcony Version: 0.1.1 Summary: Read any resource
+in your AWS Account. You can generate terraform code for them, too. License:
+GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
+Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
+Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
+:: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
+(>=3.1.2,<4.0.0) Requires-Dist: PyYAML (>=6.0,<7.0) Requires-Dist: boto3
 (>=1.24.80,<2.0.0) Requires-Dist: inflect (>=6.0.0,<7.0.0) Requires-Dist:
 jmespath (>=1.0.1,<2.0.0) Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0)
 Requires-Dist: mkdocs-material (>=8.5.7,<10.0.0) Requires-Dist: mkdocstrings
 [python] (>=0.21.2,<0.22.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-
 Dist: rich (>=13.3.4,<14.0.0) Requires-Dist: typer (>=0.7.0,<0.8.0)
 Description-Content-Type: text/markdown # balcony
 [Build_and_publish_a_Docker_image_to_ghcr.io]  [Build_and_Deploy_Documentation
@@ -18,20 +19,15 @@
 parameters for each operation. By **establishing relations between operations
 over required parameters**, it's **able to auto-fill** them by reading the
 related operation beforehand. By simply entering their name, balcony enables
 developers to easily list their AWS resources. ## Installation & Documentation
 **[https://oguzhan-yilmaz.github.io/balcony/](https://oguzhan-yilmaz.github.io/
 balcony/quickstart)** Balcony's documentation website contains quickstart
 guide, usage cookbook and more. ## Features & GIFs > click to play the videos
-### List available AWS Services `balcony aws` to see every AWS service
-available. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/
-visuals/aws-services-list.gif) ### List Resource Nodes of an AWS Service
-`balcony aws ` to see every Resource Node of a service. ![](https://github.com/
-oguzhan-yilmaz/balcony/blob/main/docs/visuals/resource-node-list.gif) ###
-Reading a Resource Node `balcony aws  ` to read operations of a Resource Node.
-![](https://github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/reading-a-
-resource-node.gif) ### Documentation and Input & Output of Operations Use the
-`--list`, `-l` flag to print the given AWS API Operations documentation, input
-& output structure. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/
-docs/visuals/list-option.gif) ### Enable Debug messages Use the `--debug`, `-d`
-flag to see what's going on under the hood! ![](https://github.com/oguzhan-
-yilmaz/balcony/blob/main/docs/visuals/debug-messages.gif)
+### List Resource Nodes of an AWS Service `balcony aws ` to see every Resource
+Node of a service. ![](https://github.com/oguzhan-yilmaz/balcony/blob/main/
+docs/visuals/resource-node-list.gif) ### Reading a Resource Node `balcony aws
+` to read operations of a Resource Node. ![](https://github.com/oguzhan-yilmaz/
+balcony/blob/main/docs/visuals/reading-a-resource-node.gif) ### Documentation
+and Input & Output of Operations Use the `--list`, `-l` flag to print the given
+AWS API Operations documentation, input & output structure. ![](https://
+github.com/oguzhan-yilmaz/balcony/blob/main/docs/visuals/list-option.gif)
```

