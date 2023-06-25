# Comparing `tmp/calcipy-1.3.0.tar.gz` & `tmp/calcipy-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calcipy-1.3.0.tar", max compression
+gzip compressed data, was "calcipy-1.4.0.tar", max compression
```

## Comparing `calcipy-1.3.0.tar` & `calcipy-1.4.0.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.3.0/LICENSE
--rw-r--r--   0        0        0      167 2023-06-21 12:44:59.035443 calcipy-1.3.0/calcipy/__init__.py
--rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.3.0/calcipy/can_skip.py
--rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.3.0/calcipy/check_for_stale_packages/__init__.py
--rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.3.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
--rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.3.0/calcipy/cli.py
--rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.3.0/calcipy/code_tag_collector/__init__.py
--rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.3.0/calcipy/code_tag_collector/_collector.py
--rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.3.0/calcipy/dot_dict/__init__.py
--rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.3.0/calcipy/dot_dict/_dot_dict.py
--rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.3.0/calcipy/experiments/__init__.py
--rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.3.0/calcipy/experiments/check_duplicate_test_names.py
--rw-r--r--   0        0        0     3271 2023-02-23 02:19:12.613926 calcipy-1.3.0/calcipy/file_search.py
--rw-r--r--   0        0        0     1942 2023-05-17 11:00:03.480459 calcipy-1.3.0/calcipy/invoke_helpers.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.3.0/calcipy/md_writer/__init__.py
--rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.3.0/calcipy/md_writer/_writer.py
--rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.3.0/calcipy/noxfile/__init__.py
--rw-r--r--   0        0        0     6546 2023-04-22 15:10:18.113523 calcipy-1.3.0/calcipy/noxfile/_noxfile.py
--rw-r--r--   0        0        0     1258 2023-05-17 10:59:02.930491 calcipy-1.3.0/calcipy/scripts.py
--rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.3.0/calcipy/tasks/__init__.py
--rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.3.0/calcipy/tasks/all_tasks.py
--rw-r--r--   0        0        0     1884 2023-05-16 23:59:46.273109 calcipy-1.3.0/calcipy/tasks/cl.py
--rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.3.0/calcipy/tasks/defaults.py
--rw-r--r--   0        0        0     3617 2023-05-16 23:59:46.277097 calcipy-1.3.0/calcipy/tasks/doc.py
--rw-r--r--   0        0        0     3896 2023-05-28 12:34:20.588583 calcipy-1.3.0/calcipy/tasks/lint.py
--rw-r--r--   0        0        0      462 2023-05-16 23:59:46.283536 calcipy-1.3.0/calcipy/tasks/nox.py
--rw-r--r--   0        0        0     1667 2023-05-17 10:56:42.232544 calcipy-1.3.0/calcipy/tasks/pack.py
--rw-r--r--   0        0        0      565 2023-05-16 23:59:46.291723 calcipy-1.3.0/calcipy/tasks/stale.py
--rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.3.0/calcipy/tasks/tags.py
--rw-r--r--   0        0        0     3667 2023-05-16 23:59:46.301475 calcipy-1.3.0/calcipy/tasks/test.py
--rw-r--r--   0        0        0      642 2023-05-16 23:59:46.303934 calcipy-1.3.0/calcipy/tasks/types.py
--rw-r--r--   0        0        0     6651 2023-06-21 12:45:04.355949 calcipy-1.3.0/docs/README.md
--rw-r--r--   0        0        0     6537 2023-06-21 12:44:59.060686 calcipy-1.3.0/pyproject.toml
--rw-r--r--   0        0        0    11265 1970-01-01 00:00:00.000000 calcipy-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-17 12:45:29.997841 calcipy-1.4.0/LICENSE
+-rw-r--r--   0        0        0      167 2023-06-25 19:59:53.761206 calcipy-1.4.0/calcipy/__init__.py
+-rw-r--r--   0        0        0     1241 2023-05-13 10:55:19.213121 calcipy-1.4.0/calcipy/can_skip.py
+-rw-r--r--   0        0        0      175 2023-03-02 02:58:57.029784 calcipy-1.4.0/calcipy/check_for_stale_packages/__init__.py
+-rw-r--r--   0        0        0     8399 2023-06-21 08:48:44.073873 calcipy-1.4.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py
+-rw-r--r--   0        0        0     6436 2023-05-17 11:02:50.475557 calcipy-1.4.0/calcipy/cli.py
+-rw-r--r--   0        0        0      154 2023-03-02 02:58:57.946199 calcipy-1.4.0/calcipy/code_tag_collector/__init__.py
+-rw-r--r--   0        0        0    11270 2023-06-21 12:22:01.579173 calcipy-1.4.0/calcipy/code_tag_collector/_collector.py
+-rw-r--r--   0        0        0      140 2023-03-02 02:58:58.498973 calcipy-1.4.0/calcipy/dot_dict/__init__.py
+-rw-r--r--   0        0        0      803 2023-02-25 23:58:05.004832 calcipy-1.4.0/calcipy/dot_dict/_dot_dict.py
+-rw-r--r--   0        0        0        0 2023-04-05 02:28:27.975837 calcipy-1.4.0/calcipy/experiments/__init__.py
+-rw-r--r--   0        0        0     1988 2023-06-18 22:07:03.089724 calcipy-1.4.0/calcipy/experiments/check_duplicate_test_names.py
+-rw-r--r--   0        0        0     3294 2023-06-21 22:43:42.721881 calcipy-1.4.0/calcipy/file_search.py
+-rw-r--r--   0        0        0     1858 2023-06-25 19:44:08.544986 calcipy-1.4.0/calcipy/invoke_helpers.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:58.973806 calcipy-1.4.0/calcipy/md_writer/__init__.py
+-rw-r--r--   0        0        0     7789 2023-06-21 12:26:00.681287 calcipy-1.4.0/calcipy/md_writer/_writer.py
+-rw-r--r--   0        0        0      162 2023-03-02 02:58:59.584964 calcipy-1.4.0/calcipy/noxfile/__init__.py
+-rw-r--r--   0        0        0     6441 2023-06-25 19:20:04.315707 calcipy-1.4.0/calcipy/noxfile/_noxfile.py
+-rw-r--r--   0        0        0     1418 2023-06-23 11:18:02.014243 calcipy-1.4.0/calcipy/scripts.py
+-rw-r--r--   0        0        0        0 2023-02-21 03:18:10.928974 calcipy-1.4.0/calcipy/tasks/__init__.py
+-rw-r--r--   0        0        0     3488 2023-05-17 11:01:15.749443 calcipy-1.4.0/calcipy/tasks/all_tasks.py
+-rw-r--r--   0        0        0     2026 2023-06-25 19:43:32.341457 calcipy-1.4.0/calcipy/tasks/cl.py
+-rw-r--r--   0        0        0     1169 2023-05-17 10:45:25.212981 calcipy-1.4.0/calcipy/tasks/defaults.py
+-rw-r--r--   0        0        0     3676 2023-06-25 19:58:27.487137 calcipy-1.4.0/calcipy/tasks/doc.py
+-rw-r--r--   0        0        0     1771 2023-06-25 19:43:32.338425 calcipy-1.4.0/calcipy/tasks/executable_utils.py
+-rw-r--r--   0        0        0     4191 2023-06-25 19:43:32.342494 calcipy-1.4.0/calcipy/tasks/lint.py
+-rw-r--r--   0        0        0      487 2023-06-25 19:20:04.874448 calcipy-1.4.0/calcipy/tasks/nox.py
+-rw-r--r--   0        0        0     1703 2023-06-25 19:43:32.341707 calcipy-1.4.0/calcipy/tasks/pack.py
+-rw-r--r--   0        0        0      611 2023-06-25 19:05:50.289154 calcipy-1.4.0/calcipy/tasks/stale.py
+-rw-r--r--   0        0        0     1506 2023-05-16 23:59:46.294332 calcipy-1.4.0/calcipy/tasks/tags.py
+-rw-r--r--   0        0        0     3656 2023-06-25 19:15:31.479851 calcipy-1.4.0/calcipy/tasks/test.py
+-rw-r--r--   0        0        0      772 2023-06-25 19:43:32.341220 calcipy-1.4.0/calcipy/tasks/types.py
+-rw-r--r--   0        0        0     6651 2023-06-25 20:00:00.310899 calcipy-1.4.0/docs/README.md
+-rw-r--r--   0        0        0     6579 2023-06-25 19:59:53.799463 calcipy-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11265 1970-01-01 00:00:00.000000 calcipy-1.4.0/PKG-INFO
```

### Comparing `calcipy-1.3.0/LICENSE` & `calcipy-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/can_skip.py` & `calcipy-1.4.0/calcipy/can_skip.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py` & `calcipy-1.4.0/calcipy/check_for_stale_packages/_check_for_stale_packages.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/cli.py` & `calcipy-1.4.0/calcipy/cli.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/code_tag_collector/_collector.py` & `calcipy-1.4.0/calcipy/code_tag_collector/_collector.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/dot_dict/_dot_dict.py` & `calcipy-1.4.0/calcipy/dot_dict/_dot_dict.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/experiments/check_duplicate_test_names.py` & `calcipy-1.4.0/calcipy/experiments/check_duplicate_test_names.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/file_search.py` & `calcipy-1.4.0/calcipy/file_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,11 +92,11 @@
         path_project: Path to the project directory
         ignore_patterns: glob ignore patterns
 
     Returns:
         Dict[str, List[Path]]: where keys are the suffix (without leading dot) and values the list of paths
 
     """
-    file_lookup = defaultdict(list)
+    file_lookup: Dict[str, List[Path]] = defaultdict(list)
     for path_file in find_project_files(path_project, ignore_patterns or []):
         file_lookup[path_file.suffix.lstrip('.')].append(path_file)
     return dict(file_lookup)
```

### Comparing `calcipy-1.3.0/calcipy/invoke_helpers.py` & `calcipy-1.4.0/calcipy/invoke_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,25 +22,22 @@
     """Returns False on Windows and some CI environments."""
     if platform.system() == 'Windows':
         return False
     return not environ.get('GITHUB_ACTION')
 
 
 @beartype
-def run(ctx: Context, *run_args: Any, **run_kwargs: Any) -> Result:
+def run(ctx: Context, *run_args: Any, **run_kwargs: Any) -> Optional[Result]:
     """Wrap invoke.run to run within the `working_dir`."""
     working_dir = '.'
     with suppress(AttributeError):
         working_dir = ctx.config.gto.working_dir
 
     with ctx.cd(working_dir):
-        res = ctx.run(*run_args, **run_kwargs)
-    if not res:
-        raise NotImplementedError('No response from `ctx.run`')
-    return res
+        return ctx.run(*run_args, **run_kwargs)
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 # Invoke Task Helpers
 
 
 @lru_cache(maxsize=1)
```

### Comparing `calcipy-1.3.0/calcipy/md_writer/_writer.py` & `calcipy-1.4.0/calcipy/md_writer/_writer.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/noxfile/_noxfile.py` & `calcipy-1.4.0/calcipy/noxfile/_noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,17 +50,14 @@
 
 if read_package_name() == 'corallium':
     # 'poetry export' will fail on circular dependencies, so use no instead of nox-poetry
     from nox import session as nox_session
 else:
     from nox_poetry import session as nox_session  # type: ignore[no-redef]
 
-BASE_NOX_COMMAND = 'poetry run nox --error-on-missing-interpreters'
-"""Reused base arguments to nox."""
-
 
 @lru_cache(maxsize=1)
 @beartype
 def _get_pythons() -> List[str]:
     """Get python versions from the `.tool-versions` file."""
     return [str(ver) for ver in get_tool_versions()['python']]
```

### Comparing `calcipy-1.3.0/calcipy/scripts.py` & `calcipy-1.4.0/calcipy/scripts.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,21 @@
 def start_lint() -> None:  # pragma: no cover
     """Run CLI with only the lint namespace."""
     from .tasks import lint
     _start_subset([lint])
 
 
 @beartype
+def start_pack() -> None:  # pragma: no cover
+    """Run CLI with only the pack namespace."""
+    from .tasks import pack
+    _start_subset([pack])
+
+
+@beartype
 def start_tags() -> None:  # pragma: no cover
     """Run CLI with only the tags namespace."""
     from .tasks import tags
     _start_subset([tags])
 
 
 @beartype
```

### Comparing `calcipy-1.3.0/calcipy/tasks/all_tasks.py` & `calcipy-1.4.0/calcipy/tasks/all_tasks.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/tasks/cl.py` & `calcipy-1.4.0/calcipy/tasks/cl.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from beartype import beartype
 from beartype.typing import Literal, Optional
 from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import get_doc_subdir, get_project_path, run
+from .executable_utils import GH_MESSAGE, check_installed, python_dir
 
 SuffixT = Optional[Literal['alpha', 'beta', 'rc']]
 """Prerelease Suffix Type."""
 
 
 @task()
 def write(ctx: Context) -> None:
@@ -24,27 +25,29 @@
     - https://semver.org/
     - https://calver.org/
 
     Returns:
         List[DoitAction]: doit actions
 
     """
