# Comparing `tmp/pyerfa-2.0.1.tar.gz` & `tmp/pyerfa-2.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerfa-2.0.1.tar", last modified: Fri Oct 13 19:02:52 2023, max compression
+gzip compressed data, was "pyerfa-2.0.1.1.tar", last modified: Thu Oct 19 18:22:44 2023, max compression
```

## Comparing `pyerfa-2.0.1.tar` & `pyerfa-2.0.1.1.tar`

### file list

```diff
@@ -1,350 +1,350 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.112925 pyerfa-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.056923 pyerfa-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.056923 pyerfa-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2023-10-13 19:02:20.000000 pyerfa-2.0.1/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-13 19:02:20.000000 pyerfa-2.0.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-13 19:02:20.000000 pyerfa-2.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-13 19:02:20.000000 pyerfa-2.0.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2023-10-13 19:02:20.000000 pyerfa-2.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-10-13 19:02:20.000000 pyerfa-2.0.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-10-13 19:02:20.000000 pyerfa-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2023-10-13 19:02:52.112925 pyerfa-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-10-13 19:02:20.000000 pyerfa-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-10-13 19:02:20.000000 pyerfa-2.0.1/README_REPO_IMPORT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-10-13 19:02:20.000000 pyerfa-2.0.1/RELEASING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.060923 pyerfa-2.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.056923 pyerfa-2.0.1/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.060923 pyerfa-2.0.1/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.060923 pyerfa-2.0.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/credits.rst
--rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-13 19:02:20.000000 pyerfa-2.0.1/docs/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.060923 pyerfa-2.0.1/erfa/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-10-13 19:02:51.000000 pyerfa-2.0.1/erfa/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)   738983 2023-10-13 19:02:41.000000 pyerfa-2.0.1/erfa/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/core.py.templ
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.064924 pyerfa-2.0.1/erfa/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    19730 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/tests/test_erfa.py
--rw-r--r--   0 runner    (1001) docker     (127)   154942 2023-10-13 19:02:41.000000 pyerfa-2.0.1/erfa/tests/test_ufunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/tests/test_ufunc.py.templ
--rw-r--r--   0 runner    (1001) docker     (127)   451391 2023-10-13 19:02:41.000000 pyerfa-2.0.1/erfa/ufunc.c
--rw-r--r--   0 runner    (1001) docker     (127)    35896 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/ufunc.c.templ
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    36765 2023-10-13 19:02:20.000000 pyerfa-2.0.1/erfa_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.056923 pyerfa-2.0.1/liberfa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.068924 pyerfa-2.0.1/liberfa/erfa/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/.git
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.056923 pyerfa-2.0.1/liberfa/erfa/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.068924 pyerfa-2.0.1/liberfa/erfa/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    28654 2023-10-13 19:02:46.000000 pyerfa-2.0.1/liberfa/erfa/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (127)    42494 2023-10-13 19:02:45.000000 pyerfa-2.0.1/liberfa/erfa/aclocal.m4
--rwxr-xr-x   0 runner    (1001) docker     (127)      116 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/bootstrap.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.068924 pyerfa-2.0.1/liberfa/erfa/build-aux/
--rwxrwxrwx   0 runner    (1001) docker     (127)     7400 2022-03-18 13:09:08.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/compile
--rwxrwxrwx   0 runner    (1001) docker     (127)    49482 2022-01-31 14:43:17.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/config.guess
--rwxrwxrwx   0 runner    (1001) docker     (127)    35406 2022-01-31 14:43:17.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/config.sub
--rwxrwxrwx   0 runner    (1001) docker     (127)    23568 2022-03-18 13:09:08.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/depcomp
--rwxrwxrwx   0 runner    (1001) docker     (127)    15358 2022-03-18 13:09:08.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/install-sh
--rwxrwxrwx   0 runner    (1001) docker     (127)   327299 2022-03-24 16:13:52.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/ltmain.sh
--rwxrwxrwx   0 runner    (1001) docker     (127)     6878 2022-03-18 13:09:08.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/missing
--rwxrwxrwx   0 runner    (1001) docker     (127)     4879 2022-03-18 13:09:08.000000 pyerfa-2.0.1/liberfa/erfa/build-aux/test-driver
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-10-13 19:02:46.000000 pyerfa-2.0.1/liberfa/erfa/config.h.in
--rwxr-xr-x   0 runner    (1001) docker     (127)   441029 2023-10-13 19:02:45.000000 pyerfa-2.0.1/liberfa/erfa/configure
--rw-r--r--   0 runner    (1001) docker     (127)      941 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/configure.ac
--rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/erfa.pc.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.076924 pyerfa-2.0.1/liberfa/erfa/m4/
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/m4/erfa-numver.m4
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/meson.build
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.112925 pyerfa-2.0.1/liberfa/erfa/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/Makefile.am
--rw-r--r--   0 runner    (1001) docker     (127)    83996 2023-10-13 19:02:46.000000 pyerfa-2.0.1/liberfa/erfa/src/Makefile.in
--rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/a2af.c
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/a2tf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ab.c
--rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ae2hd.c
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/af2a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/anp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/anpm.c
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apcg.c
--rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apcg13.c
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apci.c
--rw-r--r--   0 runner    (1001) docker     (127)     8531 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apci13.c
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apco.c
--rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apco13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9633 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apcs.c
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apcs13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/aper.c
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/aper13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apio.c
--rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/apio13.c
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atcc13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atccq.c
--rw-r--r--   0 runner    (1001) docker     (127)     6825 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atci13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atciq.c
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atciqn.c
--rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atciqz.c
--rw-r--r--   0 runner    (1001) docker     (127)    11074 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atco13.c
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atic13.c
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/aticq.c
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/aticqn.c
--rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atio13.c
--rw-r--r--   0 runner    (1001) docker     (127)    10095 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atioq.c
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atoc13.c
--rw-r--r--   0 runner    (1001) docker     (127)    10518 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atoi13.c
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/atoiq.c
--rw-r--r--   0 runner    (1001) docker     (127)     5300 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/bi00.c
--rw-r--r--   0 runner    (1001) docker     (127)     7078 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/bp00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/bp06.c
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/bpn2xy.c
--rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2i00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2i00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2i06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2ibpn.c
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2ixy.c
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2ixys.c
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2t00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6569 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2t00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2t06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2tcio.c
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2teqx.c
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2tpe.c
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/c2txy.c
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/cal2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/cp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/cpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/cr.c
--rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/d2dtf.c
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/d2tf.c
--rw-r--r--   0 runner    (1001) docker     (127)    11826 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/dat.c
--rw-r--r--   0 runner    (1001) docker     (127)    62193 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/dtdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/dtf2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eceq06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ecm06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ee00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ee00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ee00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5221 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ee06a.c
--rw-r--r--   0 runner    (1001) docker     (127)    10981 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eect00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eform.c
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eo06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eors.c
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/epb.c
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/epb2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/epj.c
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/epj2jd.c
--rw-r--r--   0 runner    (1001) docker     (127)   150627 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/epv00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eqec06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/eqeq94.c
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/era00.c
--rw-r--r--   0 runner    (1001) docker     (127)    27288 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfa.h
--rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfadatextra.c
--rw-r--r--   0 runner    (1001) docker     (127)      545 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfadatextra.h
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfaextra.h
--rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfam.h
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/erfaversion.c
--rw-r--r--   0 runner    (1001) docker     (127)     4407 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fad03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fae03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/faf03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/faju03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fal03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/falp03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fama03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fame03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fane03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/faom03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fapa03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fasa03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/faur03.c
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fave03.c
--rw-r--r--   0 runner    (1001) docker     (127)    10928 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk425.c
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk45z.c
--rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk524.c
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk52h.c
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk54z.c
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk5hip.c
--rw-r--r--   0 runner    (1001) docker     (127)     6695 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fk5hz.c
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fw2m.c
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/fw2xy.c
--rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/g2icrs.c
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gc2gd.c
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gc2gde.c
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gd2gc.c
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gd2gce.c
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gmst00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5960 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gmst06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gmst82.c
--rw-r--r--   0 runner    (1001) docker     (127)     6063 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gst00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gst00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gst06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gst06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/gst94.c
--rw-r--r--   0 runner    (1001) docker     (127)     6187 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/h2fk5.c
--rw-r--r--   0 runner    (1001) docker     (127)     5936 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/hd2ae.c
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/hd2pa.c
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/hfk5z.c
--rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/icrs2g.c
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ir.c
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/jd2cal.c
--rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/jdcalf.c
--rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ld.c
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ldn.c
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ldsun.c
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/lteceq.c
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ltecm.c
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/lteqec.c
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ltp.c
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ltpb.c
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ltpecl.c
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ltpequ.c
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/meson.build
--rw-r--r--   0 runner    (1001) docker     (127)    23973 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/moon98.c
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/num00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/num00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/num06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/numat.c
--rw-r--r--   0 runner    (1001) docker     (127)   118469 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/nut00a.c
--rw-r--r--   0 runner    (1001) docker     (127)    17696 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/nut00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/nut06a.c
--rw-r--r--   0 runner    (1001) docker     (127)    14956 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/nut80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/nutm80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/obl06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/obl80.c
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/p06e.c
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/p2pv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/p2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     5342 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pap.c
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pas.c
--rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pb06.c
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pdp.c
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pfw06.c
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/plan94.c
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pm.c
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmat00.c
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmat06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmat76.c
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmp.c
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmpx.c
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pmsafe.c
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn.c
--rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn00.c
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     7396 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6854 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pn06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pnm00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pnm00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pnm06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pnm80.c
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pom00.c
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ppp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ppsp.c
--rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pr00.c
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/prec76.c
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pv2p.c
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pv2s.c
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvdpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvm.c
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvmpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvppv.c
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvstar.c
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvtob.c
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvu.c
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvup.c
--rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pvxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/pxp.c
--rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/refco.c
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rm2v.c
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rv2m.c
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rx.c
--rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3977 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rxr.c
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ry.c
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/rz.c
--rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s00.c
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s00b.c
--rw-r--r--   0 runner    (1001) docker     (127)    14065 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s06.c
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s2c.c
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s2p.c
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s2pv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/s2xpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/sepp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/seps.c
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/sp00.c
--rw-r--r--   0 runner    (1001) docker     (127)     9300 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/starpm.c
--rw-r--r--   0 runner    (1001) docker     (127)    10571 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/starpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/sxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/sxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)   242393 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/t_erfa_c.c
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/t_erfa_c_extra.c
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/taitt.c
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/taiut1.c
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/taiutc.c
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tcbtdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tcgtt.c
--rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tdbtcb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tdbtt.c
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tf2a.c
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tf2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tpors.c
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tporv.c
--rw-r--r--   0 runner    (1001) docker     (127)     5106 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tpsts.c
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tpstv.c
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tpxes.c
--rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tpxev.c
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tr.c
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/trxp.c
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/trxpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tttai.c
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tttcg.c
--rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/tttdb.c
--rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ttut1.c
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ut1tai.c
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ut1tt.c
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/ut1utc.c
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/utctai.c
--rw-r--r--   0 runner    (1001) docker     (127)     6051 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/utcut1.c
--rw-r--r--   0 runner    (1001) docker     (127)   132290 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/xy06.c
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/xys00a.c
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/xys00b.c
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/xys06a.c
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/zp.c
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/zpv.c
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-13 19:02:21.000000 pyerfa-2.0.1/liberfa/erfa/src/zr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.112925 pyerfa-2.0.1/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-13 19:02:20.000000 pyerfa-2.0.1/licenses/ERFA.rst
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-13 19:02:20.000000 pyerfa-2.0.1/licenses/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 19:02:52.112925 pyerfa-2.0.1/pyerfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-13 19:02:52.000000 pyerfa-2.0.1/pyerfa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-13 19:02:20.000000 pyerfa-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-10-13 19:02:52.112925 pyerfa-2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2023-10-13 19:02:20.000000 pyerfa-2.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-10-13 19:02:20.000000 pyerfa-2.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.759023 pyerfa-2.0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/README_REPO_IMPORT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/RELEASING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.763023 pyerfa-2.0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.763023 pyerfa-2.0.1.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.767023 pyerfa-2.0.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/docs/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.771023 pyerfa-2.0.1.1/erfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/erfa/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)   738983 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/core.py.templ
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.775023 pyerfa-2.0.1.1/erfa/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20140 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/test_erfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154942 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/tests/test_ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/tests/test_ufunc.py.templ
+-rw-r--r--   0 runner    (1001) docker     (127)   451427 2023-10-19 18:22:30.000000 pyerfa-2.0.1.1/erfa/ufunc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    35932 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/ufunc.c.templ
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36765 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/erfa_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/liberfa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.779023 pyerfa-2.0.1.1/liberfa/erfa/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.git
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.751023 pyerfa-2.0.1.1/liberfa/erfa/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.779023 pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    28654 2023-10-19 18:22:37.000000 pyerfa-2.0.1.1/liberfa/erfa/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6878 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42494 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/aclocal.m4
+-rwxr-xr-x   0 runner    (1001) docker     (127)      116 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/bootstrap.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.787023 pyerfa-2.0.1.1/liberfa/erfa/build-aux/
+-rwxrwxrwx   0 runner    (1001) docker     (127)     7400 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/compile
+-rwxrwxrwx   0 runner    (1001) docker     (127)    49482 2022-01-31 14:43:17.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.guess
+-rwxrwxrwx   0 runner    (1001) docker     (127)    35406 2022-01-31 14:43:17.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.sub
+-rwxrwxrwx   0 runner    (1001) docker     (127)    23568 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/depcomp
+-rwxrwxrwx   0 runner    (1001) docker     (127)    15358 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/install-sh
+-rwxrwxrwx   0 runner    (1001) docker     (127)   327299 2022-03-24 16:13:52.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/ltmain.sh
+-rwxrwxrwx   0 runner    (1001) docker     (127)     6878 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/missing
+-rwxrwxrwx   0 runner    (1001) docker     (127)     4879 2022-03-18 13:09:08.000000 pyerfa-2.0.1.1/liberfa/erfa/build-aux/test-driver
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/config.h.in
+-rwxr-xr-x   0 runner    (1001) docker     (127)   441029 2023-10-19 18:22:36.000000 pyerfa-2.0.1.1/liberfa/erfa/configure
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/configure.ac
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/erfa.pc.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.791023 pyerfa-2.0.1.1/liberfa/erfa/m4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/m4/erfa-numver.m4
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/meson.build
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.899024 pyerfa-2.0.1.1/liberfa/erfa/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.am
+-rw-r--r--   0 runner    (1001) docker     (127)    83996 2023-10-19 18:22:37.000000 pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5054 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/a2af.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/a2tf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ab.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5890 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ae2hd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/af2a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/anp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3596 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/anpm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcg.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcg13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8241 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apci.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8531 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apci13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apco.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12772 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apco13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9633 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apcs13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aper.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aper13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apio.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11440 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/apio13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atcc13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atccq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6825 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atci13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6500 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciqn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6301 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atciqz.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11074 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atco13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atic13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aticq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/aticqn.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10082 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atio13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10095 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atioq.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoc13.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10518 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoi13.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/atoiq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5300 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bi00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bp00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bp06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/bpn2xy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5951 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2i06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ibpn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5738 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ixy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2ixys.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6569 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2t06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2tcio.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2teqx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7359 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2tpe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/c2txy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cal2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/cr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8407 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/d2dtf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/d2tf.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dat.c
+-rw-r--r--   0 runner    (1001) docker     (127)    62193 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dtdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/dtf2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eceq06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ecm06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ee06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10981 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eect00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eform.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eo06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epb2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epj.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epj2jd.c
+-rw-r--r--   0 runner    (1001) docker     (127)   150627 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/epv00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eqec06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/eqeq94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/era00.c
+-rw-r--r--   0 runner    (1001) docker     (127)    27288 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfa.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2697 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.c
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfaextra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5873 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfam.h
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/erfaversion.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fad03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fae03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faf03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faju03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fal03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/falp03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fama03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fame03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fane03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faom03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fapa03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fasa03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/faur03.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fave03.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10928 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk425.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk45z.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10986 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk524.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk52h.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk54z.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk5hip.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6695 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fk5hz.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fw2m.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/fw2xy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6979 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/g2icrs.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gc2gd.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gc2gde.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gd2gc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gd2gce.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5960 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6318 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gmst82.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/gst94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6187 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/h2fk5.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5936 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hd2ae.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hd2pa.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/hfk5z.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/icrs2g.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ir.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/jd2cal.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6231 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/jdcalf.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6265 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ld.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ldn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ldsun.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/lteceq.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltecm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/lteqec.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpecl.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ltpequ.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/meson.build
+-rw-r--r--   0 runner    (1001) docker     (127)    23973 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/moon98.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/num06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/numat.c
+-rw-r--r--   0 runner    (1001) docker     (127)   118469 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    17696 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14956 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nut80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/nutm80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/obl06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/obl80.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p06e.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p2pv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/p2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pap.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pas.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6406 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pb06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pdp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pfw06.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/plan94.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5419 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmat76.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmpx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pmsafe.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7396 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6854 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pn06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5373 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pnm80.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pom00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ppp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ppsp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6429 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pr00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/prec76.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pv2p.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pv2s.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvdpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvm.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvmpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvppv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvstar.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvtob.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvu.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvup.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4404 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pvxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/pxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/refco.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rm2v.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rv2m.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rx.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3860 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rxr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ry.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/rz.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14238 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2p.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2pv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/s2xpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sepp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/seps.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sp00.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9300 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/starpm.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10571 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/starpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/sxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)   242393 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c_extra.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taitt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taiut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6088 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/taiutc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tcbtdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tcgtt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5763 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tdbtcb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tdbtt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tf2a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tf2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7257 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpors.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tporv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5106 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpsts.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpstv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpxes.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tpxev.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tr.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/trxp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/trxpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttcg.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4964 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/tttdb.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4413 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ttut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1tai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1tt.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/ut1utc.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/utctai.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6051 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/utcut1.c
+-rw-r--r--   0 runner    (1001) docker     (127)   132290 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xy06.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5600 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys00a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys00b.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/xys06a.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zp.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zpv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-10-19 18:22:06.000000 pyerfa-2.0.1.1/liberfa/erfa/src/zr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.903024 pyerfa-2.0.1.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/licenses/ERFA.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/licenses/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 18:22:44.903024 pyerfa-2.0.1.1/pyerfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 18:22:44.000000 pyerfa-2.0.1.1/pyerfa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-10-19 18:22:44.907024 pyerfa-2.0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2023-10-19 18:22:05.000000 pyerfa-2.0.1.1/tox.ini
```

### Comparing `pyerfa-2.0.1/.github/workflows/ci_workflows.yml` & `pyerfa-2.0.1.1/.github/workflows/ci_workflows.yml`

 * *Files 3% similar despite different names*

```diff
@@ -125,17 +125,20 @@
       test_extras: test
       test_command: pytest --pyargs erfa
       targets: |
         # Linux wheels
         - cp3*-manylinux_x86_64
         - cp3*-musllinux_x86_64
         - cp3*-manylinux_aarch64
