# Comparing `tmp/delfino_core-5.1.0.tar.gz` & `tmp/delfino_core-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delfino_core-5.1.0.tar", max compression
+gzip compressed data, was "delfino_core-5.1.1.tar", max compression
```

## Comparing `delfino_core-5.1.0.tar` & `delfino_core-5.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1078 2023-06-25 12:57:57.859073 delfino_core-5.1.0/LICENSE.md
--rw-r--r--   0        0        0     5291 2023-06-25 12:57:57.859073 delfino_core-5.1.0/README.md
--rw-r--r--   0        0        0     4291 2023-06-25 12:57:57.859073 delfino_core-5.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/__init__.py
--rw-r--r--   0        0        0      293 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/backports.py
--rw-r--r--   0        0        0        0 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/__init__.py
--rw-r--r--   0        0        0     9055 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/dependencies_update.py
--rw-r--r--   0        0        0     4253 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/format.py
--rw-r--r--   0        0        0     6681 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/lint.py
--rw-r--r--   0        0        0     3471 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/switch_python_version.py
--rw-r--r--   0        0        0     7883 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/test.py
--rw-r--r--   0        0        0     3392 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/typecheck.py
--rw-r--r--   0        0        0      748 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/commands/verify_all.py
--rw-r--r--   0        0        0      904 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/config.py
--rw-r--r--   0        0        0     1720 2023-06-25 12:57:57.859073 delfino_core-5.1.0/src/delfino_core/utils.py
--rw-r--r--   0        0        0     7551 1970-01-01 00:00:00.000000 delfino_core-5.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-06-25 13:19:48.163020 delfino_core-5.1.1/LICENSE.md
+-rw-r--r--   0        0        0     5291 2023-06-25 13:19:48.163020 delfino_core-5.1.1/README.md
+-rw-r--r--   0        0        0     4246 2023-06-25 13:19:48.163020 delfino_core-5.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/__init__.py
+-rw-r--r--   0        0        0      293 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/backports.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/__init__.py
+-rw-r--r--   0        0        0     9018 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/dependencies_update.py
+-rw-r--r--   0        0        0     4416 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/format.py
+-rw-r--r--   0        0        0     6812 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/lint.py
+-rw-r--r--   0        0        0     3471 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/switch_python_version.py
+-rw-r--r--   0        0        0     7858 2023-06-25 13:19:48.163020 delfino_core-5.1.1/src/delfino_core/commands/test.py
+-rw-r--r--   0        0        0     3446 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/commands/typecheck.py
+-rw-r--r--   0        0        0      748 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/commands/verify_all.py
+-rw-r--r--   0        0        0      904 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/config.py
+-rw-r--r--   0        0        0     1720 2023-06-25 13:19:48.167020 delfino_core-5.1.1/src/delfino_core/utils.py
+-rw-r--r--   0        0        0     7501 1970-01-01 00:00:00.000000 delfino_core-5.1.1/PKG-INFO
```

### Comparing `delfino_core-5.1.0/LICENSE.md` & `delfino_core-5.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/README.md` & `delfino_core-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/pyproject.toml` & `delfino_core-5.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name="delfino-core"
-version="5.1.0"
+version="5.1.1"
 authors = ["Radek Lát <radek.lat@gmail.com>"]
 description="Delfino core plugin"
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/radeklat/delfino-core"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/dependencies_update.py` & `delfino_core-5.1.1/src/delfino_core/commands/dependencies_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,16 +74,16 @@
                 if ask("Do you want to open a new pull request now in a web browser?"):
                     webbrowser.open(url)
                 else:
                     secho(f"\nOpen a new pull request by visiting:\n\n\t{url}\n", fg="green")
 
     def _link_to_open_a_pull_request(self) -> Optional[str]:
         url = self._repo.remote().url
-        match = re.match("git@github.com:(.*)\\.git", url)
-        if not match:
+
+        if not (match := re.match("git@github.com:(.*)\\.git", url)):
             match = re.match("https://github.com/(.*)\\.git", url)
 
         return f"https://github.com/{match.group(1)}/pull/new/{self._repo.active_branch}" if match else None
 
     def _read_dependency_file(self) -> str:
         with open(self._FILENAME, encoding="utf-8") as file:
             return file.read()