-    run(ctx, 'poetry run cz changelog')
+    run(ctx, f'{python_dir()}/cz changelog')
     path_cl = get_project_path() / 'CHANGELOG.md'
     if not path_cl.is_file():
         msg = f'Could not locate the changelog at: {path_cl}'
         raise FileNotFoundError(msg)
     path_cl.replace(get_doc_subdir() / path_cl.name)
 
 
 @beartype
 def bumpz(ctx: Context, *, suffix: SuffixT = None) -> None:
     """Bumps project version based on commits & settings in pyproject.toml."""
+    check_installed(ctx, executable='gh', message=GH_MESSAGE)
+
     opt_cz_args = f' --prerelease={suffix}' if suffix else ''
-    run(ctx, f'poetry run cz bump{opt_cz_args} --annotated-tag --no-verify --gpg-sign')
+    run(ctx, f'{python_dir()}/cz bump{opt_cz_args} --annotated-tag --no-verify --gpg-sign')
 
     run(ctx, 'git push origin --tags --no-verify')
 
     get_last_tag = 'git tag --list --sort=-creatordate | head -n 1'
     opt_gh_args = ' --prerelease' if suffix else ''
     run(ctx, f'gh release create --generate-notes $({get_last_tag}){opt_gh_args}')
```

### Comparing `calcipy-1.3.0/calcipy/tasks/defaults.py` & `calcipy-1.4.0/calcipy/tasks/defaults.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/tasks/doc.py` & `calcipy-1.4.0/calcipy/tasks/doc.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 )
 from invoke.context import Context
 from invoke.exceptions import UnexpectedExit
 
 from ..cli import task
 from ..invoke_helpers import get_doc_subdir, get_project_path, run
 from ..md_writer import write_autoformatted_md_sections