+        - pp39-manylinux_x86_64
         # MacOS X wheels - we deliberately do not build universal2 wheels.
         # Note that the arm64 wheels are not actually tested so we
         # rely on local manual testing of these to make sure they are ok.
         - cp3*macosx_x86_64
         - cp3*macosx_arm64
+        - pp39-macosx_x86_64
         # Windows wheels
         - cp3*win32
         - cp3*win_amd64
+        - pp39-win_amd64
     secrets:
       pypi_token: ${{ secrets.pypi_token }}
```

### Comparing `pyerfa-2.0.1/AUTHORS.rst` & `pyerfa-2.0.1.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/CHANGES.rst` & `pyerfa-2.0.1.1/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-2.0.1 (2023-11-13)
+2.0.1.1 (2023-10-19)
+====================
+- Ensured pyerfa works on PyPy too with the Python limited API. [gh-120]
+- Ensure any non-contigous multi-dimensional inputs are recognized
+  properly, so that, e.g., a non-contiguous matrix is copied as
+  needed before input to the erfa functions. [gh-124]
+
+2.0.1 (2023-10-13)
 ==================
 
 - Bundled liberfa version update to v2.0.1, which is derived from SOFA
-  version 19 (20231011), which has a few bug fixes.
-- Fix dangling pointer leading to unexpected behavior with ``-O3``.
-- PyERFA now only uses the Python limited API.
-- Ensure things work under python 3.12 and recent setuptools-scm.
+  version 19 (20231011), which has a few bug fixes. [gh-118]
+- Fix dangling pointer leading to unexpected behavior with ``-O3``. [gh-104]
+- PyERFA now only uses the Python limited API. [gh-94]
+- Ensure things work under python 3.12 and recent setuptools-scm. [gh-113]
 
 2.0.0.3 (2023-03-22)
 ====================
 
 - Ensure minimum numpy version of 1.17 continues to work (for astropy LTS).
 
 2.0.0.2 (2023-03-19)
