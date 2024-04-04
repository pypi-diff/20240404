# Comparing `tmp/Canaille-0.0.8.tar.gz` & `tmp/Canaille-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Canaille-0.0.8.tar", last modified: Tue Mar 15 13:17:30 2022, max compression
+gzip compressed data, was "Canaille-0.0.9.tar", max compression
```

## Comparing `Canaille-0.0.8.tar` & `Canaille-0.0.9.tar`

### file list

```diff
@@ -1,204 +1,150 @@
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.814062 Canaille-0.0.8/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/Canaille.egg-info/
--rw-rw-r--   0 camille   (1000) camille   (1000)     2360 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/PKG-INFO
--rw-rw-r--   0 camille   (1000) camille   (1000)     6688 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/SOURCES.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)        1 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/dependency_links.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)       51 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/entry_points.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)      136 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/requires.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)        9 2022-03-15 13:17:30.000000 Canaille-0.0.8/Canaille.egg-info/top_level.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)      166 2022-03-14 09:03:05.000000 Canaille-0.0.8/MANIFEST.in
--rw-rw-r--   0 camille   (1000) camille   (1000)     2360 2022-03-15 13:17:30.814062 Canaille-0.0.8/PKG-INFO
--rw-rw-r--   0 camille   (1000) camille   (1000)     1570 2021-12-02 10:06:31.000000 Canaille-0.0.8/README.md
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/
--rw-rw-r--   0 camille   (1000) camille   (1000)     5970 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/__init__.py
--rw-rw-r--   0 camille   (1000) camille   (1000)    17757 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/account.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     5205 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/admin.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     3957 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/apputils.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     1447 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/commands.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/conf/
--rw-rw-r--   0 camille   (1000) camille   (1000)     6063 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/conf/config.sample.toml
--rw-rw-r--   0 camille   (1000) camille   (1000)     1009 2021-09-30 09:33:15.000000 Canaille-0.0.8/canaille/conf/oauth-authorization-server.sample.json
--rw-rw-r--   0 camille   (1000) camille   (1000)     2229 2021-10-11 16:19:43.000000 Canaille-0.0.8/canaille/conf/openid-configuration.sample.json
--rw-rw-r--   0 camille   (1000) camille   (1000)     1946 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/configuration.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     2190 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/flaskutils.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     6577 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/forms.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     2888 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/groups.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     2530 2022-03-15 10:40:07.000000 Canaille-0.0.8/canaille/installation.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/ldap_backend/
--rw-rw-r--   0 camille   (1000) camille   (1000)        0 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/ldap_backend/__init__.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     5195 2022-03-15 10:40:07.000000 Canaille-0.0.8/canaille/ldap_backend/backend.py
--rw-rw-r--   0 camille   (1000) camille   (1000)    12312 2022-03-14 17:42:52.000000 Canaille-0.0.8/canaille/ldap_backend/ldapobject.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/ldap_backend/schemas/
--rw-rw-r--   0 camille   (1000) camille   (1000)    15415 2022-03-14 17:16:47.000000 Canaille-0.0.8/canaille/ldap_backend/schemas/oauth2-openldap.ldif
--rw-rw-r--   0 camille   (1000) camille   (1000)    15134 2022-03-14 09:03:05.000000 Canaille-0.0.8/canaille/ldap_backend/schemas/oauth2-openldap.schema
--rw-rw-r--   0 camille   (1000) camille   (1000)     3625 2022-02-14 10:14:28.000000 Canaille-0.0.8/canaille/mails.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     5816 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/models.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/oidc/
--rw-rw-r--   0 camille   (1000) camille   (1000)      416 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/oidc/__init__.py
--rw-rw-r--   0 camille   (1000) camille   (1000)      842 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/oidc/authorizations.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     8330 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/oidc/clients.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     1179 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/oidc/consents.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     6319 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/oidc/models.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     6610 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/oidc/oauth.py
--rw-rw-r--   0 camille   (1000) camille   (1000)    11356 2022-03-14 09:03:05.000000 Canaille-0.0.8/canaille/oidc/oauth2utils.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     1165 2022-03-14 17:26:09.000000 Canaille-0.0.8/canaille/oidc/tokens.py
--rw-rw-r--   0 camille   (1000) camille   (1000)      505 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/oidc/well_known.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/static/css/
--rw-rw-r--   0 camille   (1000) camille   (1000)     1267 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/static/css/base.css
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.774062 Canaille-0.0.8/canaille/static/datatables/
--rw-rw-r--   0 camille   (1000) camille   (1000)     1047 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/datatables/French.json
--rw-rw-r--   0 camille   (1000) camille   (1000)     2625 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/datatables/dataTables.semanticui.min.css
--rw-rw-r--   0 camille   (1000) camille   (1000)     3629 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/datatables/dataTables.semanticui.min.js
--rw-rw-r--   0 camille   (1000) camille   (1000)    13892 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/datatables/jquery.dataTables.min.css
--rw-rw-r--   0 camille   (1000) camille   (1000)    84647 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/datatables/jquery.dataTables.min.js
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.786063 Canaille-0.0.8/canaille/static/fomanticui/
--rw-rw-r--   0 camille   (1000) camille   (1000)  1665037 2021-09-30 09:33:15.000000 Canaille-0.0.8/canaille/static/fomanticui/semantic.css
--rw-rw-r--   0 camille   (1000) camille   (1000)   973084 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/semantic.js
--rw-rw-r--   0 camille   (1000) camille   (1000)  1373716 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/static/fomanticui/semantic.min.css
--rw-rw-r--   0 camille   (1000) camille   (1000)   369694 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/semantic.min.js
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.786063 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/
--rw-rw-r--   0 camille   (1000) camille   (1000)    40166 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    63983 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    39924 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    24676 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.woff
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/default/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.794062 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/
--rw-rw-r--   0 camille   (1000) camille   (1000)   133034 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)   715447 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)   132728 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    89824 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    76612 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)   202902 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    93888 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.otf
--rw-rw-r--   0 camille   (1000) camille   (1000)   896430 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)   202616 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)   103300 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    79444 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)    34390 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)   144170 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    34092 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    16800 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    13584 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff2
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.794062 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/images/
--rw-rw-r--   0 camille   (1000) camille   (1000)    28123 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/images/flags.png
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/github/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.798063 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/
--rw-rw-r--   0 camille   (1000) camille   (1000)    53604 2021-07-27 16:31:35.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons-local.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    87358 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    31740 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    17772 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.woff
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/material/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.798063 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/
--rw-rw-r--   0 camille   (1000) camille   (1000)   143258 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)   280687 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)   128180 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    57620 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    44300 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff2
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/fonts/
--rw-rw-r--   0 camille   (1000) camille   (1000)    26105 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    80884 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    59032 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    28052 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    22992 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)    27882 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    83985 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    62308 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    29920 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    24428 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)    27726 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    83394 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    60936 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    29836 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    24440 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)    26668 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.eot
--rw-rw-r--   0 camille   (1000) camille   (1000)    80331 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    60524 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.ttf
--rw-rw-r--   0 camille   (1000) camille   (1000)    28660 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.woff
--rw-rw-r--   0 camille   (1000) camille   (1000)    23484 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.woff2
--rw-rw-r--   0 camille   (1000) camille   (1000)     2797 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/fonts/lato.css
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/html5shiv/
--rw-rw-r--   0 camille   (1000) camille   (1000)     2731 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/static/html5shiv/html5shiv.min.js
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/img/
--rw-rw-r--   0 camille   (1000) camille   (1000)     4219 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-c.png
--rw-rw-r--   0 camille   (1000) camille   (1000)     1484 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-c.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)    20351 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-full.png
--rw-rw-r--   0 camille   (1000) camille   (1000)    12278 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-full.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)     7764 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-head.png
--rw-rw-r--   0 camille   (1000) camille   (1000)     5790 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-head.svg
--rw-rw-r--   0 camille   (1000) camille   (1000)     8749 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-label.png
--rw-rw-r--   0 camille   (1000) camille   (1000)     6835 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/img/canaille-label.svg
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/jquery/
--rw-rw-r--   0 camille   (1000) camille   (1000)    89501 2021-09-30 09:33:15.000000 Canaille-0.0.8/canaille/static/jquery/jquery.min.js
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/js/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.806063 Canaille-0.0.8/canaille/static/js/admin/
--rw-rw-r--   0 camille   (1000) camille   (1000)      239 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/js/admin/client_edit.js
--rw-rw-r--   0 camille   (1000) camille   (1000)      137 2021-12-14 15:47:41.000000 Canaille-0.0.8/canaille/static/js/base.js
--rw-rw-r--   0 camille   (1000) camille   (1000)      239 2021-09-30 09:33:15.000000 Canaille-0.0.8/canaille/static/js/confirm.js
--rw-rw-r--   0 camille   (1000) camille   (1000)      277 2021-12-02 10:06:31.000000 Canaille-0.0.8/canaille/static/js/invite.js
--rw-rw-r--   0 camille   (1000) camille   (1000)      584 2021-12-10 12:55:47.000000 Canaille-0.0.8/canaille/static/js/profile.js
--rw-rw-r--   0 camille   (1000) camille   (1000)      432 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/static/js/users.js
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/templates/
--rw-rw-r--   0 camille   (1000) camille   (1000)      910 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/about.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1712 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/error.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1673 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/firstlogin.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      292 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/templates/flask.j2
--rw-rw-r--   0 camille   (1000) camille   (1000)     3860 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/fomanticui.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1906 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/forgotten-password.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     3958 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/group.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1344 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/groups.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      125 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/home.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     5675 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/invite.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1802 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/login.html
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/templates/mail/
--rw-rw-r--   0 camille   (1000) camille   (1000)     2813 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/mail/admin.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     3471 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/mail/firstlogin.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      405 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/templates/mail/firstlogin.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)     3442 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/mail/invitation.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      307 2021-12-02 10:06:31.000000 Canaille-0.0.8/canaille/templates/mail/invitation.txt
--rw-rw-r--   0 camille   (1000) camille   (1000)     3538 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/mail/reset.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      332 2021-12-02 10:06:31.000000 Canaille-0.0.8/canaille/templates/mail/reset.txt
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/templates/oidc/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/templates/oidc/admin/
--rw-rw-r--   0 camille   (1000) camille   (1000)     1433 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/templates/oidc/admin/authorization_list.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      661 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/admin/authorization_view.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      375 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/admin/client_add.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     3450 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/admin/client_edit.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1746 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/admin/client_list.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1658 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/templates/oidc/admin/token_list.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     3014 2022-02-14 10:14:28.000000 Canaille-0.0.8/canaille/templates/oidc/admin/token_view.html
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/templates/oidc/user/
--rw-rw-r--   0 camille   (1000) camille   (1000)     2139 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/user/authorize.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     3250 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/oidc/user/consent_list.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     1730 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/password.html
--rw-rw-r--   0 camille   (1000) camille   (1000)    13055 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/profile.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      608 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/reset-password.html
--rw-rw-r--   0 camille   (1000) camille   (1000)     2498 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/userlist.html
--rw-rw-r--   0 camille   (1000) camille   (1000)      994 2022-01-24 16:21:53.000000 Canaille-0.0.8/canaille/templates/users.html
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/themes/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/themes/default/
--rw-rw-r--   0 camille   (1000) camille   (1000)     5221 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/themes/default/base.html
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/translations/
--rw-rw-r--   0 camille   (1000) camille   (1000)      525 2021-07-27 16:31:36.000000 Canaille-0.0.8/canaille/translations/README.md
--rw-rw-r--   0 camille   (1000) camille   (1000)      155 2021-12-02 10:06:31.000000 Canaille-0.0.8/canaille/translations/babel.cfg
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/canaille/translations/fr/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.810063 Canaille-0.0.8/canaille/translations/fr/LC_MESSAGES/
--rw-rw-r--   0 camille   (1000) camille   (1000)    24231 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/translations/fr/LC_MESSAGES/messages.mo
--rw-rw-r--   0 camille   (1000) camille   (1000)    43680 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/translations/fr/LC_MESSAGES/messages.po
--rw-rw-r--   0 camille   (1000) camille   (1000)    26933 2022-03-03 08:46:27.000000 Canaille-0.0.8/canaille/translations/messages.pot
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.814062 Canaille-0.0.8/doc/
--rw-rw-r--   0 camille   (1000) camille   (1000)        0 2021-07-27 16:31:36.000000 Canaille-0.0.8/doc/__init__.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     2348 2022-01-24 16:21:53.000000 Canaille-0.0.8/doc/conf.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     2467 2022-03-15 13:17:30.814062 Canaille-0.0.8/setup.cfg
--rw-rw-r--   0 camille   (1000) camille   (1000)       39 2021-07-27 16:31:36.000000 Canaille-0.0.8/setup.py
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.770063 Canaille-0.0.8/tests/
-drwxrwxr-x   0 camille   (1000) camille   (1000)        0 2022-03-15 13:17:30.814062 Canaille-0.0.8/tests/commands/
--rw-rw-r--   0 camille   (1000) camille   (1000)        0 2021-12-02 10:06:31.000000 Canaille-0.0.8/tests/commands/__init__.py
--rw-rw-r--   0 camille   (1000) camille   (1000)      344 2022-03-15 10:40:07.000000 Canaille-0.0.8/tests/commands/test_check.py
--rw-rw-r--   0 camille   (1000) camille   (1000)     5459 2022-03-15 10:40:07.000000 Canaille-0.0.8/tests/commands/test_install.py
+-rw-r--r--   0        0        0     1056 2022-06-05 16:00:54.343609 Canaille-0.0.9/LICENSE.rst
+-rw-r--r--   0        0        0     1617 2022-04-06 07:27:27.018678 Canaille-0.0.9/README.md
+-rw-r--r--   0        0        0      250 2022-05-18 14:49:49.577814 Canaille-0.0.9/build.py
+-rw-r--r--   0        0        0     6099 2022-04-06 14:31:44.888084 Canaille-0.0.9/canaille/__init__.py
+-rw-r--r--   0        0        0    18734 2022-05-18 09:12:31.533414 Canaille-0.0.9/canaille/account.py
+-rw-r--r--   0        0        0     5205 2022-04-06 07:27:27.018678 Canaille-0.0.9/canaille/admin.py
+-rw-r--r--   0        0        0     3957 2022-01-01 10:22:02.261144 Canaille-0.0.9/canaille/apputils.py
+-rw-r--r--   0        0        0     1447 2022-04-06 07:27:27.018678 Canaille-0.0.9/canaille/commands.py
+-rw-r--r--   0        0        0     6438 2022-04-13 15:11:03.255524 Canaille-0.0.9/canaille/conf/config.sample.toml
+-rw-r--r--   0        0        0     1009 2021-09-15 17:07:33.036792 Canaille-0.0.9/canaille/conf/oauth-authorization-server.sample.json
+-rw-r--r--   0        0        0     2229 2021-10-03 11:45:12.656547 Canaille-0.0.9/canaille/conf/openid-configuration.sample.json
+-rw-r--r--   0        0        0     1946 2022-01-23 18:35:16.067158 Canaille-0.0.9/canaille/configuration.py
+-rw-r--r--   0        0        0     2190 2022-04-06 07:27:27.018678 Canaille-0.0.9/canaille/flaskutils.py
+-rw-r--r--   0        0        0     6580 2022-04-06 15:35:38.025488 Canaille-0.0.9/canaille/forms.py
+-rw-r--r--   0        0        0     2912 2022-04-06 07:27:27.018678 Canaille-0.0.9/canaille/groups.py
+-rw-r--r--   0        0        0     2530 2022-05-06 13:15:46.387907 Canaille-0.0.9/canaille/installation.py
+-rw-r--r--   0        0        0        0 2022-01-23 18:35:16.067158 Canaille-0.0.9/canaille/ldap_backend/__init__.py
+-rw-r--r--   0        0        0     5241 2022-05-18 14:57:52.961703 Canaille-0.0.9/canaille/ldap_backend/backend.py
+-rw-r--r--   0        0        0    12312 2022-04-06 07:27:27.018678 Canaille-0.0.9/canaille/ldap_backend/ldapobject.py
+-rw-r--r--   0        0        0    15813 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/ldap_backend/schemas/oauth2-openldap.ldif
+-rw-r--r--   0        0        0    15547 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/ldap_backend/schemas/oauth2-openldap.schema
+-rw-r--r--   0        0        0     3625 2022-04-06 07:27:27.022011 Canaille-0.0.9/canaille/mails.py
+-rw-r--r--   0        0        0     5801 2022-05-18 14:57:52.961703 Canaille-0.0.9/canaille/models.py
+-rw-r--r--   0        0        0      416 2022-01-23 12:10:45.884376 Canaille-0.0.9/canaille/oidc/__init__.py
+-rw-r--r--   0        0        0      842 2022-04-06 07:27:27.022011 Canaille-0.0.9/canaille/oidc/authorizations.py
+-rw-r--r--   0        0        0     8926 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/oidc/clients.py
+-rw-r--r--   0        0        0     1179 2022-01-23 18:35:16.067158 Canaille-0.0.9/canaille/oidc/consents.py
+-rw-r--r--   0        0        0      113 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/oidc/forms.py
+-rw-r--r--   0        0        0     6496 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/oidc/models.py
+-rw-r--r--   0        0        0    10645 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/oidc/oauth.py
+-rw-r--r--   0        0        0    11335 2022-04-13 15:11:03.258857 Canaille-0.0.9/canaille/oidc/oauth2utils.py
+-rw-r--r--   0        0        0     1190 2022-04-06 07:27:27.022011 Canaille-0.0.9/canaille/oidc/tokens.py
+-rw-r--r--   0        0        0      505 2022-01-23 12:10:45.884376 Canaille-0.0.9/canaille/oidc/well_known.py
+-rw-r--r--   0        0        0     1267 2022-04-06 07:27:27.022011 Canaille-0.0.9/canaille/static/css/base.css
+-rw-r--r--   0        0        0     1047 2021-12-22 10:09:00.103938 Canaille-0.0.9/canaille/static/datatables/French.json
+-rw-r--r--   0        0        0     2625 2020-10-23 07:10:11.093586 Canaille-0.0.9/canaille/static/datatables/dataTables.semanticui.min.css
+-rw-r--r--   0        0        0     3629 2020-10-23 07:10:11.093586 Canaille-0.0.9/canaille/static/datatables/dataTables.semanticui.min.js
+-rw-r--r--   0        0        0    13892 2020-10-23 07:10:11.093586 Canaille-0.0.9/canaille/static/datatables/jquery.dataTables.min.css
+-rw-r--r--   0        0        0    84647 2020-10-23 07:10:11.093586 Canaille-0.0.9/canaille/static/datatables/jquery.dataTables.min.js
+-rw-r--r--   0        0        0  1665037 2021-09-17 09:44:54.995406 Canaille-0.0.9/canaille/static/fomanticui/semantic.css
+-rw-r--r--   0        0        0   973084 2021-12-22 10:09:00.107271 Canaille-0.0.9/canaille/static/fomanticui/semantic.js
+-rw-r--r--   0        0        0  1373716 2022-04-06 07:27:27.025343 Canaille-0.0.9/canaille/static/fomanticui/semantic.min.css
+-rw-r--r--   0        0        0   369694 2021-12-22 10:09:00.113938 Canaille-0.0.9/canaille/static/fomanticui/semantic.min.js
+-rw-r--r--   0        0        0    40166 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.eot
+-rw-r--r--   0        0        0    63983 2021-12-22 10:09:00.113938 Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.svg
+-rw-r--r--   0        0        0    39924 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.ttf
+-rw-r--r--   0        0        0    24676 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.woff
+-rw-r--r--   0        0        0   133034 2020-10-28 17:31:37.775141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.eot
+-rw-r--r--   0        0        0   715447 2021-12-22 10:09:00.117271 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.svg
+-rw-r--r--   0        0        0   132728 2020-10-28 17:31:37.785141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.ttf
+-rw-r--r--   0        0        0    89824 2020-10-28 17:31:37.788474 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff
+-rw-r--r--   0        0        0    76612 2020-10-28 17:31:37.791808 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff2
+-rw-r--r--   0        0        0   202902 2020-10-28 17:31:37.795141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.eot
+-rw-r--r--   0        0        0    93888 2020-10-23 07:10:11.133586 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.otf
+-rw-r--r--   0        0        0   896430 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.svg
+-rw-r--r--   0        0        0   202616 2020-10-28 17:31:37.801807 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.ttf
+-rw-r--r--   0        0        0   103300 2020-10-28 17:31:37.801807 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff
+-rw-r--r--   0        0        0    79444 2020-10-28 17:31:37.801807 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff2
+-rw-r--r--   0        0        0    34390 2020-10-28 17:31:37.801807 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.eot
+-rw-r--r--   0        0        0   144170 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.svg
+-rw-r--r--   0        0        0    34092 2020-10-28 17:31:37.801807 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.ttf
+-rw-r--r--   0        0        0    16800 2020-10-28 17:31:37.805141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff
+-rw-r--r--   0        0        0    13584 2020-10-28 17:31:37.805141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff2
+-rw-r--r--   0        0        0    28123 2020-10-28 17:31:37.775141 Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/images/flags.png
+-rw-r--r--   0        0        0    53604 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons-local.ttf
+-rw-r--r--   0        0        0    87358 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.svg
+-rw-r--r--   0        0        0    31740 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.ttf
+-rw-r--r--   0        0        0    17772 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.woff
+-rw-r--r--   0        0        0   143258 2021-08-23 19:57:21.436055 Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.eot
+-rw-r--r--   0        0        0   280687 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.svg
+-rw-r--r--   0        0        0   128180 2021-08-23 19:57:21.439388 Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.ttf
+-rw-r--r--   0        0        0    57620 2021-08-23 19:57:21.439388 Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff
+-rw-r--r--   0        0        0    44300 2021-08-23 19:57:21.439388 Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff2
+-rw-r--r--   0        0        0    26105 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.eot
+-rw-r--r--   0        0        0    80884 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.svg
+-rw-r--r--   0        0        0    59032 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.ttf
+-rw-r--r--   0        0        0    28052 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.woff
+-rw-r--r--   0        0        0    22992 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.woff2
+-rw-r--r--   0        0        0    27882 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.eot
+-rw-r--r--   0        0        0    83985 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.svg
+-rw-r--r--   0        0        0    62308 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.ttf
+-rw-r--r--   0        0        0    29920 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.woff
+-rw-r--r--   0        0        0    24428 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.woff2
+-rw-r--r--   0        0        0    27726 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.eot
+-rw-r--r--   0        0        0    83394 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.svg
+-rw-r--r--   0        0        0    60936 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.ttf
+-rw-r--r--   0        0        0    29836 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.woff
+-rw-r--r--   0        0        0    24440 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.woff2
+-rw-r--r--   0        0        0    26668 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.eot
+-rw-r--r--   0        0        0    80331 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.svg
+-rw-r--r--   0        0        0    60524 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.ttf
+-rw-r--r--   0        0        0    28660 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.woff
+-rw-r--r--   0        0        0    23484 2020-10-28 14:03:50.000000 Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.woff2
+-rw-r--r--   0        0        0     2797 2020-10-28 15:06:58.152649 Canaille-0.0.9/canaille/static/fonts/lato.css
+-rw-r--r--   0        0        0     2731 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/static/html5shiv/html5shiv.min.js
+-rw-r--r--   0        0        0     4219 2020-11-05 16:47:07.039061 Canaille-0.0.9/canaille/static/img/canaille-c.png
+-rw-r--r--   0        0        0     1484 2020-11-05 16:47:07.042394 Canaille-0.0.9/canaille/static/img/canaille-c.svg
+-rw-r--r--   0        0        0    20351 2020-11-05 11:13:07.176919 Canaille-0.0.9/canaille/static/img/canaille-full.png
+-rw-r--r--   0        0        0    12278 2020-11-05 11:13:07.176919 Canaille-0.0.9/canaille/static/img/canaille-full.svg
+-rw-r--r--   0        0        0     7764 2020-11-05 11:43:54.187998 Canaille-0.0.9/canaille/static/img/canaille-head.png
+-rw-r--r--   0        0        0     5790 2020-11-05 11:13:07.176919 Canaille-0.0.9/canaille/static/img/canaille-head.svg
+-rw-r--r--   0        0        0     8749 2020-11-05 11:13:07.176919 Canaille-0.0.9/canaille/static/img/canaille-label.png
+-rw-r--r--   0        0        0     6835 2020-11-05 11:13:07.176919 Canaille-0.0.9/canaille/static/img/canaille-label.svg
+-rw-r--r--   0        0        0    89501 2021-03-02 17:27:20.000000 Canaille-0.0.9/canaille/static/jquery/jquery.min.js
+-rw-r--r--   0        0        0      239 2020-11-23 16:07:40.895243 Canaille-0.0.9/canaille/static/js/admin/client_edit.js
+-rw-r--r--   0        0        0      137 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/static/js/base.js
+-rw-r--r--   0        0        0      239 2021-08-23 19:57:21.439388 Canaille-0.0.9/canaille/static/js/confirm.js
+-rw-r--r--   0        0        0      277 2021-12-01 11:22:16.439438 Canaille-0.0.9/canaille/static/js/invite.js
+-rw-r--r--   0        0        0      584 2021-12-10 18:31:01.193001 Canaille-0.0.9/canaille/static/js/profile.js
+-rw-r--r--   0        0        0      432 2020-10-23 07:10:11.143586 Canaille-0.0.9/canaille/static/js/users.js
+-rw-r--r--   0        0        0      910 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/templates/about.html
+-rw-r--r--   0        0        0     1712 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/templates/error.html
+-rw-r--r--   0        0        0     1673 2021-12-22 10:09:00.120605 Canaille-0.0.9/canaille/templates/firstlogin.html
+-rw-r--r--   0        0        0      292 2020-10-31 16:56:45.597111 Canaille-0.0.9/canaille/templates/flask.j2
+-rw-r--r--   0        0        0     3856 2022-04-06 07:27:27.025343 Canaille-0.0.9/canaille/templates/fomanticui.html
+-rw-r--r--   0        0        0     1906 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/forgotten-password.html
+-rw-r--r--   0        0        0     3958 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/group.html
+-rw-r--r--   0        0        0     1344 2021-12-31 17:22:23.094025 Canaille-0.0.9/canaille/templates/groups.html
+-rw-r--r--   0        0        0      125 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/home.html
+-rw-r--r--   0        0        0     5675 2022-01-05 11:14:59.949728 Canaille-0.0.9/canaille/templates/invite.html
+-rw-r--r--   0        0        0     1828 2022-04-06 14:31:44.888084 Canaille-0.0.9/canaille/templates/login.html
+-rw-r--r--   0        0        0     2813 2022-01-23 12:10:45.884376 Canaille-0.0.9/canaille/templates/mail/admin.html
+-rw-r--r--   0        0        0     3471 2022-01-01 10:22:02.261144 Canaille-0.0.9/canaille/templates/mail/firstlogin.html
+-rw-r--r--   0        0        0      405 2020-11-23 08:14:34.269702 Canaille-0.0.9/canaille/templates/mail/firstlogin.txt
+-rw-r--r--   0        0        0     3442 2022-01-01 10:22:02.261144 Canaille-0.0.9/canaille/templates/mail/invitation.html
+-rw-r--r--   0        0        0      307 2021-12-01 11:22:16.439438 Canaille-0.0.9/canaille/templates/mail/invitation.txt
+-rw-r--r--   0        0        0     3538 2022-01-01 10:22:02.264477 Canaille-0.0.9/canaille/templates/mail/reset.html
+-rw-r--r--   0        0        0      332 2021-12-01 08:40:00.844587 Canaille-0.0.9/canaille/templates/mail/reset.txt
+-rw-r--r--   0        0        0     1437 2022-04-06 07:27:27.025343 Canaille-0.0.9/canaille/templates/oidc/admin/authorization_list.html
+-rw-r--r--   0        0        0      661 2022-01-23 12:10:45.884376 Canaille-0.0.9/canaille/templates/oidc/admin/authorization_view.html
+-rw-r--r--   0        0        0      375 2022-01-23 12:10:45.884376 Canaille-0.0.9/canaille/templates/oidc/admin/client_add.html
+-rw-r--r--   0        0        0     3450 2022-01-23 18:35:16.070491 Canaille-0.0.9/canaille/templates/oidc/admin/client_edit.html
+-rw-r--r--   0        0        0     1746 2022-01-23 18:35:16.070491 Canaille-0.0.9/canaille/templates/oidc/admin/client_list.html
+-rw-r--r--   0        0        0     1658 2022-04-06 07:27:27.025343 Canaille-0.0.9/canaille/templates/oidc/admin/token_list.html
+-rw-r--r--   0        0        0     3014 2022-04-06 07:27:27.025343 Canaille-0.0.9/canaille/templates/oidc/admin/token_view.html
+-rw-r--r--   0        0        0     2139 2022-05-20 12:13:09.555811 Canaille-0.0.9/canaille/templates/oidc/user/authorize.html
+-rw-r--r--   0        0        0     3250 2022-01-23 18:35:16.070491 Canaille-0.0.9/canaille/templates/oidc/user/consent_list.html
+-rw-r--r--   0        0        0     1712 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/templates/oidc/user/logout.html
+-rw-r--r--   0        0        0     1756 2022-04-06 14:31:44.888084 Canaille-0.0.9/canaille/templates/password.html
+-rw-r--r--   0        0        0    13145 2022-04-06 16:13:12.619993 Canaille-0.0.9/canaille/templates/profile.html
+-rw-r--r--   0        0        0      608 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/reset-password.html
+-rw-r--r--   0        0        0     2498 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/userlist.html
+-rw-r--r--   0        0        0      994 2021-12-22 10:09:00.123938 Canaille-0.0.9/canaille/templates/users.html
+-rw-r--r--   0        0        0     5321 2022-04-06 16:13:12.623327 Canaille-0.0.9/canaille/themes/default/base.html
+-rw-r--r--   0        0        0      525 2021-01-01 14:12:24.184502 Canaille-0.0.9/canaille/translations/README.md
+-rw-r--r--   0        0        0      105 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/translations/babel.cfg
+-rw-r--r--   0        0        0    45426 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/translations/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0    28032 2022-06-05 16:00:54.343609 Canaille-0.0.9/canaille/translations/messages.pot
+-rw-r--r--   0        0        0     2747 2022-06-05 16:25:35.887613 Canaille-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3225 2022-06-05 16:26:59.852885 Canaille-0.0.9/PKG-INFO
```

### Comparing `Canaille-0.0.8/README.md` & `Canaille-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     <img src="doc/_static/consent.png" width="225" alt="Canaille consent page" />
 </div>
 
 # Try it!
 
 ```bash
 cd demo
-./run.sh
+./run.sh # or `docker-compose up` to run it with docker
 ```
 
 # Documentation
 
 ⚠ Canaille is under heavy development and may not fit a production environment yet. However, [contributions](CONTRIBUTING.rst) are welcome! ⚠
 
 - Please have a look on our [documentation](https://canaille.readthedocs.io);
```

### Comparing `Canaille-0.0.8/canaille/__init__.py` & `Canaille-0.0.9/canaille/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,14 +175,17 @@
 
         @app.context_processor
         def global_processor():
             from .flaskutils import current_user
 
             return {
                 "has_smtp": "SMTP" in app.config,
+                "has_password_recovery": app.config.get(
+                    "ENABLE_PASSWORD_RECOVERY", True
+                ),
                 "logo_url": app.config.get("LOGO"),
                 "favicon_url": app.config.get("FAVICON", app.config.get("LOGO")),
                 "website_name": app.config.get("NAME", "Canaille"),
                 "user": current_user(),
                 "menu": True,
             }
```

### Comparing `Canaille-0.0.8/canaille/account.py` & `Canaille-0.0.9/canaille/account.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,17 +44,28 @@
 
 
 bp = Blueprint("account", __name__)
 
 
 @bp.route("/")
 def index():
-    if not current_user():
+    user = current_user()
+
+    if not user:
         return redirect(url_for("account.login"))
-    return redirect(url_for("account.profile_edition", username=current_user().uid[0]))
+
+    if user.can_edit_self or user.can_manage_users:
+        return redirect(
+            url_for("account.profile_edition", username=current_user().uid[0])
+        )
+
+    if user.can_use_oidc:
+        return redirect(url_for("oidc.consents.consents"))
+
+    return redirect(url_for("account.about"))
 
 
 @bp.route("/about")
 def about():
     try:
         version = pkg_resources.get_distribution("canaille").version
     except pkg_resources.DistributionNotFound:
@@ -129,15 +140,16 @@
         user.logout()
     return redirect("/")
 
 
 @bp.route("/firstlogin/<uid>", methods=("GET", "POST"))
 def firstlogin(uid):
     user = User.get(uid)
-    user and not user.has_password() or abort(404)
+    if not user or user.has_password():
+        abort(404)
 
     form = ForgottenPasswordForm(request.form or None, data={"login": uid})
     if not request.form:
         return render_template("firstlogin.html", form=form, uid=uid)
 
     if not form.validate():
         flash(_("Could not send the password initialization link."), "error")
@@ -375,38 +387,47 @@
 
     return user
 
 
 @bp.route("/profile/<username>", methods=("GET", "POST"))
 @user_needed()
 def profile_edition(user, username):
-    user.can_manage_users or username == user.uid[0] or abort(403)
+    if not user.can_manage_users and not (
+        user.can_edit_self and username == user.uid[0]
+    ):
+        abort(403)
 
     if request.method == "GET" or request.form.get("action") == "edit":
         return profile_edit(user, username)
 
     if request.form.get("action") == "delete":
         return profile_delete(user, username)
 
     if request.form.get("action") == "password-initialization-mail":
-        user = User.get(username) or abort(404)
+        user = User.get(username)
+        if not user:
+            abort(404)
+
         if send_password_initialization_mail(user):
             flash(
                 _(
                     "A password initialization link has been sent at the user email address. It should be received within 10 minutes."
                 ),
                 "success",
             )
         else:
             flash(_("Could not send the password initialization email"), "error")
 
         return profile_edit(user, username)
 
     if request.form.get("action") == "password-reset-mail":
-        user = User.get(username) or abort(404)
+        user = User.get(username)
+        if not user:
+            abort(404)
+
         if send_password_reset_mail(user):
             flash(
                 _(
                     "A password reset link has been sent at the user email address. It should be received within 10 minutes."
                 ),
                 "success",
             )
@@ -418,18 +439,21 @@
     abort(400)
 
 
 def profile_edit(editor, username):
     menuitem = "profile" if username == editor.uid[0] else "users"
     fields = editor.read | editor.write
     if username != editor.uid[0]:
-        user = User.get(username) or abort(404)
+        user = User.get(username)
     else:
         user = editor
 
+    if not user:
+        abort(404)
+
     data = {
         k: getattr(user, k)[0]
         if getattr(user, k) and isinstance(getattr(user, k), list)
         else getattr(user, k) or ""
         for k in fields
         if hasattr(user, k)
     }
@@ -484,71 +508,91 @@
 
 
 def profile_delete(user, username):
     self_deletion = username == user.uid[0]
     if self_deletion:
         user.logout()
     else:
-        user = User.get(username) or abort(404)
+        user = User.get(username)
+
+    if not user:
+        abort(404)
 
     flash(_("The user %(user)s has been sucessfuly deleted", user=user.name), "success")
     user.delete()
 
     if self_deletion:
         return redirect(url_for("account.index"))
     return redirect(url_for("account.users"))
 
 
 @bp.route("/impersonate/<username>")
 @permissions_needed("impersonate_users")
 def impersonate(user, username):
-    u = User.get(username) or abort(404)
-    u.login()
+    puppet = User.get(username)
+    if not puppet:
+        abort(404)
+
+    puppet.login()
     return redirect(url_for("account.index"))
 
 
 @bp.route("/reset", methods=["GET", "POST"])
 @smtp_needed()
 def forgotten():
+    if not current_app.config.get("ENABLE_PASSWORD_RECOVERY", True):
+        abort(404)
+
     form = ForgottenPasswordForm(request.form)
     if not request.form:
         return render_template("forgotten-password.html", form=form)
 
     if not form.validate():
         flash(_("Could not send the password reset link."), "error")
         return render_template("forgotten-password.html", form=form)
 
     user = User.get(form.login.data)
+    success_message = _(
+        "A password reset link has been sent at your email address. You should receive it within 10 minutes."
+    )
+    if current_app.config.get("HIDE_INVALID_LOGINS", True) and (
+        not user or not user.can_edit_self
+    ):
+        flash(success_message, "success")
+        return render_template("forgotten-password.html", form=form)
 
-    if not user:
+    if not user.can_edit_self:
         flash(
             _(
-                "A password reset link has been sent at your email address. You should receive it within 10 minutes."
+                "The user '%(user)s' does not have permissions to update their password. "
+                "We cannot send a password reset email.",
+                user=user.name,
             ),
             "success",
         )
         return render_template("forgotten-password.html", form=form)
 
     success = send_password_reset_mail(user)
 
     if success:
+        flash(success_message, "success")
+    else:
         flash(
-            _(
-                "A password reset link has been sent at your email address. You should receive it within 10 minutes."
-            ),
-            "success",
+            _("We encountered an issue while we sent the password recovery email."),
+            "error",
         )
-    else:
-        flash(_("Could not reset your password"), "error")
 
     return render_template("forgotten-password.html", form=form)
 
 
 @bp.route("/reset/<uid>/<hash>", methods=["GET", "POST"])
 def reset(uid, hash):
+    if not current_app.config.get("ENABLE_PASSWORD_RECOVERY", True):
+        abort(404)
+
     form = PasswordResetForm(request.form)
     user = User.get(uid)
 
     if not user or hash != profile_hash(
         user.uid[0], user.mail[0], user.userPassword[0] if user.has_password() else ""
     ):
         flash(
```

### Comparing `Canaille-0.0.8/canaille/admin.py` & `Canaille-0.0.9/canaille/admin.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/apputils.py` & `Canaille-0.0.9/canaille/apputils.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/commands.py` & `Canaille-0.0.9/canaille/commands.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/conf/config.sample.toml` & `Canaille-0.0.9/canaille/conf/config.sample.toml`

 * *Files 13% similar despite different names*

```diff
@@ -29,20 +29,26 @@
 # with your production URLs.
 OAUTH2_METADATA_FILE = "canaille/conf/oauth-authorization-server.json"
 OIDC_METADATA_FILE = "canaille/conf/openid-configuration.json"
 
 # If you have a sentry instance, you can set its dsn here:
 # SENTRY_DSN = "https://examplePublicKey@o0.ingest.sentry.io/0"
 
-# If HIDE_INVALID_LOGINS is set to true, when a user tries to sign in with
-# an invalid login, a message is shown saying that the login does not
-# exist. If HIDE_INVALID_LOGINS is set to false (the default) a message is
-# shown saying that the password is wrong, but does not give a clue
-# wether the login exists or not.
-# HIDE_INVALID_LOGINS = false
+# If HIDE_INVALID_LOGINS is set to true (the default), when an user
+# tries to sign in with an invalid login, a message is shown indicating
+# that the password is wrong, but does not give a clue wether the login
+# exists or not.
+# If HIDE_INVALID_LOGINS is set to false, when an user tries to sign in with
+# an invalid login, a message is shown indicating that the login does not
+# exist.
+# HIDE_INVALID_LOGINS = true
+
+# If ENABLE_PASSWORD_RECOVERY is false, then users cannot ask for a password
+# recovery link by email. This option is true by default.
+# ENABLE_PASSWORD_RECOVERY = true
 
 # The validity duration of registration invitations, in seconds.
 # Defaults to 2 days
 # INVITATION_EXPIRATION = 172800
 
 [LOGGING]
 # LEVEL can be one value among:
@@ -101,26 +107,27 @@
 # filter against group membership.
 # Here are some examples
 #     FILTER = 'uid=admin'
 #     FILTER = 'memberof=cn=admins,ou=groups,dc=mydomain,dc=tld'
 #
 # The 'PERMISSIONS' parameter that is an list of items the users in the access
 # control will be able to manage. 'PERMISSIONS' is optionnal. Values can be:
+# - "edit_self" to allow users to edit their own profile
 # - "use_oidc" to allow OpenID Connect authentication
 # - "manage_oidc" to allow OpenID Connect client managements
 # - "manage_users" to allow other users management
 # - "manage_groups" to allow group edition and creation
 # - "delete_account" allows a user to delete his own account. If used with
 #                    manage_users, the user can delete any account
 # - "impersonate_users" to allow a user to take the identity of another user
 #
 # The 'READ' and 'WRITE' attributes are the LDAP attributes of the user
 # object that users will be able to read and/or write.
 [ACL.DEFAULT]
-PERMISSIONS = ["use_oidc"]
+PERMISSIONS = ["edit_self", "use_oidc"]
 READ = ["uid", "groups"]
 WRITE = ["givenName", "sn", "userPassword", "telephoneNumber", "jpegPhoto", "mail", "labeledURI"]
 
 [ACL.ADMIN]
 FILTER = "memberof=cn=moderators,ou=groups,dc=mydomain,dc=tld"
 PERMISSIONS = [
     "manage_users",
@@ -135,14 +142,16 @@
 # openssl genrsa -out private.pem 4096
 # openssl rsa -in private.pem -pubout -outform PEM -out public.pem
 [JWT]
 # The path to the private key.
 PRIVATE_KEY = "canaille/conf/private.pem"
 # The path to the public key.
 PUBLIC_KEY = "canaille/conf/public.pem"
+# The URI of the identity provider
+ISS = "https://auth.mydomain.tld"
 # The key type parameter
 # KTY = "RSA"
 # The key algorithm
 # ALG = "RS256"
 # The time the JWT will be valid, in seconds
 # EXP = 3600
```

### Comparing `Canaille-0.0.8/canaille/conf/oauth-authorization-server.sample.json` & `Canaille-0.0.9/canaille/conf/oauth-authorization-server.sample.json`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/conf/openid-configuration.sample.json` & `Canaille-0.0.9/canaille/conf/openid-configuration.sample.json`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/configuration.py` & `Canaille-0.0.9/canaille/configuration.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/flaskutils.py` & `Canaille-0.0.9/canaille/flaskutils.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/forms.py` & `Canaille-0.0.9/canaille/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     if Group.get(field.data):
         raise wtforms.ValidationError(
             _("The group '{group}' already exists").format(group=field.data)
         )
 
 
 def existing_login(form, field):
-    if current_app.config.get("HIDE_INVALID_LOGINS", False) and not User.get(
+    if not current_app.config.get("HIDE_INVALID_LOGINS", True) and not User.get(
         field.data
     ):
         raise wtforms.ValidationError(
             _("The login '{login}' does not exist").format(login=field.data)
         )
```

### Comparing `Canaille-0.0.8/canaille/groups.py` & `Canaille-0.0.9/canaille/groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 
     return render_template("group.html", form=form, edited_group=None, members=None)
 
 
 @bp.route("/<groupname>", methods=("GET", "POST"))
 @permissions_needed("manage_groups")
 def group(user, groupname):
-    group = Group.get(groupname) or abort(404)
+    group = Group.get(groupname)
+
+    if not group:
+        abort(404)
 
     if request.method == "GET" or request.form.get("action") == "edit":
         return edit_group(group)
 
     if request.form.get("action") == "delete":
         return delete_group(group)
```

### Comparing `Canaille-0.0.8/canaille/installation.py` & `Canaille-0.0.9/canaille/installation.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/ldap_backend/backend.py` & `Canaille-0.0.9/canaille/ldap_backend/backend.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,34 @@
 from canaille.configuration import ConfigurationException
 from flask import g
 from flask import render_template
 from flask import request
 from flask_babel import gettext as _
 
 
-def setup_ldap_models(app):
+def setup_ldap_models(config):
     from .ldapobject import LDAPObject
     from ..models import Group
     from ..models import User
 
-    LDAPObject.root_dn = app.config["LDAP"]["ROOT_DN"]
+    LDAPObject.root_dn = config["LDAP"]["ROOT_DN"]
 
-    user_base = app.config["LDAP"]["USER_BASE"]
-    if user_base.endswith(app.config["LDAP"]["ROOT_DN"]):
-        user_base = user_base[: -len(app.config["LDAP"]["ROOT_DN"]) - 1]
+    user_base = config["LDAP"]["USER_BASE"]
+    if user_base.endswith(config["LDAP"]["ROOT_DN"]):
+        user_base = user_base[: -len(config["LDAP"]["ROOT_DN"]) - 1]
     User.base = user_base
-    User.id = app.config["LDAP"].get("USER_ID_ATTRIBUTE", User.DEFAULT_ID_ATTRIBUTE)
-    User.object_class = [
-        app.config["LDAP"].get("USER_CLASS", User.DEFAULT_OBJECT_CLASS)
-    ]
-
-    group_base = app.config["LDAP"].get("GROUP_BASE")
-    if group_base.endswith(app.config["LDAP"]["ROOT_DN"]):
-        group_base = group_base[: -len(app.config["LDAP"]["ROOT_DN"]) - 1]
+    User.id = config["LDAP"].get("USER_ID_ATTRIBUTE", User.DEFAULT_ID_ATTRIBUTE)
+    User.object_class = [config["LDAP"].get("USER_CLASS", User.DEFAULT_OBJECT_CLASS)]
+
+    group_base = config["LDAP"].get("GROUP_BASE")
+    if group_base.endswith(config["LDAP"]["ROOT_DN"]):
+        group_base = group_base[: -len(config["LDAP"]["ROOT_DN"]) - 1]
     Group.base = group_base
-    Group.id = app.config["LDAP"].get("GROUP_ID_ATTRIBUTE", Group.DEFAULT_ID_ATTRIBUTE)
-    Group.object_class = [
-        app.config["LDAP"].get("GROUP_CLASS", Group.DEFAULT_OBJECT_CLASS)
-    ]
+    Group.id = config["LDAP"].get("GROUP_ID_ATTRIBUTE", Group.DEFAULT_ID_ATTRIBUTE)
+    Group.object_class = [config["LDAP"].get("GROUP_CLASS", Group.DEFAULT_OBJECT_CLASS)]
 
 
 def setup_backend(app):
     try:  # pragma: no-cover
         if request.endpoint == "static":
             return
     except RuntimeError:
@@ -80,28 +76,31 @@
                 description=message,
             ),
             500,
         )
 
 
 def teardown_backend(app):
-    if "ldap" in g:
+    if g.get("ldap"):
         g.ldap.unbind_s()
+        g.ldap = None
 
 
 def init_backend(app):
-    setup_ldap_models(app)
+    setup_ldap_models(app.config)
 
     @app.before_request
     def before_request():
-        return setup_backend(app)
+        if not app.config["TESTING"]:
+            return setup_backend(app)
 
     @app.after_request
     def after_request(response):
-        teardown_backend(app)
+        if not app.config["TESTING"]:
+            teardown_backend(app)
         return response
 
 
 def validate_configuration(config):
     from canaille.models import User, Group
 
     try:
```

### Comparing `Canaille-0.0.8/canaille/ldap_backend/ldapobject.py` & `Canaille-0.0.9/canaille/ldap_backend/ldapobject.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/ldap_backend/schemas/oauth2-openldap.ldif` & `Canaille-0.0.9/canaille/ldap_backend/schemas/oauth2-openldap.ldif`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,22 @@
         EQUALITY caseExactMatch
         ORDERING caseExactOrderingMatch
         SUBSTR caseExactSubstringsMatch
         SYNTAX 1.3.6.1.4.1.1466.115.121.1.15
         SINGLE-VALUE
         USAGE userApplications
         X-ORIGIN 'OAuth 2.0' )
+olcAttributeTypes: ( 1.3.6.1.4.1.56207.1.1.39 NAME 'oauthPostLogoutRedirectURI'
+        DESC 'OAuth 2.0 Post logout redirection URI'
+        EQUALITY caseIgnoreMatch
+        ORDERING caseIgnoreOrderingMatch
+        SUBSTR caseIgnoreSubstringsMatch
+        SYNTAX 1.3.6.1.4.1.1466.115.121.1.15
+        USAGE userApplications
+        X-ORIGIN 'OAuth 2.0' )
 olcObjectClasses: ( 1.3.6.1.4.1.56207.1.2.1 NAME 'oauthClient'
         DESC 'OAuth 2.0 Authorization Code'
         SUP top
         STRUCTURAL
         MUST  oauthClientID
         MAY ( description $
               oauthClientName $
@@ -348,15 +356,16 @@
               oauthPolicyURI $
               oauthJWKURI $
               oauthJWK $
               oauthTokenEndpointAuthMethod $
               oauthSoftwareID $
               oauthSoftwareVersion $
               oauthAudience $
-              oauthPreconsent )
+              oauthPreconsent $
+              oauthPostLogoutRedirectURI )
         )
         X-ORIGIN 'OAuth 2.0' )
 olcObjectClasses: ( 1.3.6.1.4.1.56207.1.2.2 NAME 'oauthAuthorizationCode'
         DESC 'OAuth 2.0 Authorization Code'
         SUP top
         STRUCTURAL
         MUST  oauthAuthorizationCodeID
```

### Comparing `Canaille-0.0.8/canaille/ldap_backend/schemas/oauth2-openldap.schema` & `Canaille-0.0.9/canaille/ldap_backend/schemas/oauth2-openldap.schema`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,23 @@
         EQUALITY caseExactMatch
         ORDERING caseExactOrderingMatch
         SUBSTR caseExactSubstringsMatch
         SYNTAX 1.3.6.1.4.1.1466.115.121.1.15
         SINGLE-VALUE
         USAGE userApplications
         X-ORIGIN 'OAuth 2.0' )
+attributetypes (  1.3.6.1.4.1.56207.1.1.39 NAME 'oauthPostLogoutRedirectURI'
+        DESC 'OAuth 2.0 Post logout redirection URI'
+        EQUALITY caseExactMatch
+        ORDERING caseExactOrderingMatch
+        SUBSTR caseExactSubstringsMatch
+        SYNTAX 1.3.6.1.4.1.1466.115.121.1.15
+        SINGLE-VALUE
+        USAGE userApplications
+        X-ORIGIN 'OAuth 2.0' )
 objectclass ( 1.3.6.1.4.1.56207.1.2.1 NAME 'oauthClient'
         DESC 'OAuth 2.0 Authorization Code'
         SUP top
         STRUCTURAL
         MUST  oauthClientID
         MAY ( description $
               oauthClientName $
@@ -345,15 +354,16 @@
               oauthPolicyURI $
               oauthJWKURI $
               oauthJWK $
               oauthTokenEndpointAuthMethod $
               oauthSoftwareID $
               oauthSoftwareVersion $
               oauthAudience $
-              oauthPreconsent )
+              oauthPreconsent $
+              oauthPostLogoutRedirectURI )
         )
         X-ORIGIN 'OAuth 2.0' )
 objectclass ( 1.3.6.1.4.1.56207.1.2.2 NAME 'oauthAuthorizationCode'
         DESC 'OAuth 2.0 Authorization Code'
         SUP top
         STRUCTURAL
         MUST  oauthAuthorizationCodeID
```

### Comparing `Canaille-0.0.8/canaille/mails.py` & `Canaille-0.0.9/canaille/mails.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/models.py` & `Canaille-0.0.9/canaille/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -118,25 +118,23 @@
 
     @property
     def groups(self):
         if self._groups is None:
             self.load_groups()
         return self._groups
 
-    def set_groups(self, values, conn=None):
+    def set_groups(self, values):
         before = self._groups
-        after = [
-            v if isinstance(v, Group) else Group.get(dn=v, conn=conn) for v in values
-        ]
+        after = [v if isinstance(v, Group) else Group.get(dn=v) for v in values]
         to_add = set(after) - set(before)
         to_del = set(before) - set(after)
         for group in to_add:
-            group.add_member(self, conn=conn)
+            group.add_member(self)
         for group in to_del:
-            group.remove_member(self, conn=conn)
+            group.remove_member(self)
         self._groups = after
 
     def load_permissions(self, conn=None):
         conn = conn or self.ldap()
 
         for access_group_name, details in current_app.config["ACL"].items():
             if not details.get("FILTER") or (
@@ -150,14 +148,18 @@
     def can_read(self, field):
         return field in self.read | self.write
 
     def can_writec(self, field):
         return field in self.write
 
     @property
+    def can_edit_self(self):
+        return "edit_self" in self.permissions
+
+    @property
     def can_use_oidc(self):
         return "use_oidc" in self.permissions
 
     @property
     def can_manage_users(self):
         return "manage_users" in self.permissions
 
@@ -194,14 +196,14 @@
     def get_members(self, conn=None):
         return [
             User.get(dn=user_dn, conn=conn)
             for user_dn in self.member
             if User.get(dn=user_dn, conn=conn)
         ]
 
-    def add_member(self, user, conn=None):
+    def add_member(self, user):
         self.member = self.member + [user.dn]
-        self.save(conn=conn)
+        self.save()
 
-    def remove_member(self, user, conn=None):
+    def remove_member(self, user):
         self.member = [m for m in self.member if m != user.dn]
-        self.save(conn=conn)
+        self.save()
```

### Comparing `Canaille-0.0.8/canaille/oidc/authorizations.py` & `Canaille-0.0.9/canaille/oidc/authorizations.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/oidc/clients.py` & `Canaille-0.0.9/canaille/oidc/clients.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,14 +48,19 @@
         render_kw={"placeholder": "https://mydomain.tld"},
     )
     redirect_uris = wtforms.URLField(
         _("Redirect URIs"),
         validators=[wtforms.validators.DataRequired()],
         render_kw={"placeholder": "https://mydomain.tld/callback"},
     )
+    post_logout_redirect_uris = wtforms.URLField(
+        _("Post logout redirect URIs"),
+        validators=[wtforms.validators.Optional()],
+        render_kw={"placeholder": "https://mydomain.tld/you-have-been-disconnected"},
+    )
     grant_type = wtforms.SelectMultipleField(
         _("Grant types"),
         validators=[wtforms.validators.DataRequired()],
         choices=[
             ("password", "password"),
             ("authorization_code", "authorization_code"),
             ("implicit", "implicit"),
@@ -159,14 +164,15 @@
         client_id=client_id,
         issue_date=client_id_issued_at,
         name=form["name"].data,
         contact=form["contact"].data,
         uri=form["uri"].data,
         grant_type=form["grant_type"].data,
         redirect_uris=[form["redirect_uris"].data],
+        post_logout_redirect_uris=[form["post_logout_redirect_uris"].data],
         response_type=form["response_type"].data,
         scope=form["scope"].data.split(" "),
         token_endpoint_auth_method=form["token_endpoint_auth_method"].data,
         logo_uri=form["logo_uri"].data,
         tos_uri=form["tos_uri"].data,
         policy_uri=form["policy_uri"].data,
         software_id=form["software_id"].data,
@@ -197,18 +203,27 @@
     if request.form.get("action") == "delete":
         return client_delete(client_id)
 
     abort(400)
 
 
 def client_edit(client_id):
-    client = Client.get(client_id) or abort(404)
+    client = Client.get(client_id)
+
+    if not client:
+        abort(404)
+
     data = dict(client)
     data["scope"] = " ".join(data["scope"])
     data["redirect_uris"] = data["redirect_uris"][0]
+    data["post_logout_redirect_uris"] = (
+        data["post_logout_redirect_uris"][0]
+        if data["post_logout_redirect_uris"]
+        else ""
+    )
     data["preconsent"] = client.preconsent
     form = ClientAdd(request.form or None, data=data, client=client)
 
     if not request.form:
         return render_template(
             "oidc/admin/client_edit.html", form=form, client=client, menuitem="admin"
         )
@@ -222,14 +237,15 @@
     else:
         client.update(
             name=form["name"].data,
             contact=form["contact"].data,
             uri=form["uri"].data,
             grant_type=form["grant_type"].data,
             redirect_uris=[form["redirect_uris"].data],
+            post_logout_redirect_uris=[form["post_logout_redirect_uris"].data],
             response_type=form["response_type"].data,
             scope=form["scope"].data.split(" "),
             token_endpoint_auth_method=form["token_endpoint_auth_method"].data,
             logo_uri=form["logo_uri"].data,
             tos_uri=form["tos_uri"].data,
             policy_uri=form["policy_uri"].data,
             software_id=form["software_id"].data,
@@ -247,14 +263,18 @@
 
     return render_template(
         "oidc/admin/client_edit.html", form=form, client=client, menuitem="admin"
     )
 
 
 def client_delete(client_id):
-    client = Client.get(client_id) or abort(404)
+    client = Client.get(client_id)
+
+    if not client:
+        abort(404)
+
     flash(
         _("The client has been deleted."),
         "success",
     )
     client.delete()
     return redirect(url_for("oidc.clients.index"))
```

### Comparing `Canaille-0.0.8/canaille/oidc/consents.py` & `Canaille-0.0.9/canaille/oidc/consents.py`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/oidc/models.py` & `Canaille-0.0.9/canaille/oidc/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     attribute_table = {
         "description": "description",
         "client_id": "oauthClientID",
         "name": "oauthClientName",
         "contact": "oauthClientContact",
         "uri": "oauthClientURI",
         "redirect_uris": "oauthRedirectURIs",
+        "post_logout_redirect_uris": "oauthPostLogoutRedirectURI",
         "logo_uri": "oauthLogoURI",
         "issue_date": "oauthIssueDate",
         "secret": "oauthClientSecret",
         "secret_expires_date": "oauthClientSecretExpDate",
         "grant_type": "oauthGrantType",
         "response_type": "oauthResponseType",
         "scope": "oauthScope",
@@ -33,17 +34,14 @@
         "token_endpoint_auth_method": "oauthTokenEndpointAuthMethod",
         "software_id": "oauthSoftwareID",
         "software_version": "oauthSoftwareVersion",
         "audience": "oauthAudience",
         "preconsent": "oauthPreconsent",
     }
 
-    def get_client_id(self):
-        return self.id
-
     def get_default_redirect_uri(self):
         return self.redirect_uris[0]
 
     def get_allowed_scope(self, scope):
         return util.list_to_scope(self.scope)
 
     def check_redirect_uri(self, redirect_uri):
@@ -51,16 +49,18 @@
 
     def has_client_secret(self):
         return bool(self.secret)
 
     def check_client_secret(self, client_secret):
         return client_secret == self.secret
 
-    def check_token_endpoint_auth_method(self, method):
-        return method == self.token_endpoint_auth_method
+    def check_endpoint_auth_method(self, method, endpoint):
+        if endpoint == "token":
+            return method == self.token_endpoint_auth_method
+        return True
 
     def check_response_type(self, response_type):
         return all(r in self.response_type for r in response_type.split(" "))
 
     def check_grant_type(self, grant_type):
         return grant_type in self.grant_type
 
@@ -137,17 +137,14 @@
     def expire_date(self):
         return self.issue_date + datetime.timedelta(seconds=int(self.lifetime))
 
     @property
     def revoked(self):
         return bool(self.revokation_date)
 
-    def get_client_id(self):
-        return Client.get(self.client).id
-
     def get_scope(self):
         return " ".join(self.scope)
 
     def get_expires_in(self):
         return int(self.lifetime)
 
     def get_issued_at(self):
@@ -167,14 +164,20 @@
 
     def is_expired(self):
         return (
             self.issue_date + datetime.timedelta(seconds=int(self.lifetime))
             < datetime.datetime.now()
         )
 
+    def is_revoked(self):
+        return bool(self.revokation_date)
+
+    def check_client(self, client):
+        return client.client_id == Client.get(self.client).client_id
+
 
 class Consent(LDAPObject):
     object_class = ["oauthConsent"]
     base = "ou=consents,ou=oauth"
     id = "cn"
     attribute_table = {
         "cn": "cn",
```

### Comparing `Canaille-0.0.8/canaille/oidc/oauth2utils.py` & `Canaille-0.0.9/canaille/oidc/oauth2utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 def get_jwt_config(grant):
 
     with open(current_app.config["JWT"]["PRIVATE_KEY"]) as pk:
         return {
             "key": pk.read(),
             "alg": current_app.config["JWT"].get("ALG", DEFAULT_JWT_ALG),
-            "iss": authorization.metadata["issuer"],
+            "iss": current_app.config["JWT"]["ISS"],
             "exp": current_app.config["JWT"].get("EXP", DEFAULT_JWT_EXP),
         }
 
 
 def generate_user_info(user, scope):
     user = User.get(dn=user)
     claims = ["sub"]
@@ -246,63 +246,64 @@
         return False
 
     def token_revoked(self, token):
         return bool(token.revokation_date)
 
 
 class RevocationEndpoint(_RevocationEndpoint):
-    def query_token(self, token, token_type_hint, client):
+    def query_token(self, token, token_type_hint):
+        print("query_token")
         if token_type_hint == "access_token":
-            return Token.filter(client=client.dn, access_token=token)
+            return Token.filter(access_token=token)
         elif token_type_hint == "refresh_token":
-            return Token.filter(client=client.dn, refresh_token=token)
+            return Token.filter(refresh_token=token)
 
-        item = Token.filter(client=client.dn, access_token=token)
+        item = Token.filter(access_token=token)
         if item:
             return item[0]
 
-        item = Token.filter(client=client.dn, refresh_token=token)
+        item = Token.filter(refresh_token=token)
         if item:
             return item[0]
 
         return None
 
-    def revoke_token(self, token):
+    def revoke_token(self, token, request):
         token.revokation_date = datetime.datetime.now()
         token.save()
 
 
 class IntrospectionEndpoint(_IntrospectionEndpoint):
-    def query_token(self, token, token_type_hint, client):
+    def query_token(self, token, token_type_hint):
         if token_type_hint == "access_token":
             tok = Token.filter(access_token=token)
         elif token_type_hint == "refresh_token":
             tok = Token.filter(refresh_token=token)
         else:
             tok = Token.filter(access_token=token)
             if not tok:
                 tok = Token.filter(refresh_token=token)
-        if tok:
-            tok = tok[0]
-            if client.dn in tok.audience:
-                return tok
+        return tok[0] if tok else None
+
+    def check_permission(self, token, client, request):
+        return client.dn in token.audience
 
     def introspect_token(self, token):
         client_id = Client.get(token.client).client_id
         user = User.get(dn=token.subject)
         audience = [Client.get(aud).client_id for aud in token.audience]
         return {
             "active": True,
             "client_id": client_id,
             "token_type": token.type,
             "username": user.name,
             "scope": token.get_scope(),
             "sub": user.uid[0],
             "aud": audience,
-            "iss": authorization.metadata["issuer"],
+            "iss": current_app.config["JWT"]["ISS"],
             "exp": token.get_expires_at(),
             "iat": token.get_issued_at(),
         }
 
 
 class CodeChallenge(_CodeChallenge):
     def get_authorization_code_challenge(self, authorization_code):
```

### Comparing `Canaille-0.0.8/canaille/oidc/tokens.py` & `Canaille-0.0.9/canaille/oidc/tokens.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     )
     return render_template("oidc/admin/token_list.html", items=items, menuitem="admin")
 
 
 @bp.route("/<token_id>", methods=["GET", "POST"])
 @permissions_needed("manage_oidc")
 def view(user, token_id):
-    token = Token.get(token_id=token_id) or abort(404)
+    token = Token.get(token_id=token_id)
+
+    if not token:
+        abort(404)
+
     token_client = Client.get(token.client)
     token_user = User.get(dn=token.subject)
     token_audience = [Client.get(aud) for aud in token.audience]
     return render_template(
         "oidc/admin/token_view.html",
         token=token,
         token_client=token_client,
```

### Comparing `Canaille-0.0.8/canaille/static/css/base.css` & `Canaille-0.0.9/canaille/static/css/base.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/datatables/French.json` & `Canaille-0.0.9/canaille/static/datatables/French.json`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/datatables/dataTables.semanticui.min.css` & `Canaille-0.0.9/canaille/static/datatables/dataTables.semanticui.min.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/datatables/dataTables.semanticui.min.js` & `Canaille-0.0.9/canaille/static/datatables/dataTables.semanticui.min.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/datatables/jquery.dataTables.min.css` & `Canaille-0.0.9/canaille/static/datatables/jquery.dataTables.min.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/datatables/jquery.dataTables.min.js` & `Canaille-0.0.9/canaille/static/datatables/jquery.dataTables.min.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/semantic.css` & `Canaille-0.0.9/canaille/static/fomanticui/semantic.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/semantic.js` & `Canaille-0.0.9/canaille/static/fomanticui/semantic.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/semantic.min.css` & `Canaille-0.0.9/canaille/static/fomanticui/semantic.min.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/semantic.min.js` & `Canaille-0.0.9/canaille/static/fomanticui/semantic.min.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.eot` & `Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/basic/assets/fonts/icons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/basic/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.eot` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff2` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.eot` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.otf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.otf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff2` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.eot` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff2` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/fonts/outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/default/assets/images/flags.png` & `Canaille-0.0.9/canaille/static/fomanticui/themes/default/assets/images/flags.png`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons-local.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons-local.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/github/assets/fonts/octicons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/github/assets/fonts/octicons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.eot` & `Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.svg` & `Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.ttf` & `Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff` & `Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff2` & `Canaille-0.0.9/canaille/static/fomanticui/themes/material/assets/fonts/icons.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.eot` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.svg` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.ttf` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.woff` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700.woff2` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.eot` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.svg` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.ttf` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.woff` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-700italic.woff2` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-700italic.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.eot` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.svg` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.ttf` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.woff` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-italic.woff2` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-italic.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.eot` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.eot`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.svg` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.ttf` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.ttf`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.woff` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato-v17-latin-regular.woff2` & `Canaille-0.0.9/canaille/static/fonts/lato-v17-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/fonts/lato.css` & `Canaille-0.0.9/canaille/static/fonts/lato.css`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/html5shiv/html5shiv.min.js` & `Canaille-0.0.9/canaille/static/html5shiv/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-c.png` & `Canaille-0.0.9/canaille/static/img/canaille-c.png`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-c.svg` & `Canaille-0.0.9/canaille/static/img/canaille-c.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-full.png` & `Canaille-0.0.9/canaille/static/img/canaille-full.png`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-full.svg` & `Canaille-0.0.9/canaille/static/img/canaille-full.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-head.png` & `Canaille-0.0.9/canaille/static/img/canaille-head.png`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-head.svg` & `Canaille-0.0.9/canaille/static/img/canaille-head.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-label.png` & `Canaille-0.0.9/canaille/static/img/canaille-label.png`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/img/canaille-label.svg` & `Canaille-0.0.9/canaille/static/img/canaille-label.svg`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/jquery/jquery.min.js` & `Canaille-0.0.9/canaille/static/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/static/js/profile.js` & `Canaille-0.0.9/canaille/static/js/profile.js`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/about.html` & `Canaille-0.0.9/canaille/templates/about.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/error.html` & `Canaille-0.0.9/canaille/templates/error.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/firstlogin.html` & `Canaille-0.0.9/canaille/templates/firstlogin.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/fomanticui.html` & `Canaille-0.0.9/canaille/templates/fomanticui.html`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 {% if field_visible %}
     <div class="ui
         {% if suffix_text %}right{% endif %}
         {% if corner_indicator %}corner{% endif %}
         {% if labeled %}labeled{% endif %}
         {% if icon %}left icon {% endif %}
         {% if field.type not in ("BooleanField", "RadioField") %}input{% endif %}
-        ">
+    ">
 {% endif %}
 {% if icon %}<i class="{{ icon }} icon"></i>{% endif %}
 
 {% if field.type not in ("SelectField", "SelectMultipleField") %}
     {{ field(**kwargs) }}
 {% elif field.render_kw and "readonly" in field.render_kw %}
     {{ field(class_="ui fluid dropdown multiple read-only", **kwargs) }}
```

### Comparing `Canaille-0.0.8/canaille/templates/forgotten-password.html` & `Canaille-0.0.9/canaille/templates/forgotten-password.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/group.html` & `Canaille-0.0.9/canaille/templates/group.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/groups.html` & `Canaille-0.0.9/canaille/templates/groups.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/invite.html` & `Canaille-0.0.9/canaille/templates/invite.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/login.html` & `Canaille-0.0.9/canaille/templates/login.html`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
             {% if "password" in form %}
                 {% block password_field scoped %}{{ sui.render_field(form.password, icon="key", noindicator=true) }}{% endblock %}
             {% endif %}
 
             <div class="ui right aligned container">
                 <div class="ui stackable buttons">
-                    {% if has_smtp %}
+                    {% if has_smtp and has_password_recovery %}
                         <a type="button" class="ui right floated button" href="{{ url_for('account.forgotten') }}">{{ _("Forgotten password") }}</a>
                     {% endif %}
                     <button type="submit" class="ui right floated primary button">{{ _("Continue") }}</button>
                 </div>
             </div>
         </form>
     </div>
```

#### html2text {}

```diff
@@ -4,9 +4,10 @@
 {{{{ __((""SSiiggnn iinn aatt %%((wweebbssiittee))ss"",, wweebbssiittee==wweebbssiittee__nnaammee)) }}}}
 {{%% ttrraannss %%}}LLoogg--iinn aanndd mmaannaaggee yyoouurr aauutthhoorriizzaattiioonnss..{{%% eennddttrraannss %%}}
 {{ form.hidden_tag() if form.hidden_tag }} {% block login_field scoped %}{
 { sui.render_field(form.login, icon="user", noindicator=true) }}{% endblock %}
 {% if "password" in form %} {% block password_field scoped %}{
 { sui.render_field(form.password, icon="key", noindicator=true) }}{% endblock
 %} {% endif %}
-{% if has_smtp %} _{_{_ ___(_"_F_o_r_g_o_t_t_e_n_ _p_a_s_s_w_o_r_d_"_)_ _}_} {% endif %} {{ _("Continue") }}
+{% if has_smtp and has_password_recovery %} _{_{_ ___(_"_F_o_r_g_o_t_t_e_n_ _p_a_s_s_w_o_r_d_"_)_ _}_} {%
+endif %} {{ _("Continue") }}
 {% endblock %}
```

### Comparing `Canaille-0.0.8/canaille/templates/mail/admin.html` & `Canaille-0.0.9/canaille/templates/mail/admin.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/mail/firstlogin.html` & `Canaille-0.0.9/canaille/templates/mail/firstlogin.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/mail/invitation.html` & `Canaille-0.0.9/canaille/templates/mail/invitation.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/mail/reset.html` & `Canaille-0.0.9/canaille/templates/mail/reset.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/authorization_list.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/authorization_list.html`

 * *Files 0% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         </thead>
         {% for authorization in authorizations %}
             <tr>
                 <td><a href="{{ url_for('oidc.authorizations.view', authorization_id=authorization.authorization_code_id) }}">{{ authorization.authorization_code_id }}</a></td>
                 <td><a href="{{ url_for('oidc.clients.edit', client_id=authorization.client_id) }}">{{ authorization.client_id }}</a></td>
                 <td>{{ authorization.subject }}</td>
                 <td data-order="{{ authorization.issue_date|timestamp }}>{{ authorization.issue_date }}</td>
-            </tr>
+                </tr>
         {% endfor %}
     </table>
 
 {% endblock %}
```

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/authorization_view.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/authorization_view.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/client_edit.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/client_edit.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/client_list.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/client_list.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/token_list.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/token_list.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/admin/token_view.html` & `Canaille-0.0.9/canaille/templates/oidc/admin/token_view.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/oidc/user/authorize.html` & `Canaille-0.0.9/canaille/templates/oidc/user/authorize.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 {% block content %}
     <div class="ui segment">
         {% if client.logo_uri %}
             <img class="ui centered tiny image" src="{{ client.logo_uri }}" alt="{{ client.name }}">
         {% endif %}
 
-        <h2 class="ui header">{{ gettext('The application %(name)s is requesting access to:', name=client.name) }}</h3>
+        <h2 class="ui header">{{ gettext('The application %(name)s is requesting access to:', name=client.name) }}</h2>
 
         <div class="ui divided items">
             {% for claim in grant.request.scope.split(" ") %}
                 {% if claim not in ignored_claims %}
                     <div class="item">
                         {% if claim in claims %}
                             <div>
```

### Comparing `Canaille-0.0.8/canaille/templates/oidc/user/consent_list.html` & `Canaille-0.0.9/canaille/templates/oidc/user/consent_list.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/password.html` & `Canaille-0.0.9/canaille/templates/password.html`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
             {{ form.hidden_tag() if form.hidden_tag }}
             {{ sui.render_field(form.password, icon="key", noindicator=true) }}
 
             <div class="ui right aligned container">
                 <div class="ui stackable buttons">
                     <a type="button" class="ui right floated button" href="{{ url_for('account.login') }}">{{ _("I am not %(username)s", username=username) }}</a>
-                    {% if has_smtp %}
+                    {% if has_smtp and has_password_recovery %}
                         <a type="button" class="ui right floated button" href="{{ url_for('account.forgotten') }}">{{ _("Forgotten password") }}</a>
                     {% endif %}
                     <button type="submit" class="ui right floated primary button">{{ _("Sign in") }}</button>
                 </div>
             </div>
         </form>
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 {% extends theme('base.html') %} {% import 'fomanticui.html' as sui %} {% block
 content %}
 {% if logo_url %} _[_{_{_ _w_e_b_s_i_t_e___n_a_m_e_ _}_}_]{% else %} {% endif %}
 {{{{ __((""SSiiggnn iinn aass %%((uusseerrnnaammee))ss"",, uusseerrnnaammee==uusseerrnnaammee)) }}}}
 {{%% ttrraannss %%}}PPlleeaassee eenntteerr yyoouurr ppaasssswwoorrdd ffoorr tthhiiss aaccccoouunntt..{{%% eennddttrraannss %%}}
 {{ form.hidden_tag() if form.hidden_tag }} {{ sui.render_field(form.password,
 icon="key", noindicator=true) }}
-_{_{_ ___(_"_I_ _a_m_ _n_o_t_ _%_(_u_s_e_r_n_a_m_e_)_s_"_,_ _u_s_e_r_n_a_m_e_=_u_s_e_r_n_a_m_e_)_ _}_} {% if has_smtp %} _{_{_ __
-_(_"_F_o_r_g_o_t_t_e_n_ _p_a_s_s_w_o_r_d_"_)_ _}_} {% endif %} {{ _("Sign in") }}
+_{_{_ ___(_"_I_ _a_m_ _n_o_t_ _%_(_u_s_e_r_n_a_m_e_)_s_"_,_ _u_s_e_r_n_a_m_e_=_u_s_e_r_n_a_m_e_)_ _}_} {% if has_smtp and
+has_password_recovery %} _{_{_ ___(_"_F_o_r_g_o_t_t_e_n_ _p_a_s_s_w_o_r_d_"_)_ _}_} {% endif %} {{ _("Sign
+in") }}
 {% endblock %}
```

### Comparing `Canaille-0.0.8/canaille/templates/profile.html` & `Canaille-0.0.9/canaille/templates/profile.html`

 * *Files 1% similar despite different names*

```diff
@@ -177,41 +177,41 @@
                             <p>{% trans %}The user will not be able to authenticate unless the password is set{% endtrans %}</p>
                         {% endif %}
                     </div>
 
                 {% elif not edited_user.has_password() %}
 
                     <div class="ui message warning">
-                        {% if has_smtp %}
+                        {% if has_smtp and edited_user.can_edit_self %}
                             {% if request.method == "POST" and request.form.action == "password-initialization-mail" %}
                                 <button type="submit" name="action" value="password-initialization-mail" class="ui right floated button">
                                     {% trans %}Send again{% endtrans %}
                                 </button>
                             {% else %}
                                 <button type="submit" name="action" value="password-initialization-mail" class="ui right floated primary button">
                                     {% trans %}Send email{% endtrans %}
                                 </button>
                             {% endif %}
                         {% endif %}
                         <div class="header">
                             {% trans %}This user does not have a password yet{% endtrans %}
                         </div>
-                        {% if has_smtp %}
+                        {% if has_smtp and edited_user.can_edit_self %}
                             <p>{% trans %}You can solve this by:{% endtrans %}</p>
                             <ul class="ui list">
                                 <li>{% trans %}setting a password using this form;{% endtrans %}</li>
                                 <li>{% trans %}sending the user a password initialization mail, by clicking this button;{% endtrans %}</li>
                                 <li>{% trans %}or simply waiting for the user to sign-in a first time, and then receive a password initialization mail.{% endtrans %}</li>
                             </ul>
                         {% else %}
                             <p>{% trans %}The user will not be able to authenticate unless the password is set{% endtrans %}</p>
                         {% endif %}
                     </div>
 
-                {% elif has_smtp and edited_user.uid != user.uid and edited_user.has_password() %}
+                {% elif has_smtp and edited_user.uid != user.uid and edited_user.has_password() and edited_user.can_edit_self %}
 
                     <div class="ui message info">
                         <button type="submit" name="action" value="password-reset-mail" class="ui right floated button">
                             {% if request.method == "POST" and request.form.action == "password-reset-mail" %}
                                 {% trans %}Send again{% endtrans %}
                             {% else %}
                                 {% trans %}Send mail{% endtrans %}
```

#### html2text {}

```diff
@@ -70,31 +70,32 @@
     * {% trans %}or simply waiting for the user to sign-in a first time, and
       then receive a password initialization mail.{% endtrans %}
 {% else %}
 {% trans %}The user will not be able to authenticate unless the password is set
 {% endtrans %}
 {% endif %}
 {% elif not edited_user.has_password() %}
-{% if has_smtp %} {% if request.method == "POST" and request.form.action ==
-"password-initialization-mail" %} {% trans %}Send again{% endtrans %} {% else
-%} {% trans %}Send email{% endtrans %} {% endif %} {% endif %}
+{% if has_smtp and edited_user.can_edit_self %} {% if request.method == "POST"
+and request.form.action == "password-initialization-mail" %} {% trans %}Send
+again{% endtrans %} {% else %} {% trans %}Send email{% endtrans %} {% endif %}
+{% endif %}
 {% trans %}This user does not have a password yet{% endtrans %}
-{% if has_smtp %}
+{% if has_smtp and edited_user.can_edit_self %}
 {% trans %}You can solve this by:{% endtrans %}
     * {% trans %}setting a password using this form;{% endtrans %}
     * {% trans %}sending the user a password initialization mail, by clicking
       this button;{% endtrans %}
     * {% trans %}or simply waiting for the user to sign-in a first time, and
       then receive a password initialization mail.{% endtrans %}
 {% else %}
 {% trans %}The user will not be able to authenticate unless the password is set
 {% endtrans %}
 {% endif %}
 {% elif has_smtp and edited_user.uid != user.uid and edited_user.has_password()
-%}
+and edited_user.can_edit_self %}
 {% if request.method == "POST" and request.form.action == "password-reset-mail"
 %} {% trans %}Send again{% endtrans %} {% else %} {% trans %}Send mail{%
 endtrans %} {% endif %}
 {% trans %}Password reset{% endtrans %}
 {% trans %}If the user has forgotten his password, you can send him a password
 reset email by clicking this button.{% endtrans %}
 {% endif %} {% endif %}
```

### Comparing `Canaille-0.0.8/canaille/templates/reset-password.html` & `Canaille-0.0.9/canaille/templates/reset-password.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/userlist.html` & `Canaille-0.0.9/canaille/templates/userlist.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/templates/users.html` & `Canaille-0.0.9/canaille/templates/users.html`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/themes/default/base.html` & `Canaille-0.0.9/canaille/themes/default/base.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,21 @@
                     {% if logo_url %}
                         <div class="header item">
                             <a href="/" class="logo">
                                 <img class="ui image" src="{{ logo_url }}" alt="{{ website_name }}" />
                             </a>
                         </div>
                     {% endif %}
-                    <a class="item {% if menuitem == "profile" %}active{% endif %}"
-                        href="{{ url_for('account.profile_edition', username=user.uid[0]) }}">
-                        <i class="id card icon"></i>
-                        {% trans %}My profile{% endtrans %}
-                    </a>
+                    {% if user.can_edit_self %}
+                        <a class="item {% if menuitem == "profile" %}active{% endif %}"
+                            href="{{ url_for('account.profile_edition', username=user.uid[0]) }}">
+                            <i class="id card icon"></i>
+                            {% trans %}My profile{% endtrans %}
+                        </a>
+                    {% endif %}
                     {% if user.can_use_oidc %}
                         <a class="item {% if menuitem == "consents" %}active{% endif %}"
                             href="{{ url_for('oidc.consents.consents') }}">
                             <i class="handshake icon"></i>
                             {% trans %}My consents{% endtrans %}
                         </a>
                     {% endif %}
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% import 'flask.j2' as flask %}
 {% if logo_url %}
 {% endif %} {% block style %}{% endblock %}
 {% block menu %} {% if user and menu %} {% if logo_url %}
 _[_{_{_ _w_e_b_s_i_t_e___n_a_m_e_ _}_}_]
-{% endif %}
+{% endif %} {% if user.can_edit_self %}
 }active{% endif %}" href="{{ url_for('account.profile_edition',
 username=user.uid[0]) }}"> {% trans %}My profile{% endtrans %}
-{% if user.can_use_oidc %}
+{% endif %} {% if user.can_use_oidc %}
 }active{% endif %}" href="{{ url_for('oidc.consents.consents') }}"> {% trans
 %}My consents{% endtrans %}
 {% endif %} {% if user.can_manage_users %}
 }active{% endif %}" href="{{ url_for('account.users') }}"> {% trans %}Users{%
 endtrans %}
 {% endif %} {% if user.can_manage_groups %}
 }active{% endif %}" href="{{ url_for('groups.groups') }}"> {% trans %}Groups{%
