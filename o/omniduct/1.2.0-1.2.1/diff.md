# Comparing `tmp/omniduct-1.2.0.tar.gz` & `tmp/omniduct-1.2.1.tar.gz`

## Comparing `omniduct-1.2.0.tar` & `omniduct-1.2.1.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 omniduct-1.2.0/MANIFEST.in
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/Makefile
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/conf.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/contributions.rst
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/deployment.rst
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/extensions.rst
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/index.rst
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/installation.rst
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/make.bat
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/protocols.rst
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/python_deps.txt
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/quickstart.rst
--rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/core.rst
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/overview.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/registry.rst
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/caches/overview.rst
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/caches/reference/filesystem.rst
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/overview.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/druid.rst
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/hiveserver2.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/neo4j.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/presto.rst
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/pyspark.rst
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/databases/reference/sqlalchemy.rst
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/filesystems/overview.rst
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/filesystems/reference/local.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/filesystems/reference/s3.rst
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/filesystems/reference/webhdfs.rst
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/remotes/overview.rst
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/remotes/reference/ssh.rst
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 omniduct-1.2.0/docs/api/remotes/reference/ssh_paramiko.rst
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/MANIFEST.in
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/README.md
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/setup.py
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/example_wrapper/__init__.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/example_wrapper/_version.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/example_wrapper/services.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omniduct-1.2.0/example_wrapper/example_wrapper/services.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/__init__.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/_version.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/_version_info.py
--rw-r--r--   0        0        0    23338 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/duct.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/errors.py
--rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/logo.png
--rw-r--r--   0        0        0    53763 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/logo.svg
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/protocols.py
--rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/caches/__init__.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/caches/_serializers.py
--rw-r--r--   0        0        0    20690 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/caches/base.py
--rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/caches/filesystem.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/__init__.py
--rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/_cursor_formatters.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/_cursor_serializer.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/_namespaces.py
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/_pandas.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/_schemas.py
--rw-r--r--   0        0        0    41053 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/base.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/druid.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/exasol.py
--rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/hiveserver2.py
--rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/neo4j.py
--rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/presto.py
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/pyspark.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/sqlalchemy.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/databases/stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/__init__.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/_pyarrow_compat.py
--rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/_webhdfs_helpers.py
--rw-r--r--   0        0        0    35881 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/base.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/local.py
--rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/s3.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/stub.py
--rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/filesystems/webhdfs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/remotes/__init__.py
--rw-r--r--   0        0        0    16474 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/remotes/base.py
--rw-r--r--   0        0        0    21990 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/remotes/ssh.py
--rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/remotes/ssh_paramiko.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/remotes/stub.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/restful/__init__.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/restful/base.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/__init__.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/about.py
--rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/config.py
--rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/debug.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/decorators.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/dependencies.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/magics.py
--rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/ports.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/processes.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/proxies.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/storage.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omniduct-1.2.0/omniduct/utils/submodules.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 omniduct-1.2.0/tests/test_restful.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.0/tests/databases/__init__.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omniduct-1.2.0/tests/databases/test__namespaces.py
--rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 omniduct-1.2.0/tests/databases/test_base.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omniduct-1.2.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 omniduct-1.2.0/LICENSE
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 omniduct-1.2.0/README.md
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 omniduct-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 omniduct-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 omniduct-1.2.1/MANIFEST.in
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/Makefile
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/conf.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/contributions.rst
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/deployment.rst
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/extensions.rst
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/index.rst
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/installation.rst
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/make.bat
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/protocols.rst
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/python_deps.txt
+-rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/quickstart.rst
+-rw-r--r--   0        0        0     1206 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/core.rst
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/overview.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/registry.rst
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/caches/overview.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/caches/reference/filesystem.rst
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/overview.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/druid.rst
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/hiveserver2.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/neo4j.rst
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/presto.rst
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/pyspark.rst
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/databases/reference/sqlalchemy.rst
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/overview.rst
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/local.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/s3.rst
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/filesystems/reference/webhdfs.rst
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/overview.rst
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/reference/ssh.rst
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 omniduct-1.2.1/docs/api/remotes/reference/ssh_paramiko.rst
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/MANIFEST.in
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/README.md
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/setup.py
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/__init__.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/_version.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/services.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 omniduct-1.2.1/example_wrapper/example_wrapper/services.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/__init__.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/_version.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/_version_info.py
+-rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/duct.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/errors.py
+-rw-r--r--   0        0        0    21834 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/logo.png
+-rw-r--r--   0        0        0    53763 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/logo.svg
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/protocols.py
+-rw-r--r--   0        0        0    12051 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/__init__.py
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/_serializers.py
+-rw-r--r--   0        0        0    20694 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/base.py
+-rw-r--r--   0        0        0     4877 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/caches/filesystem.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/__init__.py
+-rw-r--r--   0        0        0     7224 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_cursor_formatters.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_cursor_serializer.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_namespaces.py
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_pandas.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/_schemas.py
+-rw-r--r--   0        0        0    41077 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/base.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/druid.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/exasol.py
+-rw-r--r--   0        0        0    24756 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/hiveserver2.py
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/neo4j.py
+-rw-r--r--   0        0        0    10230 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/presto.py
+-rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/pyspark.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/sqlalchemy.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/databases/stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/__init__.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/_pyarrow_compat.py
+-rw-r--r--   0        0        0     5375 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/_webhdfs_helpers.py
+-rw-r--r--   0        0        0    35915 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/base.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/local.py
+-rw-r--r--   0        0        0    10569 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/s3.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/stub.py
+-rw-r--r--   0        0        0     6238 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/filesystems/webhdfs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/__init__.py
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/base.py
+-rw-r--r--   0        0        0    21990 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/ssh.py
+-rw-r--r--   0        0        0     7871 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/ssh_paramiko.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/remotes/stub.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/restful/__init__.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/restful/base.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/__init__.py
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/about.py
+-rw-r--r--   0        0        0    12787 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/config.py
+-rw-r--r--   0        0        0    10670 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/debug.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/decorators.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/dependencies.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/magics.py
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/ports.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/processes.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/proxies.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/storage.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 omniduct-1.2.1/omniduct/utils/submodules.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/__init__.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/test_restful.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/test__namespaces.py
+-rw-r--r--   0        0        0     3399 2020-02-02 00:00:00.000000 omniduct-1.2.1/tests/databases/test_base.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 omniduct-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 omniduct-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 omniduct-1.2.1/README.md
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 omniduct-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 omniduct-1.2.1/PKG-INFO
```

### Comparing `omniduct-1.2.0/docs/Makefile` & `omniduct-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/conf.py` & `omniduct-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/deployment.rst` & `omniduct-1.2.1/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/extensions.rst` & `omniduct-1.2.1/docs/extensions.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/index.rst` & `omniduct-1.2.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/installation.rst` & `omniduct-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/make.bat` & `omniduct-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/protocols.rst` & `omniduct-1.2.1/docs/protocols.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/quickstart.rst` & `omniduct-1.2.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/core.rst` & `omniduct-1.2.1/docs/api/core.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/overview.rst` & `omniduct-1.2.1/docs/api/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/caches/overview.rst` & `omniduct-1.2.1/docs/api/caches/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/databases/overview.rst` & `omniduct-1.2.1/docs/api/databases/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/filesystems/overview.rst` & `omniduct-1.2.1/docs/api/filesystems/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/docs/api/remotes/overview.rst` & `omniduct-1.2.1/docs/api/remotes/overview.rst`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/example_wrapper/README.md` & `omniduct-1.2.1/example_wrapper/README.md`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/example_wrapper/setup.py` & `omniduct-1.2.1/example_wrapper/setup.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/example_wrapper/example_wrapper/__init__.py` & `omniduct-1.2.1/example_wrapper/example_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/example_wrapper/example_wrapper/services.py` & `omniduct-1.2.1/example_wrapper/example_wrapper/services.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/example_wrapper/example_wrapper/services.yml` & `omniduct-1.2.1/example_wrapper/example_wrapper/services.yml`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/__init__.py` & `omniduct-1.2.1/omniduct/__init__.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/_version.py` & `omniduct-1.2.1/omniduct/_version.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/duct.py` & `omniduct-1.2.1/omniduct/duct.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import pwd
 import re
 from abc import abstractmethod
 from builtins import input
 from enum import Enum
 
-from interface_meta import InterfaceMeta, quirk_docs
+from interface_meta import InterfaceMeta, inherit_docs
 
 from omniduct.errors import DuctProtocolUnknown, DuctServerUnreachable
 from omniduct.utils.debug import logger, logging_scope
 from omniduct.utils.dependencies import check_dependencies
 from omniduct.utils.ports import is_port_bound, naive_load_balancer
 
 
@@ -257,15 +257,15 @@
                 )
                 self.disconnect()
                 self.__prepared = False
         except AttributeError:
             pass
         object.__setattr__(self, key, value)
 
-    @quirk_docs("_prepare")
+    @inherit_docs("_prepare")
     def prepare(self):
         """
         Prepare a Duct subclass for use (if not already prepared).
 
         This method is called before the value of any of the fields referenced
         in `self.connection_fields` are retrieved. The fields include, by
         default: 'host', 'port', 'remote', 'cache', 'username', and 'password'.
@@ -472,15 +472,15 @@
                 raise DuctServerUnreachable(
                     f"Cannot connect to '{self.host}:{self.port}' on your current "
                     "connection. Please check your connection before trying again."
                 )
 
     # Connection
     @logging_scope("Connecting")
-    @quirk_docs("_connect")
+    @inherit_docs("_connect")
     def connect(self):
         """
         Connect to the service backing this client.
 
         It is not normally necessary for a user to manually call this function,
         since when a connection is required, it is automatically created.
 
@@ -507,15 +507,15 @@
             )
         return self
 
     @abstractmethod
     def _connect(self):
         raise NotImplementedError
 
-    @quirk_docs("_is_connected")
+    @inherit_docs("_is_connected")
     def is_connected(self):
         """
         Check whether this `Duct` instances is currently connected.
 
         This method checks to see whether a `Duct` instance is currently
         connected. This is performed by verifying that the remote host and port
         are still accessible, and then by calling `Duct._is_connected`, which
@@ -536,15 +536,15 @@
 
         return self._is_connected()
 
     @abstractmethod
     def _is_connected(self):
         raise NotImplementedError
 
-    @quirk_docs("_disconnect")
+    @inherit_docs("_disconnect")
     def disconnect(self):
         """
         Disconnect this client from backing service.
 
         This method is automatically called during reconnections and/or at
         Python interpreter shutdown. It first calls `Duct._disconnect` (which
         should be implemented by subclasses) and then notifies the
```

