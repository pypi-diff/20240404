# Comparing `tmp/graphinate-0.2.8.tar.gz` & `tmp/graphinate-0.2.9.tar.gz`

## Comparing `graphinate-0.2.8.tar` & `graphinate-0.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 graphinate-0.2.8/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 graphinate-0.2.8/STATS.md
--rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 graphinate-0.2.8/mkdocs.yml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 graphinate-0.2.8/sonar-project.properties
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/dependabot.yml
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/workflows/publish-docs.yaml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/workflows/test-beta.yml
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 graphinate-0.2.8/.github/workflows/test.yml
--rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/acknowledge.md
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/dev.md
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/gen_ref_pages.py
--rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/index.md
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/intro.md
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/start.md
--rw-r--r--   0        0        0    25635 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/assets/images/logo-128.png
--rw-r--r--   0        0        0    32663 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/assets/images/network_graph.png
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/assets/stylesheets/extra.css
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/examples/code.md
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/examples/github.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/examples/math.md
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/examples/web.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/usage/cli.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 graphinate-0.2.8/docs/usage/lib.md
--rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/code/python_ast.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/code/python_dependencies.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/code/requirements.txt
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/_client.py
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/commits_visibilty_graph.py
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/followers.graphql
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/followers.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/graphql.config.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/repositories.graphql
--rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/repositories.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/github/requirements.txt
--rw-r--r--   0        0        0    24051 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/math/graph_atlas.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/math/polygonal_graph.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/web/page_links.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 graphinate-0.2.8/examples/web/requirements.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/genric_graph.graphql
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/graphql.config.yml
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/house_of_graphs.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/ethernet/traceroute.py
--rw-r--r--   0        0        0  2499201 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/social/albums.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/social/musicisians.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/text/nlp_graph.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/text/requirements.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/time_series/requirements.txt
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 graphinate-0.2.8/playground/time_series/visibility_graph.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/__main__.py
--rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/builders.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/cli.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/color.py
--rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/modeling.py
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/typing.py
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/materializers/__init__.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/materializers/matplotlib.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/__init__.py
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/starlette/__init__.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/starlette/views.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/graphiql/__init__.py
--rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/graphiql/index.html
--rw-r--r--   0        0        0    29055 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/static/images/logo-128.png
--rw-r--r--   0        0        0    32663 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/static/images/network_graph.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/viewer/__init__.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/viewer/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/voyager/__init__.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/server/web/voyager/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/tools/__init__.py
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/tools/gui.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 graphinate-0.2.8/src/graphinate/tools/mutators.py
--rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_builders.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_cli.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_color.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_materializers.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_modeling.py
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_server.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 graphinate-0.2.8/tests/graphinate/test_tools.py
--rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 graphinate-0.2.8/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 graphinate-0.2.8/LICENSE
--rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 graphinate-0.2.8/README.md
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 graphinate-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    14190 2020-02-02 00:00:00.000000 graphinate-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 graphinate-0.2.9/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 graphinate-0.2.9/STATS.md
+-rw-r--r--   0        0        0     3068 2020-02-02 00:00:00.000000 graphinate-0.2.9/mkdocs.yml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 graphinate-0.2.9/sonar-project.properties
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/workflows/publish-docs.yaml
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/workflows/test-beta.yml
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 graphinate-0.2.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0     2923 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/acknowledge.md
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/dev.md
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/gen_ref_pages.py
+-rw-r--r--   0        0        0     4508 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/index.md
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/intro.md
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/start.md
+-rw-r--r--   0        0        0    25635 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/assets/images/logo-128.png
+-rw-r--r--   0        0        0    32663 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/assets/images/network_graph.png
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/assets/stylesheets/extra.css
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/examples/code.md
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/examples/github.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/examples/math.md
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/examples/web.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/usage/cli.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 graphinate-0.2.9/docs/usage/lib.md
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/code/python_ast.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/code/python_dependencies.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/code/requirements.txt
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/_client.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/commits_visibilty_graph.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/followers.graphql
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/followers.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/graphql.config.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/repositories.graphql
+-rw-r--r--   0        0        0     4521 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/repositories.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/github/requirements.txt
+-rw-r--r--   0        0        0    24051 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/math/graph_atlas.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/math/polygonal_graph.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/web/page_links.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 graphinate-0.2.9/examples/web/requirements.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/genric_graph.graphql
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/graphql.config.yml
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/house_of_graphs.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/ethernet/traceroute.py
+-rw-r--r--   0        0        0  2499201 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/social/albums.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/social/musicisians.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/text/nlp_graph.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/text/requirements.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/time_series/requirements.txt
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 graphinate-0.2.9/playground/time_series/visibility_graph.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/__init__.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/__main__.py
+-rw-r--r--   0        0        0    30283 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/builders.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/cli.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/color.py
+-rw-r--r--   0        0        0    10046 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/modeling.py
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/typing.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/materializers/__init__.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/materializers/matplotlib.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/__init__.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/starlette/__init__.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/starlette/views.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/graphiql/__init__.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/graphiql/index.html
+-rw-r--r--   0        0        0    29055 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/static/images/logo-128.png
+-rw-r--r--   0        0        0    32663 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/static/images/network_graph.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/viewer/__init__.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/viewer/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/voyager/__init__.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/server/web/voyager/index.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/tools/__init__.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/tools/gui.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 graphinate-0.2.9/src/graphinate/tools/mutators.py
+-rw-r--r--   0        0        0     5216 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     9691 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_builders.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_cli.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_color.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_materializers.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_modeling.py
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_server.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 graphinate-0.2.9/tests/graphinate/test_tools.py
+-rw-r--r--   0        0        0    13926 2020-02-02 00:00:00.000000 graphinate-0.2.9/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 graphinate-0.2.9/LICENSE
+-rw-r--r--   0        0        0    11562 2020-02-02 00:00:00.000000 graphinate-0.2.9/README.md
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 graphinate-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    14190 2020-02-02 00:00:00.000000 graphinate-0.2.9/PKG-INFO
```

### Comparing `graphinate-0.2.8/mkdocs.yml` & `graphinate-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.github/workflows/codeql.yml` & `graphinate-0.2.9/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.github/workflows/publish-docs.yaml` & `graphinate-0.2.9/.github/workflows/publish-docs.yaml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.github/workflows/publish.yml` & `graphinate-0.2.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.github/workflows/test-beta.yml` & `graphinate-0.2.9/.github/workflows/test-beta.yml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.github/workflows/test.yml` & `graphinate-0.2.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/acknowledge.md` & `graphinate-0.2.9/docs/acknowledge.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/gen_ref_pages.py` & `graphinate-0.2.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/index.md` & `graphinate-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/intro.md` & `graphinate-0.2.9/docs/intro.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/start.md` & `graphinate-0.2.9/docs/start.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/assets/images/logo-128.png` & `graphinate-0.2.9/docs/assets/images/logo-128.png`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/assets/images/network_graph.png` & `graphinate-0.2.9/docs/assets/images/network_graph.png`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/examples/code.md` & `graphinate-0.2.9/docs/examples/code.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/examples/github.md` & `graphinate-0.2.9/docs/examples/github.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/usage/cli.md` & `graphinate-0.2.9/docs/usage/cli.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/docs/usage/lib.md` & `graphinate-0.2.9/docs/usage/lib.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/code/python_ast.py` & `graphinate-0.2.9/examples/code/python_ast.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/code/python_dependencies.py` & `graphinate-0.2.9/examples/code/python_dependencies.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/github/_client.py` & `graphinate-0.2.9/examples/github/_client.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/github/commits_visibilty_graph.py` & `graphinate-0.2.9/examples/github/commits_visibilty_graph.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/github/followers.py` & `graphinate-0.2.9/examples/github/followers.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/github/repositories.py` & `graphinate-0.2.9/examples/github/repositories.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/math/graph_atlas.py` & `graphinate-0.2.9/examples/math/graph_atlas.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/math/polygonal_graph.py` & `graphinate-0.2.9/examples/math/polygonal_graph.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/examples/web/page_links.py` & `graphinate-0.2.9/examples/web/page_links.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/playground/house_of_graphs.py` & `graphinate-0.2.9/playground/house_of_graphs.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/playground/social/albums.json` & `graphinate-0.2.9/playground/social/albums.json`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/playground/social/musicisians.py` & `graphinate-0.2.9/playground/social/musicisians.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/playground/time_series/visibility_graph.py` & `graphinate-0.2.9/playground/time_series/visibility_graph.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/builders.py` & `graphinate-0.2.9/src/graphinate/builders.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/cli.py` & `graphinate-0.2.9/src/graphinate/cli.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/color.py` & `graphinate-0.2.9/src/graphinate/color.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/modeling.py` & `graphinate-0.2.9/src/graphinate/modeling.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/typing.py` & `graphinate-0.2.9/src/graphinate/typing.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/materializers/__init__.py` & `graphinate-0.2.9/src/graphinate/materializers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     Args:
         model: GraphModel
         title: the GraphModel name
         graph_type: GraphType
         default_node_attributes:
         builder: Builder instance
         actualizer: function that will consume the resulting built graph and
-                    actualises it (e.g. display, serve, print etc.)
+                    actualises it (e.g., display, serves, print etc.)
         **kwargs:
 
     Returns:
         None
     """
     title = title or model.name
     if ENABLE_GUI and builder is None and actualizer is None:
```

