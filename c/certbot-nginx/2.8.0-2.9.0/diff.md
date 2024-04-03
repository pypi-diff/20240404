# Comparing `tmp/certbot-nginx-2.8.0.tar.gz` & `tmp/certbot-nginx-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-nginx-2.8.0.tar", last modified: Tue Dec  5 19:13:58 2023, max compression
+gzip compressed data, was "certbot-nginx-2.9.0.tar", last modified: Thu Feb  8 19:45:26 2024, max compression
```

## Comparing `certbot-nginx-2.8.0.tar` & `certbot-nginx-2.9.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    11984 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      242 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1361 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       25 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/
--rw-rw-r--   0 willg     (1000) willg     (1000)       28 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       52 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    55346 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/configurator.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3275 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/constants.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1554 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/display_ops.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9806 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/http_01.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    10981 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/nginxparser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9840 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/obj.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    32772 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/parser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    16118 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/parser_obj.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       26 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    51859 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/configurator_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1632 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/display_ops_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    10230 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/http_01_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    16901 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/nginxparser_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9436 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/obj_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    11587 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/parser_obj_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    24674 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/parser_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4884 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/test_util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/
--rw-rw-r--   0 willg     (1000) willg     (1000)      125 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/broken.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       25 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/comment_in_file.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      579 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/edge_cases.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      540 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/foo.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      181 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/invalid_unicode_comments.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/mime.types
--rw-rw-r--   0 willg     (1000) willg     (1000)      197 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/minimalistic_comments.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      585 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/multiline_quotes.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2684 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/nginx.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       45 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/server.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      501 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/both.com
--rw-rw-r--   0 willg     (1000) willg     (1000)      211 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/default
--rw-rw-r--   0 willg     (1000) willg     (1000)      133 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/example.com
--rw-rw-r--   0 willg     (1000) willg     (1000)       73 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/example.net
--rw-rw-r--   0 willg     (1000) willg     (1000)      144 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/globalssl.com
--rw-rw-r--   0 willg     (1000) willg     (1000)       87 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/headers.com
--rw-rw-r--   0 willg     (1000) willg     (1000)       72 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/ipv6.com
--rw-rw-r--   0 willg     (1000) willg     (1000)      156 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/ipv6ssl.com
--rw-rw-r--   0 willg     (1000) willg     (1000)      383 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/migration.com
--rw-rw-r--   0 willg     (1000) willg     (1000)      111 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/sslon.com
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.871180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/
--rw-rw-r--   0 willg     (1000) willg     (1000)      911 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/fastcgi_params
--rw-rw-r--   0 willg     (1000) willg     (1000)     2258 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-utf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1805 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-win
--rw-rw-r--   0 willg     (1000) willg     (1000)     2085 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/mime.types
--rw-rw-r--   0 willg     (1000) willg     (1000)      222 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi-ui.conf.1.4.1
--rw-rw-r--   0 willg     (1000) willg     (1000)      287 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi.rules
--rw-rw-r--   0 willg     (1000) willg     (1000)     5288 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi_core.rules
--rw-rw-r--   0 willg     (1000) willg     (1000)     1601 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/nginx.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      180 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/proxy_params
--rw-rw-r--   0 willg     (1000) willg     (1000)      465 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/scgi_params
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)     2593 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/default
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)     2593 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/default
--rw-rw-r--   0 willg     (1000) willg     (1000)      532 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/uwsgi_params
--rw-rw-r--   0 willg     (1000) willg     (1000)     3072 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/win-utf
--rw-rw-r--   0 willg     (1000) willg     (1000)      308 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/valid_unicode_comments.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/
--rw-rw-r--   0 willg     (1000) willg     (1000)      741 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-old.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      766 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls12-only.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      749 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls13-session-tix-on.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      774 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-nginx-2.8.0/certbot_nginx/py.typed
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/certbot_nginx.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1361 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)     4241 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       81 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      159 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       14 2023-12-05 19:13:58.000000 certbot-nginx-2.8.0/certbot_nginx.egg-info/top_level.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:13:58.875180 certbot-nginx-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     1988 2023-12-05 19:13:53.000000 certbot-nginx-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11984 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      242 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1412 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       25 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.247117 certbot-nginx-2.9.0/certbot_nginx/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       28 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.251117 certbot-nginx-2.9.0/certbot_nginx/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       52 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    55369 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/configurator.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3275 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/constants.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1554 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/display_ops.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9806 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/http_01.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10981 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/nginxparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9840 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/obj.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    32772 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/parser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16118 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/parser_obj.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.251117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       26 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    51859 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/configurator_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1632 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/display_ops_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10230 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/http_01_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16901 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/nginxparser_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9436 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/obj_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11587 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/parser_obj_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24674 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/parser_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4884 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/test_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.247117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.251117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      125 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/broken.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       25 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/comment_in_file.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      579 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/edge_cases.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      540 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/foo.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      181 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/invalid_unicode_comments.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/mime.types
+-rw-rw-r--   0 erica     (1001) erica     (1001)      197 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/minimalistic_comments.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      585 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/multiline_quotes.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2684 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/nginx.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       45 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/server.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.251117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      501 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/both.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)      211 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/default
+-rw-rw-r--   0 erica     (1001) erica     (1001)      133 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/example.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)       73 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/example.net
+-rw-rw-r--   0 erica     (1001) erica     (1001)      144 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/globalssl.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)       87 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/headers.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)       72 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/ipv6.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)      156 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/ipv6ssl.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)      383 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/migration.com
+-rw-rw-r--   0 erica     (1001) erica     (1001)      111 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/sites-enabled/sslon.com
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.247117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.247117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      911 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/fastcgi_params
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2258 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-utf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1805 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-win
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2085 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/mime.types
+-rw-rw-r--   0 erica     (1001) erica     (1001)      222 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi-ui.conf.1.4.1
+-rw-rw-r--   0 erica     (1001) erica     (1001)      287 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi.rules
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5288 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi_core.rules
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1601 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/nginx.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      180 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/proxy_params
+-rw-rw-r--   0 erica     (1001) erica     (1001)      465 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/scgi_params
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2593 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/default
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2593 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/default
+-rw-rw-r--   0 erica     (1001) erica     (1001)      532 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/uwsgi_params
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3072 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/win-utf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      308 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/valid_unicode_comments.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      741 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-old.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      766 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls12-only.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      749 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls13-session-tix-on.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      774 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-nginx-2.9.0/certbot_nginx/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/certbot_nginx.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1412 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4241 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       81 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      159 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       14 2024-02-08 19:45:26.000000 certbot-nginx-2.9.0/certbot_nginx.egg-info/top_level.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:26.255117 certbot-nginx-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2038 2024-02-08 19:45:18.000000 certbot-nginx-2.9.0/setup.py
```

### Comparing `certbot-nginx-2.8.0/LICENSE.txt` & `certbot-nginx-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/PKG-INFO` & `certbot-nginx-2.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx
-Version: 2.8.0
+Version: 2.9.0
 Summary: Nginx plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,23 +13,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: acme>=2.8.0