### Comparing `omniduct-1.2.0/omniduct/logo.png` & `omniduct-1.2.1/omniduct/logo.png`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/logo.svg` & `omniduct-1.2.1/omniduct/logo.svg`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/protocols.py` & `omniduct-1.2.1/omniduct/protocols.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/registry.py` & `omniduct-1.2.1/omniduct/registry.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/caches/_serializers.py` & `omniduct-1.2.1/omniduct/caches/_serializers.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/caches/base.py` & `omniduct-1.2.1/omniduct/caches/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import functools
 from abc import abstractmethod
 
 import dateutil
 import pandas
 import yaml
 from decorator import decorator
-from interface_meta import quirk_docs
+from interface_meta import inherit_docs
 
 from omniduct.duct import Duct
 from omniduct.utils.config import config
 from omniduct.utils.debug import logger
 from omniduct.utils.decorators import function_args_as_kwargs, require_connection
 
 from ._serializers import PickleSerializer
@@ -130,15 +130,15 @@
 class Cache(Duct):
     """
     An abstract class providing the common API for all cache clients.
     """
 
     DUCT_TYPE = Duct.Type.CACHE
 
-    @quirk_docs("_init", mro=True)
+    @inherit_docs("_init", mro=True)
     def __init__(self, **kwargs):  # pylint: disable=super-init-not-called
         Duct.__init_with_kwargs__(self, kwargs)
         self._init(**kwargs)
 
     @abstractmethod
     def _init(self):
         pass