### Comparing `graphinate-0.2.8/src/graphinate/materializers/matplotlib.py` & `graphinate-0.2.9/src/graphinate/materializers/matplotlib.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/__init__.py` & `graphinate-0.2.9/src/graphinate/server/__init__.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/starlette/__init__.py` & `graphinate-0.2.9/src/graphinate/server/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/web/graphiql/index.html` & `graphinate-0.2.9/src/graphinate/server/web/graphiql/index.html`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/web/static/images/logo-128.png` & `graphinate-0.2.9/src/graphinate/server/web/static/images/logo-128.png`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/web/static/images/network_graph.png` & `graphinate-0.2.9/src/graphinate/server/web/static/images/network_graph.png`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/web/viewer/index.html` & `graphinate-0.2.9/src/graphinate/server/web/viewer/index.html`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/server/web/voyager/index.html` & `graphinate-0.2.9/src/graphinate/server/web/voyager/index.html`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/tools/gui.py` & `graphinate-0.2.9/src/graphinate/tools/gui.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/src/graphinate/tools/mutators.py` & `graphinate-0.2.9/src/graphinate/tools/mutators.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/conftest.py` & `graphinate-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_builders.py` & `graphinate-0.2.9/tests/graphinate/test_builders.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_cli.py` & `graphinate-0.2.9/tests/graphinate/test_cli.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_color.py` & `graphinate-0.2.9/tests/graphinate/test_color.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_materializers.py` & `graphinate-0.2.9/tests/graphinate/test_materializers.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_modeling.py` & `graphinate-0.2.9/tests/graphinate/test_modeling.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_server.py` & `graphinate-0.2.9/tests/graphinate/test_server.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/tests/graphinate/test_tools.py` & `graphinate-0.2.9/tests/graphinate/test_tools.py`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/.gitignore` & `graphinate-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/LICENSE` & `graphinate-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/README.md` & `graphinate-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `graphinate-0.2.8/pyproject.toml` & `graphinate-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Graphinate"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
     { name = "Eran Rivlis", email = "eran@rivlis.info" },
 ]
 description = "Graphinate. Data to Graphs."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
