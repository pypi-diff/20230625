# Comparing `tmp/dagster_polars-0.0.1.tar.gz` & `tmp/dagster_polars-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster_polars-0.0.1.tar", max compression
+gzip compressed data, was "dagster_polars-0.0.2.tar", max compression
```

## Comparing `dagster_polars-0.0.1.tar` & `dagster_polars-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0    11344 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/LICENSE
--rw-r--r--   0        0        0     2031 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/README.md
--rw-r--r--   0        0        0      314 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/__init__.py
--rw-r--r--   0        0        0       76 2023-06-12 07:41:16.377835 dagster_polars-0.0.1/dagster_polars/_version.py
--rw-r--r--   0        0        0        0 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/__init__.py
--rw-r--r--   0        0        0     6354 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/base.py
--rw-r--r--   0        0        0     1263 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/io_managers/parquet.py
--rw-r--r--   0        0        0        0 2023-06-12 07:40:39.647304 dagster_polars-0.0.1/dagster_polars/py.typed
--rw-r--r--   0        0        0     2736 2023-06-12 07:41:16.377835 dagster_polars-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3194 1970-01-01 00:00:00.000000 dagster_polars-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2443 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/README.md
+-rw-r--r--   0        0        0      324 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/__init__.py
+-rw-r--r--   0        0        0       76 2023-06-25 09:30:38.628701 dagster_polars-0.0.2/dagster_polars/_version.py
+-rw-r--r--   0        0        0        0 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/__init__.py
+-rw-r--r--   0        0        0     5977 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/base.py
+-rw-r--r--   0        0        0     7200 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/bigquery.py
+-rw-r--r--   0        0        0     1278 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/parquet.py
+-rw-r--r--   0        0        0     3936 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/io_managers/utils.py
+-rw-r--r--   0        0        0        0 2023-06-25 09:30:11.752404 dagster_polars-0.0.2/dagster_polars/py.typed
+-rw-r--r--   0        0        0     2806 2023-06-25 09:30:38.624701 dagster_polars-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3689 1970-01-01 00:00:00.000000 dagster_polars-0.0.2/PKG-INFO
```

### Comparing `dagster_polars-0.0.1/LICENSE` & `dagster_polars-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster_polars-0.0.1/README.md` & `dagster_polars-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,41 @@
 # `dagster-polars`
 
 [Polars](https://github.com/pola-rs/polars) integration library for [Dagster](https://github.com/dagster-io/dagster).
 
 ## Features
- - `PolarsIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
+ - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
+ - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
+ - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
-   - logs various metadata about the DataFrame - size, schema, sample, stats, ...
-   - the "columns" input metadata value can be used to select a subset of columns
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark).
+ - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified).
 
 ## Quickstart
 
 ### Installation
 
 ```shell
 pip install dagster-polars
 ```
 
+To use the `BigQueryPolarsIOManager` you need to install the `gcp` extra:
+```shell
+pip install 'dagster-polars[gcp]'
+```
+
+
 ### Usage
 ```python
+import polars as pl
 from dagster import asset, Definitions
 from dagster_polars import PolarsParquetIOManager
-import polars as pl
 
 
 @asset(io_manager_key="polars_parquet_io_manager")
 def upstream() -> pl.DataFrame:
     df: pl.DataFrame = ...
     return df
 
@@ -57,10 +64,10 @@
 
 ### Testing
 ```shell
 poetry run pytest
 ```
 
 ## TODO
-
+ - [ ] Add `PolarsDeltaIOManager`
  - [ ] Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
  - [ ] Maybe use `DagsterTypeLoader` ?
```

### Comparing `dagster_polars-0.0.1/dagster_polars/io_managers/base.py` & `dagster_polars-0.0.2/dagster_polars/io_managers/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     TableSchema,
     UPathIOManager,
 )
 from dagster import _check as check
 from pydantic.fields import Field, PrivateAttr
 from upath import UPath
 