@@ -175,16 +175,15 @@
         result = _run("pipenv update --outdated")
 
         pipfile = self._read_dependency_file()
 
         available_updates = []
 
         for line in result.stdout.decode().split(os.linesep) + result.stderr.decode().split(os.linesep):
-            match = re.match(self._SKIP_PATTERN, line) or re.match(self._OUTDATED_PATTEN, line)
-            if not match:
+            if not (match := re.match(self._SKIP_PATTERN, line) or re.match(self._OUTDATED_PATTEN, line)):
                 continue
 
             package = match.group("package")
             installed = match.group("installed").lstrip(self._VERSION_CONSTRAINT_CHARS)
             available = match.group("available").lstrip(self._VERSION_CONSTRAINT_CHARS)
 
             # Keep only packages defined in Pipfile with a different version available
@@ -203,17 +202,16 @@
     _FILENAME = "pyproject.toml"
 
     def print_outdated_packages_and_lock_if_changed(self) -> bool:
         secho("Updating packages based on version pinning. This will take a while ...", fg="yellow")
         _run("poetry update")
 
         secho("Checking outdated packages. This will take a while ...", fg="yellow")
-        result = _run("poetry show --outdated --why --ansi")
 
-        if not result.stdout:
+        if not (result := _run("poetry show --outdated --why --ansi")).stdout:
             return False
 
         pyproject_toml = self._read_dependency_file()
 
         self._show_edit_prompt_and_wait(available_updates=result.stdout.decode())
 
         return self._read_dependency_file() != pyproject_toml
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/format.py` & `delfino_core-5.1.1/src/delfino_core/commands/format.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,22 +9,30 @@
 from delfino.terminal_output import print_header, run_command_example
 from delfino.validation import assert_pip_package_installed
 from packaging.specifiers import SpecifierSet
 
 from delfino_core.config import CorePluginConfig, pass_plugin_app_context
 
 
-def _check_result(app_context: AppContext[CorePluginConfig], result: CompletedProcess, check: bool, msg: str):
+def _check_result(
+    app_context: AppContext[CorePluginConfig],
+    result: CompletedProcess,
+    check: bool,
+    msg: str,
+):
     if result.returncode == 1 and check:
         msg_lines = [
             f"{msg} before commit. Try following:",
             f" * Run formatter manually with `{run_command_example(run_format, app_context)}` before committing code.",
         ]
         if not app_context.plugin_config.disable_pre_commit:
-            msg_lines.insert(1, " * Enable pre-commit hook by running `pre-commit install` in the repository.")
+            msg_lines.insert(
+                1,
+                " * Enable pre-commit hook by running `pre-commit install` in the repository.",
+            )
 
         click.secho(
             "\n".join(msg_lines),
             fg="red",
             err=True,
         )
         raise click.Abort()
@@ -58,60 +66,79 @@
 
 
 @click.command("format")
 @click.option("--check", is_flag=True, help="Only check formatting, don't reformat the code.")
 @click.option("--quiet", is_flag=True, help="Don't show progress. Only errors.")
 @files_folders_option
 @pass_plugin_app_context
-def run_format(app_context: AppContext[CorePluginConfig], files_folders: Tuple[Path, ...], check: bool, quiet: bool):
+def run_format(
+    app_context: AppContext[CorePluginConfig],
+    files_folders: Tuple[Path, ...],
+    check: bool,
+    quiet: bool,
+):
     """Runs black code formatter and isort on source code."""
     plugin_config = app_context.plugin_config
 
     assert_pip_package_installed("isort")
     assert_pip_package_installed("black")
     assert_pip_package_installed("pyupgrade")
 
     if not plugin_config.disable_pre_commit:
         assert_pip_package_installed("pre-commit")
         # ensure pre-commit is installed
         run("pre-commit install", stdout=PIPE, on_error=OnError.EXIT)
 
     if not files_folders:
