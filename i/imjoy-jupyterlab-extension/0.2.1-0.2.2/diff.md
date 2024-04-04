# Comparing `tmp/imjoy_jupyterlab_extension-0.2.1.tar.gz` & `tmp/imjoy_jupyterlab_extension-0.2.2.tar.gz`

## Comparing `imjoy_jupyterlab_extension-0.2.1.tar` & `imjoy_jupyterlab_extension-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/.copier-answers.yml
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/.prettierignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/.yarnrc.yml
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/RELEASE.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/Untitled.ipynb
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/babel.config.js
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/install.json
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/jest.config.js
--rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/setup.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/tsconfig.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/tsconfig.test.json
--rw-r--r--   0        0        0   389863 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/yarn.lock
--rw-r--r--   0        0        0  4893937 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/docs/Screenshot 2023-11-14 at 11.14.19.png
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/_version.py
--rw-r--r--   0        0        0    21004 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/build_log.json
--rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/package.json
--rw-r--r--   0        0        0    34010 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js
--rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js.map
--rw-r--r--   0        0        0    29101 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/remoteEntry.4ec6ba01760800a64c63.js
--rw-r--r--   0        0        0    27997 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/remoteEntry.4ec6ba01760800a64c63.js.map
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/style.js
--rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js
--rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js.map
--rw-r--r--   0        0        0   187964 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js
--rw-r--r--   0        0        0   265384 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js.map
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/scripts/publish.sh
--rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/src/comm-connection.js
--rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/src/imjoy-extension.js
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/src/index.ts
--rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/src/utils.js
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/src/__tests__/imjoy-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/style/index.js
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/README.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/playwright.config.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/yarn.lock
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/ui-tests/tests/imjoy-jupyterlab-extension.spec.ts
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/.gitignore
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/LICENSE
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/README.md
--rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/.copier-answers.yml
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/.prettierignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/.yarnrc.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/babel.config.js
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/install.json
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/jest.config.js
+-rw-r--r--   0        0        0     6598 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/setup.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/tsconfig.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/tsconfig.test.json
+-rw-r--r--   0        0        0   389863 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/yarn.lock
+-rw-r--r--   0        0        0  4893937 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/docs/Screenshot 2023-11-14 at 11.14.19.png
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0    21004 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/build_log.json
+-rw-r--r--   0        0        0     5846 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0    34010 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js
+-rw-r--r--   0        0        0    49473 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js.map
+-rw-r--r--   0        0        0    29101 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/remoteEntry.8f8e573811b7938685a1.js
+-rw-r--r--   0        0        0    27997 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/remoteEntry.8f8e573811b7938685a1.js.map
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0    19369 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js
+-rw-r--r--   0        0        0    14857 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js.map
+-rw-r--r--   0        0        0   187964 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js
+-rw-r--r--   0        0        0   265384 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js.map
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/scripts/publish.sh
+-rw-r--r--   0        0        0     7754 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/src/comm-connection.js
+-rw-r--r--   0        0        0    10177 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/src/imjoy-extension.js
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/src/index.ts
+-rw-r--r--   0        0        0     5995 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/src/utils.js
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/src/__tests__/imjoy-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/style/index.js
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/README.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/ui-tests/tests/imjoy-jupyterlab-extension.spec.ts
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/README.md
+-rw-r--r--   0        0        0     2478 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6074 2020-02-02 00:00:00.000000 imjoy_jupyterlab_extension-0.2.2/PKG-INFO
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/RELEASE.md` & `imjoy_jupyterlab_extension-0.2.2/RELEASE.md`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/jest.config.js` & `imjoy_jupyterlab_extension-0.2.2/jest.config.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/package.json` & `imjoy_jupyterlab_extension-0.2.2/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9735416666666667%*

 * *Differences: {"'jupyterlab'": "{'outputDir': 'imjoy_jupyterlab_extension/labextension'}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf imjoy_jupyterlab_extension/labextension "*

 * *              "imjoy_jupyterlab_extension/_version.py'}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -105,15 +105,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/imjoy-team/imjoy-jupyterlab-extension",
     "jupyterlab": {
         "extension": true,
-        "outputDir": "imjoy-jupyterlab-extension/labextension"
+        "outputDir": "imjoy_jupyterlab_extension/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -145,15 +145,15 @@
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf imjoy-jupyterlab-extension/labextension imjoy-jupyterlab-extension/_version.py",
+        "clean:labextension": "rimraf imjoy_jupyterlab_extension/labextension imjoy_jupyterlab_extension/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -187,9 +187,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/tsconfig.json` & `imjoy_jupyterlab_extension-0.2.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/yarn.lock` & `imjoy_jupyterlab_extension-0.2.2/yarn.lock`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/docs/Screenshot 2023-11-14 at 11.14.19.png` & `imjoy_jupyterlab_extension-0.2.2/docs/Screenshot 2023-11-14 at 11.14.19.png`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/__init__.py` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/__init__.py`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/build_log.json` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/build_log.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930548960641552%*

 * *Differences: {'0': "{'output': {'path': "*

 * *      "'/Users/wei.ouyang/workspace/imjoy-jupyterlab-extension/imjoy_jupyterlab_extension/labextension/static'}, "*

 * *      "'plugins': {1: {'_options': {'shared': {'imjoy-jupyterlab-extension': {'version': "*

 * *      "'0.2.2'}}}}}}"}*