```

### Comparing `omniduct-1.2.0/omniduct/caches/filesystem.py` & `omniduct-1.2.1/omniduct/caches/filesystem.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/_cursor_formatters.py` & `omniduct-1.2.1/omniduct/databases/_cursor_formatters.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/_cursor_serializer.py` & `omniduct-1.2.1/omniduct/databases/_cursor_serializer.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/_namespaces.py` & `omniduct-1.2.1/omniduct/databases/_namespaces.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/_pandas.py` & `omniduct-1.2.1/omniduct/databases/_pandas.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/_schemas.py` & `omniduct-1.2.1/omniduct/databases/_schemas.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/base.py` & `omniduct-1.2.1/omniduct/databases/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 from abc import abstractmethod
 
 import jinja2
 import jinja2.meta
 import sqlparse
 from decorator import decorator
-from interface_meta import quirk_docs, override
+from interface_meta import inherit_docs, override
 
 from omniduct.caches.base import cached_method
 from omniduct.duct import Duct
 from omniduct.filesystems.local import LocalFsClient
 from omniduct.utils.debug import logger, logging_scope
 from omniduct.utils.decorators import require_connection
 from omniduct.utils.magics import (
@@ -92,15 +92,15 @@
     @property
     def NAMESPACE_DEFAULTS_WRITE(self):
         """
         Unless overridden, this is the same as `NAMESPACE_DEFAULTS_READ`.
         """
         return self.NAMESPACE_DEFAULTS_READ
 
-    @quirk_docs("_init", mro=True)
+    @inherit_docs("_init", mro=True)
     # pylint: disable-next=super-init-not-called
     def __init__(
         self,
         session_properties=None,
         templates=None,
         template_context=None,
         default_format_opts=None,
@@ -264,15 +264,15 @@
         serializer=lambda self, kwargs: CursorSerializer(),
         use_cache=lambda self, kwargs: kwargs.pop("use_cache", False),
         metadata=lambda self, kwargs: {
             "statement": kwargs["statement"],
             "session_properties": kwargs["session_properties"],
         },
     )
-    @quirk_docs("_execute")
+    @inherit_docs("_execute")
     @require_connection
     def execute(
         self, statement, wait=True, cursor=None, session_properties=None, **kwargs
     ):
         """
         Execute a statement against this database and return a cursor object.
 
@@ -706,15 +706,15 @@
            object: The results of the query formatted as nominated.
         """
         statement = self.template_render(name, context, by_name=True)
         return self.query(statement, **kwargs)
 
     # Uploading/querying data into data store
     @logging_scope("Query [CTAS]", timed=True)
-    @quirk_docs("_query_to_table")
+    @inherit_docs("_query_to_table")
     def query_to_table(self, statement, table, if_exists="fail", **kwargs):
         """
         Run a query and store the results in a table in this database.
 
         Args:
             statement: The statement to be executed.
             table (str): The name of the table into which the dataframe should
@@ -730,15 +730,15 @@
             DB-API cursor: The cursor object associated with the execution.
         """
         assert if_exists in {"fail", "replace", "append"}
         table = self._parse_namespaces(table, write=True)
         return self._query_to_table(statement, table, if_exists=if_exists, **kwargs)
 
     @logging_scope("Dataframe Upload", timed=True)
-    @quirk_docs("_dataframe_to_table")
+    @inherit_docs("_dataframe_to_table")
     @require_connection
     def dataframe_to_table(self, df, table, if_exists="fail", **kwargs):
         """
         Upload a local pandas dataframe into a table in this database.
 
         Args:
             df (pandas.DataFrame): The dataframe to upload into the database.
@@ -780,15 +780,15 @@
             defaults=defaults
             if defaults
             else (
                 self.NAMESPACE_DEFAULTS_WRITE if write else self.NAMESPACE_DEFAULTS_READ
             ),
         )
 
-    @quirk_docs("_table_list")
+    @inherit_docs("_table_list")
     def table_list(self, namespace=None, renew=True, **kwargs):
         """
         Return a list of table names in the data source as a DataFrame.
 
         Args:
             namespace (str): The namespace in which to look for tables.
             renew (bool): Whether to renew the table list or use cached results
@@ -802,15 +802,15 @@
             self._parse_namespaces(namespace, level=1), renew=renew, **kwargs
         )
 
     @abstractmethod
     def _table_list(self, namespace, **kwargs):
         pass
 
