# Comparing `tmp/seoul256_jupyterlab_theme-0.1.0.tar.gz` & `tmp/seoul256_jupyterlab_theme-0.2.0.tar.gz`

## Comparing `seoul256_jupyterlab_theme-0.1.0.tar` & `seoul256_jupyterlab_theme-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/.copier-answers.yml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/.prettierignore
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/RELEASE.md
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/install.json
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/tsconfig.json
--rw-r--r--   0        0        0   182058 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/yarn.lock
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/.._version.py.icloud
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/_version.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/package.json
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/568.8626ba9b2a05ed2f8a88.js
--rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/remoteEntry.94050887224872452913.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/style.js
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    17203 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.css
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.js
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/src/index.ts
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/style/custom.css
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/style/index.css
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/style/style.css
--rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/style/variables.css
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/LICENSE
--rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/README.md
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/.copier-answers.yml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/.prettierignore
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/install.json
+-rw-r--r--   0        0        0     6431 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   182058 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/yarn.lock
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/_version.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/package.json
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/568.8626ba9b2a05ed2f8a88.js
+-rw-r--r--   0        0        0     6294 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/remoteEntry.2bd21849baf1c7c34b32.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/style.js
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    17204 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.js
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/src/index.ts
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/style/custom.css
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/style/index.css
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/style/style.css
+-rw-r--r--   0        0        0    15794 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/style/variables.css
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2504 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/README.md
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5377 2020-02-02 00:00:00.000000 seoul256_jupyterlab_theme-0.2.0/PKG-INFO
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/RELEASE.md` & `seoul256_jupyterlab_theme-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/package.json` & `seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9690656565656565%*

 * *Differences: {"'jupyterlab'": "{'_build': OrderedDict([('load', 'static/remoteEntry.2bd21849baf1c7c34b32.js'), "*

 * *                 "('extension', './extension')])}",*

 * * "'stylelint'": "{'rules': {'selector-class-pattern': "*

 * *                "'^([a-zA-Z]*)(-[a-zA-Z0-9]+)*$|^([a-z][a-z0-9]*)(-[a-z0-9]+)*$', "*

 * *                "'selector-pseudo-element-colon-notation': 'single', "*

 * *                "'shorthand-property-no-redundant-values': None, 'no-descending-specificity': "*

 * *                "[True, OrderedDict([('ignore', ['sel […]*

```diff
@@ -96,14 +96,18 @@
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/muwizayeon/seoul256-jupyterlab-theme",
     "jupyterlab": {
+        "_build": {
+            "extension": "./extension",
+            "load": "static/remoteEntry.2bd21849baf1c7c34b32.js"
+        },
         "extension": true,
         "outputDir": "seoul256_jupyterlab_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -159,15 +163,26 @@
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
         "rules": {
             "alpha-value-notation": null,
             "color-function-notation": null,
+            "no-descending-specificity": [
+                true,
+                {
+                    "ignore": [
+                        "selectors-within-list"
+                    ]
+                }
+            ],
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-zA-Z]*)(-[a-zA-Z0-9]+)*$|^([a-z][a-z0-9]*)(-[a-z0-9]+)*$",
             "selector-no-vendor-prefix": null,
+            "selector-pseudo-element-colon-notation": "single",
+            "shorthand-property-no-redundant-values": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/tsconfig.json` & `seoul256_jupyterlab_theme-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/yarn.lock` & `seoul256_jupyterlab_theme-0.2.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/__init__.py` & `seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/package.json` & `seoul256_jupyterlab_theme-0.2.0/package.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9690656565656565%*

 * *Differences: {"'jupyterlab'": "{delete: ['_build']}",*

 * * "'stylelint'": "{'rules': {'selector-class-pattern': "*

 * *                "'^([a-zA-Z]*)(-[a-zA-Z0-9]+)*$|^([a-z][a-z0-9]*)(-[a-z0-9]+)*$', "*

 * *                "'selector-pseudo-element-colon-notation': 'single', "*

 * *                "'shorthand-property-no-redundant-values': None, 'no-descending-specificity': "*

 * *                "[True, OrderedDict([('ignore', ['selectors-within-list'])])]}}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -96,18 +96,14 @@
     ],
     "files": [
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/muwizayeon/seoul256-jupyterlab-theme",
     "jupyterlab": {
-        "_build": {
-            "extension": "./extension",
-            "load": "static/remoteEntry.94050887224872452913.js"
-        },
         "extension": true,
         "outputDir": "seoul256_jupyterlab_theme/labextension",
         "themePath": "style/index.css"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
@@ -163,15 +159,26 @@
             "stylelint-config-recommended",
             "stylelint-config-standard",
             "stylelint-prettier/recommended"
         ],
         "rules": {
             "alpha-value-notation": null,
             "color-function-notation": null,
+            "no-descending-specificity": [
+                true,
+                {
+                    "ignore": [
+                        "selectors-within-list"
+                    ]
+                }
+            ],
             "property-no-vendor-prefix": null,
+            "selector-class-pattern": "^([a-zA-Z]*)(-[a-zA-Z0-9]+)*$|^([a-z][a-z0-9]*)(-[a-z0-9]+)*$",
             "selector-no-vendor-prefix": null,
+            "selector-pseudo-element-colon-notation": "single",
+            "shorthand-property-no-redundant-values": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.2.0"
 }
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/568.8626ba9b2a05ed2f8a88.js` & `seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/568.8626ba9b2a05ed2f8a88.js`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/static/remoteEntry.94050887224872452913.js` & `seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/static/remoteEntry.2bd21849baf1c7c34b32.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
     var e, r, t, n, o, a, i, u, l, s, f, p, d, c, h, v, m = {
-            869: (e, r, t) => {
+            284: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(568).then((() => () => t(568))),
                         "./extension": () => t.e(568).then((() => () => t(568)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
@@ -98,15 +98,15 @@
                     var o = a[e] = a[e] || {},
                         u = o[r];
                     (!u || !u.loaded && (1 != !u.eager ? n : i > u.from)) && (o[r] = {
                         get: () => b.e(568).then((() => () => b(568))),
                         from: i,
                         eager: !1
                     })
-                })("seoul256-jupyterlab-theme", "0.1.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                })("seoul256-jupyterlab-theme", "0.2.0"), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         b.g.importScripts && (e = b.g.location + "");
         var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -257,10 +257,10 @@
                     u && u(b)
                 }
                 for (r && r(t); l < a.length; l++) o = a[l], b.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunkseoul256_jupyterlab_theme = self.webpackChunkseoul256_jupyterlab_theme || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })();
-    var y = b(869);
+    var y = b(284);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["seoul256-jupyterlab-theme"] = y
 })();
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.css` & `seoul256_jupyterlab_theme-0.2.0/seoul256_jupyterlab_theme/labextension/themes/seoul256-jupyterlab-theme/index.css`

 * *Files 3% similar despite different names*

```diff
@@ -398,41 +398,41 @@
 
   /* Sidebar-related styles */
 
   --jp-sidebar-min-width: 180px;
 }
 
 /* Notebook tab bar */