+from .executable_utils import python_dir
 
 
 @beartype
 def _diagram_task(ctx: Context, pdoc_out_path: Path) -> None:
     """Return actions to generate code diagrams in the module documentation directory.
 
     Note: must be run after `document` because pdoc will delete these files
@@ -50,15 +51,15 @@
 
 [Full Size](./classes.svg)
 """
     pkg_name = read_package_name()
     path_diagram = pdoc_out_path / pkg_name / '_code_diagrams.md'
     ensure_dir(path_diagram.parent)
     path_diagram.write_text(diagram_md)
-    run(ctx, f'poetry run pyreverse {pkg_name} --output svg --output-directory {path_diagram.parent}')
+    run(ctx, f'{python_dir()}/pyreverse {pkg_name} --output svg --output-directory {path_diagram.parent}')
 
 
 @beartype
 def get_out_dir() -> Path:
     """Retrieve the mkdocs-specified site directory."""
     mkdocs_config = read_yaml_file(get_project_path() / MKDOCS_CONFIG)
     return Path(mkdocs_config.get('site_dir', 'releases/site'))
@@ -72,15 +73,15 @@
     delete_dir(auto_doc_path)
     _diagram_task(ctx, auto_doc_path)
 
     # Find and trim trailing whitespace
     for path_md in auto_doc_path.rglob('*.md'):
         trim_trailing_whitespace(path_md)
 
