# Comparing `tmp/nbprint-0.1.5.tar.gz` & `tmp/nbprint-0.1.6.tar.gz`

## Comparing `nbprint-0.1.5.tar` & `nbprint-0.1.6.tar`

### file list

```diff
@@ -1,96 +1,94 @@
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/.eslintrc.js
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/build.mjs
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/package.json
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/playwright.config.js
--rw-r--r--   0        0        0    55380 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/yarn.lock
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/css/embedded.css
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/css/table-of-content.css
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/js/embedded.js
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/js/index.js
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/js/nbconvert.js
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/js/nbprint.js
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/js/components/table-of-content.js
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/src/less/index.less
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbprint-0.1.5/js/tests/index.spec.js
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/__main__.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/cli.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/__init__.py
--rw-r--r--   0        0        0    11247 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/base.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/__init__.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/border.py
--rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/common.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/css.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/display.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/spacing.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/style.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/common/text.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/__init__.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/base.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/common.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/cover.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/image.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/page.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/pagebreak.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/content/table_of_contents.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/__init__.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/config.py
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/context.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/exceptions.py
--rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/outputs.py
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/core/parameters.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/page/__init__.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/page/base.py
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/page/global_.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/config/page/page_number.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/__init__.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/__init__.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/code.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/context.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/cover.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/markdown.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/basic/parameters.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/finance/__init__.py
--rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/finance/content.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/finance/context.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/finance/parameters.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/research/__init__.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/research/content.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/example/research/context.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/embedded.css
--rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/embedded.js
--rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/embedded.js.map
--rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/fontawesome.min.css
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/index.css
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/index.js
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/index.js.map
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/extension/table-of-content.css
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/conf.json
--rw-r--r--   0        0        0     3590 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/index.html.j2
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.css
--rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.js
--rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.js.map
--rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/fontawesome.min.css
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/index.js
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/index.js.map
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/nbprint.css
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/templates/nbprint/static/table-of-content.css
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/tests/test_all.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/tests/test_e2e.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/tests/config/common/test_styles.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/utils/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/utils/format.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/utils/image.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/utils/ipython.py
--rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/base.html.j2
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/browser-open.html
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/error.html
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/index.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/mathjax.html.j2
--rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/mermaidjs.html.j2
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 nbprint-0.1.5/nbprint/voila/page.html
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nbprint-0.1.5/.gitignore
--rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nbprint-0.1.5/LICENSE
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 nbprint-0.1.5/README.md
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 nbprint-0.1.5/pyproject.toml
--rw-r--r--   0        0        0    22565 2020-02-02 00:00:00.000000 nbprint-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/.eslintrc.js
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/build.mjs
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/package.json
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/playwright.config.js
+-rw-r--r--   0        0        0    55380 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/yarn.lock
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/css/embedded.css
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/css/table-of-content.css
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/embedded.js
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/index.js
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/nbconvert.js
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/nbprint.js
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/js/components/table-of-content.js
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/src/less/index.less
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbprint-0.1.6/js/tests/index.spec.js
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/__main__.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/cli.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/__init__.py
+-rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/base.py
+-rw-r--r--   0        0        0     6032 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/page.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/border.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/common.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/css.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/display.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/spacing.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/style.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/common/text.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/__init__.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/base.py
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/common.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/cover.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/image.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/page.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/pagebreak.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/content/table_of_contents.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/__init__.py
+-rw-r--r--   0        0        0     6737 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/config.py
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/context.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/exceptions.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/outputs.py
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/config/core/parameters.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/__init__.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/__init__.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/code.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/context.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/cover.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/markdown.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/page.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/basic/parameters.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/__init__.py
+-rw-r--r--   0        0        0     8129 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/content.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/context.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/finance/parameters.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/__init__.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/content.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/example/research/context.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.css
+-rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.js
+-rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/embedded.js.map
+-rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/fontawesome.min.css
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.css
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.js
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/index.js.map
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/extension/table-of-content.css
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/conf.json
+-rw-r--r--   0        0        0     3599 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/index.html.j2
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.css
+-rw-r--r--   0        0        0  2006689 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js
+-rw-r--r--   0        0        0  3302746 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js.map
+-rw-r--r--   0        0        0    80795 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/fontawesome.min.css
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/index.js
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/index.js.map
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/nbprint.css
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/templates/nbprint/static/table-of-content.css
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/test_all.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/test_e2e.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/tests/config/common/test_styles.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/format.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/image.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/utils/ipython.py
+-rw-r--r--   0        0        0     9842 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/base.html.j2
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/browser-open.html
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/error.html
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/index.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/mathjax.html.j2
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/mermaidjs.html.j2
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 nbprint-0.1.6/nbprint/voila/page.html
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 nbprint-0.1.6/.gitignore
+-rw-r--r--   0        0        0    11349 2020-02-02 00:00:00.000000 nbprint-0.1.6/LICENSE
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 nbprint-0.1.6/README.md
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 nbprint-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 nbprint-0.1.6/PKG-INFO
```