+from dagster_polars.io_managers.utils import get_polars_metadata
+
 POLARS_DATA_FRAME_ANNOTATIONS = [
     Any,
     pl.DataFrame,
     Dict[str, pl.DataFrame],
     Mapping[str, pl.DataFrame],
     type(None),
     None,
@@ -119,15 +121,15 @@
     describe = df.describe().fill_null(pl.lit("null"))
     return {
         col: {stat: describe[col][i] for i, stat in enumerate(describe["describe"].to_list())}
         for col in describe.columns[1:]
     }
 
 
-class BasePolarsIOManager(ConfigurableIOManager, UPathIOManager):
+class BasePolarsUPathIOManager(ConfigurableIOManager, UPathIOManager):
     # This is a base class which doesn't define the specific format (parquet, csv, etc) to use
     """
     `IOManager` for `polars` based on the `UPathIOManager`.
     Features:
      - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
      - logs various metadata about the DataFrame - size, schema, sample, stats, ...
      - the "columns" input metadata value can be used to select a subset of columns
@@ -171,23 +173,8 @@
             return ldf.collect(streaming=True)
         elif context.dagster_type.typing_type in POLARS_LAZY_FRAME_ANNOTATIONS:
             return ldf
         else:
             raise NotImplementedError(f"Can't load object for type annotation {context.dagster_type.typing_type}")
 
     def get_metadata(self, context: OutputContext, obj: pl.DataFrame) -> Dict[str, MetadataValue]:
-        assert context.metadata is not None
-        schema, table = get_metadata_table_and_schema(
-            context=context, df=obj, descriptions=context.metadata.get("descriptions")
-        )
-
-        metadata = {
-            "stats": MetadataValue.json(get_polars_df_stats(obj)),
-            "row_count": MetadataValue.int(len(obj)),
-        }
-
-        if table is not None:
-            metadata["table"] = table
-        else:
-            metadata["schema"] = schema
-
-        return metadata
+        return get_polars_metadata(context, obj)
```

### Comparing `dagster_polars-0.0.1/dagster_polars/io_managers/parquet.py` & `dagster_polars-0.0.2/dagster_polars/io_managers/parquet.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import fsspec
 import polars as pl
 import pyarrow.dataset as ds
 from dagster import InitResourceContext, InputContext, OutputContext, io_manager
 from upath import UPath
 
-from dagster_polars.io_managers.base import BasePolarsIOManager
+from dagster_polars.io_managers.base import BasePolarsUPathIOManager
 
 
-class PolarsParquetIOManager(BasePolarsIOManager):
+class PolarsParquetIOManager(BasePolarsUPathIOManager):
     extension: str = ".parquet"
 
-    __doc__ = BasePolarsIOManager.__doc__ + """\nWorks with Parquet files"""  # type: ignore
+    __doc__ = BasePolarsUPathIOManager.__doc__ + """\nWorks with Parquet files"""  # type: ignore
 
     def dump_df_to_path(self, context: OutputContext, df: pl.DataFrame, path: UPath):
         with path.open("wb") as file:
             df.write_parquet(file)
 
     def scan_df_from_path(self, path: UPath, context: InputContext) -> pl.LazyFrame:
         fs: Union[fsspec.AbstractFileSystem, None] = None
```

### Comparing `dagster_polars-0.0.1/pyproject.toml` & `dagster_polars-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dagster-polars"
-version = "0.0.1"
+version = "0.0.2"
 description = "Dagster integration library for Polars"
 authors = [
     "Daniel Gafni <danielgafni16@gmail.com>"
 ]
 readme = "README.md"
 packages = [{include = "dagster_polars"}]
 repository = "https://github.com/danielgafni/dagster-polars"
@@ -26,14 +26,20 @@
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dagster = "^1.3.5"
 polars = ">=0.17.0"
 pyarrow = ">=8.0.0"
+dagster-gcp = "^0.19.5"
+
+
+[tool.poetry.extras]
+gcp = ["dagster-gcp"]
+
 
 
 [tool.poetry.group.dev.dependencies]
 hypothesis = "^6.77.0"
 pytest = "^7.3.1"
 deepdiff = "^6.3.0"
 isort = "^5.12.0"
```

### Comparing `dagster_polars-0.0.1/PKG-INFO` & `dagster_polars-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-polars
-Version: 0.0.1
+Version: 0.0.2
 Summary: Dagster integration library for Polars
 Home-page: https://github.com/danielgafni/dagster-polars
 License: Apache-2.0
 Keywords: dagster,polars,ETL,dataframe
 Author: Daniel Gafni
 Author-email: danielgafni16@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -16,47 +16,56 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Provides-Extra: gcp
 Requires-Dist: dagster (>=1.3.5,<2.0.0)
+Requires-Dist: dagster-gcp (>=0.19.5,<0.20.0) ; extra == "gcp"
 Requires-Dist: polars (>=0.17.0)
 Requires-Dist: pyarrow (>=8.0.0)
 Project-URL: Repository, https://github.com/danielgafni/dagster-polars
 Description-Content-Type: text/markdown
 
 # `dagster-polars`
 
 [Polars](https://github.com/pola-rs/polars) integration library for [Dagster](https://github.com/dagster-io/dagster).
 
 ## Features
- - `PolarsIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
+ - All IOManagers log various metadata about the DataFrame - size, schema, sample, stats, ...
+ - For all IOManagers the `"columns"` input metadata key can be used to select a subset of columns to load
+ - `BasePolarsUPathIOManager` is a base class for IO managers that work with Polars DataFrames. Shouldn't be used directly unless you want to implement your own `IOManager`.
    - returns the correct type (`polars.DataFrame` or `polars.LazyFrame`) based on the type annotation
-   - logs various metadata about the DataFrame - size, schema, sample, stats, ...
-   - the "columns" input metadata value can be used to select a subset of columns
    - inherits all the features of the `UPathIOManager` - works with local and remote filesystems (like S3),
        supports loading multiple partitions (use `dict[str, pl.DataFrame]` type annotation), ...
    - Implemented serialization formats:
      - `PolarsParquetIOManager` - for reading and writing files in Apache Parquet format. Supports reading partitioned Parquet datasets (for example, often produced by Spark).
+ - `BigQueryPolarsIOManager` - for reading and writing data from/to [BigQuery](https://cloud.google.com/bigquery). Supports writing partitioned tables (`"partition_expr"` input metadata key must be specified).
 
 ## Quickstart
 
 ### Installation
 
 ```shell
 pip install dagster-polars
 ```
 
+To use the `BigQueryPolarsIOManager` you need to install the `gcp` extra:
+```shell
+pip install 'dagster-polars[gcp]'
+```
+
+
 ### Usage
 ```python
+import polars as pl
 from dagster import asset, Definitions
 from dagster_polars import PolarsParquetIOManager
-import polars as pl
 
 
 @asset(io_manager_key="polars_parquet_io_manager")
 def upstream() -> pl.DataFrame:
     df: pl.DataFrame = ...
     return df
 
@@ -85,11 +94,11 @@
 
 ### Testing
 ```shell
 poetry run pytest
 ```
 
 ## TODO
-
+ - [ ] Add `PolarsDeltaIOManager`
  - [ ] Data validation like in [dagster-pandas](https://docs.dagster.io/integrations/pandas#validating-pandas-dataframes-with-dagster-types)
  - [ ] Maybe use `DagsterTypeLoader` ?
```