```diff
@@ -88,15 +88,15 @@
                     ]
                 }
             ]
         },
         "output": {
             "filename": "[name].[contenthash].js",
             "hashFunction": "sha256",
-            "path": "/Users/wei.ouyang/workspace/imjoy-jupyterlab-extension/imjoy-jupyterlab-extension/labextension/static",
+            "path": "/Users/wei.ouyang/workspace/imjoy-jupyterlab-extension/imjoy_jupyterlab_extension/labextension/static",
             "publicPath": "auto"
         },
         "plugins": [
             {
                 "definitions": {
                     "process": "process/browser"
                 }
@@ -623,15 +623,15 @@
                             "requiredVersion": "^2.0.1",
                             "singleton": true
                         },
                         "imjoy-core": {},
                         "imjoy-jupyterlab-extension": {
                             "import": "/Users/wei.ouyang/workspace/imjoy-jupyterlab-extension/lib/index.js",
                             "singleton": true,
-                            "version": "0.2.1"
+                            "version": "0.2.2"
                         },
                         "react": {
                             "import": false,
                             "requiredVersion": "^18.2.0",
                             "singleton": true
                         },
                         "react-dom": {
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/package.json` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9746990740740742%*

 * *Differences: {"'jupyterlab'": "{'outputDir': 'imjoy_jupyterlab_extension/labextension', '_build': {'load': "*

 * *                 "'static/remoteEntry.8f8e573811b7938685a1.js'}}",*

 * * "'scripts'": "{'clean:labextension': 'rimraf imjoy_jupyterlab_extension/labextension "*

 * *              "imjoy_jupyterlab_extension/_version.py'}",*

 * * "'version'": "'0.2.2'"}*