-    @quirk_docs("_table_exists")
+    @inherit_docs("_table_exists")
     def table_exists(self, table, renew=True, **kwargs):
         """
         Check whether a table exists.
 
         Args:
             table (str): The table for which to check.
             renew (bool): Whether to renew the table list or use cached results
@@ -824,15 +824,15 @@
             table=self._parse_namespaces(table), renew=renew, **kwargs
         )
 
     @abstractmethod
     def _table_exists(self, table, **kwargs):
         pass
 
-    @quirk_docs("_table_drop")
+    @inherit_docs("_table_drop")
     def table_drop(self, table, **kwargs):
         """
         Remove a table from the database.
 
         Args:
             table (str): The table to drop.
             **kwargs (dict): Additional arguments passed through to implementation.
@@ -844,15 +844,15 @@
             table=self._parse_namespaces(table, write=True), **kwargs
         )
 
     @abstractmethod
     def _table_drop(self, table, **kwargs):
         pass
 
-    @quirk_docs("_table_desc")
+    @inherit_docs("_table_desc")
     def table_desc(self, table, renew=True, **kwargs):
         """
         Describe a table in the database.
 
         Args:
             table (str): The table to describe.
             renew (bool): Whether to renew the results (default: True).
@@ -865,15 +865,15 @@
             table=self._parse_namespaces(table), renew=renew, **kwargs
         )
 
     @abstractmethod
     def _table_desc(self, table, **kwargs):
         pass
 
-    @quirk_docs("_table_partition_cols")
+    @inherit_docs("_table_partition_cols")
     def table_partition_cols(self, table, renew=True, **kwargs):
         """
         Extract the columns by which a table is partitioned (if database supports partitions).
 
         Args:
             table (str): The table from which to extract data.
             renew (bool): Whether to renew the results (default: True).
@@ -887,15 +887,15 @@
         )
 
     def _table_partition_cols(self, table, **kwargs):
         raise NotImplementedError(
             f"Database backend `{self.__class__.__name__}` does not support, or has not implemented, support for extracting partition columns."
         )
 
-    @quirk_docs("_table_head")
+    @inherit_docs("_table_head")
     def table_head(self, table, n=10, renew=True, **kwargs):
         """
         Retrieve the first `n` rows from a table.
 
         Args:
             table (str): The table from which to extract data.
             n (int): The number of rows to extract.
@@ -911,15 +911,15 @@
             table=self._parse_namespaces(table), n=n, renew=renew, **kwargs
         )
 
     @abstractmethod
     def _table_head(self, table, n=10, **kwargs):
         pass
 
-    @quirk_docs("_table_props")
+    @inherit_docs("_table_props")
     def table_props(self, table, renew=True, **kwargs):
         """
         Retrieve the properties associated with a table.
 
         Args:
             table (str): The table from which to extract data.
             renew (bool): Whether to renew the table list or use cached results