@@ -29,15 +29,15 @@
 keywords = ['graph', 'declarative']
 dependencies = [
     "click==8.1.7",
     "inflect==7.0.0",
     "loguru==0.7.2",
     "matplotlib==3.8.2",
     "networkx==3.2.1",
-    "strawberry-graphql[asgi,opentelemetry]==0.215.1"
+    "strawberry-graphql[asgi,opentelemetry]==0.216.0"
 ]
 
 
 [project.urls]
 "Homepage" = "https://erivlis.github.io/graphinate"
 "Documentation" = "https://erivlis.github.io/graphinate"
 "Bug Tracker" = "https://github.com/erivlis/graphinate/issues"
```

### Comparing `graphinate-0.2.8/PKG-INFO` & `graphinate-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Graphinate
-Version: 0.2.8
+Version: 0.2.9
 Summary: Graphinate. Data to Graphs.
 Project-URL: Homepage, https://erivlis.github.io/graphinate
 Project-URL: Documentation, https://erivlis.github.io/graphinate
 Project-URL: Bug Tracker, https://github.com/erivlis/graphinate/issues
 Project-URL: Source, https://github.com/erivlis/graphinate
 Author-email: Eran Rivlis <eran@rivlis.info>
 License-File: LICENSE
@@ -28,15 +28,15 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Requires-Dist: click==8.1.7
 Requires-Dist: inflect==7.0.0
 Requires-Dist: loguru==0.7.2
 Requires-Dist: matplotlib==3.8.2
 Requires-Dist: networkx==3.2.1