-    run(ctx, f'poetry run mkdocs build --site-dir {get_out_dir()}')
+    run(ctx, f'{python_dir()}/mkdocs build --site-dir {get_out_dir()}')
 
 
 @beartype
 def _is_mkdocs_local() -> bool:
     """Check if mkdocs is configured for local output.
 
     See notes on local-link configuration here: https://github.com/timothycrosley/portray/issues/65
@@ -99,21 +100,21 @@
 def watch(ctx: Context) -> None:
     """Serve local documentation for local editing."""
     if _is_mkdocs_local():  # pragma: no cover
         path_doc_index = get_out_dir() / 'index.html'
         open_in_browser(path_doc_index)
     else:  # pragma: no cover
         webbrowser.open('http://localhost:8000')
-        run(ctx, 'poetry run mkdocs serve --dirtyreload')
+        run(ctx, f'{python_dir()}/mkdocs serve --dirtyreload')
 
 
 @task()
 def deploy(ctx: Context) -> None:
     """Deploy docs to the Github `gh-pages` branch."""
     if _is_mkdocs_local():  # pragma: no cover
         raise NotImplementedError('Not yet configured to deploy documentation without "use_directory_urls"')
 
     with suppress(UnexpectedExit):
         run(ctx, 'pre-commit uninstall')  # To prevent pre-commit failures when mkdocs calls push
-    run(ctx, 'poetry run mkdocs gh-deploy --force')
+    run(ctx, f'{python_dir()}/mkdocs gh-deploy --force')
     with suppress(UnexpectedExit):
         run(ctx, 'pre-commit install')  # Restore pre-commit
```

### Comparing `calcipy-1.3.0/calcipy/tasks/lint.py` & `calcipy-1.4.0/calcipy/tasks/lint.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,95 +6,99 @@
 from beartype.typing import Optional
 from corallium.file_helpers import read_package_name
 from corallium.log import logger
 from invoke.context import Context
 
 from ..cli import task
 from ..invoke_helpers import run
+from .executable_utils import PRE_COMMIT_MESSAGE, check_installed, python_dir, python_m
 
 # ==============================================================================
 # Linting
 
 
 @beartype
 def _inner_task(
     ctx: Context,
     *,
-    cli_args: str,
-    command: str = 'python -m ruff check',
+    command: str,
+    cli_args: str = '',
+    run_as_module: bool = True,
     target: Optional[str] = None,
 ) -> None:
     """Shared task logic."""
     file_args = []
     with suppress(AttributeError):
         file_args = ctx.config.gto.file_args
     if file_args:
         target = ' '.join([str(_a) for _a in file_args])
     elif target is None:
         target = f'./{read_package_name()} ./tests'
-    run(ctx, f'poetry run {command} {target}{cli_args}')
+
+    cmd = f'{python_m()} {command}' if run_as_module else f'{python_dir()}/{command}'
+    run(ctx, f'{cmd} {target} {cli_args}'.strip())
 
 
 @task(default=True)
 def check(ctx: Context) -> None:
     """Run ruff as check-only."""
-    _inner_task(ctx, cli_args='')
+    _inner_task(ctx, command='ruff check')
 
 
 @task()
 def autopep8(ctx: Context) -> None:
     """Run autopep8.
 
     FYI: This is temporary until ruff implements white space rules
     https://github.com/charliermarsh/ruff/issues/970
 
     """
-    cli_args = ' --aggressive --recursive --in-place --max-line-length=120'
-    _inner_task(ctx, cli_args=cli_args, command='python -m autopep8')
+    cli_args = '--aggressive --recursive --in-place --max-line-length=120'
+    _inner_task(ctx, command='autopep8', cli_args=cli_args)
 
 
 @task(pre=[autopep8])
 def fix(ctx: Context) -> None:
     """Run ruff and apply fixes."""
-    _inner_task(ctx, cli_args=' --fix')
+    _inner_task(ctx, command='ruff check', cli_args='--fix')
 
 
 @task()
 def watch(ctx: Context) -> None:
     """Run ruff as check-only."""
-    _inner_task(ctx, cli_args=' --watch --show-source')
+    _inner_task(ctx, command='ruff check', cli_args='--watch --show-source')
 
 
 @task()
 def flake8(ctx: Context) -> None:
     """Run flake8."""
-    _inner_task(ctx, cli_args='', command='python -m flake8')
+    _inner_task(ctx, command='flake8', run_as_module=False)
 
 
 @task(
     help={
         'report': 'if provided, show the pylint summary report',
     },
 )
 def pylint(ctx: Context, *, report: bool = False) -> None:
     """Run pylint."""
-    cli_args = ' --report=y' if report else ''
-    _inner_task(ctx, cli_args=cli_args, command='python -m pylint')
+    cli_args = '--report=y' if report else ''
+    _inner_task(ctx, command='pylint', cli_args=cli_args)
 
 
 # ==============================================================================
 # Security
 
 
 @task()
 def security(ctx: Context) -> None:
     """Attempt to identify possible security vulnerabilities."""
     logger.text('Note: Selectively override bandit with "# nosec"', is_header=True)
     pkg_name = read_package_name()
-    run(ctx, f'poetry run bandit --recursive {pkg_name} -s B101')
+    run(ctx, f'{python_dir()}/bandit --recursive {pkg_name} -s B101')
 
     # See additional semgrep rules at:
     #   https://semgrep.dev/explore
     #   https://github.com/returntocorp/semgrep-rules/tree/develop/python
     #   https://awesomeopensource.com/project/returntocorp/semgrep-rules?categorypage=45
     semgrep_configs = ' '.join([  # noqa: FLY002
         '--config=p/ci',
@@ -106,28 +110,30 @@
         '--config=r/generic',
         '--config=r/json',
         '--config=r/python',
         '--config=r/terraform',
         '--config=r/yaml',
     ])
     logger.text('Note: Selectively override semgrep with "# nosem"', is_header=True)
-    run(ctx, f'poetry run semgrep ci --autofix {semgrep_configs}')
+    run(ctx, f'{python_dir()}/semgrep ci --autofix {semgrep_configs}')
 
 
 # ==============================================================================
 # Pre-Commit
 
 
 @task(
     help={
         'no_update': 'Skip updating the pre-commit hooks',
     },
 )
 def pre_commit(ctx: Context, *, no_update: bool = False) -> None:
     """Run pre-commit."""
+    check_installed(ctx, executable='pre-commit', message=PRE_COMMIT_MESSAGE)
+
     run(ctx, 'pre-commit install')
     if not no_update:
         run(ctx, 'pre-commit autoupdate')
 
     all_hook_stages = [
         'commit', 'merge-commit', 'push', 'prepare-commit-msg', 'commit-msg', 'post-checkout',
         'post-commit', 'post-merge', 'post-rewrite', 'manual',
```

### Comparing `calcipy-1.3.0/calcipy/tasks/pack.py` & `calcipy-1.4.0/calcipy/tasks/pack.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from corallium.file_helpers import LOCK, PROJECT_TOML
 from corallium.log import logger
 from invoke.context import Context
 
 from .. import can_skip  # Required for mocking can_skip.can_skip
 from ..cli import task
 from ..invoke_helpers import run
-from ..noxfile._noxfile import BASE_NOX_COMMAND
+from .executable_utils import python_dir
 
 
 @task()
 def install_extras(ctx: Context) -> None:
     """Run poetry install with all extras."""
     poetry_config = file_helpers.read_pyproject()['tool']['poetry']
     extras = (poetry_config.get('extras') or {}).keys()
@@ -31,23 +31,23 @@
 @task(
     help={
         'to_test_pypi': 'Publish to the TestPyPi repository',
     },
 )
 def publish(ctx: Context, *, to_test_pypi: bool = False) -> None:
     """Build the distributed format(s) and publish."""
-    run(ctx, f'{BASE_NOX_COMMAND} --session build_dist build_check')
+    run(ctx, f'{python_dir()}/nox --error-on-missing-interpreters --session build_dist build_check')
 
     cmd = 'poetry publish'
     if to_test_pypi:
         cmd += ' --repository testpypi'
     run(ctx, cmd)
 
 
 @task()
 def check_licenses(ctx: Context) -> None:
     """Check licenses for compatibility with `licensecheck`."""
     res = run(ctx, 'which licensecheck', warn=True, hide=True)
-    if res.exited == 1:
+    if not res or res.exited == 1:
         logger.warning('`licensecheck` not found. installing with pipx')
         run(ctx, 'pipx install licensecheck')
     run(ctx, 'licensecheck')
```

### Comparing `calcipy-1.3.0/calcipy/tasks/stale.py` & `calcipy-1.4.0/calcipy/tasks/stale.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Stale Packages CLI."""
 
 from invoke.context import Context
 
 from ..check_for_stale_packages import check_for_stale_packages as cfsp
 from ..cli import task
 from ..invoke_helpers import run