```

### Comparing `omniduct-1.2.0/omniduct/databases/druid.py` & `omniduct-1.2.1/omniduct/databases/druid.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/exasol.py` & `omniduct-1.2.1/omniduct/databases/exasol.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/hiveserver2.py` & `omniduct-1.2.1/omniduct/databases/hiveserver2.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/neo4j.py` & `omniduct-1.2.1/omniduct/databases/neo4j.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/presto.py` & `omniduct-1.2.1/omniduct/databases/presto.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/pyspark.py` & `omniduct-1.2.1/omniduct/databases/pyspark.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/databases/sqlalchemy.py` & `omniduct-1.2.1/omniduct/databases/sqlalchemy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import absolute_import
 
+import urllib
+
 from interface_meta import override
 
 from omniduct.utils.debug import logger
 
 from .base import DatabaseClient
 from ._schemas import SchemasMixin
 from . import _pandas
@@ -58,15 +60,16 @@
         self.connection = None
 
     @property
     def db_uri(self):
         # pylint: disable-next=consider-using-f-string
         return "{dialect}://{login}@{host_port}/{database}".format(
             dialect=self.dialect + (f"+{self.driver}" if self.driver else ""),
-            login=self.username + (f":{self.password}" if self.password else ""),
+            login=self.username
+            + (f":{urllib.parse.quote_plus(self.password)}" if self.password else ""),
             host_port=self.host + (f":{self.port}" if self.port else ""),
             database=self.database,
         )
 
     @override
     def _connect(self):
         import sqlalchemy
```

### Comparing `omniduct-1.2.0/omniduct/databases/stub.py` & `omniduct-1.2.1/omniduct/databases/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/_pyarrow_compat.py` & `omniduct-1.2.1/omniduct/filesystems/_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/_webhdfs_helpers.py` & `omniduct-1.2.1/omniduct/filesystems/_webhdfs_helpers.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/base.py` & `omniduct-1.2.1/omniduct/filesystems/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 from abc import abstractmethod
 from collections import OrderedDict, namedtuple
 
 import pandas as pd
-from interface_meta import quirk_docs, override
+from interface_meta import inherit_docs, override
 
 from omniduct.duct import Duct
 from omniduct.utils.decorators import require_connection
 from omniduct.utils.magics import MagicsProvider, process_line_arguments
 
 
 class FileSystemClient(Duct, MagicsProvider):