### Comparing `nbprint-0.1.5/js/.eslintrc.js` & `nbprint-0.1.6/js/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/build.mjs` & `nbprint-0.1.6/js/build.mjs`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/package.json` & `nbprint-0.1.6/js/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9583333333333334%*

 * *Differences: {"'version'": "'0.1.6'"}*

```diff
@@ -33,9 +33,9 @@
         "lint": "prettier --check \"src/js/*.js\" \"src/less/*.less\" \"tests/*.spec.js\" \"*.js\" \"*.json\"",
         "prepack": "npm run build",
         "start:examples": "http-server -p 3000 -o examples/",
         "start:tests": "http-server -p 3000 ",
         "test": "TZ=UTC playwright test"
     },
     "types": "index.d.ts",
-    "version": "0.1.5"
+    "version": "0.1.6"
 }
```

### Comparing `nbprint-0.1.5/js/playwright.config.js` & `nbprint-0.1.6/js/playwright.config.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/yarn.lock` & `nbprint-0.1.6/js/yarn.lock`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/css/embedded.css` & `nbprint-0.1.6/js/src/css/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/css/table-of-content.css` & `nbprint-0.1.6/js/src/css/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/js/embedded.js` & `nbprint-0.1.6/js/src/js/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/js/nbconvert.js` & `nbprint-0.1.6/js/src/js/nbconvert.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/js/nbprint.js` & `nbprint-0.1.6/js/src/js/nbprint.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/js/components/table-of-content.js` & `nbprint-0.1.6/js/src/js/components/table-of-content.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/js/src/less/index.less` & `nbprint-0.1.6/js/src/less/index.less`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/base.py` & `nbprint-0.1.6/nbprint/config/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 class _SerializeAsAnyMeta(ModelMetaclass):
     def __new__(self, name: str, bases: Tuple[type], namespaces: Dict[str, Any], **kwargs):
         annotations: dict = namespaces.get("__annotations__", {}).copy()
         for field, annotation in annotations.items():
             if not field.startswith("__"):
                 annotations[field] = SerializeAsAny[annotation]
         namespaces["__annotations__"] = annotations
-        return super().__new__(self, name, bases, namespaces, **kwargs)
+        clz = super().__new__(self, name, bases, namespaces, **kwargs)
+        return clz
 
 
 class Type(BaseModel):
     module: str
     name: str
 
     @classmethod
     def from_string(cls, str: str) -> "Type":
-        module, name = str.split(":")
+        module, name = str.rsplit(".", 1)
         return Type(module=module, name=name)
 
     def to_string(self) -> str:
         return f"{self.module}:{self.name}"
 
     def type(self) -> Type["Type"]:
         return getattr(import_module(self.module), self.name)
@@ -62,15 +63,15 @@
     CONTENT = "content"
     PAGE = "page"
     LAYOUT = "layout"
 
 
 class BaseModel(BaseModel, metaclass=_SerializeAsAnyMeta):
     # type info
-    type: Type
+    type: Type = Field(alias="_target_")
 
     # basic metadata
     tags: List[str] = Field(default_factory=list)
     role: Role = Role.UNDEFINED
     ignore: bool = False
 
     # frontend code
@@ -89,16 +90,16 @@
 
     class Config:
         arbitrary_types_allowed: bool = False
         extra: str = "ignore"
         validate_assignment: bool = True
 
     def __init__(self, **kwargs):
