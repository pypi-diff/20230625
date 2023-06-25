# Comparing `tmp/OEISsequences-0.1.8.tar.gz` & `tmp/OEISsequences-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OEISsequences-0.1.8.tar", last modified: Sat Dec 31 23:51:55 2022, max compression
+gzip compressed data, was "OEISsequences-0.1.9.tar", last modified: Sun Feb 12 18:09:45 2023, max compression
```

## Comparing `OEISsequences-0.1.8.tar` & `OEISsequences-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-31 23:51:55.258292 OEISsequences-0.1.8/
--rw-rw-rw-   0        0        0    11515 2022-12-04 15:54:39.000000 OEISsequences-0.1.8/LICENSE
-drwxrwxrwx   0        0        0        0 2022-12-31 23:51:55.236088 OEISsequences-0.1.8/OEISsequences.egg-info/
--rw-rw-rw-   0        0        0     4592 2022-12-31 23:51:54.000000 OEISsequences-0.1.8/OEISsequences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2022-12-31 23:51:54.000000 OEISsequences-0.1.8/OEISsequences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-31 23:51:54.000000 OEISsequences-0.1.8/OEISsequences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2022-12-31 23:51:54.000000 OEISsequences-0.1.8/OEISsequences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-12-31 23:51:54.000000 OEISsequences-0.1.8/OEISsequences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4592 2022-12-31 23:51:55.258292 OEISsequences-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3993 2022-12-04 15:54:39.000000 OEISsequences-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-12-31 23:51:55.258292 OEISsequences-0.1.8/oeis_sequences/
--rw-rw-rw-   0        0        0   810467 2022-12-31 23:46:58.000000 OEISsequences-0.1.8/oeis_sequences/OEISsequences.py
--rw-rw-rw-   0        0        0       46 2022-12-04 15:54:39.000000 OEISsequences-0.1.8/oeis_sequences/__init__.py
--rw-rw-rw-   0        0        0       86 2022-12-31 23:51:55.320884 OEISsequences-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      970 2022-12-31 23:50:38.000000 OEISsequences-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-12 18:09:45.273692 OEISsequences-0.1.9/
+-rw-rw-rw-   0        0        0    11521 2023-02-12 17:42:00.000000 OEISsequences-0.1.9/LICENSE
+drwxrwxrwx   0        0        0        0 2023-02-12 18:09:45.273692 OEISsequences-0.1.9/OEISsequences.egg-info/
+-rw-rw-rw-   0        0        0     4592 2023-02-12 18:09:45.000000 OEISsequences-0.1.9/OEISsequences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-02-12 18:09:45.000000 OEISsequences-0.1.9/OEISsequences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-12 18:09:45.000000 OEISsequences-0.1.9/OEISsequences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-02-12 18:09:45.000000 OEISsequences-0.1.9/OEISsequences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-02-12 18:09:45.000000 OEISsequences-0.1.9/OEISsequences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4592 2023-02-12 18:09:45.273692 OEISsequences-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3993 2022-12-04 15:54:39.000000 OEISsequences-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-12 18:09:45.273692 OEISsequences-0.1.9/oeis_sequences/
+-rw-rw-rw-   0        0        0   846877 2023-02-12 18:05:26.000000 OEISsequences-0.1.9/oeis_sequences/OEISsequences.py
+-rw-rw-rw-   0        0        0       46 2022-12-04 15:54:39.000000 OEISsequences-0.1.9/oeis_sequences/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-02-12 18:09:45.273692 OEISsequences-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      970 2023-02-12 17:41:06.000000 OEISsequences-0.1.9/setup.py
```

### Comparing `OEISsequences-0.1.8/LICENSE` & `OEISsequences-0.1.9/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2021, 2022 Chai Wah Wu
+   Copyright 2021, 2022, 2023 Chai Wah Wu
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `OEISsequences-0.1.8/OEISsequences.egg-info/PKG-INFO` & `OEISsequences-0.1.9/OEISsequences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OEISsequences
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python functions to generate OEIS sequences
 Home-page: https://github.com/postvakje/oeis-sequences
 Author: Chai Wah Wu
 Author-email: cwwuieee@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `OEISsequences-0.1.8/PKG-INFO` & `OEISsequences-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OEISsequences
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python functions to generate OEIS sequences
 Home-page: https://github.com/postvakje/oeis-sequences
 Author: Chai Wah Wu
 Author-email: cwwuieee@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `OEISsequences-0.1.8/README.md` & `OEISsequences-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `OEISsequences-0.1.8/oeis_sequences/OEISsequences.py` & `OEISsequences-0.1.9/oeis_sequences/OEISsequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     starmap,
     zip_longest,
     tee,
 )
 from fractions import Fraction
 from collections import Counter, deque
 from math import factorial, floor, comb, prod, isqrt
