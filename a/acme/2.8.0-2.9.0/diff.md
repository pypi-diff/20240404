# Comparing `tmp/acme-2.8.0.tar.gz` & `tmp/acme-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acme-2.8.0.tar", last modified: Tue Dec  5 19:13:55 2023, max compression
+gzip compressed data, was "acme-2.9.0.tar", last modified: Thu Feb  8 19:45:23 2024, max compression
```

## Comparing `acme-2.8.0.tar` & `acme-2.9.0.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10786 2023-12-05 19:13:52.000000 acme-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      236 2023-12-05 19:13:52.000000 acme-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1359 2023-12-05 19:13:55.911222 acme-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       39 2023-12-05 19:13:52.000000 acme-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.907222 acme-2.8.0/acme/
--rw-rw-r--   0 willg     (1000) willg     (1000)      736 2023-12-05 19:13:52.000000 acme-2.8.0/acme/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.907222 acme-2.8.0/acme/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       37 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.907222 acme-2.8.0/acme/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       17 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    18961 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/challenges_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    34794 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/client_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    13489 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/crypto_util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1534 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/errors_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1719 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/fields_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1839 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/jose_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2082 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/jws_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    19730 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/messages_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9928 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/standalone_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2571 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/test_util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/acme/_internal/tests/testdata/
--rw-rw-r--   0 willg     (1000) willg     (1000)      858 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/README
--rw-rw-r--   0 willg     (1000) willg     (1000)     2752 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-100sans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1866 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-idnsans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1289 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-ipsans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1310 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-ipv6sans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1397 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-nocn.der
--rw-rw-r--   0 willg     (1000) willg     (1000)      786 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert-san.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      771 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert.der
--rw-rw-r--   0 willg     (1000) willg     (1000)      709 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/cert.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1683 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/critical-san.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     2577 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-100sans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      676 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-6sans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1691 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-idnsans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      920 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-ipsans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      952 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-ipv6sans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      932 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-mixed.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      452 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-nosans.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      574 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr-san.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      607 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr.der
--rw-rw-r--   0 willg     (1000) willg     (1000)      550 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/csr.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      684 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/dsa512_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      306 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/ec_secp384r1_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      749 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa1024_cert.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      887 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa1024_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1294 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa2048_cert.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1704 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa2048_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      298 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa256_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     1814 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa4096_cert.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)     3247 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa4096_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      493 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/testdata/rsa512_key.pem
--rw-rw-r--   0 willg     (1000) willg     (1000)      396 2023-12-05 19:13:52.000000 acme-2.8.0/acme/_internal/tests/util_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    22456 2023-12-05 19:13:52.000000 acme-2.8.0/acme/challenges.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    31138 2023-12-05 19:13:52.000000 acme-2.8.0/acme/client.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    18051 2023-12-05 19:13:52.000000 acme-2.8.0/acme/crypto_util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4315 2023-12-05 19:13:52.000000 acme-2.8.0/acme/errors.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1652 2023-12-05 19:13:52.000000 acme-2.8.0/acme/fields.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2564 2023-12-05 19:13:52.000000 acme-2.8.0/acme/jws.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    26242 2023-12-05 19:13:52.000000 acme-2.8.0/acme/messages.py
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 acme-2.8.0/acme/py.typed
--rw-rw-r--   0 willg     (1000) willg     (1000)    12983 2023-12-05 19:13:52.000000 acme-2.8.0/acme/standalone.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      303 2023-12-05 19:13:52.000000 acme-2.8.0/acme/util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/acme.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1359 2023-12-05 19:13:55.000000 acme-2.8.0/acme.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)     2514 2023-12-05 19:13:55.000000 acme-2.8.0/acme.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:13:55.000000 acme-2.8.0/acme.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      231 2023-12-05 19:13:55.000000 acme-2.8.0/acme.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        5 2023-12-05 19:13:55.000000 acme-2.8.0/acme.egg-info/top_level.txt
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/docs/
--rw-rw-r--   0 willg     (1000) willg     (1000)        9 2023-12-05 19:13:52.000000 acme-2.8.0/docs/.gitignore
--rw-rw-r--   0 willg     (1000) willg     (1000)     7434 2023-12-05 19:13:52.000000 acme-2.8.0/docs/Makefile
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/docs/_static/
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 acme-2.8.0/docs/_static/.gitignore
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/docs/_templates/
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 acme-2.8.0/docs/_templates/.gitignore
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/docs/api/
--rw-rw-r--   0 willg     (1000) willg     (1000)       68 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/challenges.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       56 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/client.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       56 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/errors.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       56 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/fields.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      161 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/jose.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       62 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/messages.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       68 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api/standalone.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)       88 2023-12-05 19:13:52.000000 acme-2.8.0/docs/api.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)     9795 2023-12-05 19:13:52.000000 acme-2.8.0/docs/conf.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      479 2023-12-05 19:13:52.000000 acme-2.8.0/docs/index.rst
--rw-rw-r--   0 willg     (1000) willg     (1000)      167 2023-12-05 19:13:52.000000 acme-2.8.0/docs/jws-help.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)     7259 2023-12-05 19:13:52.000000 acme-2.8.0/docs/make.bat
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/docs/man/
--rw-rw-r--   0 willg     (1000) willg     (1000)       46 2023-12-05 19:13:52.000000 acme-2.8.0/docs/man/jws.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:55.911222 acme-2.8.0/examples/
--rw-rw-r--   0 willg     (1000) willg     (1000)     7123 2023-12-05 19:13:52.000000 acme-2.8.0/examples/http01_example.py
--rw-rw-r--   0 willg     (1000) willg     (1000)       63 2023-12-05 19:13:52.000000 acme-2.8.0/pytest.ini
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:13:55.911222 acme-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     2288 2023-12-05 19:13:53.000000 acme-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2024-02-08 19:45:17.000000 acme-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      236 2024-02-08 19:45:17.000000 acme-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1410 2024-02-08 19:45:23.083103 acme-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       39 2024-02-08 19:45:17.000000 acme-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.079103 acme-2.9.0/acme/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      736 2024-02-08 19:45:17.000000 acme-2.9.0/acme/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.079103 acme-2.9.0/acme/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       37 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.079103 acme-2.9.0/acme/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       17 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18961 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/challenges_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    34794 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/client_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13489 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/crypto_util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1534 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/errors_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1719 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/fields_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1839 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/jose_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2082 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/jws_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    19730 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/messages_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9928 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/standalone_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2571 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/test_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/acme/_internal/tests/testdata/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      858 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/README
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2752 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-100sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1866 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-idnsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1289 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-ipsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1310 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-ipv6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1397 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-nocn.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      786 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      771 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      709 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1683 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/critical-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2577 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-100sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      676 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1691 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-idnsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      920 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-ipsans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      952 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-ipv6sans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      932 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-mixed.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      452 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-nosans.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      574 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr-san.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      607 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr.der
+-rw-rw-r--   0 erica     (1001) erica     (1001)      550 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/csr.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      684 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/dsa512_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      306 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/ec_secp384r1_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      749 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa1024_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      887 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa1024_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1294 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa2048_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1704 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa2048_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      298 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa256_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1814 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa4096_cert.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3247 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa4096_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      493 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/testdata/rsa512_key.pem
+-rw-rw-r--   0 erica     (1001) erica     (1001)      396 2024-02-08 19:45:17.000000 acme-2.9.0/acme/_internal/tests/util_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22456 2024-02-08 19:45:17.000000 acme-2.9.0/acme/challenges.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    31138 2024-02-08 19:45:17.000000 acme-2.9.0/acme/client.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    18051 2024-02-08 19:45:17.000000 acme-2.9.0/acme/crypto_util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4315 2024-02-08 19:45:17.000000 acme-2.9.0/acme/errors.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1652 2024-02-08 19:45:17.000000 acme-2.9.0/acme/fields.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2564 2024-02-08 19:45:17.000000 acme-2.9.0/acme/jws.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    26242 2024-02-08 19:45:17.000000 acme-2.9.0/acme/messages.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 acme-2.9.0/acme/py.typed
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12983 2024-02-08 19:45:17.000000 acme-2.9.0/acme/standalone.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      303 2024-02-08 19:45:17.000000 acme-2.9.0/acme/util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/acme.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1410 2024-02-08 19:45:23.000000 acme-2.9.0/acme.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2514 2024-02-08 19:45:23.000000 acme-2.9.0/acme.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:23.000000 acme-2.9.0/acme.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      231 2024-02-08 19:45:23.000000 acme-2.9.0/acme.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        5 2024-02-08 19:45:23.000000 acme-2.9.0/acme.egg-info/top_level.txt
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/docs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        9 2024-02-08 19:45:17.000000 acme-2.9.0/docs/.gitignore
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7434 2024-02-08 19:45:17.000000 acme-2.9.0/docs/Makefile
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/docs/_static/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 acme-2.9.0/docs/_static/.gitignore
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/docs/_templates/
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 acme-2.9.0/docs/_templates/.gitignore
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/docs/api/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       68 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/challenges.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/client.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/errors.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       56 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/fields.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      161 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/jose.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       62 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/messages.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       68 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api/standalone.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)       88 2024-02-08 19:45:17.000000 acme-2.9.0/docs/api.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9795 2024-02-08 19:45:17.000000 acme-2.9.0/docs/conf.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      479 2024-02-08 19:45:17.000000 acme-2.9.0/docs/index.rst
+-rw-rw-r--   0 erica     (1001) erica     (1001)      156 2024-02-08 19:45:17.000000 acme-2.9.0/docs/jws-help.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7259 2024-02-08 19:45:17.000000 acme-2.9.0/docs/make.bat
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/docs/man/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2024-02-08 19:45:17.000000 acme-2.9.0/docs/man/jws.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:23.083103 acme-2.9.0/examples/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7123 2024-02-08 19:45:17.000000 acme-2.9.0/examples/http01_example.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)       63 2024-02-08 19:45:17.000000 acme-2.9.0/pytest.ini
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:23.083103 acme-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2338 2024-02-08 19:45:18.000000 acme-2.9.0/setup.py
```

### Comparing `acme-2.8.0/LICENSE.txt` & `acme-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/PKG-INFO` & `acme-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: acme
-Version: 2.8.0
+Version: 2.9.0
 Summary: ACME protocol implementation in Python
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: cryptography>=3.2.1
 Requires-Dist: josepy>=1.13.0
 Requires-Dist: PyOpenSSL!=23.1.0,>=17.5.0