```

### Comparing `pyerfa-2.0.1/LICENSE.rst` & `pyerfa-2.0.1.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/MANIFEST.in` & `pyerfa-2.0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/PKG-INFO` & `pyerfa-2.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerfa
-Version: 2.0.1
+Version: 2.0.1.1
 Summary: Python bindings for ERFA
 Home-page: https://github.com/liberfa/pyerfa
 Author: The PyERFA Developers
 License: BSD 3-Clause License
 Keywords: astronomy,astrophysics,cosmology,space,science,coordinate
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyerfa-2.0.1/README.rst` & `pyerfa-2.0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/README_REPO_IMPORT.rst` & `pyerfa-2.0.1.1/README_REPO_IMPORT.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/RELEASING.rst` & `pyerfa-2.0.1.1/RELEASING.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/docs/Makefile` & `pyerfa-2.0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/docs/_templates/layout.html` & `pyerfa-2.0.1.1/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/docs/conf.py` & `pyerfa-2.0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/docs/make.bat` & `pyerfa-2.0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/core.py` & `pyerfa-2.0.1.1/erfa/core.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/core.py.templ` & `pyerfa-2.0.1.1/erfa/core.py.templ`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/helpers.py` & `pyerfa-2.0.1.1/erfa/helpers.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/tests/helper.py` & `pyerfa-2.0.1.1/erfa/tests/helper.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/tests/test_erfa.py` & `pyerfa-2.0.1.1/erfa/tests/test_erfa.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,27 @@
 
 
 def test_float32_input():
     # Regression test for gh-8615
     xyz = np.array([[1, 0, 0], [0.9, 0.1, 0]])
     out64 = erfa.p2s(xyz)
     out32 = erfa.p2s(xyz.astype('f4'))
-    np.testing.assert_allclose(out32, out64, rtol=1.e-5)
+    assert_allclose(out32, out64, rtol=1.e-5)
+
+
+def test_non_contiguous_matrix():
+    # Regression test for gh-123 (astropy gh-15503)
+    matrix = np.array([[1, 0, 0, 5],
+                       [0, 1, 0, 6],
+                       [0, 0, 1, 7]], dtype='float')[:, :3]
+    vector = np.array([1., 2., 3.])
+    assert_array_equal(matrix, np.eye(3))
+    conv = erfa.rxp(matrix, vector)
+    assert_array_equal(matrix @ vector, vector)
+    assert_array_equal(conv, vector)
 
 
 class TestAstromNotInplace:
     def setup_method(self):
         self.mjd_array = np.array(
             [58827.15925499, 58827.15925499, 58827.15925499,
              58827.15925499, 58827.15925499])
```

### Comparing `pyerfa-2.0.1/erfa/tests/test_ufunc.py` & `pyerfa-2.0.1.1/erfa/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/tests/test_ufunc.py.templ` & `pyerfa-2.0.1.1/erfa/tests/test_ufunc.py.templ`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa/ufunc.c` & `pyerfa-2.0.1.1/erfa/ufunc.c`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 // On gcc<10 we can run into the following:
 //
 //   error: dereferencing pointer to incomplete type 'PyTypeObject'
 //
 // As mentioned in https://github.com/numpy/numpy/issues/16970,
 // the workaround is to define a fake _typeobject struct.
 