-        if "type" not in kwargs:
-            kwargs["type"] = Type(module=self.__class__.__module__, name=self.__class__.__name__)
+        if "_target_" not in kwargs:
+            kwargs["_target_"] = Type(module=self.__class__.__module__, name=self.__class__.__name__)
         super().__init__(**kwargs)
 
     @validator("css", pre=True)
     def convert_css_string_or_path_to_string_or_path(cls, v):
         if isinstance(v, str):
             if v.strip().endswith(".css"):
                 # TODO resolve relative to class?
@@ -141,15 +142,15 @@
         nb_vars.add(self._nb_var_name)
 
     @staticmethod
     def _to_type(value, model_type=None):
         if value is None:
             value = {}
 
-        if model_type is None and "type" in value:
+        if model_type is None and "_target_" in value:
             # derive type from instantiation
             model_type = BaseModel
 
         if isinstance(value, dict):
             return model_type(**value).type.load(**value)
 
         return value
@@ -203,17 +204,17 @@
         )
         cell.metadata.nbprint.attrs = " ".join(f"{k}={dumps(v)}" for k, v in (self.attrs or {}).items())
 
     def _base_generate_meta(self, metadata: dict = None) -> Optional[NotebookNode]:
         cell = new_code_cell(metadata=metadata)
         cell.metadata.tags = list(set(["nbprint"] + (self.tags or [])))
 
-        # TODO consolidate with self.json()?
+        # TODO consolidate with self.model_dump_json(by_alias=True)?
         self._base_set_nbprint_metadata(cell)
-        cell.metadata.nbprint.data = self.json()
+        cell.metadata.nbprint.data = self.model_dump_json(by_alias=True)
         return cell
 
     def _base_generate_md_meta(self, metadata: dict = None) -> Optional[NotebookNode]:
         cell = new_markdown_cell(metadata=metadata)
         cell.metadata.tags = list(set(["nbprint"] + (self.tags or [])))
         self._base_set_nbprint_metadata(cell)
         return cell
@@ -251,15 +252,15 @@
                 ast.Assign(
                     targets=[ast.Name(id=self.nb_var_name, ctx=ast.Store())],
                     value=value,
                     lineno=1,
                 )
             )
         else:
-            data = self.json()
+            data = self.model_dump_json(by_alias=True)
             mod.body.append(
                 ast.ImportFrom(
                     module=self.type.module,
                     names=[ast.alias(name=self.type.name)],
                     level=0,
                 )
             )
```

### Comparing `nbprint-0.1.5/nbprint/config/common/border.py` & `nbprint-0.1.6/nbprint/config/common/border.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/common/common.py` & `nbprint-0.1.6/nbprint/config/common/common.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/common/display.py` & `nbprint-0.1.6/nbprint/config/common/display.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/common/spacing.py` & `nbprint-0.1.6/nbprint/config/common/spacing.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/common/style.py` & `nbprint-0.1.6/nbprint/config/common/style.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/common/text.py` & `nbprint-0.1.6/nbprint/config/common/text.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/content/base.py` & `nbprint-0.1.6/nbprint/config/content/base.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/content/common.py` & `nbprint-0.1.6/nbprint/config/content/common.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/content/image.py` & `nbprint-0.1.6/nbprint/config/content/image.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from IPython.display import Image, display
+from IPython.display import HTML, Image
 from pathlib import Path
 from pydantic import Field, FilePath, validator
 from typing import List, Optional
 
 from .base import Content
 
 
@@ -25,13 +25,14 @@
             v = Path(v).resolve()
         if v and isinstance(v, Path):
             v = v.read_bytes()
         return v
 
     def __call__(self, ctx=None, *args, **kwargs):
         if self.path:
-            display(Image(filename=self.path))
+            img = Image(filename=self.path)
         else:
-            display(Image(data=self.content))
+            img = Image(data=self.content)
+        return HTML(f"""<img src="data:image/png;base64,{img._repr_png_()}">""")
 
     def __repr__(self) -> str:
         return f"Image(path='{self.path}', content=[{len(self.content)} bytes])"