```

### Comparing `Canaille-0.0.8/canaille/translations/README.md` & `Canaille-0.0.9/canaille/translations/README.md`

 * *Files identical despite different names*

### Comparing `Canaille-0.0.8/canaille/translations/fr/LC_MESSAGES/messages.po` & `Canaille-0.0.9/canaille/translations/fr/LC_MESSAGES/messages.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,151 +1,168 @@
 # French translations for PROJECT.
 # Copyright (C) 2020 ORGANIZATION
 # This file is distributed under the same license as the PROJECT project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2020.
 # Camille <camille@yaal.coop>, 2021-2022.
-# Éloi Rivard <eloi@yaal.fr>, 2020-2022.
+# Éloi Rivard <eloi.rivard@aquilenet.fr>, 2020-2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: contact@yaal.fr\n"
-"POT-Creation-Date: 2022-02-23 10:58+0100\n"
-"PO-Revision-Date: 2022-02-23 10:59+0100\n"
-"Last-Translator: Éloi Rivard <eloi@yaal.fr>\n"
-"Language: fr_FR\n"
-"Language-Team: French - France <equipe@yaal.fr>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1)\n"
+"POT-Creation-Date: 2022-06-02 15:50+0200\n"
+"PO-Revision-Date: 2022-06-02 15:55+0200\n"
+"Last-Translator: Éloi Rivard <eloi.rivard@aquilenet.fr>\n"
+"Language: fr\n"
+"Language-Team: French <traduc@traduc.org>\n"
+"Plural-Forms: nplurals=2; plural=(n > 1)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.1\n"
 "X-Generator: Gtranslator 40.0\n"
 
