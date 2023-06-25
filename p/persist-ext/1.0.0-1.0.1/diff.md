# Comparing `tmp/persist_ext-1.0.0.tar.gz` & `tmp/persist_ext-1.0.1.tar.gz`

## Comparing `persist_ext-1.0.0.tar` & `persist_ext-1.0.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.commitlintrc.json
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.copier-answers.yml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.czrc
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.nvmrc
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.yarnrc.yml
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 persist_ext-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 persist_ext-1.0.0/RELEASE.md
--rwxr-xr-x   0        0        0      636 2020-02-02 00:00:00.000000 persist_ext-1.0.0/bootstrap-local.sh
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 persist_ext-1.0.0/commitlint.config.js
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 persist_ext-1.0.0/install.json
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 persist_ext-1.0.0/package.json
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 persist_ext-1.0.0/requirements.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 persist_ext-1.0.0/setup.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 persist_ext-1.0.0/tsconfig.json
--rw-r--r--   0        0        0   343565 2020-02-02 00:00:00.000000 persist_ext-1.0.0/yarn.lock
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.devcontainer/Dockerfile
--rwxr-xr-x   0        0        0      766 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.devcontainer/bootstrap.sh
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.devcontainer/docker-compose.yml
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.husky/commit-msg
--rwxr-xr-x   0        0        0       87 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.husky/pre-commit
--rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.husky/prepare-commit-msg
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.husky/_/.gitignore
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.husky/_/husky.sh
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.vscode/settings.json
--rw-r--r--   0        0        0  1089465 2020-02-02 00:00:00.000000 persist_ext-1.0.0/examples/Altair_Example_Gallery.ipynb
--rw-r--r--   0        0        0    80414 2020-02-02 00:00:00.000000 persist_ext-1.0.0/examples/Demo.ipynb
--rw-r--r--   0        0        0   567149 2020-02-02 00:00:00.000000 persist_ext-1.0.0/examples/Untitled.ipynb
--rw-r--r--   0        0        0  1235439 2020-02-02 00:00:00.000000 persist_ext-1.0.0/examples/basic_ext_test.ipynb
--rw-r--r--   0        0        0  1243763 2020-02-02 00:00:00.000000 persist_ext-1.0.0/examples/dev.ipynb
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/_version.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/extension/__init__.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/extension/apply.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/extension/enable_ext.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/package.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/schemas/persist_ext/console.json
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/schemas/persist_ext/package.json.orig
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/schemas/persist_ext/plugin.json
--rw-r--r--   0        0        0   263384 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js.LICENSE.txt
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/155.21129ced1d879f0785fa.js
--rw-r--r--   0        0        0    12625 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/17.d52f368f1721d2514b10.js
--rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/272.a40ea1c1eb6b824dbf6c.js
--rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/282.31b993d15efa9f4b427f.js
--rw-r--r--   0        0        0   180692 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/330.0233761a4ed55ca778a8.js
--rw-r--r--   0        0        0   463180 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/418.202205bf18e8d9b7adfc.js
--rw-r--r--   0        0        0    30824 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/420.2aacdf240ecd17037004.js
--rw-r--r--   0        0        0    70490 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js.LICENSE.txt
--rw-r--r--   0        0        0   160914 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/506.47e0d0aa5a743badc447.js
--rw-r--r--   0        0        0    63526 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js.LICENSE.txt
--rw-r--r--   0        0        0   110006 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/576.f46a9cef552a1687b51f.js
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/653.20ef6fe99a41cdb60b2f.js
--rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/687.e84391682616a2de3d0a.js
--rw-r--r--   0        0        0    36455 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/746.86cff8949c0d25126e86.js
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/746.86cff8949c0d25126e86.js.LICENSE.txt
--rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/remoteEntry.d8fbea7fc2e06194799e.js
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/style.js
--rw-r--r--   0        0        0   113607 2020-02-02 00:00:00.000000 persist_ext-1.0.0/persist_ext/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 persist_ext-1.0.0/schema/console.json
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 persist_ext-1.0.0/schema/plugin.json
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/constants.ts
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/index.ts
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/index.ts
--rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/trrackableCell.ts
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/trrackableCellFactory.ts
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/ExtractDataBtn.tsx
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/OutputHeader.tsx
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/commands.ts
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/extract_helpers.ts
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/index.ts
--rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/cells/output/renderer.ts
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/components/CommandButton.tsx
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/cellFactoryPlugin.ts
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/index.ts
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/idePlugin/nbExtension.ts
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/idePlugin/plugin.ts
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/logConsole/console.ts
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/extension/logConsole/logLevelSwitcher.tsx
--rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/interactions/apply.ts
--rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/interactions/helpers.ts
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/interactions/types.ts
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/index.ts
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/notebookActions.ts
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/utils.ts
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/kernel/dataset.ts
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/kernel/exec.ts
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/kernel/index.ts
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/notebook/kernel/utils.ts
--rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/component.tsx
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/helper.ts
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/index.ts
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/init.ts
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/manager.ts
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/renderer.tsx
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/trrack/types.ts
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/IDEGlobal.ts
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/applyReduce.ts
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/deepClone.ts
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/disposable.ts
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/flavoredId.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/icons.ts
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/immer.ts
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/index.ts
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/jsonpath.ts
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/logging.ts
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/nullable.ts
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/objectToKeyValuePairs.ts
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/pipe.ts
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/prettify.ts
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/svg.d.ts
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/tsHelpers.ts
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/utils/uuid.ts
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/helpers.ts
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/index.ts
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/listeners.ts
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/manager.ts
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/renderer.ts
--rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/aggregate.ts
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/encoding.ts
--rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/filter.ts
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/helper.ts
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/index.ts
--rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/processor.ts
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/selection.ts
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/spec.ts
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 persist_ext-1.0.0/src/vegaL/spec/view.ts
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/base.css
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/index.css
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/index.js
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/output-area.css
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/output-header.css
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/output-trrack.css
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 persist_ext-1.0.0/style/trrack.css
--rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 persist_ext-1.0.0/.gitignore
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 persist_ext-1.0.0/LICENSE
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 persist_ext-1.0.0/README.md
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 persist_ext-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 persist_ext-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.commitlintrc.json
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.copier-answers.yml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.czrc
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.nvmrc
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.yarnrc.yml
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 persist_ext-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 persist_ext-1.0.1/RELEASE.md
+-rwxr-xr-x   0        0        0      636 2020-02-02 00:00:00.000000 persist_ext-1.0.1/bootstrap-local.sh
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 persist_ext-1.0.1/commitlint.config.js
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 persist_ext-1.0.1/install.json
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 persist_ext-1.0.1/package.json
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 persist_ext-1.0.1/requirements.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 persist_ext-1.0.1/setup.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 persist_ext-1.0.1/tsconfig.json
+-rw-r--r--   0        0        0   343565 2020-02-02 00:00:00.000000 persist_ext-1.0.1/yarn.lock
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.devcontainer/Dockerfile
+-rwxr-xr-x   0        0        0      766 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.devcontainer/bootstrap.sh
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.devcontainer/docker-compose.yml
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.husky/commit-msg
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.husky/pre-commit
+-rwxr-xr-x   0        0        0      130 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.husky/prepare-commit-msg
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.husky/_/.gitignore
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.husky/_/husky.sh
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.vscode/settings.json
+-rw-r--r--   0        0        0  1089465 2020-02-02 00:00:00.000000 persist_ext-1.0.1/examples/Altair_Example_Gallery.ipynb
+-rw-r--r--   0        0        0    80414 2020-02-02 00:00:00.000000 persist_ext-1.0.1/examples/Demo.ipynb
+-rw-r--r--   0        0        0   567149 2020-02-02 00:00:00.000000 persist_ext-1.0.1/examples/Untitled.ipynb
+-rw-r--r--   0        0        0  1235439 2020-02-02 00:00:00.000000 persist_ext-1.0.1/examples/basic_ext_test.ipynb
+-rw-r--r--   0        0        0  1243763 2020-02-02 00:00:00.000000 persist_ext-1.0.1/examples/dev.ipynb
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/_version.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/extension/__init__.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/extension/apply.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/extension/enable_ext.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/package.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/schemas/persist_ext/console.json
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/schemas/persist_ext/package.json.orig
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/schemas/persist_ext/plugin.json
+-rw-r--r--   0        0        0   263384 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js.LICENSE.txt
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/155.21129ced1d879f0785fa.js
+-rw-r--r--   0        0        0    12625 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/17.d52f368f1721d2514b10.js
+-rw-r--r--   0        0        0     8868 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/272.a40ea1c1eb6b824dbf6c.js
+-rw-r--r--   0        0        0     6861 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/282.31b993d15efa9f4b427f.js
+-rw-r--r--   0        0        0   180692 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/330.0233761a4ed55ca778a8.js
+-rw-r--r--   0        0        0   463180 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/418.202205bf18e8d9b7adfc.js
+-rw-r--r--   0        0        0    30824 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/420.2aacdf240ecd17037004.js
+-rw-r--r--   0        0        0    70490 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js.LICENSE.txt
+-rw-r--r--   0        0        0   160914 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/506.47e0d0aa5a743badc447.js
+-rw-r--r--   0        0        0    63526 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js.LICENSE.txt
+-rw-r--r--   0        0        0   110006 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/576.f46a9cef552a1687b51f.js
+-rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/653.20ef6fe99a41cdb60b2f.js
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/687.e84391682616a2de3d0a.js
+-rw-r--r--   0        0        0    36455 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/746.86cff8949c0d25126e86.js
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/746.86cff8949c0d25126e86.js.LICENSE.txt
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/remoteEntry.2d4c8bc416f5f71f9434.js
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/style.js
+-rw-r--r--   0        0        0   113607 2020-02-02 00:00:00.000000 persist_ext-1.0.1/persist_ext/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 persist_ext-1.0.1/schema/console.json
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 persist_ext-1.0.1/schema/plugin.json
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/constants.ts
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/index.ts
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/index.ts
+-rw-r--r--   0        0        0     3221 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/trrackableCell.ts
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/trrackableCellFactory.ts
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/ExtractDataBtn.tsx
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/OutputHeader.tsx
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/commands.ts
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/extract_helpers.ts
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/index.ts
+-rw-r--r--   0        0        0     6282 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/cells/output/renderer.ts
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/components/CommandButton.tsx
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/cellFactoryPlugin.ts
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/index.ts
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/idePlugin/nbExtension.ts
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/idePlugin/plugin.ts
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/logConsole/console.ts
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/extension/logConsole/logLevelSwitcher.tsx
+-rw-r--r--   0        0        0     5905 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/interactions/apply.ts
+-rw-r--r--   0        0        0     3348 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/interactions/helpers.ts
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/interactions/types.ts
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/index.ts
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/notebookActions.ts
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/utils.ts
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/kernel/dataset.ts
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/kernel/exec.ts
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/kernel/index.ts
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/notebook/kernel/utils.ts
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/component.tsx
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/helper.ts
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/index.ts
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/init.ts
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/manager.ts
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/renderer.tsx
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/trrack/types.ts
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/IDEGlobal.ts
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/applyReduce.ts
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/deepClone.ts
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/disposable.ts
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/flavoredId.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/icons.ts
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/immer.ts
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/index.ts
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/jsonpath.ts
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/logging.ts
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/nullable.ts
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/objectToKeyValuePairs.ts
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/pipe.ts
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/prettify.ts
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/svg.d.ts
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/tsHelpers.ts
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/utils/uuid.ts
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/helpers.ts
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/index.ts
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/listeners.ts
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/manager.ts
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/renderer.ts
+-rw-r--r--   0        0        0     6898 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/aggregate.ts
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/encoding.ts
+-rw-r--r--   0        0        0     5341 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/filter.ts
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/helper.ts
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/index.ts
+-rw-r--r--   0        0        0     9089 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/processor.ts
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/selection.ts
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/spec.ts
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 persist_ext-1.0.1/src/vegaL/spec/view.ts
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/base.css
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/index.css
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/index.js
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/output-area.css
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/output-header.css
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/output-trrack.css
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 persist_ext-1.0.1/style/trrack.css
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 persist_ext-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 persist_ext-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 persist_ext-1.0.1/README.md
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 persist_ext-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5413 2020-02-02 00:00:00.000000 persist_ext-1.0.1/PKG-INFO
```

### Comparing `persist_ext-1.0.0/.copier-answers.yml` & `persist_ext-1.0.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/RELEASE.md` & `persist_ext-1.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/bootstrap-local.sh` & `persist_ext-1.0.1/bootstrap-local.sh`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/package.json` & `persist_ext-1.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -215,9 +215,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `persist_ext-1.0.0/requirements.txt` & `persist_ext-1.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/tsconfig.json` & `persist_ext-1.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/yarn.lock` & `persist_ext-1.0.1/yarn.lock`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/.devcontainer/Dockerfile` & `persist_ext-1.0.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/.devcontainer/bootstrap.sh` & `persist_ext-1.0.1/.devcontainer/bootstrap.sh`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/.devcontainer/devcontainer.json` & `persist_ext-1.0.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/.husky/_/husky.sh` & `persist_ext-1.0.1/.husky/_/husky.sh`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/examples/Altair_Example_Gallery.ipynb` & `persist_ext-1.0.1/examples/Altair_Example_Gallery.ipynb`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/examples/Demo.ipynb` & `persist_ext-1.0.1/examples/Demo.ipynb`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/examples/Untitled.ipynb` & `persist_ext-1.0.1/examples/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/examples/basic_ext_test.ipynb` & `persist_ext-1.0.1/examples/basic_ext_test.ipynb`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/examples/dev.ipynb` & `persist_ext-1.0.1/examples/dev.ipynb`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/__init__.py` & `persist_ext-1.0.1/persist_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/extension/apply.py` & `persist_ext-1.0.1/persist_ext/extension/apply.py`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/extension/enable_ext.py` & `persist_ext-1.0.1/persist_ext/extension/enable_ext.py`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/package.json` & `persist_ext-1.0.1/persist_ext/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9803685897435896%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.2d4c8bc416f5f71f9434.js'}}",*

 * * "'version'": "'1.0.1'"}*

```diff
@@ -133,15 +133,15 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "schema/*.json"
     ],
     "homepage": "https://github.com/visdesignlab/persist",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.d8fbea7fc2e06194799e.js",