```

### Comparing `nbprint-0.1.5/nbprint/config/content/page.py` & `nbprint-0.1.6/nbprint/config/content/page.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/core/config.py` & `nbprint-0.1.6/nbprint/config/core/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+from hydra import compose, initialize_config_dir
+from hydra.utils import instantiate
 from nbformat import NotebookNode
 from nbformat.v4 import new_notebook
 from omegaconf import DictConfig, OmegaConf
 from pathlib import Path
 from pprint import pprint
 from pydantic import Field, PrivateAttr, validator
 from sys import version_info
 from typing import Dict, List, Union
 
 from ... import __version__
 from ..base import BaseModel, Role, Type, _append_or_extend
 from ..content import Content
-from ..page import PageGlobal
+from ..page import Page
 from .context import Context
 from .outputs import Outputs
 from .parameters import Parameters
 
 __all__ = (
     "Configuration",
     "load",
@@ -22,15 +24,15 @@
 
 
 class Configuration(BaseModel):
     name: str
     resources: Dict[str, BaseModel] = Field(default_factory=dict)
     outputs: Outputs
     parameters: Parameters = Field(default_factory=Parameters)
-    page: PageGlobal = Field(default_factory=PageGlobal)
+    page: Page = Field(default_factory=Page)
     context: Context = Field(default_factory=Context)
     content: List[Content] = Field(default_factory=list)
 
     # basic metadata
     tags: List[str] = Field(default=["nbprint:config"])
     role: Role = Role.CONFIGURATION
     ignore: bool = True
@@ -55,15 +57,15 @@
 
     @validator("parameters", pre=True)
     def convert_parameters_from_obj(cls, v):
         return BaseModel._to_type(v, Parameters)
 
     @validator("page", pre=True)
     def convert_page_from_obj(cls, v):
-        return BaseModel._to_type(v, PageGlobal)
+        return BaseModel._to_type(v, Page)
 
     @validator("context", pre=True)
     def convert_context_from_obj(cls, v):
         return BaseModel._to_type(v, Context)
 
     @validator("content", pre=True)
     def convert_content_from_obj(cls, v):
@@ -104,15 +106,15 @@
         # pass in parent=self, attr=context so we do config.context
         _append_or_extend(
             nb.cells, self.context.generate(metadata=base_meta.copy(), config=self, parent=self, attr="context")
         )
 
         # resources: Dict[str, SerializeAsAny[BaseModel]] = Field(default_factory=dict)
         # TODO omitting resources, referenced directly in yaml
-        # cell.metadata.nbprint.resources = {k: v.json() for k, v in self.resources.items()}
+        # cell.metadata.nbprint.resources = {k: v.model_dump_json(by_alias=True) for k, v in self.resources.items()}
 
         # outputs: SerializeAsAny[Outputs]
         # TODO skipping, consumed internally
 
         # now setup the page layout
         # pass in parent=self, attr=page so we do config.page
         _append_or_extend(
@@ -135,16 +137,16 @@
         cell.metadata.nbprint.data = ""
 
         # add extras
         cell.metadata.nbprint.debug = self.debug
 
         # add resources
         # TODO do this or no?
-        # cell.metadata.nbprint.resources = {k: v.json() for k, v in self.resources.items()}
-        cell.metadata.nbprint.outputs = self.outputs.json()
+        # cell.metadata.nbprint.resources = {k: v.model_dump_json(by_alias=True) for k, v in self.resources.items()}
+        cell.metadata.nbprint.outputs = self.outputs.model_dump_json(by_alias=True)
         return cell
 
     def _generate_resources_cells(self, metadata: dict = None):
         cell = super()._base_generate(metadata=metadata, config=None)
 
         # omit the data
         cell.metadata.nbprint.data = ""
@@ -169,14 +171,21 @@
 
         if isinstance(path_or_model, DictConfig):
             container = OmegaConf.to_container(path_or_model, resolve=True, throw_on_missing=True)
             return Configuration(name=name, **container)
 
         raise TypeError(f"Path or model malformed: {path_or_model} {type(path_or_model)}")
 
+    @staticmethod
+    def load_hydra(folder, file, name):
+        with initialize_config_dir(version_base=None, config_dir=folder, job_name=name):
+            cfg = compose(config_name=file, overrides=[f"+name={name}"])
+            config = instantiate(cfg)
+            return config
+
     def run(self):
         gen = self.generate(self)
         if self.debug:
             pprint(gen)
         self.outputs.run(self, gen)
```

### Comparing `nbprint-0.1.5/nbprint/config/core/context.py` & `nbprint-0.1.6/nbprint/config/core/context.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/config/core/outputs.py` & `nbprint-0.1.6/nbprint/config/core/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
     def _get_uuid(self, config: "Configuration") -> str:
         return uuid4()
 
     def _get_sha(self, config: "Configuration") -> str:
         import hashlib
 
-        m = hashlib.sha256(config.json())
+        m = hashlib.sha256(config.model_dump_json(by_alias=True))
         m.update(config)
         return m.hexdigest()
 
     def run(self, config: "Configuration", gen: NotebookNode) -> Path:
         # create file or folder path
         file = str(
             Path(self.path_root).resolve()
```

### Comparing `nbprint-0.1.5/nbprint/config/core/parameters.py` & `nbprint-0.1.6/nbprint/config/core/parameters.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/example/basic/markdown.py` & `nbprint-0.1.6/nbprint/example/basic/markdown.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from IPython.display import Markdown
 
 from nbprint import Content
 
+__all__ = ("ExampleMarkdownBlock",)
+
 
 class ExampleMarkdownBlock(Content):
     def __call__(self, ctx=None, *args, **kwargs):
         return Markdown(
             """# Performance
 Now some discussion of the performance, as well as some charts
 Lorem ipsum dolor sit amet, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
```

### Comparing `nbprint-0.1.5/nbprint/example/finance/content.py` & `nbprint-0.1.6/nbprint/example/finance/content.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/example/research/content.py` & `nbprint-0.1.6/nbprint/example/research/content.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/embedded.css` & `nbprint-0.1.6/nbprint/extension/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/embedded.js` & `nbprint-0.1.6/nbprint/extension/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/embedded.js.map` & `nbprint-0.1.6/nbprint/extension/embedded.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/fontawesome.min.css` & `nbprint-0.1.6/nbprint/extension/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/index.css` & `nbprint-0.1.6/nbprint/extension/index.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/index.js` & `nbprint-0.1.6/nbprint/extension/index.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/index.js.map` & `nbprint-0.1.6/nbprint/extension/index.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/extension/table-of-content.css` & `nbprint-0.1.6/nbprint/extension/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/index.html.j2` & `nbprint-0.1.6/nbprint/templates/nbprint/index.html.j2`

 * *Files 6% similar despite different names*

```diff
@@ -87,17 +87,17 @@
 
     {% if cell.metadata["nbprint"].get("ignore", False) %}
         {# Don't generate any visual elements if nbprint_ignore tag is set #}
     {% else %}
         <div class="{{ cell.metadata["nbprint"]["class"] }}" {{ cell.metadata["nbprint"]["attrs"] }} data-nbprint-id="{{ cell.metadata["nbprint"]["id"] }}" data-nbprint-parent-id="{{ cell.metadata["nbprint"].get("parent-id", "") }}">
 
         <!-- TODO should we make this like `ignore` as a first-order attribute? -->
-        {% if cell.metadata["nbprint"].get("role", "content") == "content" %}
+        <!-- if cell.metadata["nbprint"].get("role", "content") == "content" %} -->
         {{ super() }}
-        {% endif %}
+        <!-- endif -->
 
         </div>
     {% endif %}
 {% else %}
     {{ super() }}
 {% endif %}
 {% endblock any_cell %}
```

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.css` & `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.js` & `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/embedded.js.map` & `nbprint-0.1.6/nbprint/templates/nbprint/static/embedded.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/fontawesome.min.css` & `nbprint-0.1.6/nbprint/templates/nbprint/static/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/index.js` & `nbprint-0.1.6/nbprint/templates/nbprint/static/index.js`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/index.js.map` & `nbprint-0.1.6/nbprint/templates/nbprint/static/index.js.map`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/nbprint.css` & `nbprint-0.1.6/nbprint/templates/nbprint/static/nbprint.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/templates/nbprint/static/table-of-content.css` & `nbprint-0.1.6/nbprint/templates/nbprint/static/table-of-content.css`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/tests/test_e2e.py` & `nbprint-0.1.6/nbprint/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/tests/config/common/test_styles.py` & `nbprint-0.1.6/nbprint/tests/config/common/test_styles.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/utils/format.py` & `nbprint-0.1.6/nbprint/utils/format.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/utils/image.py` & `nbprint-0.1.6/nbprint/utils/image.py`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/voila/base.html.j2` & `nbprint-0.1.6/nbprint/voila/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/voila/browser-open.html` & `nbprint-0.1.6/nbprint/voila/browser-open.html`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/voila/index.html.j2` & `nbprint-0.1.6/nbprint/voila/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/voila/mathjax.html.j2` & `nbprint-0.1.6/nbprint/voila/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/nbprint/voila/mermaidjs.html.j2` & `nbprint-0.1.6/nbprint/voila/mermaidjs.html.j2`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/.gitignore` & `nbprint-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/LICENSE` & `nbprint-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/README.md` & `nbprint-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nbprint-0.1.5/pyproject.toml` & `nbprint-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "jupyterlab>=4,<5",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "nbprint"
 description = "A framework for customizing NBConvert templates and building reports"
-version = "0.1.5"
+version = "0.1.6"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
 authors = [
     { name = "Tim Paine", email = "t.paine154@gmail.com" },
 ]
 keywords = [
@@ -48,34 +48,41 @@
     "pydantic>=2,<3",
     "pydantic_extra_types",
     "strenum",
     "typer",
 ]
 
 [project.optional-dependencies]
+hydra = [
+    "hydra-core",
+]
 develop = [
     "check-manifest",
     "isort>=5,<6",
     "ruff>=0.3,<0.4",
+    # test
     "pytest",
     "pytest-cov",
+    # hydra
+    "hydra-core",
     # notebook deps
     "matplotlib",
     "pandas",
     "perspective-python",
     "seaborn",
     "superstore",
 ]
 test = [
     "pytest",
     "pytest-cov",
 ]
 
 [project.scripts]
 nbprint = "nbprint.cli:main"
+nbprint-hydra = "nbprint.cli:main_hydra"
 
 [project.urls]
 repository = "https://github.com/timkpaine/nbprint"
 homepage = "https://github.com/timkpaine/nbprint"
 
 [tool.hatch.build]
 artifacts = [
```

### Comparing `nbprint-0.1.5/PKG-INFO` & `nbprint-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nbprint
-Version: 0.1.5
+Version: 0.1.6
 Summary: A framework for customizing NBConvert templates and building reports
 Project-URL: repository, https://github.com/timkpaine/nbprint
 Project-URL: homepage, https://github.com/timkpaine/nbprint
 Author-email: Tim Paine <t.paine154@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -227,23 +227,26 @@
 Requires-Dist: omegaconf
 Requires-Dist: pydantic-extra-types
 Requires-Dist: pydantic<3,>=2
 Requires-Dist: strenum
 Requires-Dist: typer
 Provides-Extra: develop
 Requires-Dist: check-manifest; extra == 'develop'
+Requires-Dist: hydra-core; extra == 'develop'
 Requires-Dist: isort<6,>=5; extra == 'develop'
 Requires-Dist: matplotlib; extra == 'develop'
 Requires-Dist: pandas; extra == 'develop'
 Requires-Dist: perspective-python; extra == 'develop'
 Requires-Dist: pytest; extra == 'develop'
 Requires-Dist: pytest-cov; extra == 'develop'
 Requires-Dist: ruff<0.4,>=0.3; extra == 'develop'
 Requires-Dist: seaborn; extra == 'develop'
 Requires-Dist: superstore; extra == 'develop'
+Provides-Extra: hydra
+Requires-Dist: hydra-core; extra == 'hydra'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/timkpaine/nbprint#gh-light-mode-only">
   <img src="https://github.com/timkpaine/nbprint/raw/main/docs/img/logo-light.png?raw=true#gh-light-mode-only" alt="nbprint" width="400"></a>
```