-#: canaille/account.py:82 canaille/account.py:107 canaille/oidc/oauth.py:77
+#: canaille/account.py:93 canaille/account.py:118 canaille/oidc/oauth.py:88
 msgid "Login failed, please check your information"
 msgstr "La connexion a échoué, veuillez vérifier vos informations."
 
-#: canaille/account.py:113
+#: canaille/account.py:124
 #, python-format
 msgid "Connection successful. Welcome %(user)s"
 msgstr "Connexion réussie. Bienvenue %(user)s"
 
-#: canaille/account.py:126
+#: canaille/account.py:137
 #, python-format
 msgid "You have been disconnected. See you next time %(user)s"
 msgstr "Vous avez été déconnecté·e. À bientôt %(user)s"
 
-#: canaille/account.py:143
+#: canaille/account.py:155
 msgid "Could not send the password initialization link."
 msgstr "Impossible d'envoyer le courriel d'initialisation de mot de passe."
 
-#: canaille/account.py:148
+#: canaille/account.py:160
 msgid ""
 "A password initialization link has been sent at your email address. You "
 "should receive it within 10 minutes."
 msgstr ""
 "Un lien d'initialisation de votre mot de passe vous a été envoyé par mail. "
 "Vous devriez le recevoir d'ici une dizaine de minutes."
 