-.lm-dockpanel-tabbar {
+.lm-DockPanel-tabBar {
   background: transparent;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab {
+.lm-DockPanel-tabBar .lm-TabBar-tab {
   margin-left: 2px;
   transition: text-shadow cubic-bezier(0, 0.2, 0, 0.2) 0.2s,
     color cubic-bezier(0, 0.2, 0, 0.2) 0.2s, opacity 0.2s;
-  padding: 1px 8px 0.0001px;
+  padding: 1px 8px 0.0001px 8px;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab.jp-mod-current::before {
+.lm-DockPanel-tabBar .lm-TabBar-tab.jp-mod-current:before {
   top: auto;
   bottom: calc(-1 * var(--jp-border-width));
   height: 1.5px;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab.lm-mod-closable > .lm-tabbar-tabcloseicon {
+.lm-DockPanel-tabBar .lm-TabBar-tab.lm-mod-closable > .lm-TabBar-tabCloseIcon {
   opacity: 0;
 }
 
-.lm-dockpanel-tabbar
-  .lm-tabbar-tab.lm-mod-closable:hover:not(.lm-mod-current)
-  > .lm-tabbar-tabcloseicon
-  .lm-dockpanel-tabbar
-  .lm-tabbar-tab.lm-mod-closable.lm-mod-current
-  > .lm-tabbar-tabcloseicon {
+.lm-DockPanel-tabBar
+  .lm-TabBar-tab.lm-mod-closable:hover:not(.lm-mod-current)
+  > .lm-TabBar-tabCloseIcon,
+.lm-DockPanel-tabBar
+  .lm-TabBar-tab.lm-mod-closable.lm-mod-current
+  > .lm-TabBar-tabCloseIcon {
   opacity: 1;
 }
 
 /* Custom  */
 
 /* Dialog - Rename file */
 input.jp-mod-styled {
@@ -442,15 +442,15 @@
 select.jp-mod-styled {
   background: var(--seoul256-dark-black);
 }
 
 /* Background */
 
 /* Seould 256 Dark Style */
-.lm-dockpanel-tabbar .lm-tabbar-tab.jp-mod-current::before {
+.lm-DockPanel-tabBar .lm-TabBar-tab.jp-mod-current:before {
   background: linear-gradient(
     to right,
     #941e34,
     #bc6f25,
     #6789ca,
     #455f54,
     #594743
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/src/index.ts` & `seoul256_jupyterlab_theme-0.2.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/style/style.css` & `seoul256_jupyterlab_theme-0.2.0/style/style.css`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 /* Notebook tab bar */
-.lm-dockpanel-tabbar {
+.lm-DockPanel-tabBar {
   background: transparent;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab {
+.lm-DockPanel-tabBar .lm-TabBar-tab {
   margin-left: 2px;
   transition: text-shadow cubic-bezier(0, 0.2, 0, 0.2) 0.2s,
     color cubic-bezier(0, 0.2, 0, 0.2) 0.2s, opacity 0.2s;
-  padding: 1px 8px 0.0001px;
+  padding: 1px 8px 0.0001px 8px;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab.jp-mod-current::before {
+.lm-DockPanel-tabBar .lm-TabBar-tab.jp-mod-current:before {
   top: auto;
   bottom: calc(-1 * var(--jp-border-width));
   height: 1.5px;
 }
 
-.lm-dockpanel-tabbar .lm-tabbar-tab.lm-mod-closable > .lm-tabbar-tabcloseicon {
+.lm-DockPanel-tabBar .lm-TabBar-tab.lm-mod-closable > .lm-TabBar-tabCloseIcon {
   opacity: 0;
 }
 
-.lm-dockpanel-tabbar
-  .lm-tabbar-tab.lm-mod-closable:hover:not(.lm-mod-current)
-  > .lm-tabbar-tabcloseicon
-  .lm-dockpanel-tabbar
-  .lm-tabbar-tab.lm-mod-closable.lm-mod-current
-  > .lm-tabbar-tabcloseicon {
+.lm-DockPanel-tabBar
+  .lm-TabBar-tab.lm-mod-closable:hover:not(.lm-mod-current)
+  > .lm-TabBar-tabCloseIcon,
+.lm-DockPanel-tabBar
+  .lm-TabBar-tab.lm-mod-closable.lm-mod-current
+  > .lm-TabBar-tabCloseIcon {
   opacity: 1;
 }
```

### Comparing `seoul256_jupyterlab_theme-0.1.0/style/variables.css` & `seoul256_jupyterlab_theme-0.2.0/style/variables.css`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/.gitignore` & `seoul256_jupyterlab_theme-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/LICENSE` & `seoul256_jupyterlab_theme-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/README.md` & `seoul256_jupyterlab_theme-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/pyproject.toml` & `seoul256_jupyterlab_theme-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `seoul256_jupyterlab_theme-0.1.0/PKG-INFO` & `seoul256_jupyterlab_theme-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seoul256_jupyterlab_theme
-Version: 0.1.0
+Version: 0.2.0
 Summary: A JupyterLab theme with Seoul 256 color scheme
 Project-URL: Homepage, https://github.com/muwizayeon/seoul256-jupyterlab-theme
 Project-URL: Bug Tracker, https://github.com/muwizayeon/seoul256-jupyterlab-theme/issues
 Project-URL: Repository, https://github.com/muwizayeon/seoul256-jupyterlab-theme.git
 Author-email: muwizayeon <muwizayeon@gmail.com>
 License: BSD 3-Clause License
```

