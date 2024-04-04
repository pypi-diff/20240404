# Comparing `tmp/nb_cli-1.4.0.tar.gz` & `tmp/nb_cli-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nb_cli-1.4.0.tar", last modified: Wed Feb 28 07:20:00 2024, max compression
+gzip compressed data, was "nb_cli-1.4.1.tar", last modified: Thu Apr  4 08:51:35 2024, max compression
```

## Comparing `nb_cli-1.4.0.tar` & `nb_cli-1.4.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
--rw-r--r--   0        0        0     1065 2024-02-28 07:19:38.870690 nb_cli-1.4.0/LICENSE
--rw-r--r--   0        0        0     4105 2024-02-28 07:19:38.870690 nb_cli-1.4.0/README.md
--rw-r--r--   0        0        0      795 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/__init__.py
--rw-r--r--   0        0        0      202 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/__main__.py
--rw-r--r--   0        0        0     3300 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/__init__.py
--rw-r--r--   0        0        0      257 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/__init__.py
--rw-r--r--   0        0        0     6880 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/adapter.py
--rw-r--r--   0        0        0     4257 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/driver.py
--rw-r--r--   0        0        0     7209 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/plugin.py
--rw-r--r--   0        0        0    11119 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/project.py
--rw-r--r--   0        0        0     3421 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/commands/self.py
--rw-r--r--   0        0        0     5491 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/customize.py
--rw-r--r--   0        0        0     1987 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/cli/utils.py
--rw-r--r--   0        0        0    11457 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/compat.py
--rw-r--r--   0        0        0      429 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/config/__init__.py
--rw-r--r--   0        0        0      813 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/config/model.py
--rw-r--r--   0        0        0     6296 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/config/parser.py
--rw-r--r--   0        0        0      347 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/consts.py
--rw-r--r--   0        0        0      472 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/exceptions.py
--rw-r--r--   0        0        0      214 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/extensions.py
--rw-r--r--   0        0        0     3177 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/__init__.py
--rw-r--r--   0        0        0      901 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/adapter.py
--rw-r--r--   0        0        0     2527 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/data.py
--rw-r--r--   0        0        0      411 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/driver.py
--rw-r--r--   0        0        0     6710 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/meta.py
--rw-r--r--   0        0        0     3192 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/pip.py
--rw-r--r--   0        0        0     1593 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/plugin.py
--rw-r--r--   0        0        0     3012 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/process.py
--rw-r--r--   0        0        0     2952 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/project.py
--rw-r--r--   0        0        0     5858 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/reloader.py
--rw-r--r--   0        0        0     2292 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/script.py
--rw-r--r--   0        0        0     1881 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/signal.py
--rw-r--r--   0        0        0     4193 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/store.py
--rw-r--r--   0        0        0      734 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/handlers/venv.py
--rw-r--r--   0        0        0     1258 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/i18n.py
--rw-r--r--   0        0        0     9123 2024-02-28 07:20:00.702796 nb_cli-1.4.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
--rw-r--r--   0        0        0    14124 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
--rw-r--r--   0        0        0      635 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/log/__init__.py
--rw-r--r--   0        0        0        0 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/py.typed
--rw-r--r--   0        0        0      143 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/cookiecutter.json
--rw-r--r--   0        0        0      196 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0      925 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
--rw-r--r--   0        0        0      376 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
--rw-r--r--   0        0        0       73 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0      883 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
--rw-r--r--   0        0        0      789 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
--rw-r--r--   0        0        0      164 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/plugin/cookiecutter.json
--rw-r--r--   0        0        0      315 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/plugin/hooks/post_gen_project.py
--rw-r--r--   0        0        0      503 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
--rw-r--r--   0        0        0       87 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
--rw-r--r--   0        0        0        0 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
--rw-r--r--   0        0        0      318 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/bootstrap/cookiecutter.json
--rw-r--r--   0        0        0      236 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      141 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0      232 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      620 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0      501 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/cookiecutter.json
--rw-r--r--   0        0        0      307 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/hooks/post_gen_project.py
--rw-r--r--   0        0        0      236 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/hooks/pre_gen_project.py
--rw-r--r--   0        0        0      157 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
--rw-r--r--   0        0        0       16 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
--rw-r--r--   0        0        0        0 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
--rw-r--r--   0        0        0     2087 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
--rw-r--r--   0        0        0      328 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
--rw-r--r--   0        0        0      666 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
--rw-r--r--   0        0        0      232 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/meta/_package_version.py.jinja
--rw-r--r--   0        0        0      110 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/meta/nonebot_version.py.jinja
--rw-r--r--   0        0        0      105 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/meta/pip_version.py.jinja
--rw-r--r--   0        0        0      142 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/meta/python_version.py.jinja
--rw-r--r--   0        0        0      181 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
--rw-r--r--   0        0        0     1091 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/project/_prepare.py.jinja
--rw-r--r--   0        0        0      151 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/project/run_project.py.jinja
--rw-r--r--   0        0        0      274 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/script/_entrypoint.py.jinja
--rw-r--r--   0        0        0      158 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/script/list_scripts.py.jinja
--rw-r--r--   0        0        0      333 2024-02-28 07:19:38.870690 nb_cli-1.4.0/nb_cli/template/scripts/script/run_script.py.jinja
--rw-r--r--   0        0        0      203 2024-02-28 07:19:38.874690 nb_cli-1.4.0/pdm_build.py
--rw-r--r--   0        0        0     3033 2024-02-28 07:20:00.706796 nb_cli-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5307 1970-01-01 00:00:00.000000 nb_cli-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-04 08:51:13.586230 nb_cli-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4105 2024-04-04 08:51:13.586230 nb_cli-1.4.1/README.md
+-rw-r--r--   0        0        0      795 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/__init__.py
+-rw-r--r--   0        0        0      202 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/__main__.py
+-rw-r--r--   0        0        0     3300 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/__init__.py
+-rw-r--r--   0        0        0      257 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/__init__.py
+-rw-r--r--   0        0        0     6880 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/adapter.py
+-rw-r--r--   0        0        0     4257 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/driver.py
+-rw-r--r--   0        0        0     7209 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/plugin.py
+-rw-r--r--   0        0        0    11119 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/project.py
+-rw-r--r--   0        0        0     3421 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/commands/self.py
+-rw-r--r--   0        0        0     5491 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/customize.py
+-rw-r--r--   0        0        0     2022 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/cli/utils.py
+-rw-r--r--   0        0        0    11457 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/compat.py
+-rw-r--r--   0        0        0      429 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/config/__init__.py
+-rw-r--r--   0        0        0      813 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/config/model.py
+-rw-r--r--   0        0        0     6288 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/config/parser.py
+-rw-r--r--   0        0        0      347 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/consts.py
+-rw-r--r--   0        0        0      472 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/exceptions.py
+-rw-r--r--   0        0        0      214 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/extensions.py
+-rw-r--r--   0        0        0     3177 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/__init__.py
+-rw-r--r--   0        0        0      901 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/adapter.py
+-rw-r--r--   0        0        0     2527 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/data.py
+-rw-r--r--   0        0        0      411 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/driver.py
+-rw-r--r--   0        0        0     6710 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/meta.py
+-rw-r--r--   0        0        0     3192 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/pip.py
+-rw-r--r--   0        0        0     1593 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/plugin.py
+-rw-r--r--   0        0        0     3012 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/process.py
+-rw-r--r--   0        0        0     2952 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/project.py
+-rw-r--r--   0        0        0     5891 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/reloader.py
+-rw-r--r--   0        0        0     2292 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/script.py
+-rw-r--r--   0        0        0     1881 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/signal.py
+-rw-r--r--   0        0        0     4193 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/store.py
+-rw-r--r--   0        0        0      734 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/handlers/venv.py
+-rw-r--r--   0        0        0     1244 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/i18n.py
+-rw-r--r--   0        0        0     9123 2024-04-04 08:51:35.054046 nb_cli-1.4.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo
+-rw-r--r--   0        0        0    14124 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po
+-rw-r--r--   0        0        0      635 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/log/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/py.typed
+-rw-r--r--   0        0        0      143 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/cookiecutter.json
+-rw-r--r--   0        0        0      196 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      925 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      376 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/bot.{{cookiecutter.py}}
+-rw-r--r--   0        0        0       73 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      883 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      789 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}
+-rw-r--r--   0        0        0      164 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/plugin/cookiecutter.json
+-rw-r--r--   0        0        0      315 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/plugin/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      503 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/__init__.{{cookiecutter.py}}
+-rw-r--r--   0        0        0       87 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/config.{{cookiecutter.py}}
+-rw-r--r--   0        0        0        0 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/plugin/{{cookiecutter.plugin_slug}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      318 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/bootstrap/cookiecutter.json
+-rw-r--r--   0        0        0      236 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/bootstrap/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      141 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0      232 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      620 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      501 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/cookiecutter.json
+-rw-r--r--   0        0        0      307 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      236 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/hooks/pre_gen_project.py
+-rw-r--r--   0        0        0      157 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env
+-rw-r--r--   0        0        0       16 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.dev
+-rw-r--r--   0        0        0        0 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.env.prod
+-rw-r--r--   0        0        0     2087 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore
+-rw-r--r--   0        0        0      328 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/README.md
+-rw-r--r--   0        0        0      666 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/{{cookiecutter.custom.source_dir}}/plugins/.gitkeep
+-rw-r--r--   0        0        0      232 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/scripts/meta/_package_version.py.jinja
+-rw-r--r--   0        0        0      110 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/scripts/meta/nonebot_version.py.jinja
+-rw-r--r--   0        0        0      105 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/scripts/meta/pip_version.py.jinja
+-rw-r--r--   0        0        0      142 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/scripts/meta/python_version.py.jinja
+-rw-r--r--   0        0        0      181 2024-04-04 08:51:13.586230 nb_cli-1.4.1/nb_cli/template/scripts/plugin/list_builtin_plugin.py.jinja
+-rw-r--r--   0        0        0     1091 2024-04-04 08:51:13.590231 nb_cli-1.4.1/nb_cli/template/scripts/project/_prepare.py.jinja
+-rw-r--r--   0        0        0      151 2024-04-04 08:51:13.590231 nb_cli-1.4.1/nb_cli/template/scripts/project/run_project.py.jinja
+-rw-r--r--   0        0        0      274 2024-04-04 08:51:13.590231 nb_cli-1.4.1/nb_cli/template/scripts/script/_entrypoint.py.jinja
+-rw-r--r--   0        0        0      158 2024-04-04 08:51:13.590231 nb_cli-1.4.1/nb_cli/template/scripts/script/list_scripts.py.jinja
+-rw-r--r--   0        0        0      333 2024-04-04 08:51:13.590231 nb_cli-1.4.1/nb_cli/template/scripts/script/run_script.py.jinja
+-rw-r--r--   0        0        0      203 2024-04-04 08:51:13.590231 nb_cli-1.4.1/pdm_build.py
+-rw-r--r--   0        0        0     3219 2024-04-04 08:51:35.062045 nb_cli-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5317 1970-01-01 00:00:00.000000 nb_cli-1.4.1/PKG-INFO
```

### Comparing `nb_cli-1.4.0/LICENSE` & `nb_cli-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/README.md` & `nb_cli-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/__init__.py` & `nb_cli-1.4.1/nb_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/__init__.py` & `nb_cli-1.4.1/nb_cli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/commands/adapter.py` & `nb_cli-1.4.1/nb_cli/cli/commands/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             Choice(f"{x}/adapters/")
             for x in Path(".").glob("*/")
             if x.is_dir() and not x.name.startswith(".") and not x.name.startswith("_")
         ]
         try:
             output_dir = (
                 await ListPrompt(
-                    _("Where to store the adapter?"), detected + [Choice(_("Other"))]
+                    _("Where to store the adapter?"), [*detected, Choice(_("Other"))]
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             ).name
             if output_dir == _("Other"):
                 output_dir = await InputPrompt(
                     _("Output Dir:"),
                     validator=lambda x: len(x) > 0 and Path(x).is_dir(),
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
```

### Comparing `nb_cli-1.4.0/nb_cli/cli/commands/driver.py` & `nb_cli-1.4.1/nb_cli/cli/commands/driver.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/commands/plugin.py` & `nb_cli-1.4.1/nb_cli/cli/commands/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
             and not any(
                 p.name.startswith("_") or p.name.startswith(".") for p in d.parents
             )
         ]
         try:
             output_dir = (
                 await ListPrompt(
-                    _("Where to store the plugin?"), detected + [Choice(_("Other"))]
+                    _("Where to store the plugin?"), [*detected, Choice(_("Other"))]
                 ).prompt_async(style=CLI_DEFAULT_STYLE)
             ).name
             if output_dir == _("Other"):
                 output_dir = await InputPrompt(
                     _("Output Dir:"),
                     validator=lambda x: len(x) > 0 and Path(x).is_dir(),
                     error_message=_("Invalid output dir!"),
```

### Comparing `nb_cli-1.4.0/nb_cli/cli/commands/project.py` & `nb_cli-1.4.1/nb_cli/cli/commands/project.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/commands/self.py` & `nb_cli-1.4.1/nb_cli/cli/commands/self.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/customize.py` & `nb_cli-1.4.1/nb_cli/cli/customize.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/cli/utils.py` & `nb_cli-1.4.1/nb_cli/cli/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import wraps, partial
 from collections.abc import Coroutine
 from typing_extensions import ParamSpec
 from typing import Any, TypeVar, Callable, Optional
 
-import anyio
 import click
+import anyio.to_thread
+import anyio.from_thread
 from noneprompt import InputPrompt
 from prompt_toolkit.styles import Style
 
 from nb_cli import _
 from nb_cli.config import Driver, Plugin, Adapter
 from nb_cli.handlers import format_package_results
```

### Comparing `nb_cli-1.4.0/nb_cli/compat.py` & `nb_cli-1.4.1/nb_cli/compat.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/config/model.py` & `nb_cli-1.4.1/nb_cli/config/model.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/config/parser.py` & `nb_cli-1.4.1/nb_cli/config/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     @property
     def working_dir(self) -> Path:
         return (self._working_dir or self._global_working_dir or Path.cwd()).resolve()
 
     @staticmethod
     def _locate_project_root(cwd: Optional[Path] = None) -> Path:
         cwd = (cwd or Path.cwd()).resolve()
-        for dir in (cwd,) + tuple(cwd.parents):
+        for dir in (cwd, *cwd.parents):
             if dir.joinpath(CONFIG_FILE).is_file():
                 return dir
         raise ProjectNotFoundError(
             _(
                 "Cannot find project root directory! {config_file} file not exists."
             ).format(config_file=CONFIG_FILE)
         )
```

### Comparing `nb_cli-1.4.0/nb_cli/handlers/__init__.py` & `nb_cli-1.4.1/nb_cli/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/adapter.py` & `nb_cli-1.4.1/nb_cli/handlers/adapter.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/data.py` & `nb_cli-1.4.1/nb_cli/handlers/data.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/meta.py` & `nb_cli-1.4.1/nb_cli/handlers/meta.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/pip.py` & `nb_cli-1.4.1/nb_cli/handlers/pip.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/plugin.py` & `nb_cli-1.4.1/nb_cli/handlers/plugin.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/process.py` & `nb_cli-1.4.1/nb_cli/handlers/process.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/project.py` & `nb_cli-1.4.1/nb_cli/handlers/project.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/reloader.py` & `nb_cli-1.4.1/nb_cli/handlers/reloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
         default_excludes = [".*", ".py[cod]", ".sw.*", "~*"]
         self.excludes = [
             default for default in default_excludes if default not in includes
         ]
         self.exclude_dirs = []
         for e in excludes:
-            p = Path(e)
+            p = Path(e).expanduser()
             try:
                 is_dir = p.is_dir()
             except OSError:  # pragma: no cover
                 # gets raised on Windows for values like "*.py"
                 is_dir = False
 
             if is_dir:
-                self.exclude_dirs.append(p)
+                self.exclude_dirs.append(p.resolve())
             else:
                 self.excludes.append(e)
         self.excludes = list(set(self.excludes))
 
     def __call__(self, path: Path) -> bool:
         for include_pattern in self.includes:
             if path.match(include_pattern):
@@ -161,15 +161,15 @@
 
         if self.logger:
             self.logger.info(_("Stopped reloader."))
 
     async def should_restart(self) -> Optional[list[Path]]:
         changes = await self.watcher.__anext__()
         if changes:
-            unique_paths = {Path(c[1]) for c in changes}
+            unique_paths = {Path(c[1]).resolve() for c in changes}
             return [p for p in unique_paths if self.watch_filter(p)]
         return None
 
     def handle_exit(self, sig, frame):
         self.should_exit.set()
 
     def _display_path(self, path: Path) -> str:
```

### Comparing `nb_cli-1.4.0/nb_cli/handlers/script.py` & `nb_cli-1.4.1/nb_cli/handlers/script.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/signal.py` & `nb_cli-1.4.1/nb_cli/handlers/signal.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/store.py` & `nb_cli-1.4.1/nb_cli/handlers/store.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/handlers/venv.py` & `nb_cli-1.4.1/nb_cli/handlers/venv.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/i18n.py` & `nb_cli-1.4.1/nb_cli/i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Optional
 
 from .consts import WINDOWS
 
 
 def _get_win_locale_with_ctypes() -> Optional[str]:
-    import ctypes  # noqa: F811
+    import ctypes
 
     kernel32 = ctypes.windll.kernel32
     lcid: int = kernel32.GetUserDefaultUILanguage()
     return locale.windows_locale.get(lcid)
 
 
 def _get_win_locale_from_registry() -> Optional[str]:
```

### Comparing `nb_cli-1.4.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo` & `nb_cli-1.4.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.mo`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po` & `nb_cli-1.4.1/nb_cli/locale/zh_CN/LC_MESSAGES/nb-cli.po`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/log/__init__.py` & `nb_cli-1.4.1/nb_cli/log/__init__.py`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}` & `nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/adapter.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}` & `nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/event.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}` & `nb_cli-1.4.1/nb_cli/template/adapter/{{cookiecutter.adapter_slug}}/message.{{cookiecutter.py}}`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb_cli-1.4.1/nb_cli/template/project/bootstrap/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore` & `nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml` & `nb_cli-1.4.1/nb_cli/template/project/simple/{{cookiecutter.computed.project_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/nb_cli/template/scripts/project/_prepare.py.jinja` & `nb_cli-1.4.1/nb_cli/template/scripts/project/_prepare.py.jinja`

 * *Files identical despite different names*

### Comparing `nb_cli-1.4.0/pyproject.toml` & `nb_cli-1.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nb-cli"
-version = "1.4.0"
+version = "1.4.1"
 description = "CLI for nonebot2"
 authors = [
     { name = "yanyongyu", email = "yyy@nonebot.dev" },
 ]
 readme = "README.md"
 keywords = [
     "bot",
@@ -21,27 +21,27 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 requires-python = ">=3.9, <4.0"
 dependencies = [
     "click ~=8.1",
-    "anyio ~=3.6",
     "httpx ~=0.18",
     "jinja2 ~=3.0",
-    "cashews ~=6.0",
     "wcwidth ~=0.2",
     "tomlkit ~=0.10",
     "watchfiles ~=0.16",
+    "anyio >=3.6, < 5.0",
     "cookiecutter ~=2.2",
     "virtualenv ~=20.21",
+    "cashews >=6.0, <8.0",
     "typing-extensions ~=4.4",
     "pyfiglet >=1.0.1, <2.0.0",
     "noneprompt >=0.1.9, <1.0.0",
-    "pydantic >=1.10.0,<3.0.0,!=2.5.0,!=2.5.1",
+    "pydantic >=1.10.0, <3.0.0, !=2.5.0, !=2.5.1",
     "importlib-metadata >=4.6; python_version < '3.10'",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
@@ -52,15 +52,15 @@
 nb = "nb_cli.__main__:main"
 
 [tool.pdm.dev-dependencies]
 i18n = [
     "babel ~=2.11",
 ]
 dev = [
-    "ruff ~=0.2.0",
+    "ruff ~=0.3.0",
     "isort ~=5.10",
     "black >=22.3.0",
     "nonemoji ~=0.1",
     "pre-commit ~=3.1",
     "importlib-metadata",
 ]
 docs = [
@@ -126,28 +126,38 @@
     "nb_cli/template/",
 ]
 line-length = 88
 target-version = "py39"
 
 [tool.ruff.lint]
 select = [
-    "E",
-    "W",
     "F",
+    "W",
+    "E",
     "UP",
-    "C",
-    "T",
+    "ASYNC",
+    "C4",
+    "T10",
+    "T20",
+    "PYI",
     "PT",
     "Q",
+    "RUF",
 ]
 ignore = [
     "E402",
-    "C901",
     "UP037",
+    "RUF001",
+    "RUF002",
+    "RUF003",
 ]
 
+[tool.ruff.lint.flake8-pytest-style]
+fixture-parentheses = false
+mark-parentheses = false
+
 [build-system]
 requires = [
     "pdm-backend",
     "babel~=2.11",
 ]
 build-backend = "pdm.backend"
```

### Comparing `nb_cli-1.4.0/PKG-INFO` & `nb_cli-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nb-cli
-Version: 1.4.0
+Version: 1.4.1
 Summary: CLI for nonebot2
 Keywords: bot qq nonebot bot qq nonebot
 Home-page: https://cli.nonebot.dev/
 Author-Email: yanyongyu <yyy@nonebot.dev>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
@@ -12,23 +12,23 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://cli.nonebot.dev/
 Project-URL: Repository, https://github.com/nonebot/nb-cli
 Requires-Python: <4.0,>=3.9
 Requires-Dist: click~=8.1
-Requires-Dist: anyio~=3.6
 Requires-Dist: httpx~=0.18
 Requires-Dist: jinja2~=3.0
-Requires-Dist: cashews~=6.0
 Requires-Dist: wcwidth~=0.2
 Requires-Dist: tomlkit~=0.10
 Requires-Dist: watchfiles~=0.16
+Requires-Dist: anyio<5.0,>=3.6
 Requires-Dist: cookiecutter~=2.2
 Requires-Dist: virtualenv~=20.21
+Requires-Dist: cashews<8.0,>=6.0
 Requires-Dist: typing-extensions~=4.4
 Requires-Dist: pyfiglet<2.0.0,>=1.0.1
 Requires-Dist: noneprompt<1.0.0,>=0.1.9
 Requires-Dist: pydantic!=2.5.0,!=2.5.1,<3.0.0,>=1.10.0
 Requires-Dist: importlib-metadata>=4.6; python_version < "3.10"
 Description-Content-Type: text/markdown
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_3i4rb4uz_/tmpvyowb034_TarContainer/0/78", line 190, column 0: CDATA terminal not found*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: nb-cli Version: 1.4.0 Summary: CLI for nonebot2
+Metadata-Version: 2.1 Name: nb-cli Version: 1.4.1 Summary: CLI for nonebot2
 Keywords: bot qq nonebot bot qq nonebot Home-page: https://cli.nonebot.dev/
 Author-Email: yanyongyu
 nonebot.dev> License: MIT Classifier: Development Status :: 5 - Production/
 Stable Classifier: Framework :: Robot Framework Classifier: Framework :: Robot
 Framework :: Library Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Project-URL: Homepage, https://cli.nonebot.dev/ Project-URL:
 Repository, https://github.com/nonebot/nb-cli Requires-Python: <4.0,>=3.9
-Requires-Dist: click~=8.1 Requires-Dist: anyio~=3.6 Requires-Dist: httpx~=0.18
-Requires-Dist: jinja2~=3.0 Requires-Dist: cashews~=6.0 Requires-Dist:
-wcwidth~=0.2 Requires-Dist: tomlkit~=0.10 Requires-Dist: watchfiles~=0.16
-Requires-Dist: cookiecutter~=2.2 Requires-Dist: virtualenv~=20.21 Requires-
-Dist: typing-extensions~=4.4 Requires-Dist: pyfiglet<2.0.0,>=1.0.1 Requires-
-Dist: noneprompt<1.0.0,>=0.1.9 Requires-Dist:
+Requires-Dist: click~=8.1 Requires-Dist: httpx~=0.18 Requires-Dist: jinja2~=3.0
+Requires-Dist: wcwidth~=0.2 Requires-Dist: tomlkit~=0.10 Requires-Dist:
+watchfiles~=0.16 Requires-Dist: anyio<5.0,>=3.6 Requires-Dist:
+cookiecutter~=2.2 Requires-Dist: virtualenv~=20.21 Requires-Dist:
+cashews<8.0,>=6.0 Requires-Dist: typing-extensions~=4.4 Requires-Dist:
+pyfiglet<2.0.0,>=1.0.1 Requires-Dist: noneprompt<1.0.0,>=0.1.9 Requires-Dist:
 pydantic!=2.5.0,!=2.5.1,<3.0.0,>=1.10.0 Requires-Dist: importlib-metadata>=4.6;
 python_version < "3.10" Description-Content-Type: text/markdown
                                    _[_n_o_n_e_b_o_t_]
                   # NB CLI _â¨ NoneBot2 å½ä»¤è¡å·¥å· â¨_
                    _[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]_[_s_i_t_e_]_[_p_r_e_-_c_o_m_m_i_t_]
          _[_Q_Q_ _C_h_a_t_ _G_r_o_u_p_]_[_Q_Q_ _C_h_a_n_n_e_l_]_[_T_e_l_e_g_r_a_m_ _C_h_a_n_n_e_l_]_[_D_i_s_c_o_r_d_ _S_e_r_v_e_r_]
                       _æ___æ_¡_£ Â· _å_®__è_£_ Â· _N_o_n_e_B_o_t_ _æ___æ_¡_£
```

