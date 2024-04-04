# Comparing `tmp/pminit-0.3.0.tar.gz` & `tmp/pminit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pminit-0.3.0.tar", max compression
+gzip compressed data, was "pminit-0.4.0.tar", max compression
```

## Comparing `pminit-0.3.0.tar` & `pminit-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       57 2024-01-25 22:32:54.431142 pminit-0.3.0/pminit/__init__.py
--rw-r--r--   0        0        0     1216 2024-01-25 22:32:54.431142 pminit-0.3.0/pminit/cli.py
--rw-r--r--   0        0        0     1231 2024-01-25 22:32:54.431142 pminit-0.3.0/post-install-hook.py
--rw-r--r--   0        0        0     1043 2024-01-25 22:35:02.228428 pminit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    17781 2024-01-25 22:32:54.446750 pminit-0.3.0/pythonmonkey/package-lock.json
--rw-r--r--   0        0        0      706 2024-01-25 22:32:54.446750 pminit-0.3.0/pythonmonkey/package.json
--rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2024-04-04 20:50:40.973190 pminit-0.4.0/pminit/__init__.py
+-rw-r--r--   0        0        0     1176 2024-04-04 20:50:40.973304 pminit-0.4.0/pminit/cli.py
+-rw-r--r--   0        0        0     1192 2024-04-04 20:50:40.974188 pminit-0.4.0/post-install-hook.py
+-rw-r--r--   0        0        0     1005 2024-04-04 20:51:24.489678 pminit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    19961 2024-04-04 20:50:40.974439 pminit-0.4.0/pythonmonkey/package-lock.json
+-rw-r--r--   0        0        0      679 2024-04-04 20:50:40.974539 pminit-0.4.0/pythonmonkey/package.json
+-rw-r--r--   0        0        0      431 1970-01-01 00:00:00.000000 pminit-0.4.0/PKG-INFO
```

### Comparing `pminit-0.3.0/post-install-hook.py` & `pminit-0.4.0/post-install-hook.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import subprocess
-import sys
-import shutil
-
-def execute(cmd: str):
-    popen = subprocess.Popen(cmd, stdout = subprocess.PIPE, stderr = subprocess.STDOUT,
-        shell = True, text = True )
-    for stdout_line in iter(popen.stdout.readline, ""):
-        sys.stdout.write(stdout_line)
-        sys.stdout.flush()
-
-    popen.stdout.close()
-    return_code = popen.wait()
-    if return_code:
-        raise subprocess.CalledProcessError(return_code, cmd)
-
-def main():
-    node_package_manager = 'npm'
-    # check if npm is installed on the system
-    if (shutil.which(node_package_manager) is None):
-        print("""
-
-PythonMonkey Build Error:
-
-    
-  *    It appears npm is not installed on this system.
-  *    npm is required for PythonMonkey to build.
-  *    Please install NPM and Node.js before installing PythonMonkey.
-  *    Refer to the documentation for installing NPM and Node.js here: https://nodejs.org/en/download
-
-
-        """)
-        raise Exception("PythonMonkey build error: Unable to find npm on the system.")
-    else:
-        execute(f"cd pythonmonkey && {node_package_manager} i --no-package-lock") # do not update package-lock.json
-
-if __name__ == "__main__":
-    main()
-
+import subprocess
+import sys
+import shutil
+
+def execute(cmd: str):
+    popen = subprocess.Popen(cmd, stdout = subprocess.PIPE, stderr = subprocess.STDOUT,
+        shell = True, text = True )
+    for stdout_line in iter(popen.stdout.readline, ""):
+        sys.stdout.write(stdout_line)
+        sys.stdout.flush()
+
+    popen.stdout.close()
+    return_code = popen.wait()
+    if return_code:
+        raise subprocess.CalledProcessError(return_code, cmd)
+
+def main():
+    node_package_manager = 'npm'
+    # check if npm is installed on the system
+    if (shutil.which(node_package_manager) is None):
+        print("""
+
+PythonMonkey Build Error:
+
+    
+  *    It appears npm is not installed on this system.
+  *    npm is required for PythonMonkey to build.
+  *    Please install NPM and Node.js before installing PythonMonkey.
+  *    Refer to the documentation for installing NPM and Node.js here: https://nodejs.org/en/download
+
+
+        """)
+        raise Exception("PythonMonkey build error: Unable to find npm on the system.")
+    else:
+        execute(f"cd pythonmonkey && {node_package_manager} i --no-package-lock") # do not update package-lock.json
+
+if __name__ == "__main__":
+    main()
+
```

### Comparing `pminit-0.3.0/pyproject.toml` & `pminit-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-[tool.poetry]
-name = "pminit"
-version = "0.3.0"
-description = "Post-install hook for PythonMonkey"
-authors = [
-  "Tom Tang <xmader@distributive.network>",
-  "Caleb Aikens <caleb@distributive.network>",
-  "Wes Garland <wes@distributive.network>",
-  "Hamada Gasmallah <hamada@distributive.network>"
-]
-include = [
-  # Install extra files into the pythonmonkey package
-  "pythonmonkey/package*.json",
-  { path = "pythonmonkey/node_modules/**/*", format = "wheel" },
-  # pip builds (and actually installs from) the wheel when installing from sdist
-  # we don't want node_modules inside the sdist package
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-
-[tool.poetry-dynamic-versioning]
-enable = false
-vcs = "git"
-style = "pep440"
-bump = true
-
-[tool.poetry.build]
-script = "post-install-hook.py"
-generate-setup-file = false
-
-[tool.poetry.scripts]
-pminit = "pminit.cli:main"
-
-[build-system]
-requires = ["poetry-core>=1.1.1", "poetry-dynamic-versioning==1.1.1"]
-build-backend = "poetry_dynamic_versioning.backend"
-
+[tool.poetry]
+name = "pminit"
+version = "0.4.0"
+description = "Post-install hook for PythonMonkey"
+authors = [
+  "Tom Tang <xmader@distributive.network>",
+  "Caleb Aikens <caleb@distributive.network>",
+  "Wes Garland <wes@distributive.network>",
+  "Hamada Gasmallah <hamada@distributive.network>"
+]
+include = [
+  # Install extra files into the pythonmonkey package
+  "pythonmonkey/package*.json",
+  { path = "pythonmonkey/node_modules/**/*", format = "wheel" },
+  # pip builds (and actually installs from) the wheel when installing from sdist
+  # we don't want node_modules inside the sdist package
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+
+[tool.poetry-dynamic-versioning]
+enable = false
+vcs = "git"
+style = "pep440"
+bump = true
+
+[tool.poetry.build]
+script = "post-install-hook.py"
+generate-setup-file = false
+
+[tool.poetry.scripts]
+pminit = "pminit.cli:main"
+
+[build-system]
+requires = ["poetry-core>=1.1.1", "poetry-dynamic-versioning==1.1.1"]
+build-backend = "poetry_dynamic_versioning.backend"
+
```

### Comparing `pminit-0.3.0/pythonmonkey/package-lock.json` & `pminit-0.4.0/pythonmonkey/package-lock.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5833333333333334%*

 * *Differences: {"'lockfileVersion'": '3',*

 * * "'packages'": "OrderedDict([('', OrderedDict([('name', 'pythonmonkey'), ('version', '0.0.1'), "*

 * *               "('license', 'MIT'), ('dependencies', OrderedDict([('core-js', '^3.35.1'), "*

 * *               "('ctx-module', '^1.0.14')]))])), ('node_modules/asn1.js', OrderedDict([('version', "*

 * *               "'5.4.1'), ('resolved', 'https://registry.npmjs.org/asn1.js/-/asn1.js-5.4.1.tgz'), "*

 * *               "('integrity', "*

 * *               "'sha512-+I//4cYPccV8LdmBLiX8CYvf9Sp3vQsrqu2QNXR […]*

```diff
@@ -1,439 +1,518 @@
 {
-    "dependencies": {
-        "asn1.js": {
+    "lockfileVersion": 3,
+    "name": "pythonmonkey",
+    "packages": {
+        "": {
             "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
+                "core-js": "^3.35.1",
+                "ctx-module": "^1.0.14"
             },
-            "integrity": "sha512-+I//4cYPccV8LdmBLiX8CYvf9Sp3vQsrqu2QNXRcrbiWvcx/UdlFiqUJJzxRQxgsZmvhXhn4cSKeSmoFjVdupA==",
-            "requires": {
+            "license": "MIT",
+            "name": "pythonmonkey",
+            "version": "0.0.1"
+        },
+        "node_modules/asn1.js": {
+            "dependencies": {
                 "bn.js": "^4.0.0",
                 "inherits": "^2.0.1",
                 "minimalistic-assert": "^1.0.0",
                 "safer-buffer": "^2.1.0"
             },
+            "integrity": "sha512-+I//4cYPccV8LdmBLiX8CYvf9Sp3vQsrqu2QNXRcrbiWvcx/UdlFiqUJJzxRQxgsZmvhXhn4cSKeSmoFjVdupA==",
             "resolved": "https://registry.npmjs.org/asn1.js/-/asn1.js-5.4.1.tgz",
             "version": "5.4.1"
         },
-        "base64-js": {
+        "node_modules/asn1.js/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/base64-js": {
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
             "integrity": "sha512-AKpaYlHn8t4SVbOHCy+b5+KKgvR4vrsD8vbvrbiQJps7fKDTkjkDry6ji0rUJjC0kzbNePLwzxq8iypo41qeWA==",
             "resolved": "https://registry.npmjs.org/base64-js/-/base64-js-1.5.1.tgz",
             "version": "1.5.1"
         },
-        "bn.js": {
+        "node_modules/bn.js": {
             "integrity": "sha512-eXRvHzWyYPBuB4NBy0cmYQjGitUrtqwbvlzP3G6VFnNRbsZQIxQ10PbKKHt8gZ/HW/D/747aDl+QkDqg3KQLMQ==",
             "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-5.2.1.tgz",
             "version": "5.2.1"
         },
-        "brorand": {
+        "node_modules/brorand": {
             "integrity": "sha512-cKV8tMCEpQs4hK/ik71d6LrPOnpkpGBR0wzxqr68g2m/LB2GxVYQroAjMJZRVM1Y4BCjCKc3vAamxSzOY2RP+w==",
             "resolved": "https://registry.npmjs.org/brorand/-/brorand-1.1.0.tgz",
             "version": "1.1.0"
         },
-        "browserify-aes": {
-            "integrity": "sha512-+7CHXqGuspUn/Sl5aO7Ea0xWGAtETPXNSAjHo48JfLdPWcMng33Xe4znFvQweqc/uzk5zSOI3H52CYnjCfb5hA==",
-            "requires": {
+        "node_modules/browserify-aes": {
+            "dependencies": {
                 "buffer-xor": "^1.0.3",
                 "cipher-base": "^1.0.0",
                 "create-hash": "^1.1.0",
                 "evp_bytestokey": "^1.0.3",
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
             },
+            "integrity": "sha512-+7CHXqGuspUn/Sl5aO7Ea0xWGAtETPXNSAjHo48JfLdPWcMng33Xe4znFvQweqc/uzk5zSOI3H52CYnjCfb5hA==",
             "resolved": "https://registry.npmjs.org/browserify-aes/-/browserify-aes-1.2.0.tgz",
             "version": "1.2.0"
         },
-        "browserify-cipher": {
-            "integrity": "sha512-sPhkz0ARKbf4rRQt2hTpAHqn47X3llLkUGn+xEJzLjwY8LRs2p0v7ljvI5EyoRO/mexrNunNECisZs+gw2zz1w==",
-            "requires": {
+        "node_modules/browserify-cipher": {
+            "dependencies": {
                 "browserify-aes": "^1.0.4",
                 "browserify-des": "^1.0.0",
                 "evp_bytestokey": "^1.0.0"
             },
+            "integrity": "sha512-sPhkz0ARKbf4rRQt2hTpAHqn47X3llLkUGn+xEJzLjwY8LRs2p0v7ljvI5EyoRO/mexrNunNECisZs+gw2zz1w==",
             "resolved": "https://registry.npmjs.org/browserify-cipher/-/browserify-cipher-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "browserify-des": {
-            "integrity": "sha512-BioO1xf3hFwz4kc6iBhI3ieDFompMhrMlnDFC4/0/vd5MokpuAc3R+LYbwTA9A5Yc9pq9UYPqffKpW2ObuwX5A==",
-            "requires": {
+        "node_modules/browserify-des": {
+            "dependencies": {
                 "cipher-base": "^1.0.1",
                 "des.js": "^1.0.0",
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.1.2"
             },
+            "integrity": "sha512-BioO1xf3hFwz4kc6iBhI3ieDFompMhrMlnDFC4/0/vd5MokpuAc3R+LYbwTA9A5Yc9pq9UYPqffKpW2ObuwX5A==",
             "resolved": "https://registry.npmjs.org/browserify-des/-/browserify-des-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "browserify-rsa": {
-            "integrity": "sha512-AdEER0Hkspgno2aR97SAf6vi0y0k8NuOpGnVH3O99rcA5Q6sh8QxcngtHuJ6uXwnfAXNM4Gn1Gb7/MV1+Ymbog==",
-            "requires": {
+        "node_modules/browserify-rsa": {
+            "dependencies": {
                 "bn.js": "^5.0.0",
                 "randombytes": "^2.0.1"
             },
+            "integrity": "sha512-AdEER0Hkspgno2aR97SAf6vi0y0k8NuOpGnVH3O99rcA5Q6sh8QxcngtHuJ6uXwnfAXNM4Gn1Gb7/MV1+Ymbog==",
             "resolved": "https://registry.npmjs.org/browserify-rsa/-/browserify-rsa-4.1.0.tgz",
             "version": "4.1.0"
         },
-        "browserify-sign": {
-            "integrity": "sha512-/vrA5fguVAKKAVTNJjgSm1tRQDHUU6DbwO9IROu/0WAzC8PKhucDSh18J0RMvVeHAn5puMd+QHC2erPRNf8lmg==",
-            "requires": {
-                "bn.js": "^5.1.1",
-                "browserify-rsa": "^4.0.1",
+        "node_modules/browserify-sign": {
+            "dependencies": {
+                "bn.js": "^5.2.1",
+                "browserify-rsa": "^4.1.0",
                 "create-hash": "^1.2.0",
                 "create-hmac": "^1.1.7",
-                "elliptic": "^6.5.3",
+                "elliptic": "^6.5.4",
                 "inherits": "^2.0.4",
-                "parse-asn1": "^5.1.5",
-                "readable-stream": "^3.6.0",
-                "safe-buffer": "^5.2.0"
-            },
-            "resolved": "https://registry.npmjs.org/browserify-sign/-/browserify-sign-4.2.1.tgz",
-            "version": "4.2.1"
+                "parse-asn1": "^5.1.6",
+                "readable-stream": "^3.6.2",
+                "safe-buffer": "^5.2.1"
+            },
+            "engines": {
+                "node": ">= 4"
+            },
+            "integrity": "sha512-1rudGyeYY42Dk6texmv7c4VcQ0EsvVbLwZkA+AQB7SxvXxmcD93jcHie8bzecJ+ChDlmAm2Qyu0+Ccg5uhZXCg==",
+            "resolved": "https://registry.npmjs.org/browserify-sign/-/browserify-sign-4.2.2.tgz",
+            "version": "4.2.2"
         },
-        "buffer": {
-            "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
-            "requires": {
+        "node_modules/buffer": {
+            "dependencies": {
                 "base64-js": "^1.3.1",
                 "ieee754": "^1.2.1"
             },
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
+            "integrity": "sha512-FTiCpNxtwiZZHEZbcbTIcZjERVICn9yq/pDFkTl95/AxzD1naBctN7YO68riM/gLSDY7sdrMby8hofADYuuqOA==",
             "resolved": "https://registry.npmjs.org/buffer/-/buffer-6.0.3.tgz",
             "version": "6.0.3"
         },
-        "buffer-xor": {
+        "node_modules/buffer-xor": {
             "integrity": "sha512-571s0T7nZWK6vB67HI5dyUF7wXiNcfaPPPTl6zYCNApANjIvYJTg7hlud/+cJpdAhS7dVzqMLmfhfHR3rAcOjQ==",
             "resolved": "https://registry.npmjs.org/buffer-xor/-/buffer-xor-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "cipher-base": {
-            "integrity": "sha512-Kkht5ye6ZGmwv40uUDZztayT2ThLQGfnj/T71N/XzeZeo3nf8foyW7zGTsPYkEya3m5f3cAypH+qe7YOrM1U2Q==",
-            "requires": {
+        "node_modules/cipher-base": {
+            "dependencies": {
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
             },
+            "integrity": "sha512-Kkht5ye6ZGmwv40uUDZztayT2ThLQGfnj/T71N/XzeZeo3nf8foyW7zGTsPYkEya3m5f3cAypH+qe7YOrM1U2Q==",
             "resolved": "https://registry.npmjs.org/cipher-base/-/cipher-base-1.0.4.tgz",
             "version": "1.0.4"
         },
-        "core-js": {
-            "integrity": "sha512-rd4rYZNlF3WuoYuRIDEmbR/ga9CeuWX9U05umAvgrrZoHY4Z++cp/xwPQMvUpBB4Ag6J8KfD80G0zwCyaSxDww==",
-            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.32.0.tgz",
-            "version": "3.32.0"
-        },
-        "create-ecdh": {
-            "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
-            },
-            "integrity": "sha512-mf+TCx8wWc9VpuxfP2ht0iSISLZnt0JgWlrOKZiNqyUZWnjIaCIVNQArMHnCZKfEYRg6IM7A+NeJoN8gf/Ws0A==",
-            "requires": {
+        "node_modules/core-js": {
+            "funding": {
+                "type": "opencollective",
+                "url": "https://opencollective.com/core-js"
+            },
+            "hasInstallScript": true,
+            "integrity": "sha512-IgdsbxNyMskrTFxa9lWHyMwAJU5gXOPP+1yO+K59d50VLVAIDAbs7gIv705KzALModfK3ZrSZTPNpC0PQgIZuw==",
+            "resolved": "https://registry.npmjs.org/core-js/-/core-js-3.35.1.tgz",
+            "version": "3.35.1"
+        },
+        "node_modules/create-ecdh": {
+            "dependencies": {
                 "bn.js": "^4.1.0",
                 "elliptic": "^6.5.3"
             },
+            "integrity": "sha512-mf+TCx8wWc9VpuxfP2ht0iSISLZnt0JgWlrOKZiNqyUZWnjIaCIVNQArMHnCZKfEYRg6IM7A+NeJoN8gf/Ws0A==",
             "resolved": "https://registry.npmjs.org/create-ecdh/-/create-ecdh-4.0.4.tgz",
             "version": "4.0.4"
         },
-        "create-hash": {
-            "integrity": "sha512-z00bCGNHDG8mHAkP7CtT1qVu+bFQUPjYq/4Iv3C3kWjTFV10zIjfSoeqXo9Asws8gwSHDGj/hl2u4OGIjapeCg==",
-            "requires": {
+        "node_modules/create-ecdh/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/create-hash": {
+            "dependencies": {
                 "cipher-base": "^1.0.1",
                 "inherits": "^2.0.1",
                 "md5.js": "^1.3.4",
                 "ripemd160": "^2.0.1",
                 "sha.js": "^2.4.0"
             },
+            "integrity": "sha512-z00bCGNHDG8mHAkP7CtT1qVu+bFQUPjYq/4Iv3C3kWjTFV10zIjfSoeqXo9Asws8gwSHDGj/hl2u4OGIjapeCg==",
             "resolved": "https://registry.npmjs.org/create-hash/-/create-hash-1.2.0.tgz",
             "version": "1.2.0"
         },
-        "create-hmac": {
-            "integrity": "sha512-MJG9liiZ+ogc4TzUwuvbER1JRdgvUFSB5+VR/g5h82fGaIRWMWddtKBHi7/sVhfjQZ6SehlyhvQYrcYkaUIpLg==",
-            "requires": {
+        "node_modules/create-hmac": {
+            "dependencies": {
                 "cipher-base": "^1.0.3",
                 "create-hash": "^1.1.0",
                 "inherits": "^2.0.1",
                 "ripemd160": "^2.0.0",
                 "safe-buffer": "^5.0.1",
                 "sha.js": "^2.4.8"
             },
+            "integrity": "sha512-MJG9liiZ+ogc4TzUwuvbER1JRdgvUFSB5+VR/g5h82fGaIRWMWddtKBHi7/sVhfjQZ6SehlyhvQYrcYkaUIpLg==",
             "resolved": "https://registry.npmjs.org/create-hmac/-/create-hmac-1.1.7.tgz",
             "version": "1.1.7"
         },
-        "crypto-browserify": {
-            "integrity": "sha512-fz4spIh+znjO2VjL+IdhEpRJ3YN6sMzITSBijk6FK2UvTqruSQW+/cCZTSNsMiZNvUeq0CqurF+dAbyiGOY6Wg==",
-            "requires": {
+        "node_modules/crypto-browserify": {
+            "dependencies": {
                 "browserify-cipher": "^1.0.0",
                 "browserify-sign": "^4.0.0",
                 "create-ecdh": "^4.0.0",
                 "create-hash": "^1.1.0",
                 "create-hmac": "^1.1.0",
                 "diffie-hellman": "^5.0.0",
                 "inherits": "^2.0.1",
                 "pbkdf2": "^3.0.3",
                 "public-encrypt": "^4.0.0",
                 "randombytes": "^2.0.0",
                 "randomfill": "^1.0.3"
             },
+            "engines": {
+                "node": "*"
+            },
+            "integrity": "sha512-fz4spIh+znjO2VjL+IdhEpRJ3YN6sMzITSBijk6FK2UvTqruSQW+/cCZTSNsMiZNvUeq0CqurF+dAbyiGOY6Wg==",
             "resolved": "https://registry.npmjs.org/crypto-browserify/-/crypto-browserify-3.12.0.tgz",
             "version": "3.12.0"
         },
-        "ctx-module": {
-            "integrity": "sha512-eH4h/bv64YuzCHMUZs93j57/4zNJHyQWOIz5CPAs1gJ/4yznPD9HoCLCXjQlST2AxOLOKNvV67n+A8dALtLA+Q==",
-            "requires": {
+        "node_modules/ctx-module": {
+            "dependencies": {
                 "buffer": "^6.0.3",
                 "crypto-browserify": "^3.12.0"
             },
+            "integrity": "sha512-eH4h/bv64YuzCHMUZs93j57/4zNJHyQWOIz5CPAs1gJ/4yznPD9HoCLCXjQlST2AxOLOKNvV67n+A8dALtLA+Q==",
             "resolved": "https://registry.npmjs.org/ctx-module/-/ctx-module-1.0.14.tgz",
             "version": "1.0.14"
         },
-        "des.js": {
-            "integrity": "sha512-r17GxjhUCjSRy8aiJpr8/UadFIzMzJGexI3Nmz4ADi9LYSFx4gTBp80+NaX/YsXWWLhpZ7v/v/ubEc/bCNfKwg==",
-            "requires": {
+        "node_modules/des.js": {
+            "dependencies": {
                 "inherits": "^2.0.1",
                 "minimalistic-assert": "^1.0.0"
             },
+            "integrity": "sha512-r17GxjhUCjSRy8aiJpr8/UadFIzMzJGexI3Nmz4ADi9LYSFx4gTBp80+NaX/YsXWWLhpZ7v/v/ubEc/bCNfKwg==",
             "resolved": "https://registry.npmjs.org/des.js/-/des.js-1.1.0.tgz",
             "version": "1.1.0"
         },
-        "diffie-hellman": {
+        "node_modules/diffie-hellman": {
             "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
-            },
-            "integrity": "sha512-kqag/Nl+f3GwyK25fhUMYj81BUOrZ9IuJsjIcDE5icNM9FJHAVm3VcUDxdLPoQtTuUylWm6ZIknYJwwaPxsUzg==",
-            "requires": {
                 "bn.js": "^4.1.0",
                 "miller-rabin": "^4.0.0",
                 "randombytes": "^2.0.0"
             },
+            "integrity": "sha512-kqag/Nl+f3GwyK25fhUMYj81BUOrZ9IuJsjIcDE5icNM9FJHAVm3VcUDxdLPoQtTuUylWm6ZIknYJwwaPxsUzg==",
             "resolved": "https://registry.npmjs.org/diffie-hellman/-/diffie-hellman-5.0.3.tgz",
             "version": "5.0.3"
         },
-        "elliptic": {
+        "node_modules/diffie-hellman/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/elliptic": {
             "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
-            },
-            "integrity": "sha512-iLhC6ULemrljPZb+QutR5TQGB+pdW6KGD5RSegS+8sorOZT+rdQFbsQFJgvN3eRqNALqJer4oQ16YvJHlU8hzQ==",
-            "requires": {
                 "bn.js": "^4.11.9",
                 "brorand": "^1.1.0",
                 "hash.js": "^1.0.0",
                 "hmac-drbg": "^1.0.1",
                 "inherits": "^2.0.4",
                 "minimalistic-assert": "^1.0.1",
                 "minimalistic-crypto-utils": "^1.0.1"
             },
+            "integrity": "sha512-iLhC6ULemrljPZb+QutR5TQGB+pdW6KGD5RSegS+8sorOZT+rdQFbsQFJgvN3eRqNALqJer4oQ16YvJHlU8hzQ==",
             "resolved": "https://registry.npmjs.org/elliptic/-/elliptic-6.5.4.tgz",
             "version": "6.5.4"
         },
-        "evp_bytestokey": {
-            "integrity": "sha512-/f2Go4TognH/KvCISP7OUsHn85hT9nUkxxA9BEWxFn+Oj9o8ZNLm/40hdlgSLyuOimsrTKLUMEorQexp/aPQeA==",
-            "requires": {
+        "node_modules/elliptic/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/evp_bytestokey": {
+            "dependencies": {
                 "md5.js": "^1.3.4",
                 "safe-buffer": "^5.1.1"
             },
+            "integrity": "sha512-/f2Go4TognH/KvCISP7OUsHn85hT9nUkxxA9BEWxFn+Oj9o8ZNLm/40hdlgSLyuOimsrTKLUMEorQexp/aPQeA==",
             "resolved": "https://registry.npmjs.org/evp_bytestokey/-/evp_bytestokey-1.0.3.tgz",
             "version": "1.0.3"
         },
-        "hash-base": {
-            "integrity": "sha512-1nmYp/rhMDiE7AYkDw+lLwlAzz0AntGIe51F3RfFfEqyQ3feY2eI/NcwC6umIQVOASPMsWJLJScWKSSvzL9IVA==",
-            "requires": {
+        "node_modules/hash-base": {
+            "dependencies": {
                 "inherits": "^2.0.4",
                 "readable-stream": "^3.6.0",
                 "safe-buffer": "^5.2.0"
             },
+            "engines": {
+                "node": ">=4"
+            },
+            "integrity": "sha512-1nmYp/rhMDiE7AYkDw+lLwlAzz0AntGIe51F3RfFfEqyQ3feY2eI/NcwC6umIQVOASPMsWJLJScWKSSvzL9IVA==",
             "resolved": "https://registry.npmjs.org/hash-base/-/hash-base-3.1.0.tgz",
             "version": "3.1.0"
         },
-        "hash.js": {
-            "integrity": "sha512-taOaskGt4z4SOANNseOviYDvjEJinIkRgmp7LbKP2YTTmVxWBl87s/uzK9r+44BclBSp2X7K1hqeNfz9JbBeXA==",
-            "requires": {
+        "node_modules/hash.js": {
+            "dependencies": {
                 "inherits": "^2.0.3",
                 "minimalistic-assert": "^1.0.1"
             },
+            "integrity": "sha512-taOaskGt4z4SOANNseOviYDvjEJinIkRgmp7LbKP2YTTmVxWBl87s/uzK9r+44BclBSp2X7K1hqeNfz9JbBeXA==",
             "resolved": "https://registry.npmjs.org/hash.js/-/hash.js-1.1.7.tgz",
             "version": "1.1.7"
         },
-        "hmac-drbg": {
-            "integrity": "sha512-Tti3gMqLdZfhOQY1Mzf/AanLiqh1WTiJgEj26ZuYQ9fbkLomzGchCws4FyrSd4VkpBfiNhaE1On+lOz894jvXg==",
-            "requires": {
+        "node_modules/hmac-drbg": {
+            "dependencies": {
                 "hash.js": "^1.0.3",
                 "minimalistic-assert": "^1.0.0",
                 "minimalistic-crypto-utils": "^1.0.1"
             },
+            "integrity": "sha512-Tti3gMqLdZfhOQY1Mzf/AanLiqh1WTiJgEj26ZuYQ9fbkLomzGchCws4FyrSd4VkpBfiNhaE1On+lOz894jvXg==",
             "resolved": "https://registry.npmjs.org/hmac-drbg/-/hmac-drbg-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "ieee754": {
+        "node_modules/ieee754": {
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
             "integrity": "sha512-dcyqhDvX1C46lXZcVqCpK+FtMRQVdIMN6/Df5js2zouUsqG7I6sFxitIC+7KYK29KdXOLHdu9zL4sFnoVQnqaA==",
             "resolved": "https://registry.npmjs.org/ieee754/-/ieee754-1.2.1.tgz",
             "version": "1.2.1"
         },
-        "inherits": {
+        "node_modules/inherits": {
             "integrity": "sha512-k/vGaX4/Yla3WzyMCvTQOXYeIHvqOKtnqBduzTHpzpQZzAskKMhZ2K+EnBiSM9zGSoIFeMpXKxa4dYeZIQqewQ==",
             "resolved": "https://registry.npmjs.org/inherits/-/inherits-2.0.4.tgz",
             "version": "2.0.4"
         },
-        "md5.js": {
-            "integrity": "sha512-xitP+WxNPcTTOgnTJcrhM0xvdPepipPSf3I8EIpGKeFLjt3PlJLIDG3u8EX53ZIubkb+5U2+3rELYpEhHhzdkg==",
-            "requires": {
+        "node_modules/md5.js": {
+            "dependencies": {
                 "hash-base": "^3.0.0",
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.1.2"
             },
+            "integrity": "sha512-xitP+WxNPcTTOgnTJcrhM0xvdPepipPSf3I8EIpGKeFLjt3PlJLIDG3u8EX53ZIubkb+5U2+3rELYpEhHhzdkg==",
             "resolved": "https://registry.npmjs.org/md5.js/-/md5.js-1.3.5.tgz",
             "version": "1.3.5"
         },
-        "miller-rabin": {
-            "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
+        "node_modules/miller-rabin": {
+            "bin": {
+                "miller-rabin": "bin/miller-rabin"
             },
-            "integrity": "sha512-115fLhvZVqWwHPbClyntxEVfVDfl9DLLTuJvq3g2O/Oxi8AiNouAHvDSzHS0viUJc+V5vm3eq91Xwqn9dp4jRA==",
-            "requires": {
+            "dependencies": {
                 "bn.js": "^4.0.0",
                 "brorand": "^1.0.1"
             },
+            "integrity": "sha512-115fLhvZVqWwHPbClyntxEVfVDfl9DLLTuJvq3g2O/Oxi8AiNouAHvDSzHS0viUJc+V5vm3eq91Xwqn9dp4jRA==",
             "resolved": "https://registry.npmjs.org/miller-rabin/-/miller-rabin-4.0.1.tgz",
             "version": "4.0.1"
         },
-        "minimalistic-assert": {
+        "node_modules/miller-rabin/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/minimalistic-assert": {
             "integrity": "sha512-UtJcAD4yEaGtjPezWuO9wC4nwUnVH/8/Im3yEHQP4b67cXlD/Qr9hdITCU1xDbSEXg2XKNaP8jsReV7vQd00/A==",
             "resolved": "https://registry.npmjs.org/minimalistic-assert/-/minimalistic-assert-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "minimalistic-crypto-utils": {
+        "node_modules/minimalistic-crypto-utils": {
             "integrity": "sha512-JIYlbt6g8i5jKfJ3xz7rF0LXmv2TkDxBLUkiBeZ7bAx4GnnNMr8xFpGnOxn6GhTEHx3SjRrZEoU+j04prX1ktg==",
             "resolved": "https://registry.npmjs.org/minimalistic-crypto-utils/-/minimalistic-crypto-utils-1.0.1.tgz",
             "version": "1.0.1"
         },
-        "parse-asn1": {
-            "integrity": "sha512-RnZRo1EPU6JBnra2vGHj0yhp6ebyjBZpmUCLHWiFhxlzvBCCpAuZ7elsBp1PVAbQN0/04VD/19rfzlBSwLstMw==",
-            "requires": {
+        "node_modules/parse-asn1": {
+            "dependencies": {
                 "asn1.js": "^5.2.0",
                 "browserify-aes": "^1.0.0",
                 "evp_bytestokey": "^1.0.0",
                 "pbkdf2": "^3.0.3",
                 "safe-buffer": "^5.1.1"
             },
+            "integrity": "sha512-RnZRo1EPU6JBnra2vGHj0yhp6ebyjBZpmUCLHWiFhxlzvBCCpAuZ7elsBp1PVAbQN0/04VD/19rfzlBSwLstMw==",
             "resolved": "https://registry.npmjs.org/parse-asn1/-/parse-asn1-5.1.6.tgz",
             "version": "5.1.6"
         },
-        "pbkdf2": {
-            "integrity": "sha512-iuh7L6jA7JEGu2WxDwtQP1ddOpaJNC4KlDEFfdQajSGgGPNi4OyDc2R7QnbY2bR9QjBVGwgvTdNJZoE7RaxUMA==",
-            "requires": {
+        "node_modules/pbkdf2": {
+            "dependencies": {
                 "create-hash": "^1.1.2",
                 "create-hmac": "^1.1.4",
                 "ripemd160": "^2.0.1",
                 "safe-buffer": "^5.0.1",
                 "sha.js": "^2.4.8"
             },
+            "engines": {
+                "node": ">=0.12"
+            },
+            "integrity": "sha512-iuh7L6jA7JEGu2WxDwtQP1ddOpaJNC4KlDEFfdQajSGgGPNi4OyDc2R7QnbY2bR9QjBVGwgvTdNJZoE7RaxUMA==",
             "resolved": "https://registry.npmjs.org/pbkdf2/-/pbkdf2-3.1.2.tgz",
             "version": "3.1.2"
         },
-        "public-encrypt": {
+        "node_modules/public-encrypt": {
             "dependencies": {
-                "bn.js": {
-                    "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
-                    "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
-                    "version": "4.12.0"
-                }
-            },
-            "integrity": "sha512-zVpa8oKZSz5bTMTFClc1fQOnyyEzpl5ozpi1B5YcvBrdohMjH2rfsBtyXcuNuwjsDIXmBYlF2N5FlJYhR29t8Q==",
-            "requires": {
                 "bn.js": "^4.1.0",
                 "browserify-rsa": "^4.0.0",
                 "create-hash": "^1.1.0",
                 "parse-asn1": "^5.0.0",
                 "randombytes": "^2.0.1",
                 "safe-buffer": "^5.1.2"
             },
+            "integrity": "sha512-zVpa8oKZSz5bTMTFClc1fQOnyyEzpl5ozpi1B5YcvBrdohMjH2rfsBtyXcuNuwjsDIXmBYlF2N5FlJYhR29t8Q==",
             "resolved": "https://registry.npmjs.org/public-encrypt/-/public-encrypt-4.0.3.tgz",
             "version": "4.0.3"
         },
-        "randombytes": {
-            "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
-            "requires": {
+        "node_modules/public-encrypt/node_modules/bn.js": {
+            "integrity": "sha512-c98Bf3tPniI+scsdk237ku1Dc3ujXQTSgyiPUDEOe7tRkhrqridvh8klBv0HCEso1OLOYcHuCv/cS6DNxKH+ZA==",
+            "resolved": "https://registry.npmjs.org/bn.js/-/bn.js-4.12.0.tgz",
+            "version": "4.12.0"
+        },
+        "node_modules/randombytes": {
+            "dependencies": {
                 "safe-buffer": "^5.1.0"
             },
+            "integrity": "sha512-vYl3iOX+4CKUWuxGi9Ukhie6fsqXqS9FE2Zaic4tNFD2N2QQaXOMFbuKK4QmDHC0JO6B1Zp41J0LpT0oR68amQ==",
             "resolved": "https://registry.npmjs.org/randombytes/-/randombytes-2.1.0.tgz",
             "version": "2.1.0"
         },
-        "randomfill": {
-            "integrity": "sha512-87lcbR8+MhcWcUiQ+9e+Rwx8MyR2P7qnt15ynUlbm3TU/fjbgz4GsvfSUDTemtCCtVCqb4ZcEFlyPNTh9bBTLw==",
-            "requires": {
+        "node_modules/randomfill": {
+            "dependencies": {
                 "randombytes": "^2.0.5",
                 "safe-buffer": "^5.1.0"
             },
+            "integrity": "sha512-87lcbR8+MhcWcUiQ+9e+Rwx8MyR2P7qnt15ynUlbm3TU/fjbgz4GsvfSUDTemtCCtVCqb4ZcEFlyPNTh9bBTLw==",
             "resolved": "https://registry.npmjs.org/randomfill/-/randomfill-1.0.4.tgz",
             "version": "1.0.4"
         },
-        "readable-stream": {
-            "integrity": "sha512-9u/sniCrY3D5WdsERHzHE4G2YCXqoG5FTHUiCC4SIbr6XcLZBY05ya9EKjYek9O5xOAwjGq+1JdGBAS7Q9ScoA==",
-            "requires": {
+        "node_modules/readable-stream": {
+            "dependencies": {
                 "inherits": "^2.0.3",
                 "string_decoder": "^1.1.1",
                 "util-deprecate": "^1.0.1"
             },
+            "engines": {
+                "node": ">= 6"
+            },
+            "integrity": "sha512-9u/sniCrY3D5WdsERHzHE4G2YCXqoG5FTHUiCC4SIbr6XcLZBY05ya9EKjYek9O5xOAwjGq+1JdGBAS7Q9ScoA==",
             "resolved": "https://registry.npmjs.org/readable-stream/-/readable-stream-3.6.2.tgz",
             "version": "3.6.2"
         },
-        "ripemd160": {
-            "integrity": "sha512-ii4iagi25WusVoiC4B4lq7pbXfAp3D9v5CwfkY33vffw2+pkDjY1D8GaN7spsxvCSx8dkPqOZCEZyfxcmJG2IA==",
-            "requires": {
+        "node_modules/ripemd160": {
+            "dependencies": {
                 "hash-base": "^3.0.0",
                 "inherits": "^2.0.1"
             },
+            "integrity": "sha512-ii4iagi25WusVoiC4B4lq7pbXfAp3D9v5CwfkY33vffw2+pkDjY1D8GaN7spsxvCSx8dkPqOZCEZyfxcmJG2IA==",
             "resolved": "https://registry.npmjs.org/ripemd160/-/ripemd160-2.0.2.tgz",
             "version": "2.0.2"
         },
-        "safe-buffer": {
+        "node_modules/safe-buffer": {
+            "funding": [
+                {
+                    "type": "github",
+                    "url": "https://github.com/sponsors/feross"
+                },
+                {
+                    "type": "patreon",
+                    "url": "https://www.patreon.com/feross"
+                },
+                {
+                    "type": "consulting",
+                    "url": "https://feross.org/support"
+                }
+            ],
             "integrity": "sha512-rp3So07KcdmmKbGvgaNxQSJr7bGVSVk5S9Eq1F+ppbRo70+YeaDxkw5Dd8NPN+GD6bjnYm2VuPuCXmpuYvmCXQ==",
             "resolved": "https://registry.npmjs.org/safe-buffer/-/safe-buffer-5.2.1.tgz",
             "version": "5.2.1"
         },
-        "safer-buffer": {
+        "node_modules/safer-buffer": {
             "integrity": "sha512-YZo3K82SD7Riyi0E1EQPojLz7kpepnSQI9IyPbHHg1XXXevb5dJI7tpyN2ADxGcQbHG7vcyRHk0cbwqcQriUtg==",
             "resolved": "https://registry.npmjs.org/safer-buffer/-/safer-buffer-2.1.2.tgz",
             "version": "2.1.2"
         },
-        "sha.js": {
-            "integrity": "sha512-QMEp5B7cftE7APOjk5Y6xgrbWu+WkLVQwk8JNjZ8nKRciZaByEW6MubieAiToS7+dwvrjGhH8jRXz3MVd0AYqQ==",
-            "requires": {
+        "node_modules/sha.js": {
+            "bin": {
+                "sha.js": "bin.js"
+            },
+            "dependencies": {
                 "inherits": "^2.0.1",
                 "safe-buffer": "^5.0.1"
             },
+            "integrity": "sha512-QMEp5B7cftE7APOjk5Y6xgrbWu+WkLVQwk8JNjZ8nKRciZaByEW6MubieAiToS7+dwvrjGhH8jRXz3MVd0AYqQ==",
             "resolved": "https://registry.npmjs.org/sha.js/-/sha.js-2.4.11.tgz",
             "version": "2.4.11"
         },
-        "string_decoder": {
-            "integrity": "sha512-hkRX8U1WjJFd8LsDJ2yQ/wWWxaopEsABU1XfkM8A+j0+85JAGppt16cr1Whg6KIbb4okU6Mql6BOj+uup/wKeA==",
-            "requires": {
+        "node_modules/string_decoder": {
+            "dependencies": {
                 "safe-buffer": "~5.2.0"
             },
+            "integrity": "sha512-hkRX8U1WjJFd8LsDJ2yQ/wWWxaopEsABU1XfkM8A+j0+85JAGppt16cr1Whg6KIbb4okU6Mql6BOj+uup/wKeA==",
             "resolved": "https://registry.npmjs.org/string_decoder/-/string_decoder-1.3.0.tgz",
             "version": "1.3.0"
         },
-        "util-deprecate": {
+        "node_modules/util-deprecate": {
             "integrity": "sha512-EPD5q1uXyFxJpCrLnCc1nHnq3gOa6DZBocAIiI2TaSCA7VCJ1UJDMagCzIkXNsUYfD1daK//LTEQ8xiIbrHtcw==",
             "resolved": "https://registry.npmjs.org/util-deprecate/-/util-deprecate-1.0.2.tgz",
             "version": "1.0.2"
         }
     },
-    "lockfileVersion": 1,
-    "name": "pythonmonkey",
     "requires": true,
     "version": "0.0.1"
 }
```