@@ -19,15 +19,15 @@
         DEFAULT_PORT (int): The default port for the filesystem service (defined
             by subclasses).
     """
 
     DUCT_TYPE = Duct.Type.FILESYSTEM
     DEFAULT_PORT = None
 
-    @quirk_docs("_init", mro=True)
+    @inherit_docs("_init", mro=True)
     def __init__(  # pylint: disable=super-init-not-called
         self, cwd=None, home=None, read_only=False, global_writes=False, **kwargs
     ):
         """
         cwd (None, str): The path prefix to use as the current working directory
             (if None, the user's home directory is used where that makes sense).
         home (None, str): The path prefix to use as the current users' home
@@ -49,15 +49,15 @@
     @abstractmethod
     def _init(self):
         pass
 
     # Path properties and helpers
 
     @property
-    @quirk_docs("_path_home")
+    @inherit_docs("_path_home")
     @require_connection
     def path_home(self):
         """
         str: The path prefix to use as the current users' home directory. Unless
         `cwd` is set, this will be the prefix to use for all non-absolute path
         references on this filesystem. This is assumed not to change between
         connections, and so will not be updated on client reconnections. Unless
@@ -92,15 +92,15 @@
     @path_cwd.setter
     def path_cwd(self, path_cwd):
         path_cwd = self._path(path_cwd)
         assert self.isdir(path_cwd), "Specified path does not exist."
         self._path_cwd = path_cwd
 
     @property
-    @quirk_docs("_path_separator")
+    @inherit_docs("_path_separator")
     def path_separator(self):
         """
         str: The character(s) to use in separating path components. Typically
         this will be '/'.
         """
         return self._path_separator()
 
@@ -244,15 +244,15 @@
             raise RuntimeError(
                 f"Attempt to write outside of home directory without setting `{self.name}`.`global_writes` to `True`."
             )
         return True
 
     # Filesystem accessors
 
-    @quirk_docs("_exists")
+    @inherit_docs("_exists")
     @require_connection
     def exists(self, path):
         """
         Check whether nominated path exists on this filesytem.
 
         Args:
             path (str): The path for which to check existence.
@@ -263,15 +263,15 @@
         """
         return self._exists(self._path(path))
 
     @abstractmethod
     def _exists(self, path):
         raise NotImplementedError
 
-    @quirk_docs("_isdir")
+    @inherit_docs("_isdir")
     @require_connection
     def isdir(self, path):
         """
         Check whether a nominated path is directory.
 
         Args:
             path (str): The path for which to check directory nature.
@@ -282,15 +282,15 @@
         """
         return self._isdir(self._path(path))
 
     @abstractmethod
     def _isdir(self, path):
         raise NotImplementedError
 
-    @quirk_docs("_isfile")
+    @inherit_docs("_isfile")
     @require_connection
     def isfile(self, path):
         """
         Check whether a nominated path is a file.
 
         Args:
             path (str): The path for which to check file nature.
@@ -309,15 +309,15 @@
     @abstractmethod
     def _dir(self, path):
         """
         This method should return a generator over `FileSystemFileDesc` objects.
         """
         raise NotImplementedError
 
-    @quirk_docs("_dir")
+    @inherit_docs("_dir")
     @require_connection
     def dir(self, path=None):
         """
         Retrieve information about the children of a nominated directory.
 
         This method returns a generator over `FileSystemFileDesc` objects that
         represent the files/directories that a present as children of the
@@ -382,15 +382,15 @@
                 .sort_values(["type", "name"])
                 .reset_index(drop=True)
                 .dropna(axis="columns", how="all")
                 .drop(axis=1, labels=["fs", "path"])
             )
         return "Directory has no contents."
 
-    @quirk_docs("_walk")
+    @inherit_docs("_walk")
     @require_connection
     def walk(self, path=None):
         """
         Explore the filesystem tree starting at a nominated path.
 
         This method returns a generator which recursively walks over all paths
         that are children of `path`, one result for each directory, of form:
@@ -419,15 +419,15 @@
 
         for dirname in dirs:
             for walked in self._walk(
                 self._path(self.path_join(path, dirname))
             ):  # Note: using _walk directly here, which may fail if disconnected during walk.
                 yield walked
 
-    @quirk_docs("_find")
+    @inherit_docs("_find")
     @require_connection
     def find(self, path_prefix=None, **attrs):
         """
         Find a file or directory based on certain attributes.
 
         This method searches for files or folders which satisfy certain
         constraints on the attributes of the file (as encoded into
@@ -471,15 +471,15 @@
 
         for dirname in dirs:
             for match in self._find(
                 self._path(self.path_join(path_prefix, dirname)), **attrs
             ):  # Note: using _find directly here, which may fail if disconnected during find.
                 yield match
 
-    @quirk_docs("_mkdir")
+    @inherit_docs("_mkdir")
     @require_connection
     def mkdir(self, path, recursive=True, exist_ok=False):
         """
         Create a directory at the given path.
 
         Args:
             path (str): The path of the directory to create.
@@ -494,15 +494,15 @@
         self._assert_path_is_writable(path)
         return self._mkdir(self._path(path), recursive, exist_ok)
 
     @abstractmethod
     def _mkdir(self, path, recursive, exist_ok):
         raise NotImplementedError
 
-    @quirk_docs("_remove")
+    @inherit_docs("_remove")
     @require_connection
     def remove(self, path, recursive=False):
         """
         Remove file(s) at a nominated path.
 
         Directories (and their contents) will not be removed unless `recursive`
         is set to `True`.
@@ -523,15 +523,15 @@
 
     @abstractmethod
     def _remove(self, path, recursive):
         raise NotImplementedError
 
     # File handling
 
-    @quirk_docs("_open")
+    @inherit_docs("_open")
     @require_connection
     def open(self, path, mode="rt"):
         """
         Open a file for reading and/or writing.
 
         This method opens the file at the given path for reading and/or writing
         operations. The object returned is programmatically interchangeable with
@@ -549,15 +549,15 @@
         if "w" in mode or "a" in mode or "+" in mode:
             self._assert_path_is_writable(path)
         return self._open(self._path(path), mode=mode)
 
     def _open(self, path, mode):
         return FileSystemFile(self, path, mode)
 
-    @quirk_docs("_file_read_")
+    @inherit_docs("_file_read_")
     @require_connection
     def _file_read(self, path, size=-1, offset=0, binary=False):
         """
         This method is used by `FileSystemFile` to read the contents of files.
         `._file_read_` may be left unimplemented if `.open()` returns a different
         kind of file handle.
 
@@ -573,15 +573,15 @@
         return self._file_read_(
             self._path(path), size=size, offset=offset, binary=binary
         )
 
     def _file_read_(self, path, size=-1, offset=0, binary=False):
         raise NotImplementedError
 
-    @quirk_docs("_file_write_")
+    @inherit_docs("_file_write_")
     @require_connection
     def _file_write(self, path, s, binary=False):
         """
         This method is used by `FileSystemFile` to write to files.
         `._file_write_` may be left unimplemented if `.open()` returns a different
         kind of file handle.
 
@@ -595,15 +595,15 @@
         """
         self._assert_path_is_writable(path)
         return self._file_write_(self._path(path), s, binary)
 
     def _file_write_(self, path, s, binary):
         raise NotImplementedError
 
-    @quirk_docs("_file_append_")
+    @inherit_docs("_file_append_")
     @require_connection
     def _file_append(self, path, s, binary=False):
         """
         This method is used by `FileSystemFile` to append content to files.
         `._file_append_` may be left unimplemented if `.open()` returns a different
         kind of file handle.
 
@@ -619,15 +619,15 @@
         return self._file_append_(self._path(path), s, binary)
 
     def _file_append_(self, path, s, binary):
         raise NotImplementedError
 
     # File transfer
 
-    @quirk_docs("_download")
+    @inherit_docs("_download")
     def download(self, source, dest=None, overwrite=False, fs=None):
         """
         Download files to another filesystem.
 
         This method (recursively) downloads a file/folder from path `source` on
         this filesystem to the path `dest` on filesytem `fs`, overwriting any
         existing file if `overwrite` is `True`.
```

### Comparing `omniduct-1.2.0/omniduct/filesystems/local.py` & `omniduct-1.2.1/omniduct/filesystems/local.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/s3.py` & `omniduct-1.2.1/omniduct/filesystems/s3.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/stub.py` & `omniduct-1.2.1/omniduct/filesystems/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/filesystems/webhdfs.py` & `omniduct-1.2.1/omniduct/filesystems/webhdfs.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/remotes/base.py` & `omniduct-1.2.1/omniduct/remotes/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import getpass
 import re
 from abc import abstractmethod
 
-from interface_meta import quirk_docs, override
+from interface_meta import inherit_docs, override
 
 from omniduct.duct import Duct
 from omniduct.errors import DuctAuthenticationError, DuctServerUnreachable
 from omniduct.filesystems.base import FileSystemClient
 from omniduct.utils.decorators import require_connection
 from omniduct.utils.ports import get_free_local_port, is_local_port_free
 
@@ -116,15 +116,15 @@
     smartcard (dict): Mapping of smartcard names to system libraries
         compatible with `ssh-add -s '<system library>' ...`.
     """
 
     DUCT_TYPE = Duct.Type.REMOTE
     DEFAULT_PORT = None
 
-    @quirk_docs("_init", mro=True)
+    @inherit_docs("_init", mro=True)
     def __init__(
         self, smartcards=None, **kwargs
     ):  # pylint: disable=super-init-not-called
         """
         Args:
             smartcards (dict): Mapping of smartcard names to system libraries
                 compatible with `ssh-add -s '<system library>' ...`.
@@ -213,15 +213,15 @@
         if i != 0:
             raise RuntimeError(
                 "Unexpected error while adding card. Check your passcode and try again."
             )
 
         return True
 
-    @quirk_docs("_execute")
+    @inherit_docs("_execute")
     @require_connection
     def execute(self, cmd, **kwargs):
         """
         Execute a command on the remote server.
 
         Args:
             cmd (str): The command to run on the remote associated with this
@@ -260,15 +260,15 @@
                 m
             ), f"Host not valid: {remote_host}. Must be a string of form 'hostname(:port)'."
 
             host = m.group("host")
             port = m.group("port") or remote_port
         return host, port, local_port
 