-#: canaille/account.py:154 canaille/account.py:398
+#: canaille/account.py:166 canaille/account.py:418
 msgid "Could not send the password initialization email"
 msgstr "Impossible d'envoyer le courriel d'initialisation de mot de passe."
 
-#: canaille/account.py:247 canaille/account.py:324
+#: canaille/account.py:255 canaille/account.py:338
 msgid "User account creation failed."
 msgstr "La création du compte utilisateur a échoué."
 
-#: canaille/account.py:268 canaille/account.py:296
+#: canaille/account.py:276 canaille/account.py:304
 msgid "The invitation link that brought you here was invalid."
 msgstr "Le lien d'invitation qui vous a amené ici est invalide."
 
-#: canaille/account.py:275
+#: canaille/account.py:283
 msgid "The invitation link that brought you here has expired."
 msgstr "Le lien d'invitation qui vous a amené ici a expiré."
 
-#: canaille/account.py:282
+#: canaille/account.py:290
 msgid "Your account has already been created."
 msgstr "Votre compte a déjà été créé."
 
-#: canaille/account.py:289
+#: canaille/account.py:297
 msgid "You are already logged in, you cannot create an account."
 msgstr "Vous êtes déjà connectés, vous ne pouvez pas créer de compte."
 
-#: canaille/account.py:329
+#: canaille/account.py:316 canaille/forms.py:179 canaille/forms.py:227
+#: canaille/templates/groups.html:11 canaille/templates/userlist.html:17
+#: canaille/themes/default/base.html:61
+msgid "Groups"
+msgstr "Groupes"
+
+#: canaille/account.py:343
 msgid "You account has been created successfuly."
 msgstr "Votre compte utilisateur a été créé avec succès."
 