-struct _typeobject {
+#ifndef PYPY_VERSION
+typedef struct _typeobject {
     int dummy;
 };
+#endif
 
 #define MODULE_DOCSTRING \
     "Ufunc wrappers of the ERFA routines.\n\n" \
     "These ufuncs vectorize the ERFA functions assuming structured dtypes\n" \
     "for vector and matrix arguments. Status codes are vectors as well.\n" \
     "Python wrappers are also provided, which convert between\n" \
     "trailing dimensions and structured dtypes where necessary,\n" \
@@ -2607,23 +2609,23 @@
     double (*_rb)[3][3] = &b_rb;
     double b_rp[3][3];
     double (*_rp)[3][3] = &b_rp;
     double b_rbp[3][3];
     double (*_rbp)[3][3] = &b_rbp;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rb += s_rb, rp += s_rp, rbp += s_rbp) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rb) {
             _rb = ((double (*)[3][3])rb);
@@ -2668,23 +2670,23 @@
     double (*_rb)[3][3] = &b_rb;
     double b_rp[3][3];
     double (*_rp)[3][3] = &b_rp;
     double b_rbp[3][3];
     double (*_rbp)[3][3] = &b_rbp;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rb += s_rb, rp += s_rp, rbp += s_rbp) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rb) {
             _rb = ((double (*)[3][3])rb);
@@ -2721,15 +2723,15 @@
     npy_intp s_y = *steps++;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     double (*_x);
     double (*_y);
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, rbpn += s_rbpn, x += s_x, y += s_y) {
         if (copy_rbpn) {
             copy_to_double33(rbpn, is_rbpn0, is_rbpn1, *_rbpn);
         }
         else {
@@ -2754,15 +2756,15 @@
     npy_intp s_rc2i = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rc2i += s_rc2i) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rc2i) {
             _rc2i = ((double (*)[3][3])rc2i);
@@ -2787,15 +2789,15 @@
     npy_intp s_rc2i = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rc2i += s_rc2i) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rc2i) {
             _rc2i = ((double (*)[3][3])rc2i);
@@ -2820,15 +2822,15 @@
     npy_intp s_rc2i = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rc2i += s_rc2i) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rc2i) {
             _rc2i = ((double (*)[3][3])rc2i);
@@ -2857,19 +2859,19 @@
     double (*_date2);
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbpn += s_rbpn, rc2i += s_rc2i) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (copy_rbpn) {
             copy_to_double33(rbpn, is_rbpn0, is_rbpn1, *_rbpn);
@@ -2906,15 +2908,15 @@
     double (*_date2);
     double (*_x);
     double (*_y);
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, x += s_x, y += s_y, rc2i += s_rc2i) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _x = ((double (*))x);
         _y = ((double (*))y);
