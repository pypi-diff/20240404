# Comparing `tmp/owasp-depscan-5.3.0.tar.gz` & `tmp/owasp-depscan-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owasp-depscan-5.3.0.tar", last modified: Tue Apr  2 10:34:25 2024, max compression
+gzip compressed data, was "owasp-depscan-5.3.1.tar", last modified: Thu Apr  4 21:28:11 2024, max compression
```

## Comparing `owasp-depscan-5.3.0.tar` & `owasp-depscan-5.3.1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/depscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/depscan/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58212 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/github.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/license.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12443 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/normalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/orasclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/depscan/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/owasp_depscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 10:34:25.000000 owasp-depscan-5.3.0/owasp_depscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:34:25.803510 owasp-depscan-5.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_bom.py
--rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_csaf.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_explainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_norm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_pkg_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.783510 owasp-depscan-5.3.0/vendor/choosealicense.com/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.791510 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/fields.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/meta.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_data/rules.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.799510 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/0bsd.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/afl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/isc.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit-0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-pl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-rl.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ncsa.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/osl-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/postgresql.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/upl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/vim.txt
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/wtfpl.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/zlib.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.787510 owasp-depscan-5.3.0/vendor/spdx/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:34:25.799510 owasp-depscan-5.3.0/vendor/spdx/json/
--rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-04-02 10:34:16.000000 owasp-depscan-5.3.0/vendor/spdx/json/licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    26607 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.456152 owasp-depscan-5.3.1/depscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38835 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.460152 owasp-depscan-5.3.1/depscan/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59180 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16718 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14577 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81781 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12619 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/orasclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20394 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14763 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/depscan/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/owasp_depscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    28084 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-04 21:28:11.000000 owasp-depscan-5.3.1/owasp_depscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.464152 owasp-depscan-5.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    32402 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_bom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37991 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_csaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8072 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_pkg_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.464152 owasp-depscan-5.3.1/vendor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.456152 owasp-depscan-5.3.1/vendor/choosealicense.com/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.464152 owasp-depscan-5.3.1/vendor/choosealicense.com/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_data/fields.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_data/meta.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2830 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_data/rules.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/0bsd.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11142 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/afl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35944 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/agpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12624 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/artistic-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-2-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-3-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-4-clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc-by-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21473 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cecill-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14802 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15986 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ecl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12461 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/epl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15112 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/epl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14163 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/eupl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/eupl-1.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gfdl-1.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19293 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36394 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/isc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27491 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lgpl-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lgpl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    19902 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lppl-1.3c.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mit-0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18103 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mpl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ms-pl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ms-rl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ncsa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26179 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/odbl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ofl-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11580 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/osl-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/postgresql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/upl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/vim.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/wtfpl.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/zlib.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.456152 owasp-depscan-5.3.1/vendor/spdx/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 21:28:11.472152 owasp-depscan-5.3.1/vendor/spdx/json/
+-rw-r--r--   0 runner    (1001) docker     (127)   275192 2024-04-04 21:28:01.000000 owasp-depscan-5.3.1/vendor/spdx/json/licenses.json
```

### Comparing `owasp-depscan-5.3.0/LICENSE` & `owasp-depscan-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/PKG-INFO` & `owasp-depscan-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.3.0
+Version: 5.3.1
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.6
+Requires-Dist: appthreat-vulnerability-db==5.6.7
 Requires-Dist: defusedxml
 Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