-#: canaille/account.py:371
+#: canaille/account.py:385
 msgid "User account creation succeed."
 msgstr "La création du compte utilisateur a réussi."
 
-#: canaille/account.py:392
+#: canaille/account.py:412
 msgid ""
 "A password initialization link has been sent at the user email address. It "
 "should be received within 10 minutes."
 msgstr ""
 "Un lien d'initialisation de mot de passe a été envoyé à l'utilisateur par "
 "mail. Il devrait arriver d'ici une dizaine de minutes."
 
-#: canaille/account.py:406
+#: canaille/account.py:429
 msgid ""
 "A password reset link has been sent at the user email address. It should be "
 "received within 10 minutes."
 msgstr ""
 "Un lien de réinitialisation de mot de passe a été envoyé à l'utilisateur par "
 "mail. Il devrait arriver d'ici une dizaine de minutes."
 
-#: canaille/account.py:412
+#: canaille/account.py:435
 msgid "Could not send the password reset email"
 msgstr "Impossible d'envoyer le lien de réinitialisation."
 
-#: canaille/account.py:443
+#: canaille/account.py:469
 msgid "Profile edition failed."
 msgstr "L'édition du profil a échoué."
 
-#: canaille/account.py:471
+#: canaille/account.py:497
 msgid "Profile updated successfuly."
 msgstr "Le profil a été mis à jour avec succès."
 
