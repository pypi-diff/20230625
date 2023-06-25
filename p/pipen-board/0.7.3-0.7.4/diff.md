# Comparing `tmp/pipen_board-0.7.3.tar.gz` & `tmp/pipen_board-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipen_board-0.7.3.tar", max compression
+gzip compressed data, was "pipen_board-0.7.4.tar", max compression
```

## Comparing `pipen_board-0.7.3.tar` & `pipen_board-0.7.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     6884 2023-06-23 21:47:43.898396 pipen_board-0.7.3/README.md
--rw-r--r--   0        0        0      269 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/__init__.py
--rw-r--r--   0        0        0      517 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/additional_auto.toml
--rw-r--r--   0        0        0    15248 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/apis.py
--rw-r--r--   0        0        0     4594 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/cli.py
--rw-r--r--   0        0        0    31923 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/data_manager.py
--rw-r--r--   0        0        0     6233 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/defaults.py
--rw-r--r--   0        0        0    23628 2023-06-23 21:47:43.898396 pipen_board-0.7.3/pipen_board/frontend/build/assets/favicon.png
--rw-r--r--   0        0        0   625768 2023-06-23 21:47:43.902396 pipen_board-0.7.3/pipen_board/frontend/build/assets/index.css
--rw-r--r--   0        0        0   770013 2023-06-23 21:47:43.906396 pipen_board-0.7.3/pipen_board/frontend/build/assets/index.js
--rw-r--r--   0        0        0     4128 2023-06-23 21:47:43.906396 pipen_board-0.7.3/pipen_board/frontend/build/assets/schema.json
--rw-r--r--   0        0        0      406 2023-06-23 21:47:43.906396 pipen_board-0.7.3/pipen_board/frontend/build/index.html
--rw-r--r--   0        0        0     7742 2023-06-23 21:47:43.910396 pipen_board-0.7.3/pipen_board/plugin.py
--rw-r--r--   0        0        0     3831 2023-06-23 21:47:43.910396 pipen_board-0.7.3/pipen_board/quart_app.py
--rw-r--r--   0        0        0       22 2023-06-23 21:47:43.910396 pipen_board-0.7.3/pipen_board/version.py
--rw-r--r--   0        0        0      890 2023-06-23 21:47:43.910396 pipen_board-0.7.3/pyproject.toml
--rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 pipen_board-0.7.3/setup.py
--rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 pipen_board-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     6884 2023-06-25 01:00:54.881711 pipen_board-0.7.4/README.md
+-rw-r--r--   0        0        0      269 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/additional_auto.toml
+-rw-r--r--   0        0        0    15248 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/apis.py
+-rw-r--r--   0        0        0     4594 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/cli.py
+-rw-r--r--   0        0        0    31923 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/data_manager.py
+-rw-r--r--   0        0        0     6233 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/defaults.py
+-rw-r--r--   0        0        0     1159 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/frontend/build/assets/favicon-running.png
+-rw-r--r--   0        0        0    15525 2023-06-25 01:00:54.881711 pipen_board-0.7.4/pipen_board/frontend/build/assets/favicon.png
+-rw-r--r--   0        0        0   625768 2023-06-25 01:00:54.885711 pipen_board-0.7.4/pipen_board/frontend/build/assets/index.css
+-rw-r--r--   0        0        0   770560 2023-06-25 01:00:54.889711 pipen_board-0.7.4/pipen_board/frontend/build/assets/index.js
+-rw-r--r--   0        0        0     4128 2023-06-25 01:00:54.889711 pipen_board-0.7.4/pipen_board/frontend/build/assets/schema.json
+-rw-r--r--   0        0        0      406 2023-06-25 01:00:54.889711 pipen_board-0.7.4/pipen_board/frontend/build/index.html
+-rw-r--r--   0        0        0     7742 2023-06-25 01:00:54.897711 pipen_board-0.7.4/pipen_board/plugin.py
+-rw-r--r--   0        0        0     4007 2023-06-25 01:00:54.897711 pipen_board-0.7.4/pipen_board/quart_app.py
+-rw-r--r--   0        0        0       22 2023-06-25 01:00:54.897711 pipen_board-0.7.4/pipen_board/version.py
+-rw-r--r--   0        0        0      890 2023-06-25 01:00:54.897711 pipen_board-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     8044 1970-01-01 00:00:00.000000 pipen_board-0.7.4/setup.py
+-rw-r--r--   0        0        0     7708 1970-01-01 00:00:00.000000 pipen_board-0.7.4/PKG-INFO
```

### Comparing `pipen_board-0.7.3/README.md` & `pipen_board-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/additional_auto.toml` & `pipen_board-0.7.4/pipen_board/additional_auto.toml`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/apis.py` & `pipen_board-0.7.4/pipen_board/apis.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/cli.py` & `pipen_board-0.7.4/pipen_board/cli.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/data_manager.py` & `pipen_board-0.7.4/pipen_board/data_manager.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/defaults.py` & `pipen_board-0.7.4/pipen_board/defaults.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/frontend/build/assets/index.css` & `pipen_board-0.7.4/pipen_board/frontend/build/assets/index.css`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/frontend/build/assets/index.js` & `pipen_board-0.7.4/pipen_board/frontend/build/assets/index.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -346,15 +346,15 @@
         var N = !1;
         if ((y === void 0 || y < 0) && (y = 0), y > this.length || ((T === void 0 || T > this.length) && (T = this.length), T <= 0) || (T >>>= 0, y >>>= 0, T <= y)) return "";
         for (M || (M = "utf8");;) switch (M) {
             case "hex":
                 return Y(this, y, T);
             case "utf8":
             case "utf-8":
-                return W(this, y, T);
+                return G(this, y, T);
             case "ascii":
                 return F(this, y, T);
             case "latin1":
             case "binary":
                 return te(this, y, T);
             case "base64":
                 return U(this, y, T);
@@ -387,15 +387,15 @@
     }, u.prototype.swap64 = function() {
         var y = this.length;
         if (y % 8 !== 0) throw new RangeError("Buffer size must be a multiple of 64-bits");
         for (var T = 0; T < y; T += 8) S(this, T, T + 7), S(this, T + 1, T + 6), S(this, T + 2, T + 5), S(this, T + 3, T + 4);
         return this
     }, u.prototype.toString = function() {
         var y = this.length;
-        return y === 0 ? "" : arguments.length === 0 ? W(this, 0, y) : w.apply(this, arguments)
+        return y === 0 ? "" : arguments.length === 0 ? G(this, 0, y) : w.apply(this, arguments)
     }, u.prototype.toLocaleString = u.prototype.toString, u.prototype.equals = function(y) {
         if (!u.isBuffer(y)) throw new TypeError("Argument must be a Buffer");
         return this === y ? !0 : u.compare(this, y) === 0
     }, u.prototype.inspect = function() {
         var y = "",
             T = t.INSPECT_MAX_BYTES;
         return y = this.toString("hex", 0, T).replace(/(.{2})/g, "$1 ").trim(), this.length > T && (y += " ... "), "<Buffer " + y + ">"
@@ -481,15 +481,15 @@
         return q($(y, M.length - T), M, T, N)
     }
 
     function L(M, y, T, N) {
         return q(re(y), M, T, N)
     }
 
-    function G(M, y, T, N) {
+    function W(M, y, T, N) {
         return q(P(y), M, T, N)
     }
 
     function A(M, y, T, N) {
         return q(ue(y, M.length - T), M, T, N)
     }
     u.prototype.write = function(y, T, N, J) {
@@ -507,15 +507,15 @@
             case "utf-8":
                 return B(this, y, T, N);
             case "ascii":
             case "latin1":
             case "binary":
                 return L(this, y, T, N);
             case "base64":
-                return G(this, y, T, N);
+                return W(this, y, T, N);
             case "ucs2":
             case "ucs-2":
             case "utf16le":
             case "utf-16le":
                 return A(this, y, T, N);
             default:
                 if (H) throw new TypeError("Unknown encoding: " + J);
@@ -528,15 +528,15 @@
         }
     };
 
     function U(M, y, T) {
         return y === 0 && T === M.length ? e.fromByteArray(M) : e.fromByteArray(M.slice(y, T))
     }
 
