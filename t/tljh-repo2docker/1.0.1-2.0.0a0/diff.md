# Comparing `tmp/tljh_repo2docker-1.0.1.tar.gz` & `tmp/tljh_repo2docker-2.0.0a0.tar.gz`

## Comparing `tljh_repo2docker-1.0.1.tar` & `tljh_repo2docker-2.0.0a0.tar`

### file list

```diff
@@ -1,25 +1,139 @@
--rw-r--r--   0        0        0     7136 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/__init__.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/__version__.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/builder.py
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/docker.py
--rw-r--r--   0        0        0      826 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/images.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/logs.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/static/css/style.css
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/static/js/images.js
--rw-r--r--   0        0        0     2377 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/static/vendor/xterm-addon-fit.js
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/static/vendor/xterm.css
--rw-r--r--   0        0        0   251949 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/static/vendor/xterm.js
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/templates/admin.html
--rw-r--r--   0        0        0     6418 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/templates/images.html
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/templates/page.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/__init__.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/conftest.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_builder.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_images.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_logs.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/tljh_repo2docker/tests/utils.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/LICENSE
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 tljh_repo2docker-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/.prettierignore
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/CHANGELOG.md
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/dev-requirements.txt
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/jupyterhub_config.py
+-rw-r--r--   0        0        0   279512 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/package-lock.json
+-rw-r--r--   0        0        0     4888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/package.json
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/pytest.ini
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/setup.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tsconfig.json
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/webpack.config.js
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/AxiosContext.tsx
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/ButtonWithConfirm.tsx
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/JupyterhubContext.ts
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/LoadingAnimation.tsx
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/SmallTextField.tsx
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/axiosclient.ts
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/style.css
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/theme.ts
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/common/utils.ts
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/App.tsx
+-rw-r--r--   0        0        0     3888 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/EnvironmentList.tsx
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/LogDialog.tsx
+-rw-r--r--   0        0        0     8432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/NewEnvironmentDialog.tsx
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/RemoveEnvironmentButton.tsx
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/main.tsx
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/environments/types.ts
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/App.tsx
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/NewServerDialog.tsx
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/OpenServerButton.tsx
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/RemoveServerButton.tsx
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/ServersList.tsx
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/main.tsx
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/src/servers/types.ts
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/__main__.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/_version.py
+-rw-r--r--   0        0        0     7037 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/app.py
+-rw-r--r--   0        0        0     5523 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/base.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/builder.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/docker.py
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/environments.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/logs.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/model.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/servers.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/servers_api.py
+-rw-r--r--   0        0        0    11453 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/images/jupyterhub-80.png
+-rw-r--r--   0        0        0     9576 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1431d1cef06ad04f5458.woff2
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/169619821ea93019d1bb.woff2
+-rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/182712ab85f1472cdb2f.woff
+-rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/198a421f279162d59143.woff
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1a05a4887ccb810cb4dd.woff
+-rw-r--r--   0        0        0    14424 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/1f075502d0094a398e21.woff
+-rw-r--r--   0        0        0    15860 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/227c93190fe7f82de3f8.woff2
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/249853776d22a271b2b5.woff
+-rw-r--r--   0        0        0    10184 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/252057e589a0379208ed.woff
+-rw-r--r--   0        0        0    13448 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/268f264f58eba5c07c88.woff
+-rw-r--r--   0        0        0     5560 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3230f9b040f3c630e0c3.woff2
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/32fc45a3d1e8ea11fabc.woff2
+-rw-r--r--   0        0        0     5548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3425a701027d0699e369.woff2
+-rw-r--r--   0        0        0    13548 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3503ec5cc6330e21f695.woff
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/35b9d6be04b95f0f0530.woff2
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/392a45a84c081c4b412d.woff
+-rw-r--r--   0        0        0    14384 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/3f2b9a42f643e62a49b7.woff
+-rw-r--r--   0        0        0    15000 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4777461b144e55145268.woff2
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/4df79f684fcbca8386bd.woff
+-rw-r--r--   0        0        0     6936 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/50e795c1345353b0e996.woff2
+-rw-r--r--   0        0        0     8428 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/5b5f2f31962967dfc22c.woff
+-rw-r--r--   0        0        0    14968 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/62ced72e5832f02c2796.woff2
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/657896dad292ee9a0a0a.woff
+-rw-r--r--   0        0        0    10540 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/662bc4c2c037bb0bd529.woff
+-rw-r--r--   0        0        0    14420 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/666d7a2f9db53cf52e2d.woff
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/6fb9cffb1d3e72bf9293.woff2
+-rw-r--r--   0        0        0     9628 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/71a33b6b50457b2c903a.woff2
+-rw-r--r--   0        0        0    15344 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/804378952da8a10faae2.woff2
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8472d69545c7409091b4.woff
+-rw-r--r--   0        0        0    11872 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/861b791f9de857a6e7bc.woff2
+-rw-r--r--   0        0        0     6444 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/8ecd7085cfe9bc2c22ac.woff
+-rw-r--r--   0        0        0    11800 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9165081d10e1ba601384.woff2
+-rw-r--r--   0        0        0     8700 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/965aebef74db72eaf236.woff
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/9ac81fefbe6c319ea40b.woff2
+-rw-r--r--   0        0        0     6300 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/a84892c56152037b3552.woff
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/af4d91666ea345601bea.woff
+-rw-r--r--   0        0        0    15744 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/b009a76ad6afe4ebd301.woff2
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/bd9854c751441ccc1a70.woff2
+-rw-r--r--   0        0        0    14684 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/be4d02458ce53887dc37.woff2
+-rw-r--r--   0        0        0    10168 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1cc6d6fc851b3a2f79d.woff
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c1d66054fe23e181d92c.woff
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c35e4c3958e209d17b31.woff2
+-rw-r--r--   0        0        0    15740 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/c48fb6765a9fcb00b330.woff2
+-rw-r--r--   0        0        0     9840 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/cad7d3d9cb265e334e58.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d010f1f324e111a22e53.woff2
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/d8642a3d1d4ef6179644.woff2
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/db2632771401f61463fe.woff2
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dc7dcec8e3f654e0ed63.woff2
+-rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/dfdff8fa12eac629d29f.woff
+-rw-r--r--   0        0        0     4752 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/e0e8ba725ebd107367a8.woff
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/eaa367bbd0b333a7f80b.woff
+-rw-r--r--   0        0        0    11824 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/ed67ad54b1a8f5d21150.woff2
+-rw-r--r--   0        0        0  1060959 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/environments.js.LICENSE.txt
+-rw-r--r--   0        0        0    15920 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f25d774ecfe0996f8eb5.woff2
+-rw-r--r--   0        0        0    14956 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f52426bf18280380fe67.woff
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f708607d2a7290fb8bfa.woff
+-rw-r--r--   0        0        0     8660 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/f8a034d72aa6828199d4.woff
+-rw-r--r--   0        0        0  1062513 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/static/js/servers.js.LICENSE.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/images.html
+-rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/page.html
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/templates/servers.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/__init__.py
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/conftest.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_builder.py
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_images.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_logs.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/utils.py
+-rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/package-lock.json
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/package.json
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/admin-linux.png
+-rw-r--r--   0        0        0   108741 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-console-linux.png
+-rw-r--r--   0        0        0    51218 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-dialog-linux.png
+-rw-r--r--   0        0        0    29532 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-list-linux.png
+-rw-r--r--   0        0        0    43210 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-remove-confirm-linux.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environment-removed-linux.png
+-rw-r--r--   0        0        0    24456 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/environments-page-linux.png
+-rw-r--r--   0        0        0    29865 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/login-page-linux.png
+-rw-r--r--   0        0        0    25943 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/running-servers-linux.png
+-rw-r--r--   0        0        0    41305 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-remove-confirm-linux.png
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/server-removed-linux.png
+-rw-r--r--   0        0        0    49850 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-dialog-linux.png
+-rw-r--r--   0        0        0    22244 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/servers-page-linux.png
+-rw-r--r--   0        0        0    20933 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/ui-tests/tests/ui.test.ts-snapshots/user-linux.png
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/LICENSE
+-rw-r--r--   0        0        0     8219 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/README.md
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0    10226 2020-02-02 00:00:00.000000 tljh_repo2docker-2.0.0a0/PKG-INFO
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/__init__.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-import os
-
 from aiodocker import Docker
 from dockerspawner import DockerSpawner
-from jinja2 import Environment, BaseLoader
+from jinja2 import BaseLoader, Environment
 from jupyter_client.localinterfaces import public_ips
-from jupyterhub.handlers.static import CacheControlStaticFilesHandler
 from jupyterhub.traitlets import ByteSpecification
-from tljh.hooks import hookimpl
 from tljh.configurer import load_config
+from tljh.hooks import hookimpl
 from traitlets import Unicode
 from traitlets.config import Configurable
 
-from .builder import BuildHandler
 from .docker import list_images
-from .images import ImagesHandler
-from .logs import LogsHandler
 
 # Default CPU period
 # See: https://docs.docker.com/config/containers/resource_constraints/#limit-a-containers-access-to-memory#configure-the-default-cfs-scheduler
 CPU_PERIOD = 100_000
 
+TLJH_R2D_ADMIN_SCOPE = "custom:tljh_repo2docker:admin"
 
-class SpawnerMixin(Configurable):
 
+class SpawnerMixin(Configurable):
     """
     Mixin for spawners that derive from DockerSpawner, to use local Docker images
     built with tljh-repo2docker.
 
     Call `set_limits` in the spawner `start` method to set the memory and cpu limits.
     """
 
@@ -129,21 +124,20 @@
     async def set_limits(self):
         """
         Set the user environment limits if they are defined in the image
         """
         imagename = self.user_options.get("image")
         async with Docker() as docker:
             image = await docker.images.inspect(imagename)
-
-        mem_limit = image["ContainerConfig"]["Labels"].get(
-            "tljh_repo2docker.mem_limit", None
-        )
-        cpu_limit = image["ContainerConfig"]["Labels"].get(
-            "tljh_repo2docker.cpu_limit", None
-        )
+        config = image.get("ContainerConfig", None)
+        if not config:
+            config = image.get("Config", {})
+        label = config.get("Labels", {})
+        mem_limit = label.get("tljh_repo2docker.mem_limit", None)
+        cpu_limit = label.get("tljh_repo2docker.cpu_limit", None)
 
         # override the spawner limits if defined in the image
         if mem_limit:
             self.mem_limit = mem_limit
         if cpu_limit:
             self.cpu_limit = float(cpu_limit)
 
@@ -169,45 +163,16 @@
 @hookimpl
 def tljh_custom_jupyterhub_config(c):
     # hub
     c.JupyterHub.hub_ip = public_ips()[0]
     c.JupyterHub.cleanup_servers = False
     c.JupyterHub.spawner_class = Repo2DockerSpawner
 
-    # add extra templates for the service UI
-    c.JupyterHub.template_paths.insert(
-        0, os.path.join(os.path.dirname(__file__), "templates")
-    )
-
     # spawner
     c.DockerSpawner.cmd = ["jupyterhub-singleuser"]
     c.DockerSpawner.pull_policy = "Never"
     c.DockerSpawner.remove = True
 
-    # fetch limits from the TLJH config
-    tljh_config = load_config()
-    limits = tljh_config["limits"]
-    cpu_limit = limits["cpu"]
-    mem_limit = limits["memory"]
-
-    c.JupyterHub.tornado_settings.update(
-        {"default_cpu_limit": cpu_limit, "default_mem_limit": mem_limit}
-    )
-
-    # register the handlers to manage the user images
-    c.JupyterHub.extra_handlers.extend(
-        [
-            (r"environments", ImagesHandler),
-            (r"api/environments", BuildHandler),
-            (r"api/environments/([^/]+)/logs", LogsHandler),
-            (
-                r"environments-static/(.*)",
-                CacheControlStaticFilesHandler,
-                {"path": os.path.join(os.path.dirname(__file__), "static")},
-            ),
-        ]
-    )
-
 
 @hookimpl
 def tljh_extra_hub_pip_packages():
-    return ["dockerspawner~=0.11", "jupyter_client~=6.1", "aiodocker~=0.19"]
+    return ["dockerspawner~=0.11", "jupyter_client>=6.1,<8", "aiodocker~=0.19"]
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/builder.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import json
 import re
 
 from aiodocker import Docker, DockerError
-from jupyterhub.apihandlers import APIHandler
-from jupyterhub.utils import admin_only
 from tornado import web
 
+from .base import BaseHandler, require_admin_role
 from .docker import build_image
 
 IMAGE_NAME_RE = r"^[a-z0-9-_]+$"
 
 
-class BuildHandler(APIHandler):
+class BuildHandler(BaseHandler):
     """
     Handle requests to build user environments as Docker images
     """
 
     @web.authenticated
-    @admin_only
+    @require_admin_role
     async def delete(self):
         data = self.get_json_body()
         name = data["name"]
         async with Docker() as docker:
             try:
                 await docker.images.delete(name)
             except DockerError as e:
                 raise web.HTTPError(e.status, e.message)
 
         self.set_status(200)
+        self.set_header("content-type", "application/json")
         self.finish(json.dumps({"status": "ok"}))
 
     @web.authenticated
-    @admin_only
+    @require_admin_role
     async def post(self):
         data = self.get_json_body()
         repo = data["repo"]
         ref = data["ref"]
         name = data["name"].lower()
         memory = data["memory"]
         cpu = data["cpu"]
@@ -64,17 +64,16 @@
                 f"The name of the environment is restricted to the following characters: {IMAGE_NAME_RE}",
             )
 
         extra_buildargs = []
         if buildargs:
             for barg in buildargs.split("\n"):
                 if "=" not in barg:
-                    raise web.HTTPError(
-                        400,
-                        "Invalid build argument format"
-                    )
+                    raise web.HTTPError(400, "Invalid build argument format")
                 extra_buildargs.append(barg)
-
-        await build_image(repo, ref, name, memory, cpu, username, password, extra_buildargs)
+        await build_image(
+            repo, ref, name, memory, cpu, username, password, extra_buildargs
+        )
 
         self.set_status(200)
+        self.set_header("content-type", "application/json")
         self.finish(json.dumps({"status": "ok"}))
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/docker.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-
 from urllib.parse import urlparse
 
 from aiodocker import Docker
 
 
 async def list_images():
     """
@@ -51,16 +50,22 @@
         for container in r2d_containers
         if "repo2docker.build" in container["Labels"]
     ]
     return containers
 
 
 async def build_image(
-    repo, ref, name="", memory=None, cpu=None, username=None, password=None,
-    extra_buildargs=None
+    repo,
+    ref,
+    name="",
+    memory=None,
+    cpu=None,
+    username=None,
+    password=None,
+    extra_buildargs=None,
 ):
     """
     Build an image given a repo, ref and limits
     """
     ref = ref or "HEAD"
     if len(ref) >= 40:
         ref = ref[:7]
@@ -92,24 +97,18 @@
         "1100",
         "--no-run",
         "--image-name",
         image_name,
     ]
 
     for label in labels:
-        cmd += [
-            "--label",
-            label
-        ]
+        cmd += ["--label", label]
 
     for barg in extra_buildargs or []:
-        cmd += [
-            "--build-arg",
-            barg
-        ]
+        cmd += ["--build-arg", barg]
 
     cmd.append(repo)
 
     config = {
         "Cmd": cmd,
         "Image": "quay.io/jupyterhub/repo2docker:main",
         "Labels": {
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/images.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/environments.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from inspect import isawaitable
-from jupyterhub.handlers.base import BaseHandler
-from jupyterhub.utils import admin_only
+
 from tornado import web
 
+from .base import BaseHandler, require_admin_role
 from .docker import list_containers, list_images
 
 
-class ImagesHandler(BaseHandler):
+class EnvironmentsHandler(BaseHandler):
     """
     Handler to show the list of environments as Docker images
     """
 
     @web.authenticated
-    @admin_only
+    @require_admin_role
     async def get(self):
         images = await list_images()
         containers = await list_containers()
         result = self.render_template(
             "images.html",
             images=images + containers,
             default_mem_limit=self.settings.get("default_mem_limit"),
             default_cpu_limit=self.settings.get("default_cpu_limit"),
+            machine_profiles=self.settings.get("machine_profiles", []),
         )
         if isawaitable(result):
             self.write(await result)
         else:
             self.write(result)
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/logs.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 
 from aiodocker import Docker
-from jupyterhub.apihandlers import APIHandler
-from jupyterhub.utils import admin_only
 from tornado import web
-from tornado.ioloop import IOLoop
 from tornado.iostream import StreamClosedError
 
+from .base import BaseHandler, require_admin_role
 
-class LogsHandler(APIHandler):
+
+class LogsHandler(BaseHandler):
     """
     Expose a handler to follow the build logs.
     """
+
     @web.authenticated
-    @admin_only
+    @require_admin_role
     async def get(self, name):
         self.set_header("Content-Type", "text/event-stream")
         self.set_header("Cache-Control", "no-cache")
 
         async with Docker() as docker:
             containers = await docker.containers.list(
                 filters=json.dumps({"label": [f"repo2docker.build={name}"]})
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_builder.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pytest
-
 from aiodocker import Docker, DockerError
 
-from .utils import add_environment, wait_for_image, remove_environment
+from .utils import add_environment, remove_environment, wait_for_image
 
 
 @pytest.mark.asyncio
 async def test_add_environment(app, minimal_repo, image_name):
     name, ref = image_name.split(":")
     r = await add_environment(app, repo=minimal_repo, name=name, ref=ref)
     assert r.status_code == 200
@@ -39,32 +38,39 @@
 
 @pytest.mark.asyncio
 async def test_uppercase_repo(app, minimal_repo_uppercase, generated_image_name):
     r = await add_environment(app, repo=minimal_repo_uppercase)
     assert r.status_code == 200
     image = await wait_for_image(image_name=generated_image_name)
     assert (
-        image["ContainerConfig"]["Labels"]["tljh_repo2docker.image_name"] == generated_image_name
+        image["ContainerConfig"]["Labels"]["tljh_repo2docker.image_name"]
+        == generated_image_name
     )
 
 
 @pytest.mark.asyncio
 async def test_no_repo(app, image_name):
     name, ref = image_name.split(":")
     r = await add_environment(app, repo="", name=name, ref=ref)
     assert r.status_code == 400
 
 
 @pytest.mark.asyncio
 @pytest.mark.parametrize(
-    "memory, cpu", [("abcded", ""), ("", "abcde"),],
+    "memory, cpu",
+    [
+        ("abcded", ""),
+        ("", "abcde"),
+    ],
 )
 async def test_wrong_limits(app, minimal_repo, image_name, memory, cpu):
     name, ref = image_name.split(":")
-    r = await add_environment(app, repo=minimal_repo, name=name, ref=ref, memory=memory, cpu=cpu)
+    r = await add_environment(
+        app, repo=minimal_repo, name=name, ref=ref, memory=memory, cpu=cpu
+    )
     assert r.status_code == 400
     assert "must be a number" in r.text
 
 
 @pytest.mark.asyncio
 async def test_wrong_name(app, minimal_repo):
     r = await add_environment(app, repo=minimal_repo, name="#WRONG_NAME#")
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_images.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_images.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,51 @@
 import pytest
-
 from jupyterhub.tests.utils import get_page
 
-from .utils import add_environment, wait_for_image
+from .utils import add_environment, get_service_page, wait_for_image
 
 
 @pytest.mark.asyncio
 async def test_images_list_admin(app):
-    cookies = await app.login_user('admin')
-    r = await get_page('environments', app, cookies=cookies, allow_redirects=False)
+    cookies = await app.login_user("admin")
+    r = await get_service_page(
+        "environments",
+        app,
+        cookies=cookies,
+        allow_redirects=True,
+    )
     r.raise_for_status()
-    assert 'Repository' in r.text
+    assert (
+        '{"images": [], "default_mem_limit": "None", "default_cpu_limit":"None", "machine_profiles": []}'
+        in r.text
+    )
 
 
 @pytest.mark.asyncio
 async def test_images_list_not_admin(app):
-    cookies = await app.login_user('wash')
-    r = await get_page('environments', app, cookies=cookies, allow_redirects=False)
+    cookies = await app.login_user("wash")
+    r = await get_service_page(
+        "environments", app, cookies=cookies, allow_redirects=True
+    )
     assert r.status_code == 403
 
 
 @pytest.mark.asyncio
 async def test_spawn_page(app, minimal_repo, image_name):
-    cookies = await app.login_user('admin')
+    cookies = await app.login_user("admin")
 
     # go to the spawn page
-    r = await get_page('spawn', app, cookies=cookies, allow_redirects=False)
+    r = await get_page("spawn", app, cookies=cookies, allow_redirects=False)
     r.raise_for_status()
     assert minimal_repo not in r.text
 
     # add a new envionment
     name, ref = image_name.split(":")
     r = await add_environment(app, repo=minimal_repo, name=name, ref=ref)
     assert r.status_code == 200
     await wait_for_image(image_name=image_name)
 
     # the environment should be on the page
-    r = await get_page('spawn', app, cookies=cookies, allow_redirects=False)
+    r = await get_page("spawn", app, cookies=cookies, allow_redirects=False)
     r.raise_for_status()
     assert r.status_code == 200
     assert minimal_repo in r.text
```