-#: canaille/account.py:491
+#: canaille/account.py:520
 #, python-format
 msgid "The user %(user)s has been sucessfuly deleted"
 msgstr "L'utilisateur %(user)s a bien été supprimé"
 
-#: canaille/account.py:515
+#: canaille/account.py:550
 msgid "Could not send the password reset link."
 msgstr "Impossible d'envoyer le lien de réinitialisation."
 
-#: canaille/account.py:522 canaille/account.py:533
+#: canaille/account.py:554
 msgid ""
 "A password reset link has been sent at your email address. You should "
 "receive it within 10 minutes."
 msgstr ""
 "Un lien de ré-initialisation de votre mot de passe vous a été envoyé par "
 "mail. Vous devriez le recevoir d'ici une dizaine de minutes."
 
-#: canaille/account.py:539
-msgid "Could not reset your password"
-msgstr "Impossible de réinitialiser votre mot de passe"
+#: canaille/account.py:565
+#, python-format
+msgid ""
+"The user '%(user)s' does not have permissions to update their password. We "
+"cannot send a password reset email."
+msgstr ""
+"L'utilisateur '%(user)s' n'a pas la permission d'éditer son mot de passe. "
+"Nous ne pouvons pas lui envoyer un email de réinitialisation."
+
+#: canaille/account.py:580
+msgid "We encountered an issue while we sent the password recovery email."
+msgstr ""
+"Nous avons rencontré un problème lors de l'envoi de l'email de "
+"réinitialisation de mot de passe."
 
-#: canaille/account.py:553
+#: canaille/account.py:599
 msgid "The password reset link that brought you here was invalid."
 msgstr "Le lien de réinitialisation qui vous a amené ici est invalide."
 
-#: canaille/account.py:562
+#: canaille/account.py:608
 msgid "Your password has been updated successfuly"
 msgstr "Votre mot de passe a correctement été mis à jour."
 
 #: canaille/admin.py:23 canaille/templates/userlist.html:14
 msgid "Email"
 msgstr "Courriel"
 
 #: canaille/admin.py:29 canaille/forms.py:47 canaille/forms.py:71
-#: canaille/forms.py:123 canaille/forms.py:224
+#: canaille/forms.py:123 canaille/forms.py:221
 msgid "jane@doe.com"
 msgstr "camille@dupont.fr"
 
 #: canaille/admin.py:42 canaille/admin.py:44
 msgid "The test invitation mail has been sent correctly"
 msgstr "L'invitation de test a été envoyée correctement"
 
@@ -161,15 +178,15 @@
 msgid "Invitation on {website_name}"
 msgstr "Invitation sur {website_name}"
 
 #: canaille/apputils.py:41
 msgid "John Doe"
 msgstr "Camille Dupont"
 
-#: canaille/apputils.py:44 canaille/forms.py:95 canaille/forms.py:212
+#: canaille/apputils.py:44 canaille/forms.py:95 canaille/forms.py:209
 msgid "jdoe"
 msgstr "cdupont"
 
 #: canaille/apputils.py:47
 msgid "john@doe.com"
 msgstr "camille@dupont.fr"
 