-from operator import mul, xor, add, or_, and_, ior, ixor
+from operator import mul, xor, add, or_, and_, ior, ixor, iand
 from operator import sub as operator_sub
 from re import finditer, split, sub
 from statistics import pvariance
 from sympy.core.numbers import igcdex
 from sympy import (
     factorint,
     divisors,
@@ -130,14 +130,15 @@
     ceiling,
     log,
     simplify,
     perfect_power,
     convex_hull,
     GF,
     binomial,
+    I,
 )
 from sympy.functions import hyper, partition, euler
 from sympy.ntheory import (
     mobius,
     jacobi_symbol,
     legendre_symbol,
     sqrt_mod,
@@ -1659,15 +1660,15 @@
         if d <= n:
             s += 1
             n -= d
     return s
 
 
 def A026741(n):
-    return n if n % 2 else n // 2
+    return n if n & 1 else n >> 1
 
 
 def A006567_gen():
     return filter(
         lambda p: str(p) != str(p)[::-1] and isprime(int(str(p)[::-1])),
         (prime(n) for n in count(1)),
     )
@@ -2834,15 +2835,18 @@
     m, x = 1, 0
     for n in count(0):
         x, m = x * n + m * (n * (n - 1) // 2), -m
         yield x
 
 
 def A003893_gen():  # generator of terms
-    a, b, = (
+    (
+        a,
+        b,
+    ) = (
         0,
         1,
     )
     yield a
     while True:
         a, b = b, (a + b) % 10
         yield a
@@ -6616,15 +6620,15 @@
     for n in count(max(startvalue, 2)):
         nd = sum(n * e // p for p, e in factorint(n).items())
         if is_square(nd**2 + n**2) and gcd(n, nd, isqrt(nd**2 + n**2)) == 1:
             yield n
 
 
 def A235800(n):
-    return 4 * (n // 2) + 3 if n % 2 else n // 2
+    return ((n & -2) << 1) + 3 if n & 1 else n >> 1
 
 
 def A241816(n):
     s = bin(n)[2:]
     for i in range(len(s) - 2, -1, -1):
         if s[i : i + 2] == "10":
             return int(s[:i] + "01" + s[i + 2 :], 2)
@@ -14847,15 +14851,19 @@
     for i in count(9, 2):
         g *= i
         if isprime(g - h):
             yield i
 
 
 def A257342(n):
-    m, y, t, = (
+    (
+        m,
+        y,
+        t,
+    ) = (
         2,
         Fraction(0, 1),
         10 ** (n + 1),
     )
     for i in count(2):
         for j in range(1, i):
             x = Fraction(j, i)
@@ -17187,15 +17195,18 @@
             q = int(s + "1" + s[::-1])
             if isprime(q):
                 return q
         l += 1
 
 
 def A153568(n):
-    a, b, = (
+    (
+        a,
+        b,
+    ) = (
         0,
         1,
     )
     for _ in range(n):
         a, b = b, a + b
     return (lambda m: 2 * sum(a // k for k in range(1, m + 1)) - m * m)(isqrt(a))
 
@@ -18218,15 +18229,18 @@
         for c in multiset_permutations("0" * (l - 10) + "1" * 10, l):
             n = 2 * int("1" + "".join(c), 2)
             if sum(int(d) for d in format(n * (n + 2), "b")) == 11:
                 yield n + 1
 
 
 def A261694_gen():  # generator of terms
-    a, b, = (
+    (
+        a,
+        b,
+    ) = (
         0,
         1,
     )
     while True:
         yield a
         a, b = b, (a + b) % 21
 
@@ -20303,15 +20317,15 @@
 
 
 def A000330(n):
     return n * (n + 1) * (2 * n + 1) // 6
 
 
 def A001405(n):
-    return comb(n, n // 2)
+    return comb(n, n >> 1)
 
 
 def A001405_gen():  # generator of terms
     yield 1
     a = 1
     for i in count(1):
         a = 2 * a * i // (i + 1) if i & 1 else 2 * a
@@ -20575,15 +20589,15 @@
     return filter(lambda n: divisor_sigma(n) > 2 * n, count(max(startvalue, 1)))
 
 
 @lru_cache(maxsize=None)
 def A001190(n):
     if n <= 1:
         return n
-    m = n // 2 + n % 2
+    m = sum(divmod(n, 2))
     return (
         sum(A001190(i + 1) * A001190(n - 1 - i) for i in range(m - 1))
         + (1 - n % 2) * A001190(m) * (A001190(m) + 1) // 2
     )
 
 
 def A008292_T(n, k):
@@ -21457,36 +21471,24 @@
     return int(n == 2)
 
 
 def A063524(n):
     return int(n == 1)
 
 
-def A014081(n):
-    return sum(len(d) - 1 for d in split("0+", bin(n)[2:]) if d != "")
-
-
-def A053645(n):
-    return 0 if n <= 1 else int(bin(n)[3:], 2)
-
-
 @lru_cache(maxsize=None)
 def A346422(n):
     return (
         1
         if n <= 1
         else A346422(int((s := bin(n)[2:])[1:], 2))
         * (1 + sum(len(d) - 1 for d in split("0+", s) if d != ""))
     )
 
 
-def A245195(n):
-    return 2 ** A014081(n)
-
-
 def A245565(n):
     return RLT(n, lambda m: next(islice(A000129_gen(), m + 1, None)))
 
 
 def A329722(n):
     return RLT(n, lambda m: 1 if m <= 1 else lucas(m - 2))
 
@@ -22692,19 +22694,19 @@
             if m - p in pset:
                 c += 1
         if c == n:
             return m
 
 
 def A014494(n):
-    return (2 * n + 1) * (n + n % 2)
+    return (2 * n + 1) * (n + (n & 1))
 
 
 def A352115(n):
-    return (n + 1) * (2 * n * (n + 2) + 3 * (n % 2)) // 3
+    return (n << 1) * (n + 1) * (n + 2) // 3 + (n + 1) * (n & 1)
 
 
 def A351653(n):
     return int("".join(str(len(list(g))) for k, g in groupby(str(n))))
 
 
 def A318927(n):
@@ -23423,27 +23425,29 @@
 
 @lru_cache(maxsize=None)
 def A352289(n):
     return 1 if n == 1 else 2 * prime(A352289(n - 1))
 
 
 def A064989(n):
-    return prod(1 if p == 2 else prevprime(p) * e for p, e in factorint(n).items())
+    return prod(
+        prevprime(p) ** e for p, e in factorint(n >> (~n & n - 1).bit_length()).items()
+    )
 
 
 def A252463(n):
-    return A064989(n) if n % 2 else n // 2
+    return A064989(n) if n & 1 else n >> 1
 
 
 def A353412(n):
     return int(
         bin(
             prod(1 if p == 2 else prevprime(p) * e for p, e in factorint(n).items())
-            if n % 2
-            else n // 2
+            if n & 1
+            else n >> 1
         )[2:].rstrip("0"),
         2,
     )
 
 
 def A051064(n):
     c = 1
@@ -24647,39 +24651,39 @@
 
 
 def A114113(n):
     return 1 if n == 1 else (m := n // 2) * (n + 1) + (n + 1 - m) * (n - 2 * m)
 
 
 def A033999(n):
-    return -1 if n % 2 else 1
+    return -1 if n & 1 else 1
 
 
 def A354008(n):
     return (
         1
         if n == 1
         else (k := (m := n // 2) * (n + 1) + (n + 1 - m) * (n - 2 * m)) // gcd(k, n)
     )
 
 
 def A141310(n):
-    return 2 if n % 2 else n + 1
+    return 2 if n & 1 else n + 1
 
 
 def A130883(n):
     return n * (2 * n - 1) + 1
 
 
 def A128918(n):
-    return n * (n - 1) // 2 + 1 + (n - 1) * (n % 2)
+    return n * (n - 1) // 2 + 1 + (n - 1) * (n & 1)
 
 
 def A131179(n):
-    return n * (n + 1) // 2 + (1 - n) * (n % 2)
+    return n * (n + 1) // 2 + (1 - n) * (n & 1)
 
 
 def A008836(n):
     return -1 if sum(factorint(n).values()) % 2 else 1
 
 
 def A354334(n):
@@ -25325,15 +25329,15 @@
 
 
 def A095815(n):
     return n + max(int(d) for d in str(n))
 
 
 def A016116(n):
-    return 1 << n // 2
+    return 1 << (n >> 1)
 
 
 def A007590(n):
     return n**2 // 2
 
 
 def A000212(n):
@@ -25356,15 +25360,15 @@
         aqueue.append(a)
         if f:
             b = aqueue.popleft()
         f = not f
 
 
 def A098844(n):
-    return n * prod(n // 2**k for k in range(1, n.bit_length() - 1))
+    return n * prod(n >> k for k in range(1, n.bit_length() - 1))
 
 
 def A033485_gen():  # generator of terms
     aqueue, f, b, a = deque([2]), True, 1, 2
     yield from (1, 2)
     while True:
         a += b
@@ -25407,15 +25411,15 @@
         aqueue.append(a)
         if f:
             b = aqueue.popleft()
         f = not f
 
 
 def A008794(n):
-    return (n // 2) ** 2
+    return (n >> 1) ** 2
 
 
 @lru_cache(maxsize=None)
 def A320225(n):
     return 1 if n == 1 else sum(A320225(d) * (n // d - 1) for d in range(1, n))
 
 
@@ -27235,15 +27239,15 @@
         if n == 0
         else ((1 << n) - 1) * prod((1 << i) - 1 for i in range(2, 2 * n - 1, 2))
         << n * (n + 1) + 2
     )
 
 
 def A003053(n):
-    return (1 << (n // 2) ** 2) * prod(
+    return (1 << (n >> 1) ** 2) * prod(
         (1 << i) - 1 for i in range(2, 2 * ((n - 1) // 2) + 1, 2)
     )
 
 
 def A090770(n):
     return prod((1 << i) - 1 for i in range(2, 2 * n + 1, 2)) << (n + 1) ** 2
 
@@ -30823,18 +30827,14 @@
     return ((m := isqrt(k := n**3)) + int(k - m * (m + 1) >= 1)) ** 2
 
 
 def A077119(n):
     return ((m := isqrt(k := n**3)) + int(k - m * (m + 1) >= 1)) ** 2 - k
 
 
-def A004524(n):
-    return (n >> 2) + (n + 1 >> 2)
-
-
 def A011548(n):
     return (m := isqrt(k := 10 ** (n << 1) << 1)) + int(k - m * (m + 1) >= 1)
 
 
 def A001670(n):
     return (m := isqrt(n)) + int(n - m * (m + 1) >= 1) << 1
 
@@ -34888,7 +34888,1653 @@
 
 def A166590(n):
     return prod((p + 2) ** e for p, e in factorint(n).items())
 
 
 def A322361(n):
     return gcd(n, prod(nextprime(p) ** e for p, e in factorint(n).items()))
+
+
+def A123066(n):
+    return 1 + sum(1 if primenu(i) & 1 else -1 for i in range(1, n + 1))
+
+
+def A162511(n):
+    return -1 if reduce(lambda a, b: ~(a ^ b), factorint(n).values(), 0) & 1 else 1
+
+
+def A327666(n):
+    return sum(
+        -1 if reduce(lambda a, b: ~(a ^ b), factorint(i).values(), 0) & 1 else 1
+        for i in range(1, n + 1)
+    )
+
+
+def A065043(n):
+    return (reduce(ixor, factorint(n).values(), 0) & 1) ^ 1
+
+
+def A055037(n):
+    return sum(
+        1 for i in range(1, n + 1) if not (reduce(ixor, factorint(i).values(), 0) & 1)
+    )
+
+
+def A066829(n):
+    return reduce(ixor, factorint(n).values(), 0) & 1
+
+
+def A055038(n):
+    return sum(1 for i in range(1, n + 1) if reduce(ixor, factorint(i).values(), 0) & 1)
+
+
+def A002053(n):
+    return next(
+        filter(
+            lambda m: -n
+            == sum(
+                -1 if reduce(ixor, factorint(i).values(), 0) & 1 else 1
+                for i in range(1, m + 1)
+            ),
+            count(1),
+        )
+    )
+
+
+def A056239(n):
+    return sum(primepi(p) * e for p, e in factorint(n).items())
+
+
+def A359362(n):
+    return (sum((f := factorint(n)).values()) + 1) * sum(
+        primepi(p) * e for p, e in f.items()
+    )
+
+
+def A239122(n):
+    return sum(
+        -i if reduce(ixor, factorint(i).values(), 0) & 1 else i for i in range(1, n + 1)
+    )
+
+
+def A212496(n):
+    return sum(
+        -1 if reduce(ixor, factorint(i).values(), i) & 1 else 1 for i in range(1, n + 1)
+    )
+
+
+def A166486(n):
+    return (0, 1, 1, 1)[n & 3]
+
+
+@lru_cache(maxsize=None)
+def A127699(n):
+    return 1 if n == 1 else lcm(n, A127699(reduced_totient(n)))
+
+
+def A359098_gen():  # generator of terms
+    for a in count(3):
+        a10 = 10**a
+        for ad in range(1, 10):
+            for b in range(2, a):
+                b10 = 10**b
+                for bd in range(1, 10):
+                    for c in range(1, b):
+                        c10 = 10**c
+                        for cd in range(1, 10):
+                            for dd in range(1, 10):
+                                yield ad * a10 + bd * b10 + cd * c10 + dd
+
+
+def A358934(n):
+    return sum(f := fib2(n)) ** 5 - f[1] ** 5
+
+
+def A110299(n):
+    c = 0
+    for i in range(n):
+        c = (c << 1) + prime(i + 1)
+    return c
+
+
+def A358737_gen():  # generator of terms
+    for a in count(3):
+        a10 = 10**a
+        for ad in range(1, 10):
+            for b in range(2, a):
+                b10 = 10**b
+                for bd in range(1, 10):
+                    for c in range(1, b):
+                        c10 = 10**c
+                        yield from (
+                            max(primefactors(ad * a10 + bd * b10 + cd * c10 + dd))
+                            for cd in range(1, 10)
+                            for dd in range(1, 10)
+                        )
+
+
+def A359473(n):
+    return int(all(map(lambda m: not ((k := m + 1) & -k) ^ k, factorint(n).values())))
+
+
+def A036537_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: all(
+            map(lambda m: not ((k := m + 1) & -k) ^ k, factorint(n).values())
+        ),
+        count(max(startvalue, 1)),
+    )
+
+
+def A162643_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: any(map(lambda m: ((k := m + 1) & -k) ^ k, factorint(n).values())),
+        count(max(startvalue, 1)),
+    )
+
+
+def A072587_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: not all(map(lambda m: m & 1, factorint(n).values())),
+        count(max(startvalue, 1)),
+    )
+
+
+def A295316(n):
+    return int(all(map(lambda m: m & 1, factorint(n).values())))
+
+
+if sys.version_info >= (3, 10):
+
+    def A359464(n):
+        return reduce(ixor, (d.bit_count() for d in factorint(n).values()), 1) & 1
+
+else:
+
+    def A359464(n):
+        return reduce(ixor, (bin(d).count("1") for d in factorint(n).values()), 1) & 1
+
+
+def A175496_gen(startvalue=2):  # generator of terms
+    return filter(
+        lambda n: max(f := factorint(n).values()) > 1
+        and all(map(lambda m: not ((k := m + 1) & -k) ^ k, f)),
+        count(max(startvalue, 2)),
+    )
+
+
+def A353457(n):
+    return prod(-int(e == 1) for p, e in factorint(n).items() if primepi(p) & 1)
+
+
+def A353458(n):
+    return prod(-int(e == 1) for p, e in factorint(n).items() if not primepi(p) & 1)
+
+
+def A353459(n):
+    f = [(primepi(p) & 1, -int(e == 1)) for p, e in factorint(n).items()]
+    return prod(e for p, e in f if not p) + prod(e for p, e in f if p)
+
+
+def A100716_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: any(map(lambda d: d[1] >= d[0], factorint(n).items())),
+        count(max(startvalue, 1)),
+    )
+
+
+def A048103_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: all(map(lambda d: d[1] < d[0], factorint(n).items())),
+        count(max(startvalue, 1)),
+    )
+
+
+def A358548_gen():  # generator of terms
+    p, q = 2, 5
+    while True:
+        while not isprime(q):
+            q += 3
+        yield q - p
+        p = q
+        q += 3
+
+
+def A358565_gen():  # generator of terms
+    p, q = 5, 11
+    while True:
+        while not isprime(q):
+            q += 3
+        yield (q - p) // 6
+        p = q
+        q += 3
+
+
+def A359469(n):
+    f = [(primepi(p) & 1, int(e == 1)) for p, e in factorint(n).items()]
+    return reduce(iand, (e for p, e in f if not p), 1) ^ reduce(
+        iand, (e for p, e in f if p), 1
+    )
+
+
+def A359550(n):
+    return int(all(map(lambda d: d[0] > d[1], factorint(n).items())))
+
+
+def A359552(n):
+    return int(any(map(lambda d: d[1] % d[0], factorint(n).items()))) ^ 1
+
+
+def A359551(n):
+    return prod(
+        1 if (d := e % p) == 0 else (-1 if d == 1 else 0)
+        for p, e in factorint(n).items()
+    )
+
+
+def A359402_gen(startvalue=0):  # generator of terms
+    return filter(
+        lambda n: (
+            r := reduce(
+                lambda c, d: (c[0] + d[0] * (e := int(d[1])), c[1] + e),
+                enumerate(bin(n)[2:], start=1),
+                (0, 0),
+            )
+        )[0]
+        << 1
+        == (n.bit_length() + 1) * r[1],
+        count(max(startvalue, 0)),
+    )
+
+
+def A053866(n):
+    return int(is_square(n) or is_square(n << 1))
+
+
+def A028982_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: int(is_square(n) or is_square(n << 1)), count(max(startvalue, 1))
+    )
+
+
+def A359495(n):
+    k = n.bit_length() - 1
+    return sum((i << 1) - k for i, j in enumerate(bin(n)[2:]) if j == "1")
+
+
+def A230877(n):
+    return sum(i for i, j in enumerate(bin(n)[2:], 1) if j == "1")
+
+
+def A230204(n):
+    return sum(i for i, j in enumerate(bin(n)[2:]) if j == "1")
+
+
+def A035263(n):
+    return (n & -n).bit_length() & 1
+
+
+def A039963(n):
+    return ((m := (n >> 1) + 1) & -m).bit_length() & 1
+
+
+def A081706_gen():  # generator of terms
+    for n in count(0):
+        if (n & -n).bit_length() & 1:
+            m = n << 2
+            yield m - 2
+            yield m - 1
+
+
+def A359592(n):
+    return (mobius(n) & 1) ^ (0 if n & 1 else mobius(n >> 1) & 1)
+
+
+def A096268(n):
+    return (~(n + 1) & n).bit_length() & 1
+
+
+def A056832(n):
+    return 1 + ((~n & n - 1).bit_length() & 1)
+
+
+def A197911(n):
+    return n + sum((~(i + 1) & i).bit_length() & 1 for i in range(n))
+
+
+def A214682(n):
+    return n >> 1 if (~n & n - 1).bit_length() & 1 else n
+
+
+def A096271(n):
+    return (~(n + 1) & n).bit_length() % 3
+
+
+def A359593(n):
+    return prod(p**e for p, e in factorint(n).items() if e % p)
+
+
+def A359594(n):
+    return prod(p**e for p, e in factorint(n).items() if not e % p)
+
+
+def A359591(n):
+    return (
+        mobius(n)
+        if n & 1
+        else (
+            0
+            if (m := n >> 1) & 1
+            else prod(-int(e == 1) for e in factorint(m).values())
+        )
+    )
+
+
+def A356809_gen():  # generator of terms
+    a, b = 1, 2
+    while True:
+        if any(p & 3 == 3 and e & 1 for p, e in factorint(a).items()):
+            yield a
+        a, b = b, a + b
+
+
+def A152822(n):
+    return (1, 1, 0, 1)[n & 3]
+
+
+def A186646(n):
+    return n if n & 3 else n >> 1
+
+
+def A283971(n):
+    return n if (n - 2) & 3 else n >> 1
+
+
+def A141726(n):
+    return (0, 8, 7, 6, 5, 4, 3, 2, 1)[n % 9]
+
+
+def A003266_gen():  # generator of terms
+    a, b, c = 1, 1, 1
+    while True:
+        yield c
+        c *= a
+        a, b = b, a + b
+
+
+def A012245(n):
+    c = 1
+    for i in count(1):
+        if (c := c * i) >= n:
+            return int(c == n)
+
+
+def A359456(n):
+    a, b, c = 1, 2, 1
+    while (c := c * a) < n:
+        a, b = b, a + b
+    return int(c == n)
+
+
+def A316341(n):
+    c, i = 1, 1
+    while (c := c * i) < n:
+        i += 1
+    return int(c == n)
+
+
+def A143963(n):
+    c, i, s = 1, 1, 0
+    while (c := c * i) <= n:
+        s += comb(n, c)
+        i += 1
+    return s
+
+
+def A359549(n):
+    return int(
+        (m := (~n & n - 1).bit_length()) < 2
+        and all(e == 2 for e in factorint(n >> m).values())
+    )
+
+
+def A359580_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: (m := (~n & n - 1).bit_length()) <= 1
+        and all(e == 2 for e in factorint(n >> m).values()),
+        count(max(startvalue, 1)),
+    )
+
+
+def A359684(n):
+    return 1 if n == 1 else max(primefactors((1 << n) - n))
+
+
+def A359685(n):
+    return max(primefactors((1 << n) + n))
+
+
+def A006127(n):
+    return (1 << n) + n
+
+
+def A000325(n):
+    return (1 << n) - n
+
+
+def A359600(n):
+    return prod(
+        prime(i) ** e
+        for i, e in enumerate(sorted(factorint(n).values(), reverse=True), 2)
+    )
+
+
+def A359421(n):
+    return prod(npartitions(d) for d in factorint(prime(n) ** 2 - 1).values())
+
+
+def A089640(n):
+    return sum(binomial(k, n - 1 - (3 * k >> 1)) for k in range(n + 1))
+
+
+def A036347_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: (reduce(ixor, (p * e for p, e in factorint(n).items()), 0) ^ n) & 1,
+        count(max(startvalue, 1)),
+    )
+
+
+def A359768(n):
+    return (reduce(ixor, (p * e for p, e in factorint(n).items()), 0) ^ n) & 1
+
+
+def A359844(n):
+    return ((n << 1) + 1) ** 8 + 1 >> 1
+
+
+def A359498(n):
+    return ((n << 1) + 1) ** 8 - 1 >> 5
+
+
+def A359499(n):
+    return ((n << 1) + 1) ** 16 - 1 >> 6
+
+
+def A359500(n):
+    return 7 ** (1 << n) - 1 >> n + 3
+
+
+def A358272(n):
+    return prod(
+        -(p ** (e & -2)) if e & 1 else p ** (e & -2) for p, e in factorint(n).items()
+    )
+
+
+def A010684(n):
+    return 3 if n & 1 else 1
+
+
+def A112033(n):
+    return 3 * (1 << (n >> 1) + (int(not n & 1) << 1))
+
+
+def A166681_gen():  # generator of terms
+    p = 13
+    while True:
+        for q in multiset_permutations(str(p)):
+            if (r := int("".join(q))) > p and isprime(r):
+                yield p
+                break
+        p = nextprime(p)
+
+
+def A048675(n):
+    return sum(e << primepi(p) - 1 for p, e in factorint(n).items())
+
+
+def A359830_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: sum(e << primepi(p) - 1 for p, e in factorint(n).items()) % 3,
+        count(max(startvalue, 1)),
+    )
+
+
+def A320770(n):
+    return -(1 << (n >> 1)) if n & 4 else 1 << (n >> 1)
+
+
+def A014848(n):
+    return n**2 - (n >> 1)
+
+
+def A173511(n):
+    return (n**2 << 2) + (n >> 1)
+
+
+def A289296(n):
+    return (n - 1) * (n | 1)
+
+
+def A090932(n):
+    return factorial(n) >> (n >> 1)
+
+
+def A110138(n):
+    return ((m := n >> 1) + (n & 1)) ** m
+
+
+def A099202(n):
+    return 1 << (n**2 >> 1)
+
+
+def A272299(n):
+    return n + (n & -2) + 3 * (n // 3)
+
+
+def A110139(n):
+    return (m := n >> 1) ** m
+
+
+def A244586(n):
+    return n | 4
+
+
+def A244584(n):
+    return n | 3
+
+
+def A244587(n):
+    return n | 5
+
+
+def A143621(n):
+    return -1 if n & 4 else 1
+
+
+def A140730(n):
+    return ((n & 3) + 1) * 5 ** (n >> 2)
+
+
+def A133874(n):
+    return 1 + (n >> 2) & 3
+
+
+def A130909(n):
+    return n & 15
+
+
+def A080412(n):
+    return (0, 1, -1, 0)[n & 3] + n
+
+
+def A038714(n):
+    return (m := n >> 2) * (m + 1)
+
+
+def A053836(n):
+    return sum(int(d, 16) for d in hex(n)[2:])
+
+
+def A008838(n):
+    return (m := n >> 3) * (m + bool(n & 7))
+
+
+def A115273(n):
+    return prod(divmod(n, 3))
+
+
+def A257848(n):
+    return (n >> 3) * (n & 7)
+
+
+def A142150(n):
+    return (n + 1 >> 1) * (n & 1 ^ 1)
+
+
+def A257849(n):
+    return prod(divmod(n, 9))
+
+
+def A004457(n):
+    return n ^ 16
+
+
+def A100281(n):
+    return n ^ (m := n >> 2) ^ (m >> 2)
+
+
+if sys.version_info >= (3, 10):
+
+    def A359496_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: sum(i for i, j in enumerate(bin(n)[2:]) if j == "1") << 1
+            < n.bit_count() * (n.bit_length() - 1),
+            count(max(startvalue, 0)),
+        )
+
+    def A088149(n):
+        if n == 1:
+            return 2
+        for p in count((1 << n) - 1, 2):
+            if p.bit_count() >= n and isprime(p):
+                m = p.bit_length()
+                l = 1 << m - 1
+                k, cset, q = l - 1, {p}, p
+                for _ in range(m - 1):
+                    p = bool(p & l) + ((p & k) << 1)
+                    if p not in cset and isprime(p):
+                        cset.add(p)
+                if len(cset) == n:
+                    return q
+
+    def A088148(n):
+        if n == 1:
+            return 2
+        for p in count((1 << n) - 1):
+            if p.bit_count() >= n:
+                m = p.bit_length()
+                l = 1 << m - 1
+                k, cset, q = l - 1, set(), p
+                for _ in range(m):
+                    if p not in cset and isprime(p):
+                        cset.add(p)
+                    p = bool(p & l) + ((p & k) << 1)
+                if len(cset) == n:
+                    return q
+
+else:
+
+    def A359496_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: sum(i for i, j in enumerate(bin(n)[2:]) if j == "1") << 1
+            < bin(n).count("1") * (n.bit_length() - 1),
+            count(max(startvalue, 0)),
+        )
+
+    def A088149(n):
+        if n == 1:
+            return 2
+        for p in count((1 << n) - 1, 2):
+            if bin(p).count("1") >= n and isprime(p):
+                m = p.bit_length()
+                l = 1 << m - 1
+                k, cset, q = l - 1, {p}, p
+                for _ in range(m - 1):
+                    p = bool(p & l) + ((p & k) << 1)
+                    if p not in cset and isprime(p):
+                        cset.add(p)
+                if len(cset) == n:
+                    return q
+
+    def A088148(n):
+        if n == 1:
+            return 2
+        for p in count((1 << n) - 1):
+            if bin(p).count("1") >= n:
+                m = p.bit_length()
+                l = 1 << m - 1
+                k, cset, q = l - 1, set(), p
+                for _ in range(m):
+                    if p not in cset and isprime(p):
+                        cset.add(p)
+                    p = bool(p & l) + ((p & k) << 1)
+                if len(cset) == n:
+                    return q
+
+
+def A161602_gen(startvalue=1):  # generator of terms
+    return filter(lambda n: n > int(bin(n)[-1:1:-1], 2), count(max(startvalue, 1)))
+
+
+def A161603_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: n > int(bin(n)[-1:1:-1], 2), count(max(startvalue | 1, 1), 2)
+    )
+
+
+def A161601_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: n < int(bin(n)[-1:1:-1], 2), count(max(startvalue | 1, 1), 2)
+    )
+
+
+def A359840_gen():  # generator of terms
+    return map(
+        int,
+        filter(
+            lambda s: isprime(int(s, 5)), (gmpy2digits(prime(i), 4) for i in count(1))
+        ),
+    )
+
+
+def A059995(n):
+    return n // 10
+
+
+def A359841(n):
+    return (
+        (
+            10,
+            11,
+            12,
+            13,
+            14,
+            15,
+            16,
+            17,
+            18,
+            19,
+            20,
+            22,
+            24,
+            26,
+            28,
+            30,
+            33,
+            36,
+            39,
+            40,
+            44,
+            48,
+            50,
+            55,
+            60,
+            66,
+            70,
+            77,
+            80,
+            88,
+            90,
+            99,
+        )[n - 1]
+        if n <= 32
+        else (n - 23) * 10
+    )
+
+
+def A077947(n):
+    return (k := (m := 1 << n + 2) // 7) + int((m - 7 * k << 1) >= 7)
+
+
+def A080413(n):
+    return ((n & 3) << 1) + bool(n & 4) + (n & -8)
+
+
+def A080414(n):
+    return ((n & 6) >> 1) + ((n & 1) << 2) + (n & -8)
+
+
+def A080542(n):
+    return (1 + (n & 1)) * (1 << n.bit_length() - 2) + (n >> 1) if n > 1 else n
+
+
+def A080541(n):
+    return (
+        ((n & (m := 1 << n.bit_length() - 2) - 1) << 1) + (m << 1) + bool(m & n)
+        if n > 1
+        else n
+    )
+
+
+def A059893(n):
+    return int("1" + bin(n)[:2:-1], 2)
+
+
+def A168427(n):
+    return (21, 3, 9, 27)[n & 3] if n else 1
+
+
+def A336953(n):
+    if n == 0:
+        return 0
+    l, m = -(n % n.bit_length()), bin(n)[2:]
+    return int(m[l:] + m[:l], 2)
+
+
+def A038572(n):
+    return (n >> 1) + (1 << n.bit_length() - 1 if n & 1 else 0)
+
+
+def A006257(n):
+    return bool(n & (m := 1 << n.bit_length() - 1)) + ((n & m - 1) << 1) if n else 0
+
+
+def A062050(n):
+    return n - (1 << n.bit_length() - 1) + 1
+
+
+def A053645(n):
+    return n & (1 << n.bit_length() - 1) - 1
+
+
+def A359329(n):
+    return (n * (n - 4) + n * (n & 1)) >> 1
+
+
+def A000165(n):
+    return factorial(n) << n
+
+
+def A283027(n):
+    return n**4 * (n**4 * (n**8 + 1) + 2) >> 2
+
+
+def A283031(n):
+    return n**7 * (n**6 * (n**12 + 1) + 2) >> 2
+
+
+def A359832(n):
+    return (n & 1) | ((~n & n - 1).bit_length() & 1)
+
+
+def A328981(n):
+    return ((n & 1) | ((~n & n - 1).bit_length() & 1)) ^ 1
+
+
+def A359559(n):
+    return (
+        Matrix(
+            n,
+            n,
+            [
+                i - j + (1 if i > j else -1) if i != j else I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).det()
+        * (1, -I, -1, I)[n & 3]
+    )
+
+
+def A359560(n):
+    return (
+        Matrix(
+            n,
+            n,
+            [
+                i - j + (1 if i > j else -1) if i != j else I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).per()
+        * (1, -I, -1, I)[n & 3]
+        if n
+        else 1
+    )
+
+
+def A359561(n):
+    return (
+        Matrix(
+            n,
+            n,
+            [
+                (n + j - i if i > j else j - i - n) if i != j else n * I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).det()
+        * (1, -I, -1, I)[n & 3]
+    )
+
+
+def A359562(n):
+    return (
+        Matrix(
+            n,
+            n,
+            [
+                (n + j - i if i > j else j - i - n) if i != j else n * I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).per()
+        * (1, -I, -1, I)[n & 3]
+        if n
+        else 1
+    )
+
+
+def A359614(n):
+    return min(
+        Matrix(
+            n,
+            n,
+            [
+                (d[i - j] if i > j else -d[j - i]) if i != j else d[0] * I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).det()
+        * (1, -I, -1, I)[n & 3]
+        for d in permutations(range(1, n + 1))
+    )
+
+
+def A359615(n):
+    return max(
+        Matrix(
+            n,
+            n,
+            [
+                (d[i - j] if i > j else -d[j - i]) if i != j else d[0] * I
+                for i in range(n)
+                for j in range(n)
+            ],
+        ).det()
+        * (1, -I, -1, I)[n & 3]
+        for d in permutations(range(1, n + 1))
+    )
+
+
+def A359616(n):
+    return (
+        min(
+            Matrix(
+                n,
+                n,
+                [
+                    (d[i - j] if i > j else -d[j - i]) if i != j else d[0] * I
+                    for i in range(n)
+                    for j in range(n)
+                ],
+            ).per()
+            * (1, -I, -1, I)[n & 3]
+            for d in permutations(range(1, n + 1))
+        )
+        if n
+        else 1
+    )
+
+
+def A359617(n):
+    return (
+        max(
+            Matrix(
+                n,
+                n,
+                [
+                    (d[i - j] if i > j else -d[j - i]) if i != j else d[0] * I
+                    for i in range(n)
+                    for j in range(n)
+                ],
+            ).per()
+            * (1, -I, -1, I)[n & 3]
+            for d in permutations(range(1, n + 1))
+        )
+        if n
+        else 1
+    )
+
+
+def A293296(n):
+    return (n**2 << 1) - (n >> 2)
+
+
+def A007877(n):
+    return (0, 1, 2, 1)[n & 3]
+
+
+def A193682(n):
+    return (0, 1, 2, 3, 0, 3, 2, 1)[n & 7]
+
+
+def A190785(n):
+    a, b = divmod(n - 1, 7)
+    return (0, 2, 3, 5, 7, 9, 11)[b] + 12 * a
+
+
+def A004525(n):
+    return ((n >> 1) & -2) + bool(n & 3)
+
+
+def A004524(n):
+    return -(bool((m := n + 1) & 3) ^ 1) + ((m >> 1) & -2)
+
+
+def A004655(n):
+    return 10 ** (n >> 2) << (n & 3)
+
+
+def A047573(n):
+    a, b = divmod(n - 1, 7)
+    return (0, 1, 2, 4, 5, 6, 7)[b] + (a << 3)
+
+
+def A257844(n):
+    return (n >> 2) * (n & 3)
+
+
+def A238170(n):
+    return isqrt(n**9)
+
+
+def A360080(n):
+    if n <= 1:
+        return 1
+    m = 1 << (1 << n) - 1
+    i = m
+    while i := nextprime(i):
+        if isprime((k := i << 1) + 1):
+            return k - (m << 1) + 1
+
+
+def A360081(n):
+    m = 1 << 3 * (1 << n) - 1
+    i = m
+    while i := nextprime(i):
+        if isprime((k := i << 1) + 1):
+            return k - (m << 1) + 1
+
+
+def A360067(n):
+    return Matrix(
+        n, n, [i**j * (i - j) for i in range(1, n + 1) for j in range(1, n + 1)]
+    ).det()
+
+
+def A002450(n):
+    return ((1 << (n << 1)) - 1) // 3
+
+
+def A048647(n):
+    return n ^ ((n & ((1 << (m := n.bit_length()) + (m & 1)) - 1) // 3) << 1)
+
+
+def A271324(n):
+    return n + (n >> 2) + (n & 3)
+
+
+def A063224(n):
+    return n - 1 + sum(divmod(n - 1, 3))
+
+
+def A273308(n):
+    return n + sum(divmod(n, 3)) if n > 1 else 0
+
+
+def A063200(n):
+    return n - 1 + sum(divmod(n - 1, 3)) if n > 1 else 1
+
+
+def A265888(n):
+    return n + (-(n >> 2) if n & 1 else n >> 2)
+
+
+def A063695(n):
+    return n & ((1 << (m := n.bit_length()) + (m & 1 ^ 1)) - 1) // 3
+
+
+def A090569(n):
+    return (n - 1 & ((1 << (m := (n - 1).bit_length()) + (m & 1 ^ 1)) - 1) // 3) + 1
+
+
+def A063694(n):
+    return n & ((1 << (m := n.bit_length()) + (m & 1)) - 1) // 3
+
+
+def A088442(n):
+    return ((n & ((1 << (m := n.bit_length()) + (m & 1)) - 1) // 3) << 1) + 1
+
+
+def A004514(n):
+    return (n & ((1 << (m := n.bit_length()) + (m & 1)) - 1) // 3) << 1
+
+
+def A200675(n):
+    return 1 << (n >> 2)
+
+
+def A055264(n):
+    return (0, 1, 3, 6)[n & 3] + 9 * (n >> 2)
+
+
+def A174438(n):
+    return (0, 2, 5, 8)[n & 3] + 9 * (n >> 2)
+
+
+def A122461(n):
+    return n >> 1 & -2
+
+
+def A122587(n):
+    return int(bin(n)[2 : 3 + (n.bit_length() & 1 ^ 1)], 2)
+
+
+def A214864(n):
+    return (10, 11, 14, 15)[n - 1 & 3] + ((n - 1 & -4) << 2)
+
+
+def A131478(n):
+    return n**4 + 3 >> 2
+
+
+def A030301(n):
+    return n.bit_length() & 1 ^ 1
+
+
+def A030300(n):
+    return n.bit_length() & 1
+
+
+def A000975(n):
+    return ((1 << n + 1) - 1 - (n & 1 ^ 1)) // 3
+
+
+def A079954(n):
+    return ((1 << k) - 2) // 3 if (k := n.bit_length()) & 1 else n - ((1 << k) - 1) // 3
+
+
+def A079947(n):
+    return n - ((1 << k) - 2) // 3 if (k := n.bit_length()) & 1 else ((1 << k) - 1) // 3
+
+
+def A206925(n):
+    s = bin(n)[2:]
+    k = len(s)
+    return sum(
+        1
+        for i in range(k)
+        for j in range(i + 1, k + 1)
+        if s[i:j] == s[j - 1 : i - 1 - k : -1]
+    )
+
+
+def A187323(n):
+    return 3 * (n >> 2) + bool(n & 2) + n // 3
+
+
+def A187321(n):
+    return 3 * (n >> 2) + bool(n & 2)
+
+
+def A187324(n):
+    return (n >> 2) + bool(n & 2) + n // 3
+
+
+def A187322(n):
+    return (n >> 1) + (3 * n >> 2)
+
+
+def A186421(n):
+    return (n >> 1) | 1 if n & 1 else n
+
+
+def A087960(n):
+    return -1 if n + 1 & 2 else 1
+
+
+def A186423(n):
+    return (
+        6 * n * (n + 1)
+        + 3
+        + (-2 * n - 1 if n & 1 else 2 * n + 1)
+        + (4 if n + 1 & 2 else -4)
+    ) >> 4
+
+
+def A186424(n):
+    return (n * (3 * n + 2) + 1 if n & 1 else n * (3 * n + 4) + 2) >> 1
+
+
+def A062717(n):
+    return (n * (3 * n + 4) + 1 if n & 1 else n * (3 * n + 2)) >> 1
+
+
+def A001318(n):
+    return (n * (3 * n + 4) + 1 if n & 1 else n * (3 * n + 2)) >> 3
+
+
+def A177332(n):
+    return (n * (n * (2 * n + 3) + 1) + 84) // 174
+
+
+def A129756(n):
+    return (n >> 1) | 1
+
+
+def A131078(n):
+    return int(not n - 1 & 4)
+
+
+def A131479(n):
+    return n**4 >> 2
+
+
+def A133872(n):
+    return int(not n & 2)
+
+
+def A112030(n):
+    return (3, 1, -3, -1)[n & 3]
+
+
+def A099254(n):
+    a, b = divmod(n, 3)
+    return (1 + (b & 1)) * (-a - 1 if a & 1 else a + 1)
+
+
+def A008217(n):
+    return (n >> 2) * (n + 1 >> 2)
+
+
+def A038715(n):
+    return (n >> 2) * (1 + (n + 1 >> 2))
+
+
+def A051036(n):
+    return comb(n, n >> 2)
+
+
+def A037827(n):
+    s = "0" * (n.bit_length() & 1) + bin(n)[2:]
+    return sum(1 for i in range(0, len(s) - 2, 2) if s[i : i + 2] >= s[i + 2 : i + 4])
+
+
+def A173562(n):
+    return n**2 + (n >> 2)
+
+
+def A173707(n):
+    return n * (n * (n * (n + 2) + 1) - 4) // 12
+
+
+def A160529(n):
+    return 25 * (n >> 2) + (0, 1, 5, 6)[n & 3]
+
+
+def A360297(n):
+    p = prime(n)
+    q = nextprime(p)
+    s, k = p + q, 1
+    while s % (q := nextprime(q)):
+        k += 1
+        s += q
+    return k
+
+
+def A360311(n):
+    p = prime(n)
+    q = nextprime(p)
+    s, k = p + q, 1
+    while s % (q := nextprime(q)):
+        k += 1
+        s += q
+    return s
+
+
+def A360312(n):
+    p = prime(n)
+    q = nextprime(p)
+    s, k = p + q, 1
+    while s % (q := nextprime(q)):
+        k += 1
+        s += q
+    return q
+
+
+def A295643(n):
+    return (n >> 2) ** 2
+
+
+def A360376(n):
+    p = prime(n)
+    s, k = p, 0
+    while (s + 1) % (p := nextprime(p)):
+        k += 1
+        s *= p
+    return k
+
+
+def A360406(n):
+    p = prime(n)
+    q = nextprime(p)
+    s, k = p * q, 1
+    while (s - 1) % (q := nextprime(q)):
+        k += 1
+        s *= q
+    return k
+
+
+def A038040(n):
+    return divisor_count(n) * n
+
+
+def A360388_gen(startvalue=1):  # generator of terms
+    for n in count(max(startvalue, 1)):
+        b = tuple(int(d) for d in bin(n)[2:])
+        m = len(b)
+        if all(reduce(ixor, (b[i] & b[i + k] for i in range(m - k))) for k in range(m)):
+            yield n
+
+
+def A053006_gen(startvalue=1):  # generator of terms
+    return filter(lambda n: n_order(2, (n << 1) - 1) & 1, count(max(startvalue, 1)))
+
+
+def A036259_gen(startvalue=1):  # generator of terms
+    return filter(lambda n: n_order(2, n) & 1, count(max(startvalue, 1) | 1, 2))
+
+
+def A067695(n):
+    if n == 1:
+        return 1
+    f, g = map(tuple, zip(*sorted(factorint(n).items())))
+    return f[g.index(min(g))]
+
+
+def A359612(n):
+    return (f := list(map(tuple, zip(*sorted(factorint(n).items(), reverse=True)))))[0][
+        f[1].index(min(f[1]))
+    ]
+
+
+def A360053_gen():  # generator of terms
+    for i in count(1):
+        p = prime(i)
+        if all((pow(2, p - 1, prime(j) ** 2) - 1 for j in range(1, i))):
+            yield p
+
+
+def A359178_gen(startvalue=2):  # generator of terms
+    return filter(
+        lambda n: (f := list(factorint(n).values())).count(min(f)) == 1,
+        count(max(startvalue, 2)),
+    )
+
+
+def A348699_gen():  # generator of terms
+    return filter(
+        lambda p: isprime(sum(1 for d in str(p) if d in {"2", "3", "5", "7"})),
+        (prime(i) for i in count(1)),
+    )
+
+
+def A092619_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: isprime(sum(1 for d in str(n) if d in {"2", "3", "5", "7"})),
+        count(max(startvalue, 1)),
+    )
+
+
+def A085557_gen(startvalue=1):  # generator of terms
+    return filter(
+        lambda n: len(s := str(n))
+        < (sum(1 for d in s if d in {"2", "3", "5", "7"}) << 1),
+        count(max(startvalue, 1)),
+    )
+
+
+def A046034_gen():  # generator of terms
+    yield from (int("".join(d)) for l in count(1) for d in product("2357", repeat=l))
+
+
+def A084544(n):
+    m = (3 * n + 1).bit_length() - 1 >> 1
+    return int(
+        "".join(
+            (
+                str(
+                    ((3 * n + 1 - (1 << (m << 1))) // (3 << ((m - 1 - j) << 1)) & 3) + 1
+                )
+                for j in range(m)
+            )
+        )
+    )
+
+
+def A046034(n):
+    m = (3 * n + 1).bit_length() - 1 >> 1
+    return int(
+        "".join(
+            (
+                "2357"[(3 * n + 1 - (1 << (m << 1))) // (3 << ((m - 1 - j) << 1)) & 3]
+                for j in range(m)
+            )
+        )
+    )
+
+
+def A084544_gen():  # generator of terms
+    yield from (int("".join(d)) for l in count(1) for d in product("1234", repeat=l))
+
+
+def A045926(n):
+    m = (3 * n + 1).bit_length() - 1 >> 1
+    return (
+        int(
+            "".join(
+                (
+                    str(
+                        ((3 * n + 1 - (1 << (m << 1))) // (3 << ((m - 1 - j) << 1)) & 3)
+                        + 1
+                    )
+                    for j in range(m)
+                )
+            )
+        )
+        << 1
+    )
+
+
+def A045926_gen():  # generator of terms
+    yield from (
+        int("".join(d)) << 1 for l in count(1) for d in product("1234", repeat=l)
+    )
+
+
+def A358348(n):
+    return (0, 1, 4, 7, 9, 10, 13, 16, 17)[m := n % 9] + (n - m << 1)
+
+
+def A189510(n):
+    return (9, 1, 4, 9, 4, 2, 9, 7, 1, 9, 1, 5, 9, 4, 7, 9, 7, 8)[n % 18] if n else 1
+
+
+def A145389(n):
+    return (9, 1, 3, 6, 1, 6, 3, 1, 9)[n % 9] if n else 0
+
+
+def A061579(n):
+    return (r := isqrt((n << 3) + 1) - 1 >> 1) * (r + 2) - n
+
+
+def A137688(n):
+    return 1 << (isqrt((n << 3) + 1) - 1 >> 1)
+
+
+def A181133(n):
+    return n + (isqrt((n << 3) + 1) - 1 >> 1)
+
+
+def A022846(n):
+    return isqrt(n**2 << 3) + 1 >> 1
+
+
+def A023532(n):
+    return bool(is_square((n << 3) + 9)) ^ 1
+
+
+def A089633_gen():  # generator of terms
+    return ((1 << t) - (1 << k) - 1 for t in count(1) for k in range(t - 1, -1, -1))
+
+
+def A101688(n):
+    return isqrt((m := n << 1) + 1) - (isqrt((m << 2) + 8) + 1 >> 1) + 1
+
+
+if sys.version_info >= (3, 10):
+
+    def A014081(n):
+        return (n & (n >> 1)).bit_count()
+
+    def A245195(n):
+        return 1 << (n & (n >> 1)).bit_count()
+
+    def A020985(n):
+        return -1 if (n & (n >> 1)).bit_count() & 1 else 1
+
+    def A020986(n):
+        return sum(-1 if (m & (m >> 1)).bit_count() & 1 else 1 for m in range(n + 1))
+
+    def A020987(n):
+        return (n & (n >> 1)).bit_count() & 1
+
+    def A022155_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: (n & (n >> 1)).bit_count() & 1, count(max(startvalue, 0))
+        )
+
+    def A203463_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: (n & (n >> 1)).bit_count() & 1 ^ 1, count(max(startvalue, 0))
+        )
+
+    def A203531_gen():  # generator of terms
+        c, a = 0, 1
+        for n in count(0):
+            if (n & (n >> 1)).bit_count() & 1 ^ a:
+                c += 1
+            else:
+                yield c
+                c = 1
+                a ^= 1
+
+    def A020990(n):
+        return sum(
+            -1 if ((m & (m >> 1)).bit_count() ^ m) & 1 else 1 for m in range(n + 1)
+        )
+
+    def A213786(n):
+        return sum(
+            (-1 if (i & (i >> 1)).bit_count() & 1 else 1)
+            * sum(
+                -1 if (j & (j >> 1)).bit_count() & 1 else 1 for j in range(i + 1, n + 1)
+            )
+            for i in range(1, n + 1)
+        )
+
+    def A213626(n):
+        return sum(
+            (-1 if (i & (i >> 1)).bit_count() & 1 else 1)
+            * sum(
+                (-1 if (j & (j >> 1)).bit_count() & 1 else 1)
+                * sum(
+                    -1 if (k & (k >> 1)).bit_count() & 1 else 1
+                    for k in range(j + 1, n + 1)
+                )
+                for j in range(i + 1, n + 1)
+            )
+            for i in range(n + 1)
+        )
+
+    def A359045(n):
+        return sum(
+            (-1 if (i & (i >> 1)).bit_count() & 1 else 1)
+            * sum(
+                (-1 if (j & (j >> 1)).bit_count() & 1 else 1)
+                * sum(
+                    -1 if (k & (k >> 1)).bit_count() & 1 else 1
+                    for k in range(j + 1, n + 1)
+                )
+                for j in range(i + 1, n + 1)
+            )
+            for i in range(1, n + 1)
+        )
+
+    def A239904(n):
+        return n - n.bit_count() + (n & (n >> 1)).bit_count()
+
+else:
+
+    def A014081(n):
+        return bin(n & (n >> 1)).count("1")
+
+    def A245195(n):
+        return 1 << bin(n & (n >> 1)).count("1")
+
+    def A020985(n):
+        return -1 if bin(n & (n >> 1)).count("1") & 1 else 1
+
+    def A020986(n):
+        return sum(-1 if bin(m & (m >> 1)).count("1") & 1 else 1 for m in range(n + 1))
+
+    def A020987(n):
+        return bin(n & (n >> 1)).count("1") & 1
+
+    def A022155_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: bin(n & (n >> 1)).count("1") & 1, count(max(startvalue, 0))
+        )
+
+    def A203463_gen(startvalue=0):  # generator of terms
+        return filter(
+            lambda n: bin(n & (n >> 1)).count("1") & 1 ^ 1, count(max(startvalue, 0))
+        )
+
+    def A203531_gen():  # generator of terms
+        c, a = 0, 1
+        for n in count(0):
+            if bin(n & (n >> 1)).count("1") & 1 ^ a:
+                c += 1
+            else:
+                yield c
+                c = 1
+                a ^= 1
+
+    def A020990(n):
+        return sum(
+            -1 if (bin(m & (m >> 1)).count("1") ^ m) & 1 else 1 for m in range(n + 1)
+        )
+
+    def A213786(n):
+        return sum(
+            (-1 if bin(i & (i >> 1)).count("1") & 1 else 1)
+            * sum(
+                -1 if bin(j & (j >> 1)).count("1") & 1 else 1
+                for j in range(i + 1, n + 1)
+            )
+            for i in range(1, n + 1)
+        )
+
+    def A213626(n):
+        return sum(
+            (-1 if bin(i & (i >> 1)).count("1") & 1 else 1)
+            * sum(
+                (-1 if bin(j & (j >> 1)).count("1") & 1 else 1)
+                * sum(
+                    -1 if bin(k & (k >> 1)).count("1") & 1 else 1
+                    for k in range(j + 1, n + 1)
+                )
+                for j in range(i + 1, n + 1)
+            )
+            for i in range(n + 1)
+        )
+
+    def A359045(n):
+        return sum(
+            (-1 if bin(i & (i >> 1)).count("1") & 1 else 1)
+            * sum(
+                (-1 if bin(j & (j >> 1)).count("1") & 1 else 1)
+                * sum(
+                    -1 if bin(k & (k >> 1)).count("1") & 1 else 1
+                    for k in range(j + 1, n + 1)
+                )
+                for j in range(i + 1, n + 1)
+            )
+            for i in range(1, n + 1)
+        )
+
+    def A239904(n):
+        return n - bin(n).count("1") + bin(n & (n >> 1)).count("1")
+
+
+def A014493(n):
+    return ((n << 1) - 1) * (n - (n & 1 ^ 1))
+
+
+def A352116(n):
+    return n * ((n - 1) << 1) * (n + 1) // 3 + n * (n & 1)
+
+
+def A000447(n):
+    return n * ((n**2 << 2) - 1) // 3
```

### Comparing `OEISsequences-0.1.8/setup.py` & `OEISsequences-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 with open("requirements.txt", "r") as fh:
     requirements = [line.strip() for line in fh]
 
 setup(
    name='OEISsequences',
    python_requires='>= 3.8',
-   version='0.1.8',
+   version='0.1.9',
    author='Chai Wah Wu',
    author_email='cwwuieee@gmail.com',
    packages=find_packages(),
    url='https://github.com/postvakje/oeis-sequences',
    license='LICENSE',
    description='Python functions to generate OEIS sequences',
    long_description=long_description,
```