### Comparing `tljh_repo2docker-1.0.1/tljh_repo2docker/tests/test_logs.py` & `tljh_repo2docker-2.0.0a0/tljh_repo2docker/tests/test_logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 
 import pytest
+from jupyterhub.tests.utils import async_requests
 
-from jupyterhub.tests.utils import api_request, async_requests
-
-from .utils import add_environment, wait_for_image
+from .utils import add_environment, api_request, wait_for_image
 
 
 def next_event(it):
     """read an event from an eventstream
     From: https://github.com/jupyterhub/jupyterhub/blob/81d423d6c674765400a6fe88064c1366b7070f94/jupyterhub/tests/test_api.py#L692-L700
     """
     while True:
@@ -35,10 +34,12 @@
 
     r.close()
     await wait_for_image(image_name=image_name)
 
 
 @pytest.mark.asyncio
 async def test_no_build(app, image_name, request):
-    r = await api_request(app, "environments", "image-not-found:12345", "logs", stream=True)
+    r = await api_request(
+        app, "environments", "image-not-found:12345", "logs", stream=True
+    )
     request.addfinalizer(r.close)
     assert r.status_code == 404
```

### Comparing `tljh_repo2docker-1.0.1/LICENSE` & `tljh_repo2docker-2.0.0a0/LICENSE`

 * *Files identical despite different names*