+            "load": "static/remoteEntry.2d4c8bc416f5f71f9434.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "persist_ext/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -220,9 +220,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `persist_ext-1.0.0/persist_ext/labextension/schemas/persist_ext/console.json` & `persist_ext-1.0.1/persist_ext/labextension/schemas/persist_ext/console.json`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/schemas/persist_ext/package.json.orig` & `persist_ext-1.0.1/persist_ext/labextension/schemas/persist_ext/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9807692307692307%*

 * *Differences: {"'version'": "'1.0.1'"}*

```diff
@@ -215,9 +215,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.0.1"
 }
```

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js` & `persist_ext-1.0.1/persist_ext/labextension/static/117.d12f72e66f5cd6d77551.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/155.21129ced1d879f0785fa.js` & `persist_ext-1.0.1/persist_ext/labextension/static/155.21129ced1d879f0785fa.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/17.d52f368f1721d2514b10.js` & `persist_ext-1.0.1/persist_ext/labextension/static/17.d52f368f1721d2514b10.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/272.a40ea1c1eb6b824dbf6c.js` & `persist_ext-1.0.1/persist_ext/labextension/static/272.a40ea1c1eb6b824dbf6c.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/282.31b993d15efa9f4b427f.js` & `persist_ext-1.0.1/persist_ext/labextension/static/282.31b993d15efa9f4b427f.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/330.0233761a4ed55ca778a8.js` & `persist_ext-1.0.1/persist_ext/labextension/static/330.0233761a4ed55ca778a8.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/418.202205bf18e8d9b7adfc.js` & `persist_ext-1.0.1/persist_ext/labextension/static/418.202205bf18e8d9b7adfc.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/420.2aacdf240ecd17037004.js` & `persist_ext-1.0.1/persist_ext/labextension/static/420.2aacdf240ecd17037004.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js` & `persist_ext-1.0.1/persist_ext/labextension/static/486.cf7d033b10a71ae22584.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/506.47e0d0aa5a743badc447.js` & `persist_ext-1.0.1/persist_ext/labextension/static/506.47e0d0aa5a743badc447.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js` & `persist_ext-1.0.1/persist_ext/labextension/static/574.dd15c2c64f0acad65e7a.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/576.f46a9cef552a1687b51f.js` & `persist_ext-1.0.1/persist_ext/labextension/static/576.f46a9cef552a1687b51f.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/653.20ef6fe99a41cdb60b2f.js` & `persist_ext-1.0.1/persist_ext/labextension/static/653.20ef6fe99a41cdb60b2f.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/687.e84391682616a2de3d0a.js` & `persist_ext-1.0.1/persist_ext/labextension/static/687.e84391682616a2de3d0a.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/746.86cff8949c0d25126e86.js` & `persist_ext-1.0.1/persist_ext/labextension/static/746.86cff8949c0d25126e86.js`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/remoteEntry.d8fbea7fc2e06194799e.js` & `persist_ext-1.0.1/persist_ext/labextension/static/remoteEntry.2d4c8bc416f5f71f9434.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -138,15 +138,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@trrack/core", "1.2.0", (() => Promise.all([S.e(574), S.e(155)]).then((() => () => S(2574))))), l("@trrack/vis-react", "1.3.0", (() => Promise.all([S.e(117), S.e(602), S.e(85)]).then((() => () => S(9117))))), l("d3", "7.8.5", (() => Promise.all([S.e(330), S.e(17), S.e(576)]).then((() => () => S(4576))))), l("immutable-json-patch", "5.1.2", (() => S.e(272).then((() => () => S(8272))))), l("jsonpath-plus", "7.2.0", (() => S.e(653).then((() => () => S(5653))))), l("lodash", "4.17.21", (() => S.e(486).then((() => () => S(6486))))), l("persist_ext", "1.0.0", (() => Promise.all([S.e(330), S.e(418), S.e(17), S.e(746), S.e(602), S.e(420)]).then((() => () => S(5681))))), l("uuid", "9.0.0", (() => S.e(687).then((() => () => S(9687))))), l("vega-lite", "5.11.0", (() => Promise.all([S.e(330), S.e(418), S.e(506)]).then((() => () => S(1047)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@trrack/core", "1.2.0", (() => Promise.all([S.e(574), S.e(155)]).then((() => () => S(2574))))), l("@trrack/vis-react", "1.3.0", (() => Promise.all([S.e(117), S.e(602), S.e(85)]).then((() => () => S(9117))))), l("d3", "7.8.5", (() => Promise.all([S.e(330), S.e(17), S.e(576)]).then((() => () => S(4576))))), l("immutable-json-patch", "5.1.2", (() => S.e(272).then((() => () => S(8272))))), l("jsonpath-plus", "7.2.0", (() => S.e(653).then((() => () => S(5653))))), l("lodash", "4.17.21", (() => S.e(486).then((() => () => S(6486))))), l("persist_ext", "1.0.1", (() => Promise.all([S.e(330), S.e(418), S.e(17), S.e(746), S.e(602), S.e(420)]).then((() => () => S(5681))))), l("uuid", "9.0.0", (() => S.e(687).then((() => () => S(9687))))), l("vega-lite", "5.11.0", (() => Promise.all([S.e(330), S.e(418), S.e(506)]).then((() => () => S(1047)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         S.g.importScripts && (e = S.g.location + "");
         var r = S.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
```