-Requires-Dist: certbot>=2.8.0
+Requires-Dist: acme>=2.9.0
+Requires-Dist: certbot>=2.9.0
 Requires-Dist: importlib_resources>=1.3.1; python_version < "3.9"
 Requires-Dist: PyOpenSSL!=23.1.0,>=17.5.0
 Requires-Dist: pyparsing>=2.2.1
 Requires-Dist: setuptools>=41.6.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/configurator.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/configurator.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,16 +167,16 @@
             if session_tix_off:
                 config_filename = "options-ssl-nginx-tls12-only.conf"
             else:
                 config_filename = "options-ssl-nginx-old.conf"
 
         file_manager = ExitStack()
         atexit.register(file_manager.close)
-        ref = importlib_resources.files("certbot_nginx").joinpath(
-            "_internal", "tls_configs", config_filename)
+        ref = (importlib_resources.files("certbot_nginx").joinpath("_internal")
+               .joinpath("tls_configs").joinpath(config_filename))
 
         return str(file_manager.enter_context(importlib_resources.as_file(ref)))
 
     @property
     def mod_ssl_conf(self) -> str:
         """Full absolute path to SSL configuration file."""
         return os.path.join(self.config.config_dir, constants.MOD_SSL_CONF_DEST)
@@ -697,15 +697,15 @@
         return util.get_filtered_names(all_names)
 
     def _get_snakeoil_paths(self) -> Tuple[str, str]:
         """Generate invalid certs that let us create ssl directives for Nginx"""
         # TODO: generate only once
         tmp_dir = os.path.join(self.config.work_dir, "snakeoil")
         le_key = crypto_util.generate_key(
-            key_size=1024, key_dir=tmp_dir, keyname="key.pem",
+            key_size=2048, key_dir=tmp_dir, keyname="key.pem",
             strict_permissions=self.config.strict_permissions)
         assert le_key.file is not None
         key = OpenSSL.crypto.load_privatekey(
             OpenSSL.crypto.FILETYPE_PEM, le_key.pem)
         cert = acme_crypto_util.gen_ss_cert(key, domains=[socket.gethostname()])
         cert_pem = OpenSSL.crypto.dump_certificate(
             OpenSSL.crypto.FILETYPE_PEM, cert)