```

### Comparing `owasp-depscan-5.3.0/README.md` & `owasp-depscan-5.3.1/README.md`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/cli.py` & `owasp-depscan-5.3.1/depscan/cli.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/analysis.py` & `owasp-depscan-5.3.1/depscan/lib/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,27 +221,45 @@
             return pkg_tree, tree
     return pkg_tree, Tree(
         get_pkg_display(purl, purl, extra_text=extra_text),
         style=Style(color="bright_red" if pkg_severity == "CRITICAL" else None),
     )
 
 
+def is_lang_sw_edition(package_issue):
+    """Check if the specified sw_edition belongs to any application package type"""
+    if package_issue and package_issue["affected_location"].get("cpe_uri"):
+        all_parts = CPE_FULL_REGEX.match(
+            package_issue["affected_location"].get("cpe_uri")
+        )
+        if not all_parts or all_parts.group("sw_edition") in ("*", "-"):
+            return True
+        if (
+            config.LANG_PKG_TYPES.get(all_parts.group("sw_edition"))
+            or all_parts.group("sw_edition")
+            in config.LANG_PKG_TYPES.values()
+        ):
+            return True
+        return False
+    return True
+
+
 def is_os_target_sw(package_issue):
     """
     Since we rely on NVD, we filter those target_sw that definitely belong to a language
     """
     if package_issue and package_issue["affected_location"].get("cpe_uri"):
         all_parts = CPE_FULL_REGEX.match(
             package_issue["affected_location"].get("cpe_uri")
         )
         if (
             all_parts
-            and all_parts.group("target_sw") != "*"
+            and all_parts.group("target_sw") not in ("*", "-")
             and (
-                all_parts.group("target_sw") in config.LANG_PKG_TYPES.keys()
+                config.LANG_PKG_TYPES.get(all_parts.group("target_sw"))
                 or all_parts.group("target_sw")
                 in config.LANG_PKG_TYPES.values()
             )
         ):
             return False
     return True
 
@@ -363,40 +381,44 @@
         # If the match was based on name and version alone then the alias might legitimately lack a full purl
         # Such results are usually false positives but could yield good hits at times
         # So, instead of suppressing fully we try our best to tune and reduce the FP
         if not purl.startswith("pkg:"):
             if options.project_type in config.OS_PKG_TYPES:
                 if vendor and (
                     vendor in config.LANG_PKG_TYPES.values()
-                    or vendor in config.LANG_PKG_TYPES.keys()
+                    or config.LANG_PKG_TYPES.get(vendor)
                 ):
                     fp_count += 1
                     continue
                 # Some nvd data might match application CVEs for
                 # OS vendors which can be filtered
                 if not is_os_target_sw(package_issue):
                     fp_count += 1
                     continue
         else:
             purl_obj = parse_purl(purl)
             if purl_obj:
                 version_used = purl_obj.get("version")
                 package_type = purl_obj.get("type")
                 qualifiers = purl_obj.get("qualifiers", {})
+                # Filter application CVEs from distros
+                if (config.LANG_PKG_TYPES.get(package_type) or package_type in config.LANG_PKG_TYPES.values()) and ((vendor and vendor in config.OS_PKG_TYPES) or not is_lang_sw_edition(package_issue)):
+                    fp_count += 1
+                    continue
                 if package_type in config.OS_PKG_TYPES:
                     # Bug #208 - do not report application CVEs
                     if vendor and (
                         vendor in config.LANG_PKG_TYPES.values()
-                        or vendor in config.LANG_PKG_TYPES.keys()
+                        or config.LANG_PKG_TYPES.get(vendor)
                     ):
                         fp_count += 1
                         continue
                     if package_type and (
                         package_type in config.LANG_PKG_TYPES.values()
-                        or package_type in config.LANG_PKG_TYPES.keys()
+                        or config.LANG_PKG_TYPES.get(package_type)
                     ):
                         fp_count += 1
                         continue
                     if (
                         vendor
                         and oci_product_types
                         and vendor not in oci_product_types
```

### Comparing `owasp-depscan-5.3.0/depscan/lib/audit.py` & `owasp-depscan-5.3.1/depscan/lib/audit.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/bom.py` & `owasp-depscan-5.3.1/depscan/lib/bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/config.py` & `owasp-depscan-5.3.1/depscan/lib/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,14 +152,15 @@
     "json-smart": "json-smart-v2",
     "ojdbc7": "jdbc",
     "System.Text": ".net",
     "System.Net": "asp.net_core",
     "Microsoft.IdentityModel.Clients.ActiveDirectory": "active_directory_authentication_library",
     "starkbank_ecdsa": "ecdsa-elixir",
     "php-pear": "pear-core-minimal",
+    "Selenium.WebDriver": "selenium"
 }
 
 # Default ignore list
 ignore_directories = [
     ".git",
     ".svn",
     ".mvn",
```

### Comparing `owasp-depscan-5.3.0/depscan/lib/csaf.py` & `owasp-depscan-5.3.1/depscan/lib/csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/explainer.py` & `owasp-depscan-5.3.1/depscan/lib/explainer.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/github.py` & `owasp-depscan-5.3.1/depscan/lib/github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/license.py` & `owasp-depscan-5.3.1/depscan/lib/license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/logger.py` & `owasp-depscan-5.3.1/depscan/lib/logger.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/normalize.py` & `owasp-depscan-5.3.1/depscan/lib/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,16 @@
             vendor.startswith("org.")
             or vendor.startswith("io.")
             or vendor.startswith("com.")
             or vendor.startswith("net.")
         ):
             tmpA = vendor.split(".")
             # Automatically add short vendor forms