-    @quirk_docs("_port_forward_start")
+    @inherit_docs("_port_forward_start")
     @require_connection
     def port_forward(self, remote_host, remote_port=None, local_port=None):
         """
         Initiate a port forward connection.
 
         This method establishes a local port forwarding from a local port `local`
         to remote port `remote`. If `local` is `None`, an available local port is
@@ -350,15 +350,15 @@
         if remote_host is not None and remote_port is not None:
             return (
                 self.__port_forwarding_register.lookup(remote_host, remote_port)
                 is not None
             )
         return self.__port_forwarding_register.reverse_lookup(local_port) is not None
 
-    @quirk_docs("_port_forward_stop")
+    @inherit_docs("_port_forward_stop")
     def port_forward_stop(self, local_port=None, remote_host=None, remote_port=None):
         """
         Disconnect an existing port forward connection.
 
         If a local port is provided, then the forwarding (if any) associated
         with that port is found and stopped; otherwise any established port
         forwarding associated with the nominated remote service is stopped.
@@ -443,15 +443,15 @@
     def _port_forward_start(self, local_port, remote_host, remote_port):
         raise NotImplementedError
 
     @abstractmethod
     def _port_forward_stop(self, local_port, remote_host, remote_port, connection):
         raise NotImplementedError
 
-    @quirk_docs("_is_port_bound")
+    @inherit_docs("_is_port_bound")
     @require_connection
     def is_port_bound(self, host, port):
         """
         Check whether a port on a remote host is accessible.
 
         This method checks to see whether a particular port is active on a
         given host by attempting to establish a connection with it.
```

### Comparing `omniduct-1.2.0/omniduct/remotes/ssh.py` & `omniduct-1.2.1/omniduct/remotes/ssh.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/remotes/ssh_paramiko.py` & `omniduct-1.2.1/omniduct/remotes/ssh_paramiko.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/remotes/stub.py` & `omniduct-1.2.1/omniduct/remotes/stub.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/restful/base.py` & `omniduct-1.2.1/omniduct/restful/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 from urllib.parse import urljoin
 
-from interface_meta import quirk_docs, override
+from interface_meta import inherit_docs, override
 
 from omniduct.duct import Duct
 from omniduct.utils.decorators import require_connection
 
 
 class RestClientBase(Duct):
     """