-        files_folders = (plugin_config.sources_directory, plugin_config.tests_directory)
-        if app_context.pyproject_toml.tool.delfino.local_commands_directory.exists():
-            files_folders += (app_context.pyproject_toml.tool.delfino.local_commands_directory,)
+        files_folders = (
+            plugin_config.sources_directory,
+            plugin_config.tests_directory,
+            *[folder for folder in app_context.pyproject_toml.tool.delfino.local_command_folders if folder.exists()],
+        )
 
     python_version = app_context.pyproject_toml.tool.poetry.dependencies.get("python", "3")
     # see `pypgrade -h` for range of supported versions
     min_python_version = _find_min_minor_version(python_version, 3, 6, 11)
     flags = [f"--py3{min_python_version}-plus"]
     if not check:
         flags.append("--exit-zero-even-if-changed")
 
-    print_header(f"Upgrading code to Python 3{'.' + min_python_version if min_python_version else ''}", icon="⬆️")
+    print_header(
+        f"Upgrading code to Python 3{'.' + min_python_version if min_python_version else ''}",
+        icon="⬆️",
+    )
 
     _check_result(
         app_context,
-        run(["pyupgrade", *_all_python_files(files_folders), *flags], on_error=OnError.PASS),
+        run(
+            ["pyupgrade", *_all_python_files(files_folders), *flags],
+            on_error=OnError.PASS,
+        ),
         check,
         "Code was not formatted",
     )
 
     flags = []
 
     if check:
         flags.append("--check")
 
     print_header("Sorting imports", icon="ℹ")
 
     _check_result(
-        app_context, run(["isort", *files_folders, *flags], on_error=OnError.PASS), check, "Import were not sorted"
+        app_context,
+        run(["isort", *files_folders, *flags], on_error=OnError.PASS),
+        check,
+        "Import were not sorted",
     )
 
     print_header("Formatting code", icon="🖤")
 
     if quiet:
         flags.append("--quiet")
 
     _check_result(
-        app_context, run(["black", *files_folders, *flags], on_error=OnError.PASS), check, "Code was not formatted"
+        app_context,
+        run(["black", *files_folders, *flags], on_error=OnError.PASS),
+        check,
+        "Code was not formatted",
     )
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/lint.py` & `delfino_core-5.1.1/src/delfino_core/commands/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 from delfino_core.utils import execute_commands_group
 
 
 @click.command()
 @pass_args
 @files_folders_option
 @pass_plugin_app_context
-def lint_pydocstyle(app_context: AppContext[CorePluginConfig], passed_args: Tuple[str, ...], files_folders: Tuple[str]):
+def lint_pydocstyle(
+    app_context: AppContext[CorePluginConfig],
+    passed_args: Tuple[str, ...],
+    files_folders: Tuple[str],
+):
     """Run docstring linting on source code.
 
     Docstring linting is done via pydocstyle. The pydocstyle config can be found in the
     `pyproject.toml` file under `[tool.pydocstyle]`. This ensures compliance with PEP 257,
     with a few exceptions. Note that pylint also carries out additional documentation
     style checks.
     """
