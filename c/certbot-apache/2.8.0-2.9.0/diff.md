# Comparing `tmp/certbot-apache-2.8.0.tar.gz` & `tmp/certbot-apache-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-apache-2.8.0.tar", last modified: Tue Dec  5 19:13:57 2023, max compression
+gzip compressed data, was "certbot-apache-2.9.0.tar", last modified: Thu Feb  8 19:45:24 2024, max compression
```

## Comparing `certbot-apache-2.8.0.tar` & `certbot-apache-2.9.0.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.291202 certbot-apache-2.8.0/
--rw-rw-r--   0 willg     (1000) willg     (1000)    10786 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/LICENSE.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      306 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/MANIFEST.in
--rw-r--r--   0 willg     (1000) willg     (1000)     1389 2023-12-05 19:13:57.291202 certbot-apache-2.8.0/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)       26 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/README.rst
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/
--rw-rw-r--   0 willg     (1000) willg     (1000)       29 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/__init__.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/
--rw-rw-r--   0 willg     (1000) willg     (1000)       29 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     7697 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/apache_util.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     8072 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/apacheparser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5893 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/assertions.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/augeas_lens/
--rw-rw-r--   0 willg     (1000) willg     (1000)     7528 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/augeas_lens/httpd.aug
--rw-rw-r--   0 willg     (1000) willg     (1000)    21112 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/augeasparser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)   112791 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/configurator.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4020 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/constants.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4576 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/display_ops.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    14986 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/dualparser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2973 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/entrypoint.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     8415 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/http_01.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    22825 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/interfaces.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9299 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/obj.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      694 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_alpine.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      676 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_arch.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4700 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_centos.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      604 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_darwin.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5285 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_debian.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3460 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_fedora.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2427 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_gentoo.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      670 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_suse.py
--rw-rw-r--   0 willg     (1000) willg     (1000)      681 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/override_void.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    36804 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/parser.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5823 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/parsernode_util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/tests/
--rw-rw-r--   0 willg     (1000) willg     (1000)       27 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/__init__.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    12943 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/augeasnode_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     8939 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/autohsts_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    10972 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/centos_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     4408 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/complex_parsing_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     2816 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/configurator_reverter_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    77986 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/configurator_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9283 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/debian_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3748 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/display_ops_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    24089 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/dualnode_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1718 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/entrypoint_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     8161 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/fedora_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5590 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/gentoo_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     9189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/http_01_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     5165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/obj_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)    16692 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/parser_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     1625 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_configurator_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3554 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_test.py
--rw-rw-r--   0 willg     (1000) willg     (1000)     3275 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_util_test.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/
--rw-rw-r--   0 willg     (1000) willg     (1000)    11753 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)    13077 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.279202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/
--rw-rw-r--   0 willg     (1000) willg     (1000)      366 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/README
--rw-rw-r--   0 willg     (1000) willg     (1000)     2926 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      213 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/centos.example.com.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     9295 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1252 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      824 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/
--rw-rw-r--   0 willg     (1000) willg     (1000)     3739 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      139 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-dav.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       41 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-lua.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      742 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      957 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       41 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       88 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-systemd.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      451 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/01-cgi.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       51 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sites
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/
--rw-rw-r--   0 willg     (1000) willg     (1000)      890 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/
--rw-rw-r--   0 willg     (1000) willg     (1000)     1078 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      267 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/dummy.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       26 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_fnmatch.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1234 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/
--rw-rw-r--   0 willg     (1000) willg     (1000)     6533 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)       46 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/bad_conf_file.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/serve-cgi-bin.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      982 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/authz_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       93 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     2372 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      203 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       66 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/rewrite.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     3405 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       97 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.load
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/authz_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       93 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     2372 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      203 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)      320 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/ports.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      282 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/another_wildcard.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      266 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/old-and-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      322 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/wildcard.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      282 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/another_wildcard.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      266 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/old-and-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      322 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/wildcard.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      153 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/sites
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/
--rw-rw-r--   0 willg     (1000) willg     (1000)     6536 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1014 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/serve-cgi-bin.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1014 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/serve-cgi-bin.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      981 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)     3405 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       97 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.load
--rw-rw-r--   0 willg     (1000) willg     (1000)      397 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/ports.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      295 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/000-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1140 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      295 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/000-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       47 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/sites
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/
--rw-rw-r--   0 willg     (1000) willg     (1000)     6533 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      982 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars
--rw-rw-r--   0 willg     (1000) willg     (1000)      320 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/ports.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      474 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1280 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      474 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1280 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/
--rw-rw-r--   0 willg     (1000) willg     (1000)     6749 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.283202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)       46 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/bad_conf_file.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/serve-cgi-bin.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      455 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      982 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/authz_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       93 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     2372 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      203 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       66 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/rewrite.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     3405 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       97 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.load
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      165 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/authz_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)       93 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav.load
--rw-rw-r--   0 willg     (1000) willg     (1000)     2372 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      203 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.load
--rw-rw-r--   0 willg     (1000) willg     (1000)      320 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/ports.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/
--rw-rw-r--   0 willg     (1000) willg     (1000)      266 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/000-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      941 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1112 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1201 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      228 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttp.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      378 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttps.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/empty.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1157 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      377 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/mod_macro-example.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)       90 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/no-directives.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1568 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      289 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/wildcard.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/
--rw-rw-r--   0 willg     (1000) willg     (1000)      266 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/000-default.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      941 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1112 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1201 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      228 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttp.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      378 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttps.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1157 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      377 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/mod_macro-example.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      222 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/non-symlink.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1568 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      289 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/wildcard.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      153 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/sites
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.275202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/
--rw-rw-r--   0 willg     (1000) willg     (1000)     6303 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)    13077 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/
--rw-rw-r--   0 willg     (1000) willg     (1000)     5308 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2520 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     5041 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2883 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      225 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_info.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1518 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1707 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      458 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_status.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1015 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2959 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      206 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/10_mod_mem_cache.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2652 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      189 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/41_mod_http2.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      758 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      406 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/46_mod_ldap.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/
--rw-rw-r--   0 willg     (1000) willg     (1000)     8596 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     1462 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)     2804 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include
--rw-rw-r--   0 willg     (1000) willg     (1000)      213 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/gentoo.example.com.conf
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/
--rw-rw-r--   0 willg     (1000) willg     (1000)     3136 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2
--rw-rw-r--   0 willg     (1000) willg     (1000)      141 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/sites
--rw-rw-r--   0 willg     (1000) willg     (1000)    10805 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tests/util.py
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.287202 certbot-apache-2.8.0/certbot_apache/_internal/tls_configs/
--rw-rw-r--   0 willg     (1000) willg     (1000)     1005 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)      977 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf
--rw-rw-r--   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:52.000000 certbot-apache-2.8.0/certbot_apache/py.typed
-drwxrwxr-x   0 willg     (1000) willg     (1000)        0 2023-12-05 19:13:57.291202 certbot-apache-2.8.0/certbot_apache.egg-info/
--rw-r--r--   0 willg     (1000) willg     (1000)     1389 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/PKG-INFO
--rw-rw-r--   0 willg     (1000) willg     (1000)    16853 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/SOURCES.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)        1 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/dependency_links.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       74 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/entry_points.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)      156 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/requires.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       15 2023-12-05 19:13:57.000000 certbot-apache-2.8.0/certbot_apache.egg-info/top_level.txt
--rw-rw-r--   0 willg     (1000) willg     (1000)       38 2023-12-05 19:13:57.291202 certbot-apache-2.8.0/setup.cfg
--rw-rw-r--   0 willg     (1000) willg     (1000)     1931 2023-12-05 19:13:53.000000 certbot-apache-2.8.0/setup.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10786 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/LICENSE.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      306 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/MANIFEST.in
+-rw-r--r--   0 erica     (1001) erica     (1001)     1440 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)       26 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/README.rst
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.643110 certbot-apache-2.9.0/certbot_apache/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       29 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/__init__.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       29 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7720 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/apache_util.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8072 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/apacheparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5893 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/assertions.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/augeas_lens/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     7528 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/augeas_lens/httpd.aug
+-rw-rw-r--   0 erica     (1001) erica     (1001)    21112 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/augeasparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)   112791 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/configurator.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4020 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/constants.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4576 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/display_ops.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    14986 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/dualparser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2973 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/entrypoint.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8415 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/http_01.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    22825 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/interfaces.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9299 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/obj.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      694 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_alpine.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      676 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_arch.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4700 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_centos.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      604 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_darwin.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5285 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_debian.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3460 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_fedora.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2427 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_gentoo.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      670 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_suse.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)      681 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/override_void.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    36804 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/parser.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5823 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/parsernode_util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/tests/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       27 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/__init__.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    12943 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/augeasnode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8939 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/autohsts_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10972 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/centos_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     4408 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/complex_parsing_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2816 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/configurator_reverter_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    77986 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/configurator_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9283 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/debian_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3748 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/display_ops_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    24089 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/dualnode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1718 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/entrypoint_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8161 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/fedora_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5590 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/gentoo_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/http_01_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/obj_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16692 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/parser_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1625 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_configurator_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3554 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_test.py
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3275 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_util_test.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.643110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.639110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.639110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/
+-rw-rw-r--   0 erica     (1001) erica     (1001)    11753 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13077 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.647110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      366 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/README
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2926 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      213 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/centos.example.com.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     9295 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1252 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      824 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3739 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      139 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-dav.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       41 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-lua.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      742 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      957 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       41 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       88 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-systemd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      451 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/01-cgi.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       51 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      890 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1078 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      267 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/conf-enabled/dummy.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       26 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_fnmatch.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1234 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.643110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6533 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/bad_conf_file.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       66 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/rewrite.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.load
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      282 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/another_wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/old-and-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      322 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-available/wildcard.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      282 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/another_wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/old-and-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      322 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/sites-enabled/wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6536 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1014 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1014 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      981 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.651110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      397 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      295 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1140 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      295 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-enabled/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       47 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.643110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6533 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      474 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1280 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      474 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1280 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6749 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)       46 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/bad_conf_file.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/serve-cgi-bin.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/other-vhosts-access-log.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      455 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/serve-cgi-bin.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      982 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       66 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/rewrite.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3405 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       97 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.load
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      165 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/authz_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)       93 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2372 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      203 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.load
+-rw-rw-r--   0 erica     (1001) erica     (1001)      320 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/ports.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.655110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      941 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1112 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1201 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      228 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttp.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      378 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/duplicatehttps.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/empty.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1157 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      377 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/mod_macro-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)       90 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/no-directives.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1568 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      289 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/wildcard.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/
+-rw-rw-r--   0 erica     (1001) erica     (1001)      266 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/000-default.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      941 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1112 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1201 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      228 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttp.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      378 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/duplicatehttps.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1157 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      377 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/mod_macro-example.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      222 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/non-symlink.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1568 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      289 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/wildcard.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      153 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/sites
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.643110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     6303 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)    13077 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5308 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2520 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     5041 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2883 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      225 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_info.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1518 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1707 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      458 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_status.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1015 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2959 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      206 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/10_mod_mem_cache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2652 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      189 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/41_mod_http2.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      758 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      406 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/46_mod_ldap.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     8596 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1462 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)     2804 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include
+-rw-rw-r--   0 erica     (1001) erica     (1001)      213 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/gentoo.example.com.conf
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     3136 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2
+-rw-rw-r--   0 erica     (1001) erica     (1001)      141 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/sites
+-rw-rw-r--   0 erica     (1001) erica     (1001)    10805 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tests/util.py
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache/_internal/tls_configs/
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1005 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)      977 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf
+-rw-rw-r--   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:17.000000 certbot-apache-2.9.0/certbot_apache/py.typed
+drwxrwxr-x   0 erica     (1001) erica     (1001)        0 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/certbot_apache.egg-info/
+-rw-r--r--   0 erica     (1001) erica     (1001)     1440 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/PKG-INFO
+-rw-rw-r--   0 erica     (1001) erica     (1001)    16853 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/SOURCES.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)        1 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/dependency_links.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       74 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/entry_points.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)      156 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/requires.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       15 2024-02-08 19:45:24.000000 certbot-apache-2.9.0/certbot_apache.egg-info/top_level.txt
+-rw-rw-r--   0 erica     (1001) erica     (1001)       38 2024-02-08 19:45:24.659110 certbot-apache-2.9.0/setup.cfg
+-rw-rw-r--   0 erica     (1001) erica     (1001)     1981 2024-02-08 19:45:18.000000 certbot-apache-2.9.0/setup.py
```

### Comparing `certbot-apache-2.8.0/LICENSE.txt` & `certbot-apache-2.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/PKG-INFO` & `certbot-apache-2.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-apache
-Version: 2.8.0
+Version: 2.9.0
 Summary: Apache plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,24 +13,25 @@
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
 Requires-Dist: python-augeas
 Requires-Dist: setuptools>=41.6.0
 Provides-Extra: dev
 Requires-Dist: apacheconfig>=0.3.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/apache_util.py` & `certbot-apache-2.9.0/certbot_apache/_internal/apache_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,10 +253,10 @@
     Find a TLS Apache config file in the dedicated storage.
     :param str prefix: prefix of the TLS Apache config file to find
     :return: the path the TLS Apache config file
     :rtype: str
     """
     file_manager = ExitStack()
     atexit.register(file_manager.close)
-    ref = importlib_resources.files("certbot_apache").joinpath(
-        "_internal", "tls_configs", "{0}-options-ssl-apache.conf".format(prefix))
+    ref = (importlib_resources.files("certbot_apache").joinpath("_internal")
+           .joinpath("tls_configs").joinpath("{0}-options-ssl-apache.conf".format(prefix)))
     return str(file_manager.enter_context(importlib_resources.as_file(ref)))
```

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/apacheparser.py` & `certbot-apache-2.9.0/certbot_apache/_internal/apacheparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/assertions.py` & `certbot-apache-2.9.0/certbot_apache/_internal/assertions.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/augeas_lens/httpd.aug` & `certbot-apache-2.9.0/certbot_apache/_internal/augeas_lens/httpd.aug`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/augeasparser.py` & `certbot-apache-2.9.0/certbot_apache/_internal/augeasparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/configurator.py` & `certbot-apache-2.9.0/certbot_apache/_internal/configurator.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/constants.py` & `certbot-apache-2.9.0/certbot_apache/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/display_ops.py` & `certbot-apache-2.9.0/certbot_apache/_internal/display_ops.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/dualparser.py` & `certbot-apache-2.9.0/certbot_apache/_internal/dualparser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/entrypoint.py` & `certbot-apache-2.9.0/certbot_apache/_internal/entrypoint.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/http_01.py` & `certbot-apache-2.9.0/certbot_apache/_internal/http_01.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/interfaces.py` & `certbot-apache-2.9.0/certbot_apache/_internal/interfaces.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/obj.py` & `certbot-apache-2.9.0/certbot_apache/_internal/obj.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_alpine.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_alpine.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_arch.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_arch.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_centos.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_centos.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_darwin.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_darwin.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_debian.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_debian.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_fedora.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_fedora.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_gentoo.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_gentoo.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_suse.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_suse.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/override_void.py` & `certbot-apache-2.9.0/certbot_apache/_internal/override_void.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/parser.py` & `certbot-apache-2.9.0/certbot_apache/_internal/parser.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/parsernode_util.py` & `certbot-apache-2.9.0/certbot_apache/_internal/parsernode_util.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/augeasnode_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/augeasnode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/autohsts_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/autohsts_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/centos_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/centos_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/complex_parsing_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/complex_parsing_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/configurator_reverter_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/configurator_reverter_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/configurator_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/debian_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/debian_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/display_ops_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/display_ops_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/dualnode_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/dualnode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/entrypoint_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/entrypoint_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/fedora_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/fedora_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/gentoo_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/gentoo_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/http_01_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/http_01_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/obj_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/obj_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/parser_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/parser_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_configurator_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_configurator_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/parsernode_util_test.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/parsernode_util_test.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/httpd.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf/magic`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/autoindex.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/userdir.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.d/welcome.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-base.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-mpm.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/httpd/conf.modules.d/00-proxy.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/centos7_apache/apache/sysconfig/httpd`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/complex_parsing/test_variables.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/augeas_vhosts/apache2/mods-enabled/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/default_vhost/apache2/sites-available/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-available/multi-vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multi_vhosts/apache2/sites-enabled/multi-vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/apache2.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-available/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/conf-enabled/security.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/envvars`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-available/ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/mods-enabled/dav_svn.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/certbot.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl-port-only.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/encryption-example.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-available/ocsp-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/certbot.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl-port-only.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/default-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/encryption-example.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/debian_apache_2_4/multiple_vhosts/apache2/sites-enabled/ocsp-ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/httpd.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/magic`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_default_settings.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_error_documents.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_languages.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_autoindex.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_log_config.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_mime.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mod_userdir.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/00_mpm.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/40_mod_ssl.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/modules.d/45_mod_dav.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_ssl_vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/00_default_vhost.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/apache2/vhosts.d/default_vhost.include`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/testdata/gentoo_apache/apache/conf.d/apache2`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tests/util.py` & `certbot-apache-2.9.0/certbot_apache/_internal/tests/util.py`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tls_configs/current-options-ssl-apache.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf` & `certbot-apache-2.9.0/certbot_apache/_internal/tls_configs/old-options-ssl-apache.conf`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/certbot_apache.egg-info/PKG-INFO` & `certbot-apache-2.9.0/certbot_apache.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-apache
-Version: 2.8.0
+Version: 2.9.0
 Summary: Apache plugin for Certbot
 Home-page: https://github.com/certbot/certbot
 Author: Certbot Project
 Author-email: certbot-dev@eff.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
@@ -13,24 +13,25 @@
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
 Requires-Dist: python-augeas
 Requires-Dist: setuptools>=41.6.0
 Provides-Extra: dev
 Requires-Dist: apacheconfig>=0.3.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
```

### Comparing `certbot-apache-2.8.0/certbot_apache.egg-info/SOURCES.txt` & `certbot-apache-2.9.0/certbot_apache.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `certbot-apache-2.8.0/setup.py` & `certbot-apache-2.9.0/setup.py`

 * *Files 2% similar despite different names*

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
@@ -39,14 +39,15 @@
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