+from .executable_utils import python_dir
 
 
 @task(
     default=True,
     help={
         'stale_months': 'Cutoff in months for when a package may be stale enough to be a risk',
     },
 )
 def check_for_stale_packages(ctx: Context, *, stale_months: int = 48) -> None:
     """Identify stale dependencies."""
     cfsp(stale_months=stale_months)
-    run(ctx, 'poetry run pip-check --cmd="poetry run pip" --hide-unchanged')
+    run(ctx, f'{python_dir()}/pip-check --cmd="poetry run pip" --hide-unchanged')
```

### Comparing `calcipy-1.3.0/calcipy/tasks/tags.py` & `calcipy-1.4.0/calcipy/tasks/tags.py`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/calcipy/tasks/test.py` & `calcipy-1.4.0/calcipy/tasks/test.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 from corallium.file_helpers import open_in_browser, read_package_name
 from invoke.context import Context
 
 from ..cli import task
 from ..experiments import check_duplicate_test_names
 from ..invoke_helpers import run
 from .defaults import from_ctx
+from .executable_utils import python_dir
 
 _STEPWISE_ARGS = ' --failed-first --new-first --exitfirst -vv --no-cov'
 
 
 @beartype
 def _inner_task(
     ctx: Context,
     *,
-    cli_args: str,
+    command: str = 'pytest',
+    cli_args: str = '',
     keyword: str = '',
     marker: str = '',
     min_cover: int = 0,
-    command: str = 'python -m pytest',
 ) -> None:
     """Shared task logic."""
     if keyword:
         cli_args += f' -k "{keyword}"'
     if marker:
         cli_args += f' -m "{marker}"'
     if fail_under := min_cover or int(from_ctx(ctx, 'test', 'min_cover')):
         cli_args += f' --cov-fail-under={fail_under}'
-    run(ctx, f'poetry run {command} ./tests{cli_args}')
+    run(ctx, f'{python_dir()}/{command} ./tests{cli_args}')
 
 
 @task()
 def check(_ctx: Context) -> None:
     """Run pytest checks, such as identifying ."""
     if duplciates := check_duplicate_test_names.run(Path('tests')):
         raise RuntimeError(f'Duplicate test names found ({duplciates}). See above for details.')  # noqa: EM102
@@ -93,16 +94,16 @@
     pkg_name = read_package_name()
     _inner_task(ctx, cli_args='', min_cover=min_cover,
                 command=f'coverage run --branch --source={pkg_name} --module pytest')
 
     cov_dir = Path(out_dir or from_ctx(ctx, 'test', 'out_dir'))
     cov_dir.mkdir(exist_ok=True, parents=True)
     print('')  # noqa: T201
-    for cmd in (
-        'poetry run python -m coverage report --show-missing',  # Write to STDOUT
-        f'poetry run python -m coverage html --directory={cov_dir}',  # Write to HTML
-        'poetry run python -m coverage json',  # Create coverage.json file for "_handle_coverage"
+    for cli_args in (
+        'report --show-missing',  # Write to STDOUT
+        f'html --directory={cov_dir}',  # Write to HTML
+        'json',  # Create coverage.json file for "_handle_coverage"
     ):
-        run(ctx, cmd)
+        run(ctx, f'{python_dir()}/coverage {cli_args}')
 
     if view:  # pragma: no cover
         open_in_browser(cov_dir / 'index.html')
```