@@ -47,15 +51,17 @@
 
 
 @click.command()
 @pass_args
 @files_folders_option
 @pass_plugin_app_context
 def lint_pycodestyle(
-    app_context: AppContext[CorePluginConfig], passed_args: Tuple[str, ...], files_folders: Tuple[str]
+    app_context: AppContext[CorePluginConfig],
+    passed_args: Tuple[str, ...],
+    files_folders: Tuple[str],
 ):
     """Run PEP8 checking on code.
 
     PEP8 checking is done via pycodestyle.
 
     Why pycodestyle and pylint? So far, pylint does not check against every convention in PEP8. As pylint's
     functionality grows, we should move all PEP8 checking to pylint and remove pycodestyle.
@@ -100,38 +106,44 @@
     checked_dirs: List[Path],
     pylintrc_folder: Path,
     passed_args: Tuple[str, ...],
 ):
     print_header(", ".join(map(str, checked_dirs)), level=3)
 
     run(
-        ["pylint", "-j", str(cpu_count()), "--rcfile", pylintrc_folder / ".pylintrc", *passed_args, *checked_dirs],
+        [
+            "pylint",
+            "-j",
+            str(cpu_count()),
+            "--rcfile",
+            pylintrc_folder / ".pylintrc",
+            *passed_args,
+            *checked_dirs,
+        ],
         stdout=PIPE,
         on_error=OnError.ABORT,
         env_update_path={"PYTHONPATH": sources_dir},
     )
 
     print_no_issues_found()
 
 
 @lru_cache(maxsize=1)
 def cpu_count():
     if getenv("CI", ""):
-        cpu_shares = Path("/sys/fs/cgroup/cpu/cpu.shares")
-        if cpu_shares.is_file():
+        if (cpu_shares := Path("/sys/fs/cgroup/cpu/cpu.shares")).is_file():
             return int(cpu_shares.read_text(encoding="utf-8").strip()) // 1024
 
     log = logging.getLogger("cpu_count")
     fallback_msg = "Number of CPUs could not be determined. Falling back to 1."
 
     if pip_package_installed("psutil"):
         import psutil  # pylint: disable=import-outside-toplevel
 
-        count = psutil.cpu_count(logical=False)
-        if not count:
+        if not (count := psutil.cpu_count(logical=False)):
             log.warning(fallback_msg)
             return 1
         return count
 
     log.warning(f"`psutil` is not installed. {fallback_msg}")
     return 1
 
@@ -140,30 +152,35 @@
     app_context: AppContext[CorePluginConfig],
     files_folders: Optional[Tuple[str]] = None,
     include_tests: bool = True,
     include_commands: bool = True,
 ) -> List[Path]:
     if files_folders:
         return [Path(path) for path in files_folders]
-    local_commands_directory = app_context.pyproject_toml.tool.delfino.local_commands_directory
     plugin_config = app_context.plugin_config
     target_paths: List[Path] = [plugin_config.sources_directory]
 
     if include_tests and plugin_config.tests_directory.exists():
         target_paths.append(plugin_config.tests_directory)
-    if include_commands and local_commands_directory.exists():
-        target_paths.append(local_commands_directory)
+    if include_commands:
+        target_paths.extend(
+            folder for folder in app_context.pyproject_toml.tool.delfino.local_command_folders if folder.exists()
+        )
     return target_paths
 
 
 @click.command()
 @files_folders_option
 @pass_args
 @pass_plugin_app_context
-def lint_pylint(app_context: AppContext[CorePluginConfig], passed_args: Tuple[str, ...], files_folders: Tuple[str]):
+def lint_pylint(
+    app_context: AppContext[CorePluginConfig],
+    passed_args: Tuple[str, ...],
+    files_folders: Tuple[str],
+):
     """Run pylint on code.
 
     The bulk of our code conventions are enforced via pylint. The pylint config can be
     found in the `.pylintrc` file.
     """
     assert_pip_package_installed("pylint")
 
@@ -174,15 +191,20 @@
         if plugin_config.tests_directory.exists() and path_is_relative_to(path, plugin_config.tests_directory):
             return plugin_config.tests_directory
         return app_context.project_root
 
     target_paths = build_target_paths(app_context, files_folders)
     grouped_paths = groupby(target_paths, get_pylintrc_folder)
     for pylintrc_folder, paths in grouped_paths:
-        run_pylint(app_context.plugin_config.sources_directory, list(paths), pylintrc_folder, passed_args)
+        run_pylint(
+            app_context.plugin_config.sources_directory,
+            list(paths),
+            pylintrc_folder,
+            passed_args,
+        )
 
 
 @click.command(help="Runs all linting commands. Configured by the ``lint_commands`` setting.")
 @files_folders_option
 @pass_plugin_app_context
 @click.pass_context
 def lint(
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/switch_python_version.py` & `delfino_core-5.1.1/src/delfino_core/commands/switch_python_version.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/test.py` & `delfino_core-5.1.1/src/delfino_core/commands/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,29 +100,27 @@
 
 
 def _get_total_coverage(coverage_dat: Path) -> str:
     """Return coverage percentage, as captured in coverage dat file; e.g., returns "100%"."""
     output = run(
         "coverage report", stdout=PIPE, env_update={"COVERAGE_FILE": coverage_dat}, on_error=OnError.EXIT
     ).stdout.decode()
-    match = re.search(r"TOTAL.*?([\d.]+%)", output)
-    if match is None:
+
+    if (match := re.search(r"TOTAL.*?([\d.]+%)", output)) is None:
         raise RuntimeError(f"Regex failed on output: {output}")
     return match.group(1)
 
 
 def _combined_coverage_reports(reports_directory: Path, test_types: List[str]) -> Path:
     coverage_dat_combined = reports_directory / "coverage.dat"
 
     coverage_files = []  # we'll make a copy because `combine` will erase them
 
     for test_type in test_types:
-        coverage_dat = reports_directory / f"coverage-{test_type}.dat"
-
-        if not coverage_dat.exists():
+        if not (coverage_dat := reports_directory / f"coverage-{test_type}.dat").exists():
             click.secho(
                 f"Could not find coverage dat file for {test_type} tests: {coverage_dat}",
                 fg="yellow",
             )
         else:
             print(f"{test_type.title()} test coverage: {_get_total_coverage(coverage_dat)}")
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/typecheck.py` & `delfino_core-5.1.1/src/delfino_core/commands/typecheck.py`

 * *Files 15% similar despite different names*

```diff
@@ -46,15 +46,19 @@
 
     args.extend(paths)
 
     if summary_only:
         args.extend(["|", "tail", "-n", "1"])
 
     if print_second_level_headers:
-        print_header(f"{'Strict' if strict else 'Optional'} types", level=2, icon="⚠️" if strict else "ℹ️")
+        print_header(
+            f"{'Strict' if strict else 'Optional'} types",
+            level=2,
+            icon="⚠️" if strict else "ℹ️",
+        )
 
     run(args, env_update_path={"MYPYPATH": mypypath}, on_error=OnError.ABORT)
 
 
 def is_path_relative_to_paths(path: Path, paths: List[Path]) -> bool:
     for _path in paths:
         try:
@@ -62,15 +66,19 @@
             return True
         except ValueError:
             continue
     return False
 
 
 @click.command()
-@click.option("--summary-only", is_flag=True, help="Suppress error messages and show only summary error count.")
+@click.option(
+    "--summary-only",
+    is_flag=True,
+    help="Suppress error messages and show only summary error count.",
+)
 @files_folders_option
 @pass_args
 @pass_plugin_app_context
 def typecheck(
     app_context: AppContext[CorePluginConfig],
     passed_args: Tuple[str, ...],
     summary_only: bool,
@@ -87,19 +95,23 @@
     plugin_config = app_context.plugin_config
     ensure_reports_dir(plugin_config)
 
     if files_folders:
         target_paths = [Path(path) for path in files_folders]
     else:
         target_paths = [plugin_config.sources_directory, plugin_config.tests_directory]
-        if app_context.pyproject_toml.tool.delfino.local_commands_directory.exists():
-            target_paths.append(app_context.pyproject_toml.tool.delfino.local_commands_directory)
+        target_paths.extend(
+            folder for folder in app_context.pyproject_toml.tool.delfino.local_command_folders if folder.exists()
+        )
 
     strict_paths = plugin_config.typecheck.strict_directories
-    grouped_paths = groupby(target_paths, lambda current_path: is_path_relative_to_paths(current_path, strict_paths))
+    grouped_paths = groupby(
+        target_paths,
+        lambda current_path: is_path_relative_to_paths(current_path, strict_paths),
+    )
 
     for force_typing, group in grouped_paths:
         report_filepath = (
             plugin_config.reports_directory / "typecheck" / f"junit-{'strict' if force_typing else 'nonstrict'}.xml"
         )
         _run_typecheck(
             list(group),
```

### Comparing `delfino_core-5.1.0/src/delfino_core/commands/verify_all.py` & `delfino_core-5.1.1/src/delfino_core/commands/verify_all.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/src/delfino_core/config.py` & `delfino_core-5.1.1/src/delfino_core/config.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/src/delfino_core/utils.py` & `delfino_core-5.1.1/src/delfino_core/utils.py`

 * *Files identical despite different names*

### Comparing `delfino_core-5.1.0/PKG-INFO` & `delfino_core-5.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delfino-core
-Version: 5.1.0
+Version: 5.1.1
 Summary: Delfino core plugin
 Home-page: https://github.com/radeklat/delfino-core
 License: MIT
 Author: Radek Lát
 Author-email: radek.lat@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -14,15 +14,14 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Provides-Extra: all
 Provides-Extra: dependencies-update
 Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,37 +1,36 @@
-Metadata-Version: 2.1 Name: delfino-core Version: 5.1.0 Summary: Delfino core
+Metadata-Version: 2.1 Name: delfino-core Version: 5.1.1 Summary: Delfino core
 plugin Home-page: https://github.com/radeklat/delfino-core License: MIT Author:
 Radek LÃ¡t Author-email: radek.lat@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Topic :: Software
-Development Classifier: Topic :: Utilities Provides-Extra: all Provides-Extra:
-dependencies-update Provides-Extra: format Provides-Extra: lint Provides-Extra:
-test Provides-Extra: typecheck Provides-Extra: verify-all Requires-Dist: black
-; extra == "all" or extra == "verify-all" or extra == "format" Requires-Dist:
-coverage ; extra == "all" or extra == "verify-all" or extra == "test" Requires-
-Dist: delfino (>=0.29.0) Requires-Dist: gitpython ; extra == "all" or extra ==
-"dependencies-update" Requires-Dist: isort ; extra == "all" or extra ==
-"verify-all" or extra == "format" Requires-Dist: mypy ; extra == "all" or extra
-== "verify-all" or extra == "typecheck" Requires-Dist: pre-commit ; extra ==
-"all" or extra == "verify-all" or extra == "format" Requires-Dist: psutil ;
-extra == "all" or extra == "verify-all" or extra == "lint" Requires-Dist:
-pycodestyle ; extra == "all" or extra == "verify-all" or extra == "lint"
-Requires-Dist: pydocstyle ; extra == "all" or extra == "verify-all" or extra ==
-"lint" Requires-Dist: pylint ; extra == "all" or extra == "verify-all" or extra
-== "lint" Requires-Dist: pytest ; extra == "all" or extra == "verify-all" or
-extra == "test" Requires-Dist: pytest-cov ; extra == "all" or extra == "verify-
-all" or extra == "test" Requires-Dist: pyupgrade ; extra == "all" or extra ==
-"verify-all" or extra == "format" Requires-Dist: shellingham Description-
-Content-Type: text/markdown
+Classifier: Topic :: Software Development Classifier: Topic :: Utilities
+Provides-Extra: all Provides-Extra: dependencies-update Provides-Extra: format
+Provides-Extra: lint Provides-Extra: test Provides-Extra: typecheck Provides-
+Extra: verify-all Requires-Dist: black ; extra == "all" or extra == "verify-
+all" or extra == "format" Requires-Dist: coverage ; extra == "all" or extra ==
+"verify-all" or extra == "test" Requires-Dist: delfino (>=0.29.0) Requires-
+Dist: gitpython ; extra == "all" or extra == "dependencies-update" Requires-
+Dist: isort ; extra == "all" or extra == "verify-all" or extra == "format"
+Requires-Dist: mypy ; extra == "all" or extra == "verify-all" or extra ==
+"typecheck" Requires-Dist: pre-commit ; extra == "all" or extra == "verify-all"
+or extra == "format" Requires-Dist: psutil ; extra == "all" or extra ==
+"verify-all" or extra == "lint" Requires-Dist: pycodestyle ; extra == "all" or
+extra == "verify-all" or extra == "lint" Requires-Dist: pydocstyle ; extra ==
+"all" or extra == "verify-all" or extra == "lint" Requires-Dist: pylint ; extra
+== "all" or extra == "verify-all" or extra == "lint" Requires-Dist: pytest ;
+extra == "all" or extra == "verify-all" or extra == "test" Requires-Dist:
+pytest-cov ; extra == "all" or extra == "verify-all" or extra == "test"
+Requires-Dist: pyupgrade ; extra == "all" or extra == "verify-all" or extra ==
+"format" Requires-Dist: shellingham Description-Content-Type: text/markdown
                     ****** ð  Delfino Core   ð ******
               **** A Delfino plugin with core functionality. ****
  [CircleCI] [Codecov] [GitHub_tag_(latest_SemVer)] [Maintenance] [GitHub_last
                   commit] [PyPI_-_Python_Version] [Downloads]
 # Commands | Command | Description | |-----------------------|-----------------
 ------------------------------------| | coverage-open | Open coverage results
 in default browser. | | coverage-report | Analyse coverage and generate a term/
```