@@ -25,15 +25,15 @@
             (default: `False`).
         endpoint_prefix (str): The base_url path relative to the host at
             which the API is accessible (default: `''`).
     """
 
     DUCT_TYPE = Duct.Type.RESTFUL
 
-    @quirk_docs("_init", mro=True)
+    @inherit_docs("_init", mro=True)
     def __init__(  # pylint: disable=super-init-not-called
         self,
         server_protocol="http",
         assume_json=False,
         endpoint_prefix="",
         default_timeout=None,
         **kwargs,
```

### Comparing `omniduct-1.2.0/omniduct/utils/about.py` & `omniduct-1.2.1/omniduct/utils/about.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/config.py` & `omniduct-1.2.1/omniduct/utils/config.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/debug.py` & `omniduct-1.2.1/omniduct/utils/debug.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/decorators.py` & `omniduct-1.2.1/omniduct/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/dependencies.py` & `omniduct-1.2.1/omniduct/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/magics.py` & `omniduct-1.2.1/omniduct/utils/magics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from abc import ABCMeta, abstractmethod
 
-from interface_meta import quirk_docs
+from interface_meta import inherit_docs
 
 
 def process_line_arguments(f):
     def wrapped(*args, **kwargs):
         args = list(args)
         new_args, new_kwargs = _process_line_arguments(args.pop(0))
         args += new_args
@@ -45,15 +45,15 @@
             if reached_kwargs:
                 raise ValueError(f"Positional argument `{arg}` after keyword argument.")
             args.append(arg)
     return args, kwargs
 
 
 class MagicsProvider(metaclass=ABCMeta):
-    @quirk_docs("_register_magics")
+    @inherit_docs("_register_magics")
     def register_magics(self, base_name=None):
         base_name = base_name or self.name
         if base_name is None:
             raise RuntimeError("Cannot register magics without a base_name.")
 
         try:
             from IPython import get_ipython
```

### Comparing `omniduct-1.2.0/omniduct/utils/ports.py` & `omniduct-1.2.1/omniduct/utils/ports.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/processes.py` & `omniduct-1.2.1/omniduct/utils/processes.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/omniduct/utils/proxies.py` & `omniduct-1.2.1/omniduct/utils/proxies.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/tests/databases/test__namespaces.py` & `omniduct-1.2.1/tests/databases/test__namespaces.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/tests/databases/test_base.py` & `omniduct-1.2.1/tests/databases/test_base.py`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/.gitignore` & `omniduct-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/LICENSE` & `omniduct-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/README.md` & `omniduct-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `omniduct-1.2.0/pyproject.toml` & `omniduct-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 requires-python = ">=3.7"
 dependencies = [
     "decorator",
-    "interface_meta>=1.1.0,<2",
+    "interface_meta>=1.2.0,<2",
     "jinja2",
     "lazy-object-proxy",
     "packaging",
     "pandas>=0.20.3",
     "progressbar2>=3.30.0",
     "python-dateutil",
     "pyyaml",
```

### Comparing `omniduct-1.2.0/PKG-INFO` & `omniduct-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: omniduct
-Version: 1.2.0
+Version: 1.2.1
 Summary: A toolkit providing a uniform interface for connecting to and extracting data from a wide variety of (potentially remote) data stores (including HDFS, Hive, Presto, MySQL, etc).
 Project-URL: Homepage, https://github.com/airbnb/omniduct
 Author-email: Matthew Wardrop <mpwardrop@gmail.com>, Dan Frank <danfrankj@gmail.com>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7
 Requires-Dist: decorator
-Requires-Dist: interface-meta<2,>=1.1.0
+Requires-Dist: interface-meta<2,>=1.2.0
 Requires-Dist: jinja2
 Requires-Dist: lazy-object-proxy
 Requires-Dist: packaging
 Requires-Dist: pandas>=0.20.3
 Requires-Dist: progressbar2>=3.30.0
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
```