### Comparing `calcipy-1.3.0/docs/README.md` & `calcipy-1.4.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `calcipy-1.3.0/pyproject.toml` & `calcipy-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.commitizen]
-version = "1.3.0"
+version = "1.4.0"
 version_files = ["calcipy/__init__.py:^__version", "pyproject.toml:^version"]
 
 [tool.poetry]
 authors = ["Kyle King <dev.act.kyle@gmail.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
@@ -26,20 +26,20 @@
 include = ["LICENSE"]
 keywords = ["nox", "python-poetry"]
 license = "MIT"
 maintainers = []
 name = "calcipy"
 readme = "docs/README.md"
 repository = "https://github.com/kyleking/calcipy"
-version = "1.3.0"
+version = "1.4.0"
 
 [tool.poetry.dependencies]
 python = "^3.8.12"
 arrow = {optional = true, version = ">=1.2.3"} # tags
-autopep8 = {optional = true, version = ">=2.0.1"} # flake8
+autopep8 = {optional = true, version = ">=2.0.1"} # lint
 bandit = {optional = true, version = ">=1.7.4"} # lint
 beartype = ">=0.12.0"
 bidict = {optional = true, version = ">=0.22.1"} # stale
 commitizen = {optional = true, version = ">=2.42.0"} # doc
 corallium = ">=0.2.2"
 dlint = {optional = true, version = ">=0.14.0"} # flake8
 flake8 = {optional = true, version = ">=6.0.0"} # flake8
@@ -166,17 +166,18 @@
 pytest-recording = ">=0.12.0"
 pytest-subprocess = ">=1.4.1"
 types-pyyaml = ">=6.0.12.6"
 types-setuptools = ">=67.3.0.1"
 
 [tool.poetry.scripts]
 calcipy = "calcipy.scripts:start"
-calcipy_lint = "calcipy.scripts:start_lint"
-calcipy_tags = "calcipy.scripts:start_tags"
-calcipy_types = "calcipy.scripts:start_types"
+calcipy-lint = "calcipy.scripts:start_lint"
+calcipy-pack = "calcipy.scripts:start_pack"
+calcipy-tags = "calcipy.scripts:start_tags"
+calcipy-types = "calcipy.scripts:start_types"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/kyleking/calcipy/issues"
 "Changelog" = "https://github.com/kyleking/calcipy/blob/main/docs/docs/CHANGELOG.md"
 
 [tool.pyright]
 include = ["calcipy"]
```

### Comparing `calcipy-1.3.0/PKG-INFO` & `calcipy-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcipy
-Version: 1.3.0
+Version: 1.4.0
 Summary: Python package to simplify development
 Home-page: https://github.com/kyleking/calcipy
 License: MIT
 Keywords: nox,python-poetry
 Author: Kyle King
 Author-email: dev.act.kyle@gmail.com
 Requires-Python: >=3.8.12,<4.0.0
```