@@ -209,19 +226,19 @@
 msgid "Password confirmation"
 msgstr "Confirmation du mot de passe"
 
 #: canaille/forms.py:86 canaille/forms.py:145
 msgid "Password and confirmation do not match."
 msgstr "Le mot de passe et sa confirmation ne correspondent pas."
 
-#: canaille/forms.py:94 canaille/forms.py:211
+#: canaille/forms.py:94 canaille/forms.py:208
 msgid "Username"
 msgstr "Identifiant"
 
-#: canaille/forms.py:98 canaille/forms.py:197 canaille/oidc/clients.py:36
+#: canaille/forms.py:98 canaille/forms.py:194 canaille/oidc/clients.py:36
 #: canaille/templates/groups.html:17
 #: canaille/templates/oidc/admin/client_list.html:23
 #: canaille/templates/userlist.html:11
 msgid "Name"
 msgstr "Nom"
 
 #: canaille/forms.py:100
@@ -236,15 +253,15 @@
 msgid "Family Name"
 msgstr "Nom de famille"
 
 #: canaille/forms.py:111
 msgid "Doe"
 msgstr "Dupont"
 
-#: canaille/forms.py:117 canaille/forms.py:217
+#: canaille/forms.py:117 canaille/forms.py:214
 msgid "Email address"
 msgstr "Courriel"
 
 #: canaille/forms.py:119
 msgid ""
 "This email will be used as a recovery address to reset the password if needed"
 msgstr ""
@@ -279,63 +296,57 @@
 msgid "Website"
 msgstr "Site internet"
 
 #: canaille/forms.py:158
 msgid "https://mywebsite.tld"
 msgstr "https://mon-site-internet.fr"
 
-#: canaille/forms.py:182 canaille/forms.py:230
-#: canaille/templates/groups.html:11 canaille/templates/userlist.html:17
-#: canaille/themes/default/base.html:59
-msgid "Groups"
-msgstr "Groupes"
-
-#: canaille/forms.py:184
+#: canaille/forms.py:181
 msgid "users, admins ..."
 msgstr "utilisateurs, administrateurs ..."
 
-#: canaille/forms.py:200
+#: canaille/forms.py:197
 msgid "group"
 msgstr "groupe"
 
-#: canaille/forms.py:204 canaille/templates/groups.html:18
+#: canaille/forms.py:201 canaille/templates/groups.html:18
 msgid "Description"
 msgstr "Description"
 
-#: canaille/forms.py:215
+#: canaille/forms.py:212
 msgid "Username editable by the invitee"
 msgstr "L'identifiant sera éditable par la personne invitée"
 
-#: canaille/groups.py:44
+#: canaille/groups.py:40
 msgid "Group creation failed."
 msgstr "La création du groupe a échoué."
 
-#: canaille/groups.py:56
+#: canaille/groups.py:52
 #, python-format
 msgid "The group %(group)s has been sucessfully created"
 msgstr "Le groupe %(group)s a bien été créé"
 
-#: canaille/groups.py:93
+#: canaille/groups.py:92
 msgid "Group edition failed."
 msgstr "L'édition du groupe a échoué."
 
-#: canaille/groups.py:102
+#: canaille/groups.py:101
 #, python-format
 msgid "The group %(group)s has been sucessfully deleted"
 msgstr "Le groupe %(group)s a bien été supprimé"
 
 #: canaille/mails.py:95
 msgid "You have been invited to create an account on {website_name}"
 msgstr "Vous êtes invités à vous créer un compte sur {website_name}"
 
-#: canaille/ldap_backend/backend.py:48
+#: canaille/ldap_backend/backend.py:50
 msgid "Could not connect to the LDAP server '{uri}'"
 msgstr "Impossible de se connecter au serveur LDAP '{uri}'"
 
-#: canaille/ldap_backend/backend.py:64
+#: canaille/ldap_backend/backend.py:66
 msgid "LDAP authentication failed with user '{user}'"
 msgstr ""
 "L'authentification au serveur LDAP a échoué pour l'utilisateur '{user}'"
 
 #: canaille/oidc/clients.py:41
 msgid "Contact"
 msgstr "Contact"
@@ -345,118 +356,135 @@
 msgstr "URI"
 
 #: canaille/oidc/clients.py:51
 msgid "Redirect URIs"
 msgstr "URIs de redirection"
 
 #: canaille/oidc/clients.py:56
+msgid "Post logout redirect URIs"
+msgstr "URIs de redirection post-déconnexion"
+
+#: canaille/oidc/clients.py:61
 msgid "Grant types"
 msgstr "Grant types"
 
-#: canaille/oidc/clients.py:68 canaille/templates/oidc/admin/token_view.html:33
+#: canaille/oidc/clients.py:73 canaille/templates/oidc/admin/token_view.html:33
 msgid "Scope"
 msgstr "Scope"
 
-#: canaille/oidc/clients.py:74
+#: canaille/oidc/clients.py:79
 msgid "Response types"
 msgstr "Types de réponse"
 
-#: canaille/oidc/clients.py:80
+#: canaille/oidc/clients.py:85
 msgid "Token Endpoint Auth Method"
 msgstr "Token Endpoint Auth Method"
 
-#: canaille/oidc/clients.py:90
+#: canaille/oidc/clients.py:95
 msgid "Token audiences"
 msgstr "Token audiences"
 
-#: canaille/oidc/clients.py:96
+#: canaille/oidc/clients.py:101
 msgid "Logo URI"
 msgstr "URI du logo"
 
-#: canaille/oidc/clients.py:101
+#: canaille/oidc/clients.py:106
 msgid "Terms of service URI"
 msgstr "URI des conditions d'utilisation"
 
-#: canaille/oidc/clients.py:106
+#: canaille/oidc/clients.py:111
 msgid "Policy URI"
 msgstr "URI de la politique de confidentialité"
 
-#: canaille/oidc/clients.py:111
+#: canaille/oidc/clients.py:116
 msgid "Software ID"
 msgstr "ID du logiciel"
 
-#: canaille/oidc/clients.py:116
+#: canaille/oidc/clients.py:121
 msgid "Software Version"
 msgstr "Version du logiciel"
 
-#: canaille/oidc/clients.py:121
+#: canaille/oidc/clients.py:126
 msgid "JWK"
 msgstr "JWK"
 
-#: canaille/oidc/clients.py:126
+#: canaille/oidc/clients.py:131
 msgid "JKW URI"
 msgstr "URI du JWK"
 
-#: canaille/oidc/clients.py:131
+#: canaille/oidc/clients.py:136
 msgid "Pre-consent"
 msgstr "Pré-autorisé"
 
-#: canaille/oidc/clients.py:149
+#: canaille/oidc/clients.py:154
 msgid "The client has not been added. Please check your information."
 msgstr "Le client n'a pas été ajouté. Veuillez vérifier vos informations."
 
-#: canaille/oidc/clients.py:184
+#: canaille/oidc/clients.py:190
 msgid "The client has been created."
 msgstr "Le client a été créé."
 
-#: canaille/oidc/clients.py:218
+#: canaille/oidc/clients.py:233
 msgid "The client has not been edited. Please check your information."
 msgstr "Le client n'a pas été édité. Veuillez vérifier vos informations."
 
-#: canaille/oidc/clients.py:244
+#: canaille/oidc/clients.py:260
 msgid "The client has been edited."
 msgstr "Le client a été édité."
 
-#: canaille/oidc/clients.py:256
+#: canaille/oidc/clients.py:276
 msgid "The client has been deleted."
 msgstr "Le client a été supprimé."
 
 #: canaille/oidc/consents.py:36
 msgid "Could not delete this access"
 msgstr "Impossible de supprimer cet accès."
 
 #: canaille/oidc/consents.py:40
 msgid "The access has been revoked"
 msgstr "L'accès a été révoqué."
 
-#: canaille/oidc/oauth.py:37
+#: canaille/oidc/oauth.py:43
 msgid "Personnal information about yourself, such as your name or your gender."
 msgstr "Vos informations personnelles, comme votre nom ou votre genre."
 
-#: canaille/oidc/oauth.py:39
+#: canaille/oidc/oauth.py:45
 msgid "Your email address."
 msgstr "Votre adresse email."
 
-#: canaille/oidc/oauth.py:40
+#: canaille/oidc/oauth.py:46
 msgid "Your postal address."
 msgstr "Votre adresse postale."
 
-#: canaille/oidc/oauth.py:41
+#: canaille/oidc/oauth.py:47
 msgid "Your phone number."
 msgstr "Votre numéro de téléphone."
 
-#: canaille/oidc/oauth.py:42
+#: canaille/oidc/oauth.py:48
 msgid "Groups you are belonging to"
 msgstr "Les groupes auxquels vous appartenez"
 
-#: canaille/oidc/oauth.py:125
+#: canaille/oidc/oauth.py:136
 msgid "You have been successfully logged out."
 msgstr "Vous avez été déconnecté·e."
 
-#: canaille/templates/about.html:12 canaille/themes/default/base.html:102
+#: canaille/oidc/oauth.py:317
+#, python-format
+msgid "You have been disconnected"
+msgstr "Vous avez été déconnecté·e."
+
+#: canaille/oidc/oauth.py:325
+msgid "An error happened during the logout"
+msgstr "Une erreur est survenue lors de la déconnexion"
+
+#: canaille/oidc/oauth.py:337
+msgid "You have not been disconnected"
+msgstr "Vous n'avez pas été déconnecté"
+
+#: canaille/templates/about.html:12 canaille/themes/default/base.html:104
 msgid "About canaille"
 msgstr "À propos de canaille"
 
 #: canaille/templates/about.html:14
 msgid "Free and open-source identity provider."
 msgstr "Fournisseur d'identité numérique libre"
 
@@ -802,15 +830,15 @@
 "Êtes-vous sûrs de vouloir supprimer votre compte ? Cette action est "
 "irrévocable et toutes vos données seront supprimées pour toujours."
 
 #: canaille/templates/profile.html:51
 msgid "User creation"
 msgstr "Nouvel utilisateur"
 
-#: canaille/templates/profile.html:53 canaille/themes/default/base.html:39
+#: canaille/templates/profile.html:53 canaille/themes/default/base.html:40
 msgid "My profile"
 msgstr "Mon profil"
 
 #: canaille/templates/profile.html:55
 msgid "User profile edition"
 msgstr "Édition d'un profil utilisateur"
 
@@ -1194,15 +1222,15 @@
 msgstr "Changer d'utilisateur"
 
 #: canaille/templates/oidc/user/authorize.html:45
 msgid "Accept"
 msgstr "Accepter"
 
 #: canaille/templates/oidc/user/consent_list.html:18
-#: canaille/themes/default/base.html:45
+#: canaille/themes/default/base.html:47
 msgid "My consents"
 msgstr "Mes autorisations"
 
 #: canaille/templates/oidc/user/consent_list.html:21
 msgid "Consult and revoke the authorization you gave to websites."
 msgstr "Consultez et révoquez les autorisation que vous avez données."
 
@@ -1227,42 +1255,65 @@
 msgstr "Rien ici"
 
 #: canaille/templates/oidc/user/consent_list.html:65
 msgid "You did not authorize applications yet."
 msgstr ""
 "Vous n'avez pas encore autorisé d'application à accéder à votre profil."
 
+#: canaille/templates/oidc/user/logout.html:9
+#: canaille/themes/default/base.html:90
+msgid "Log out"
+msgstr "Déconnexion"
+
+#: canaille/templates/oidc/user/logout.html:10
+msgid "Do you want to log out?"
+msgstr "Voulez vous vous déconnecter ?"
+
+#: canaille/templates/oidc/user/logout.html:14
+#, python-format
+msgid "You are currently logged in as %(username)s."
+msgstr "Vous êtes identifiés en tant que %(username)s"
+
+#: canaille/templates/oidc/user/logout.html:16
+#, python-format
+msgid "The application %(client_name)s want to disconnect your account."
+msgstr "L'application %(client_name)s demande votre déconnexion."
+
+#: canaille/templates/oidc/user/logout.html:33
+msgid "Stay logged"
+msgstr "Rester connecté"
+
+#: canaille/templates/oidc/user/logout.html:36
+msgid "Logout"
+msgstr "Déconnexion"
+
 #: canaille/themes/default/base.html:10
 msgid "authorization interface"
 msgstr " - Interface de gestion des autorisations"
 
-#: canaille/themes/default/base.html:52
+#: canaille/themes/default/base.html:54
 msgid "Users"
 msgstr "Utilisateurs"
 
-#: canaille/themes/default/base.html:69
+#: canaille/themes/default/base.html:71
 msgid "Clients"
 msgstr "Clients"
 
-#: canaille/themes/default/base.html:73
+#: canaille/themes/default/base.html:75
 msgid "Tokens"
 msgstr "Jetons"
 
-#: canaille/themes/default/base.html:77
+#: canaille/themes/default/base.html:79
 msgid "Codes"
 msgstr "Codes"
 
-#: canaille/themes/default/base.html:81
+#: canaille/themes/default/base.html:83
 msgid "Emails"
 msgstr "Courriels"
 
-#: canaille/themes/default/base.html:88
-msgid "Log out"
-msgstr "Déconnexion"
-
 #~ msgid "Logged in as"
 #~ msgstr "Connecté en tant que"
 
 #~ msgid "Create Client"
 #~ msgstr "Créer un client"
 
 #~ msgid "My accesses"
@@ -1418,7 +1469,10 @@
 #~ "below and follow the instructions.\n"
 #~ "                "
 #~ msgstr ""
 #~ "\n"
 #~ "Vous avez été invité à créer un compte sur %(site_name)s. Pour continuer, "
 #~ "vous pouvez cliquer sur le bouton «Créer mon compte» ci-dessous et suivre "
 #~ "les instructions."
+
+#~ msgid "Could not reset your password"
+#~ msgstr "Impossible de réinitialiser votre mot de passe"
```

### Comparing `Canaille-0.0.8/canaille/translations/messages.pot` & `Canaille-0.0.9/canaille/translations/messages.pot`

 * *Files 1% similar despite different names*

```diff
@@ -4,136 +4,149 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-02-23 10:58+0100\n"
+"POT-Creation-Date: 2022-06-02 15:50+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
+"Generated-By: Babel 2.10.1\n"
 
-#: canaille/account.py:82 canaille/account.py:107 canaille/oidc/oauth.py:77
+#: canaille/account.py:93 canaille/account.py:118 canaille/oidc/oauth.py:88
 msgid "Login failed, please check your information"
 msgstr ""
 
-#: canaille/account.py:113
+#: canaille/account.py:124
 #, python-format
 msgid "Connection successful. Welcome %(user)s"
 msgstr ""
 
-#: canaille/account.py:126
+#: canaille/account.py:137
 #, python-format
 msgid "You have been disconnected. See you next time %(user)s"
 msgstr ""
 
-#: canaille/account.py:143
+#: canaille/account.py:155
 msgid "Could not send the password initialization link."
 msgstr ""
 
-#: canaille/account.py:148
+#: canaille/account.py:160
 msgid ""
 "A password initialization link has been sent at your email address. You "
 "should receive it within 10 minutes."
 msgstr ""
 
-#: canaille/account.py:154 canaille/account.py:398
+#: canaille/account.py:166 canaille/account.py:418
 msgid "Could not send the password initialization email"
 msgstr ""
 