```

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/constants.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/display_ops.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/display_ops.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/http_01.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/http_01.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/nginxparser.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/nginxparser.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/obj.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/obj.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/parser.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/parser_obj.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/parser_obj.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/configurator_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/display_ops_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/display_ops_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/http_01_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/http_01_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/nginxparser_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/nginxparser_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/obj_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/obj_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/parser_obj_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/parser_obj_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/parser_test.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/parser_test.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/test_util.py` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/edge_cases.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/edge_cases.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/foo.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/foo.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/multiline_quotes.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/multiline_quotes.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/nginx.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/fastcgi_params` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/fastcgi_params`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-utf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-utf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-win` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/koi-win`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/mime.types` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/mime.types`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi_core.rules` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/naxsi_core.rules`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/nginx.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/default` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-available/default`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/default` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/sites-enabled/default`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/uwsgi_params` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/uwsgi_params`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/win-utf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tests/testdata/etc_nginx/ubuntu_nginx_1_4_6/default_vhost/nginx/win-utf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-old.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-old.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls12-only.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls12-only.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls13-session-tix-on.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx-tls13-session-tix-on.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx.conf` & `certbot-nginx-2.9.0/certbot_nginx/_internal/tls_configs/options-ssl-nginx.conf`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/certbot_nginx.egg-info/PKG-INFO` & `certbot-nginx-2.9.0/certbot_nginx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-nginx
-Version: 2.8.0
+Version: 2.9.0
 Summary: Nginx plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,23 +13,24 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 License-File: LICENSE.txt
-Requires-Dist: acme>=2.8.0
-Requires-Dist: certbot>=2.8.0
+Requires-Dist: acme>=2.9.0
+Requires-Dist: certbot>=2.9.0
 Requires-Dist: importlib_resources>=1.3.1; python_version < "3.9"
 Requires-Dist: PyOpenSSL!=23.1.0,>=17.5.0
 Requires-Dist: pyparsing>=2.2.1
 Requires-Dist: setuptools>=41.6.0
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-nginx-2.8.0/certbot_nginx.egg-info/SOURCES.txt` & `certbot-nginx-2.9.0/certbot_nginx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-nginx-2.8.0/setup.py` & `certbot-nginx-2.9.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages
 from setuptools import setup
 
-version = '2.8.0'
+version = '2.9.0'
 
 install_requires = [
     # We specify the minimum acme and certbot version as the current plugin
     # version for simplicity. See
     # https://github.com/certbot/certbot/issues/8761 for more info.
     f'acme>={version}',
     f'certbot>={version}',
@@ -37,14 +37,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Internet :: WWW/HTTP',
         'Topic :: Security',
         'Topic :: System :: Installation/Setup',
         'Topic :: System :: Networking',
         'Topic :: System :: Systems Administration',
         'Topic :: Utilities',
     ],
```