-Requires-Dist: strawberry-graphql[asgi,opentelemetry]==0.215.1
+Requires-Dist: strawberry-graphql[asgi,opentelemetry]==0.216.0
 Provides-Extra: dev
 Requires-Dist: pipdeptree; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-gen-files; extra == 'docs'
 Requires-Dist: mkdocs-git-revision-date-localized-plugin; extra == 'docs'
 Requires-Dist: mkdocs-glightbox; extra == 'docs'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Graphinate Version: 0.2.8 Summary: Graphinate. Data
+Metadata-Version: 2.1 Name: Graphinate Version: 0.2.9 Summary: Graphinate. Data
 to Graphs. Project-URL: Homepage, https://erivlis.github.io/graphinate Project-
 URL: Documentation, https://erivlis.github.io/graphinate Project-URL: Bug
 Tracker, https://github.com/erivlis/graphinate/issues Project-URL: Source,
 https://github.com/erivlis/graphinate Author-email: Eran Rivlis
 rivlis.info> License-File: LICENSE Keywords: declarative,graph Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
@@ -14,15 +14,15 @@
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: Programming
 Language :: Python :: Implementation :: CPython Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed Requires-Python: >=3.9 Requires-Dist: click==8.1.7
 Requires-Dist: inflect==7.0.0 Requires-Dist: loguru==0.7.2 Requires-Dist:
 matplotlib==3.8.2 Requires-Dist: networkx==3.2.1 Requires-Dist: strawberry-
-graphql[asgi,opentelemetry]==0.215.1 Provides-Extra: dev Requires-Dist:
+graphql[asgi,opentelemetry]==0.216.0 Provides-Extra: dev Requires-Dist:
 pipdeptree; extra == 'dev' Requires-Dist: ruff; extra == 'dev' Provides-Extra:
 docs Requires-Dist: mkdocs-gen-files; extra == 'docs' Requires-Dist: mkdocs-
 git-revision-date-localized-plugin; extra == 'docs' Requires-Dist: mkdocs-
 glightbox; extra == 'docs' Requires-Dist: mkdocs-literate-nav; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs' Requires-Dist: mkdocs-section-
 index; extra == 'docs' Requires-Dist: mkdocstrings-python; extra == 'docs'
 Provides-Extra: plot Requires-Dist: scipy>=1.11.4; extra == 'plot' Provides-
```