### Comparing `persist_ext-1.0.0/persist_ext/labextension/static/third-party-licenses.json` & `persist_ext-1.0.1/persist_ext/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/schema/console.json` & `persist_ext-1.0.1/schema/console.json`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/trrackableCell.ts` & `persist_ext-1.0.1/src/cells/trrackableCell.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/output/ExtractDataBtn.tsx` & `persist_ext-1.0.1/src/cells/output/ExtractDataBtn.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/output/OutputHeader.tsx` & `persist_ext-1.0.1/src/cells/output/OutputHeader.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/output/commands.ts` & `persist_ext-1.0.1/src/cells/output/commands.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/output/extract_helpers.ts` & `persist_ext-1.0.1/src/cells/output/extract_helpers.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/cells/output/renderer.ts` & `persist_ext-1.0.1/src/cells/output/renderer.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/components/CommandButton.tsx` & `persist_ext-1.0.1/src/components/CommandButton.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/extension/cellFactoryPlugin.ts` & `persist_ext-1.0.1/src/extension/cellFactoryPlugin.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/extension/idePlugin/nbExtension.ts` & `persist_ext-1.0.1/src/extension/idePlugin/nbExtension.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/extension/idePlugin/plugin.ts` & `persist_ext-1.0.1/src/extension/idePlugin/plugin.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/extension/logConsole/console.ts` & `persist_ext-1.0.1/src/extension/logConsole/console.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/extension/logConsole/logLevelSwitcher.tsx` & `persist_ext-1.0.1/src/extension/logConsole/logLevelSwitcher.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/interactions/apply.ts` & `persist_ext-1.0.1/src/interactions/apply.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/interactions/helpers.ts` & `persist_ext-1.0.1/src/interactions/helpers.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/interactions/types.ts` & `persist_ext-1.0.1/src/interactions/types.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/notebook/notebookActions.ts` & `persist_ext-1.0.1/src/notebook/notebookActions.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/notebook/kernel/dataset.ts` & `persist_ext-1.0.1/src/notebook/kernel/dataset.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/notebook/kernel/exec.ts` & `persist_ext-1.0.1/src/notebook/kernel/exec.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/trrack/component.tsx` & `persist_ext-1.0.1/src/trrack/component.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/trrack/init.ts` & `persist_ext-1.0.1/src/trrack/init.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/trrack/manager.ts` & `persist_ext-1.0.1/src/trrack/manager.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/trrack/renderer.tsx` & `persist_ext-1.0.1/src/trrack/renderer.tsx`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/trrack/types.ts` & `persist_ext-1.0.1/src/trrack/types.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/utils/IDEGlobal.ts` & `persist_ext-1.0.1/src/utils/IDEGlobal.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/utils/logging.ts` & `persist_ext-1.0.1/src/utils/logging.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/listeners.ts` & `persist_ext-1.0.1/src/vegaL/listeners.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/manager.ts` & `persist_ext-1.0.1/src/vegaL/manager.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/renderer.ts` & `persist_ext-1.0.1/src/vegaL/renderer.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/aggregate.ts` & `persist_ext-1.0.1/src/vegaL/spec/aggregate.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/encoding.ts` & `persist_ext-1.0.1/src/vegaL/spec/encoding.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/filter.ts` & `persist_ext-1.0.1/src/vegaL/spec/filter.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/helper.ts` & `persist_ext-1.0.1/src/vegaL/spec/helper.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/processor.ts` & `persist_ext-1.0.1/src/vegaL/spec/processor.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/selection.ts` & `persist_ext-1.0.1/src/vegaL/spec/selection.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/spec.ts` & `persist_ext-1.0.1/src/vegaL/spec/spec.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/src/vegaL/spec/view.ts` & `persist_ext-1.0.1/src/vegaL/spec/view.ts`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/style/base.css` & `persist_ext-1.0.1/style/base.css`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/style/output-area.css` & `persist_ext-1.0.1/style/output-area.css`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/.gitignore` & `persist_ext-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/LICENSE` & `persist_ext-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/README.md` & `persist_ext-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/pyproject.toml` & `persist_ext-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `persist_ext-1.0.0/PKG-INFO` & `persist_ext-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persist_ext
-Version: 1.0.0
+Version: 1.0.1
 Summary: PersIst is a JupyterLab extension to enable persistent interactive visualizations in JupyterLab notebooks.
 Project-URL: Homepage, https://github.com/visdesignlab/persist
 Project-URL: Bug Tracker, https://github.com/visdesignlab/persist/issues
 Project-URL: Repository, https://github.com/visdesignlab/persist.git
 Author-email: Kiran Gadhave <kirangadhave2@gmail.com>
 License: BSD 3-Clause License
```