-            if len(tmpA) > 1 and len(tmpA[1]) > 3:
+            # Increase to 6 to reduce false positives when the package name is core
+            if len(tmpA) > 1 and len(tmpA[1]) > 6:
                 if tmpA[1] != name:
                     vendor_aliases.add(tmpA[1])
     # Add some common vendor aliases
     if purl.startswith("pkg:golang") and not name.startswith("go"):
         vendor_aliases.add("go")
         # Ignore third party alternatives for builtins
         if "golang" not in vendor and name not in [
@@ -204,15 +205,16 @@
         elif "lib" not in name:
             name_aliases.add("lib" + name)
         if "-bin" not in name:
             name_aliases.add(name + "-bin")
     else:
         # Filter vendor aliases that are also name aliases for non pypi packages
         # This is needed for numpy which has the vendor name numpy
-        if not purl.startswith("pkg:pypi"):
+        # Also needed for nuget. Eg: selenium:selenium
+        if not purl.startswith("pkg:pypi") and not purl.startswith("pkg:nuget"):
             vendor_aliases = [
                 x for x in vendor_aliases if x not in name_aliases or x == vendor
             ]
     if len(vendor_aliases) > 1:
         for vvar in list(vendor_aliases):
             for nvar in list(name_aliases):
                 pkg_list.append(
```

### Comparing `owasp-depscan-5.3.0/depscan/lib/orasclient.py` & `owasp-depscan-5.3.1/depscan/lib/orasclient.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/pkg_query.py` & `owasp-depscan-5.3.1/depscan/lib/pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/depscan/lib/utils.py` & `owasp-depscan-5.3.1/depscan/lib/utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/owasp_depscan.egg-info/PKG-INFO` & `owasp-depscan-5.3.1/owasp_depscan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owasp-depscan
-Version: 5.3.0
+Version: 5.3.1
 Summary: Fully open-source security audit for project dependencies based on known vulnerabilities and advisories.
 Author-email: Team AppThreat <cloud@appthreat.com>
 License: MIT
 Project-URL: Homepage, https://github.com/owasp-dep-scan/dep-scan
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: appthreat-vulnerability-db==5.6.6
+Requires-Dist: appthreat-vulnerability-db==5.6.7
 Requires-Dist: defusedxml
 Requires-Dist: oras~=0.1.26
 Requires-Dist: PyYAML
 Requires-Dist: rich
 Requires-Dist: quart
 Requires-Dist: PyGithub
 Requires-Dist: toml
```

### Comparing `owasp-depscan-5.3.0/owasp_depscan.egg-info/SOURCES.txt` & `owasp-depscan-5.3.1/owasp_depscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/pyproject.toml` & `owasp-depscan-5.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "owasp-depscan"
-version = "5.3.0"
+version = "5.3.1"
 description = "Fully open-source security audit for project dependencies based on known vulnerabilities and advisories."
 authors = [
     {name = "Team AppThreat", email = "cloud@appthreat.com"},
 ]
 dependencies = [
-    "appthreat-vulnerability-db==5.6.6",
+    "appthreat-vulnerability-db==5.6.7",
     "defusedxml",
     "oras~=0.1.26",
     "PyYAML",
     "rich",
     "quart",
     "PyGithub",
     "toml",
```

### Comparing `owasp-depscan-5.3.0/test/test_analysis.py` & `owasp-depscan-5.3.1/test/test_analysis.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_bom.py` & `owasp-depscan-5.3.1/test/test_bom.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_csaf.py` & `owasp-depscan-5.3.1/test/test_csaf.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_github.py` & `owasp-depscan-5.3.1/test/test_github.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_license.py` & `owasp-depscan-5.3.1/test/test_license.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_norm.py` & `owasp-depscan-5.3.1/test/test_norm.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_pkg_query.py` & `owasp-depscan-5.3.1/test/test_pkg_query.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/test/test_utils.py` & `owasp-depscan-5.3.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/fields.yml` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_data/fields.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/meta.yml` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_data/meta.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_data/rules.yml` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_data/rules.yml`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/0bsd.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/0bsd.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/afl-3.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/afl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/agpl-3.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/apache-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/artistic-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/artistic-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-2-clause.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-2-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-3-clause-clear.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-3-clause.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-3-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsd-4-clause.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsd-4-clause.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/bsl-1.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/bsl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-4.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc-by-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc-by-sa-4.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cc0-1.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cc0-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cecill-2.1.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cecill-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-p-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-s-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/cern-ohl-w-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ecl-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ecl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-1.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/epl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/epl-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/epl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.1.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/eupl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/eupl-1.2.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/eupl-1.2.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gfdl-1.3.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gfdl-1.3.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/gpl-3.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/gpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/isc.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/isc.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-2.1.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lgpl-2.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lgpl-3.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lgpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/lppl-1.3c.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/lppl-1.3c.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit-0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mit-0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mit.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mit.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mpl-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mpl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-pl.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ms-pl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ms-rl.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ms-rl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/mulanpsl-2.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ncsa.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ncsa.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/odbl-1.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/odbl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/ofl-1.1.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/ofl-1.1.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/osl-3.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/osl-3.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/postgresql.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/postgresql.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/unlicense.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/unlicense.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/upl-1.0.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/upl-1.0.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/vim.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/vim.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/wtfpl.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/wtfpl.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/choosealicense.com/_licenses/zlib.txt` & `owasp-depscan-5.3.1/vendor/choosealicense.com/_licenses/zlib.txt`

 * *Files identical despite different names*

### Comparing `owasp-depscan-5.3.0/vendor/spdx/json/licenses.json` & `owasp-depscan-5.3.1/vendor/spdx/json/licenses.json`

 * *Files identical despite different names*

