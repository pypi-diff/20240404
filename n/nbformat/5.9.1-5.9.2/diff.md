# Comparing `tmp/nbformat-5.9.1.tar.gz` & `tmp/nbformat-5.9.2.tar.gz`

## Comparing `nbformat-5.9.1.tar` & `nbformat-5.9.2.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbformat-5.9.1/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbformat-5.9.1/.mailmap
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 nbformat-5.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nbformat-5.9.1/.readthedocs.yaml
--rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 nbformat-5.9.1/CHANGELOG.md
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 nbformat-5.9.1/README.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nbformat-5.9.1/RELEASING.md
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbformat-5.9.1/index.js
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 nbformat-5.9.1/package.json
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/dependabot.yml
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/scripts/create_npmrc.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/scripts/parse_ref.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4902 2020-02-02 00:00:00.000000 nbformat-5.9.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/Makefile
--rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/api.rst
--rw-r--r--   0        0        0    10122 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/conf.py
--rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/format_description.rst
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/index.rst
--rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/make.bat
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 nbformat-5.9.1/docs/markup.rst
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/_imports.py
--rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/_struct.py
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/_version.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/converter.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/current.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/json_compat.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/notebooknode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/py.typed
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/reader.py
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/sentinel.py
--rw-r--r--   0        0        0    21475 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/sign.py
--rw-r--r--   0        0        0    22578 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/validator.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/warnings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/corpus/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/corpus/words.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/corpus/tests/__init__.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/corpus/tests/test_words.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v1/__init__.py
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v1/convert.py
--rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v1/nbbase.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v1/nbjson.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v1/rwbase.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/__init__.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/convert.py
--rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/nbbase.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/nbjson.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/nbpy.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/nbxml.py
--rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v2/rwbase.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/__init__.py
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/convert.py
--rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/nbbase.py
--rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/nbformat.v3.schema.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/nbjson.py
--rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/nbpy.py
--rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v3/rwbase.py
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/__init__.py
--rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/convert.py
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbbase.py
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.0.schema.json
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.1.schema.json
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.2.schema.json
--rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.3.schema.json
--rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.4.schema.json
--rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.5.schema.json
--rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbformat.v4.schema.json
--rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/nbjson.py
--rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 nbformat-5.9.1/nbformat/v4/rwbase.py
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 nbformat-5.9.1/scripts/jupyter-trust
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/base.py
--rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/invalid.ipynb
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/invalid_cell_id.ipynb
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/invalid_unique_cell_id.ipynb
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/many_tracebacks.ipynb
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/no_min_version.ipynb
--rw-r--r--   0        0        0    46130 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test2.ipynb
--rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test3.ipynb
--rw-r--r--   0        0        0    15843 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test3_no_metadata.ipynb
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test3_no_min_version.ipynb
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test3_no_worksheets.ipynb
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test3_worksheet_with_no_cells.ipynb
--rw-r--r--   0        0        0    16074 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4.5.ipynb
--rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4.ipynb
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4custom.ipynb
--rw-r--r--   0        0        0    17485 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4docinfo.ipynb
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4jupyter_metadata.ipynb
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4jupyter_metadata_timings.ipynb
--rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test4plus.ipynb
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_api.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_convert.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_nbformat.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_reader.py
--rw-r--r--   0        0        0     9318 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_sign.py
--rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/test_validator.py
--rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4_5_invalid_metadata.ipynb
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4_5_no_cell_id.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v1/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v1/nbexamples.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v1/test_json.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v1/test_nbbase.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v2/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v2/nbexamples.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v2/test_json.py
--rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v2/test_nbbase.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v2/test_nbpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/formattest.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/nbexamples.py
--rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/test_json.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/test_misc.py
--rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/test_nbbase.py
--rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v3/test_nbpy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/__init__.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/formattest.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/nbexamples.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/test_convert.py
--rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/test_json.py
--rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/test_nbbase.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 nbformat-5.9.1/tests/v4/test_validate.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbformat-5.9.1/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbformat-5.9.1/LICENSE
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 nbformat-5.9.1/pyproject.toml
--rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 nbformat-5.9.1/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbformat-5.9.2/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbformat-5.9.2/.mailmap
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 nbformat-5.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nbformat-5.9.2/.readthedocs.yaml
+-rw-r--r--   0        0        0    16063 2020-02-02 00:00:00.000000 nbformat-5.9.2/CHANGELOG.md
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2303 2020-02-02 00:00:00.000000 nbformat-5.9.2/README.md
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 nbformat-5.9.2/RELEASING.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbformat-5.9.2/index.js
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 nbformat-5.9.2/package.json
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/scripts/create_npmrc.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/scripts/parse_ref.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 nbformat-5.9.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7417 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/Makefile
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/api.rst
+-rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/conf.py
+-rw-r--r--   0        0        0    15210 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/format_description.rst
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/index.rst
+-rw-r--r--   0        0        0     7248 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/make.bat
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 nbformat-5.9.2/docs/markup.rst
+-rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/_imports.py
+-rw-r--r--   0        0        0    11260 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/_struct.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/_version.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/converter.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/current.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/json_compat.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/notebooknode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/py.typed
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/reader.py
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/sentinel.py
+-rw-r--r--   0        0        0    21476 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/sign.py
+-rw-r--r--   0        0        0    22596 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/validator.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/warnings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/corpus/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/corpus/words.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/corpus/tests/__init__.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/corpus/tests/test_words.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v1/__init__.py
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v1/convert.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v1/nbbase.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v1/nbjson.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v1/rwbase.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/__init__.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/convert.py
+-rw-r--r--   0        0        0     5551 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/nbbase.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/nbjson.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/nbpy.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/nbxml.py
+-rw-r--r--   0        0        0     5829 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v2/rwbase.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/__init__.py
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/convert.py
+-rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/nbbase.py
+-rw-r--r--   0        0        0    12198 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/nbformat.v3.schema.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/nbjson.py
+-rw-r--r--   0        0        0     7996 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/nbpy.py
+-rw-r--r--   0        0        0     6297 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v3/rwbase.py
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/__init__.py
+-rw-r--r--   0        0        0     9459 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/convert.py
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbbase.py
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.0.schema.json
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.1.schema.json
+-rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.2.schema.json
+-rw-r--r--   0        0        0    14000 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.3.schema.json
+-rw-r--r--   0        0        0    15703 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.4.schema.json
+-rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.5.schema.json
+-rw-r--r--   0        0        0    16104 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbformat.v4.schema.json
+-rw-r--r--   0        0        0     1963 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/nbjson.py
+-rw-r--r--   0        0        0     4258 2020-02-02 00:00:00.000000 nbformat-5.9.2/nbformat/v4/rwbase.py
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 nbformat-5.9.2/scripts/jupyter-trust
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/base.py
+-rw-r--r--   0        0        0    17365 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/invalid.ipynb
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/invalid_cell_id.ipynb
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/invalid_unique_cell_id.ipynb
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/many_tracebacks.ipynb
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/no_min_version.ipynb
+-rw-r--r--   0        0        0    46130 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test2.ipynb
+-rw-r--r--   0        0        0    15875 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test3.ipynb
+-rw-r--r--   0        0        0    15843 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test3_no_metadata.ipynb
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test3_no_min_version.ipynb
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test3_no_worksheets.ipynb
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test3_worksheet_with_no_cells.ipynb
+-rw-r--r--   0        0        0    16074 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4.5.ipynb
+-rw-r--r--   0        0        0    17400 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4.ipynb
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4custom.ipynb
+-rw-r--r--   0        0        0    17485 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4docinfo.ipynb
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4jupyter_metadata.ipynb
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4jupyter_metadata_timings.ipynb
+-rw-r--r--   0        0        0    18282 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test4plus.ipynb
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_api.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_convert.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_nbformat.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_reader.py
+-rw-r--r--   0        0        0     9336 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_sign.py
+-rw-r--r--   0        0        0    11973 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/test_validator.py
+-rw-r--r--   0        0        0     1400 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4_5_invalid_metadata.ipynb
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4_5_no_cell_id.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v1/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v1/nbexamples.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v1/test_json.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v1/test_nbbase.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v2/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v2/nbexamples.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v2/test_json.py
+-rw-r--r--   0        0        0     4324 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v2/test_nbbase.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v2/test_nbpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/formattest.py
+-rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/nbexamples.py
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/test_json.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/test_misc.py
+-rw-r--r--   0        0        0     6005 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/test_nbbase.py
+-rw-r--r--   0        0        0     1391 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v3/test_nbpy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/__init__.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/formattest.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/nbexamples.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/test_convert.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/test_json.py
+-rw-r--r--   0        0        0     3024 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/test_nbbase.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 nbformat-5.9.2/tests/v4/test_validate.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 nbformat-5.9.2/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbformat-5.9.2/LICENSE
+-rw-r--r--   0        0        0     5621 2020-02-02 00:00:00.000000 nbformat-5.9.2/pyproject.toml
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 nbformat-5.9.2/PKG-INFO
```

### Comparing `nbformat-5.9.1/.mailmap` & `nbformat-5.9.2/.mailmap`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/.pre-commit-config.yaml` & `nbformat-5.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/CHANGELOG.md` & `nbformat-5.9.2/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,52 @@
 (changelog)=
 
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 5.9.2
+
+([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.9.1...80dd726ec87218e0b428a857b4cc656e7e9950d3))
+
+### Bugs fixed
+
+- Fix version handling [#372](https://github.com/jupyter/nbformat/pull/372) ([@blink1073](https://github.com/blink1073))
+
+### Maintenance and upkeep improvements
+
+- Fix encoding warnings [#371](https://github.com/jupyter/nbformat/pull/371) ([@blink1073](https://github.com/blink1073))
+- Update link to notebook security [#370](https://github.com/jupyter/nbformat/pull/370) ([@blink1073](https://github.com/blink1073))
+
+### Documentation improvements
+
+- Update link to notebook security [#370](https://github.com/jupyter/nbformat/pull/370) ([@blink1073](https://github.com/blink1073))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbformat/graphs/contributors?from=2023-07-10&to=2023-07-31&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Ablink1073+updated%3A2023-07-10..2023-07-31&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 5.9.1
 
 ([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.9.0...c348f9d12f05b4e0350413c74f58cd9e4f54a550))
 
 ### Maintenance and upkeep improvements
 
 - Fix deprecation warning when importing from jsonschema [#368](https://github.com/jupyter/nbformat/pull/368) ([@eladkal](https://github.com/eladkal))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbformat/graphs/contributors?from=2023-05-31&to=2023-07-10&type=c))
 
 [@eladkal](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Aeladkal+updated%3A2023-05-31..2023-07-10&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbformat+involves%3Apre-commit-ci+updated%3A2023-05-31..2023-07-10&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 5.9.0
 
 ([Full Changelog](https://github.com/jupyter/nbformat/compare/v5.8.0...1b5e8e4e9af98f9c9b0843ba155b8756103d094d))
 
 ### Maintenance and upkeep improvements
 
 - Support Python 3.12 [#363](https://github.com/jupyter/nbformat/pull/363) ([@blink1073](https://github.com/blink1073))
```