@@ -2944,15 +2946,15 @@
     double (*_x);
     double (*_y);
     double (*_s);
     double b_rc2i[3][3];
     double (*_rc2i)[3][3] = &b_rc2i;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, x += s_x, y += s_y, s += s_s, rc2i += s_rc2i) {
         _x = ((double (*))x);
         _y = ((double (*))y);
         _s = ((double (*))s);
         if (!copy_rc2i) {
@@ -2990,15 +2992,15 @@
     double (*_utb);
     double (*_xp);
     double (*_yp);
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, tta += s_tta, ttb += s_ttb, uta += s_uta, utb += s_utb, xp += s_xp, yp += s_yp, rc2t += s_rc2t) {
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
@@ -3039,15 +3041,15 @@
     double (*_utb);
     double (*_xp);
     double (*_yp);
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, tta += s_tta, ttb += s_ttb, uta += s_uta, utb += s_utb, xp += s_xp, yp += s_yp, rc2t += s_rc2t) {
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
@@ -3088,15 +3090,15 @@
     double (*_utb);
     double (*_xp);
     double (*_yp);
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, tta += s_tta, ttb += s_ttb, uta += s_uta, utb += s_utb, xp += s_xp, yp += s_yp, rc2t += s_rc2t) {
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
@@ -3130,23 +3132,23 @@
     double (*_era);
     double b_rpom[3][3];
     double (*_rpom)[3][3] = &b_rpom;
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2i0 = *steps++;
     npy_intp is_rc2i1 = *steps++;
-    int copy_rc2i = (is_rc2i1 != sizeof(double) &&
+    int copy_rc2i = (is_rc2i1 != sizeof(double) ||
               is_rc2i0 != 3 * sizeof(double));
     npy_intp is_rpom0 = *steps++;
     npy_intp is_rpom1 = *steps++;
-    int copy_rpom = (is_rpom1 != sizeof(double) &&
+    int copy_rpom = (is_rpom1 != sizeof(double) ||
               is_rpom0 != 3 * sizeof(double));
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, rc2i += s_rc2i, era += s_era, rpom += s_rpom, rc2t += s_rc2t) {
         if (copy_rc2i) {
             copy_to_double33(rc2i, is_rc2i0, is_rc2i1, *_rc2i);
         }
         else {
@@ -3187,23 +3189,23 @@
     double (*_gst);
     double b_rpom[3][3];
     double (*_rpom)[3][3] = &b_rpom;
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     npy_intp is_rpom0 = *steps++;
     npy_intp is_rpom1 = *steps++;
-    int copy_rpom = (is_rpom1 != sizeof(double) &&
+    int copy_rpom = (is_rpom1 != sizeof(double) ||
               is_rpom0 != 3 * sizeof(double));
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, rbpn += s_rbpn, gst += s_gst, rpom += s_rpom, rc2t += s_rc2t) {
         if (copy_rbpn) {
             copy_to_double33(rbpn, is_rbpn0, is_rbpn1, *_rbpn);
         }
         else {
@@ -3257,15 +3259,15 @@
     double (*_deps);
     double (*_xp);
     double (*_yp);
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, tta += s_tta, ttb += s_ttb, uta += s_uta, utb += s_utb, dpsi += s_dpsi, deps += s_deps, xp += s_xp, yp += s_yp, rc2t += s_rc2t) {
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
@@ -3314,15 +3316,15 @@
     double (*_y);
     double (*_xp);
     double (*_yp);
     double b_rc2t[3][3];
     double (*_rc2t)[3][3] = &b_rc2t;
     npy_intp is_rc2t0 = *steps++;
     npy_intp is_rc2t1 = *steps++;
-    int copy_rc2t = (is_rc2t1 != sizeof(double) &&
+    int copy_rc2t = (is_rc2t1 != sizeof(double) ||
               is_rc2t0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, tta += s_tta, ttb += s_ttb, uta += s_uta, utb += s_utb, x += s_x, y += s_y, xp += s_xp, yp += s_yp, rc2t += s_rc2t) {
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
@@ -3376,15 +3378,15 @@
     npy_intp s_c_retval = *steps++;
     double b_rnpb[3][3];
     double (*_rnpb)[3][3] = &b_rnpb;
     double (*_s);
     double _c_retval;
     npy_intp is_rnpb0 = *steps++;
     npy_intp is_rnpb1 = *steps++;
-    int copy_rnpb = (is_rnpb1 != sizeof(double) &&
+    int copy_rnpb = (is_rnpb1 != sizeof(double) ||
               is_rnpb0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, rnpb += s_rnpb, s += s_s, c_retval += s_c_retval) {
         if (copy_rnpb) {
             copy_to_double33(rnpb, is_rnpb0, is_rnpb1, *_rnpb);
         }
         else {
@@ -3415,15 +3417,15 @@
     double (*_phib);
     double (*_psi);
     double (*_eps);
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, gamb += s_gamb, phib += s_phib, psi += s_psi, eps += s_eps, r += s_r) {
         _gamb = ((double (*))gamb);
         _phib = ((double (*))phib);
         _psi = ((double (*))psi);
         _eps = ((double (*))eps);
@@ -3482,15 +3484,15 @@
     char *rp = *args++;
     npy_intp s_rp = *steps++;
     double (*_epj);
     double b_rp[3][3];
     double (*_rp)[3][3] = &b_rp;
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, epj += s_epj, rp += s_rp) {
         _epj = ((double (*))epj);
         if (!copy_rp) {
             _rp = ((double (*)[3][3])rp);
         }
@@ -3511,15 +3513,15 @@
     char *rpb = *args++;
     npy_intp s_rpb = *steps++;
     double (*_epj);
     double b_rpb[3][3];
     double (*_rpb)[3][3] = &b_rpb;
     npy_intp is_rpb0 = *steps++;
     npy_intp is_rpb1 = *steps++;
-    int copy_rpb = (is_rpb1 != sizeof(double) &&
+    int copy_rpb = (is_rpb1 != sizeof(double) ||
               is_rpb0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, epj += s_epj, rpb += s_rpb) {
         _epj = ((double (*))epj);
         if (!copy_rpb) {
             _rpb = ((double (*)[3][3])rpb);
         }
@@ -3597,15 +3599,15 @@
     npy_intp s_rmatn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatn[3][3];
     double (*_rmatn)[3][3] = &b_rmatn;
     npy_intp is_rmatn0 = *steps++;
     npy_intp is_rmatn1 = *steps++;
-    int copy_rmatn = (is_rmatn1 != sizeof(double) &&
+    int copy_rmatn = (is_rmatn1 != sizeof(double) ||
               is_rmatn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatn += s_rmatn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatn) {
             _rmatn = ((double (*)[3][3])rmatn);
@@ -3630,15 +3632,15 @@
     npy_intp s_rmatn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatn[3][3];
     double (*_rmatn)[3][3] = &b_rmatn;
     npy_intp is_rmatn0 = *steps++;
     npy_intp is_rmatn1 = *steps++;
-    int copy_rmatn = (is_rmatn1 != sizeof(double) &&
+    int copy_rmatn = (is_rmatn1 != sizeof(double) ||
               is_rmatn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatn += s_rmatn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatn) {
             _rmatn = ((double (*)[3][3])rmatn);
@@ -3663,15 +3665,15 @@
     npy_intp s_rmatn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatn[3][3];
     double (*_rmatn)[3][3] = &b_rmatn;
     npy_intp is_rmatn0 = *steps++;
     npy_intp is_rmatn1 = *steps++;
-    int copy_rmatn = (is_rmatn1 != sizeof(double) &&
+    int copy_rmatn = (is_rmatn1 != sizeof(double) ||
               is_rmatn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatn += s_rmatn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatn) {
             _rmatn = ((double (*)[3][3])rmatn);
@@ -3699,15 +3701,15 @@
     double (*_epsa);
     double (*_dpsi);
     double (*_deps);
     double b_rmatn[3][3];
     double (*_rmatn)[3][3] = &b_rmatn;
     npy_intp is_rmatn0 = *steps++;
     npy_intp is_rmatn1 = *steps++;
-    int copy_rmatn = (is_rmatn1 != sizeof(double) &&
+    int copy_rmatn = (is_rmatn1 != sizeof(double) ||
               is_rmatn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, epsa += s_epsa, dpsi += s_dpsi, deps += s_deps, rmatn += s_rmatn) {
         _epsa = ((double (*))epsa);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
         if (!copy_rmatn) {
@@ -3841,15 +3843,15 @@
     npy_intp s_rmatn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatn[3][3];
     double (*_rmatn)[3][3] = &b_rmatn;
     npy_intp is_rmatn0 = *steps++;
     npy_intp is_rmatn1 = *steps++;
-    int copy_rmatn = (is_rmatn1 != sizeof(double) &&
+    int copy_rmatn = (is_rmatn1 != sizeof(double) ||
               is_rmatn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatn += s_rmatn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatn) {
             _rmatn = ((double (*)[3][3])rmatn);
@@ -4069,15 +4071,15 @@
     npy_intp s_rbp = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rbp[3][3];
     double (*_rbp)[3][3] = &b_rbp;
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbp += s_rbp) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rbp) {
             _rbp = ((double (*)[3][3])rbp);
@@ -4102,15 +4104,15 @@
     npy_intp s_rbp = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rbp[3][3];
     double (*_rbp)[3][3] = &b_rbp;
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbp += s_rbp) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rbp) {
             _rbp = ((double (*)[3][3])rbp);
@@ -4135,15 +4137,15 @@
     npy_intp s_rmatp = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatp[3][3];
     double (*_rmatp)[3][3] = &b_rmatp;
     npy_intp is_rmatp0 = *steps++;
     npy_intp is_rmatp1 = *steps++;
-    int copy_rmatp = (is_rmatp1 != sizeof(double) &&
+    int copy_rmatp = (is_rmatp1 != sizeof(double) ||
               is_rmatp0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatp += s_rmatp) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatp) {
             _rmatp = ((double (*)[3][3])rmatp);
@@ -4193,31 +4195,31 @@
     double (*_rbp)[3][3] = &b_rbp;
     double b_rn[3][3];
     double (*_rn)[3][3] = &b_rn;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     npy_intp is_rn0 = *steps++;
     npy_intp is_rn1 = *steps++;
-    int copy_rn = (is_rn1 != sizeof(double) &&
+    int copy_rn = (is_rn1 != sizeof(double) ||
               is_rn0 != 3 * sizeof(double));
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, dpsi += s_dpsi, deps += s_deps, epsa += s_epsa, rb += s_rb, rp += s_rp, rbp += s_rbp, rn += s_rn, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
@@ -4294,31 +4296,31 @@
     double (*_rbp)[3][3] = &b_rbp;
     double b_rn[3][3];
     double (*_rn)[3][3] = &b_rn;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     npy_intp is_rn0 = *steps++;
     npy_intp is_rn1 = *steps++;
-    int copy_rn = (is_rn1 != sizeof(double) &&
+    int copy_rn = (is_rn1 != sizeof(double) ||
               is_rn0 != 3 * sizeof(double));
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, dpsi += s_dpsi, deps += s_deps, epsa += s_epsa, rb += s_rb, rp += s_rp, rbp += s_rbp, rn += s_rn, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
@@ -4395,31 +4397,31 @@
     double (*_rbp)[3][3] = &b_rbp;
     double b_rn[3][3];
     double (*_rn)[3][3] = &b_rn;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     npy_intp is_rn0 = *steps++;
     npy_intp is_rn1 = *steps++;
-    int copy_rn = (is_rn1 != sizeof(double) &&
+    int copy_rn = (is_rn1 != sizeof(double) ||
               is_rn0 != 3 * sizeof(double));
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, dpsi += s_dpsi, deps += s_deps, epsa += s_epsa, rb += s_rb, rp += s_rp, rbp += s_rbp, rn += s_rn, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
@@ -4496,31 +4498,31 @@
     double (*_rbp)[3][3] = &b_rbp;
     double b_rn[3][3];
     double (*_rn)[3][3] = &b_rn;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     npy_intp is_rn0 = *steps++;
     npy_intp is_rn1 = *steps++;
-    int copy_rn = (is_rn1 != sizeof(double) &&
+    int copy_rn = (is_rn1 != sizeof(double) ||
               is_rn0 != 3 * sizeof(double));
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, dpsi += s_dpsi, deps += s_deps, epsa += s_epsa, rb += s_rb, rp += s_rp, rbp += s_rbp, rn += s_rn, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
@@ -4597,31 +4599,31 @@
     double (*_rbp)[3][3] = &b_rbp;
     double b_rn[3][3];
     double (*_rn)[3][3] = &b_rn;
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rb0 = *steps++;
     npy_intp is_rb1 = *steps++;
-    int copy_rb = (is_rb1 != sizeof(double) &&
+    int copy_rb = (is_rb1 != sizeof(double) ||
               is_rb0 != 3 * sizeof(double));
     npy_intp is_rp0 = *steps++;
     npy_intp is_rp1 = *steps++;
-    int copy_rp = (is_rp1 != sizeof(double) &&
+    int copy_rp = (is_rp1 != sizeof(double) ||
               is_rp0 != 3 * sizeof(double));
     npy_intp is_rbp0 = *steps++;
     npy_intp is_rbp1 = *steps++;
-    int copy_rbp = (is_rbp1 != sizeof(double) &&
+    int copy_rbp = (is_rbp1 != sizeof(double) ||
               is_rbp0 != 3 * sizeof(double));
     npy_intp is_rn0 = *steps++;
     npy_intp is_rn1 = *steps++;
-    int copy_rn = (is_rn1 != sizeof(double) &&
+    int copy_rn = (is_rn1 != sizeof(double) ||
               is_rn0 != 3 * sizeof(double));
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, dpsi += s_dpsi, deps += s_deps, epsa += s_epsa, rb += s_rb, rp += s_rp, rbp += s_rbp, rn += s_rn, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         _dpsi = ((double (*))dpsi);
         _deps = ((double (*))deps);
@@ -4673,15 +4675,15 @@
     npy_intp s_rbpn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rbpn) {
             _rbpn = ((double (*)[3][3])rbpn);
@@ -4706,15 +4708,15 @@
     npy_intp s_rbpn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rbpn) {
             _rbpn = ((double (*)[3][3])rbpn);
@@ -4739,15 +4741,15 @@
     npy_intp s_rbpn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rbpn[3][3];
     double (*_rbpn)[3][3] = &b_rbpn;
     npy_intp is_rbpn0 = *steps++;
     npy_intp is_rbpn1 = *steps++;
-    int copy_rbpn = (is_rbpn1 != sizeof(double) &&
+    int copy_rbpn = (is_rbpn1 != sizeof(double) ||
               is_rbpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rbpn += s_rbpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rbpn) {
             _rbpn = ((double (*)[3][3])rbpn);
@@ -4772,15 +4774,15 @@
     npy_intp s_rmatpn = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rmatpn[3][3];
     double (*_rmatpn)[3][3] = &b_rmatpn;
     npy_intp is_rmatpn0 = *steps++;
     npy_intp is_rmatpn1 = *steps++;
-    int copy_rmatpn = (is_rmatpn1 != sizeof(double) &&
+    int copy_rmatpn = (is_rmatpn1 != sizeof(double) ||
               is_rmatpn0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rmatpn += s_rmatpn) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rmatpn) {
             _rmatpn = ((double (*)[3][3])rmatpn);
@@ -4808,15 +4810,15 @@
     double (*_xp);
     double (*_yp);
     double (*_sp);
     double b_rpom[3][3];
     double (*_rpom)[3][3] = &b_rpom;
     npy_intp is_rpom0 = *steps++;
     npy_intp is_rpom1 = *steps++;
-    int copy_rpom = (is_rpom1 != sizeof(double) &&
+    int copy_rpom = (is_rpom1 != sizeof(double) ||
               is_rpom0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, xp += s_xp, yp += s_yp, sp += s_sp, rpom += s_rpom) {
         _xp = ((double (*))xp);
         _yp = ((double (*))yp);
         _sp = ((double (*))sp);
         if (!copy_rpom) {
@@ -5499,15 +5501,15 @@
     double (*_tta);
     double (*_ttb);
     double b_rnpb[3][3];
     double (*_rnpb)[3][3] = &b_rnpb;
     double _c_retval;
     npy_intp is_rnpb0 = *steps++;
     npy_intp is_rnpb1 = *steps++;
-    int copy_rnpb = (is_rnpb1 != sizeof(double) &&
+    int copy_rnpb = (is_rnpb1 != sizeof(double) ||
               is_rnpb0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, uta += s_uta, utb += s_utb, tta += s_tta, ttb += s_ttb, rnpb += s_rnpb, c_retval += s_c_retval) {
         _uta = ((double (*))uta);
         _utb = ((double (*))utb);
         _tta = ((double (*))tta);
         _ttb = ((double (*))ttb);
@@ -5920,15 +5922,15 @@
     npy_intp s_s5h = *steps++;
     double b_r5h[3][3];
     double (*_r5h)[3][3] = &b_r5h;
     double b_s5h[3];
     double (*_s5h)[3] = &b_s5h;
     npy_intp is_r5h0 = *steps++;
     npy_intp is_r5h1 = *steps++;
-    int copy_r5h = (is_r5h1 != sizeof(double) &&
+    int copy_r5h = (is_r5h1 != sizeof(double) ||
               is_r5h0 != 3 * sizeof(double));
     npy_intp is_s5h0 = *steps++;
     int copy_s5h = (is_s5h0 != sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r5h += s_r5h, s5h += s_s5h) {
         if (!copy_r5h) {
             _r5h = ((double (*)[3][3])r5h);
@@ -6210,15 +6212,15 @@
     npy_intp s_rm = *steps++;
     double (*_date1);
     double (*_date2);
     double b_rm[3][3];
     double (*_rm)[3][3] = &b_rm;
     npy_intp is_rm0 = *steps++;
     npy_intp is_rm1 = *steps++;
-    int copy_rm = (is_rm1 != sizeof(double) &&
+    int copy_rm = (is_rm1 != sizeof(double) ||
               is_rm0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, date1 += s_date1, date2 += s_date2, rm += s_rm) {
         _date1 = ((double (*))date1);
         _date2 = ((double (*))date2);
         if (!copy_rm) {
             _rm = ((double (*)[3][3])rm);
@@ -6306,15 +6308,15 @@
     char *rm = *args++;
     npy_intp s_rm = *steps++;
     double (*_epj);
     double b_rm[3][3];
     double (*_rm)[3][3] = &b_rm;
     npy_intp is_rm0 = *steps++;
     npy_intp is_rm1 = *steps++;
-    int copy_rm = (is_rm1 != sizeof(double) &&
+    int copy_rm = (is_rm1 != sizeof(double) ||
               is_rm0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, epj += s_epj, rm += s_rm) {
         _epj = ((double (*))epj);
         if (!copy_rm) {
             _rm = ((double (*)[3][3])rm);
         }
@@ -7912,19 +7914,19 @@
     char *r = *args++;
     npy_intp s_r = *steps++;
     double (*_phi);
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r_in0 = *steps++;
     npy_intp is_r_in1 = *steps++;
-    int copy_r_in = (is_r_in1 != sizeof(double) &&
+    int copy_r_in = (is_r_in1 != sizeof(double) ||
               is_r_in0 != 3 * sizeof(double));
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, phi += s_phi, r += s_r, r_in += s_r_in) {
         _phi = ((double (*))phi);
         if (!copy_r) {
             _r = ((double (*)[3][3])r);
         }
@@ -7950,19 +7952,19 @@
     char *r = *args++;
     npy_intp s_r = *steps++;
     double (*_theta);
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r_in0 = *steps++;
     npy_intp is_r_in1 = *steps++;
-    int copy_r_in = (is_r_in1 != sizeof(double) &&
+    int copy_r_in = (is_r_in1 != sizeof(double) ||
               is_r_in0 != 3 * sizeof(double));
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, theta += s_theta, r += s_r, r_in += s_r_in) {
         _theta = ((double (*))theta);
         if (!copy_r) {
             _r = ((double (*)[3][3])r);
         }
@@ -7988,19 +7990,19 @@
     char *r = *args++;
     npy_intp s_r = *steps++;
     double (*_psi);
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r_in0 = *steps++;
     npy_intp is_r_in1 = *steps++;
-    int copy_r_in = (is_r_in1 != sizeof(double) &&
+    int copy_r_in = (is_r_in1 != sizeof(double) ||
               is_r_in0 != 3 * sizeof(double));
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, psi += s_psi, r += s_r, r_in += s_r_in) {
         _psi = ((double (*))psi);
         if (!copy_r) {
             _r = ((double (*)[3][3])r);
         }
@@ -8079,19 +8081,19 @@
     npy_intp s_c = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     double b_c[3][3];
     double (*_c)[3][3] = &b_c;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     npy_intp is_c0 = *steps++;
     npy_intp is_c1 = *steps++;
-    int copy_c = (is_c1 != sizeof(double) &&
+    int copy_c = (is_c1 != sizeof(double) ||
               is_c0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, c += s_c) {
         if (copy_r) {
             copy_to_double33(r, is_r0, is_r1, *_r);
         }
         else {
@@ -8168,15 +8170,15 @@
     npy_intp n_o = *dimensions++;
     char *r = *args++;
     npy_intp s_r = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r) {
         if (!copy_r) {
             _r = ((double (*)[3][3])r);
         }
         eraIr(*_r);
@@ -8231,15 +8233,15 @@
     npy_intp n_o = *dimensions++;
     char *r = *args++;
     npy_intp s_r = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r) {
         if (!copy_r) {
             _r = ((double (*)[3][3])r);
         }
         eraZr(*_r);
@@ -8264,23 +8266,23 @@
     double (*_a)[3][3] = &b_a;
     double b_b[3][3];
     double (*_b)[3][3] = &b_b;
     double b_atb[3][3];
     double (*_atb)[3][3] = &b_atb;
     npy_intp is_a0 = *steps++;
     npy_intp is_a1 = *steps++;
-    int copy_a = (is_a1 != sizeof(double) &&
+    int copy_a = (is_a1 != sizeof(double) ||
               is_a0 != 3 * sizeof(double));
     npy_intp is_b0 = *steps++;
     npy_intp is_b1 = *steps++;
-    int copy_b = (is_b1 != sizeof(double) &&
+    int copy_b = (is_b1 != sizeof(double) ||
               is_b0 != 3 * sizeof(double));
     npy_intp is_atb0 = *steps++;
     npy_intp is_atb1 = *steps++;
-    int copy_atb = (is_atb1 != sizeof(double) &&
+    int copy_atb = (is_atb1 != sizeof(double) ||
               is_atb0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, a += s_a, b += s_b, atb += s_atb) {
         if (copy_a) {
             copy_to_double33(a, is_a0, is_a1, *_a);
         }
         else {
@@ -8313,19 +8315,19 @@
     npy_intp s_rt = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     double b_rt[3][3];
     double (*_rt)[3][3] = &b_rt;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     npy_intp is_rt0 = *steps++;
     npy_intp is_rt1 = *steps++;
-    int copy_rt = (is_rt1 != sizeof(double) &&
+    int copy_rt = (is_rt1 != sizeof(double) ||
               is_rt0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, rt += s_rt) {
         if (copy_r) {
             copy_to_double33(r, is_r0, is_r1, *_r);
         }
         else {
@@ -8356,15 +8358,15 @@
     double (*_r)[3][3] = &b_r;
     double b_p[3];
     double (*_p)[3] = &b_p;
     double b_rp[3];
     double (*_rp)[3] = &b_rp;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     npy_intp is_p0 = *steps++;
     int copy_p = (is_p0 != sizeof(double));
     npy_intp is_rp0 = *steps++;
     int copy_rp = (is_rp0 != sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, p += s_p, rp += s_rp) {
@@ -8403,15 +8405,15 @@
     npy_intp s_rpv = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     double (*_pv)[2][3];
     double (*_rpv)[2][3];
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, pv += s_pv, rpv += s_rpv) {
         if (copy_r) {
             copy_to_double33(r, is_r0, is_r1, *_r);
         }
         else {
@@ -8438,15 +8440,15 @@
     double (*_r)[3][3] = &b_r;
     double b_p[3];
     double (*_p)[3] = &b_p;
     double b_trp[3];
     double (*_trp)[3] = &b_trp;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     npy_intp is_p0 = *steps++;
     int copy_p = (is_p0 != sizeof(double));
     npy_intp is_trp0 = *steps++;
     int copy_trp = (is_trp0 != sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, p += s_p, trp += s_trp) {
@@ -8485,15 +8487,15 @@
     npy_intp s_trpv = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     double (*_pv)[2][3];
     double (*_trpv)[2][3];
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, pv += s_pv, trpv += s_trpv) {
         if (copy_r) {
             copy_to_double33(r, is_r0, is_r1, *_r);
         }
         else {
@@ -8516,15 +8518,15 @@
     npy_intp s_w = *steps++;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     double b_w[3];
     double (*_w)[3] = &b_w;
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     npy_intp is_w0 = *steps++;
     int copy_w = (is_w0 != sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, r += s_r, w += s_w) {
         if (copy_r) {
             copy_to_double33(r, is_r0, is_r1, *_r);
@@ -8555,15 +8557,15 @@
     double (*_w)[3] = &b_w;
     double b_r[3][3];
     double (*_r)[3][3] = &b_r;
     npy_intp is_w0 = *steps++;
     int copy_w = (is_w0 != sizeof(double));
     npy_intp is_r0 = *steps++;
     npy_intp is_r1 = *steps++;
-    int copy_r = (is_r1 != sizeof(double) &&
+    int copy_r = (is_r1 != sizeof(double) ||
               is_r0 != 3 * sizeof(double));
     for (i_o = 0; i_o < n_o;
          i_o++, w += s_w, r += s_r) {
         if (copy_w) {
             copy_to_double3(w, is_w0, *_w);
         }
         else {
```

### Comparing `pyerfa-2.0.1/erfa/ufunc.c.templ` & `pyerfa-2.0.1.1/erfa/ufunc.c.templ`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 // On gcc<10 we can run into the following:
 //
 //   error: dereferencing pointer to incomplete type 'PyTypeObject'
 //
 // As mentioned in https://github.com/numpy/numpy/issues/16970,
 // the workaround is to define a fake _typeobject struct.
 
-struct _typeobject {
+#ifndef PYPY_VERSION
+typedef struct _typeobject {
     int dummy;
 };
+#endif
 
 #define MODULE_DOCSTRING \
     "Ufunc wrappers of the ERFA routines.\n\n" \
     "These ufuncs vectorize the ERFA functions assuming structured dtypes\n" \
     "for vector and matrix arguments. Status codes are vectors as well.\n" \
     "Python wrappers are also provided, which convert between\n" \
     "trailing dimensions and structured dtypes where necessary,\n" \
@@ -140,15 +142,15 @@
   {%- for i in range(arg.ndim or 1) %}
     npy_intp is_{{ arg_name }}{{ i }} = *steps++;
   {%- endfor %}
   {#- /* copy should be made if buffer not contiguous;
          note: one can only have 1 or 2 dimensions */ #}
   {%- if arg.ndim == 2 %}
     int copy_{{ arg_name
-        }} = (is_{{ arg_name }}1 != sizeof({{ arg.ctype }}) &&
+        }} = (is_{{ arg_name }}1 != sizeof({{ arg.ctype }}) ||
               is_{{ arg_name }}0 != {{ arg.shape[1] }} * sizeof({{ arg.ctype }}));
   {%- else %}
     int copy_{{ arg_name }} = (is_{{ arg_name }}0 != sizeof({{ arg.ctype }}));
   {%- endif %}
 {%- endmacro %}
 
 {%- for func in funcs %}
```

### Comparing `pyerfa-2.0.1/erfa/version.py` & `pyerfa-2.0.1.1/erfa/version.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/erfa_generator.py` & `pyerfa-2.0.1.1/erfa_generator.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/.github/workflows/ci_workflows.yml` & `pyerfa-2.0.1.1/liberfa/erfa/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/INFO` & `pyerfa-2.0.1.1/liberfa/erfa/INFO`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/LICENSE` & `pyerfa-2.0.1.1/liberfa/erfa/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/Makefile.in` & `pyerfa-2.0.1.1/liberfa/erfa/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/README.rst` & `pyerfa-2.0.1.1/liberfa/erfa/README.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/RELEASE.rst` & `pyerfa-2.0.1.1/liberfa/erfa/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/aclocal.m4` & `pyerfa-2.0.1.1/liberfa/erfa/aclocal.m4`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/compile` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/compile`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/config.guess` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.guess`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/config.sub` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/config.sub`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/depcomp` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/depcomp`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/install-sh` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/install-sh`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/ltmain.sh` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/ltmain.sh`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/missing` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/missing`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/build-aux/test-driver` & `pyerfa-2.0.1.1/liberfa/erfa/build-aux/test-driver`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/config.h.in` & `pyerfa-2.0.1.1/liberfa/erfa/config.h.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/configure` & `pyerfa-2.0.1.1/liberfa/erfa/configure`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/configure.ac` & `pyerfa-2.0.1.1/liberfa/erfa/configure.ac`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/m4/erfa-numver.m4` & `pyerfa-2.0.1.1/liberfa/erfa/m4/erfa-numver.m4`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/meson.build` & `pyerfa-2.0.1.1/liberfa/erfa/meson.build`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/Makefile.am` & `pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.am`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/Makefile.in` & `pyerfa-2.0.1.1/liberfa/erfa/src/Makefile.in`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/a2af.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/a2af.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/a2tf.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/a2tf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ab.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ab.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ae2hd.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ae2hd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/af2a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/af2a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/anp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/anp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/anpm.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/anpm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apcg.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apcg.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apcg13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apcg13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apci.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apci.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apci13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apci13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apco.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apco.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apco13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apco13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apcs.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apcs.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apcs13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apcs13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/aper.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/aper.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/aper13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/aper13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apio.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apio.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/apio13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/apio13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atcc13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atcc13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atccq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atccq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atci13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atci13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atciq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atciq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atciqn.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atciqn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atciqz.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atciqz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atco13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atco13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atic13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atic13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/aticq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/aticq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/aticqn.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/aticqn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atio13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atio13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atioq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atioq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atoc13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atoc13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atoi13.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atoi13.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/atoiq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/atoiq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/bi00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/bi00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/bp00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/bp00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/bp06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/bp06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/bpn2xy.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/bpn2xy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2i00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2i00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2i00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2i00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2i06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2i06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2ibpn.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2ibpn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2ixy.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2ixy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2ixys.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2ixys.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2s.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2t00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2t00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2t00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2t00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2t06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2t06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2tcio.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2tcio.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2teqx.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2teqx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2tpe.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2tpe.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/c2txy.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/c2txy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/cal2jd.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/cal2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/cp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/cp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/cpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/cpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/cr.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/cr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/d2dtf.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/d2dtf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/d2tf.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/d2tf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/dat.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/dat.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/dtdb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/dtdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/dtf2d.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/dtf2d.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eceq06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eceq06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ecm06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ecm06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ee00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ee00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ee00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ee00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ee00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ee00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ee06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ee06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eect00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eect00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eform.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eform.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eo06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eo06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eors.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eors.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/epb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/epb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/epb2jd.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/epb2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/epj.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/epj.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/epj2jd.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/epj2jd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/epv00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/epv00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eqec06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eqec06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/eqeq94.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/eqeq94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/era00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/era00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfa.h` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfa.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfadatextra.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfadatextra.h` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfadatextra.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfaextra.h` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfaextra.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfam.h` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfam.h`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/erfaversion.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/erfaversion.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fad03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fad03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fae03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fae03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/faf03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/faf03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/faju03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/faju03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fal03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fal03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/falp03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/falp03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fama03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fama03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fame03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fame03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fane03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fane03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/faom03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/faom03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fapa03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fapa03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fasa03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fasa03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/faur03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/faur03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fave03.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fave03.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk425.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk425.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk45z.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk45z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk524.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk524.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk52h.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk52h.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk54z.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk54z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk5hip.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk5hip.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fk5hz.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fk5hz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fw2m.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fw2m.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/fw2xy.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/fw2xy.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/g2icrs.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/g2icrs.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gc2gd.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gc2gd.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gc2gde.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gc2gde.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gd2gc.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gd2gc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gd2gce.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gd2gce.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gmst00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gmst00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gmst06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gmst06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gmst82.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gmst82.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gst00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gst00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gst00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gst00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gst06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gst06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gst06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gst06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/gst94.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/gst94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/h2fk5.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/h2fk5.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/hd2ae.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/hd2ae.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/hd2pa.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/hd2pa.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/hfk5z.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/hfk5z.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/icrs2g.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/icrs2g.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ir.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ir.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/jd2cal.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/jd2cal.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/jdcalf.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/jdcalf.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ld.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ld.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ldn.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ldn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ldsun.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ldsun.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/lteceq.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/lteceq.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ltecm.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ltecm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/lteqec.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/lteqec.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ltp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ltp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ltpb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ltpb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ltpecl.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ltpecl.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ltpequ.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ltpequ.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/meson.build` & `pyerfa-2.0.1.1/liberfa/erfa/src/meson.build`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/moon98.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/moon98.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/num00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/num00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/num00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/num00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/num06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/num06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/numat.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/numat.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/nut00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/nut00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/nut00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/nut00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/nut06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/nut06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/nut80.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/nut80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/nutm80.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/nutm80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/obl06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/obl06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/obl80.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/obl80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/p06e.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/p06e.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/p2pv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/p2pv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/p2s.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/p2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pap.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pap.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pas.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pas.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pb06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pb06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pdp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pdp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pfw06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pfw06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/plan94.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/plan94.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pm.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmat00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmat00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmat06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmat06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmat76.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmat76.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmpx.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmpx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pmsafe.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pmsafe.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pn06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pn06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pnm00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pnm00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pnm00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pnm00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pnm06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pnm06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pnm80.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pnm80.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pom00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pom00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ppp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ppp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ppsp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ppsp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pr00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pr00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/prec76.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/prec76.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pv2p.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pv2p.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pv2s.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pv2s.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvdpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvdpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvm.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvmpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvmpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvppv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvppv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvstar.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvstar.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvtob.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvtob.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvu.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvu.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvup.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvup.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pvxpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pvxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/pxp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/pxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/refco.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/refco.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rm2v.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rm2v.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rv2m.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rv2m.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rx.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rx.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rxp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rxpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rxr.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rxr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ry.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ry.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/rz.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/rz.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s2c.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s2c.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s2p.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s2p.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s2pv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s2pv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/s2xpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/s2xpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/sepp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/sepp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/seps.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/seps.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/sp00.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/sp00.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/starpm.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/starpm.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/starpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/starpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/sxp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/sxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/sxpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/sxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/t_erfa_c.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/t_erfa_c_extra.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/t_erfa_c_extra.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/taitt.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/taitt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/taiut1.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/taiut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/taiutc.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/taiutc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tcbtdb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tcbtdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tcgtt.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tcgtt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tdbtcb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tdbtcb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tdbtt.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tdbtt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tf2a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tf2a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tf2d.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tf2d.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tpors.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tpors.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tporv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tporv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tpsts.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tpsts.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tpstv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tpstv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tpxes.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tpxes.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tpxev.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tpxev.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tr.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/trxp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/trxp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/trxpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/trxpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tttai.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tttai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tttcg.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tttcg.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/tttdb.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/tttdb.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ttut1.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ttut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ut1tai.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ut1tai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ut1tt.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ut1tt.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/ut1utc.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/ut1utc.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/utctai.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/utctai.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/utcut1.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/utcut1.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/xy06.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/xy06.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/xys00a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/xys00a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/xys00b.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/xys00b.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/xys06a.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/xys06a.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/zp.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/zp.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/zpv.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/zpv.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/liberfa/erfa/src/zr.c` & `pyerfa-2.0.1.1/liberfa/erfa/src/zr.c`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/licenses/ERFA.rst` & `pyerfa-2.0.1.1/licenses/ERFA.rst`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/pyerfa.egg-info/PKG-INFO` & `pyerfa-2.0.1.1/pyerfa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerfa
-Version: 2.0.1
+Version: 2.0.1.1
 Summary: Python bindings for ERFA
 Home-page: https://github.com/liberfa/pyerfa
 Author: The PyERFA Developers
 License: BSD 3-Clause License
 Keywords: astronomy,astrophysics,cosmology,space,science,coordinate
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pyerfa-2.0.1/pyerfa.egg-info/SOURCES.txt` & `pyerfa-2.0.1.1/pyerfa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/setup.cfg` & `pyerfa-2.0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/setup.py` & `pyerfa-2.0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `pyerfa-2.0.1/tox.ini` & `pyerfa-2.0.1.1/tox.ini`

 * *Files identical despite different names*