```diff
@@ -106,19 +106,19 @@
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "src/**/*.{ts,tsx}"
     ],
     "homepage": "https://github.com/imjoy-team/imjoy-jupyterlab-extension",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4ec6ba01760800a64c63.js",
+            "load": "static/remoteEntry.8f8e573811b7938685a1.js",
             "style": "./style"
         },
         "extension": true,
-        "outputDir": "imjoy-jupyterlab-extension/labextension"
+        "outputDir": "imjoy_jupyterlab_extension/labextension"
     },
     "keywords": [
         "jupyter",
         "jupyterlab",
         "jupyterlab-extension"
     ],
     "license": "BSD-3-Clause",
@@ -150,15 +150,15 @@
         "build:labextension": "jupyter labextension build .",
         "build:labextension:dev": "jupyter labextension build --development True .",
         "build:lib": "tsc --sourceMap",
         "build:lib:prod": "tsc",
         "build:prod": "jlpm clean && jlpm build:lib:prod && jlpm build:labextension",
         "clean": "jlpm clean:lib",
         "clean:all": "jlpm clean:lib && jlpm clean:labextension && jlpm clean:lintcache",
-        "clean:labextension": "rimraf imjoy-jupyterlab-extension/labextension imjoy-jupyterlab-extension/_version.py",
+        "clean:labextension": "rimraf imjoy_jupyterlab_extension/labextension imjoy_jupyterlab_extension/_version.py",
         "clean:lib": "rimraf lib tsconfig.tsbuildinfo",
         "clean:lintcache": "rimraf .eslintcache .stylelintcache",
         "eslint": "jlpm eslint:check --fix",
         "eslint:check": "eslint . --cache --ext .ts,.tsx",
         "install:extension": "jlpm build",
         "lint": "jlpm stylelint && jlpm prettier && jlpm eslint",
         "lint:check": "jlpm stylelint:check && jlpm prettier:check && jlpm eslint:check",
@@ -192,9 +192,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": "^([a-z][A-z\\d]*)(-[A-z\\d]+)*$",
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.2.1"
+    "version": "0.2.2"
 }
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js.map` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/lib_index_js.b3c4fd70a9b5a1095fd0.js.map`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/remoteEntry.4ec6ba01760800a64c63.js` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/remoteEntry.8f8e573811b7938685a1.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -428,15 +428,15 @@
             /******/
             var promises = [];
             /******/
             switch (name) {
                 /******/
                 case "default": {
                     /******/
-                    register("imjoy-jupyterlab-extension", "0.2.1", () => (Promise.all([__webpack_require__.e("vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
+                    register("imjoy-jupyterlab-extension", "0.2.2", () => (Promise.all([__webpack_require__.e("vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js"), __webpack_require__.e("lib_index_js")]).then(() => (() => (__webpack_require__( /*! ./lib/index.js */ "./lib/index.js"))))));
                     /******/
                 }
                 /******/
                 break;
                 /******/
             }
             /******/
@@ -1097,8 +1097,8 @@
     /******/
     var __webpack_exports__ = __webpack_require__("webpack/container/entry/imjoy-jupyterlab-extension");
     /******/
     (_JUPYTERLAB = typeof _JUPYTERLAB === "undefined" ? {} : _JUPYTERLAB)["imjoy-jupyterlab-extension"] = __webpack_exports__;
     /******/
     /******/
 })();
-//# sourceMappingURL=remoteEntry.4ec6ba01760800a64c63.js.map
+//# sourceMappingURL=remoteEntry.8f8e573811b7938685a1.js.map
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/remoteEntry.4ec6ba01760800a64c63.js.map` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/remoteEntry.8f8e573811b7938685a1.js.map`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9210526315789475%*

 * *Differences: {"'file'": "'remoteEntry.8f8e573811b7938685a1.js'",*

 * * "'sourcesContent'": "{insert: [(10, '__webpack_require__.S = {};\\nvar initPromises = {};\\nvar "*

 * *                     'initTokens = {};\\n__webpack_require__.I = (name, initScope) => '*

 * *                     '{\\n\\tif(!initScope) initScope = [];\\n\\t// handling circular init '*

 * *                     'calls\\n\\tvar initToken = initTokens[name];\\n\\tif(!initToken) initToken = '*

 * *                     'initTokens[name] = {};\\n\\tif(initScope.indexOf(initToke […]*

```diff
@@ -1,9 +1,9 @@
 {
-    "file": "remoteEntry.4ec6ba01760800a64c63.js",
+    "file": "remoteEntry.8f8e573811b7938685a1.js",
     "mappings": ";;;;;;;;;;;AAAA;AACA;AACA;AACA,EAAE;AACF;AACA;AACA,EAAE;AACF;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA,IAAI;AACJ;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;AACA;;AAEA;AACA;AACA;AACA;AACA,CAAC;;;;;;UCpCD;UACA;;UAEA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;UACA;;UAEA;UACA;;UAEA;UACA;;;;;WC5BA;WACA;WACA;WACA;WACA;WACA,iCAAiC,WAAW;WAC5C;WACA;;;;;WCPA;WACA;WACA;WACA;WACA,yCAAyC,wCAAwC;WACjF;WACA;WACA;;;;;WCPA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;;;;;WCRA;WACA;WACA;WACA,8BAA8B,sMAAsM;WACpO;;;;;WCJA;WACA;WACA;WACA;WACA,GAAG;WACH;WACA;WACA,CAAC;;;;;WCPD;;;;;WCAA;WACA;WACA;WACA;WACA,uBAAuB,4BAA4B;WACnD;WACA;WACA;WACA,iBAAiB,oBAAoB;WACrC;WACA,mGAAmG,YAAY;WAC/G;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,mEAAmE,iCAAiC;WACpG;WACA;WACA;WACA;;;;;WCzCA;WACA;WACA;WACA,uDAAuD,iBAAiB;WACxE;WACA,gDAAgD,aAAa;WAC7D;;;;;WCNA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,oJAAoJ;WACpJ;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,IAAI,aAAa;WACjB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WC7CA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;;;;WClBA;WACA;WACA,WAAW,6BAA6B,iBAAiB,GAAG,qEAAqE;WACjI;WACA;WACA;WACA,qCAAqC,aAAa,EAAE,wDAAwD,2BAA2B,4BAA4B,2BAA2B,+CAA+C,mCAAmC;WAChR;WACA;WACA;WACA,qBAAqB,8BAA8B,SAAS,sDAAsD,gBAAgB,eAAe,KAAK,6DAA6D,SAAS,SAAS,QAAQ,eAAe,KAAK,eAAe,qGAAqG,WAAW,aAAa;WAC7Y;WACA;WACA;WACA,gBAAgB,8BAA8B,qBAAqB,YAAY,sBAAsB,SAAS,iDAAiD,6FAA6F,WAAW,uBAAuB,2BAA2B,wBAAwB,KAAK,oCAAoC,oBAAoB,wBAAwB,oBAAoB,SAAS,KAAK,yBAAyB,KAAK,gCAAgC,yBAAyB,QAAQ,eAAe,KAAK,eAAe,4DAA4D;WACtoB;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA,EAAE;WACF;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,CAAC;;WAED;WACA;WACA;WACA,CAAC;WACD;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA,CAAC;WACD;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM;WACN,KAAK,WAAW;WAChB;WACA,GAAG;WACH;WACA;;;;;WCtLA;;WAEA;WACA;WACA;WACA;WACA;WACA;;WAEA;WACA;WACA;WACA,iCAAiC;;WAEjC;WACA;WACA;WACA,KAAK;WACL,eAAe;WACf;WACA;WACA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;;WAEA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA;WACA,MAAM,qBAAqB;WAC3B;WACA;WACA;WACA;WACA;WACA;;WAEA;;WAEA;WACA;WACA;;;;;WCrFA;;;;;UEAA;UACA;UACA;UACA",
     "names": [],
     "sourceRoot": "",
     "sources": [
         "webpack://imjoy-jupyterlab-extension/webpack/container-entry",
         "webpack://imjoy-jupyterlab-extension/webpack/bootstrap",
         "webpack://imjoy-jupyterlab-extension/webpack/runtime/compat get default export",
@@ -30,15 +30,15 @@
         "// define getter functions for harmony exports\n__webpack_require__.d = (exports, definition) => {\n\tfor(var key in definition) {\n\t\tif(__webpack_require__.o(definition, key) && !__webpack_require__.o(exports, key)) {\n\t\t\tObject.defineProperty(exports, key, { enumerable: true, get: definition[key] });\n\t\t}\n\t}\n};",
         "__webpack_require__.f = {};\n// This file contains only the entry chunk.\n// The chunk loading function for additional chunks\n__webpack_require__.e = (chunkId) => {\n\treturn Promise.all(Object.keys(__webpack_require__.f).reduce((promises, key) => {\n\t\t__webpack_require__.f[key](chunkId, promises);\n\t\treturn promises;\n\t}, []));\n};",
         "// This function allow to reference async chunks\n__webpack_require__.u = (chunkId) => {\n\t// return url for filenames based on template\n\treturn \"\" + chunkId + \".\" + {\"vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js\":\"fa1a9cd9c57812bbe9b2\",\"lib_index_js\":\"b3c4fd70a9b5a1095fd0\",\"style_index_js\":\"4a04af2efb9bedd57803\"}[chunkId] + \".js\";\n};",
         "__webpack_require__.g = (function() {\n\tif (typeof globalThis === 'object') return globalThis;\n\ttry {\n\t\treturn this || new Function('return this')();\n\t} catch (e) {\n\t\tif (typeof window === 'object') return window;\n\t}\n})();",
         "__webpack_require__.o = (obj, prop) => (Object.prototype.hasOwnProperty.call(obj, prop))",
         "var inProgress = {};\nvar dataWebpackPrefix = \"imjoy-jupyterlab-extension:\";\n// loadScript function to load a script via script tag\n__webpack_require__.l = (url, done, key, chunkId) => {\n\tif(inProgress[url]) { inProgress[url].push(done); return; }\n\tvar script, needAttach;\n\tif(key !== undefined) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tfor(var i = 0; i < scripts.length; i++) {\n\t\t\tvar s = scripts[i];\n\t\t\tif(s.getAttribute(\"src\") == url || s.getAttribute(\"data-webpack\") == dataWebpackPrefix + key) { script = s; break; }\n\t\t}\n\t}\n\tif(!script) {\n\t\tneedAttach = true;\n\t\tscript = document.createElement('script');\n\n\t\tscript.charset = 'utf-8';\n\t\tscript.timeout = 120;\n\t\tif (__webpack_require__.nc) {\n\t\t\tscript.setAttribute(\"nonce\", __webpack_require__.nc);\n\t\t}\n\t\tscript.setAttribute(\"data-webpack\", dataWebpackPrefix + key);\n\n\t\tscript.src = url;\n\t}\n\tinProgress[url] = [done];\n\tvar onScriptComplete = (prev, event) => {\n\t\t// avoid mem leaks in IE.\n\t\tscript.onerror = script.onload = null;\n\t\tclearTimeout(timeout);\n\t\tvar doneFns = inProgress[url];\n\t\tdelete inProgress[url];\n\t\tscript.parentNode && script.parentNode.removeChild(script);\n\t\tdoneFns && doneFns.forEach((fn) => (fn(event)));\n\t\tif(prev) return prev(event);\n\t}\n\tvar timeout = setTimeout(onScriptComplete.bind(null, undefined, { type: 'timeout', target: script }), 120000);\n\tscript.onerror = onScriptComplete.bind(null, script.onerror);\n\tscript.onload = onScriptComplete.bind(null, script.onload);\n\tneedAttach && document.head.appendChild(script);\n};",
         "// define __esModule on exports\n__webpack_require__.r = (exports) => {\n\tif(typeof Symbol !== 'undefined' && Symbol.toStringTag) {\n\t\tObject.defineProperty(exports, Symbol.toStringTag, { value: 'Module' });\n\t}\n\tObject.defineProperty(exports, '__esModule', { value: true });\n};",
-        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"imjoy-jupyterlab-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"imjoy-jupyterlab-extension\", \"0.2.1\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
+        "__webpack_require__.S = {};\nvar initPromises = {};\nvar initTokens = {};\n__webpack_require__.I = (name, initScope) => {\n\tif(!initScope) initScope = [];\n\t// handling circular init calls\n\tvar initToken = initTokens[name];\n\tif(!initToken) initToken = initTokens[name] = {};\n\tif(initScope.indexOf(initToken) >= 0) return;\n\tinitScope.push(initToken);\n\t// only runs once\n\tif(initPromises[name]) return initPromises[name];\n\t// creates a new share scope if needed\n\tif(!__webpack_require__.o(__webpack_require__.S, name)) __webpack_require__.S[name] = {};\n\t// runs all init snippets from all modules reachable\n\tvar scope = __webpack_require__.S[name];\n\tvar warn = (msg) => {\n\t\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n\t};\n\tvar uniqueName = \"imjoy-jupyterlab-extension\";\n\tvar register = (name, version, factory, eager) => {\n\t\tvar versions = scope[name] = scope[name] || {};\n\t\tvar activeVersion = versions[version];\n\t\tif(!activeVersion || (!activeVersion.loaded && (!eager != !activeVersion.eager ? eager : uniqueName > activeVersion.from))) versions[version] = { get: factory, from: uniqueName, eager: !!eager };\n\t};\n\tvar initExternal = (id) => {\n\t\tvar handleError = (err) => (warn(\"Initialization of sharing external failed: \" + err));\n\t\ttry {\n\t\t\tvar module = __webpack_require__(id);\n\t\t\tif(!module) return;\n\t\t\tvar initFn = (module) => (module && module.init && module.init(__webpack_require__.S[name], initScope))\n\t\t\tif(module.then) return promises.push(module.then(initFn, handleError));\n\t\t\tvar initResult = initFn(module);\n\t\t\tif(initResult && initResult.then) return promises.push(initResult['catch'](handleError));\n\t\t} catch(err) { handleError(err); }\n\t}\n\tvar promises = [];\n\tswitch(name) {\n\t\tcase \"default\": {\n\t\t\tregister(\"imjoy-jupyterlab-extension\", \"0.2.2\", () => (Promise.all([__webpack_require__.e(\"vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js\"), __webpack_require__.e(\"lib_index_js\")]).then(() => (() => (__webpack_require__(/*! ./lib/index.js */ \"./lib/index.js\"))))));\n\t\t}\n\t\tbreak;\n\t}\n\tif(!promises.length) return initPromises[name] = 1;\n\treturn initPromises[name] = Promise.all(promises).then(() => (initPromises[name] = 1));\n};",
         "var scriptUrl;\nif (__webpack_require__.g.importScripts) scriptUrl = __webpack_require__.g.location + \"\";\nvar document = __webpack_require__.g.document;\nif (!scriptUrl && document) {\n\tif (document.currentScript)\n\t\tscriptUrl = document.currentScript.src;\n\tif (!scriptUrl) {\n\t\tvar scripts = document.getElementsByTagName(\"script\");\n\t\tif(scripts.length) {\n\t\t\tvar i = scripts.length - 1;\n\t\t\twhile (i > -1 && (!scriptUrl || !/^http(s?):/.test(scriptUrl))) scriptUrl = scripts[i--].src;\n\t\t}\n\t}\n}\n// When supporting browsers where an automatic publicPath is not supported you must specify an output.publicPath manually via configuration\n// or pass an empty string (\"\") and set the __webpack_public_path__ variable from your code to use your own logic.\nif (!scriptUrl) throw new Error(\"Automatic publicPath is not supported in this browser\");\nscriptUrl = scriptUrl.replace(/#.*$/, \"\").replace(/\\?.*$/, \"\").replace(/\\/[^\\/]+$/, \"/\");\n__webpack_require__.p = scriptUrl;",
         "var parseVersion = (str) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar p=p=>{return p.split(\".\").map((p=>{return+p==p?+p:p}))},n=/^([^-+]+)?(?:-([^+]+))?(?:\\+(.+))?$/.exec(str),r=n[1]?p(n[1]):[];return n[2]&&(r.length++,r.push.apply(r,p(n[2]))),n[3]&&(r.push([]),r.push.apply(r,p(n[3]))),r;\n}\nvar versionLt = (a, b) => {\n\t// see webpack/lib/util/semver.js for original code\n\ta=parseVersion(a),b=parseVersion(b);for(var r=0;;){if(r>=a.length)return r<b.length&&\"u\"!=(typeof b[r])[0];var e=a[r],n=(typeof e)[0];if(r>=b.length)return\"u\"==n;var t=b[r],f=(typeof t)[0];if(n!=f)return\"o\"==n&&\"n\"==f||(\"s\"==f||\"u\"==n);if(\"o\"!=n&&\"u\"!=n&&e!=t)return e<t;r++}\n}\nvar rangeToString = (range) => {\n\t// see webpack/lib/util/semver.js for original code\n\tvar r=range[0],n=\"\";if(1===range.length)return\"*\";if(r+.5){n+=0==r?\">=\":-1==r?\"<\":1==r?\"^\":2==r?\"~\":r>0?\"=\":\"!=\";for(var e=1,a=1;a<range.length;a++){e--,n+=\"u\"==(typeof(t=range[a]))[0]?\"-\":(e>0?\".\":\"\")+(e=2,t)}return n}var g=[];for(a=1;a<range.length;a++){var t=range[a];g.push(0===t?\"not(\"+o()+\")\":1===t?\"(\"+o()+\" || \"+o()+\")\":2===t?g.pop()+\" \"+g.pop():rangeToString(t))}return o();function o(){return g.pop().replace(/^\\((.+)\\)$/,\"$1\")}\n}\nvar satisfy = (range, version) => {\n\t// see webpack/lib/util/semver.js for original code\n\tif(0 in range){version=parseVersion(version);var e=range[0],r=e<0;r&&(e=-e-1);for(var n=0,i=1,a=!0;;i++,n++){var f,s,g=i<range.length?(typeof range[i])[0]:\"\";if(n>=version.length||\"o\"==(s=(typeof(f=version[n]))[0]))return!a||(\"u\"==g?i>e&&!r:\"\"==g!=r);if(\"u\"==s){if(!a||\"u\"!=g)return!1}else if(a)if(g==s)if(i<=e){if(f!=range[i])return!1}else{if(r?f>range[i]:f<range[i])return!1;f!=range[i]&&(a=!1)}else if(\"s\"!=g&&\"n\"!=g){if(r||i<=e)return!1;a=!1,i--}else{if(i<=e||s<g!=r)return!1;a=!1}else\"s\"!=g&&\"n\"!=g&&(a=!1,i--)}}var t=[],o=t.pop.bind(t);for(n=1;n<range.length;n++){var u=range[n];t.push(1==u?o()|o():2==u?o()&o():u?satisfy(u,version):!o())}return!!o();\n}\nvar ensureExistence = (scopeName, key) => {\n\tvar scope = __webpack_require__.S[scopeName];\n\tif(!scope || !__webpack_require__.o(scope, key)) throw new Error(\"Shared module \" + key + \" doesn't exist in shared scope \" + scopeName);\n\treturn scope;\n};\nvar findVersion = (scope, key) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar findSingletonVersionKey = (scope, key) => {\n\tvar versions = scope[key];\n\treturn Object.keys(versions).reduce((a, b) => {\n\t\treturn !a || (!versions[a].loaded && versionLt(a, b)) ? b : a;\n\t}, 0);\n};\nvar getInvalidSingletonVersionMessage = (scope, key, version, requiredVersion) => {\n\treturn \"Unsatisfied version \" + version + \" from \" + (version && scope[key][version].from) + \" of shared singleton module \" + key + \" (required \" + rangeToString(requiredVersion) + \")\"\n};\nvar getSingleton = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\treturn get(scope[key][version]);\n};\nvar getSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) warn(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar getStrictSingletonVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar version = findSingletonVersionKey(scope, key);\n\tif (!satisfy(requiredVersion, version)) throw new Error(getInvalidSingletonVersionMessage(scope, key, version, requiredVersion));\n\treturn get(scope[key][version]);\n};\nvar findValidVersion = (scope, key, requiredVersion) => {\n\tvar versions = scope[key];\n\tvar key = Object.keys(versions).reduce((a, b) => {\n\t\tif (!satisfy(requiredVersion, b)) return a;\n\t\treturn !a || versionLt(a, b) ? b : a;\n\t}, 0);\n\treturn key && versions[key]\n};\nvar getInvalidVersionMessage = (scope, scopeName, key, requiredVersion) => {\n\tvar versions = scope[key];\n\treturn \"No satisfying version (\" + rangeToString(requiredVersion) + \") of shared module \" + key + \" found in shared scope \" + scopeName + \".\\n\" +\n\t\t\"Available versions: \" + Object.keys(versions).map((key) => {\n\t\treturn key + \" from \" + versions[key].from;\n\t}).join(\", \");\n};\nvar getValidVersion = (scope, scopeName, key, requiredVersion) => {\n\tvar entry = findValidVersion(scope, key, requiredVersion);\n\tif(entry) return get(entry);\n\tthrow new Error(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar warn = (msg) => {\n\tif (typeof console !== \"undefined\" && console.warn) console.warn(msg);\n};\nvar warnInvalidVersion = (scope, scopeName, key, requiredVersion) => {\n\twarn(getInvalidVersionMessage(scope, scopeName, key, requiredVersion));\n};\nvar get = (entry) => {\n\tentry.loaded = 1;\n\treturn entry.get()\n};\nvar init = (fn) => (function(scopeName, a, b, c) {\n\tvar promise = __webpack_require__.I(scopeName);\n\tif (promise && promise.then) return promise.then(fn.bind(fn, scopeName, __webpack_require__.S[scopeName], a, b, c));\n\treturn fn(scopeName, __webpack_require__.S[scopeName], a, b, c);\n});\n\nvar load = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn get(findVersion(scope, key));\n});\nvar loadFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\treturn scope && __webpack_require__.o(scope, key) ? get(findVersion(scope, key)) : fallback();\n});\nvar loadVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingleton = /*#__PURE__*/ init((scopeName, scope, key) => {\n\tensureExistence(scopeName, key);\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getValidVersion(scope, scopeName, key, version);\n});\nvar loadStrictSingletonVersionCheck = /*#__PURE__*/ init((scopeName, scope, key, version) => {\n\tensureExistence(scopeName, key);\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar loadVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn get(findValidVersion(scope, key, version) || warnInvalidVersion(scope, scopeName, key, version) || findVersion(scope, key));\n});\nvar loadSingletonFallback = /*#__PURE__*/ init((scopeName, scope, key, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingleton(scope, scopeName, key);\n});\nvar loadSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getSingletonVersion(scope, scopeName, key, version);\n});\nvar loadStrictVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tvar entry = scope && __webpack_require__.o(scope, key) && findValidVersion(scope, key, version);\n\treturn entry ? get(entry) : fallback();\n});\nvar loadStrictSingletonVersionCheckFallback = /*#__PURE__*/ init((scopeName, scope, key, version, fallback) => {\n\tif(!scope || !__webpack_require__.o(scope, key)) return fallback();\n\treturn getStrictSingletonVersion(scope, scopeName, key, version);\n});\nvar installedModules = {};\nvar moduleToHandlerMapping = {\n\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/filebrowser\", [1,4,0,9])),\n\t\"webpack/sharing/consume/default/@jupyterlab/translation\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/translation\", [1,4,0,9])),\n\t\"webpack/sharing/consume/default/@jupyterlab/apputils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/apputils\", [1,4,1,9])),\n\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\": () => (loadSingletonVersionCheck(\"default\", \"@jupyterlab/coreutils\", [1,6,0,9])),\n\t\"webpack/sharing/consume/default/@lumino/disposable\": () => (loadSingletonVersionCheck(\"default\", \"@lumino/disposable\", [1,2,0,0]))\n};\n// no consumes in initial chunks\nvar chunkMapping = {\n\t\"lib_index_js\": [\n\t\t\"webpack/sharing/consume/default/@jupyterlab/filebrowser\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/translation\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/apputils\",\n\t\t\"webpack/sharing/consume/default/@jupyterlab/coreutils\",\n\t\t\"webpack/sharing/consume/default/@lumino/disposable\"\n\t]\n};\nvar startedInstallModules = {};\n__webpack_require__.f.consumes = (chunkId, promises) => {\n\tif(__webpack_require__.o(chunkMapping, chunkId)) {\n\t\tchunkMapping[chunkId].forEach((id) => {\n\t\t\tif(__webpack_require__.o(installedModules, id)) return promises.push(installedModules[id]);\n\t\t\tif(!startedInstallModules[id]) {\n\t\t\tvar onFactory = (factory) => {\n\t\t\t\tinstalledModules[id] = 0;\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tmodule.exports = factory();\n\t\t\t\t}\n\t\t\t};\n\t\t\tstartedInstallModules[id] = true;\n\t\t\tvar onError = (error) => {\n\t\t\t\tdelete installedModules[id];\n\t\t\t\t__webpack_require__.m[id] = (module) => {\n\t\t\t\t\tdelete __webpack_require__.c[id];\n\t\t\t\t\tthrow error;\n\t\t\t\t}\n\t\t\t};\n\t\t\ttry {\n\t\t\t\tvar promise = moduleToHandlerMapping[id]();\n\t\t\t\tif(promise.then) {\n\t\t\t\t\tpromises.push(installedModules[id] = promise.then(onFactory)['catch'](onError));\n\t\t\t\t} else onFactory(promise);\n\t\t\t} catch(e) { onError(e); }\n\t\t\t}\n\t\t});\n\t}\n}",
         "// no baseURI\n\n// object to store loaded and loading chunks\n// undefined = chunk not loaded, null = chunk preloaded/prefetched\n// [resolve, reject, Promise] = chunk loading, 0 = chunk loaded\nvar installedChunks = {\n\t\"imjoy-jupyterlab-extension\": 0\n};\n\n__webpack_require__.f.j = (chunkId, promises) => {\n\t\t// JSONP chunk loading for javascript\n\t\tvar installedChunkData = __webpack_require__.o(installedChunks, chunkId) ? installedChunks[chunkId] : undefined;\n\t\tif(installedChunkData !== 0) { // 0 means \"already installed\".\n\n\t\t\t// a Promise means \"currently loading\".\n\t\t\tif(installedChunkData) {\n\t\t\t\tpromises.push(installedChunkData[2]);\n\t\t\t} else {\n\t\t\t\tif(true) { // all chunks have JS\n\t\t\t\t\t// setup Promise in chunk cache\n\t\t\t\t\tvar promise = new Promise((resolve, reject) => (installedChunkData = installedChunks[chunkId] = [resolve, reject]));\n\t\t\t\t\tpromises.push(installedChunkData[2] = promise);\n\n\t\t\t\t\t// start chunk loading\n\t\t\t\t\tvar url = __webpack_require__.p + __webpack_require__.u(chunkId);\n\t\t\t\t\t// create error before stack unwound to get useful stacktrace later\n\t\t\t\t\tvar error = new Error();\n\t\t\t\t\tvar loadingEnded = (event) => {\n\t\t\t\t\t\tif(__webpack_require__.o(installedChunks, chunkId)) {\n\t\t\t\t\t\t\tinstalledChunkData = installedChunks[chunkId];\n\t\t\t\t\t\t\tif(installedChunkData !== 0) installedChunks[chunkId] = undefined;\n\t\t\t\t\t\t\tif(installedChunkData) {\n\t\t\t\t\t\t\t\tvar errorType = event && (event.type === 'load' ? 'missing' : event.type);\n\t\t\t\t\t\t\t\tvar realSrc = event && event.target && event.target.src;\n\t\t\t\t\t\t\t\terror.message = 'Loading chunk ' + chunkId + ' failed.\\n(' + errorType + ': ' + realSrc + ')';\n\t\t\t\t\t\t\t\terror.name = 'ChunkLoadError';\n\t\t\t\t\t\t\t\terror.type = errorType;\n\t\t\t\t\t\t\t\terror.request = realSrc;\n\t\t\t\t\t\t\t\tinstalledChunkData[1](error);\n\t\t\t\t\t\t\t}\n\t\t\t\t\t\t}\n\t\t\t\t\t};\n\t\t\t\t\t__webpack_require__.l(url, loadingEnded, \"chunk-\" + chunkId, chunkId);\n\t\t\t\t}\n\t\t\t}\n\t\t}\n};\n\n// no prefetching\n\n// no preloaded\n\n// no HMR\n\n// no HMR manifest\n\n// no on chunks loaded\n\n// install a JSONP callback for chunk loading\nvar webpackJsonpCallback = (parentChunkLoadingFunction, data) => {\n\tvar [chunkIds, moreModules, runtime] = data;\n\t// add \"moreModules\" to the modules object,\n\t// then flag all \"chunkIds\" as loaded and fire callback\n\tvar moduleId, chunkId, i = 0;\n\tif(chunkIds.some((id) => (installedChunks[id] !== 0))) {\n\t\tfor(moduleId in moreModules) {\n\t\t\tif(__webpack_require__.o(moreModules, moduleId)) {\n\t\t\t\t__webpack_require__.m[moduleId] = moreModules[moduleId];\n\t\t\t}\n\t\t}\n\t\tif(runtime) var result = runtime(__webpack_require__);\n\t}\n\tif(parentChunkLoadingFunction) parentChunkLoadingFunction(data);\n\tfor(;i < chunkIds.length; i++) {\n\t\tchunkId = chunkIds[i];\n\t\tif(__webpack_require__.o(installedChunks, chunkId) && installedChunks[chunkId]) {\n\t\t\tinstalledChunks[chunkId][0]();\n\t\t}\n\t\tinstalledChunks[chunkId] = 0;\n\t}\n\n}\n\nvar chunkLoadingGlobal = self[\"webpackChunkimjoy_jupyterlab_extension\"] = self[\"webpackChunkimjoy_jupyterlab_extension\"] || [];\nchunkLoadingGlobal.forEach(webpackJsonpCallback.bind(null, 0));\nchunkLoadingGlobal.push = webpackJsonpCallback.bind(null, chunkLoadingGlobal.push.bind(chunkLoadingGlobal));",
         "__webpack_require__.nc = undefined;",
         "",
         "// module cache are used so entry inlining is disabled\n// startup\n// Load entry module and return exports\nvar __webpack_exports__ = __webpack_require__(\"webpack/container/entry/imjoy-jupyterlab-extension\");\n",
         ""
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js.map` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/style_index_js.4a04af2efb9bedd57803.js.map`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/imjoy-jupyterlab-extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js.map` & `imjoy_jupyterlab_extension-0.2.2/imjoy_jupyterlab_extension/labextension/static/vendors-node_modules_imjoy-core_dist_imjoy-loader_js-node_modules_imjoy-core_dist_imjoy-rpc_js.fa1a9cd9c57812bbe9b2.js.map`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/src/comm-connection.js` & `imjoy_jupyterlab_extension-0.2.2/src/comm-connection.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/src/imjoy-extension.js` & `imjoy_jupyterlab_extension-0.2.2/src/imjoy-extension.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/src/index.ts` & `imjoy_jupyterlab_extension-0.2.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/src/utils.js` & `imjoy_jupyterlab_extension-0.2.2/src/utils.js`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/ui-tests/README.md` & `imjoy_jupyterlab_extension-0.2.2/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/ui-tests/tests/imjoy-jupyterlab-extension.spec.ts` & `imjoy_jupyterlab_extension-0.2.2/ui-tests/tests/imjoy-jupyterlab-extension.spec.ts`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/.gitignore` & `imjoy_jupyterlab_extension-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/LICENSE` & `imjoy_jupyterlab_extension-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/README.md` & `imjoy_jupyterlab_extension-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `imjoy_jupyterlab_extension-0.2.1/pyproject.toml` & `imjoy_jupyterlab_extension-0.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling>=1.5.0,<1.22.2", "jupyterlab>=4.0.0,<5", "hatch-nodejs-version>=0.3.2"]
 build-backend = "hatchling.build"
 
 [project]
-name = "imjoy-jupyterlab-extension"
+name = "imjoy_jupyterlab_extension"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.8"
 classifiers = [
     "Framework :: Jupyter",
     "Framework :: Jupyter :: JupyterLab",
     "Framework :: Jupyter :: JupyterLab :: 4",
@@ -30,42 +30,42 @@
 [tool.hatch.version]
 source = "nodejs"
 
 [tool.hatch.metadata.hooks.nodejs]
 fields = ["description", "authors", "urls"]
 
 [tool.hatch.build.targets.sdist]
-artifacts = ["imjoy-jupyterlab-extension/labextension"]
+artifacts = ["imjoy_jupyterlab_extension/labextension"]
 exclude = [".github", "binder"]
 
 [tool.hatch.build.targets.wheel.shared-data]
-"imjoy-jupyterlab-extension/labextension" = "share/jupyter/labextensions/imjoy-jupyterlab-extension"
-"install.json" = "share/jupyter/labextensions/imjoy-jupyterlab-extension/install.json"
+"imjoy_jupyterlab_extension/labextension" = "share/jupyter/labextensions/imjoy_jupyterlab_extension"
+"install.json" = "share/jupyter/labextensions/imjoy_jupyterlab_extension/install.json"
 
 [tool.hatch.build.hooks.version]
-path = "imjoy-jupyterlab-extension/_version.py"
+path = "imjoy_jupyterlab_extension/_version.py"
 
 [tool.hatch.build.hooks.jupyter-builder]
 dependencies = ["hatch-jupyter-builder>=0.5"]
 build-function = "hatch_jupyter_builder.npm_builder"
 ensured-targets = [
-    "imjoy-jupyterlab-extension/labextension/static/style.js",
-    "imjoy-jupyterlab-extension/labextension/package.json",
+    "imjoy_jupyterlab_extension/labextension/static/style.js",
+    "imjoy_jupyterlab_extension/labextension/package.json",
 ]
-skip-if-exists = ["imjoy-jupyterlab-extension/labextension/static/style.js"]
+skip-if-exists = ["imjoy_jupyterlab_extension/labextension/static/style.js"]
 
 [tool.hatch.build.hooks.jupyter-builder.build-kwargs]
 build_cmd = "build:prod"
 npm = ["jlpm"]
 
 [tool.hatch.build.hooks.jupyter-builder.editable-build-kwargs]
 build_cmd = "install:extension"
 npm = ["jlpm"]
 source_dir = "src"
-build_dir = "imjoy-jupyterlab-extension/labextension"
+build_dir = "imjoy_jupyterlab_extension/labextension"
 
 [tool.jupyter-releaser.options]
 version_cmd = "hatch version"
 
 [tool.jupyter-releaser.hooks]
 before-build-npm = [
     "python -m pip install 'jupyterlab>=4.0.0,<5'",
```

### Comparing `imjoy_jupyterlab_extension-0.2.1/PKG-INFO` & `imjoy_jupyterlab_extension-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: imjoy-jupyterlab-extension
-Version: 0.2.1
+Name: imjoy_jupyterlab_extension
+Version: 0.2.2
 Summary: Run ImJoy plugins in JupyterLab
 Project-URL: Homepage, https://github.com/imjoy-team/imjoy-jupyterlab-extension
 Project-URL: Bug Tracker, https://github.com/imjoy-team/imjoy-jupyterlab-extension/issues
 Project-URL: Repository, https://github.com/imjoy-team/imjoy-jupyterlab-extension.git
 Author-email: Wei Ouyang <oeway007@gmail.com>
 License: BSD 3-Clause License
```