### Comparing `nbformat-5.9.1/CONTRIBUTING.md` & `nbformat-5.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/README.md` & `nbformat-5.9.2/README.md`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/RELEASING.md` & `nbformat-5.9.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/package.json` & `nbformat-5.9.2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'5.9.2'"}*

```diff
@@ -17,9 +17,9 @@
     "license": "BSD-3-Clause",
     "main": "index.js",
     "name": "nbformat-schema",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/jupyter/nbformat.git"
     },
-    "version": "5.9.1"
+    "version": "5.9.2"
 }
```

### Comparing `nbformat-5.9.1/.github/scripts/parse_ref.py` & `nbformat-5.9.2/.github/scripts/parse_ref.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/.github/workflows/prep-release.yml` & `nbformat-5.9.2/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/.github/workflows/publish-release.yml` & `nbformat-5.9.2/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/.github/workflows/tests.yml` & `nbformat-5.9.2/.github/workflows/tests.yml`

 * *Files 0% similar despite different names*

```diff
@@ -15,22 +15,22 @@
   tests:
     runs-on: ${{ matrix.os }}
     timeout-minutes: 20
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
-        python-version: ["3.8", "3.11"]
+        python-version: ["3.8", "3.12"]
         include:
           - os: windows-latest
             python-version: "3.9"
           - os: ubuntu-latest
             python-version: "pypy-3.8"
           - os: ubuntu-latest
-            python-version: "3.12.0-beta.1"
+            python-version: "3.11"
           - os: macos-latest
             python-version: "3.10"
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Run the tests
         if: ${{ !startsWith(matrix.python-version, 'pypy') && !startsWith(matrix.os, 'windows') }}
```