```

### Comparing `acme-2.8.0/acme/__init__.py` & `acme-2.9.0/acme/__init__.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/challenges_test.py` & `acme-2.9.0/acme/_internal/tests/challenges_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/client_test.py` & `acme-2.9.0/acme/_internal/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/crypto_util_test.py` & `acme-2.9.0/acme/_internal/tests/crypto_util_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/errors_test.py` & `acme-2.9.0/acme/_internal/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/fields_test.py` & `acme-2.9.0/acme/_internal/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/jose_test.py` & `acme-2.9.0/acme/_internal/tests/jose_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/jws_test.py` & `acme-2.9.0/acme/_internal/tests/jws_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/messages_test.py` & `acme-2.9.0/acme/_internal/tests/messages_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/standalone_test.py` & `acme-2.9.0/acme/_internal/tests/standalone_test.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/test_util.py` & `acme-2.9.0/acme/_internal/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/README` & `acme-2.9.0/acme/_internal/tests/testdata/README`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-100sans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert-100sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-idnsans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert-idnsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-ipsans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert-ipsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-ipv6sans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert-ipv6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-nocn.der` & `acme-2.9.0/acme/_internal/tests/testdata/cert-nocn.der`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert-san.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert.der` & `acme-2.9.0/acme/_internal/tests/testdata/cert.der`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/cert.pem` & `acme-2.9.0/acme/_internal/tests/testdata/cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/critical-san.pem` & `acme-2.9.0/acme/_internal/tests/testdata/critical-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-100sans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-100sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-6sans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-idnsans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-idnsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-ipsans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-ipsans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-ipv6sans.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-ipv6sans.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-mixed.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-mixed.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr-san.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr-san.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr.der` & `acme-2.9.0/acme/_internal/tests/testdata/csr.der`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/csr.pem` & `acme-2.9.0/acme/_internal/tests/testdata/csr.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/dsa512_key.pem` & `acme-2.9.0/acme/_internal/tests/testdata/dsa512_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa1024_cert.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa1024_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa1024_key.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa1024_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa2048_cert.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa2048_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa2048_key.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa2048_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa4096_cert.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa4096_cert.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/_internal/tests/testdata/rsa4096_key.pem` & `acme-2.9.0/acme/_internal/tests/testdata/rsa4096_key.pem`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/challenges.py` & `acme-2.9.0/acme/challenges.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/client.py` & `acme-2.9.0/acme/client.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/crypto_util.py` & `acme-2.9.0/acme/crypto_util.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/errors.py` & `acme-2.9.0/acme/errors.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/fields.py` & `acme-2.9.0/acme/fields.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/jws.py` & `acme-2.9.0/acme/jws.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/messages.py` & `acme-2.9.0/acme/messages.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme/standalone.py` & `acme-2.9.0/acme/standalone.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/acme.egg-info/PKG-INFO` & `acme-2.9.0/acme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: acme
-Version: 2.8.0
+Version: 2.9.0
 Summary: ACME protocol implementation in Python
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Requires-Python: >=3.8
 License-File: LICENSE.txt
 Requires-Dist: cryptography>=3.2.1
 Requires-Dist: josepy>=1.13.0
 Requires-Dist: PyOpenSSL!=23.1.0,>=17.5.0
```

### Comparing `acme-2.8.0/acme.egg-info/SOURCES.txt` & `acme-2.9.0/acme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/docs/Makefile` & `acme-2.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/docs/conf.py` & `acme-2.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/docs/make.bat` & `acme-2.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/examples/http01_example.py` & `acme-2.9.0/examples/http01_example.py`

 * *Files identical despite different names*

### Comparing `acme-2.8.0/setup.py` & `acme-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.8.0'
+version = '2.9.0'
 
 install_requires = [
     'cryptography>=3.2.1',
     'josepy>=1.13.0',
     # pyOpenSSL 23.1.0 is a bad release: https://github.com/pyca/pyopenssl/issues/1199
     'PyOpenSSL>=17.5.0,!=23.1.0',
     'pyrfc3339',
@@ -51,14 +51,15 @@
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
     ],
 
     packages=find_packages(),
     include_package_data=True,
     install_requires=install_requires,
```