-    function W(M, y, T) {
+    function G(M, y, T) {
         T = Math.min(M.length, T);
         for (var N = [], J = y; J < T;) {
             var ie = M[J],
                 H = null,
                 x = ie > 239 ? 4 : ie > 223 ? 3 : ie > 191 ? 2 : 1;
             if (J + x <= T) {
                 var se, _e, he, ge;
@@ -2185,27 +2185,27 @@
     } = e;
     const B = getContext("ComposedModal");
 
     function L(K) {
         bubble.call(this, t, K)
     }
 
-    function G(K) {
+    function W(K) {
         bubble.call(this, t, K)
     }
 
     function A(K) {
         bubble.call(this, t, K)
     }
 
     function U(K) {
         bubble.call(this, t, K)
     }
 
-    function W(K) {
+    function G(K) {
         bubble.call(this, t, K)
     }
 
     function j(K) {
         bubble.call(this, t, K)
     }
 
@@ -2252,15 +2252,15 @@
             tabindex: I,
             disabled: w === !0 ? !0 : void 0,
             href: S,
             "aria-pressed": r && _ === "ghost" && !S ? h : void 0,
             ...o,
             class: ["bx--btn", g && "bx--btn--expressive", (d === "small" && !g || d === "sm" && !g || d === "small" && !g) && "bx--btn--sm", d === "field" && !g || d === "md" && !g && "bx--btn--md", d === "field" && "bx--btn--field", d === "small" && "bx--btn--sm", d === "lg" && "bx--btn--lg", d === "xl" && "bx--btn--xl", _ && `bx--btn--${_}`, w && "bx--btn--disabled", r && "bx--btn--icon-only", r && "bx--tooltip__trigger", r && "bx--tooltip--a11y", r && k && `bx--btn--icon-only--${k}`, r && v && `bx--tooltip--align-${v}`, r && h && _ === "ghost" && "bx--btn--selected", o.class].filter(Boolean).join(" ")
         })
-    }, [O, d, p, m, b, E, w, S, r, l, o, _, g, h, v, k, I, D, s, u, L, G, A, U, W, j, Q, F, te, Y, oe, ae, C, Z]
+    }, [O, d, p, m, b, E, w, S, r, l, o, _, g, h, v, k, I, D, s, u, L, W, A, U, G, j, Q, F, te, Y, oe, ae, C, Z]
 }
 class Button extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1K, create_fragment$1K, safe_not_equal, {
             kind: 11,
             size: 1,
             expressive: 12,
@@ -2741,55 +2741,55 @@
 function create_fragment$1J(t) {
     let e, n, r, l, a, o, u, s, c, _, d, g, h, p, m, v, k, b, E, w, S = t[5] && create_if_block_6$6(t),
         I = t[7] && create_if_block_5$8(t);
     const D = t[31].heading,
         O = create_slot(D, t, t[50], get_heading_slot_context),
         B = O || fallback_block$h(t);
     let L = !t[5] && create_if_block_4$c(t);
-    const G = t[31].default,
-        A = create_slot(G, t, t[50], null);
+    const W = t[31].default,
+        A = create_slot(W, t, t[50], null);
     let U = t[10] && create_if_block_3$h(),
-        W = !t[5] && create_if_block$1c(t),
+        G = !t[5] && create_if_block$1c(t),
         j = [{
             role: "presentation"
         }, {
             id: t[18]
         }, t[28]],
         Q = {};
     for (let F = 0; F < j.length; F += 1) Q = assign(Q, j[F]);
     return {
         c() {
-            e = element("div"), n = element("div"), r = element("div"), S && S.c(), l = space(), I && I.c(), a = space(), o = element("h3"), B && B.c(), u = space(), L && L.c(), s = space(), c = element("div"), A && A.c(), p = space(), U && U.c(), m = space(), W && W.c(), attr(o, "id", t[24]), toggle_class(o, "bx--modal-header__heading", !0), toggle_class(r, "bx--modal-header", !0), attr(c, "id", t[23]), attr(c, "tabindex", _ = t[10] ? "0" : void 0), attr(c, "role", d = t[10] ? "region" : void 0), attr(c, "aria-label", g = t[10] ? t[22] : void 0), attr(c, "aria-labelledby", h = t[7] ? t[25] : t[24]), toggle_class(c, "bx--modal-content", !0), toggle_class(c, "bx--modal-content--with-form", t[9]), toggle_class(c, "bx--modal-scroll-content", t[10]), attr(n, "tabindex", "-1"), attr(n, "role", v = t[4] ? t[5] ? "alert" : "alertdialog" : "dialog"), attr(n, "aria-describedby", k = t[4] && !t[5] ? t[23] : void 0), attr(n, "aria-modal", "true"), attr(n, "aria-label", t[22]), toggle_class(n, "bx--modal-container", !0), toggle_class(n, "bx--modal-container--xs", t[2] === "xs"), toggle_class(n, "bx--modal-container--sm", t[2] === "sm"), toggle_class(n, "bx--modal-container--lg", t[2] === "lg"), set_attributes(e, Q), toggle_class(e, "bx--modal", !0), toggle_class(e, "bx--modal-tall", !t[5]), toggle_class(e, "is-visible", t[0]), toggle_class(e, "bx--modal--danger", t[3])
+            e = element("div"), n = element("div"), r = element("div"), S && S.c(), l = space(), I && I.c(), a = space(), o = element("h3"), B && B.c(), u = space(), L && L.c(), s = space(), c = element("div"), A && A.c(), p = space(), U && U.c(), m = space(), G && G.c(), attr(o, "id", t[24]), toggle_class(o, "bx--modal-header__heading", !0), toggle_class(r, "bx--modal-header", !0), attr(c, "id", t[23]), attr(c, "tabindex", _ = t[10] ? "0" : void 0), attr(c, "role", d = t[10] ? "region" : void 0), attr(c, "aria-label", g = t[10] ? t[22] : void 0), attr(c, "aria-labelledby", h = t[7] ? t[25] : t[24]), toggle_class(c, "bx--modal-content", !0), toggle_class(c, "bx--modal-content--with-form", t[9]), toggle_class(c, "bx--modal-scroll-content", t[10]), attr(n, "tabindex", "-1"), attr(n, "role", v = t[4] ? t[5] ? "alert" : "alertdialog" : "dialog"), attr(n, "aria-describedby", k = t[4] && !t[5] ? t[23] : void 0), attr(n, "aria-modal", "true"), attr(n, "aria-label", t[22]), toggle_class(n, "bx--modal-container", !0), toggle_class(n, "bx--modal-container--xs", t[2] === "xs"), toggle_class(n, "bx--modal-container--sm", t[2] === "sm"), toggle_class(n, "bx--modal-container--lg", t[2] === "lg"), set_attributes(e, Q), toggle_class(e, "bx--modal", !0), toggle_class(e, "bx--modal-tall", !t[5]), toggle_class(e, "is-visible", t[0]), toggle_class(e, "bx--modal--danger", t[3])
         },
         m(F, te) {
-            insert(F, e, te), append(e, n), append(n, r), S && S.m(r, null), append(r, l), I && I.m(r, null), append(r, a), append(r, o), B && B.m(o, null), append(r, u), L && L.m(r, null), append(n, s), append(n, c), A && A.m(c, null), append(n, p), U && U.m(n, null), append(n, m), W && W.m(n, null), t[44](n), t[46](e), b = !0, E || (w = [listen(n, "click", t[45]), listen(e, "keydown", t[32]), listen(e, "keydown", t[47]), listen(e, "click", t[33]), listen(e, "click", t[48]), listen(e, "mouseover", t[34]), listen(e, "mouseenter", t[35]), listen(e, "mouseleave", t[36]), listen(e, "transitionend", t[49])], E = !0)
+            insert(F, e, te), append(e, n), append(n, r), S && S.m(r, null), append(r, l), I && I.m(r, null), append(r, a), append(r, o), B && B.m(o, null), append(r, u), L && L.m(r, null), append(n, s), append(n, c), A && A.m(c, null), append(n, p), U && U.m(n, null), append(n, m), G && G.m(n, null), t[44](n), t[46](e), b = !0, E || (w = [listen(n, "click", t[45]), listen(e, "keydown", t[32]), listen(e, "keydown", t[47]), listen(e, "click", t[33]), listen(e, "click", t[48]), listen(e, "mouseover", t[34]), listen(e, "mouseenter", t[35]), listen(e, "mouseleave", t[36]), listen(e, "transitionend", t[49])], E = !0)
         },
         p(F, te) {
             F[5] ? S ? (S.p(F, te), te[0] & 32 && transition_in(S, 1)) : (S = create_if_block_6$6(F), S.c(), transition_in(S, 1), S.m(r, l)) : S && (group_outros(), transition_out(S, 1, 1, () => {
                 S = null
             }), check_outros()), F[7] ? I ? (I.p(F, te), te[0] & 128 && transition_in(I, 1)) : (I = create_if_block_5$8(F), I.c(), transition_in(I, 1), I.m(r, a)) : I && (group_outros(), transition_out(I, 1, 1, () => {
                 I = null
             }), check_outros()), O ? O.p && (!b || te[1] & 524288) && update_slot_base(O, D, F, F[50], b ? get_slot_changes(D, F[50], te, get_heading_slot_changes) : get_all_dirty_from_scope(F[50]), get_heading_slot_context) : B && B.p && (!b || te[0] & 64) && B.p(F, b ? te : [-1, -1]), (!b || te[0] & 16777216) && attr(o, "id", F[24]), F[5] ? L && (group_outros(), transition_out(L, 1, 1, () => {
                 L = null
-            }), check_outros()) : L ? (L.p(F, te), te[0] & 32 && transition_in(L, 1)) : (L = create_if_block_4$c(F), L.c(), transition_in(L, 1), L.m(r, null)), A && A.p && (!b || te[1] & 524288) && update_slot_base(A, G, F, F[50], b ? get_slot_changes(G, F[50], te, null) : get_all_dirty_from_scope(F[50]), null), (!b || te[0] & 8388608) && attr(c, "id", F[23]), (!b || te[0] & 1024 && _ !== (_ = F[10] ? "0" : void 0)) && attr(c, "tabindex", _), (!b || te[0] & 1024 && d !== (d = F[10] ? "region" : void 0)) && attr(c, "role", d), (!b || te[0] & 4195328 && g !== (g = F[10] ? F[22] : void 0)) && attr(c, "aria-label", g), (!b || te[0] & 50331776 && h !== (h = F[7] ? F[25] : F[24])) && attr(c, "aria-labelledby", h), (!b || te[0] & 512) && toggle_class(c, "bx--modal-content--with-form", F[9]), (!b || te[0] & 1024) && toggle_class(c, "bx--modal-scroll-content", F[10]), F[10] ? U || (U = create_if_block_3$h(), U.c(), U.m(n, m)) : U && (U.d(1), U = null), F[5] ? W && (group_outros(), transition_out(W, 1, 1, () => {
-                W = null
-            }), check_outros()) : W ? (W.p(F, te), te[0] & 32 && transition_in(W, 1)) : (W = create_if_block$1c(F), W.c(), transition_in(W, 1), W.m(n, null)), (!b || te[0] & 48 && v !== (v = F[4] ? F[5] ? "alert" : "alertdialog" : "dialog")) && attr(n, "role", v), (!b || te[0] & 8388656 && k !== (k = F[4] && !F[5] ? F[23] : void 0)) && attr(n, "aria-describedby", k), (!b || te[0] & 4194304) && attr(n, "aria-label", F[22]), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--xs", F[2] === "xs"), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--sm", F[2] === "sm"), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--lg", F[2] === "lg"), set_attributes(e, Q = get_spread_update(j, [{
+            }), check_outros()) : L ? (L.p(F, te), te[0] & 32 && transition_in(L, 1)) : (L = create_if_block_4$c(F), L.c(), transition_in(L, 1), L.m(r, null)), A && A.p && (!b || te[1] & 524288) && update_slot_base(A, W, F, F[50], b ? get_slot_changes(W, F[50], te, null) : get_all_dirty_from_scope(F[50]), null), (!b || te[0] & 8388608) && attr(c, "id", F[23]), (!b || te[0] & 1024 && _ !== (_ = F[10] ? "0" : void 0)) && attr(c, "tabindex", _), (!b || te[0] & 1024 && d !== (d = F[10] ? "region" : void 0)) && attr(c, "role", d), (!b || te[0] & 4195328 && g !== (g = F[10] ? F[22] : void 0)) && attr(c, "aria-label", g), (!b || te[0] & 50331776 && h !== (h = F[7] ? F[25] : F[24])) && attr(c, "aria-labelledby", h), (!b || te[0] & 512) && toggle_class(c, "bx--modal-content--with-form", F[9]), (!b || te[0] & 1024) && toggle_class(c, "bx--modal-scroll-content", F[10]), F[10] ? U || (U = create_if_block_3$h(), U.c(), U.m(n, m)) : U && (U.d(1), U = null), F[5] ? G && (group_outros(), transition_out(G, 1, 1, () => {
+                G = null
+            }), check_outros()) : G ? (G.p(F, te), te[0] & 32 && transition_in(G, 1)) : (G = create_if_block$1c(F), G.c(), transition_in(G, 1), G.m(n, null)), (!b || te[0] & 48 && v !== (v = F[4] ? F[5] ? "alert" : "alertdialog" : "dialog")) && attr(n, "role", v), (!b || te[0] & 8388656 && k !== (k = F[4] && !F[5] ? F[23] : void 0)) && attr(n, "aria-describedby", k), (!b || te[0] & 4194304) && attr(n, "aria-label", F[22]), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--xs", F[2] === "xs"), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--sm", F[2] === "sm"), (!b || te[0] & 4) && toggle_class(n, "bx--modal-container--lg", F[2] === "lg"), set_attributes(e, Q = get_spread_update(j, [{
                 role: "presentation"
             }, (!b || te[0] & 262144) && {
                 id: F[18]
             }, te[0] & 268435456 && F[28]])), toggle_class(e, "bx--modal", !0), toggle_class(e, "bx--modal-tall", !F[5]), toggle_class(e, "is-visible", F[0]), toggle_class(e, "bx--modal--danger", F[3])
         },
         i(F) {
-            b || (transition_in(S), transition_in(I), transition_in(B, F), transition_in(L), transition_in(A, F), transition_in(W), b = !0)
+            b || (transition_in(S), transition_in(I), transition_in(B, F), transition_in(L), transition_in(A, F), transition_in(G), b = !0)
         },
         o(F) {
-            transition_out(S), transition_out(I), transition_out(B, F), transition_out(L), transition_out(A, F), transition_out(W), b = !1
+            transition_out(S), transition_out(I), transition_out(B, F), transition_out(L), transition_out(A, F), transition_out(G), b = !1
         },
         d(F) {
-            F && detach(e), S && S.d(), I && I.d(), B && B.d(F), L && L.d(), A && A.d(F), U && U.d(), W && W.d(), t[44](null), t[46](null), E = !1, run_all(w)
+            F && detach(e), S && S.d(), I && I.d(), B && B.d(F), L && L.d(), A && A.d(F), U && U.d(), G && G.d(), t[44](null), t[46](null), E = !1, run_all(w)
         }
     }
 }
 
 function instance$1J(t, e, n) {
     let r, l, a, o;
     const u = ["size", "open", "danger", "alert", "passiveModal", "modalHeading", "modalLabel", "modalAriaLabel", "iconDescription", "hasForm", "hasScrollingContent", "primaryButtonText", "primaryButtonDisabled", "primaryButtonIcon", "shouldSubmitOnEnter", "secondaryButtonText", "secondaryButtons", "selectorPrimaryFocus", "preventCloseOnClickOutside", "id", "ref"];
@@ -2840,24 +2840,24 @@
         {
             primaryButtonIcon: B = void 0
         } = e,
         {
             shouldSubmitOnEnter: L = !0
         } = e,
         {
-            secondaryButtonText: G = ""
+            secondaryButtonText: W = ""
         } = e,
         {
             secondaryButtons: A = []
         } = e,
         {
             selectorPrimaryFocus: U = "[data-modal-primary-focus]"
         } = e,
         {
-            preventCloseOnClickOutside: W = !1
+            preventCloseOnClickOutside: G = !1
         } = e,
         {
             id: j = "ccs-" + Math.random().toString(36)
         } = e,
         {
             ref: Q = null
         } = e;
@@ -2915,15 +2915,15 @@
         ee = H => {
             F("click:button--secondary", {
                 text: H.text
             })
         },
         X = () => {
             F("click:button--secondary", {
-                text: G
+                text: W
             })
         },
         fe = () => {
             F("submit"), F("click:button--primary")
         };
 
     function M(H) {
@@ -2952,26 +2952,26 @@
 `,
                     se = Array.from(Q.querySelectorAll(x));
                 let _e = se.indexOf(document.activeElement);
                 _e === -1 && H.shiftKey && (_e = 0), _e += se.length + (H.shiftKey ? -1 : 1), _e %= se.length, se[_e].focus(), H.preventDefault()
             } else L && H.key === "Enter" && !O && (F("submit"), F("click:button--primary"))
         },
         J = () => {
-            !ae && !W && n(0, h = !1), n(21, ae = !1)
+            !ae && !G && n(0, h = !1), n(21, ae = !1)
         },
         ie = H => {
             H.propertyName === "transform" && F("transitionend", {
                 open: h
             })
         };
     return t.$$set = H => {
-        n(54, e = assign(assign({}, e), exclude_internal_props(H))), n(28, s = compute_rest_props(e, u)), "size" in H && n(2, g = H.size), "open" in H && n(0, h = H.open), "danger" in H && n(3, p = H.danger), "alert" in H && n(4, m = H.alert), "passiveModal" in H && n(5, v = H.passiveModal), "modalHeading" in H && n(6, k = H.modalHeading), "modalLabel" in H && n(7, b = H.modalLabel), "modalAriaLabel" in H && n(29, E = H.modalAriaLabel), "iconDescription" in H && n(8, w = H.iconDescription), "hasForm" in H && n(9, S = H.hasForm), "hasScrollingContent" in H && n(10, I = H.hasScrollingContent), "primaryButtonText" in H && n(11, D = H.primaryButtonText), "primaryButtonDisabled" in H && n(12, O = H.primaryButtonDisabled), "primaryButtonIcon" in H && n(13, B = H.primaryButtonIcon), "shouldSubmitOnEnter" in H && n(14, L = H.shouldSubmitOnEnter), "secondaryButtonText" in H && n(15, G = H.secondaryButtonText), "secondaryButtons" in H && n(16, A = H.secondaryButtons), "selectorPrimaryFocus" in H && n(30, U = H.selectorPrimaryFocus), "preventCloseOnClickOutside" in H && n(17, W = H.preventCloseOnClickOutside), "id" in H && n(18, j = H.id), "ref" in H && n(1, Q = H.ref), "$$scope" in H && n(50, d = H.$$scope)
+        n(54, e = assign(assign({}, e), exclude_internal_props(H))), n(28, s = compute_rest_props(e, u)), "size" in H && n(2, g = H.size), "open" in H && n(0, h = H.open), "danger" in H && n(3, p = H.danger), "alert" in H && n(4, m = H.alert), "passiveModal" in H && n(5, v = H.passiveModal), "modalHeading" in H && n(6, k = H.modalHeading), "modalLabel" in H && n(7, b = H.modalLabel), "modalAriaLabel" in H && n(29, E = H.modalAriaLabel), "iconDescription" in H && n(8, w = H.iconDescription), "hasForm" in H && n(9, S = H.hasForm), "hasScrollingContent" in H && n(10, I = H.hasScrollingContent), "primaryButtonText" in H && n(11, D = H.primaryButtonText), "primaryButtonDisabled" in H && n(12, O = H.primaryButtonDisabled), "primaryButtonIcon" in H && n(13, B = H.primaryButtonIcon), "shouldSubmitOnEnter" in H && n(14, L = H.shouldSubmitOnEnter), "secondaryButtonText" in H && n(15, W = H.secondaryButtonText), "secondaryButtons" in H && n(16, A = H.secondaryButtons), "selectorPrimaryFocus" in H && n(30, U = H.selectorPrimaryFocus), "preventCloseOnClickOutside" in H && n(17, G = H.preventCloseOnClickOutside), "id" in H && n(18, j = H.id), "ref" in H && n(1, Q = H.ref), "$$scope" in H && n(50, d = H.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 1 && set_store_value(Z, c = h, c), t.$$.dirty[0] & 262144 && n(25, r = `bx--modal-header__label--modal-${j}`), t.$$.dirty[0] & 262144 && n(24, l = `bx--modal-header__heading--modal-${j}`), t.$$.dirty[0] & 262144 && n(23, a = `bx--modal-body--${j}`), n(22, o = b || e["aria-label"] || E || k)
-    }, e = exclude_internal_props(e), [h, Q, g, p, m, v, k, b, w, S, I, D, O, B, L, G, A, W, j, te, Y, ae, o, a, l, r, F, Z, s, E, U, _, K, ce, z, V, $, re, ue, P, q, ee, X, fe, M, y, T, N, J, ie, d]
+    }, e = exclude_internal_props(e), [h, Q, g, p, m, v, k, b, w, S, I, D, O, B, L, W, A, G, j, te, Y, ae, o, a, l, r, F, Z, s, E, U, _, K, ce, z, V, $, re, ue, P, q, ee, X, fe, M, y, T, N, J, ie, d]
 }
 class Modal extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1J, create_fragment$1J, safe_not_equal, {
             size: 2,
             open: 0,
             danger: 3,
@@ -7248,21 +7248,21 @@
         } = e;
     const O = compute_slots(I);
     let {
         headers: B = []
     } = e, {
         rows: L = []
     } = e, {
-        size: G = void 0
+        size: W = void 0
     } = e, {
         title: A = ""
     } = e, {
         description: U = ""
     } = e, {
-        zebra: W = !1
+        zebra: G = !1
     } = e, {
         sortable: j = !1
     } = e, {
         sortKey: Q = null
     } = e, {
         sortDirection: F = "none"
     } = e, {
@@ -7394,15 +7394,15 @@
         Ce = le => {
             ae.includes(le.id) || n(23, y = le.id)
         },
         Re = le => {
             ae.includes(le.id) || n(23, y = null)
         };
     return t.$$set = le => {
-        e = assign(assign({}, e), exclude_internal_props(le)), n(37, w = compute_rest_props(e, E)), "headers" in le && n(6, B = le.headers), "rows" in le && n(39, L = le.rows), "size" in le && n(7, G = le.size), "title" in le && n(8, A = le.title), "description" in le && n(9, U = le.description), "zebra" in le && n(10, W = le.zebra), "sortable" in le && n(11, j = le.sortable), "sortKey" in le && n(0, Q = le.sortKey), "sortDirection" in le && n(1, F = le.sortDirection), "expandable" in le && n(4, te = le.expandable), "batchExpansion" in le && n(12, Y = le.batchExpansion), "expandedRowIds" in le && n(2, oe = le.expandedRowIds), "nonExpandableRowIds" in le && n(13, ae = le.nonExpandableRowIds), "radio" in le && n(14, C = le.radio), "selectable" in le && n(5, Z = le.selectable), "batchSelection" in le && n(15, K = le.batchSelection), "selectedRowIds" in le && n(3, ce = le.selectedRowIds), "nonSelectableRowIds" in le && n(16, z = le.nonSelectableRowIds), "stickyHeader" in le && n(17, V = le.stickyHeader), "useStaticWidth" in le && n(18, $ = le.useStaticWidth), "pageSize" in le && n(40, re = le.pageSize), "page" in le && n(41, ue = le.page), "$$scope" in le && n(62, D = le.$$scope)
+        e = assign(assign({}, e), exclude_internal_props(le)), n(37, w = compute_rest_props(e, E)), "headers" in le && n(6, B = le.headers), "rows" in le && n(39, L = le.rows), "size" in le && n(7, W = le.size), "title" in le && n(8, A = le.title), "description" in le && n(9, U = le.description), "zebra" in le && n(10, G = le.zebra), "sortable" in le && n(11, j = le.sortable), "sortKey" in le && n(0, Q = le.sortKey), "sortDirection" in le && n(1, F = le.sortDirection), "expandable" in le && n(4, te = le.expandable), "batchExpansion" in le && n(12, Y = le.batchExpansion), "expandedRowIds" in le && n(2, oe = le.expandedRowIds), "nonExpandableRowIds" in le && n(13, ae = le.nonExpandableRowIds), "radio" in le && n(14, C = le.radio), "selectable" in le && n(5, Z = le.selectable), "batchSelection" in le && n(15, K = le.batchSelection), "selectedRowIds" in le && n(3, ce = le.selectedRowIds), "nonSelectableRowIds" in le && n(16, z = le.nonSelectableRowIds), "stickyHeader" in le && n(17, V = le.stickyHeader), "useStaticWidth" in le && n(18, $ = le.useStaticWidth), "pageSize" in le && n(40, re = le.pageSize), "page" in le && n(41, ue = le.page), "$$scope" in le && n(62, D = le.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 64 && n(32, r = B.reduce((le, pe) => ({
             ...le,
             [pe.key]: pe.key
         }), {})), t.$$.dirty[0] & 4 && n(31, l = oe.reduce((le, pe) => ({
             ...le,
             [pe]: !0
@@ -7415,15 +7415,15 @@
         })), le), {})), t.$$.dirty[1] & 256 && set_store_value(X, S = L, S), t.$$.dirty[1] & 65536 && n(46, a = S.map(le => le.id)), t.$$.dirty[0] & 8192 | t.$$.dirty[1] & 32768 && n(20, o = a.filter(le => !ae.includes(le))), t.$$.dirty[0] & 65536 | t.$$.dirty[1] & 32768 && n(21, u = a.filter(le => !z.includes(le))), t.$$.dirty[0] & 2097160 && n(30, s = u.length > 0 && ce.length === u.length), t.$$.dirty[0] & 2097160 && n(29, c = ce.length > 0 && ce.length < u.length), t.$$.dirty[0] & 1052676 && Y && (n(4, te = !0), n(22, M = oe.length === o.length)), t.$$.dirty[0] & 49152 && (C || K) && n(5, Z = !0), t.$$.dirty[1] & 65536 && n(42, g = [...S]), t.$$.dirty[0] & 2 && n(43, h = F === "ascending"), t.$$.dirty[0] & 2049 && n(19, p = j && Q != null), t.$$.dirty[0] & 65 && n(44, m = B.find(le => le.key === Q)), t.$$.dirty[0] & 524291 | t.$$.dirty[1] & 77824 && p && (F === "none" ? n(42, g = S) : n(42, g = [...S].sort((le, pe) => {
             const me = fe(h ? le : pe, Q),
                 ye = fe(h ? pe : le, Q);
             return m != null && m.sort ? m.sort(me, ye) : typeof me == "number" && typeof ye == "number" ? me - ye : [me, ye].every(Ee => !Ee && Ee !== 0) ? 0 : !me && me !== 0 ? h ? 1 : -1 : !ye && ye !== 0 ? h ? -1 : 1 : me.toString().localeCompare(ye.toString(), "en", {
                 numeric: !0
             })
         }))), t.$$.dirty[1] & 67072 && n(27, v = N(S, ue, re)), t.$$.dirty[1] & 3584 && n(26, k = N(g, ue, re)), t.$$.dirty[0] & 64 && n(25, b = B.some(le => le.width || le.minWidth))
-    }, [Q, F, oe, ce, te, Z, B, G, A, U, W, j, Y, ae, C, K, z, V, $, p, o, u, M, y, T, b, k, v, d, c, s, l, r, P, q, X, J, w, O, L, re, ue, g, h, m, _, a, S, I, ie, H, x, se, _e, he, ge, ke, we, be, Se, Ce, Re, D]
+    }, [Q, F, oe, ce, te, Z, B, W, A, U, G, j, Y, ae, C, K, z, V, $, p, o, u, M, y, T, b, k, v, d, c, s, l, r, P, q, X, J, w, O, L, re, ue, g, h, m, _, a, S, I, ie, H, x, se, _e, he, ge, ke, we, be, Se, Ce, Re, D]
 }
 class DataTable extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1w, create_fragment$1w, safe_not_equal, {
             headers: 6,
             rows: 39,
             size: 7,
@@ -8085,22 +8085,22 @@
         }
     }
 }
 
 function create_fragment$1s(t) {
     let e, n, r, l, a, o, u, s, c, _, d, g, h, p, m, v, k, b, E, w, S, I, D, O, B = t[16] && create_if_block_10$2(t),
         L = !t[16] && (t[9] || t[26].labelText) && create_if_block_9$3(t);
-    const G = [create_if_block_6$4, create_else_block$l],
+    const W = [create_if_block_6$4, create_else_block$l],
         A = [];
 
     function U(C, Z) {
         return C[17] ? 0 : 1
     }
-    o = U(t), u = A[o] = G[o](t);
-    let W = [{
+    o = U(t), u = A[o] = W[o](t);
+    let G = [{
             "data-invalid": _ = t[21] || void 0
         }, {
             "aria-invalid": d = t[21] || void 0
         }, {
             "data-warn": g = t[13] || void 0
         }, {
             "aria-describedby": h = t[21] ? t[19] : t[13] ? t[18] : t[6] ? t[20] : void 0
@@ -8114,15 +8114,15 @@
             placeholder: t[3]
         }, {
             required: t[15]
         }, {
             readOnly: t[17]
         }, t[25]],
         j = {};
-    for (let C = 0; C < W.length; C += 1) j = assign(j, W[C]);
+    for (let C = 0; C < G.length; C += 1) j = assign(j, G[C]);
     let Q = t[22] && create_if_block_5$6(),
         F = t[22] && !t[16] && t[11] && create_if_block_4$a(t),
         te = t[22] && !t[16] && t[13] && create_if_block_3$f(t),
         Y = !t[11] && !t[13] && !t[22] && !t[16] && t[6] && create_if_block_2$h(t),
         oe = !t[22] && t[11] && create_if_block_1$n(t),
         ae = !t[22] && !t[11] && t[13] && create_if_block$10(t);
     return {
@@ -8137,15 +8137,15 @@
                 B = null
             }), check_outros()), !C[16] && (C[9] || C[26].labelText) ? L ? (L.p(C, Z), Z[0] & 67174912 && transition_in(L, 1)) : (L = create_if_block_9$3(C), L.c(), transition_in(L, 1), L.m(e, r)) : L && (group_outros(), transition_out(L, 1, 1, () => {
                 L = null
             }), check_outros());
             let K = o;
             o = U(C), o === K ? A[o].p(C, Z) : (group_outros(), transition_out(A[K], 1, 1, () => {
                 A[K] = null
-            }), check_outros(), u = A[o], u ? u.p(C, Z) : (u = A[o] = G[o](C), u.c()), transition_in(u, 1), u.m(a, s)), set_attributes(c, j = get_spread_update(W, [(!I || Z[0] & 2097152 && _ !== (_ = C[21] || void 0)) && {
+            }), check_outros(), u = A[o], u ? u.p(C, Z) : (u = A[o] = W[o](C), u.c()), transition_in(u, 1), u.m(a, s)), set_attributes(c, j = get_spread_update(G, [(!I || Z[0] & 2097152 && _ !== (_ = C[21] || void 0)) && {
                 "data-invalid": _
             }, (!I || Z[0] & 2097152 && d !== (d = C[21] || void 0)) && {
                 "aria-invalid": d
             }, (!I || Z[0] & 8192 && g !== (g = C[13] || void 0)) && {
                 "data-warn": g
             }, (!I || Z[0] & 3940416 && h !== (h = C[21] ? C[19] : C[13] ? C[18] : C[6] ? C[20] : void 0)) && {
                 "aria-describedby": h
@@ -8209,21 +8209,21 @@
     } = e, {
         invalidText: O = ""
     } = e, {
         warn: B = !1
     } = e, {
         warnText: L = ""
     } = e, {
-        ref: G = null
+        ref: W = null
     } = e, {
         required: A = !1
     } = e, {
         inline: U = !1
     } = e, {
-        readonly: W = !1
+        readonly: G = !1
     } = e;
     const j = getContext("Form"),
         Q = createEventDispatcher();
 
     function F(P) {
         return c.type !== "number" ? P : P != "" ? Number(P) : null
     }
@@ -8268,26 +8268,26 @@
 
     function $(P) {
         bubble.call(this, t, P)
     }
 
     function re(P) {
         binding_callbacks[P ? "unshift" : "push"](() => {
-            G = P, n(1, G)
+            W = P, n(1, W)
         })
     }
 
     function ue() {
         p = this.value, n(0, p)
     }
     return t.$$set = P => {
-        e = assign(assign({}, e), exclude_internal_props(P)), n(25, c = compute_rest_props(e, s)), "size" in P && n(2, h = P.size), "value" in P && n(0, p = P.value), "placeholder" in P && n(3, m = P.placeholder), "light" in P && n(4, v = P.light), "disabled" in P && n(5, k = P.disabled), "helperText" in P && n(6, b = P.helperText), "id" in P && n(7, E = P.id), "name" in P && n(8, w = P.name), "labelText" in P && n(9, S = P.labelText), "hideLabel" in P && n(10, I = P.hideLabel), "invalid" in P && n(11, D = P.invalid), "invalidText" in P && n(12, O = P.invalidText), "warn" in P && n(13, B = P.warn), "warnText" in P && n(14, L = P.warnText), "ref" in P && n(1, G = P.ref), "required" in P && n(15, A = P.required), "inline" in P && n(16, U = P.inline), "readonly" in P && n(17, W = P.readonly), "$$scope" in P && n(27, d = P.$$scope)
+        e = assign(assign({}, e), exclude_internal_props(P)), n(25, c = compute_rest_props(e, s)), "size" in P && n(2, h = P.size), "value" in P && n(0, p = P.value), "placeholder" in P && n(3, m = P.placeholder), "light" in P && n(4, v = P.light), "disabled" in P && n(5, k = P.disabled), "helperText" in P && n(6, b = P.helperText), "id" in P && n(7, E = P.id), "name" in P && n(8, w = P.name), "labelText" in P && n(9, S = P.labelText), "hideLabel" in P && n(10, I = P.hideLabel), "invalid" in P && n(11, D = P.invalid), "invalidText" in P && n(12, O = P.invalidText), "warn" in P && n(13, B = P.warn), "warnText" in P && n(14, L = P.warnText), "ref" in P && n(1, W = P.ref), "required" in P && n(15, A = P.required), "inline" in P && n(16, U = P.inline), "readonly" in P && n(17, G = P.readonly), "$$scope" in P && n(27, d = P.$$scope)
     }, t.$$.update = () => {
-        t.$$.dirty[0] & 133120 && n(21, l = D && !W), t.$$.dirty[0] & 128 && n(20, a = `helper-${E}`), t.$$.dirty[0] & 128 && n(19, o = `error-${E}`), t.$$.dirty[0] & 128 && n(18, u = `warn-${E}`)
-    }, n(22, r = !!j && j.isFluid), [p, G, h, m, v, k, b, E, w, S, I, D, O, B, L, A, U, W, u, o, a, l, r, te, Y, c, g, d, _, oe, ae, C, Z, K, ce, z, V, $, re, ue]
+        t.$$.dirty[0] & 133120 && n(21, l = D && !G), t.$$.dirty[0] & 128 && n(20, a = `helper-${E}`), t.$$.dirty[0] & 128 && n(19, o = `error-${E}`), t.$$.dirty[0] & 128 && n(18, u = `warn-${E}`)
+    }, n(22, r = !!j && j.isFluid), [p, W, h, m, v, k, b, E, w, S, I, D, O, B, L, A, U, G, u, o, a, l, r, te, Y, c, g, d, _, oe, ae, C, Z, K, ce, z, V, $, re, ue]
 }
 class TextInput extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1s, create_fragment$1s, safe_not_equal, {
             size: 2,
             value: 0,
             placeholder: 3,
@@ -8897,51 +8897,51 @@
         w = create_slot(E, t, t[14], get_subtitle_slot_context$1),
         S = w || fallback_block_1$5(t),
         I = t[15].caption,
         D = create_slot(I, t, t[14], get_caption_slot_context),
         O = D || fallback_block$d(t),
         B = t[15].default,
         L = create_slot(B, t, t[14], null);
-    let G = !t[8] && create_if_block_1$m(t),
+    let W = !t[8] && create_if_block_1$m(t),
         A = [{
             role: t[2]
         }, {
             kind: t[0]
         }, t[12], {
             style: g = "" + ((t[9] && "width: 100%;") + t[12].style)
         }],
         U = {};
-    for (let W = 0; W < A.length; W += 1) U = assign(U, A[W]);
+    for (let G = 0; G < A.length; G += 1) U = assign(U, A[G]);
     return {
         c() {
-            e = element("div"), create_component(n.$$.fragment), r = space(), l = element("div"), a = element("h3"), b && b.c(), o = space(), u = element("div"), S && S.c(), s = space(), c = element("div"), O && O.c(), _ = space(), L && L.c(), d = space(), G && G.c(), toggle_class(a, "bx--toast-notification__title", !0), toggle_class(u, "bx--toast-notification__subtitle", !0), toggle_class(c, "bx--toast-notification__caption", !0), toggle_class(l, "bx--toast-notification__details", !0), set_attributes(e, U), toggle_class(e, "bx--toast-notification", !0), toggle_class(e, "bx--toast-notification--low-contrast", t[1]), toggle_class(e, "bx--toast-notification--error", t[0] === "error"), toggle_class(e, "bx--toast-notification--info", t[0] === "info"), toggle_class(e, "bx--toast-notification--info-square", t[0] === "info-square"), toggle_class(e, "bx--toast-notification--success", t[0] === "success"), toggle_class(e, "bx--toast-notification--warning", t[0] === "warning"), toggle_class(e, "bx--toast-notification--warning-alt", t[0] === "warning-alt")
+            e = element("div"), create_component(n.$$.fragment), r = space(), l = element("div"), a = element("h3"), b && b.c(), o = space(), u = element("div"), S && S.c(), s = space(), c = element("div"), O && O.c(), _ = space(), L && L.c(), d = space(), W && W.c(), toggle_class(a, "bx--toast-notification__title", !0), toggle_class(u, "bx--toast-notification__subtitle", !0), toggle_class(c, "bx--toast-notification__caption", !0), toggle_class(l, "bx--toast-notification__details", !0), set_attributes(e, U), toggle_class(e, "bx--toast-notification", !0), toggle_class(e, "bx--toast-notification--low-contrast", t[1]), toggle_class(e, "bx--toast-notification--error", t[0] === "error"), toggle_class(e, "bx--toast-notification--info", t[0] === "info"), toggle_class(e, "bx--toast-notification--info-square", t[0] === "info-square"), toggle_class(e, "bx--toast-notification--success", t[0] === "success"), toggle_class(e, "bx--toast-notification--warning", t[0] === "warning"), toggle_class(e, "bx--toast-notification--warning-alt", t[0] === "warning-alt")
         },
-        m(W, j) {
-            insert(W, e, j), mount_component(n, e, null), append(e, r), append(e, l), append(l, a), b && b.m(a, null), append(l, o), append(l, u), S && S.m(u, null), append(l, s), append(l, c), O && O.m(c, null), append(l, _), L && L.m(l, null), append(e, d), G && G.m(e, null), h = !0, p || (m = [listen(e, "click", t[16]), listen(e, "mouseover", t[17]), listen(e, "mouseenter", t[18]), listen(e, "mouseleave", t[19])], p = !0)
+        m(G, j) {
+            insert(G, e, j), mount_component(n, e, null), append(e, r), append(e, l), append(l, a), b && b.m(a, null), append(l, o), append(l, u), S && S.m(u, null), append(l, s), append(l, c), O && O.m(c, null), append(l, _), L && L.m(l, null), append(e, d), W && W.m(e, null), h = !0, p || (m = [listen(e, "click", t[16]), listen(e, "mouseover", t[17]), listen(e, "mouseenter", t[18]), listen(e, "mouseleave", t[19])], p = !0)
         },
-        p(W, j) {
+        p(G, j) {
             const Q = {};
-            j & 1 && (Q.kind = W[0]), j & 64 && (Q.iconDescription = W[6]), n.$set(Q), k ? k.p && (!h || j & 16384) && update_slot_base(k, v, W, W[14], h ? get_slot_changes(v, W[14], j, get_title_slot_changes$2) : get_all_dirty_from_scope(W[14]), get_title_slot_context$2) : b && b.p && (!h || j & 8) && b.p(W, h ? j : -1), w ? w.p && (!h || j & 16384) && update_slot_base(w, E, W, W[14], h ? get_slot_changes(E, W[14], j, get_subtitle_slot_changes$1) : get_all_dirty_from_scope(W[14]), get_subtitle_slot_context$1) : S && S.p && (!h || j & 16) && S.p(W, h ? j : -1), D ? D.p && (!h || j & 16384) && update_slot_base(D, I, W, W[14], h ? get_slot_changes(I, W[14], j, get_caption_slot_changes) : get_all_dirty_from_scope(W[14]), get_caption_slot_context) : O && O.p && (!h || j & 32) && O.p(W, h ? j : -1), L && L.p && (!h || j & 16384) && update_slot_base(L, B, W, W[14], h ? get_slot_changes(B, W[14], j, null) : get_all_dirty_from_scope(W[14]), null), W[8] ? G && (group_outros(), transition_out(G, 1, 1, () => {
-                G = null
-            }), check_outros()) : G ? (G.p(W, j), j & 256 && transition_in(G, 1)) : (G = create_if_block_1$m(W), G.c(), transition_in(G, 1), G.m(e, null)), set_attributes(e, U = get_spread_update(A, [(!h || j & 4) && {
-                role: W[2]
+            j & 1 && (Q.kind = G[0]), j & 64 && (Q.iconDescription = G[6]), n.$set(Q), k ? k.p && (!h || j & 16384) && update_slot_base(k, v, G, G[14], h ? get_slot_changes(v, G[14], j, get_title_slot_changes$2) : get_all_dirty_from_scope(G[14]), get_title_slot_context$2) : b && b.p && (!h || j & 8) && b.p(G, h ? j : -1), w ? w.p && (!h || j & 16384) && update_slot_base(w, E, G, G[14], h ? get_slot_changes(E, G[14], j, get_subtitle_slot_changes$1) : get_all_dirty_from_scope(G[14]), get_subtitle_slot_context$1) : S && S.p && (!h || j & 16) && S.p(G, h ? j : -1), D ? D.p && (!h || j & 16384) && update_slot_base(D, I, G, G[14], h ? get_slot_changes(I, G[14], j, get_caption_slot_changes) : get_all_dirty_from_scope(G[14]), get_caption_slot_context) : O && O.p && (!h || j & 32) && O.p(G, h ? j : -1), L && L.p && (!h || j & 16384) && update_slot_base(L, B, G, G[14], h ? get_slot_changes(B, G[14], j, null) : get_all_dirty_from_scope(G[14]), null), G[8] ? W && (group_outros(), transition_out(W, 1, 1, () => {
+                W = null
+            }), check_outros()) : W ? (W.p(G, j), j & 256 && transition_in(W, 1)) : (W = create_if_block_1$m(G), W.c(), transition_in(W, 1), W.m(e, null)), set_attributes(e, U = get_spread_update(A, [(!h || j & 4) && {
+                role: G[2]
             }, (!h || j & 1) && {
-                kind: W[0]
-            }, j & 4096 && W[12], (!h || j & 4608 && g !== (g = "" + ((W[9] && "width: 100%;") + W[12].style))) && {
+                kind: G[0]
+            }, j & 4096 && G[12], (!h || j & 4608 && g !== (g = "" + ((G[9] && "width: 100%;") + G[12].style))) && {
                 style: g
-            }])), toggle_class(e, "bx--toast-notification", !0), toggle_class(e, "bx--toast-notification--low-contrast", W[1]), toggle_class(e, "bx--toast-notification--error", W[0] === "error"), toggle_class(e, "bx--toast-notification--info", W[0] === "info"), toggle_class(e, "bx--toast-notification--info-square", W[0] === "info-square"), toggle_class(e, "bx--toast-notification--success", W[0] === "success"), toggle_class(e, "bx--toast-notification--warning", W[0] === "warning"), toggle_class(e, "bx--toast-notification--warning-alt", W[0] === "warning-alt")
+            }])), toggle_class(e, "bx--toast-notification", !0), toggle_class(e, "bx--toast-notification--low-contrast", G[1]), toggle_class(e, "bx--toast-notification--error", G[0] === "error"), toggle_class(e, "bx--toast-notification--info", G[0] === "info"), toggle_class(e, "bx--toast-notification--info-square", G[0] === "info-square"), toggle_class(e, "bx--toast-notification--success", G[0] === "success"), toggle_class(e, "bx--toast-notification--warning", G[0] === "warning"), toggle_class(e, "bx--toast-notification--warning-alt", G[0] === "warning-alt")
         },
-        i(W) {
-            h || (transition_in(n.$$.fragment, W), transition_in(b, W), transition_in(S, W), transition_in(O, W), transition_in(L, W), transition_in(G), h = !0)
+        i(G) {
+            h || (transition_in(n.$$.fragment, G), transition_in(b, G), transition_in(S, G), transition_in(O, G), transition_in(L, G), transition_in(W), h = !0)
         },
-        o(W) {
-            transition_out(n.$$.fragment, W), transition_out(b, W), transition_out(S, W), transition_out(O, W), transition_out(L, W), transition_out(G), h = !1
+        o(G) {
+            transition_out(n.$$.fragment, G), transition_out(b, G), transition_out(S, G), transition_out(O, G), transition_out(L, G), transition_out(W), h = !1
         },
-        d(W) {
-            W && detach(e), destroy_component(n), b && b.d(W), S && S.d(W), O && O.d(W), L && L.d(W), G && G.d(), p = !1, run_all(m)
+        d(G) {
+            G && detach(e), destroy_component(n), b && b.d(G), S && S.d(G), O && O.d(G), L && L.d(G), W && W.d(), p = !1, run_all(m)
         }
     }
 }
 
 function fallback_block_2$3(t) {
     let e;
     return {
@@ -9806,15 +9806,15 @@
 function create_if_block$P(t) {
     let e, n;
     return e = new Button$1({
         props: {
             icon: DirectionLoopLeftFilled,
             iconDescription: "Back to History"
         }
-    }), e.$on("click", t[8]), {
+    }), e.$on("click", t[7]), {
         c() {
             create_component(e.$$.fragment)
         },
         m(r, l) {
             mount_component(e, r, l), n = !0
         },
         p: noop,
@@ -9857,50 +9857,47 @@
             I && detach(e), destroy_component(l), S && S.d()
         }
     }
 }
 
 function instance$1d(t, e, n) {
     let r;
-    component_subscribe(t, storedGlobalChanged, h => n(6, r = h));
+    component_subscribe(t, storedGlobalChanged, g => n(6, r = g));
     let {
         pipelineName: l
     } = e, {
         pipelineDesc: a = void 0
     } = e, {
         backToHistory: o = !1
     } = e, {
         configfile: u = void 0
     } = e, {
-        histories: s
-    } = e, {
-        isRunning: c = !1
-    } = e, _ = "0.0.0";
+        isRunning: s = !1
+    } = e, c = "0.0.0";
     onMount(async function() {
         try {
-            n(5, _ = await fetchAPI("/api/version", {}, "text"))
+            n(5, c = await fetchAPI("/api/version", {}, "text"))
         } catch {
-            n(5, _ = '<font style="color:red">Error</font>')
+            n(5, c = '<font style="color:red">Error</font>')
         }
     });
-    const g = () => {
-        c ? alert("Please wait until the pipeline is finished or stop it before switching to a different configuration") : (!r || confirm("You have unsaved changes. Are you sure to discard them?")) && (n(0, u = void 0), storedConfigfile.set(void 0))
+    const d = () => {
+        s ? alert("Please wait until the pipeline is finished or stop it before switching to a different configuration") : (!r || confirm("You have unsaved changes. Are you sure to discard them?")) && (n(0, u = void 0), storedConfigfile.set(void 0))
     };
-    return t.$$set = h => {
-        "pipelineName" in h && n(1, l = h.pipelineName), "pipelineDesc" in h && n(2, a = h.pipelineDesc), "backToHistory" in h && n(3, o = h.backToHistory), "configfile" in h && n(0, u = h.configfile), "histories" in h && n(7, s = h.histories), "isRunning" in h && n(4, c = h.isRunning)
-    }, [u, l, a, o, c, _, r, s, g]
+    return t.$$set = g => {
+        "pipelineName" in g && n(1, l = g.pipelineName), "pipelineDesc" in g && n(2, a = g.pipelineDesc), "backToHistory" in g && n(3, o = g.backToHistory), "configfile" in g && n(0, u = g.configfile), "isRunning" in g && n(4, s = g.isRunning)
+    }, [u, l, a, o, s, c, r, d]
 }
 class Header extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1d, create_fragment$1d, safe_not_equal, {
             pipelineName: 1,
             pipelineDesc: 2,
             backToHistory: 3,
             configfile: 0,
-            histories: 7,
             isRunning: 4
         })
     }
 }
 const History_svelte_svelte_type_style_lang = "";
 
 function create_if_block_1$l(t) {
@@ -10226,15 +10223,14 @@
     }
 }
 
 function create_fragment$1c(t) {
     let e, n, r, l, a, o, u, s, c, _, d, g, h, p, m, v, k, b, E, w, S = t[3] && create_if_block_1$l(t);
     return r = new Header({
         props: {
-            histories: t[0],
             pipelineName: t[7]
         }
     }), o = new Button$1({
         props: {
             kind: "primary",
             icon: GroupObjectsNew,
             iconDescription: "Create a New Instance",
@@ -10301,30 +10297,28 @@
             S && S.m(I, D), insert(I, e, D), insert(I, n, D), mount_component(r, n, null), append(n, l), append(n, a), mount_component(o, a, null), append(a, u), mount_component(s, a, null), append(a, c), mount_component(_, a, null), append(a, d), append(a, g), append(a, h), append(a, p), append(n, m), append(n, v), mount_component(k, v, null), b = !0, E || (w = listen(p, "change", t[13]), E = !0)
         },
         p(I, [D]) {
             I[3] ? S ? (S.p(I, D), D & 8 && transition_in(S, 1)) : (S = create_if_block_1$l(I), S.c(), transition_in(S, 1), S.m(e.parentNode, e)) : S && (group_outros(), transition_out(S, 1, 1, () => {
                 S = null
             }), check_outros());
             const O = {};
-            D & 1 && (O.histories = I[0]), r.$set(O);
-            const B = {};
-            D & 4194304 && (B.$$scope = {
+            D & 4194304 && (O.$$scope = {
                 dirty: D,
                 ctx: I
-            }), o.$set(B);
-            const L = {};
-            D & 32 && (L.disabled = I[5]), D & 4194304 && (L.$$scope = {
+            }), o.$set(O);
+            const B = {};
+            D & 32 && (B.disabled = I[5]), D & 4194304 && (B.$$scope = {
                 dirty: D,
                 ctx: I
-            }), s.$set(L);
-            const G = {};
-            D & 4 && (G.description = `For pipeline: ${I[2]}`), D & 64 && (G.rows = I[6]), D & 6291475 && (G.$$scope = {
+            }), s.$set(B);
+            const L = {};
+            D & 4 && (L.description = `For pipeline: ${I[2]}`), D & 64 && (L.rows = I[6]), D & 6291475 && (L.$$scope = {
                 dirty: D,
                 ctx: I
-            }), k.$set(G)
+            }), k.$set(L)
         },
         i(I) {
             b || (transition_in(S), transition_in(r.$$.fragment, I), transition_in(o.$$.fragment, I), transition_in(s.$$.fragment, I), transition_in(_.$$.fragment, I), transition_in(k.$$.fragment, I), b = !0)
         },
         o(I) {
             transition_out(S), transition_out(r.$$.fragment, I), transition_out(o.$$.fragment, I), transition_out(s.$$.fragment, I), transition_out(_.$$.fragment, I), transition_out(k.$$.fragment, I), b = !1
         },
@@ -10379,46 +10373,46 @@
                     })
                 })
             } catch (L) {
                 n(3, u = `<strong>Failed to delete history:</strong> <br /><br /><pre>${L}</pre>`)
             } finally {
                 n(4, s = void 0)
             }
-            u || n(0, a = a.filter((L, G) => G !== O))
+            u || n(0, a = a.filter((L, W) => W !== O))
         }, h = async (O, B) => {
             const L = prompt(`Please enter a new name for this configuration: 
 
 ` + B);
             if (!L) {
                 n(4, s = void 0);
                 return
             }
-            let G;
+            let W;
             try {
-                if (G = await fetchAPI("/api/history/saveas", {
+                if (W = await fetchAPI("/api/history/saveas", {
                         method: "POST",
                         headers: {
                             "Content-Type": "application/json"
                         },
                         body: JSON.stringify({
                             configfile: B,
                             new_name: L
                         })
-                    }), G.error) throw new Error(G.error)
+                    }), W.error) throw new Error(W.error)
             } catch (A) {
                 n(3, u = `<strong>Failed to save configuration with a new name:</strong> <br /><br /><pre>${A}</pre>`)
             } finally {
                 n(4, s = void 0)
             }
             if (!u) {
-                const A = a.find(U => U.configfile === G.configfile);
-                A ? n(0, a = [...a.filter(U => U.configfile !== G.configfile), {
+                const A = a.find(U => U.configfile === W.configfile);
+                A ? n(0, a = [...a.filter(U => U.configfile !== W.configfile), {
                     ...A,
-                    ...G
-                }]) : n(0, a = [...a, G])
+                    ...W
+                }]) : n(0, a = [...a, W])
             }
         }, p = async (O, B) => {
             let L;
             try {
                 L = await fetchAPI("/api/history/download", {
                     method: "POST",
                     headers: {
@@ -10429,43 +10423,43 @@
                     })
                 }, "blob")
             } catch (U) {
                 n(3, u = `<strong>Failed to download the schema file:</strong> <br /><br /><pre>${U}</pre>`)
             } finally {
                 n(4, s = void 0)
             }
-            const G = new Blob([L], {
+            const W = new Blob([L], {
                     type: "text/json"
                 }),
                 A = document.createElement("a");
-            A.href = URL.createObjectURL(G), A.download = a[O].name + ".schema.json", document.body.appendChild(A), A.click(), A.remove()
+            A.href = URL.createObjectURL(W), A.download = a[O].name + ".schema.json", document.body.appendChild(A), A.click(), A.remove()
         }, m = () => {
             const O = document.getElementById("schema_file");
             O.value = "", O.click()
         }, v = async O => {
             n(5, c = !0);
             const B = O.target;
             if (B.files.length === 0) {
                 n(5, c = !1);
                 return
             }
             const L = new FormData;
             L.append("schema_file", B.files[0]);
-            let G;
+            let W;
             try {
-                if (G = await fetchAPI("/api/history/upload", {
+                if (W = await fetchAPI("/api/history/upload", {
                         method: "POST",
                         body: L
-                    }), G.error) throw new Error(G.error)
+                    }), W.error) throw new Error(W.error)
             } catch (A) {
                 n(3, u = `<strong>Failed to upload the schema file:</strong> <br /><br /><pre>${A}</pre>`)
             } finally {
                 n(5, c = !1)
             }
-            u || n(0, a = [...a, G])
+            u || n(0, a = [...a, W])
         }, k = async O => {
             if (O.key !== "Enter") return;
             if (c) {
                 n(3, u = "Please wait for the previous upload to finish.");
                 return
             }
             const B = O.target.value;
@@ -10478,16 +10472,16 @@
                         headers: {
                             "Content-Type": "application/json"
                         },
                         body: JSON.stringify({
                             url: B
                         })
                     }), L.error) throw new Error(L.error)
-            } catch (G) {
-                n(3, u = `<strong>Failed to upload the schema file:</strong> <br /><br /><pre>${G}</pre>`)
+            } catch (W) {
+                n(3, u = `<strong>Failed to upload the schema file:</strong> <br /><br /><pre>${W}</pre>`)
             } finally {
                 n(5, c = !1)
             }
             u || (n(0, a = [...a, L]), O.target.value = "")
         }, b = () => {
             n(3, u = void 0)
         }, E = () => {
@@ -10766,45 +10760,45 @@
             n(14, A = ae), await tick();
             const Z = L == null ? void 0 : L.querySelectorAll("[role='tab']")[A];
             Z == null || Z.focus()
         }
     }), afterUpdate(() => {
         n(12, h = A), U > -1 && U !== A && b("change", A), U = A
     });
-    let G = !0,
+    let W = !0,
         A = h,
         U = -1;
 
-    function W(oe) {
+    function G(oe) {
         bubble.call(this, t, oe)
     }
 
     function j(oe) {
         bubble.call(this, t, oe)
     }
     const Q = () => {
-            n(5, G = !G)
+            n(5, W = !W)
         },
         F = () => {
-            n(5, G = !G)
+            n(5, W = !W)
         },
         te = () => {
-            n(5, G = !G)
+            n(5, W = !W)
         };
 
     function Y(oe) {
         binding_callbacks[oe ? "unshift" : "push"](() => {
             L = oe, n(4, L)
         })
     }
     return t.$$set = oe => {
         n(11, e = assign(assign({}, e), exclude_internal_props(oe))), n(10, o = compute_rest_props(e, a)), "selected" in oe && n(12, h = oe.selected), "type" in oe && n(0, p = oe.type), "autoWidth" in oe && n(13, m = oe.autoWidth), "iconDescription" in oe && n(1, v = oe.iconDescription), "triggerHref" in oe && n(2, k = oe.triggerHref), "$$scope" in oe && n(19, g = oe.$$scope)
     }, t.$$.update = () => {
-        t.$$.dirty[0] & 4096 && n(14, A = h), t.$$.dirty[0] & 278528 && n(3, r = c[A] || void 0), t.$$.dirty[0] & 147456 && n(15, l = s[A] || void 0), t.$$.dirty[0] & 32776 && (r && I.set(r.id), l && B.set(l.id)), t.$$.dirty[0] & 65536 && u && n(5, G = !0), t.$$.dirty[0] & 8192 && S.set(m)
-    }, e = exclude_internal_props(e), [p, v, k, r, L, G, E, w, I, D, o, e, h, m, A, l, u, s, c, g, d, W, j, Q, F, te, Y]
+        t.$$.dirty[0] & 4096 && n(14, A = h), t.$$.dirty[0] & 278528 && n(3, r = c[A] || void 0), t.$$.dirty[0] & 147456 && n(15, l = s[A] || void 0), t.$$.dirty[0] & 32776 && (r && I.set(r.id), l && B.set(l.id)), t.$$.dirty[0] & 65536 && u && n(5, W = !0), t.$$.dirty[0] & 8192 && S.set(m)
+    }, e = exclude_internal_props(e), [p, v, k, r, L, W, E, w, I, D, o, e, h, m, A, l, u, s, c, g, d, G, j, Q, F, te, Y]
 }
 class Tabs extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$1a, create_fragment$1a, safe_not_equal, {
             selected: 12,
             type: 0,
             autoWidth: 13,
@@ -10930,24 +10924,24 @@
         binding_callbacks[A ? "unshift" : "push"](() => {
             m = A, n(0, m)
         })
     }
     const L = () => {
             g || E(p)
         },
-        G = ({
+        W = ({
             key: A
         }) => {
             g || (A === "ArrowRight" ? w(1) : A === "ArrowLeft" ? w(-1) : (A === " " || A === "Enter") && E(p))
         };
     return t.$$set = A => {
         e = assign(assign({}, e), exclude_internal_props(A)), n(12, a = compute_rest_props(e, l)), "label" in A && n(1, _ = A.label), "href" in A && n(2, d = A.href), "disabled" in A && n(3, g = A.disabled), "tabindex" in A && n(4, h = A.tabindex), "id" in A && n(5, p = A.id), "ref" in A && n(0, m = A.ref), "$$scope" in A && n(14, c = A.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty & 8224 && n(6, r = o === p)
-    }, [m, _, d, g, h, p, r, u, v, k, E, w, a, o, c, s, S, I, D, O, B, L, G]
+    }, [m, _, d, g, h, p, r, u, v, k, E, w, a, o, c, s, S, I, D, O, B, L, W]
 }
 class Tab extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$19, create_fragment$19, safe_not_equal, {
             label: 1,
             href: 2,
             disabled: 3,
@@ -12995,26 +12989,26 @@
     if (_) try {
         null.error
     } catch (A) {
         var p = _(_(A));
         h["%Error.prototype%"] = p
     }
     var m = function A(U) {
-            var W;
-            if (U === "%AsyncFunction%") W = l("async function () {}");
-            else if (U === "%GeneratorFunction%") W = l("function* () {}");
-            else if (U === "%AsyncGeneratorFunction%") W = l("async function* () {}");
+            var G;
+            if (U === "%AsyncFunction%") G = l("async function () {}");
+            else if (U === "%GeneratorFunction%") G = l("function* () {}");
+            else if (U === "%AsyncGeneratorFunction%") G = l("async function* () {}");
             else if (U === "%AsyncGenerator%") {
                 var j = A("%AsyncGeneratorFunction%");
-                j && (W = j.prototype)
+                j && (G = j.prototype)
             } else if (U === "%AsyncIteratorPrototype%") {
                 var Q = A("%AsyncGenerator%");
-                Q && _ && (W = _(Q.prototype))
+                Q && _ && (G = _(Q.prototype))
             }
-            return h[U] = W, W
+            return h[U] = G, G
         },
         v = {
             "%ArrayBufferPrototype%": ["ArrayBuffer", "prototype"],
             "%ArrayPrototype%": ["Array", "prototype"],
             "%ArrayProto_entries%": ["Array", "prototype", "entries"],
             "%ArrayProto_forEach%": ["Array", "prototype", "forEach"],
             "%ArrayProto_keys%": ["Array", "prototype", "keys"],
@@ -13071,58 +13065,58 @@
         w = k.call(Function.apply, Array.prototype.splice),
         S = k.call(Function.call, String.prototype.replace),
         I = k.call(Function.call, String.prototype.slice),
         D = k.call(Function.call, RegExp.prototype.exec),
         O = /[^%.[\]]+|\[(?:(-?\d+(?:\.\d+)?)|(["'])((?:(?!\2)[^\\]|\\.)*?)\2)\]|(?=(?:\.|\[\])(?:\.|\[\]|%$))/g,
         B = /\\(\\)?/g,
         L = function(U) {
-            var W = I(U, 0, 1),
+            var G = I(U, 0, 1),
                 j = I(U, -1);
-            if (W === "%" && j !== "%") throw new e("invalid intrinsic syntax, expected closing `%`");
-            if (j === "%" && W !== "%") throw new e("invalid intrinsic syntax, expected opening `%`");
+            if (G === "%" && j !== "%") throw new e("invalid intrinsic syntax, expected closing `%`");
+            if (j === "%" && G !== "%") throw new e("invalid intrinsic syntax, expected opening `%`");
             var Q = [];
             return S(U, O, function(F, te, Y, oe) {
                 Q[Q.length] = Y ? S(oe, B, "$1") : te || F
             }), Q
         },
-        G = function(U, W) {
+        W = function(U, G) {
             var j = U,
                 Q;
             if (b(v, j) && (Q = v[j], j = "%" + Q[0] + "%"), b(h, j)) {
                 var F = h[j];
-                if (F === d && (F = m(j)), typeof F > "u" && !W) throw new r("intrinsic " + U + " exists, but is not available. Please file an issue!");
+                if (F === d && (F = m(j)), typeof F > "u" && !G) throw new r("intrinsic " + U + " exists, but is not available. Please file an issue!");
                 return {
                     alias: Q,
                     name: j,
                     value: F
                 }
             }
             throw new e("intrinsic " + U + " does not exist!")
         };
-    return getIntrinsic = function(U, W) {
+    return getIntrinsic = function(U, G) {
         if (typeof U != "string" || U.length === 0) throw new r("intrinsic name must be a non-empty string");
-        if (arguments.length > 1 && typeof W != "boolean") throw new r('"allowMissing" argument must be a boolean');
+        if (arguments.length > 1 && typeof G != "boolean") throw new r('"allowMissing" argument must be a boolean');
         if (D(/^%?[^%]*%?$/, U) === null) throw new e("`%` may not be present anywhere but at the beginning and end of the intrinsic name");
         var j = L(U),
             Q = j.length > 0 ? j[0] : "",
-            F = G("%" + Q + "%", W),
+            F = W("%" + Q + "%", G),
             te = F.name,
             Y = F.value,
             oe = !1,
             ae = F.alias;
         ae && (Q = ae[0], w(j, E([0, 1], ae)));
         for (var C = 1, Z = !0; C < j.length; C += 1) {
             var K = j[C],
                 ce = I(K, 0, 1),
                 z = I(K, -1);
             if ((ce === '"' || ce === "'" || ce === "`" || z === '"' || z === "'" || z === "`") && ce !== z) throw new e("property names with quotes must have matching quotes");
             if ((K === "constructor" || !Z) && (oe = !0), Q += "." + K, te = "%" + Q + "%", b(h, te)) Y = h[te];
             else if (Y != null) {
                 if (!(K in Y)) {
-                    if (!W) throw new r("base intrinsic for " + U + " exists, but the property is not available.");
+                    if (!G) throw new r("base intrinsic for " + U + " exists, but the property is not available.");
                     return
                 }
                 if (a && C + 1 >= j.length) {
                     var V = a(Y, K);
                     Z = !!V, Z && "get" in V && !("originalValue" in V.get) ? Y = V.get : Y = Y[K]
                 } else Z = b(Y, K), Y = Y[K];
                 Z && !oe && (h[te] = Y)
@@ -13541,36 +13535,36 @@
         t.isFloat64Array = B;
 
         function L(N) {
             return r(N) === "BigInt64Array"
         }
         t.isBigInt64Array = L;
 
-        function G(N) {
+        function W(N) {
             return r(N) === "BigUint64Array"
         }
-        t.isBigUint64Array = G;
+        t.isBigUint64Array = W;
 
         function A(N) {
             return s(N) === "[object Map]"
         }
         A.working = typeof Map < "u" && A(new Map);
 
         function U(N) {
             return typeof Map > "u" ? !1 : A.working ? A(N) : N instanceof Map
         }
         t.isMap = U;
 
-        function W(N) {
+        function G(N) {
             return s(N) === "[object Set]"
         }
-        W.working = typeof Set < "u" && W(new Set);
+        G.working = typeof Set < "u" && G(new Set);
 
         function j(N) {
-            return typeof Set > "u" ? !1 : W.working ? W(N) : N instanceof Set
+            return typeof Set > "u" ? !1 : G.working ? G(N) : N instanceof Set
         }
         t.isSet = j;
 
         function Q(N) {
             return s(N) === "[object WeakMap]"
         }
         Q.working = typeof WeakMap < "u" && Q(new WeakMap);
@@ -13815,32 +13809,32 @@
                 var ce = Z.inspect(K, C);
                 return S(ce) || (ce = _(C, ce, K)), ce
             }
             var z = d(C, Z);
             if (z) return z;
             var V = Object.keys(Z),
                 $ = c(V);
-            if (C.showHidden && (V = Object.getOwnPropertyNames(Z)), G(Z) && (V.indexOf("message") >= 0 || V.indexOf("description") >= 0)) return g(Z);
+            if (C.showHidden && (V = Object.getOwnPropertyNames(Z)), W(Z) && (V.indexOf("message") >= 0 || V.indexOf("description") >= 0)) return g(Z);
             if (V.length === 0) {
                 if (A(Z)) {
                     var re = Z.name ? ": " + Z.name : "";
                     return C.stylize("[Function" + re + "]", "special")
                 }
                 if (O(Z)) return C.stylize(RegExp.prototype.toString.call(Z), "regexp");
                 if (L(Z)) return C.stylize(Date.prototype.toString.call(Z), "date");
-                if (G(Z)) return g(Z)
+                if (W(Z)) return g(Z)
             }
             var ue = "",
                 P = !1,
                 q = ["{", "}"];
             if (v(Z) && (P = !0, q = ["[", "]"]), A(Z)) {
                 var ee = Z.name ? ": " + Z.name : "";
                 ue = " [Function" + ee + "]"
             }
-            if (O(Z) && (ue = " " + RegExp.prototype.toString.call(Z)), L(Z) && (ue = " " + Date.prototype.toUTCString.call(Z)), G(Z) && (ue = " " + g(Z)), V.length === 0 && (!P || Z.length == 0)) return q[0] + ue + q[1];
+            if (O(Z) && (ue = " " + RegExp.prototype.toString.call(Z)), L(Z) && (ue = " " + Date.prototype.toUTCString.call(Z)), W(Z) && (ue = " " + g(Z)), V.length === 0 && (!P || Z.length == 0)) return q[0] + ue + q[1];
             if (K < 0) return O(Z) ? C.stylize(RegExp.prototype.toString.call(Z), "regexp") : C.stylize("[Object]", "special");
             C.seen.push(Z);
             var X;
             return P ? X = h(C, Z, K, $, V) : X = V.map(function(fe) {
                 return p(C, Z, K, $, fe, P)
             }), C.seen.pop(), m(X, ue, q)
         }
@@ -13936,44 +13930,44 @@
 
         function D(C) {
             return C === void 0
         }
         t.isUndefined = D;
 
         function O(C) {
-            return B(C) && W(C) === "[object RegExp]"
+            return B(C) && G(C) === "[object RegExp]"
         }
         t.isRegExp = O, t.types.isRegExp = O;
 
         function B(C) {
             return typeof C == "object" && C !== null
         }
         t.isObject = B;
 
         function L(C) {
-            return B(C) && W(C) === "[object Date]"
+            return B(C) && G(C) === "[object Date]"
         }
         t.isDate = L, t.types.isDate = L;
 
-        function G(C) {
-            return B(C) && (W(C) === "[object Error]" || C instanceof Error)
+        function W(C) {
+            return B(C) && (G(C) === "[object Error]" || C instanceof Error)
         }
-        t.isError = G, t.types.isNativeError = G;
+        t.isError = W, t.types.isNativeError = W;
 
         function A(C) {
             return typeof C == "function"
         }
         t.isFunction = A;
 
         function U(C) {
             return C === null || typeof C == "boolean" || typeof C == "number" || typeof C == "string" || typeof C == "symbol" || typeof C > "u"
         }
         t.isPrimitive = U, t.isBuffer = requireIsBufferBrowser();
 
-        function W(C) {
+        function G(C) {
             return Object.prototype.toString.call(C)
         }
 
         function j(C) {
             return C < 10 ? "0" + C.toString(10) : C.toString(10)
         }
         var Q = ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"];
@@ -14519,27 +14513,27 @@
     }, Object.defineProperty(O.prototype, "writableBuffer", {
         enumerable: !1,
         get: function() {
             return this._writableState && this._writableState.getBuffer()
         }
     });
 
-    function G(z, V, $) {
+    function W(z, V, $) {
         return !z.objectMode && z.decodeStrings !== !1 && typeof V == "string" && (V = l.from(V, $)), V
     }
     Object.defineProperty(O.prototype, "writableHighWaterMark", {
         enumerable: !1,
         get: function() {
             return this._writableState.highWaterMark
         }
     });
 
     function A(z, V, $, re, ue, P) {
         if (!$) {
-            var q = G(V, re, ue);
+            var q = W(V, re, ue);
             re !== q && ($ = !0, ue = "buffer", re = q)
         }
         var ee = V.objectMode ? 1 : re.length;
         V.length += ee;
         var X = V.length < V.highWaterMark;
         if (X || (V.needDrain = !0), V.writing || V.corked) {
             var fe = V.lastBufferedRequest;
@@ -14554,28 +14548,28 @@
         return X
     }
 
     function U(z, V, $, re, ue, P, q) {
         V.writelen = re, V.writecb = q, V.writing = !0, V.sync = !0, V.destroyed ? V.onwrite(new v("write")) : $ ? z._writev(ue, V.onwrite) : z._write(ue, P, V.onwrite), V.sync = !1
     }
 
-    function W(z, V, $, re, ue) {
+    function G(z, V, $, re, ue) {
         --V.pendingcb, $ ? (process$1.nextTick(ue, re), process$1.nextTick(Z, z, V), z._writableState.errorEmitted = !0, w(z, re)) : (ue(re), z._writableState.errorEmitted = !0, w(z, re), Z(z, V))
     }
 
     function j(z) {
         z.writing = !1, z.writecb = null, z.length -= z.writelen, z.writelen = 0
     }
 
     function Q(z, V) {
         var $ = z._writableState,
             re = $.sync,
             ue = $.writecb;
         if (typeof ue != "function") throw new p;
-        if (j($), V) W(z, $, re, V, ue);
+        if (j($), V) G(z, $, re, V, ue);
         else {
             var P = oe($) || z.destroyed;
             !P && !$.corked && !$.bufferProcessing && $.bufferedRequest && Y(z, $), re ? process$1.nextTick(F, z, $, P, ue) : F(z, $, P, ue)
         }
     }
 
     function F(z, V, $, re) {
@@ -15210,25 +15204,25 @@
         s("readableAddChunk", q);
         var M = P._readableState;
         if (q === null) M.reading = !1, Q(P, M);
         else {
             var y;
             if (fe || (y = A(M, q)), y) S(P, y);
             else if (M.objectMode || q && q.length > 0)
-                if (typeof q != "string" && !M.objectMode && Object.getPrototypeOf(q) !== r.prototype && (q = a(q)), X) M.endEmitted ? S(P, new k) : G(P, M, q, !0);
+                if (typeof q != "string" && !M.objectMode && Object.getPrototypeOf(q) !== r.prototype && (q = a(q)), X) M.endEmitted ? S(P, new k) : W(P, M, q, !0);
                 else if (M.ended) S(P, new m);
             else {
                 if (M.destroyed) return !1;
-                M.reading = !1, M.decoder && !ee ? (q = M.decoder.write(q), M.objectMode || q.length !== 0 ? G(P, M, q, !1) : Y(P, M)) : G(P, M, q, !1)
+                M.reading = !1, M.decoder && !ee ? (q = M.decoder.write(q), M.objectMode || q.length !== 0 ? W(P, M, q, !1) : Y(P, M)) : W(P, M, q, !1)
             } else X || (M.reading = !1, Y(P, M))
         }
         return !M.ended && (M.length < M.highWaterMark || M.length === 0)
     }
 
-    function G(P, q, ee, X) {
+    function W(P, q, ee, X) {
         q.flowing && q.length === 0 && !q.sync ? (q.awaitDrain = 0, P.emit("data", ee)) : (q.length += q.objectMode ? 1 : ee.length, X ? q.buffer.unshift(ee) : q.buffer.push(ee), q.needReadable && F(P)), Y(P, q)
     }
 
     function A(P, q) {
         var ee;
         return !o(q) && typeof q != "string" && q !== void 0 && !P.objectMode && (ee = new p("chunk", ["string", "Buffer", "Uint8Array"], q)), ee
     }
@@ -15239,20 +15233,20 @@
         var q = new b(P);
         this._readableState.decoder = q, this._readableState.encoding = this._readableState.decoder.encoding;
         for (var ee = this._readableState.buffer.head, X = ""; ee !== null;) X += q.write(ee.data), ee = ee.next;
         return this._readableState.buffer.clear(), X !== "" && this._readableState.buffer.push(X), this._readableState.length = X.length, this
     };
     var U = 1073741824;
 
-    function W(P) {
+    function G(P) {
         return P >= U ? P = U : (P--, P |= P >>> 1, P |= P >>> 2, P |= P >>> 4, P |= P >>> 8, P |= P >>> 16, P++), P
     }
 
     function j(P, q) {
-        return P <= 0 || q.length === 0 && q.ended ? 0 : q.objectMode ? 1 : P !== P ? q.flowing && q.length ? q.buffer.head.data.length : q.length : (P > q.highWaterMark && (q.highWaterMark = W(P)), P <= q.length ? P : q.ended ? q.length : (q.needReadable = !0, 0))
+        return P <= 0 || q.length === 0 && q.ended ? 0 : q.objectMode ? 1 : P !== P ? q.flowing && q.length ? q.buffer.head.data.length : q.length : (P > q.highWaterMark && (q.highWaterMark = G(P)), P <= q.length ? P : q.ended ? q.length : (q.needReadable = !0, 0))
     }
     B.prototype.read = function(P) {
         s("read", P), P = parseInt(P, 10);
         var q = this._readableState,
             ee = P;
         if (P !== 0 && (q.emittedReadable = !1), P === 0 && q.needReadable && ((q.highWaterMark !== 0 ? q.length >= q.highWaterMark : q.length > 0) || q.ended)) return s("read: emitReadable", q.length, q.ended), q.length === 0 && q.ended ? $(this) : F(this), null;
         if (P = j(P, q), P === 0 && q.ended) return q.length === 0 && $(this), null;
@@ -17057,26 +17051,26 @@
         {
             showMoreLess: B = !1
         } = e,
         {
             id: L = "ccs-" + Math.random().toString(36)
         } = e,
         {
-            ref: G = null
+            ref: W = null
         } = e;
     const A = createEventDispatcher();
-    let U, W;
+    let U, G;
 
     function j() {
         const {
             height: X
-        } = G.getBoundingClientRect();
-        X > 0 && n(2, B = G.getBoundingClientRect().height > 255)
+        } = W.getBoundingClientRect();
+        X > 0 && n(2, B = W.getBoundingClientRect().height > 255)
     }
-    onMount(() => () => clearTimeout(W));
+    onMount(() => () => clearTimeout(G));
 
     function Q(X) {
         bubble.call(this, t, X)
     }
 
     function F(X) {
         bubble.call(this, t, X)
@@ -17114,27 +17108,27 @@
         bubble.call(this, t, X)
     }
 
     function z(X) {
         bubble.call(this, t, X)
     }
     const V = () => {
-            g(d), A("copy"), U !== "fade-in" && (n(16, U = "fade-in"), n(17, W = setTimeout(() => {
+            g(d), A("copy"), U !== "fade-in" && (n(16, U = "fade-in"), n(17, G = setTimeout(() => {
                 n(16, U = "fade-out")
             }, I)))
         },
         $ = ({
             animationName: X
         }) => {
             X === "hide-feedback" && n(16, U = void 0)
         };
 
     function re(X) {
         binding_callbacks[X ? "unshift" : "push"](() => {
-            G = X, n(1, G)
+            W = X, n(1, W)
         })
     }
 
     function ue(X) {
         bubble.call(this, t, X)
     }
 
@@ -17145,18 +17139,18 @@
     function q(X) {
         bubble.call(this, t, X)
     }
     const ee = () => {
         n(0, h = !h)
     };
     return t.$$set = X => {
-        e = assign(assign({}, e), exclude_internal_props(X)), n(22, u = compute_rest_props(e, o)), "type" in X && n(3, _ = X.type), "code" in X && n(4, d = X.code), "copy" in X && n(5, g = X.copy), "expanded" in X && n(0, h = X.expanded), "hideCopyButton" in X && n(6, p = X.hideCopyButton), "disabled" in X && n(7, m = X.disabled), "wrapText" in X && n(8, v = X.wrapText), "light" in X && n(9, k = X.light), "skeleton" in X && n(10, b = X.skeleton), "copyButtonDescription" in X && n(11, E = X.copyButtonDescription), "copyLabel" in X && n(12, w = X.copyLabel), "feedback" in X && n(13, S = X.feedback), "feedbackTimeout" in X && n(14, I = X.feedbackTimeout), "showLessText" in X && n(23, D = X.showLessText), "showMoreText" in X && n(24, O = X.showMoreText), "showMoreLess" in X && n(2, B = X.showMoreLess), "id" in X && n(15, L = X.id), "ref" in X && n(1, G = X.ref), "$$scope" in X && n(44, c = X.$$scope)
+        e = assign(assign({}, e), exclude_internal_props(X)), n(22, u = compute_rest_props(e, o)), "type" in X && n(3, _ = X.type), "code" in X && n(4, d = X.code), "copy" in X && n(5, g = X.copy), "expanded" in X && n(0, h = X.expanded), "hideCopyButton" in X && n(6, p = X.hideCopyButton), "disabled" in X && n(7, m = X.disabled), "wrapText" in X && n(8, v = X.wrapText), "light" in X && n(9, k = X.light), "skeleton" in X && n(10, b = X.skeleton), "copyButtonDescription" in X && n(11, E = X.copyButtonDescription), "copyLabel" in X && n(12, w = X.copyLabel), "feedback" in X && n(13, S = X.feedback), "feedbackTimeout" in X && n(14, I = X.feedbackTimeout), "showLessText" in X && n(23, D = X.showLessText), "showMoreText" in X && n(24, O = X.showMoreText), "showMoreLess" in X && n(2, B = X.showMoreLess), "id" in X && n(15, L = X.id), "ref" in X && n(1, W = X.ref), "$$scope" in X && n(44, c = X.$$scope)
     }, t.$$.update = () => {
-        t.$$.dirty[0] & 25165825 && n(20, r = h ? D : O), t.$$.dirty[0] & 1 && n(19, l = h ? 16 * 15 : 48), t.$$.dirty[0] & 1 && n(18, a = h ? "none" : 16 * 15 + "px"), t.$$.dirty[0] & 26 && _ === "multi" && G && (d === void 0 && j(), d && tick().then(j)), t.$$.dirty[0] & 9 && _ === "multi" && A(h ? "expand" : "collapse")
-    }, [h, G, B, _, d, g, p, m, v, k, b, E, w, S, I, L, U, W, a, l, r, A, u, D, O, s, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P, q, ee, c]
+        t.$$.dirty[0] & 25165825 && n(20, r = h ? D : O), t.$$.dirty[0] & 1 && n(19, l = h ? 16 * 15 : 48), t.$$.dirty[0] & 1 && n(18, a = h ? "none" : 16 * 15 + "px"), t.$$.dirty[0] & 26 && _ === "multi" && W && (d === void 0 && j(), d && tick().then(j)), t.$$.dirty[0] & 9 && _ === "multi" && A(h ? "expand" : "collapse")
+    }, [h, W, B, _, d, g, p, m, v, k, b, E, w, S, I, L, U, G, a, l, r, A, u, D, O, s, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P, q, ee, c]
 }
 class CodeSnippet extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$_, create_fragment$_, safe_not_equal, {
             type: 3,
             code: 4,
             copy: 5,
@@ -18530,22 +18524,22 @@
     function B(A) {
         bubble.call(this, t, A)
     }
 
     function L(A) {
         bubble.call(this, t, A)
     }
-    const G = A => {
+    const W = A => {
         n(0, m = !0), storedGlobalChanged.set(!0), S(A.detail)
     };
     return t.$$set = A => {
         "key" in A && n(1, l = A.key), "value" in A && n(9, a = A.value), "placeholder" in A && n(2, o = A.placeholder), "optionType" in A && n(10, u = A.optionType), "required" in A && n(11, s = A.required), "activeNavItem" in A && n(12, c = A.activeNavItem), "readonly" in A && n(3, _ = A.readonly), "setError" in A && n(13, d = A.setError), "removeError" in A && n(14, g = A.removeError), "pgargs" in A && n(15, h = A.pgargs), "pgargkey" in A && n(4, p = A.pgargkey), "changed" in A && n(0, m = A.changed)
     }, t.$$.update = () => {
         t.$$.dirty & 32786 && n(16, r = get_pgvalue(h, p === !0 ? l : p)), t.$$.dirty & 65537 && r !== void 0 && !m && n(5, b = r), t.$$.dirty & 1056 && (b === "" && E == null || n(9, a = applyAtomicType(b, u, !1)))
-    }, [m, l, o, _, p, b, v, k, S, a, u, s, c, d, g, h, r, I, D, O, B, L, G]
+    }, [m, l, o, _, p, b, v, k, S, a, u, s, c, d, g, h, r, I, D, O, B, L, W]
 }
 class PlainOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$O, create_fragment$O, safe_not_equal, {
             key: 1,
             value: 9,
             placeholder: 2,
@@ -18632,25 +18626,25 @@
         I = S || fallback_block_1$2(t),
         D = t[12].labelB,
         O = create_slot(D, t, t[11], get_labelB_slot_context),
         B = O || fallback_block$8(t);
     let L = [t[9], {
             style: h = t[9].style + "; user-select: none"
         }],
-        G = {};
-    for (let A = 0; A < L.length; A += 1) G = assign(G, L[A]);
+        W = {};
+    for (let A = 0; A < L.length; A += 1) W = assign(W, L[A]);
     return {
         c() {
-            e = element("div"), n = element("input"), r = space(), l = element("label"), a = element("span"), E && E.c(), o = space(), u = element("span"), s = element("span"), I && I.c(), c = space(), _ = element("span"), B && B.c(), attr(n, "role", "switch"), attr(n, "type", "checkbox"), n.checked = t[0], n.disabled = t[2], attr(n, "id", t[7]), attr(n, "name", t[8]), toggle_class(n, "bx--toggle-input", !0), toggle_class(n, "bx--toggle-input--small", t[1] === "sm"), toggle_class(a, "bx--visually-hidden", t[6]), attr(s, "aria-hidden", "true"), toggle_class(s, "bx--toggle__text--off", !0), attr(_, "aria-hidden", "true"), toggle_class(_, "bx--toggle__text--on", !0), attr(u, "style", d = t[6] && "margin-top: 0"), toggle_class(u, "bx--toggle__switch", !0), attr(l, "aria-label", g = t[5] ? void 0 : t[10]["aria-label"] || "Toggle"), attr(l, "for", t[7]), toggle_class(l, "bx--toggle-input__label", !0), set_attributes(e, G), toggle_class(e, "bx--form-item", !0)
+            e = element("div"), n = element("input"), r = space(), l = element("label"), a = element("span"), E && E.c(), o = space(), u = element("span"), s = element("span"), I && I.c(), c = space(), _ = element("span"), B && B.c(), attr(n, "role", "switch"), attr(n, "type", "checkbox"), n.checked = t[0], n.disabled = t[2], attr(n, "id", t[7]), attr(n, "name", t[8]), toggle_class(n, "bx--toggle-input", !0), toggle_class(n, "bx--toggle-input--small", t[1] === "sm"), toggle_class(a, "bx--visually-hidden", t[6]), attr(s, "aria-hidden", "true"), toggle_class(s, "bx--toggle__text--off", !0), attr(_, "aria-hidden", "true"), toggle_class(_, "bx--toggle__text--on", !0), attr(u, "style", d = t[6] && "margin-top: 0"), toggle_class(u, "bx--toggle__switch", !0), attr(l, "aria-label", g = t[5] ? void 0 : t[10]["aria-label"] || "Toggle"), attr(l, "for", t[7]), toggle_class(l, "bx--toggle-input__label", !0), set_attributes(e, W), toggle_class(e, "bx--form-item", !0)
         },
         m(A, U) {
             insert(A, e, U), append(e, n), append(e, r), append(e, l), append(l, a), E && E.m(a, null), append(l, o), append(l, u), append(u, s), I && I.m(s, null), append(u, c), append(u, _), B && B.m(_, null), p = !0, m || (v = [listen(n, "change", t[21]), listen(n, "change", t[17]), listen(n, "keyup", t[22]), listen(n, "keyup", t[18]), listen(n, "focus", t[19]), listen(n, "blur", t[20]), listen(e, "click", t[13]), listen(e, "mouseover", t[14]), listen(e, "mouseenter", t[15]), listen(e, "mouseleave", t[16])], m = !0)
         },
         p(A, [U]) {
-            (!p || U & 1) && (n.checked = A[0]), (!p || U & 4) && (n.disabled = A[2]), (!p || U & 128) && attr(n, "id", A[7]), (!p || U & 256) && attr(n, "name", A[8]), (!p || U & 2) && toggle_class(n, "bx--toggle-input--small", A[1] === "sm"), b ? b.p && (!p || U & 2048) && update_slot_base(b, k, A, A[11], p ? get_slot_changes(k, A[11], U, get_labelText_slot_changes$3) : get_all_dirty_from_scope(A[11]), get_labelText_slot_context$3) : E && E.p && (!p || U & 32) && E.p(A, p ? U : -1), (!p || U & 64) && toggle_class(a, "bx--visually-hidden", A[6]), S ? S.p && (!p || U & 2048) && update_slot_base(S, w, A, A[11], p ? get_slot_changes(w, A[11], U, get_labelA_slot_changes) : get_all_dirty_from_scope(A[11]), get_labelA_slot_context) : I && I.p && (!p || U & 8) && I.p(A, p ? U : -1), O ? O.p && (!p || U & 2048) && update_slot_base(O, D, A, A[11], p ? get_slot_changes(D, A[11], U, get_labelB_slot_changes) : get_all_dirty_from_scope(A[11]), get_labelB_slot_context) : B && B.p && (!p || U & 16) && B.p(A, p ? U : -1), (!p || U & 64 && d !== (d = A[6] && "margin-top: 0")) && attr(u, "style", d), (!p || U & 1056 && g !== (g = A[5] ? void 0 : A[10]["aria-label"] || "Toggle")) && attr(l, "aria-label", g), (!p || U & 128) && attr(l, "for", A[7]), set_attributes(e, G = get_spread_update(L, [U & 512 && A[9], (!p || U & 512 && h !== (h = A[9].style + "; user-select: none")) && {
+            (!p || U & 1) && (n.checked = A[0]), (!p || U & 4) && (n.disabled = A[2]), (!p || U & 128) && attr(n, "id", A[7]), (!p || U & 256) && attr(n, "name", A[8]), (!p || U & 2) && toggle_class(n, "bx--toggle-input--small", A[1] === "sm"), b ? b.p && (!p || U & 2048) && update_slot_base(b, k, A, A[11], p ? get_slot_changes(k, A[11], U, get_labelText_slot_changes$3) : get_all_dirty_from_scope(A[11]), get_labelText_slot_context$3) : E && E.p && (!p || U & 32) && E.p(A, p ? U : -1), (!p || U & 64) && toggle_class(a, "bx--visually-hidden", A[6]), S ? S.p && (!p || U & 2048) && update_slot_base(S, w, A, A[11], p ? get_slot_changes(w, A[11], U, get_labelA_slot_changes) : get_all_dirty_from_scope(A[11]), get_labelA_slot_context) : I && I.p && (!p || U & 8) && I.p(A, p ? U : -1), O ? O.p && (!p || U & 2048) && update_slot_base(O, D, A, A[11], p ? get_slot_changes(D, A[11], U, get_labelB_slot_changes) : get_all_dirty_from_scope(A[11]), get_labelB_slot_context) : B && B.p && (!p || U & 16) && B.p(A, p ? U : -1), (!p || U & 64 && d !== (d = A[6] && "margin-top: 0")) && attr(u, "style", d), (!p || U & 1056 && g !== (g = A[5] ? void 0 : A[10]["aria-label"] || "Toggle")) && attr(l, "aria-label", g), (!p || U & 128) && attr(l, "for", A[7]), set_attributes(e, W = get_spread_update(L, [U & 512 && A[9], (!p || U & 512 && h !== (h = A[9].style + "; user-select: none")) && {
                 style: h
             }])), toggle_class(e, "bx--form-item", !0)
         },
         i(A) {
             p || (transition_in(E, A), transition_in(I, A), transition_in(B, A), p = !0)
         },
         o(A) {
@@ -18694,53 +18688,53 @@
             id: p = "ccs-" + Math.random().toString(36)
         } = e,
         {
             name: m = void 0
         } = e;
     const v = createEventDispatcher();
 
-    function k(G) {
-        bubble.call(this, t, G)
+    function k(W) {
+        bubble.call(this, t, W)
     }
 
-    function b(G) {
-        bubble.call(this, t, G)
+    function b(W) {
+        bubble.call(this, t, W)
     }
 
-    function E(G) {
-        bubble.call(this, t, G)
+    function E(W) {
+        bubble.call(this, t, W)
     }
 
-    function w(G) {
-        bubble.call(this, t, G)
+    function w(W) {
+        bubble.call(this, t, W)
     }
 
-    function S(G) {
-        bubble.call(this, t, G)
+    function S(W) {
+        bubble.call(this, t, W)
     }
 
-    function I(G) {
-        bubble.call(this, t, G)
+    function I(W) {
+        bubble.call(this, t, W)
     }
 
-    function D(G) {
-        bubble.call(this, t, G)
+    function D(W) {
+        bubble.call(this, t, W)
     }
 
-    function O(G) {
-        bubble.call(this, t, G)
+    function O(W) {
+        bubble.call(this, t, W)
     }
     const B = () => {
             n(0, s = !s)
         },
-        L = G => {
-            (G.key === " " || G.key === "Enter") && (G.preventDefault(), n(0, s = !s))
+        L = W => {
+            (W.key === " " || W.key === "Enter") && (W.preventDefault(), n(0, s = !s))
         };
-    return t.$$set = G => {
-        n(10, e = assign(assign({}, e), exclude_internal_props(G))), n(9, l = compute_rest_props(e, r)), "size" in G && n(1, u = G.size), "toggled" in G && n(0, s = G.toggled), "disabled" in G && n(2, c = G.disabled), "labelA" in G && n(3, _ = G.labelA), "labelB" in G && n(4, d = G.labelB), "labelText" in G && n(5, g = G.labelText), "hideLabel" in G && n(6, h = G.hideLabel), "id" in G && n(7, p = G.id), "name" in G && n(8, m = G.name), "$$scope" in G && n(11, o = G.$$scope)
+    return t.$$set = W => {
+        n(10, e = assign(assign({}, e), exclude_internal_props(W))), n(9, l = compute_rest_props(e, r)), "size" in W && n(1, u = W.size), "toggled" in W && n(0, s = W.toggled), "disabled" in W && n(2, c = W.disabled), "labelA" in W && n(3, _ = W.labelA), "labelB" in W && n(4, d = W.labelB), "labelText" in W && n(5, g = W.labelText), "hideLabel" in W && n(6, h = W.hideLabel), "id" in W && n(7, p = W.id), "name" in W && n(8, m = W.name), "$$scope" in W && n(11, o = W.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty & 1 && v("toggle", {
             toggled: s
         })
     }, e = exclude_internal_props(e), [s, u, c, _, d, g, h, p, m, l, e, o, a, k, b, E, w, S, I, D, O, B, L]
 }
 class Toggle extends SvelteComponent {
@@ -19219,27 +19213,27 @@
         bubble.call(this, t, C)
     }
 
     function L(C) {
         bubble.call(this, t, C)
     }
 
-    function G(C) {
+    function W(C) {
         bubble.call(this, t, C)
     }
 
     function A(C) {
         bubble.call(this, t, C)
     }
 
     function U(C) {
         bubble.call(this, t, C)
     }
 
-    function W(C) {
+    function G(C) {
         bubble.call(this, t, C)
     }
 
     function j(C) {
         bubble.call(this, t, C)
     }
 
@@ -19268,15 +19262,15 @@
     function ae() {
         c = this.value, n(0, c)
     }
     return t.$$set = C => {
         e = assign(assign({}, e), exclude_internal_props(C)), n(18, a = compute_rest_props(e, l)), "value" in C && n(0, c = C.value), "placeholder" in C && n(2, _ = C.placeholder), "cols" in C && n(3, d = C.cols), "rows" in C && n(4, g = C.rows), "maxCount" in C && n(5, h = C.maxCount), "light" in C && n(6, p = C.light), "disabled" in C && n(7, m = C.disabled), "readonly" in C && n(8, v = C.readonly), "helperText" in C && n(9, k = C.helperText), "labelText" in C && n(10, b = C.labelText), "hideLabel" in C && n(11, E = C.hideLabel), "invalid" in C && n(12, w = C.invalid), "invalidText" in C && n(13, S = C.invalidText), "id" in C && n(14, I = C.id), "name" in C && n(15, D = C.name), "ref" in C && n(1, O = C.ref), "$$scope" in C && n(19, u = C.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 16384 && n(16, r = `error-${I}`)
-    }, [c, O, _, d, g, h, p, m, v, k, b, E, w, S, I, D, r, s, a, u, o, B, L, G, A, U, W, j, Q, F, te, Y, oe, ae]
+    }, [c, O, _, d, g, h, p, m, v, k, b, E, w, S, I, D, r, s, a, u, o, B, L, W, A, U, G, j, Q, F, te, Y, oe, ae]
 }
 class TextArea extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$K, create_fragment$K, safe_not_equal, {
             value: 0,
             placeholder: 2,
             cols: 3,
@@ -19469,22 +19463,22 @@
         n(0, p = !0), storedGlobalChanged.set(!0), w(A.target.value)
     };
 
     function L(A) {
         bubble.call(this, t, A)
     }
 
-    function G(A) {
+    function W(A) {
         bubble.call(this, t, A)
     }
     return t.$$set = A => {
         "key" in A && n(2, l = A.key), "value" in A && n(1, a = A.value), "placeholder" in A && n(3, o = A.placeholder), "required" in A && n(10, u = A.required), "activeNavItem" in A && n(11, s = A.activeNavItem), "readonly" in A && n(4, c = A.readonly), "setError" in A && n(12, _ = A.setError), "removeError" in A && n(13, d = A.removeError), "pgargs" in A && n(14, g = A.pgargs), "pgargkey" in A && n(5, h = A.pgargkey), "changed" in A && n(0, p = A.changed)
     }, t.$$.update = () => {
         t.$$.dirty & 16420 && n(15, r = get_pgvalue(g, h === !0 ? l : h)), t.$$.dirty & 32769 && r !== void 0 && !p && n(1, a = r)
-    }, [p, a, l, o, c, h, v, k, E, w, u, s, _, d, g, r, S, I, D, O, B, L, G]
+    }, [p, a, l, o, c, h, v, k, E, w, u, s, _, d, g, r, S, I, D, O, B, L, W]
 }
 class TextOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$J, create_fragment$J, safe_not_equal, {
             key: 2,
             value: 1,
             placeholder: 3,
@@ -20730,35 +20724,35 @@
         {
             hideLabel: B = !1
         } = e,
         {
             translateWithId: L = void 0
         } = e,
         {
-            id: G = "ccs-" + Math.random().toString(36)
+            id: W = "ccs-" + Math.random().toString(36)
         } = e,
         {
             name: A = void 0
         } = e,
         {
             ref: U = null
         } = e;
-    const W = createEventDispatcher();
+    const G = createEventDispatcher();
     let j = -1;
 
     function Q(z) {
         let V = j + z;
         if (c.length === 0) return;
         V < 0 ? V = c.length - 1 : V >= c.length && (V = 0);
         let $ = c[V].disabled;
         for (; $;) V = V + z, V < 0 ? V = c.length - 1 : V >= c.length && (V = 0), $ = c[V].disabled;
         n(21, j = V)
     }
     const F = () => {
-            W("select", {
+            G("select", {
                 selectedId: d,
                 selectedItem: c.find(z => z.id === d)
             })
         },
         te = ({
             target: z
         }) => {
@@ -20802,18 +20796,18 @@
         },
         ce = ({
             target: z
         }) => {
             k || n(1, m = U.contains(z) ? !m : !1)
         };
     return t.$$set = z => {
-        n(28, e = assign(assign({}, e), exclude_internal_props(z))), n(27, o = compute_rest_props(e, a)), "items" in z && n(3, c = z.items), "itemToString" in z && n(4, _ = z.itemToString), "selectedId" in z && n(0, d = z.selectedId), "type" in z && n(5, g = z.type), "direction" in z && n(6, h = z.direction), "size" in z && n(7, p = z.size), "open" in z && n(1, m = z.open), "light" in z && n(8, v = z.light), "disabled" in z && n(9, k = z.disabled), "titleText" in z && n(10, b = z.titleText), "invalid" in z && n(11, E = z.invalid), "invalidText" in z && n(12, w = z.invalidText), "warn" in z && n(13, S = z.warn), "warnText" in z && n(14, I = z.warnText), "helperText" in z && n(15, D = z.helperText), "label" in z && n(16, O = z.label), "hideLabel" in z && n(17, B = z.hideLabel), "translateWithId" in z && n(18, L = z.translateWithId), "id" in z && n(19, G = z.id), "name" in z && n(20, A = z.name), "ref" in z && n(2, U = z.ref), "$$scope" in z && n(37, s = z.$$scope)
+        n(28, e = assign(assign({}, e), exclude_internal_props(z))), n(27, o = compute_rest_props(e, a)), "items" in z && n(3, c = z.items), "itemToString" in z && n(4, _ = z.itemToString), "selectedId" in z && n(0, d = z.selectedId), "type" in z && n(5, g = z.type), "direction" in z && n(6, h = z.direction), "size" in z && n(7, p = z.size), "open" in z && n(1, m = z.open), "light" in z && n(8, v = z.light), "disabled" in z && n(9, k = z.disabled), "titleText" in z && n(10, b = z.titleText), "invalid" in z && n(11, E = z.invalid), "invalidText" in z && n(12, w = z.invalidText), "warn" in z && n(13, S = z.warn), "warnText" in z && n(14, I = z.warnText), "helperText" in z && n(15, D = z.helperText), "label" in z && n(16, O = z.label), "hideLabel" in z && n(17, B = z.hideLabel), "translateWithId" in z && n(18, L = z.translateWithId), "id" in z && n(19, W = z.id), "name" in z && n(20, A = z.name), "ref" in z && n(2, U = z.ref), "$$scope" in z && n(37, s = z.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 32 && n(23, r = g === "inline"), t.$$.dirty[0] & 9 && n(22, l = c.find(z => z.id === d)), t.$$.dirty[0] & 2 && (m || n(21, j = -1))
-    }, e = exclude_internal_props(e), [d, m, U, c, _, g, h, p, v, k, b, E, w, S, I, D, O, B, L, G, A, j, l, r, Q, F, te, o, e, u, Y, oe, ae, C, Z, K, ce, s]
+    }, e = exclude_internal_props(e), [d, m, U, c, _, g, h, p, v, k, b, E, w, S, I, D, O, B, L, W, A, j, l, r, Q, F, te, o, e, u, Y, oe, ae, C, Z, K, ce, s]
 }
 class Dropdown extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$C, create_fragment$C, safe_not_equal, {
             items: 3,
             itemToString: 4,
             selectedId: 0,
@@ -21013,22 +21007,22 @@
         n(0, h = !0), storedGlobalChanged.set(!0), _ && n(5, m = v), S(m)
     };
 
     function L(A) {
         bubble.call(this, t, A)
     }
 
-    function G(A) {
+    function W(A) {
         bubble.call(this, t, A)
     }
     return t.$$set = A => {
         "key" in A && n(1, l = A.key), "value" in A && n(12, a = A.value), "choices" in A && n(2, o = A.choices), "choicesDesc" in A && n(13, u = A.choicesDesc), "activeNavItem" in A && n(14, s = A.activeNavItem), "required" in A && n(15, c = A.required), "readonly" in A && n(3, _ = A.readonly), "pgargs" in A && n(16, d = A.pgargs), "pgargkey" in A && n(4, g = A.pgargkey), "changed" in A && n(0, h = A.changed)
     }, t.$$.update = () => {
         t.$$.dirty & 65554 && n(17, r = get_pgvalue(d, g === !0 ? l : g)), t.$$.dirty & 131077 && r !== void 0 && !h && n(5, m = o.indexOf(r)), t.$$.dirty & 36 && n(12, a = o[m])
-    }, [h, l, o, _, g, m, p, k, b, v, w, S, a, u, s, c, d, r, I, D, O, B, L, G]
+    }, [h, l, o, _, g, m, p, k, b, v, w, S, a, u, s, c, d, r, I, D, O, B, L, W]
 }
 class ChoiceOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$B, create_fragment$B, safe_not_equal, {
             key: 1,
             value: 12,
             choices: 2,
@@ -21265,27 +21259,27 @@
         bubble.call(this, t, C)
     }
 
     function L(C) {
         bubble.call(this, t, C)
     }
 
-    function G(C) {
+    function W(C) {
         bubble.call(this, t, C)
     }
 
     function A(C) {
         bubble.call(this, t, C)
     }
 
     function U(C) {
         bubble.call(this, t, C)
     }
 
-    function W(C) {
+    function G(C) {
         bubble.call(this, t, C)
     }
 
     function j(C) {
         bubble.call(this, t, C)
     }
 
@@ -21315,15 +21309,15 @@
             O = C, n(14, O)
         })
     }
     return t.$$set = C => {
         e = assign(assign({}, e), exclude_internal_props(C)), n(16, o = compute_rest_props(e, a)), "value" in C && n(4, c = C.value), "checked" in C && n(0, _ = C.checked), "group" in C && n(1, d = C.group), "indeterminate" in C && n(5, g = C.indeterminate), "skeleton" in C && n(6, h = C.skeleton), "required" in C && n(7, p = C.required), "readonly" in C && n(8, m = C.readonly), "disabled" in C && n(9, v = C.disabled), "labelText" in C && n(10, k = C.labelText), "hideLabel" in C && n(11, b = C.hideLabel), "name" in C && n(12, E = C.name), "title" in C && n(2, w = C.title), "id" in C && n(13, S = C.id), "ref" in C && n(3, I = C.ref), "$$scope" in C && n(18, s = C.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 2 && n(15, r = Array.isArray(d)), t.$$.dirty[0] & 32787 && n(0, _ = r ? d.includes(c) : _), t.$$.dirty[0] & 1 && D("check", _), t.$$.dirty[0] & 16384 && n(17, l = (O == null ? void 0 : O.offsetWidth) < (O == null ? void 0 : O.scrollWidth)), t.$$.dirty[0] & 147460 && n(2, w = !w && l ? O == null ? void 0 : O.innerText : w)
-    }, [_, d, w, I, c, g, h, p, m, v, k, b, E, S, O, r, o, l, s, u, B, L, G, A, U, W, j, Q, F, te, Y, oe, ae]
+    }, [_, d, w, I, c, g, h, p, m, v, k, b, E, S, O, r, o, l, s, u, B, L, W, A, U, G, j, Q, F, te, Y, oe, ae]
 }
 class Checkbox extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$z, create_fragment$z, safe_not_equal, {
             value: 4,
             checked: 0,
             group: 1,
@@ -22085,24 +22079,24 @@
         {
             filterItem: B = (ne, de) => ne.text.toLowerCase().includes(de.trim().toLowerCase())
         } = e,
         {
             open: L = !1
         } = e,
         {
-            light: G = !1
+            light: W = !1
         } = e,
         {
             locale: A = "en"
         } = e,
         {
             placeholder: U = ""
         } = e,
         {
-            sortItem: W = (ne, de) => ne.text.localeCompare(de.text, A, {
+            sortItem: G = (ne, de) => ne.text.localeCompare(de.text, A, {
                 numeric: !0
             })
         } = e,
         {
             translateWithId: j = void 0
         } = e,
         {
@@ -22183,15 +22177,15 @@
         de < 0 ? de = ve - 1 : de >= ve && (de = 0);
         let Te = p[de].disabled;
         for (; Te;) de = de + ne, de < 0 ? de = p.length - 1 : de >= p.length && (de = 0), Te = p[de].disabled;
         n(28, fe = de)
     }
 
     function T() {
-        return [...u.length > 1 ? u.sort(W) : u, ...s.sort(W)]
+        return [...u.length > 1 ? u.sort(G) : u, ...s.sort(G)]
     }
     afterUpdate(() => {
         u.length !== M.length && (I === "top" && n(29, o = T()), M = u, n(39, k = u.map(({
             id: ne
         }) => ne)), ee("select", {
             selectedIds: k,
             selected: u,
@@ -22298,26 +22292,26 @@
 
     function Oe(ne) {
         binding_callbacks[ne ? "unshift" : "push"](() => {
             re = ne, n(3, re)
         })
     }
     return t.$$set = ne => {
-        n(72, e = assign(assign({}, e), exclude_internal_props(ne))), n(37, d = compute_rest_props(e, _)), "items" in ne && n(38, p = ne.items), "itemToString" in ne && n(7, m = ne.itemToString), "itemToInput" in ne && n(8, v = ne.itemToInput), "selectedIds" in ne && n(39, k = ne.selectedIds), "value" in ne && n(0, b = ne.value), "size" in ne && n(9, E = ne.size), "type" in ne && n(40, w = ne.type), "direction" in ne && n(10, S = ne.direction), "selectionFeedback" in ne && n(41, I = ne.selectionFeedback), "disabled" in ne && n(11, D = ne.disabled), "filterable" in ne && n(12, O = ne.filterable), "filterItem" in ne && n(42, B = ne.filterItem), "open" in ne && n(1, L = ne.open), "light" in ne && n(13, G = ne.light), "locale" in ne && n(43, A = ne.locale), "placeholder" in ne && n(14, U = ne.placeholder), "sortItem" in ne && n(44, W = ne.sortItem), "translateWithId" in ne && n(15, j = ne.translateWithId), "translateWithIdSelection" in ne && n(16, Q = ne.translateWithIdSelection), "titleText" in ne && n(17, F = ne.titleText), "useTitleInItem" in ne && n(18, te = ne.useTitleInItem), "invalid" in ne && n(19, Y = ne.invalid), "invalidText" in ne && n(20, oe = ne.invalidText), "warn" in ne && n(21, ae = ne.warn), "warnText" in ne && n(22, C = ne.warnText), "helperText" in ne && n(23, Z = ne.helperText), "label" in ne && n(24, K = ne.label), "hideLabel" in ne && n(25, ce = ne.hideLabel), "id" in ne && n(26, z = ne.id), "name" in ne && n(27, V = ne.name), "inputRef" in ne && n(2, $ = ne.inputRef), "multiSelectRef" in ne && n(3, re = ne.multiSelectRef), "fieldRef" in ne && n(4, ue = ne.fieldRef), "selectionRef" in ne && n(5, P = ne.selectionRef), "highlightedId" in ne && n(6, q = ne.highlightedId), "$$scope" in ne && n(67, h = ne.$$scope)
+        n(72, e = assign(assign({}, e), exclude_internal_props(ne))), n(37, d = compute_rest_props(e, _)), "items" in ne && n(38, p = ne.items), "itemToString" in ne && n(7, m = ne.itemToString), "itemToInput" in ne && n(8, v = ne.itemToInput), "selectedIds" in ne && n(39, k = ne.selectedIds), "value" in ne && n(0, b = ne.value), "size" in ne && n(9, E = ne.size), "type" in ne && n(40, w = ne.type), "direction" in ne && n(10, S = ne.direction), "selectionFeedback" in ne && n(41, I = ne.selectionFeedback), "disabled" in ne && n(11, D = ne.disabled), "filterable" in ne && n(12, O = ne.filterable), "filterItem" in ne && n(42, B = ne.filterItem), "open" in ne && n(1, L = ne.open), "light" in ne && n(13, W = ne.light), "locale" in ne && n(43, A = ne.locale), "placeholder" in ne && n(14, U = ne.placeholder), "sortItem" in ne && n(44, G = ne.sortItem), "translateWithId" in ne && n(15, j = ne.translateWithId), "translateWithIdSelection" in ne && n(16, Q = ne.translateWithIdSelection), "titleText" in ne && n(17, F = ne.titleText), "useTitleInItem" in ne && n(18, te = ne.useTitleInItem), "invalid" in ne && n(19, Y = ne.invalid), "invalidText" in ne && n(20, oe = ne.invalidText), "warn" in ne && n(21, ae = ne.warn), "warnText" in ne && n(22, C = ne.warnText), "helperText" in ne && n(23, Z = ne.helperText), "label" in ne && n(24, K = ne.label), "hideLabel" in ne && n(25, ce = ne.hideLabel), "id" in ne && n(26, z = ne.id), "name" in ne && n(27, V = ne.name), "inputRef" in ne && n(2, $ = ne.inputRef), "multiSelectRef" in ne && n(3, re = ne.multiSelectRef), "fieldRef" in ne && n(4, ue = ne.fieldRef), "selectionRef" in ne && n(5, P = ne.selectionRef), "highlightedId" in ne && n(6, q = ne.highlightedId), "$$scope" in ne && n(67, h = ne.$$scope)
     }, t.$$.update = () => {
         var ne;
         t.$$.dirty[0] & 67108864 && n(34, r = `menu-${z}`), t.$$.dirty[1] & 512 && n(33, l = w === "inline"), n(32, a = e["aria-label"] || "Choose an item"), t.$$.dirty[1] & 384 && n(29, o = p.map(de => ({
             ...de,
             checked: k.includes(de.id)
         }))), t.$$.dirty[0] & 536870912 && n(31, u = o.filter(({
             checked: de
         }) => de)), t.$$.dirty[0] & 536870912 && (s = o.filter(({
             checked: de
         }) => !de)), t.$$.dirty[0] & 536870913 | t.$$.dirty[1] & 2048 && n(30, c = o.filter(de => B(de, b))), t.$$.dirty[0] & 1879052288 && n(6, q = fe > -1 ? ((ne = (O ? c : o)[fe]) == null ? void 0 : ne.id) ?? null : null)
-    }, e = exclude_internal_props(e), [b, L, $, re, ue, P, q, m, v, E, S, D, O, G, U, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, fe, o, c, u, a, l, r, ee, y, d, p, k, w, I, B, A, W, g, N, J, ie, H, x, se, _e, he, ge, ke, we, be, Se, Ce, Re, le, pe, me, ye, Ee, Oe, h]
+    }, e = exclude_internal_props(e), [b, L, $, re, ue, P, q, m, v, E, S, D, O, W, U, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, fe, o, c, u, a, l, r, ee, y, d, p, k, w, I, B, A, G, g, N, J, ie, H, x, se, _e, he, ge, ke, we, be, Se, Ce, Re, le, pe, me, ye, Ee, Oe, h]
 }
 class MultiSelect extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$y, create_fragment$y, safe_not_equal, {
             items: 38,
             itemToString: 7,
             itemToInput: 8,
@@ -22555,36 +22549,36 @@
     function B(j) {
         bubble.call(this, t, j)
     }
 
     function L(j) {
         bubble.call(this, t, j)
     }
-    const G = () => {
+    const W = () => {
             n(0, m = !0), storedGlobalChanged.set(!0)
         },
         A = j => {
             _ ? n(7, b = E) : S(j.detail.selectedIds)
         };
 
     function U(j) {
         bubble.call(this, t, j)
     }
 
-    function W(j) {
+    function G(j) {
         bubble.call(this, t, j)
     }
     return t.$$set = j => {
         "key" in j && n(1, l = j.key), "value" in j && n(11, a = j.value), "choices" in j && n(2, o = j.choices), "choicesDesc" in j && n(12, u = j.choicesDesc), "required" in j && n(13, s = j.required), "activeNavItem" in j && n(14, c = j.activeNavItem), "readonly" in j && n(3, _ = j.readonly), "setError" in j && n(15, d = j.setError), "removeError" in j && n(16, g = j.removeError), "pgargs" in j && n(17, h = j.pgargs), "pgargkey" in j && n(4, p = j.pgargkey), "changed" in j && n(0, m = j.changed)
     }, t.$$.update = () => {
         if (t.$$.dirty & 131090 && n(18, r = JSON.stringify(get_pgvalue(h, p === !0 ? l : p))), t.$$.dirty & 262149 && r !== void 0 && !m) {
             const j = JSON.parse(r);
             n(7, b = j.map(Q => o.indexOf(Q)))
         }
-    }, [m, l, o, _, p, v, k, b, E, w, S, a, u, s, c, d, g, h, r, I, D, O, B, L, G, A, U, W]
+    }, [m, l, o, _, p, v, k, b, E, w, S, a, u, s, c, d, g, h, r, I, D, O, B, L, W, A, U, G]
 }
 class MChoicesOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$x, create_fragment$x, safe_not_equal, {
             key: 1,
             value: 11,
             choices: 2,
@@ -23073,27 +23067,27 @@
         bubble.call(this, t, Y)
     }
 
     function L(Y) {
         bubble.call(this, t, Y)
     }
 
-    function G(Y) {
+    function W(Y) {
         bubble.call(this, t, Y)
     }
 
     function A(Y) {
         bubble.call(this, t, Y)
     }
 
     function U(Y) {
         bubble.call(this, t, Y)
     }
 
-    function W(Y) {
+    function G(Y) {
         bubble.call(this, t, Y)
     }
 
     function j(Y) {
         bubble.call(this, t, Y)
     }
 
@@ -23105,15 +23099,15 @@
         bubble.call(this, t, Y)
     }
     const te = () => {
         k("close")
     };
     return t.$$set = Y => {
         e = assign(assign({}, e), exclude_internal_props(Y)), n(10, l = compute_rest_props(e, r)), "type" in Y && n(0, s = Y.type), "size" in Y && n(1, c = Y.size), "filter" in Y && n(2, _ = Y.filter), "disabled" in Y && n(3, d = Y.disabled), "interactive" in Y && n(4, g = Y.interactive), "skeleton" in Y && n(5, h = Y.skeleton), "title" in Y && n(6, p = Y.title), "icon" in Y && n(7, m = Y.icon), "id" in Y && n(8, v = Y.id), "$$scope" in Y && n(12, o = Y.$$scope)
-    }, [s, c, _, d, g, h, p, m, v, k, l, u, o, a, b, E, w, S, I, D, O, B, L, G, A, U, W, j, Q, F, te]
+    }, [s, c, _, d, g, h, p, m, v, k, l, u, o, a, b, E, w, S, I, D, O, B, L, W, A, U, G, j, Q, F, te]
 }
 class Tag extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$v, create_fragment$v, safe_not_equal, {
             type: 0,
             size: 1,
             filter: 2,
@@ -23499,41 +23493,41 @@
 
     function B(F) {
         m = F, n(5, m)
     }
     const L = F => {
             F.key === "Enter" && !c && D()
         },
-        G = F => {
+        W = F => {
             n(0, p = !0), storedGlobalChanged.set(!0), I(F.detail)
         };
 
     function A(F) {
         bubble.call(this, t, F)
     }
 
     function U(F) {
         bubble.call(this, t, F)
     }
-    const W = F => {
+    const G = F => {
         O(F)
     };
 
     function j(F) {
         bubble.call(this, t, F)
     }
 
     function Q(F) {
         bubble.call(this, t, F)
     }
     return t.$$set = F => {
         "key" in F && n(1, l = F.key), "value" in F && n(11, a = F.value), "activeNavItem" in F && n(12, o = F.activeNavItem), "required" in F && n(13, u = F.required), "itype" in F && n(14, s = F.itype), "readonly" in F && n(2, c = F.readonly), "setError" in F && n(15, _ = F.setError), "removeError" in F && n(16, d = F.removeError), "pgargs" in F && n(17, g = F.pgargs), "pgargkey" in F && n(3, h = F.pgargkey), "changed" in F && n(0, p = F.changed)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 131082 && n(18, r = JSON.stringify(get_pgvalue(g, h === !0 ? l : h))), t.$$.dirty[0] & 278545 && r !== void 0 && !p && (n(4, v = JSON.parse(r)), n(11, a = v.map(F => applyAtomicType(F, s))))
-    }, [p, l, c, h, v, m, k, b, I, D, O, a, o, u, s, _, d, g, r, B, L, G, A, U, W, j, Q]
+    }, [p, l, c, h, v, m, k, b, I, D, O, a, o, u, s, _, d, g, r, B, L, W, A, U, G, j, Q]
 }
 class ArrayOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$t, create_fragment$t, safe_not_equal, {
             key: 1,
             value: 11,
             activeNavItem: 12,
@@ -23685,59 +23679,59 @@
         } = e,
         m = [],
         v = !1,
         k = "",
         b = a,
         E = a,
         w = null;
-    const S = W => W == null ? "" : typeof W == "string" ? W : JSON.stringify(W, null, 2);
+    const S = G => G == null ? "" : typeof G == "string" ? G : JSON.stringify(G, null, 2);
     a && typeof a == "object" && (b = S(a)), u && (m = ["required", ...m]);
-    const I = (W, j = !1) => {
-        if (E == null && (W === "" || W === null || W === void 0) && !u) {
+    const I = (G, j = !1) => {
+        if (E == null && (G === "" || G === null || G === void 0) && !u) {
             n(10, a = E), n(6, v = !1), d(`${c} / ${l}`);
             return
         }
-        const Q = validateData(W, m);
-        n(6, v = Q !== null), n(7, k = Q), v ? (_(`${c} / ${l}`, k), n(10, a = W)) : (d(`${c} / ${l}`), j || n(10, a = applyAtomicType(W, "auto"))), autoHeight(w)
+        const Q = validateData(G, m);
+        n(6, v = Q !== null), n(7, k = Q), v ? (_(`${c} / ${l}`, k), n(10, a = G)) : (d(`${c} / ${l}`), j || n(10, a = applyAtomicType(G, "auto"))), autoHeight(w)
     };
     onMount(() => {
         s || I(b, !0)
     });
 
-    function D(W) {
-        w = W, n(8, w)
+    function D(G) {
+        w = G, n(8, w)
     }
 
-    function O(W) {
-        b = W, n(5, b), n(16, r), n(0, p), n(15, g), n(4, h), n(1, l)
+    function O(G) {
+        b = G, n(5, b), n(16, r), n(0, p), n(15, g), n(4, h), n(1, l)
     }
 
-    function B(W) {
-        bubble.call(this, t, W)
+    function B(G) {
+        bubble.call(this, t, G)
     }
 
-    function L(W) {
-        bubble.call(this, t, W)
+    function L(G) {
+        bubble.call(this, t, G)
     }
-    const G = W => {
-        n(0, p = !0), storedGlobalChanged.set(!0), I(W.target.value)
+    const W = G => {
+        n(0, p = !0), storedGlobalChanged.set(!0), I(G.target.value)
     };
 
-    function A(W) {
-        bubble.call(this, t, W)
+    function A(G) {
+        bubble.call(this, t, G)
     }
 
-    function U(W) {
-        bubble.call(this, t, W)
+    function U(G) {
+        bubble.call(this, t, G)
     }
-    return t.$$set = W => {
-        "key" in W && n(1, l = W.key), "value" in W && n(10, a = W.value), "placeholder" in W && n(2, o = W.placeholder), "required" in W && n(11, u = W.required), "readonly" in W && n(3, s = W.readonly), "activeNavItem" in W && n(12, c = W.activeNavItem), "setError" in W && n(13, _ = W.setError), "removeError" in W && n(14, d = W.removeError), "pgargs" in W && n(15, g = W.pgargs), "pgargkey" in W && n(4, h = W.pgargkey), "changed" in W && n(0, p = W.changed)
+    return t.$$set = G => {
+        "key" in G && n(1, l = G.key), "value" in G && n(10, a = G.value), "placeholder" in G && n(2, o = G.placeholder), "required" in G && n(11, u = G.required), "readonly" in G && n(3, s = G.readonly), "activeNavItem" in G && n(12, c = G.activeNavItem), "setError" in G && n(13, _ = G.setError), "removeError" in G && n(14, d = G.removeError), "pgargs" in G && n(15, g = G.pgargs), "pgargkey" in G && n(4, h = G.pgargkey), "changed" in G && n(0, p = G.changed)
     }, t.$$.update = () => {
         t.$$.dirty & 32786 && n(16, r = get_pgvalue(g, h === !0 ? l : h)), t.$$.dirty & 65569 && r !== void 0 && !p && (n(5, b = S(r)), n(10, a = applyAtomicType(b, "auto")))
-    }, [p, l, o, s, h, b, v, k, w, I, a, u, c, _, d, g, r, D, O, B, L, G, A, U]
+    }, [p, l, o, s, h, b, v, k, w, I, a, u, c, _, d, g, r, D, O, B, L, W, A, U]
 }
 class AutoOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$s, create_fragment$s, safe_not_equal, {
             key: 1,
             value: 10,
             placeholder: 2,
@@ -23916,69 +23910,69 @@
         }
     }
 }
 
 function create_each_block$8(t, e) {
     let n, r, l, a, o, u, s, c, _, d, g, h, p, m, v, k, b, E;
 
-    function w(G) {
-        e[7](G, e[17])
+    function w(W) {
+        e[7](W, e[17])
     }
     let S = {
         size: "sm",
         title: e[15][0] ? e[15][0] : e[2],
         placeholder: e[2]
     };
     e[0][e[17]][0] !== void 0 && (S.value = e[0][e[17]][0]), l = new TextInput$1({
         props: S
     }), binding_callbacks.push(() => bind(l, "value", w)), l.$on("focus", e[8]), l.$on("blur", e[9]);
 
-    function I(G) {
-        e[10](G, e[17])
+    function I(W) {
+        e[10](W, e[17])
     }
     let D = {
         size: "sm"
     };
     e[0][e[17]][1] !== void 0 && (D.value = e[0][e[17]][1]), _ = new TextInput$1({
         props: D
     }), binding_callbacks.push(() => bind(_, "value", I)), _.$on("focus", e[11]), _.$on("blur", e[12]);
     const O = [create_if_block$k, create_else_block$a],
         B = [];
 
-    function L(G, A) {
-        return G[17] == G[0].length - 1 ? 0 : 1
+    function L(W, A) {
+        return W[17] == W[0].length - 1 ? 0 : 1
     }
     return p = L(e), m = B[p] = O[p](e), {
         key: t,
         first: null,
         c() {
             n = element("form"), r = element("div"), create_component(l.$$.fragment), o = space(), u = element("div"), u.textContent = "=", s = space(), c = element("div"), create_component(_.$$.fragment), g = space(), h = element("div"), m.c(), v = space(), attr(r, "class", "morelike-label svelte-1vanu9d"), attr(u, "class", "morelike-equal"), attr(c, "class", "morelike-value svelte-1vanu9d"), attr(h, "class", "morelike-action"), attr(n, "class", "morelike-wrapper svelte-1vanu9d"), this.first = n
         },
-        m(G, A) {
-            insert(G, n, A), append(n, r), mount_component(l, r, null), append(n, o), append(n, u), append(n, s), append(n, c), mount_component(_, c, null), append(n, g), append(n, h), B[p].m(h, null), append(n, v), k = !0, b || (E = [listen(n, "mouseenter", e[5]), listen(n, "mouseleave", e[6])], b = !0)
+        m(W, A) {
+            insert(W, n, A), append(n, r), mount_component(l, r, null), append(n, o), append(n, u), append(n, s), append(n, c), mount_component(_, c, null), append(n, g), append(n, h), B[p].m(h, null), append(n, v), k = !0, b || (E = [listen(n, "mouseenter", e[5]), listen(n, "mouseleave", e[6])], b = !0)
         },
-        p(G, A) {
-            e = G;
+        p(W, A) {
+            e = W;
             const U = {};
             A & 5 && (U.title = e[15][0] ? e[15][0] : e[2]), A & 4 && (U.placeholder = e[2]), !a && A & 1 && (a = !0, U.value = e[0][e[17]][0], add_flush_callback(() => a = !1)), l.$set(U);
-            const W = {};
-            !d && A & 1 && (d = !0, W.value = e[0][e[17]][1], add_flush_callback(() => d = !1)), _.$set(W);
+            const G = {};
+            !d && A & 1 && (d = !0, G.value = e[0][e[17]][1], add_flush_callback(() => d = !1)), _.$set(G);
             let j = p;
             p = L(e), p === j ? B[p].p(e, A) : (group_outros(), transition_out(B[j], 1, 1, () => {
                 B[j] = null
             }), check_outros(), m = B[p], m ? m.p(e, A) : (m = B[p] = O[p](e), m.c()), transition_in(m, 1), m.m(h, null))
         },
-        i(G) {
-            k || (transition_in(l.$$.fragment, G), transition_in(_.$$.fragment, G), transition_in(m), k = !0)
+        i(W) {
+            k || (transition_in(l.$$.fragment, W), transition_in(_.$$.fragment, W), transition_in(m), k = !0)
         },
-        o(G) {
-            transition_out(l.$$.fragment, G), transition_out(_.$$.fragment, G), transition_out(m), k = !1
+        o(W) {
+            transition_out(l.$$.fragment, W), transition_out(_.$$.fragment, W), transition_out(m), k = !1
         },
-        d(G) {
-            G && detach(n), destroy_component(l), destroy_component(_), B[p].d(), b = !1, run_all(E)
+        d(W) {
+            W && detach(n), destroy_component(l), destroy_component(_), B[p].d(), b = !1, run_all(E)
         }
     }
 }
 
 function create_fragment$q(t) {
     let e = [],
         n = new Map,
@@ -24220,21 +24214,21 @@
         m = ["json"],
         v = !1,
         k = "",
         b = a,
         E = a,
         w = null;
     a && typeof a == "object" && (b = JSON.stringify(a, null, 2)), u && (m = ["required", ...m]);
-    const S = (U, W = !1) => {
+    const S = (U, G = !1) => {
         if (E == null && (U === "" || U === null || U === void 0) && !u) {
             n(10, a = E), n(6, v = !1), d(`${s} / ${l}`);
             return
         }
         const j = validateData(U, m);
-        n(6, v = j !== null), n(7, k = j), v ? (_(`${s} / ${l}`, k), n(10, a = U)) : (d(`${s} / ${l}`), W || n(10, a = JSON.parse(U))), autoHeight(w)
+        n(6, v = j !== null), n(7, k = j), v ? (_(`${s} / ${l}`, k), n(10, a = U)) : (d(`${s} / ${l}`), G || n(10, a = JSON.parse(U))), autoHeight(w)
     };
     onMount(() => {
         c || S(b, !0)
     });
 
     function I(U) {
         b = U, n(5, b), n(16, r), n(0, p), n(15, g), n(4, h), n(1, l)
@@ -24251,26 +24245,26 @@
     function B(U) {
         bubble.call(this, t, U)
     }
     const L = U => {
         n(0, p = !0), storedGlobalChanged.set(!0), S(U.target.value)
     };
 
-    function G(U) {
+    function W(U) {
         bubble.call(this, t, U)
     }
 
     function A(U) {
         bubble.call(this, t, U)
     }
     return t.$$set = U => {
         "key" in U && n(1, l = U.key), "value" in U && n(10, a = U.value), "placeholder" in U && n(2, o = U.placeholder), "required" in U && n(11, u = U.required), "activeNavItem" in U && n(12, s = U.activeNavItem), "readonly" in U && n(3, c = U.readonly), "setError" in U && n(13, _ = U.setError), "removeError" in U && n(14, d = U.removeError), "pgargs" in U && n(15, g = U.pgargs), "pgargkey" in U && n(4, h = U.pgargkey), "changed" in U && n(0, p = U.changed)
     }, t.$$.update = () => {
         t.$$.dirty & 32786 && n(16, r = JSON.stringify(get_pgvalue(g, h === !0 ? l : h))), t.$$.dirty & 65569 && r !== void 0 && !p && (n(5, b = r), n(10, a = JSON.parse(b)))
-    }, [p, l, o, c, h, b, v, k, w, S, a, u, s, _, d, g, r, I, D, O, B, L, G, A]
+    }, [p, l, o, c, h, b, v, k, w, S, a, u, s, _, d, g, r, I, D, O, B, L, W, A]
 }
 class JsonOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$p, create_fragment$p, safe_not_equal, {
             key: 1,
             value: 10,
             placeholder: 2,
@@ -24796,27 +24790,27 @@
         t.$$.not_equal(a.changed, Y) && (a.changed = Y, n(0, a))
     }
 
     function L(Y) {
         t.$$.not_equal(a.value, Y) && (a.value = Y, n(0, a))
     }
 
-    function G(Y) {
+    function W(Y) {
         t.$$.not_equal(a.changed, Y) && (a.changed = Y, n(0, a))
     }
 
     function A(Y) {
         t.$$.not_equal(a.value, Y) && (a.value = Y, n(0, a))
     }
 
     function U(Y) {
         t.$$.not_equal(a.changed, Y) && (a.changed = Y, n(0, a))
     }
 
-    function W(Y) {
+    function G(Y) {
         t.$$.not_equal(a.value, Y) && (a.value = Y, n(0, a))
     }
 
     function j(Y) {
         t.$$.not_equal(a.changed, Y) && (a.changed = Y, n(0, a))
     }
 
@@ -24829,15 +24823,15 @@
     }
 
     function te(Y) {
         t.$$.not_equal(a.value, Y) && (a.value = Y, n(0, a))
     }
     return t.$$set = Y => {
         "key" in Y && n(1, l = Y.key), "data" in Y && n(0, a = Y.data), "activeNavItem" in Y && n(2, o = Y.activeNavItem), "description" in Y && n(11, u = Y.description), "readonly" in Y && n(3, s = Y.readonly), "setError" in Y && n(4, c = Y.setError), "removeError" in Y && n(5, _ = Y.removeError), "pgargs" in Y && n(6, d = Y.pgargs)
-    }, [a, l, o, s, c, _, d, h, p, m, v, u, k, b, E, w, S, I, D, O, B, L, G, A, U, W, j, Q, F, te]
+    }, [a, l, o, s, c, _, d, h, p, m, v, u, k, b, E, w, S, I, D, O, B, L, W, A, U, G, j, Q, F, te]
 }
 class NonNSOption extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$o, create_fragment$o, safe_not_equal, {
             key: 1,
             data: 0,
             activeNavItem: 2,
@@ -27005,27 +26999,27 @@
             for (let Z in a.value) C[Z] = a.value[Z].value;
             n(6, m = a.command.replace(/\$\{(\w+)\}/g, (Z, K) => C[K])), n(4, h = !1)
         };
 
     function L(C) {
         g = C, n(2, g)
     }
-    const G = () => {
+    const W = () => {
         n(2, g = !1)
     };
 
     function A(C, Z) {
         t.$$.not_equal(a.value[Z], C) && (a.value[Z] = C, n(0, a))
     }
 
     function U(C) {
         u = C, n(1, u)
     }
 
-    function W(C, Z) {
+    function G(C, Z) {
         t.$$.not_equal(a.value[Z], C) && (a.value[Z] = C, n(0, a))
     }
 
     function j(C) {
         u = C, n(1, u)
     }
     const Q = () => {
@@ -27044,15 +27038,15 @@
         E = C, n(9, E)
     }
     const ae = () => n(7, v.kind = void 0, v);
     return t.$$set = C => {
         "data" in C && n(0, a = C.data), "config_data" in C && n(16, o = C.config_data), "description" in C && n(1, u = C.description), "initDescription" in C && n(17, s = C.initDescription), "activeNavItem" in C && n(3, c = C.activeNavItem), "runStarted" in C && n(15, _ = C.runStarted), "saveConfig" in C && n(18, d = C.saveConfig), "openConfirm" in C && n(2, g = C.openConfirm)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 1 && (n(0, a), B()), t.$$.dirty[0] & 1 && n(10, r = a.value[a.configfile].value)
-    }, [a, u, g, c, h, p, m, v, b, E, r, w, S, D, O, _, o, s, d, L, G, A, U, W, j, Q, F, te, Y, oe, ae]
+    }, [a, u, g, c, h, p, m, v, b, E, r, w, S, D, O, _, o, s, d, L, W, A, U, G, j, Q, F, te, Y, oe, ae]
 }
 class RunningOptions extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$i, create_fragment$i, safe_not_equal, {
             data: 0,
             config_data: 16,
             description: 1,
@@ -27092,28 +27086,28 @@
         O = create_slot(D, t, t[12], get_actions_slot_context);
     let B = !t[5] && create_if_block_1$8(t),
         L = [{
             role: t[2]
         }, {
             kind: t[0]
         }, t[10]],
-        G = {};
-    for (let A = 0; A < L.length; A += 1) G = assign(G, L[A]);
+        W = {};
+    for (let A = 0; A < L.length; A += 1) W = assign(W, L[A]);
     return {
         c() {
-            e = element("div"), n = element("div"), create_component(r.$$.fragment), l = space(), a = element("div"), o = element("p"), k && k.c(), u = space(), s = element("div"), w && w.c(), c = space(), I && I.c(), _ = space(), O && O.c(), d = space(), B && B.c(), toggle_class(o, "bx--inline-notification__title", !0), toggle_class(s, "bx--inline-notification__subtitle", !0), toggle_class(a, "bx--inline-notification__text-wrapper", !0), toggle_class(n, "bx--inline-notification__details", !0), set_attributes(e, G), toggle_class(e, "bx--inline-notification", !0), toggle_class(e, "bx--inline-notification--low-contrast", t[1]), toggle_class(e, "bx--inline-notification--hide-close-button", t[5]), toggle_class(e, "bx--inline-notification--error", t[0] === "error"), toggle_class(e, "bx--inline-notification--info", t[0] === "info"), toggle_class(e, "bx--inline-notification--info-square", t[0] === "info-square"), toggle_class(e, "bx--inline-notification--success", t[0] === "success"), toggle_class(e, "bx--inline-notification--warning", t[0] === "warning"), toggle_class(e, "bx--inline-notification--warning-alt", t[0] === "warning-alt")
+            e = element("div"), n = element("div"), create_component(r.$$.fragment), l = space(), a = element("div"), o = element("p"), k && k.c(), u = space(), s = element("div"), w && w.c(), c = space(), I && I.c(), _ = space(), O && O.c(), d = space(), B && B.c(), toggle_class(o, "bx--inline-notification__title", !0), toggle_class(s, "bx--inline-notification__subtitle", !0), toggle_class(a, "bx--inline-notification__text-wrapper", !0), toggle_class(n, "bx--inline-notification__details", !0), set_attributes(e, W), toggle_class(e, "bx--inline-notification", !0), toggle_class(e, "bx--inline-notification--low-contrast", t[1]), toggle_class(e, "bx--inline-notification--hide-close-button", t[5]), toggle_class(e, "bx--inline-notification--error", t[0] === "error"), toggle_class(e, "bx--inline-notification--info", t[0] === "info"), toggle_class(e, "bx--inline-notification--info-square", t[0] === "info-square"), toggle_class(e, "bx--inline-notification--success", t[0] === "success"), toggle_class(e, "bx--inline-notification--warning", t[0] === "warning"), toggle_class(e, "bx--inline-notification--warning-alt", t[0] === "warning-alt")
         },
         m(A, U) {
             insert(A, e, U), append(e, n), mount_component(r, n, null), append(n, l), append(n, a), append(a, o), k && k.m(o, null), append(a, u), append(a, s), w && w.m(s, null), append(a, c), I && I.m(a, null), append(e, _), O && O.m(e, null), append(e, d), B && B.m(e, null), g = !0, h || (p = [listen(e, "click", t[14]), listen(e, "mouseover", t[15]), listen(e, "mouseenter", t[16]), listen(e, "mouseleave", t[17])], h = !0)
         },
         p(A, U) {
-            const W = {};
-            U & 1 && (W.kind = A[0]), U & 64 && (W.iconDescription = A[6]), r.$set(W), v ? v.p && (!g || U & 4096) && update_slot_base(v, m, A, A[12], g ? get_slot_changes(m, A[12], U, get_title_slot_changes) : get_all_dirty_from_scope(A[12]), get_title_slot_context) : k && k.p && (!g || U & 8) && k.p(A, g ? U : -1), E ? E.p && (!g || U & 4096) && update_slot_base(E, b, A, A[12], g ? get_slot_changes(b, A[12], U, get_subtitle_slot_changes) : get_all_dirty_from_scope(A[12]), get_subtitle_slot_context) : w && w.p && (!g || U & 16) && w.p(A, g ? U : -1), I && I.p && (!g || U & 4096) && update_slot_base(I, S, A, A[12], g ? get_slot_changes(S, A[12], U, null) : get_all_dirty_from_scope(A[12]), null), O && O.p && (!g || U & 4096) && update_slot_base(O, D, A, A[12], g ? get_slot_changes(D, A[12], U, get_actions_slot_changes) : get_all_dirty_from_scope(A[12]), get_actions_slot_context), A[5] ? B && (group_outros(), transition_out(B, 1, 1, () => {
+            const G = {};
+            U & 1 && (G.kind = A[0]), U & 64 && (G.iconDescription = A[6]), r.$set(G), v ? v.p && (!g || U & 4096) && update_slot_base(v, m, A, A[12], g ? get_slot_changes(m, A[12], U, get_title_slot_changes) : get_all_dirty_from_scope(A[12]), get_title_slot_context) : k && k.p && (!g || U & 8) && k.p(A, g ? U : -1), E ? E.p && (!g || U & 4096) && update_slot_base(E, b, A, A[12], g ? get_slot_changes(b, A[12], U, get_subtitle_slot_changes) : get_all_dirty_from_scope(A[12]), get_subtitle_slot_context) : w && w.p && (!g || U & 16) && w.p(A, g ? U : -1), I && I.p && (!g || U & 4096) && update_slot_base(I, S, A, A[12], g ? get_slot_changes(S, A[12], U, null) : get_all_dirty_from_scope(A[12]), null), O && O.p && (!g || U & 4096) && update_slot_base(O, D, A, A[12], g ? get_slot_changes(D, A[12], U, get_actions_slot_changes) : get_all_dirty_from_scope(A[12]), get_actions_slot_context), A[5] ? B && (group_outros(), transition_out(B, 1, 1, () => {
                 B = null
-            }), check_outros()) : B ? (B.p(A, U), U & 32 && transition_in(B, 1)) : (B = create_if_block_1$8(A), B.c(), transition_in(B, 1), B.m(e, null)), set_attributes(e, G = get_spread_update(L, [(!g || U & 4) && {
+            }), check_outros()) : B ? (B.p(A, U), U & 32 && transition_in(B, 1)) : (B = create_if_block_1$8(A), B.c(), transition_in(B, 1), B.m(e, null)), set_attributes(e, W = get_spread_update(L, [(!g || U & 4) && {
                 role: A[2]
             }, (!g || U & 1) && {
                 kind: A[0]
             }, U & 1024 && A[10]])), toggle_class(e, "bx--inline-notification", !0), toggle_class(e, "bx--inline-notification--low-contrast", A[1]), toggle_class(e, "bx--inline-notification--hide-close-button", A[5]), toggle_class(e, "bx--inline-notification--error", A[0] === "error"), toggle_class(e, "bx--inline-notification--info", A[0] === "info"), toggle_class(e, "bx--inline-notification--info-square", A[0] === "info-square"), toggle_class(e, "bx--inline-notification--success", A[0] === "success"), toggle_class(e, "bx--inline-notification--warning", A[0] === "warning"), toggle_class(e, "bx--inline-notification--warning-alt", A[0] === "warning-alt")
         },
         i(A) {
             g || (transition_in(r.$$.fragment, A), transition_in(k, A), transition_in(w, A), transition_in(I, A), transition_in(O, A), transition_in(B), g = !0)
@@ -28680,15 +28674,15 @@
             r && detach(e)
         }
     }
 }
 
 function create_fragment$f(t) {
     let e, n, r, l, a, o, u, s, c, _ = t[0][SECTION_PROCESSES] && Object.keys(t[0][SECTION_PROCESSES]).length > 0,
-        d, g, h, p, m, v, k, b, E, w, S, I, D, O, B, L, G, A, U, W = t[1] && !t[1].startsWith("new:"),
+        d, g, h, p, m, v, k, b, E, w, S, I, D, O, B, L, W, A, U, G = t[1] && !t[1].startsWith("new:"),
         j, Q, F, te, Y, oe, ae, C, Z, K;
 
     function ce(x) {
         t[22](x)
     }
     let z = {
         passiveModal: !0,
@@ -28750,31 +28744,31 @@
             },
             $$scope: {
                 ctx: t
             }
         }
     }), L.$on("click", t[47]);
     let J = t[1] && create_if_block_2$7(t),
-        ie = W && create_if_block_1$7(t);
+        ie = G && create_if_block_1$7(t);
     Y = new Description({
         props: {
             description: t[9]
         }
     });
     let H = t[8].kind && create_if_block$c(t);
     return {
         c() {
             create_component(e.$$.fragment), r = space(), l = element("div"), a = element("aside"), create_component(o.$$.fragment), s = space(), re && re.c(), c = space(), ue && ue.c(), d = space(), P && P.c(), g = space(), q && q.c(), h = space(), p = element("main"), ee && ee.c(), m = space(), X && X.c(), v = space();
             for (let x = 0; x < M.length; x += 1) M[x].c();
-            k = space(), T && T.c(), b = space(), N && N.c(), E = space(), w = element("div"), S = element("div"), create_component(I.$$.fragment), D = space(), O = element("span"), B = space(), create_component(L.$$.fragment), G = space(), J && J.c(), A = space(), U = element("div"), ie && ie.c(), j = space(), Q = element("div"), F = space(), te = element("aside"), create_component(Y.$$.fragment), oe = space(), H && H.c(), ae = empty(), attr(a, "class", "left svelte-q1isj3"), attr(p, "class", "svelte-q1isj3"), attr(O, "class", "separator svelte-q1isj3"), attr(S, "class", "actions-left svelte-q1isj3"), attr(U, "class", "actions-right svelte-q1isj3"), attr(w, "class", "actions svelte-q1isj3"), attr(Q, "class", "draggable"), attr(te, "class", "right svelte-q1isj3"), attr(l, "class", "container svelte-q1isj3"), attr(l, "id", "container")
+            k = space(), T && T.c(), b = space(), N && N.c(), E = space(), w = element("div"), S = element("div"), create_component(I.$$.fragment), D = space(), O = element("span"), B = space(), create_component(L.$$.fragment), W = space(), J && J.c(), A = space(), U = element("div"), ie && ie.c(), j = space(), Q = element("div"), F = space(), te = element("aside"), create_component(Y.$$.fragment), oe = space(), H && H.c(), ae = empty(), attr(a, "class", "left svelte-q1isj3"), attr(p, "class", "svelte-q1isj3"), attr(O, "class", "separator svelte-q1isj3"), attr(S, "class", "actions-left svelte-q1isj3"), attr(U, "class", "actions-right svelte-q1isj3"), attr(w, "class", "actions svelte-q1isj3"), attr(Q, "class", "draggable"), attr(te, "class", "right svelte-q1isj3"), attr(l, "class", "container svelte-q1isj3"), attr(l, "id", "container")
         },
         m(x, se) {
             mount_component(e, x, se), insert(x, r, se), insert(x, l, se), append(l, a), mount_component(o, a, null), append(a, s), re && re.m(a, null), append(a, c), ue && ue.m(a, null), append(a, d), P && P.m(a, null), append(a, g), q && q.m(a, null), append(l, h), append(l, p), ee && ee.m(p, null), append(p, m), X && X.m(p, null), append(p, v);
             for (let _e = 0; _e < M.length; _e += 1) M[_e] && M[_e].m(p, null);
-            append(p, k), T && T.m(p, null), append(p, b), N && N.m(p, null), append(l, E), append(l, w), append(w, S), mount_component(I, S, null), append(S, D), append(S, O), append(S, B), mount_component(L, S, null), append(S, G), J && J.m(S, null), append(w, A), append(w, U), ie && ie.m(U, null), append(l, j), append(l, Q), append(l, F), append(l, te), mount_component(Y, te, null), insert(x, oe, se), H && H.m(x, se), insert(x, ae, se), C = !0, Z || (K = [listen(window, "mouseup", t[13]), listen(window, "mousemove", t[12]), listen(Q, "mousedown", t[11]), listen(te, "mouseenter", t[49]), listen(te, "mouseleave", t[50])], Z = !0)
+            append(p, k), T && T.m(p, null), append(p, b), N && N.m(p, null), append(l, E), append(l, w), append(w, S), mount_component(I, S, null), append(S, D), append(S, O), append(S, B), mount_component(L, S, null), append(S, W), J && J.m(S, null), append(w, A), append(w, U), ie && ie.m(U, null), append(l, j), append(l, Q), append(l, F), append(l, te), mount_component(Y, te, null), insert(x, oe, se), H && H.m(x, se), insert(x, ae, se), C = !0, Z || (K = [listen(window, "mouseup", t[13]), listen(window, "mousemove", t[12]), listen(Q, "mousedown", t[11]), listen(te, "mouseenter", t[49]), listen(te, "mouseleave", t[50])], Z = !0)
         },
         p(x, se) {
             const _e = {};
             se[0] & 32 | se[2] & 8192 && (_e.$$scope = {
                 dirty: se,
                 ctx: x
             }), !n && se[0] & 64 && (n = !0, _e.open = x[6], add_flush_callback(() => n = !1)), e.$set(_e);
@@ -28813,15 +28807,15 @@
             }), I.$set(ge);
             const ke = {};
             se[0] & 1152 && (ke.disabled = x[7] || !x[10]), se[2] & 8192 && (ke.$$scope = {
                 dirty: se,
                 ctx: x
             }), L.$set(ke), x[1] ? J ? (J.p(x, se), se[0] & 2 && transition_in(J, 1)) : (J = create_if_block_2$7(x), J.c(), transition_in(J, 1), J.m(S, null)) : J && (group_outros(), transition_out(J, 1, 1, () => {
                 J = null
-            }), check_outros()), se[0] & 2 && (W = x[1] && !x[1].startsWith("new:")), W ? ie ? (ie.p(x, se), se[0] & 2 && transition_in(ie, 1)) : (ie = create_if_block_1$7(x), ie.c(), transition_in(ie, 1), ie.m(U, null)) : ie && (group_outros(), transition_out(ie, 1, 1, () => {
+            }), check_outros()), se[0] & 2 && (G = x[1] && !x[1].startsWith("new:")), G ? ie ? (ie.p(x, se), se[0] & 2 && transition_in(ie, 1)) : (ie = create_if_block_1$7(x), ie.c(), transition_in(ie, 1), ie.m(U, null)) : ie && (group_outros(), transition_out(ie, 1, 1, () => {
                 ie = null
             }), check_outros());
             const we = {};
             se[0] & 512 && (we.description = x[9]), Y.$set(we), x[8].kind ? H ? (H.p(x, se), se[0] & 256 && transition_in(H, 1)) : (H = create_if_block$c(x), H.c(), transition_in(H, 1), H.m(ae.parentNode, ae)) : H && (group_outros(), transition_out(H, 1, 1, () => {
                 H = null
             }), check_outros())
         },
@@ -28952,29 +28946,29 @@
         }, L = function() {
             const H = JSON.stringify(d, null, 4),
                 x = document.createElement("a"),
                 se = new Blob([H], {
                     type: "text/json"
                 });
             x.href = URL.createObjectURL(se), x.download = `${d[SECTION_PIPELINE_OPTS].name.value}.schema.json`, document.body.appendChild(x), x.click(), x.remove()
-        }, G = H => {
+        }, W = H => {
             const x = H.split("."),
                 se = x.at(-2).substring(0, 6) + "..";
             return x.splice(-2, 1, se), x.join(".")
         };
 
     function A(H) {
         p = H, n(6, p)
     }
 
     function U(H) {
         g = H, n(3, g)
     }
 
-    function W(H) {
+    function G(H) {
         g = H, n(3, g)
     }
     const j = (H, x) => d[SECTION_PROCESSES][H].order - d[SECTION_PROCESSES][x].order;
 
     function Q(H) {
         g = H, n(3, g)
     }
@@ -29057,15 +29051,15 @@
         N = H => descFocused.set(!0),
         J = H => descFocused.set(!1),
         ie = () => n(8, b.kind = void 0, b);
     return t.$$set = H => {
         "pipelineDesc" in H && n(19, o = H.pipelineDesc), "configfile" in H && n(1, u = H.configfile), "histories" in H && n(20, s = H.histories), "runStarted" in H && n(2, c = H.runStarted), "finished" in H && n(21, _ = H.finished), "data" in H && n(0, d = H.data)
     }, t.$$.update = () => {
         t.$$.dirty[0] & 24 && n(9, r = E || DEFAULT_DESCRIPTIONS[g]), t.$$.dirty[0] & 1 && n(19, o = d[SECTION_PIPELINE_OPTS].desc.value)
-    }, [d, u, c, g, E, h, p, m, b, r, a, w, S, I, D, O, B, L, G, o, s, _, A, U, W, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P, q, ee, X, fe, M, y, T, N, J, ie]
+    }, [d, u, c, g, E, h, p, m, b, r, a, w, S, I, D, O, B, L, W, o, s, _, A, U, G, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P, q, ee, X, fe, M, y, T, N, J, ie]
 }
 class Configuration extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$f, create_fragment$f, safe_not_equal, {
             pipelineDesc: 19,
             configfile: 1,
             histories: 20,
@@ -30177,30 +30171,30 @@
     const L = () => {
         const F = computeTreeLeafDepth(v);
         return r ? F + 1 : p ? F + 2 : F + 2.5
     };
     afterUpdate(() => {
         d === u && k !== u && (s.includes(d) || I(l)), k = u
     });
-    const G = () => {
+    const W = () => {
         h || (n(7, a = !a), D(l, a), B(l))
     };
 
     function A(F) {
         binding_callbacks[F ? "unshift" : "push"](() => {
             v = F, n(6, v)
         })
     }
 
     function U(F) {
         binding_callbacks[F ? "unshift" : "push"](() => {
             m = F, n(9, m)
         })
     }
-    const W = () => {
+    const G = () => {
             h || S(l)
         },
         j = F => {
             var te;
             if ((F.key === "ArrowLeft" || F.key === "ArrowRight" || F.key === "Enter") && F.stopPropagation(), r && F.key === "ArrowLeft" && (n(7, a = !1), D(l, !1), B(l)), r && F.key === "ArrowRight" && (a ? (te = m.lastChild.firstElementChild) == null || te.focus() : (n(7, a = !0), D(l, !0), B(l))), F.key === "Enter" || F.key === " ") {
                 if (F.preventDefault(), h) return;
                 n(7, a = !a), B(l), S(l), D(l, a), m.focus()
@@ -30214,15 +30208,15 @@
     }, t.$$.update = () => {
         t.$$.dirty[0] & 1 && n(8, r = Array.isArray(c)), t.$$.dirty[0] & 1048580 && n(7, a = o.includes(d)), t.$$.dirty[0] & 396 && n(10, l = {
             id: d,
             text: g,
             expanded: a,
             leaf: !r
         }), t.$$.dirty[0] & 64 && v && (n(6, v.style.marginLeft = `-${L()}rem`, v), n(6, v.style.paddingLeft = `${L()}rem`, v))
-    }, [c, _, d, g, h, p, v, a, r, m, l, u, s, b, E, w, S, D, O, B, o, G, A, U, W, j, Q]
+    }, [c, _, d, g, h, p, v, a, r, m, l, u, s, b, E, w, S, D, O, B, o, W, A, U, G, j, Q]
 }
 class TreeViewNodeList extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$8, create_fragment$8, safe_not_equal, {
             children: 0,
             root: 1,
             id: 2,
@@ -30402,15 +30396,15 @@
         expandNode: (j, Q) => {
             Q ? n(10, g = [...g, j.id]) : n(10, g = g.filter(F => F !== j.id))
         },
         focusNode: j => w("focus", j),
         toggleNode: j => w("toggle", j)
     });
 
-    function G(j) {
+    function W(j) {
         (j.key === "ArrowUp" || j.key === "ArrowDown") && j.preventDefault(), L.currentNode = j.target;
         let Q = null;
         j.key === "ArrowUp" && (Q = L.previousNode()), j.key === "ArrowDown" && (Q = L.nextNode()), Q && Q !== j.target && (Q.tabIndex = "0", Q.focus())
     }
     onMount(() => {
         const j = B.querySelector("li.bx--tree-node:not(.bx--tree-node--disabled)");
         j != null && (j.tabIndex = "0")
@@ -30423,26 +30417,26 @@
         }), Q
     }
 
     function U(j) {
         bubble.call(this, t, j)
     }
 
-    function W(j) {
+    function G(j) {
         binding_callbacks[j ? "unshift" : "push"](() => {
             B = j, n(5, B)
         })
     }
     return t.$$set = j => {
         e = assign(assign({}, e), exclude_internal_props(j)), n(8, o = compute_rest_props(e, a)), "children" in j && n(1, c = j.children), "activeId" in j && n(9, _ = j.activeId), "selectedIds" in j && n(0, d = j.selectedIds), "expandedIds" in j && n(10, g = j.expandedIds), "size" in j && n(2, h = j.size), "labelText" in j && n(3, p = j.labelText), "hideLabel" in j && n(4, m = j.hideLabel), "$$scope" in j && n(16, s = j.$$scope)
     }, t.$$.update = () => {
         t.$$.dirty & 2 && n(15, r = A(c)), t.$$.dirty & 32768 && (l = r.map(j => j.id)), t.$$.dirty & 512 && I.set(_), t.$$.dirty & 1 && D.set(d), t.$$.dirty & 1024 && O.set(g), t.$$.dirty & 32 && B && (L = document.createTreeWalker(B, NodeFilter.SHOW_ELEMENT, {
             acceptNode: j => j.classList.contains("bx--tree-node--disabled") ? NodeFilter.FILTER_REJECT : j.matches("li.bx--tree-node") ? NodeFilter.FILTER_ACCEPT : NodeFilter.FILTER_SKIP
         }))
-    }, [d, c, h, p, m, B, S, G, o, _, g, v, k, b, E, r, s, u, U, W]
+    }, [d, c, h, p, m, B, S, W, o, _, g, v, k, b, E, r, s, u, U, G]
 }
 class TreeView extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$7, create_fragment$7, safe_not_equal, {
             children: 1,
             activeId: 9,
             selectedIds: 0,
@@ -31078,62 +31072,62 @@
     const B = Q => Q[27];
     for (let Q = 0; Q < O.length; Q += 1) {
         let F = get_each_context$1(t, O, Q),
             te = B(F);
         a.set(te, l[Q] = create_each_block$1(te, F))
     }
     const L = [create_if_block_4$1, create_else_block_2$1],
-        G = [];
+        W = [];
 
     function A(Q, F) {
         return Q[3] !== void 0 ? 0 : 1
     }
-    _ = A(t), d = G[_] = L[_](t);
+    _ = A(t), d = W[_] = L[_](t);
     const U = [create_if_block_2$3, create_if_block_3$2, create_else_block_1$2],
-        W = [];
+        G = [];
 
     function j(Q, F) {
         return Q[3] === void 0 ? 0 : Q[7] ? 2 : 1
     }
-    return b = j(t), E = W[b] = U[b](t), {
+    return b = j(t), E = G[b] = U[b](t), {
         c() {
             e = element("div"), n = element("div"), r = element("div");
             for (let Q = 0; Q < l.length; Q += 1) l[Q].c();
             o = space(), u = element("div"), s = space(), c = element("div"), d.c(), h = space(), p = element("div"), m = space(), v = element("div"), k = element("div"), E.c(), attr(r, "class", "joblist svelte-1302pl0"), attr(n, "class", "jobs svelte-1302pl0"), attr(u, "class", "draggable row svelte-1302pl0"), attr(c, "class", g = "tree scrollable " + (t[2][t[3]] || "") + " svelte-1302pl0"), attr(p, "class", "draggable svelte-1302pl0"), attr(k, "class", "jobdetail svelte-1302pl0"), attr(v, "class", "details svelte-1302pl0"), attr(e, "class", "procrun-wrap svelte-1302pl0"), attr(e, "id", "procrun-wrap"), attr(e, "style", w = t[2].length === 1 ? "--jobs-height: 0" : "")
         },
         m(Q, F) {
             insert(Q, e, F), append(e, n), append(n, r);
             for (let te = 0; te < l.length; te += 1) l[te] && l[te].m(r, null);
-            append(e, o), append(e, u), append(e, s), append(e, c), G[_].m(c, null), append(e, h), append(e, p), append(e, m), append(e, v), append(v, k), W[b].m(k, null), S = !0, I || (D = [listen(u, "mousedown", t[9]), listen(p, "mousedown", t[8])], I = !0)
+            append(e, o), append(e, u), append(e, s), append(e, c), W[_].m(c, null), append(e, h), append(e, p), append(e, m), append(e, v), append(v, k), G[b].m(k, null), S = !0, I || (D = [listen(u, "mousedown", t[9]), listen(p, "mousedown", t[8])], I = !0)
         },
         p(Q, F) {
             F & 4188 && (O = Q[2], group_outros(), l = update_keyed_each(l, F, B, 1, Q, O, a, r, outro_and_destroy_block, create_each_block$1, null, get_each_context$1), check_outros());
             let te = _;
-            _ = A(Q), _ === te ? G[_].p(Q, F) : (group_outros(), transition_out(G[te], 1, 1, () => {
-                G[te] = null
-            }), check_outros(), d = G[_], d ? d.p(Q, F) : (d = G[_] = L[_](Q), d.c()), transition_in(d, 1), d.m(c, null)), (!S || F & 12 && g !== (g = "tree scrollable " + (Q[2][Q[3]] || "") + " svelte-1302pl0")) && attr(c, "class", g);
+            _ = A(Q), _ === te ? W[_].p(Q, F) : (group_outros(), transition_out(W[te], 1, 1, () => {
+                W[te] = null
+            }), check_outros(), d = W[_], d ? d.p(Q, F) : (d = W[_] = L[_](Q), d.c()), transition_in(d, 1), d.m(c, null)), (!S || F & 12 && g !== (g = "tree scrollable " + (Q[2][Q[3]] || "") + " svelte-1302pl0")) && attr(c, "class", g);
             let Y = b;
-            b = j(Q), b === Y ? W[b].p(Q, F) : (group_outros(), transition_out(W[Y], 1, 1, () => {
-                W[Y] = null
-            }), check_outros(), E = W[b], E ? E.p(Q, F) : (E = W[b] = U[b](Q), E.c()), transition_in(E, 1), E.m(k, null)), (!S || F & 4 && w !== (w = Q[2].length === 1 ? "--jobs-height: 0" : "")) && attr(e, "style", w)
+            b = j(Q), b === Y ? G[b].p(Q, F) : (group_outros(), transition_out(G[Y], 1, 1, () => {
+                G[Y] = null
+            }), check_outros(), E = G[b], E ? E.p(Q, F) : (E = G[b] = U[b](Q), E.c()), transition_in(E, 1), E.m(k, null)), (!S || F & 4 && w !== (w = Q[2].length === 1 ? "--jobs-height: 0" : "")) && attr(e, "style", w)
         },
         i(Q) {
             if (!S) {
                 for (let F = 0; F < O.length; F += 1) transition_in(l[F]);
                 transition_in(d), transition_in(E), S = !0
             }
         },
         o(Q) {
             for (let F = 0; F < l.length; F += 1) transition_out(l[F]);
             transition_out(d), transition_out(E), S = !1
         },
         d(Q) {
             Q && detach(e);
             for (let F = 0; F < l.length; F += 1) l[F].d();
-            G[_].d(), W[b].d(), I = !1, run_all(D)
+            W[_].d(), G[b].d(), I = !1, run_all(D)
         }
     }
 }
 
 function create_if_block_1$3(t) {
     let e, n, r;
     return n = new InlineNotification$1({
@@ -31571,21 +31565,21 @@
         E = function(A) {
             p = A.clientY, v = A.target.previousElementSibling.clientHeight
         },
         w = function(A) {
             if (h !== null) {
                 A.stopPropagation(), A.preventDefault();
                 const U = A.clientX - h,
-                    W = m + U < 0 ? 0 : m + U;
-                document.getElementById("procrun-wrap").style.setProperty("--tree-width", `${W}px`)
+                    G = m + U < 0 ? 0 : m + U;
+                document.getElementById("procrun-wrap").style.setProperty("--tree-width", `${G}px`)
             } else if (p !== null) {
                 A.stopPropagation(), A.preventDefault();
                 const U = A.clientY - p,
-                    W = v + U < 0 ? 0 : v + U;
-                document.getElementById("procrun-wrap").style.setProperty("--jobs-height", `${W}px`)
+                    G = v + U < 0 ? 0 : v + U;
+                document.getElementById("procrun-wrap").style.setProperty("--jobs-height", `${G}px`)
             }
         },
         S = function() {
             h = null, p = null
         },
         I = async function(A) {
             let U = [];
@@ -31598,16 +31592,16 @@
                     },
                     body: JSON.stringify({
                         name: r,
                         proc: a,
                         job: A
                     })
                 })
-            } catch (W) {
-                n(5, c.kind = "error", c), n(5, c.subtitle = `Failed to get job details: ${W}`, c)
+            } catch (G) {
+                n(5, c.kind = "error", c), n(5, c.subtitle = `Failed to get job details: ${G}`, c)
             } finally {
                 n(6, _ = !1)
             }
             return c.kind !== "error" && n(5, c.kind = void 0, c), U
         };
     o.length === 1 && (u = 0, I(0).then(A => {
         n(4, s = A)
@@ -31632,17 +31626,17 @@
                 }
             },
             U = A(s, k);
         if (!U) {
             n(5, c.kind = "error", c), n(5, c.subtitle = "Failed to find the file path", c), g = !1;
             return
         }
-        let W;
+        let G;
         try {
-            W = await fetchAPI("/api/job/get_file", {
+            G = await fetchAPI("/api/job/get_file", {
                 method: "POST",
                 headers: {
                     "Content-Type": "application/json"
                 },
                 body: JSON.stringify({
                     proc: a,
                     job: u,
@@ -31651,30 +31645,30 @@
             })
         } catch (j) {
             n(5, c.kind = "error", c), n(5, c.subtitle = `Failed to get file details: ${j}`, c)
         } finally {
             g = !1
         }
         c.kind !== "error" && (n(5, c.kind = void 0, c), n(7, d = {
-            ...W,
+            ...G,
             path: U.full,
             text: U.text
         }))
     };
     onMount(async () => {
         o.length > 0 && u === void 0 && (n(3, u = 0), n(4, s = await I(0)))
     });
     const B = async (A, U) => {
         n(3, u = A), n(4, s = await I(A))
     }, L = async () => {
         n(4, s = await I(u))
-    }, G = () => n(5, c.kind = void 0, c);
+    }, W = () => n(5, c.kind = void 0, c);
     return t.$$set = A => {
         "name" in A && n(15, r = A.name), "status" in A && n(0, l = A.status), "proc" in A && n(1, a = A.proc), "jobs" in A && n(2, o = A.jobs)
-    }, [l, a, o, u, s, c, _, d, b, E, w, S, I, D, O, r, B, L, G]
+    }, [l, a, o, u, s, c, _, d, b, E, w, S, I, D, O, r, B, L, W]
 }
 class ProcRun extends SvelteComponent {
     constructor(e) {
         super(), init(this, e, instance$4, create_fragment$4, safe_not_equal, {
             name: 15,
             status: 0,
             proc: 1,
@@ -31761,14 +31755,44 @@
 }
 
 function get_each_context_3(t, e, n) {
     const r = t.slice();
     return r[28] = e[n], r
 }
 
+function create_else_block_3(t) {
+    let e;
+    return {
+        c() {
+            e = element("link"), attr(e, "rel", "icon"), attr(e, "type", "image/png"), attr(e, "href", "./assets/favicon.png")
+        },
+        m(n, r) {
+            insert(n, e, r)
+        },
+        d(n) {
+            n && detach(e)
+        }
+    }
+}
+
+function create_if_block_17(t) {
+    let e;
+    return {
+        c() {
+            e = element("link"), attr(e, "rel", "icon"), attr(e, "type", "image/png"), attr(e, "href", "./assets/favicon-running.png")
+        },
+        m(n, r) {
+            insert(n, e, r)
+        },
+        d(n) {
+            n && detach(e)
+        }
+    }
+}
+
 function create_else_block$2(t) {
     let e, n, r, l, a, o, u = t[0][SECTION_PROCESSES] && Object.keys(t[0][SECTION_PROCESSES]).length > 0,
         s, c, _, d, g, h, p = t[2] > 0 && create_if_block_15(t),
         m = t[0][SECTION_LOG] !== null && create_if_block_14(t),
         v = t[0][SECTION_DIAGRAM] && create_if_block_13(t),
         k = t[0][SECTION_REPORTS] && create_if_block_12(t),
         b = u && create_if_block_11(t),
@@ -32759,23 +32783,23 @@
     }
 }
 
 function create_default_slot_1$1(t) {
     let e, n, r, l, a = t[0][SECTION_REPORTS] + "",
         o, u, s, c, _, d, g, h, p, m, v, k = t[0][SECTION_REPORTS] + "",
         b, E, w, S, I, D, O, B = t[0][SECTION_REPORTS] + "",
-        L, G, A, U, W, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P;
+        L, W, A, U, G, j, Q, F, te, Y, oe, ae, C, Z, K, ce, z, V, $, re, ue, P;
     return {
         c() {
-            e = element("div"), n = element("p"), r = text("Reports are generated at "), l = element("code"), o = text(a), u = text("/REPORTS"), s = space(), c = element("p"), c.textContent = " ", _ = space(), d = element("p"), d.textContent = "You can either:", g = space(), h = element("ul"), p = element("li"), m = text("Check them out by directly visiting "), v = element("code"), b = text(k), E = text("/REPORTS/index.html"), w = space(), S = element("li"), I = text("Run "), D = element("code"), O = text("pipen report serve -r "), L = text(B), G = text(", and go to "), A = element("code"), A.textContent = "REPORTS", U = text(" directory."), W = space(), j = element("li"), Q = text("Visit "), F = element("a"), te = text("the reports"), oe = text(" served by this plugin"), ae = space(), C = element("li"), Z = text(`Or check the
+            e = element("div"), n = element("p"), r = text("Reports are generated at "), l = element("code"), o = text(a), u = text("/REPORTS"), s = space(), c = element("p"), c.textContent = " ", _ = space(), d = element("p"), d.textContent = "You can either:", g = space(), h = element("ul"), p = element("li"), m = text("Check them out by directly visiting "), v = element("code"), b = text(k), E = text("/REPORTS/index.html"), w = space(), S = element("li"), I = text("Run "), D = element("code"), O = text("pipen report serve -r "), L = text(B), W = text(", and go to "), A = element("code"), A.textContent = "REPORTS", U = text(" directory."), G = space(), j = element("li"), Q = text("Visit "), F = element("a"), te = text("the reports"), oe = text(" served by this plugin"), ae = space(), C = element("li"), Z = text(`Or check the
                                     `), K = element("a"), K.textContent = "building log", ce = text(`
                                     if necessary.`), z = space(), V = element("p"), V.textContent = " ", $ = space(), re = element("p"), re.textContent = "Note that if the run fails, the reports may be incomplete.", attr(l, "class", "svelte-egdjr7"), attr(n, "class", "svelte-egdjr7"), attr(c, "class", "svelte-egdjr7"), attr(d, "class", "svelte-egdjr7"), attr(v, "class", "svelte-egdjr7"), attr(p, "class", "svelte-egdjr7"), attr(D, "class", "svelte-egdjr7"), attr(A, "class", "svelte-egdjr7"), attr(S, "class", "svelte-egdjr7"), attr(F, "target", "_blank"), attr(F, "href", Y = "/reports/" + t[0][SECTION_REPORTS].replaceAll("/", "|") + "/REPORTS/index.html"), attr(F, "class", "svelte-egdjr7"), attr(j, "class", "svelte-egdjr7"), attr(K, "href", "javascript:void(0)"), attr(K, "class", "svelte-egdjr7"), attr(C, "class", "svelte-egdjr7"), attr(h, "class", "svelte-egdjr7"), attr(V, "class", "svelte-egdjr7"), attr(re, "class", "svelte-egdjr7"), attr(e, "class", "reports-wrapper svelte-egdjr7")
         },
         m(q, ee) {
-            insert(q, e, ee), append(e, n), append(n, r), append(n, l), append(l, o), append(l, u), append(e, s), append(e, c), append(e, _), append(e, d), append(e, g), append(e, h), append(h, p), append(p, m), append(p, v), append(v, b), append(v, E), append(h, w), append(h, S), append(S, I), append(S, D), append(D, O), append(D, L), append(S, G), append(S, A), append(S, U), append(h, W), append(h, j), append(j, Q), append(j, F), append(F, te), append(j, oe), append(h, ae), append(h, C), append(C, Z), append(C, K), append(C, ce), append(e, z), append(e, V), append(e, $), append(e, re), ue || (P = listen(K, "click", prevent_default(t[11])), ue = !0)
+            insert(q, e, ee), append(e, n), append(n, r), append(n, l), append(l, o), append(l, u), append(e, s), append(e, c), append(e, _), append(e, d), append(e, g), append(e, h), append(h, p), append(p, m), append(p, v), append(v, b), append(v, E), append(h, w), append(h, S), append(S, I), append(S, D), append(D, O), append(D, L), append(S, W), append(S, A), append(S, U), append(h, G), append(h, j), append(j, Q), append(j, F), append(F, te), append(j, oe), append(h, ae), append(h, C), append(C, Z), append(C, K), append(C, ce), append(e, z), append(e, V), append(e, $), append(e, re), ue || (P = listen(K, "click", prevent_default(t[11])), ue = !0)
         },
         p(q, ee) {
             ee[0] & 1 && a !== (a = q[0][SECTION_REPORTS] + "") && set_data(o, a), ee[0] & 1 && k !== (k = q[0][SECTION_REPORTS] + "") && set_data(b, k), ee[0] & 1 && B !== (B = q[0][SECTION_REPORTS] + "") && set_data(L, B), ee[0] & 1 && Y !== (Y = "/reports/" + q[0][SECTION_REPORTS].replaceAll("/", "|") + "/REPORTS/index.html") && attr(F, "href", Y)
         },
         d(q) {
             q && detach(e), ue = !1, P()
         }
@@ -32853,46 +32877,53 @@
         d(r) {
             r && detach(e)
         }
     }
 }
 
 function create_fragment$2(t) {
-    let e, n, r, l, a, o;
-    const u = [create_if_block_1$2, create_if_block_2$2, create_else_block$2],
-        s = [];
+    let e, n, r, l, a, o, u, s;
 
-    function c(d, g) {
-        return g[0] & 1 && (e = null), !d[0] && d[4] ? 0 : (e == null && (e = Object.keys(d[0] || {}).length === 0), e ? 1 : 2)
+    function c(v, k) {
+        return v[2] > 0 && !v[1] ? create_if_block_17 : create_else_block_3
     }
-    n = c(t, [-1, -1]), r = s[n] = u[n](t);
-    let _ = t[6].kind && create_if_block$2(t);
+    let _ = c(t),
+        d = _(t);
+    const g = [create_if_block_1$2, create_if_block_2$2, create_else_block$2],
+        h = [];
+
+    function p(v, k) {
+        return k[0] & 1 && (r = null), !v[0] && v[4] ? 0 : (r == null && (r = Object.keys(v[0] || {}).length === 0), r ? 1 : 2)
+    }
+    l = p(t, [-1, -1]), a = h[l] = g[l](t);
+    let m = t[6].kind && create_if_block$2(t);
     return {
         c() {
-            r.c(), l = space(), _ && _.c(), a = empty()
+            d.c(), e = empty(), n = space(), a.c(), o = space(), m && m.c(), u = empty()
         },
-        m(d, g) {
-            s[n].m(d, g), insert(d, l, g), _ && _.m(d, g), insert(d, a, g), o = !0
+        m(v, k) {
+            d.m(document.head, null), append(document.head, e), insert(v, n, k), h[l].m(v, k), insert(v, o, k), m && m.m(v, k), insert(v, u, k), s = !0
         },
-        p(d, g) {
-            let h = n;
-            n = c(d, g), n === h ? s[n].p(d, g) : (group_outros(), transition_out(s[h], 1, 1, () => {
-                s[h] = null
-            }), check_outros(), r = s[n], r ? r.p(d, g) : (r = s[n] = u[n](d), r.c()), transition_in(r, 1), r.m(l.parentNode, l)), d[6].kind ? _ ? (_.p(d, g), g[0] & 64 && transition_in(_, 1)) : (_ = create_if_block$2(d), _.c(), transition_in(_, 1), _.m(a.parentNode, a)) : _ && (group_outros(), transition_out(_, 1, 1, () => {
-                _ = null
+        p(v, k) {
+            _ !== (_ = c(v)) && (d.d(1), d = _(v), d && (d.c(), d.m(e.parentNode, e)));
+            let b = l;
+            l = p(v, k), l === b ? h[l].p(v, k) : (group_outros(), transition_out(h[b], 1, 1, () => {
+                h[b] = null
+            }), check_outros(), a = h[l], a ? a.p(v, k) : (a = h[l] = g[l](v), a.c()), transition_in(a, 1), a.m(o.parentNode, o)), v[6].kind ? m ? (m.p(v, k), k[0] & 64 && transition_in(m, 1)) : (m = create_if_block$2(v), m.c(), transition_in(m, 1), m.m(u.parentNode, u)) : m && (group_outros(), transition_out(m, 1, 1, () => {
+                m = null
             }), check_outros())
         },
-        i(d) {
-            o || (transition_in(r), transition_in(_), o = !0)
+        i(v) {
+            s || (transition_in(a), transition_in(m), s = !0)
         },
-        o(d) {
-            transition_out(r), transition_out(_), o = !1
+        o(v) {
+            transition_out(a), transition_out(m), s = !1
         },
-        d(d) {
-            s[n].d(d), d && detach(l), _ && _.d(d), d && detach(a)
+        d(v) {
+            d.d(v), detach(e), v && detach(n), h[l].d(v), v && detach(o), m && m.d(v), v && detach(u)
         }
     }
 }
 
 function instance$2(t, e, n) {
     let {
         data: r
@@ -32913,36 +32944,36 @@
         r = void 0;
         const L = new WebSocket(`ws://${location.host}/ws`);
         L.onopen = function() {
             L.send(JSON.stringify({
                 type: "connect",
                 client: "web"
             }))
-        }, L.onmessage = async function(G) {
-            n(0, r = JSON.parse(G.data)), n(4, s = !1), n(1, o = r.FINISHED), n(12, l = getStatusPercentage(r)), d && (d = !1, n(5, c = "Log"))
+        }, L.onmessage = async function(W) {
+            n(0, r = JSON.parse(W.data)), n(4, s = !1), n(1, o = r.FINISHED), n(12, l = getStatusPercentage(r)), d && (d = !1, n(5, c = "Log"))
         }
     }
-    const p = (L, G = null) => {
-            for (const [A, U] of Object.entries(r[SECTION_PROCESSES]))(U.status === G || G === null) && (U.status = L), U.jobs = U.jobs.map(W => W === G || G === null ? L : W);
+    const p = (L, W = null) => {
+            for (const [A, U] of Object.entries(r[SECTION_PROCESSES]))(U.status === W || W === null) && (U.status = L), U.jobs = U.jobs.map(G => G === W || W === null ? L : G);
             for (const [A, U] of Object.entries(r[SECTION_PROCGROUPS]))
-                for (const [W, j] of Object.entries(U))(j.status === G || G === null) && (j.status = L), j.jobs = j.jobs.map(Q => Q === G || G === null ? L : Q);
+                for (const [G, j] of Object.entries(U))(j.status === W || W === null) && (j.status = L), j.jobs = j.jobs.map(Q => Q === W || W === null ? L : Q);
             n(0, r)
         },
         m = async () => {
             if (!confirm("Are you sure to re-run this pipeline (using the same configurations)?")) return;
             n(7, g = !0);
             let L;
             try {
-                L = await fetchAPI("/api/pipeline/rerun", {
-                    method: "POST"
-                })
-            } catch (G) {
+                if (L = await fetchAPI("/api/pipeline/rerun", {
+                        method: "POST"
+                    }), L.error) throw new Error(L.error)
+            } catch (W) {
                 n(6, _ = {
                     kind: "error",
-                    subtitle: `Run re-submission failed: ${G}.`,
+                    subtitle: `Run re-submission failed: ${W}.`,
                     timeout: 5e3
                 })
             } finally {
                 n(7, g = !1)
             }
             _.kind !== "error" && (L.ok ? (n(6, _ = {
                 kind: "success",
@@ -32957,18 +32988,18 @@
             if (!confirm("Are you sure to stop the run?")) return;
             n(7, g = !0);
             let L;
             try {
                 L = await fetchAPI("/api/pipeline/stop", {
                     method: "POST"
                 })
-            } catch (G) {
+            } catch (W) {
                 n(6, _ = {
                     kind: "error",
-                    subtitle: `Run stop failed: ${G}.`,
+                    subtitle: `Run stop failed: ${W}.`,
                     timeout: 5e3
                 })
             } finally {
                 n(7, g = !1)
             }
             _.kind !== "error" && (L.ok ? (n(6, _ = {
                 kind: "success",
@@ -32980,16 +33011,16 @@
                 timeout: 5e3
             }))
         }, k = async () => {
             n(8, h = "Loading ...");
             let L;
             try {
                 L = await fetchAPI(`/api/report_building_log?name=${u}`)
-            } catch (G) {
-                n(8, h = `Error: ${G}`)
+            } catch (W) {
+                n(8, h = `Error: ${W}`)
             }
             L && n(8, h = L.ok ? L.content || "(empty)" : `Error: ${L.msg}`)
         };
 
     function b(L) {
         c = L, n(5, c)
     }
@@ -32997,20 +33028,20 @@
     function E(L) {
         c = L, n(5, c)
     }
 
     function w(L) {
         c = L, n(5, c)
     }
-    const S = (L, G) => r[SECTION_PROCESSES][L].order - r[SECTION_PROCESSES][G].order === 0 ? L.localeCompare(G) : r[SECTION_PROCESSES][L].order - r[SECTION_PROCESSES][G].order;
+    const S = (L, W) => r[SECTION_PROCESSES][L].order - r[SECTION_PROCESSES][W].order === 0 ? L.localeCompare(W) : r[SECTION_PROCESSES][L].order - r[SECTION_PROCESSES][W].order;
 
     function I(L) {
         c = L, n(5, c)
     }
-    const D = (L, G, A) => r[SECTION_PROCGROUPS][L][G].order - r[SECTION_PROCGROUPS][L][A].order === 0 ? G.localeCompare(A) : r[SECTION_PROCGROUPS][L][G].order - r[SECTION_PROCGROUPS][L][A].order;
+    const D = (L, W, A) => r[SECTION_PROCGROUPS][L][W].order - r[SECTION_PROCGROUPS][L][A].order === 0 ? W.localeCompare(A) : r[SECTION_PROCGROUPS][L][W].order - r[SECTION_PROCGROUPS][L][A].order;
 
     function O(L) {
         c = L, n(5, c)
     }
     const B = () => n(6, _.kind = void 0, _);
     return t.$$set = L => {
         "data" in L && n(0, r = L.data), "statusPercent" in L && n(12, l = L.statusPercent), "runStarted" in L && n(2, a = L.runStarted), "finished" in L && n(1, o = L.finished), "name" in L && n(3, u = L.name)
@@ -33035,16 +33066,15 @@
     function c(h) {
         t[13](h)
     }
     let _ = {
         pipelineName: t[8],
         pipelineDesc: t[9],
         isRunning: t[2] && !t[3],
-        backToHistory: !0,
-        histories: t[1]
+        backToHistory: !0
     };
     t[0] !== void 0 && (_.configfile = t[0]), n = new Header({
         props: _
     }), binding_callbacks.push(() => bind(n, "configfile", c));
 
     function d(h) {
         t[21](h)
@@ -33066,15 +33096,15 @@
             e = element("div"), create_component(n.$$.fragment), l = space(), a = element("div"), create_component(o.$$.fragment), attr(a, "class", "pipen-tabs svelte-1w9ezow"), attr(e, "class", "body svelte-1w9ezow")
         },
         m(h, p) {
             insert(h, e, p), mount_component(n, e, null), append(e, l), append(e, a), mount_component(o, a, null), s = !0
         },
         p(h, p) {
             const m = {};
-            p & 256 && (m.pipelineName = h[8]), p & 512 && (m.pipelineDesc = h[9]), p & 12 && (m.isRunning = h[2] && !h[3]), p & 2 && (m.histories = h[1]), !r && p & 1 && (r = !0, m.configfile = h[0], add_flush_callback(() => r = !1)), n.$set(m);
+            p & 256 && (m.pipelineName = h[8]), p & 512 && (m.pipelineDesc = h[9]), p & 12 && (m.isRunning = h[2] && !h[3]), !r && p & 1 && (r = !0, m.configfile = h[0], add_flush_callback(() => r = !1)), n.$set(m);
             const v = {};
             p & 8390463 && (v.$$scope = {
                 dirty: p,
                 ctx: h
             }), !u && p & 2048 && (u = !0, v.selected = h[11], add_flush_callback(() => u = !1)), o.$set(v)
         },
         i(h) {
@@ -33602,16 +33632,16 @@
                 headers: {
                     "Content-Type": "application/json"
                 },
                 body: JSON.stringify({
                     configfile: r
                 })
             })
-        } catch (G) {
-            n(7, _ = `<strong>Failed to fetch or parse data:</strong> <br /><br /><pre>${G}</pre>`)
+        } catch (W) {
+            n(7, _ = `<strong>Failed to fetch or parse data:</strong> <br /><br /><pre>${W}</pre>`)
         } finally {
             n(6, c = !1)
         }
         _ || (IS_DEV && (window.data = L), n(2, a = L.runStarted + 0), n(4, u = L.config), n(5, s = L.run), n(8, d = u[SECTION_PIPELINE_OPTS].name.value), n(9, g = u[SECTION_PIPELINE_OPTS].desc.value), n(10, h = getStatusPercentage(s))), storedGlobalChanged.set(!1)
     });
     const v = () => {
         n(0, r = void 0)
```

### Comparing `pipen_board-0.7.3/pipen_board/frontend/build/assets/schema.json` & `pipen_board-0.7.4/pipen_board/frontend/build/assets/schema.json`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/plugin.py` & `pipen_board-0.7.4/pipen_board/plugin.py`

 * *Files identical despite different names*

### Comparing `pipen_board-0.7.3/pipen_board/quart_app.py` & `pipen_board-0.7.4/pipen_board/quart_app.py`

 * *Files 8% similar despite different names*

```diff
@@ -118,14 +118,21 @@
 
     @app.route("/api/pipeline/rerun", methods=["POST"])
     async def rerun():
         logger.info(
             f"[bold][yellow]API[/yellow][/bold] Re-Running pipeline: %s",
             data_manager._command,
         )
+
+        if not data_manager._command:
+            return {
+                "ok": False,
+                "error": "Pipeline never ran. Please reload the page.",
+            }
+
         # Run command at background
         app.add_background_task(
             data_manager.run_pipeline,
             data_manager._command,
             args.port,
             clients,
         )
```

### Comparing `pipen_board-0.7.3/pyproject.toml` & `pipen_board-0.7.4/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pipen-board"
-version = "0.7.3"
+version = "0.7.4"
 description = "Visualization configuration and running of pipen pipelines on the web"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 readme = "README.md"
 exclude = ["pipen_board/frontend/[!build]*", "pipen_board/frontend/index.html"]
 
 [tool.poetry.build]
```

### Comparing `pipen_board-0.7.3/setup.py` & `pipen_board-0.7.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 entry_points = \
 {'pipen': ['board = pipen_board:pipen_board_plugin'],
  'pipen_cli': ['cli-board = pipen_board:PipenCliBoardPlugin']}
 
 setup_kwargs = {
     'name': 'pipen-board',
-    'version': '0.7.3',
+    'version': '0.7.4',
     'description': 'Visualization configuration and running of pipen pipelines on the web',
     'long_description': '# pipen-board\n\nVisualize configuration and running of [pipen][1] pipelines on the web.\n\n## Installation\n\n```bash\npip install pipen-board\n```\n\n## Usage\n\n```bash\n$ pipen board --help\nUsage: pipen board [options] <pipeline> -- [pipeline options]\n\nConfigure and run pipen pipelines from the web\n\nRequired Arguments:\n  pipeline              The pipeline and the CLI arguments to run the pipeline.\n                        For the pipeline either\n                        `/path/to/pipeline.py:<pipeline>` or\n                        `<module.submodule>:<pipeline>` `<pipeline>` must be an\n                        instance of `Pipen` and running the pipeline should be\n                        called under `__name__ == \'__main__\'.\n\nOptions:\n  -h, --help            show help message and exit\n  -p PORT, --port PORT  Port to serve the UI wizard [default: 18521]\n  -a FILE, --additional FILE\n                        Additional arguments for the pipeline, in YAML, INI,\n                        JSON or TOML format. Can have sections\n                        `ADDITIONAL_OPTIONS` and `RUNNING_OPTIONS`. It can also\n                        have other sections and items to override the\n                        configurations generated from the pipeline. If the\n                        pipeline is provided as a python script, such as\n                        `/path/to/pipeline.py:<pipeline>`, and `<pipeline>`\n                        runs under `__name__ == \'__main__\'`, the additional\n                        file can also be specified as `auto` to generate a\n                        `RUNNING OPTIONS/Local` section to run the pipeline\n                        locally.\n  --loglevel {auto,debug,info,warning,error,critical}\n                        The logging level. If `auto`, it will be set to `debug`\n                        if `--dev` is set, otherwise `info`. [default: auto]\n  --dev                 Run the pipeline in development/debug mode. This will\n                        reload the server when changes are made to this package\n                        and reload the pipeline when page reloads for new\n                        configurations. Page cache is also disabled in this\n                        mode.\n  -w WORKDIR, --workdir WORKDIR\n                        The working directory of the pipeline. [default:\n                        .pipen]\n```\n\n## Describing arguments in docstring\n\n### Docstring schema\n\n```python\nclass ProcessOrProcessGroup:\n    """Short summary\n\n    Long description\n    Long description\n\n    Args:\n        arg1 (<metadata>): description\n            - subarg1 (<metadata>): description\n            - subarg2 (<metadata>): description\n        arg2 (<metadata>): description\n\n    <Other Sections>:\n        <content>\n    """\n```\n\nThe metadata can have multiple attributes, separated by semicolon (`;`). For example:\n\n```\narg1 (action=ns;required): description\n```\n\n### Marks\n\nYou can mark a process using `pipen.utils.mark(<mark>=<value>)` as a decorator to decorate a process. For example:\n\n```python\nfrom pipen import Proc\nfrom pipen.utils import mark\n\n@mark(board_config_no_input=True)\nclass MyProc(Proc):\n    pass\n```\n\nAvailable marks:\n\n- `board_config_no_input`: Whether to show the input section for the process in configuation page. Only affects the start processes. Default to `False`.\n- `board_config_hidden`: Whether to hide the process options in the configuration page. Note that the process is still visible in the process list. Default to `False`.\n\n### Metadata for arguments\n\n\n| Name     | Description | Allowed values |\n| -------- | ----------- | -------------- |\n| `action` | Like the `action` argument in [`argx`][2]*. | `store_true`, `store_false`, `ns`, `namespace`, `append`, `extend`, `clear_append`, `clear_extend` (other values are allowed but ignore, they may be effective for CLI use) |\n| `btype`  | Board type (option type specified directly). If specified, `action` will be ignored | `ns`, `choice`, `mchoice`, `array`, `list`, `json`, `int`, `float`, `bool`, `str`, `text`, `auto`* |\n| `type` | Fallback for `action` and `btype` | Same as `btype` |\n| `flag` | Fallback for `action=store_true` | No values needed |\n| `text`/`mline`/`mlines` | Shortcut for `btype=text` | No values needed |\n| `ns`/`namespace` | Shortcut for `btype=ns` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `array`/`list` | Shortcut for `btype=array`/`btype=list` | No values needed |\n| `choices`/`choice` | Shortcut for `btype=choice` | No values needed |\n| `mchoices`/`mchoice` | Shortcut for `btype=mchoice` | No values needed |\n| `order` | The order of the argument in the UI. | Any integer |\n| `readonly` | Whether the argument is readonly. | No values needed (True if specified, otherwise False) |\n| `required` | Whether the argument is required. | No values needed (True if specified, otherwise False) |\n| `placeholder` | The placeholder in the UI for the argument. | Any string |\n| `bitype` | The type of the elements in an array or list. | `int`, `float`, `bool`, `str`, `json`, `auto`* |\n| `itype` | Fallback for `bitype` | Same as `bitype` |\n\n- `argx*`: An argument parser for Python, compatible with `argparse`.\n- `auto*`: Automatically infer the type from a string value.\n  - Any of `True`, `TRUE`, `true`, `False`, `FALSE`, `false` will be inferred as a `bool` value.\n  - Any of `None`, `NONE`, `none`, `null`, `NULL` will be inferred as `None`.\n  - Any integers will be inferred as `int`.\n  - Any floats will be inferred as `float`.\n  - Try to parse the value as JSON. If succeed, the value will be inferred as `json`.\n  - Otherwise, the value will be inferred as `str`.\n\n### Types of options in the UI\n\nThe type of an option in the UI is determined by the `btype`, `action` or `type` metadata. If neither is specified, a `PlainText` will be used.\n\n- `BoolOption`: Shown as a switch\n- `TextOption`: Shown as a textarea (allow multiple lines)\n- `ChoiceOption`: Shown as a dropdown list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `MChoiceOption`: Shown as a multiple choice list (`subarg1` and `subarg2` in the example above are used as the choices)\n- `JsonOption`: Shown as a textarea, but the value will be validated and parsed as JSON\n- `ArrayOption`: Shown as a tag input. Items can be added or removed.\n- `AutoOption`: Shown as a 1-row textarea, and the value will be parsed automatically\n- `PlainText`: Shown as a plain text. No validation or parsing will be performed.\n- `MoreLikeOption`: Show as a box with buttons to add or remove sub-options. It\'s usally used together with `ns` type. If there is a sub-option under the option in the docstring wrapped by `<...>`, it indicates that we may have more sub-options.\n\n\n[1]: https://github.com/pwwang/pipen\n[2]: https://github.com/pwwang/argx\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pipen_board-0.7.3/PKG-INFO` & `pipen_board-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipen-board
-Version: 0.7.3
+Version: 0.7.4
 Summary: Visualization configuration and running of pipen pipelines on the web
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