### Comparing `nbformat-5.9.1/docs/Makefile` & `nbformat-5.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/docs/api.rst` & `nbformat-5.9.2/docs/api.rst`

 * *Files 8% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 Notebook signatures
 -------------------
 
 .. module:: nbformat.sign
 
 This machinery is used by the notebook web application to record which notebooks
 are *trusted*, and may show dynamic output as soon as they're loaded. See
-:ref:`notebook:notebook_security` for more information.
+:ref:`server:server_security` for more information.
 
 .. autoclass:: NotebookNotary
 
    .. automethod:: sign
 
    .. automethod:: unsign
```

### Comparing `nbformat-5.9.1/docs/conf.py` & `nbformat-5.9.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,13 +300,14 @@
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
     "jupyterclient": ("https://jupyter-client.readthedocs.io/en/stable", None),
     "nbconvert": ("https://nbconvert.readthedocs.org/en/stable", None),
     "notebook": ("https://jupyter-notebook.readthedocs.org/en/stable", None),
+    "server": ("https://jupyter-server.readthedocs.org/en/stable", None),
 }
 
 
 def setup(_):
     dest = os.path.join(HERE, "changelog.md")
     shutil.copy(os.path.join(HERE, "..", "CHANGELOG.md"), dest)
```

### Comparing `nbformat-5.9.1/docs/format_description.rst` & `nbformat-5.9.2/docs/format_description.rst`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/docs/make.bat` & `nbformat-5.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/docs/markup.rst` & `nbformat-5.9.2/docs/markup.rst`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/__init__.py` & `nbformat-5.9.2/nbformat/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/_imports.py` & `nbformat-5.9.2/nbformat/_imports.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/_struct.py` & `nbformat-5.9.2/nbformat/_struct.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/_version.py` & `nbformat-5.9.2/nbformat/_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """The version information for nbformat."""
 # Use "hatchling version xx.yy.zz" to handle version changes
 import re