-#: canaille/account.py:247 canaille/account.py:324
+#: canaille/account.py:255 canaille/account.py:338
 msgid "User account creation failed."
 msgstr ""
 
-#: canaille/account.py:268 canaille/account.py:296
+#: canaille/account.py:276 canaille/account.py:304
 msgid "The invitation link that brought you here was invalid."
 msgstr ""
 
-#: canaille/account.py:275
+#: canaille/account.py:283
 msgid "The invitation link that brought you here has expired."
 msgstr ""
 
-#: canaille/account.py:282
+#: canaille/account.py:290
 msgid "Your account has already been created."
 msgstr ""
 
-#: canaille/account.py:289
+#: canaille/account.py:297
 msgid "You are already logged in, you cannot create an account."
 msgstr ""
 
-#: canaille/account.py:329
+#: canaille/account.py:316 canaille/forms.py:179 canaille/forms.py:227
+#: canaille/templates/groups.html:11 canaille/templates/userlist.html:17
+#: canaille/themes/default/base.html:61
+msgid "Groups"
+msgstr ""
+
+#: canaille/account.py:343
 msgid "You account has been created successfuly."
 msgstr ""
 
-#: canaille/account.py:371
+#: canaille/account.py:385
 msgid "User account creation succeed."
 msgstr ""
 
-#: canaille/account.py:392
+#: canaille/account.py:412
 msgid ""
 "A password initialization link has been sent at the user email address. "
 "It should be received within 10 minutes."
 msgstr ""
 
-#: canaille/account.py:406
+#: canaille/account.py:429
 msgid ""
 "A password reset link has been sent at the user email address. It should "
 "be received within 10 minutes."
 msgstr ""
 
-#: canaille/account.py:412
+#: canaille/account.py:435
 msgid "Could not send the password reset email"
 msgstr ""
 
-#: canaille/account.py:443
+#: canaille/account.py:469
 msgid "Profile edition failed."
 msgstr ""
 
-#: canaille/account.py:471
+#: canaille/account.py:497
 msgid "Profile updated successfuly."
 msgstr ""
 
-#: canaille/account.py:491
+#: canaille/account.py:520
 #, python-format
 msgid "The user %(user)s has been sucessfuly deleted"
 msgstr ""
 
-#: canaille/account.py:515
+#: canaille/account.py:550
 msgid "Could not send the password reset link."
 msgstr ""
 
-#: canaille/account.py:522 canaille/account.py:533
+#: canaille/account.py:554
 msgid ""
 "A password reset link has been sent at your email address. You should "
 "receive it within 10 minutes."
 msgstr ""
 
-#: canaille/account.py:539
-msgid "Could not reset your password"
+#: canaille/account.py:565
+#, python-format
+msgid ""
+"The user '%(user)s' does not have permissions to update their password. "
+"We cannot send a password reset email."
+msgstr ""
+
+#: canaille/account.py:580
+msgid "We encountered an issue while we sent the password recovery email."
 msgstr ""
 
-#: canaille/account.py:553
+#: canaille/account.py:599
 msgid "The password reset link that brought you here was invalid."
 msgstr ""
 
-#: canaille/account.py:562
+#: canaille/account.py:608
 msgid "Your password has been updated successfuly"
 msgstr ""
 
 #: canaille/admin.py:23 canaille/templates/userlist.html:14
 msgid "Email"
 msgstr ""
 
 #: canaille/admin.py:29 canaille/forms.py:47 canaille/forms.py:71
-#: canaille/forms.py:123 canaille/forms.py:224
+#: canaille/forms.py:123 canaille/forms.py:221
 msgid "jane@doe.com"
 msgstr ""
 
 #: canaille/admin.py:42 canaille/admin.py:44
 msgid "The test invitation mail has been sent correctly"
 msgstr ""
 
@@ -149,15 +162,15 @@
 msgid "Invitation on {website_name}"
 msgstr ""
 
 #: canaille/apputils.py:41
 msgid "John Doe"
 msgstr ""
 
-#: canaille/apputils.py:44 canaille/forms.py:95 canaille/forms.py:212
+#: canaille/apputils.py:44 canaille/forms.py:95 canaille/forms.py:209
 msgid "jdoe"
 msgstr ""
 
 #: canaille/apputils.py:47
 msgid "john@doe.com"
 msgstr ""
 
@@ -197,19 +210,19 @@
 msgid "Password confirmation"
 msgstr ""
 
 #: canaille/forms.py:86 canaille/forms.py:145
 msgid "Password and confirmation do not match."
 msgstr ""
 
-#: canaille/forms.py:94 canaille/forms.py:211
+#: canaille/forms.py:94 canaille/forms.py:208
 msgid "Username"
 msgstr ""
 
-#: canaille/forms.py:98 canaille/forms.py:197 canaille/oidc/clients.py:36
+#: canaille/forms.py:98 canaille/forms.py:194 canaille/oidc/clients.py:36
 #: canaille/templates/groups.html:17
 #: canaille/templates/oidc/admin/client_list.html:23
 #: canaille/templates/userlist.html:11
 msgid "Name"
 msgstr ""
 
 #: canaille/forms.py:100
@@ -224,15 +237,15 @@
 msgid "Family Name"
 msgstr ""
 
 #: canaille/forms.py:111
 msgid "Doe"
 msgstr ""
 
-#: canaille/forms.py:117 canaille/forms.py:217
+#: canaille/forms.py:117 canaille/forms.py:214
 msgid "Email address"
 msgstr ""
 
 #: canaille/forms.py:119
 msgid ""
 "This email will be used as a recovery address to reset the password if "
 "needed"
@@ -266,63 +279,57 @@
 msgid "Website"
 msgstr ""
 
 #: canaille/forms.py:158
 msgid "https://mywebsite.tld"
 msgstr ""
 
-#: canaille/forms.py:182 canaille/forms.py:230
-#: canaille/templates/groups.html:11 canaille/templates/userlist.html:17
-#: canaille/themes/default/base.html:59
-msgid "Groups"
-msgstr ""
-
-#: canaille/forms.py:184
+#: canaille/forms.py:181
 msgid "users, admins ..."
 msgstr ""
 
-#: canaille/forms.py:200
+#: canaille/forms.py:197
 msgid "group"
 msgstr ""
 
-#: canaille/forms.py:204 canaille/templates/groups.html:18
+#: canaille/forms.py:201 canaille/templates/groups.html:18
 msgid "Description"
 msgstr ""
 
-#: canaille/forms.py:215
+#: canaille/forms.py:212
 msgid "Username editable by the invitee"
 msgstr ""
 
-#: canaille/groups.py:44
+#: canaille/groups.py:40
 msgid "Group creation failed."
 msgstr ""
 
-#: canaille/groups.py:56
+#: canaille/groups.py:52
 #, python-format
 msgid "The group %(group)s has been sucessfully created"
 msgstr ""
 
-#: canaille/groups.py:93
+#: canaille/groups.py:92
 msgid "Group edition failed."
 msgstr ""
 
-#: canaille/groups.py:102
+#: canaille/groups.py:101
 #, python-format
 msgid "The group %(group)s has been sucessfully deleted"
 msgstr ""
 
 #: canaille/mails.py:95
 msgid "You have been invited to create an account on {website_name}"
 msgstr ""
 
-#: canaille/ldap_backend/backend.py:48
+#: canaille/ldap_backend/backend.py:50
 msgid "Could not connect to the LDAP server '{uri}'"
 msgstr ""
 
-#: canaille/ldap_backend/backend.py:64
+#: canaille/ldap_backend/backend.py:66
 msgid "LDAP authentication failed with user '{user}'"
 msgstr ""
 
 #: canaille/oidc/clients.py:41
 msgid "Contact"
 msgstr ""
 
@@ -331,118 +338,134 @@
 msgstr ""
 
 #: canaille/oidc/clients.py:51
 msgid "Redirect URIs"
 msgstr ""
 
 #: canaille/oidc/clients.py:56
+msgid "Post logout redirect URIs"
+msgstr ""
+
+#: canaille/oidc/clients.py:61
 msgid "Grant types"
 msgstr ""
 
-#: canaille/oidc/clients.py:68 canaille/templates/oidc/admin/token_view.html:33
+#: canaille/oidc/clients.py:73 canaille/templates/oidc/admin/token_view.html:33
 msgid "Scope"
 msgstr ""
 
-#: canaille/oidc/clients.py:74
+#: canaille/oidc/clients.py:79
 msgid "Response types"
 msgstr ""
 
-#: canaille/oidc/clients.py:80
+#: canaille/oidc/clients.py:85
 msgid "Token Endpoint Auth Method"
 msgstr ""
 
-#: canaille/oidc/clients.py:90
+#: canaille/oidc/clients.py:95
 msgid "Token audiences"
 msgstr ""
 
-#: canaille/oidc/clients.py:96
+#: canaille/oidc/clients.py:101
 msgid "Logo URI"
 msgstr ""
 
-#: canaille/oidc/clients.py:101
+#: canaille/oidc/clients.py:106
 msgid "Terms of service URI"
 msgstr ""
 
-#: canaille/oidc/clients.py:106
+#: canaille/oidc/clients.py:111
 msgid "Policy URI"
 msgstr ""
 
-#: canaille/oidc/clients.py:111
+#: canaille/oidc/clients.py:116
 msgid "Software ID"
 msgstr ""
 
-#: canaille/oidc/clients.py:116
+#: canaille/oidc/clients.py:121
 msgid "Software Version"
 msgstr ""
 
-#: canaille/oidc/clients.py:121
+#: canaille/oidc/clients.py:126
 msgid "JWK"
 msgstr ""
 
-#: canaille/oidc/clients.py:126
+#: canaille/oidc/clients.py:131
 msgid "JKW URI"
 msgstr ""
 
-#: canaille/oidc/clients.py:131
+#: canaille/oidc/clients.py:136
 msgid "Pre-consent"
 msgstr ""
 
-#: canaille/oidc/clients.py:149
+#: canaille/oidc/clients.py:154
 msgid "The client has not been added. Please check your information."
 msgstr ""
 
-#: canaille/oidc/clients.py:184
+#: canaille/oidc/clients.py:190
 msgid "The client has been created."
 msgstr ""
 
-#: canaille/oidc/clients.py:218
+#: canaille/oidc/clients.py:233
 msgid "The client has not been edited. Please check your information."
 msgstr ""
 
-#: canaille/oidc/clients.py:244
+#: canaille/oidc/clients.py:260
 msgid "The client has been edited."
 msgstr ""
 
-#: canaille/oidc/clients.py:256
+#: canaille/oidc/clients.py:276
 msgid "The client has been deleted."
 msgstr ""
 
 #: canaille/oidc/consents.py:36
 msgid "Could not delete this access"
 msgstr ""
 
 #: canaille/oidc/consents.py:40
 msgid "The access has been revoked"
 msgstr ""
 
-#: canaille/oidc/oauth.py:37
+#: canaille/oidc/oauth.py:43
 msgid "Personnal information about yourself, such as your name or your gender."
 msgstr ""
 
-#: canaille/oidc/oauth.py:39
+#: canaille/oidc/oauth.py:45
 msgid "Your email address."
 msgstr ""
 
-#: canaille/oidc/oauth.py:40
+#: canaille/oidc/oauth.py:46
 msgid "Your postal address."
 msgstr ""
 
-#: canaille/oidc/oauth.py:41
+#: canaille/oidc/oauth.py:47
 msgid "Your phone number."
 msgstr ""
 
-#: canaille/oidc/oauth.py:42
+#: canaille/oidc/oauth.py:48
 msgid "Groups you are belonging to"
 msgstr ""
 
-#: canaille/oidc/oauth.py:125
+#: canaille/oidc/oauth.py:136
 msgid "You have been successfully logged out."
 msgstr ""
 
-#: canaille/templates/about.html:12 canaille/themes/default/base.html:102
+#: canaille/oidc/oauth.py:317
+msgid "You have been disconnected"
+msgstr ""
+
+#: canaille/oidc/oauth.py:325
+msgid "An error happened during the logout"
+msgstr ""
+
+#: canaille/oidc/oauth.py:337
+msgid "You have not been disconnected"
+msgstr ""
+
+#: canaille/templates/about.html:12 canaille/themes/default/base.html:104
 msgid "About canaille"
 msgstr ""
 
 #: canaille/templates/about.html:14
 msgid "Free and open-source identity provider."
 msgstr ""
 
@@ -754,15 +777,15 @@
 "and all your data will be removed forever."
 msgstr ""
 
 #: canaille/templates/profile.html:51
 msgid "User creation"
 msgstr ""
 
-#: canaille/templates/profile.html:53 canaille/themes/default/base.html:39
+#: canaille/templates/profile.html:53 canaille/themes/default/base.html:40
 msgid "My profile"
 msgstr ""
 
 #: canaille/templates/profile.html:55
 msgid "User profile edition"
 msgstr ""
 
@@ -1108,15 +1131,15 @@
 msgstr ""
 
 #: canaille/templates/oidc/user/authorize.html:45
 msgid "Accept"
 msgstr ""
 
 #: canaille/templates/oidc/user/consent_list.html:18
-#: canaille/themes/default/base.html:45
+#: canaille/themes/default/base.html:47
 msgid "My consents"
 msgstr ""
 
 #: canaille/templates/oidc/user/consent_list.html:21
 msgid "Consult and revoke the authorization you gave to websites."
 msgstr ""
 
@@ -1140,34 +1163,57 @@
 msgid "Nothing here"
 msgstr ""
 
 #: canaille/templates/oidc/user/consent_list.html:65
 msgid "You did not authorize applications yet."
 msgstr ""
 
+#: canaille/templates/oidc/user/logout.html:9
+#: canaille/themes/default/base.html:90
+msgid "Log out"
+msgstr ""
+
+#: canaille/templates/oidc/user/logout.html:10
+msgid "Do you want to log out?"
+msgstr ""
+
+#: canaille/templates/oidc/user/logout.html:14
+#, python-format
+msgid "You are currently logged in as %(username)s."
+msgstr ""
+
+#: canaille/templates/oidc/user/logout.html:16
+#, python-format
+msgid "The application %(client_name)s want to disconnect your account."
+msgstr ""
+
+#: canaille/templates/oidc/user/logout.html:33
+msgid "Stay logged"
+msgstr ""
+
+#: canaille/templates/oidc/user/logout.html:36
+msgid "Logout"
+msgstr ""
+
 #: canaille/themes/default/base.html:10
 msgid "authorization interface"
 msgstr ""
 
-#: canaille/themes/default/base.html:52
+#: canaille/themes/default/base.html:54
 msgid "Users"
 msgstr ""
 
-#: canaille/themes/default/base.html:69
+#: canaille/themes/default/base.html:71
 msgid "Clients"
 msgstr ""
 
-#: canaille/themes/default/base.html:73
+#: canaille/themes/default/base.html:75
 msgid "Tokens"
 msgstr ""
 
-#: canaille/themes/default/base.html:77
+#: canaille/themes/default/base.html:79
 msgid "Codes"
 msgstr ""
 
-#: canaille/themes/default/base.html:81
+#: canaille/themes/default/base.html:83
 msgid "Emails"
 msgstr ""
-
-#: canaille/themes/default/base.html:88
-msgid "Log out"
-msgstr ""
```

