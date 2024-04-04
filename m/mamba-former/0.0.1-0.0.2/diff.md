# Comparing `tmp/mamba_former-0.0.1.tar.gz` & `tmp/mamba_former-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mamba_former-0.0.1.tar", max compression
+gzip compressed data, was "mamba_former-0.0.2.tar", max compression
```

## Comparing `mamba_former-0.0.1.tar` & `mamba_former-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-04-04 00:00:17.570890 mamba_former-0.0.1/LICENSE
--rw-r--r--   0        0        0      692 2024-04-04 00:27:33.859935 mamba_former-0.0.1/README.md
--rw-r--r--   0        0        0       74 2024-04-04 00:27:44.557905 mamba_former-0.0.1/mamba_former/__init__.py
--rw-r--r--   0        0        0     3067 2024-04-04 00:26:46.917210 mamba_former-0.0.1/mamba_former/main.py
--rw-r--r--   0        0        0     1365 2024-04-04 00:26:41.154615 mamba_former-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1384 1970-01-01 00:00:00.000000 mamba_former-0.0.1/setup.py
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 mamba_former-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-04 00:00:17.570890 mamba_former-0.0.2/LICENSE
+-rw-r--r--   0        0        0      692 2024-04-04 00:27:33.859935 mamba_former-0.0.2/README.md
+-rw-r--r--   0        0        0       74 2024-04-04 00:27:44.557905 mamba_former-0.0.2/mamba_former/__init__.py
+-rw-r--r--   0        0        0     3067 2024-04-04 00:26:46.917210 mamba_former-0.0.2/mamba_former/main.py
+-rw-r--r--   0        0        0     1356 2024-04-04 00:40:29.629889 mamba_former-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 mamba_former-0.0.2/setup.py
+-rw-r--r--   0        0        0     1699 1970-01-01 00:00:00.000000 mamba_former-0.0.2/PKG-INFO
```

### Comparing `mamba_former-0.0.1/LICENSE` & `mamba_former-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mamba_former-0.0.1/README.md` & `mamba_former-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `mamba_former-0.0.1/mamba_former/main.py` & `mamba_former-0.0.2/mamba_former/main.py`

 * *Files identical despite different names*

### Comparing `mamba_former-0.0.1/pyproject.toml` & `mamba_former-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mamba-former"
-version = "0.0.1"
+version = "0.0.2"
 description = "Paper - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/MambaFormer"
 documentation = "https://github.com/kyegomez/MambaFormer"  # Add this if you have documentation.
 readme = "README.md"  # Assuming you have a README.md
 repository = "https://github.com/kyegomez/MambaFormer"
@@ -18,17 +18,16 @@
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
-swarms = "*"
-zetascale = "*"
+python = "^3.9"
+zetascale = "2.2.7"
 einops = "*"
 torch = "*"
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.6"
 types-toml = "^0.10.8.1"
 types-redis = "^4.3.21.6"
```

### Comparing `mamba_former-0.0.1/setup.py` & `mamba_former-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['mamba_former']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['einops', 'swarms', 'torch', 'zetascale']
+['einops', 'torch', 'zetascale==2.2.7']
 
 setup_kwargs = {
     'name': 'mamba-former',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': 'Paper - Pytorch',
     'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# MambaFormer\nImplementation of MambaFormer in Pytorch ++ Zeta from the paper: "Can Mamba Learn How to Learn? A Comparative Study on In-Context Learning Tasks"\n\n## install\n`pip3 install mamba-former`\n\n## usage\n```python\nimport torch \nfrom mamba_former.main import MambaFormer\n\n# Forward pass example\nx = torch.randint(1, 1000, (1, 100)) # Token\n# Tokens are integrers\n\n# Model\nmodel = MambaFormer(\n    dim = 512,\n    num_tokens = 1000,\n    depth = 6,\n    d_state = 512,\n    d_conv = 128,\n    heads = 8,\n    dim_head = 64,\n    return_tokens = True\n)\n\n# Forward\nout = model(x)\nprint(out)\nprint(out.shape)\n```\n\n\n# License\nMIT\n',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/MambaFormer',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
+    'python_requires': '>=3.9,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `mamba_former-0.0.1/PKG-INFO` & `mamba_former-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 Metadata-Version: 2.1
 Name: mamba-former
-Version: 0.0.1
+Version: 0.0.2
 Summary: Paper - Pytorch
 Home-page: https://github.com/kyegomez/MambaFormer
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Author: Kye Gomez
 Author-email: kye@apac.ai
-Requires-Python: >=3.6,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
-Requires-Dist: swarms
 Requires-Dist: torch
-Requires-Dist: zetascale
+Requires-Dist: zetascale (==2.2.7)
 Project-URL: Documentation, https://github.com/kyegomez/MambaFormer
 Project-URL: Repository, https://github.com/kyegomez/MambaFormer
 Description-Content-Type: text/markdown
 
 [![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)
 
 # MambaFormer
```

