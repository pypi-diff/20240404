# Comparing `tmp/numbertheory-0.0.3.tar.gz` & `tmp/numbertheory-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbertheory-0.0.3.tar", last modified: Fri Mar 29 20:54:51 2024, max compression
+gzip compressed data, was "numbertheory-0.0.4.tar", last modified: Thu Apr  4 14:29:14 2024, max compression
```

## Comparing `numbertheory-0.0.3.tar` & `numbertheory-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 20:54:51.469444 numbertheory-0.0.3/
--rw-rw-rw-   0        0        0     2025 2024-03-29 20:54:51.468443 numbertheory-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-29 20:54:51.462534 numbertheory-0.0.3/numbertheory/
--rw-rw-rw-   0        0        0      196 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/__init__.py
--rw-rw-rw-   0        0        0     1187 2024-03-29 20:43:55.000000 numbertheory-0.0.3/numbertheory/common_functions.py
--rw-rw-rw-   0        0        0      868 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/elliptic_curves.py
--rw-rw-rw-   0        0        0      955 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/fibonacci.py
--rw-rw-rw-   0        0        0      718 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/generating_primes.py
--rw-rw-rw-   0        0        0      755 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/integer_factorization.py
--rw-rw-rw-   0        0        0      559 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/modulus_operations.py
--rw-rw-rw-   0        0        0     1240 2024-03-29 15:35:51.000000 numbertheory-0.0.3/numbertheory/primality_tests.py
-drwxrwxrwx   0        0        0        0 2024-03-29 20:54:51.467521 numbertheory-0.0.3/numbertheory.egg-info/
--rw-rw-rw-   0        0        0     2025 2024-03-29 20:54:51.000000 numbertheory-0.0.3/numbertheory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2024-03-29 20:54:51.000000 numbertheory-0.0.3/numbertheory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 20:54:51.000000 numbertheory-0.0.3/numbertheory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-03-29 20:54:51.000000 numbertheory-0.0.3/numbertheory.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-29 20:54:51.000000 numbertheory-0.0.3/numbertheory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 20:54:51.469444 numbertheory-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      896 2024-03-29 20:54:47.000000 numbertheory-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:29:14.604676 numbertheory-0.0.4/
+-rw-rw-rw-   0        0        0     2795 2024-04-04 14:29:14.604676 numbertheory-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-04 14:29:14.586526 numbertheory-0.0.4/numbertheory/
+-rw-rw-rw-   0        0        0      228 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/__init__.py
+-rw-rw-rw-   0        0        0     1557 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/common_functions.py
+-rw-rw-rw-   0        0        0     1496 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/discrete-log-problem.py
+-rw-rw-rw-   0        0        0     1624 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/elliptic_curves.py
+-rw-rw-rw-   0        0        0      955 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/fibonacci.py
+-rw-rw-rw-   0        0        0      718 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/generating_primes.py
+-rw-rw-rw-   0        0        0     1385 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/integer_factorization.py
+-rw-rw-rw-   0        0        0      717 2024-04-04 14:28:12.000000 numbertheory-0.0.4/numbertheory/modulus_operations.py
+-rw-rw-rw-   0        0        0     1240 2024-04-04 14:28:13.000000 numbertheory-0.0.4/numbertheory/primality_tests.py
+drwxrwxrwx   0        0        0        0 2024-04-04 14:29:14.600676 numbertheory-0.0.4/numbertheory.egg-info/
+-rw-rw-rw-   0        0        0     2795 2024-04-04 14:29:14.000000 numbertheory-0.0.4/numbertheory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      479 2024-04-04 14:29:14.000000 numbertheory-0.0.4/numbertheory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-04 14:29:14.000000 numbertheory-0.0.4/numbertheory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-04-04 14:29:14.000000 numbertheory-0.0.4/numbertheory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-04 14:29:14.000000 numbertheory-0.0.4/numbertheory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-04 14:29:14.604676 numbertheory-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      896 2024-04-04 14:29:09.000000 numbertheory-0.0.4/setup.py
```

### Comparing `numbertheory-0.0.3/numbertheory/common_functions.py` & `numbertheory-0.0.4/numbertheory/integer_factorization.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-def gcd(a: int, b: int) -> int:
-    while b != 0:
-        a, b = b, a % b
-    return a
-
-
-def lcm(a: int, b: int) -> int:
-    return abs(a * b) // gcd(a, b)
-
-
-def extended_euclidean(a: int, b: int) -> tuple[int, int, int]:
-    x_prev, x, y_prev, y = 0, 1, 1, 0
-    while b != 0:
-        quotient = a // b
-        a, b = b, a % b
-        x_prev, x = x - quotient * x_prev, x_prev
-        y_prev, y = y - quotient * y_prev, y_prev
-    return x, y, a
-
-
-def eulers_totient(n: int) -> int:
-    if n <= 0:
-        return 0
-    count = 0
-    for i in range(1, n + 1):
-        if is_coprime(n, i):
-            count += 1
-    return count
-
-
-def eulers_criterion(a: int, p: int):
-    return mod_exp(a, (p - 1) // 2, p) == 1
-
-
-def is_coprime(a: int, b: int) -> bool:
-    return gcd(a, b) == 1
-
-
-def fast_exp(a: int, b: int) -> int:
-    res = 1
-    while b > 0:
-        if b % 2 == 1:
-            res *= a
-        a *= a
-        b //= 2
-    return res
-
-
-def mod_exp(a: int, b: int, m: int) -> int:
-    res = 1
-    a %= m
-    while b > 0:
-        if b & 1:
-            res = (res * a) % m
-        b >>= 1
-        a = (a * a) % m
-    return res
+from common_functions import gcd, mod_exp
+import random
+
+def brute_force_factorization(n: int) -> list[int]:
+    factors = {}
+    divisor = 2
+
+    while n > 1:
+        while n % divisor == 0:
+            if divisor not in factors:
+                factors[divisor] = 1
+            else:
+                factors[divisor] += 1
+            n //= divisor
+        divisor += 1
+    
+    return factors
+
+
+def fermat_factorization(n: int) -> tuple[int, int]:
+    a = int(n ** 0.5) + 1
+    b2 = a * a - n
+    while not int(b2 ** 0.5) ** 2 == b2:
+        a += 1
+        b2 = a * a - n
+    b = int(b2 ** 0.5)
+    p = a + b
+    q = a - b
+    return p, q
+
+
+def pollards_p_minus_one_factorization(n: int, b: int) -> tuple[int, int]:
+    a = 2
+    for j in range(2, b + 1):
+        a = mod_exp(a, j, n)
+    p = gcd(a - 1, n)
+    return p, n // p
+
+def pollards_rho_factorization(n: int) -> int:
+    if n == 1:
+        return n
+    if n % 2 == 0:
+        return 2
+    
+    x = (random.randint(0, 2) % (n - 2))
+    y = x
+    c = (random.randint(0, 1) % (n - 1))
+    d = 1
+ 
+    while (d == 1):
+        x = (mod_exp(x, 2, n) + c + n) % n
+        y = (mod_exp(y, 2, n) + c + n) % n
+        y = (mod_exp(y, 2, n) + c + n) % n
+ 
+        d = gcd(abs(x - y), n)
+        if (d == n):
+            return pollards_rho_factorization(n)
+     
+    return d
```

### Comparing `numbertheory-0.0.3/numbertheory/fibonacci.py` & `numbertheory-0.0.4/numbertheory/fibonacci.py`

 * *Files identical despite different names*

### Comparing `numbertheory-0.0.3/numbertheory/generating_primes.py` & `numbertheory-0.0.4/numbertheory/generating_primes.py`

 * *Files identical despite different names*

### Comparing `numbertheory-0.0.3/numbertheory/modulus_operations.py` & `numbertheory-0.0.4/numbertheory/modulus_operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from common_functions import extended_euclidean
+from common_functions import extended_euclidean, mod_exp
 
 
 def mod_inverse(a: int, m: int) -> int:
     x, _, gcd = extended_euclidean(a, m)
     if gcd != 1:
         raise ValueError("The modular inverse does not exist.")
     return x % m if x >= 0 else x + m
@@ -12,8 +12,14 @@
     sum = 0
     prod = 1
     for n_i in moduli:
         prod *= n_i
     for n_i, a_i in zip(moduli, remainders):
         p = prod // n_i
         sum += a_i * mod_inverse(p, n_i) * p
-    return sum % prod
+    return sum % prod
+
+def order_of_number(a: int, m: int) -> int:
+    for i in range(1, m):
+        if mod_exp(a, i, m) == 1:
+            return i
+    return m - 1
```

### Comparing `numbertheory-0.0.3/numbertheory/primality_tests.py` & `numbertheory-0.0.4/numbertheory/primality_tests.py`

 * *Files identical despite different names*

### Comparing `numbertheory-0.0.3/setup.py` & `numbertheory-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('../README.md', 'r') as readme:
     long_descripton = readme.read()
     
 setup(
     name='numbertheory',
-    version='0.0.3',
+    version='0.0.4',
     description='Common number theoretic functions.',
     long_description_content_type='text/markdown',
     long_description=long_descripton,
     packages=find_packages(),
     license='MIT',
     url='https://0xkilty.github.io/number-theory/',
     author='0xKilty',
```