+from importlib.metadata import version
 
-try:
-    from importlib.metadata import version
-except ImportError:
-    from importlib_metadata import version  # type:ignore
-
-__version__ = version("nbformat")
+__version__ = version("nbformat") or "0.0.0"
 
 # matches tbump regex in pyproject.toml
 _version_regex = re.compile(
     r"""
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
```

### Comparing `nbformat-5.9.1/nbformat/converter.py` & `nbformat-5.9.2/nbformat/converter.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/current.py` & `nbformat-5.9.2/nbformat/current.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/json_compat.py` & `nbformat-5.9.2/nbformat/json_compat.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/notebooknode.py` & `nbformat-5.9.2/nbformat/notebooknode.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/reader.py` & `nbformat-5.9.2/nbformat/reader.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/sentinel.py` & `nbformat-5.9.2/nbformat/sentinel.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/sign.py` & `nbformat-5.9.2/nbformat/sign.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,15 +598,15 @@
         return NotebookNotary(parent=self, data_dir=self.data_dir)
 
     def sign_notebook_file(self, notebook_path):
         """Sign a notebook from the filesystem"""
         if not os.path.exists(notebook_path):
             self.log.error("Notebook missing: %s" % notebook_path)
             self.exit(1)
-        with open(notebook_path, encoding="utf8") as f:
+        with open(notebook_path, encoding="utf-8") as f:
             nb = read(f, NO_CONVERT)
         self.sign_notebook(nb, notebook_path)
 
     def sign_notebook(self, nb, notebook_path="<stdin>"):
         """Sign a notebook that's been loaded"""
         if self.notary.check_signature(nb):
             print("Notebook already signed: %s" % notebook_path)  # noqa
```

### Comparing `nbformat-5.9.1/nbformat/validator.py` & `nbformat-5.9.2/nbformat/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         )
     elif version_minor > v.nbformat_minor:
         # load the latest schema
         schema_path = os.path.join(os.path.dirname(v.__file__), v.nbformat_schema[(None, None)])
     else:
         msg = "Cannot find appropriate nbformat schema file."
         raise AttributeError(msg)
-    with open(schema_path) as f:
+    with open(schema_path, encoding='utf-8') as f:
         schema_json = json.load(f)
     return schema_json
 
 
 def isvalid(nbjson, ref=None, version=None, version_minor=None):
     """Checks whether the given notebook JSON conforms to the current
     notebook format schema. Returns True if the JSON is valid, and
```

### Comparing `nbformat-5.9.1/nbformat/warnings.py` & `nbformat-5.9.2/nbformat/warnings.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v1/__init__.py` & `nbformat-5.9.2/nbformat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v1/convert.py` & `nbformat-5.9.2/nbformat/v1/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v1/nbbase.py` & `nbformat-5.9.2/nbformat/v1/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v1/nbjson.py` & `nbformat-5.9.2/nbformat/v1/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v1/rwbase.py` & `nbformat-5.9.2/nbformat/v1/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/__init__.py` & `nbformat-5.9.2/nbformat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/convert.py` & `nbformat-5.9.2/nbformat/v2/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/nbbase.py` & `nbformat-5.9.2/nbformat/v2/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/nbjson.py` & `nbformat-5.9.2/nbformat/v2/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/nbpy.py` & `nbformat-5.9.2/nbformat/v2/nbpy.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/nbxml.py` & `nbformat-5.9.2/nbformat/v2/nbxml.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v2/rwbase.py` & `nbformat-5.9.2/nbformat/v2/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/__init__.py` & `nbformat-5.9.2/nbformat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/convert.py` & `nbformat-5.9.2/nbformat/v3/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/nbbase.py` & `nbformat-5.9.2/nbformat/v3/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/nbformat.v3.schema.json` & `nbformat-5.9.2/nbformat/v3/nbformat.v3.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/nbjson.py` & `nbformat-5.9.2/nbformat/v3/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/nbpy.py` & `nbformat-5.9.2/nbformat/v3/nbpy.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v3/rwbase.py` & `nbformat-5.9.2/nbformat/v3/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/__init__.py` & `nbformat-5.9.2/nbformat/v4/__init__.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/convert.py` & `nbformat-5.9.2/nbformat/v4/convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbbase.py` & `nbformat-5.9.2/nbformat/v4/nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.0.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.0.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.1.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.1.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.2.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.2.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.3.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.3.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.4.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.4.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.5.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.5.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbformat.v4.schema.json` & `nbformat-5.9.2/nbformat/v4/nbformat.v4.schema.json`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/nbjson.py` & `nbformat-5.9.2/nbformat/v4/nbjson.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/nbformat/v4/rwbase.py` & `nbformat-5.9.2/nbformat/v4/rwbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/invalid.ipynb` & `nbformat-5.9.2/tests/invalid.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/invalid_cell_id.ipynb` & `nbformat-5.9.2/tests/invalid_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/invalid_unique_cell_id.ipynb` & `nbformat-5.9.2/tests/invalid_unique_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/many_tracebacks.ipynb` & `nbformat-5.9.2/tests/many_tracebacks.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test2.ipynb` & `nbformat-5.9.2/tests/test2.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test3.ipynb` & `nbformat-5.9.2/tests/test3.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test3_no_metadata.ipynb` & `nbformat-5.9.2/tests/test3_no_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4.5.ipynb` & `nbformat-5.9.2/tests/test4.5.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4.ipynb` & `nbformat-5.9.2/tests/test4.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4custom.ipynb` & `nbformat-5.9.2/tests/test4custom.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4docinfo.ipynb` & `nbformat-5.9.2/tests/test4docinfo.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4jupyter_metadata_timings.ipynb` & `nbformat-5.9.2/tests/test4jupyter_metadata_timings.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test4plus.ipynb` & `nbformat-5.9.2/tests/test4plus.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test_api.py` & `nbformat-5.9.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test_convert.py` & `nbformat-5.9.2/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test_nbformat.py` & `nbformat-5.9.2/tests/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test_reader.py` & `nbformat-5.9.2/tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/test_sign.py` & `nbformat-5.9.2/tests/test_sign.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     def tearDown(self):
         self.notary.store.close()
         shutil.rmtree(self.data_dir)
 
     def test_invalid_db_file(self):
         invalid_sql_file = os.path.join(self.data_dir, "invalid_db_file.db")
-        with open(invalid_sql_file, "w") as tempfile:
+        with open(invalid_sql_file, "w", encoding="utf-8") as tempfile:
             tempfile.write("[invalid data]")
 
         invalid_notary = sign.NotebookNotary(
             db_file=invalid_sql_file,
             secret=b"secret",
         )
         invalid_notary.sign(self.nb)
```

### Comparing `nbformat-5.9.1/tests/test_validator.py` & `nbformat-5.9.2/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4_5_invalid_metadata.ipynb` & `nbformat-5.9.2/tests/v4_5_invalid_metadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4_5_no_cell_id.ipynb` & `nbformat-5.9.2/tests/v4_5_no_cell_id.ipynb`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v1/test_nbbase.py` & `nbformat-5.9.2/tests/v1/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v2/nbexamples.py` & `nbformat-5.9.2/tests/v2/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v2/test_json.py` & `nbformat-5.9.2/tests/v2/test_json.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v2/test_nbbase.py` & `nbformat-5.9.2/tests/v2/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/formattest.py` & `nbformat-5.9.2/tests/v3/formattest.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/nbexamples.py` & `nbformat-5.9.2/tests/v3/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/test_json.py` & `nbformat-5.9.2/tests/v3/test_json.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/test_misc.py` & `nbformat-5.9.2/tests/v3/test_misc.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/test_nbbase.py` & `nbformat-5.9.2/tests/v3/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v3/test_nbpy.py` & `nbformat-5.9.2/tests/v3/test_nbpy.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4/formattest.py` & `nbformat-5.9.2/tests/v4/formattest.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4/nbexamples.py` & `nbformat-5.9.2/tests/v4/nbexamples.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4/test_convert.py` & `nbformat-5.9.2/tests/v4/test_convert.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4/test_json.py` & `nbformat-5.9.2/tests/v4/test_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,27 +104,32 @@
     def test_latest_schema_matches(self):
         """Test to ensure all schema is locked to a known version"""
         assert nbformat == 4
         assert nbformat_minor == 5
 
     def test_base_version_matches_latest(self):
         """Test to ensure latest version file matches latest verison"""
-        with open(os.path.join(BASE_PATH, "nbformat.v4.schema.json")) as schema_file:
+        with open(
+            os.path.join(BASE_PATH, "nbformat.v4.schema.json"), encoding='utf-8'
+        ) as schema_file:
             latest_schema = json.load(schema_file)
             with open(
                 os.path.join(
                     BASE_PATH,
                     "nbformat.v{major}.{minor}.schema.json".format(
                         major=nbformat, minor=nbformat_minor
                     ),
                 ),
+                encoding='utf-8',
             ) as schema_file:  # noqa
                 ver_schema = json.load(schema_file)
             assert latest_schema == ver_schema
 
     def test_latest_matches_nbformat(self):
         """Test to ensure that the nbformat version matches the description of the latest schema"""
-        with open(os.path.join(BASE_PATH, "nbformat.v4.schema.json")) as schema_file:
+        with open(
+            os.path.join(BASE_PATH, "nbformat.v4.schema.json"), encoding='utf-8'
+        ) as schema_file:
             schema = json.load(schema_file)
         assert schema["description"] == "Jupyter Notebook v{major}.{minor} JSON schema.".format(
             major=nbformat, minor=nbformat_minor
         )
```

### Comparing `nbformat-5.9.1/tests/v4/test_nbbase.py` & `nbformat-5.9.2/tests/v4/test_nbbase.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/tests/v4/test_validate.py` & `nbformat-5.9.2/tests/v4/test_validate.py`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/LICENSE` & `nbformat-5.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nbformat-5.9.1/pyproject.toml` & `nbformat-5.9.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 requires-python = ">=3.8"
 dependencies = [
     "fastjsonschema",
     "jsonschema>=2.6",
     "jupyter_core",
     "traitlets>=5.1"
@@ -64,15 +65,15 @@
 features = ["docs"]
 [tool.hatch.envs.docs.scripts]
 build = "make -C docs html SPHINXOPTS='-W'"
 
 [tool.hatch.envs.test]
 features = ["test"]
 [tool.hatch.envs.test.scripts]
-test = "python -m pytest -vv {args}"
+test = "PYTHONWARNDEFAULTENCODING=1 python -m pytest -vv {args}"
 nowarn = "test -W default {args}"
 
 [tool.hatch.envs.cov]
 features = ["test"]
 dependencies = ["coverage", "pytest-cov"]
 [tool.hatch.envs.cov.scripts]
 test = "python -m pytest -vv --cov nbformat --cov-branch --cov-report term-missing:skip-covered {args}"
@@ -147,19 +148,19 @@
     "testpath"
 ]
 ignore_missing_imports = true
 
 [tool.black]
 line-length = 100
 skip-string-normalization = true
-target-version = ["py37"]
+target-version = ["py38"]
 extend-exclude = "^/tests.*ipynb$"
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 100
 select = [
   "A", "B", "C", "DTZ", "E", "EM", "F", "FBT", "I", "ICN", "ISC", "N",
   "PLC", "PLE", "PLR", "PLW", "Q", "RUF", "S", "SIM", "T", "TID", "UP",
   "W", "YTT",
 ]
 ignore = [
```

### Comparing `nbformat-5.9.1/PKG-INFO` & `nbformat-5.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbformat
-Version: 5.9.1
+Version: 5.9.2
 Summary: The Jupyter Notebook format
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
@@ -43,14 +43,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Requires-Dist: fastjsonschema
 Requires-Dist: jsonschema>=2.6
 Requires-Dist: jupyter-core
 Requires-Dist: traitlets>=5.1
 Provides-Extra: docs
 Requires-Dist: myst-parser; extra == 'docs'
```

