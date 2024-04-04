# Comparing `tmp/tuf-3.1.0.tar.gz` & `tmp/tuf-3.1.1.tar.gz`

## Comparing `tuf-3.1.0.tar` & `tuf-3.1.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tuf-3.1.0/tox.ini
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/1.0.0-ANNOUNCEMENT.md
--rw-r--r--   0        0        0    30387 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/CONTRIBUTING.rst
--rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/GOVERNANCE.md
--rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/INSTALLATION.rst
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/MAINTAINERS.txt
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/RELEASE.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/SECURITY.md
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_config.yml
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/conf.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/index.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/index.rst
--rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/repository-library-design-ownership.jpg
--rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/repository-library-design-usage.jpg
--rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/repository-library-design.md
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/tuf-horizontal-white.png
--rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/tuf-icon-200.png
--rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/tuf-icon-32.png
--rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_posts/2022-02-21-release-1-0-0.md
--rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_posts/2022-05-04-ngclient-design.md
--rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_posts/2022-06-15-testing-ngclient.md
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md
--rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0000-use-markdown-architectural-decision-records.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0001-python-version-3-6-plus.md
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0002-pre-1-0-deprecation-strategy.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0005-use-google-python-style-guide.md
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0006-where-to-implemenent-model-serialization.md
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0008-accept-unrecognised-fields.md
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0009-what-is-a-reference-implementation.md
--rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/0010-repository-library-design.md
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/index.md
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/adr/template.md
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/api-reference.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.metadata.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.root.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.snapshot.rst
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.supporting.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.targets.rst
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.metadata.timestamp.rst
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.rst
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.api.serialization.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.ngclient.config.rst
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.ngclient.fetcher.rst
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.ngclient.rst
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-3.1.0/docs/api/tuf.ngclient.updater.rst
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/client/README.md
--rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/client/client
--rw-r--r--   0        0        0    14711 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/manual_repo/basic_repo.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/manual_repo/hashed_bin_delegation.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/manual_repo/succinct_hash_bin_delegations.py
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/repository/README.md
--rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/repository/_simplerepo.py
--rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/repository/repo
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/uploader/README.md
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/uploader/_localrepo.py
--rwxr-xr-x   0        0        0     4262 2020-02-02 00:00:00.000000 tuf-3.1.0/examples/uploader/uploader
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/build.txt
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/dev.txt
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/docs.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/lint.txt
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/main.txt
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/pinned.txt
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 tuf-3.1.0/requirements/test.txt
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/.coveragerc
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/__init__.py
--rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/aggregate_tests.py
--rw-r--r--   0        0        0    15467 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_simulator.py
--rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/simple_server.py
--rwxr-xr-x   0        0        0    41811 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_api.py
--rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_examples.py
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_fetcher_ng.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_metadata_eq_.py
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_metadata_generation.py
--rw-r--r--   0        0        0    33661 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_metadata_serialization.py
--rw-r--r--   0        0        0    20171 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_trusted_metadata_set.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_consistent_snapshot.py
--rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_delegation_graphs.py
--rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_fetch_target.py
--rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_key_rotations.py
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_ng.py
--rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_top_level_update.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_updater_validation.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/test_utils.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/__init__.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/generate_md.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/map.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/1.a.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1...json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1.root.json
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1.ö.json
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/timestamp.json
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/delegation_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/delegation_key.pub
--rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key2
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key2.pub
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key3
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/root_key3.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/snapshot_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/snapshot_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/targets_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/targets_key.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/timestamp_key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/keystore/timestamp_key.pub
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/1.root.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/role1.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/role2.json
--rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/root.json
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/snapshot.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/targets.json
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/metadata/timestamp.json
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/targets/file1.txt
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/targets/file2.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-3.1.0/tests/repository_data/repository/targets/file3.txt
--rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/api/__init__.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/api/exceptions.py
--rw-r--r--   0        0        0    75153 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/api/metadata.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/api/serialization/__init__.py
--rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/api/serialization/json.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/README.md
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/__init__.py
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/config.py
--rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/fetcher.py
--rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/updater.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/_internal/__init__.py
--rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/_internal/requests_fetcher.py
--rw-r--r--   0        0        0    19166 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/ngclient/_internal/trusted_metadata_set.py
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/repository/__init__.py
--rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 tuf-3.1.0/tuf/repository/_repository.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.1.0/.gitignore
--rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-3.1.0/LICENSE
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-3.1.0/LICENSE-MIT
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 tuf-3.1.0/README.md
--rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 tuf-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 tuf-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 tuf-3.1.1/tox.ini
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/1.0.0-ANNOUNCEMENT.md
+-rw-r--r--   0        0        0    30664 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     3805 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/GOVERNANCE.md
+-rw-r--r--   0        0        0     3270 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/INSTALLATION.rst
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/MAINTAINERS.txt
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/RELEASE.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/SECURITY.md
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_config.yml
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/conf.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/index.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/index.rst
+-rw-r--r--   0        0        0    50177 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/repository-library-design-ownership.jpg
+-rw-r--r--   0        0        0    42997 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/repository-library-design-usage.jpg
+-rw-r--r--   0        0        0    11688 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/repository-library-design.md
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/tuf-horizontal-white.png
+-rw-r--r--   0        0        0    15399 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/tuf-icon-200.png
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/tuf-icon-32.png
+-rw-r--r--   0        0        0     2551 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_posts/2022-02-21-release-1-0-0.md
+-rw-r--r--   0        0        0     4703 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_posts/2022-05-04-ngclient-design.md
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_posts/2022-06-15-testing-ngclient.md
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_posts/2022-10-21-python-tuf-security-assessment.md
+-rw-r--r--   0        0        0     5484 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/_posts/2023-01-24-securesystemslib-signer-api.md
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0000-use-markdown-architectural-decision-records.md
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0001-python-version-3-6-plus.md
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0002-pre-1-0-deprecation-strategy.md
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0003-where-to-develop-TUF-1-0-0.md
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0004-extent-of-OOP-in-metadata-model.md
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0005-use-google-python-style-guide.md
+-rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0006-where-to-implemenent-model-serialization.md
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0008-accept-unrecognised-fields.md
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0009-what-is-a-reference-implementation.md
+-rw-r--r--   0        0        0     6232 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/0010-repository-library-design.md
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/index.md
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/adr/template.md
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/api-reference.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.metadata.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.root.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.snapshot.rst
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.supporting.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.targets.rst
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.metadata.timestamp.rst
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.rst
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.api.serialization.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.ngclient.config.rst
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.ngclient.fetcher.rst
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.ngclient.rst
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 tuf-3.1.1/docs/api/tuf.ngclient.updater.rst
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/client/README.md
+-rwxr-xr-x   0        0        0     4850 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/client/client
+-rw-r--r--   0        0        0    14711 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/manual_repo/basic_repo.py
+-rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/manual_repo/hashed_bin_delegation.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/manual_repo/succinct_hash_bin_delegations.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/repository/README.md
+-rw-r--r--   0        0        0     7298 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/repository/_simplerepo.py
+-rwxr-xr-x   0        0        0     4484 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/repository/repo
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/uploader/README.md
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/uploader/_localrepo.py
+-rwxr-xr-x   0        0        0     4262 2020-02-02 00:00:00.000000 tuf-3.1.1/examples/uploader/uploader
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/build.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/dev.txt
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/docs.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/lint.txt
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/main.txt
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/pinned.txt
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 tuf-3.1.1/requirements/test.txt
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/.coveragerc
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/__init__.py
+-rwxr-xr-x   0        0        0      904 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/aggregate_tests.py
+-rw-r--r--   0        0        0    15467 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_simulator.py
+-rwxr-xr-x   0        0        0      652 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/simple_server.py
+-rwxr-xr-x   0        0        0    42938 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_api.py
+-rw-r--r--   0        0        0     5795 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_examples.py
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_fetcher_ng.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_metadata_eq_.py
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_metadata_generation.py
+-rw-r--r--   0        0        0    33661 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_metadata_serialization.py
+-rw-r--r--   0        0        0    20171 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_trusted_metadata_set.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_consistent_snapshot.py
+-rw-r--r--   0        0        0    22677 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_delegation_graphs.py
+-rw-r--r--   0        0        0     8562 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_fetch_target.py
+-rw-r--r--   0        0        0    12163 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_key_rotations.py
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_ng.py
+-rw-r--r--   0        0        0    31511 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_top_level_update.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_updater_validation.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/__init__.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/generate_md.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/ed25519_metadata/root_with_ed25519.json
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/ed25519_metadata/snapshot_with_ed25519.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/ed25519_metadata/targets_with_ed25519.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/generated_data/ed25519_metadata/timestamp_with_ed25519.json
+-rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/README.md
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/map.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/timestamp.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/role1.json
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/1.a.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1...json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1.root.json
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1.targets.json
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1.ö.json
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/timestamp.json
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/delegation_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/delegation_key.pub
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key2
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key2.pub
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key3
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/root_key3.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/snapshot_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/snapshot_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/targets_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/targets_key.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/timestamp_key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/keystore/timestamp_key.pub
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/1.root.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/role1.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/role2.json
+-rw-r--r--   0        0        0     3396 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/root.json
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/snapshot.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/targets.json
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/metadata/timestamp.json
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/targets/file1.txt
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/targets/file2.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tuf-3.1.1/tests/repository_data/repository/targets/file3.txt
+-rwxr-xr-x   0        0        0      187 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/api/__init__.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/api/exceptions.py
+-rw-r--r--   0        0        0    75312 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/api/metadata.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/api/serialization/__init__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/api/serialization/json.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/README.md
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/__init__.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/config.py
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/fetcher.py
+-rw-r--r--   0        0        0    19929 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/updater.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/_internal/__init__.py
+-rw-r--r--   0        0        0     5301 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/_internal/requests_fetcher.py
+-rw-r--r--   0        0        0    19166 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/ngclient/_internal/trusted_metadata_set.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/repository/__init__.py
+-rw-r--r--   0        0        0     9276 2020-02-02 00:00:00.000000 tuf-3.1.1/tuf/repository/_repository.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 tuf-3.1.1/.gitignore
+-rw-r--r--   0        0        0     9694 2020-02-02 00:00:00.000000 tuf-3.1.1/LICENSE
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 tuf-3.1.1/LICENSE-MIT
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 tuf-3.1.1/README.md
+-rw-r--r--   0        0        0     5189 2020-02-02 00:00:00.000000 tuf-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 tuf-3.1.1/PKG-INFO
```

### Comparing `tuf-3.1.0/tox.ini` & `tuf-3.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/1.0.0-ANNOUNCEMENT.md` & `tuf-3.1.1/docs/1.0.0-ANNOUNCEMENT.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/CHANGELOG.md` & `tuf-3.1.1/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Changelog
 
+## v3.1.1
+
+This is a security fix release to address advisory
+GHSA-77hh-43cm-v8j6. The issue does **not** affect tuf.ngclient
+users, but could affect tuf.api.metadata users.
+
+### Changed
+* Added additional input validation to
+  `tuf.api.metadata.Targets.get_delegated_role()`
+
 ## v3.1.0
 
 ### Added
 * Metadata API: move verify_delegate() to Root/Targets (#2378)
   - *verify_delegate() on Metadata is now deprecated*
 * Metadata API: add get_verification_result() as verbose alternative for
   verify_delegate() (#2481)
```

### Comparing `tuf-3.1.0/docs/CONTRIBUTING.rst` & `tuf-3.1.1/docs/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/GOVERNANCE.md` & `tuf-3.1.1/docs/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/INSTALLATION.rst` & `tuf-3.1.1/docs/INSTALLATION.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/MAINTAINERS.txt` & `tuf-3.1.1/docs/MAINTAINERS.txt`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/RELEASE.md` & `tuf-3.1.1/docs/RELEASE.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/SECURITY.md` & `tuf-3.1.1/docs/SECURITY.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/conf.py` & `tuf-3.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/index.rst` & `tuf-3.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/repository-library-design-ownership.jpg` & `tuf-3.1.1/docs/repository-library-design-ownership.jpg`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/repository-library-design-usage.jpg` & `tuf-3.1.1/docs/repository-library-design-usage.jpg`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/repository-library-design.md` & `tuf-3.1.1/docs/repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/tuf-horizontal-white.png` & `tuf-3.1.1/docs/tuf-horizontal-white.png`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/tuf-icon-200.png` & `tuf-3.1.1/docs/tuf-icon-200.png`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/tuf-icon-32.png` & `tuf-3.1.1/docs/tuf-icon-32.png`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/_posts/2022-02-21-release-1-0-0.md` & `tuf-3.1.1/docs/_posts/2022-02-21-release-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/_posts/2022-05-04-ngclient-design.md` & `tuf-3.1.1/docs/_posts/2022-05-04-ngclient-design.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/_posts/2022-06-15-testing-ngclient.md` & `tuf-3.1.1/docs/_posts/2022-06-15-testing-ngclient.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/_posts/2022-10-21-python-tuf-security-assessment.md` & `tuf-3.1.1/docs/_posts/2022-10-21-python-tuf-security-assessment.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/_posts/2023-01-24-securesystemslib-signer-api.md` & `tuf-3.1.1/docs/_posts/2023-01-24-securesystemslib-signer-api.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0000-use-markdown-architectural-decision-records.md` & `tuf-3.1.1/docs/adr/0000-use-markdown-architectural-decision-records.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0001-python-version-3-6-plus.md` & `tuf-3.1.1/docs/adr/0001-python-version-3-6-plus.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0002-pre-1-0-deprecation-strategy.md` & `tuf-3.1.1/docs/adr/0002-pre-1-0-deprecation-strategy.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0003-where-to-develop-TUF-1-0-0.md` & `tuf-3.1.1/docs/adr/0003-where-to-develop-TUF-1-0-0.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0004-extent-of-OOP-in-metadata-model.md` & `tuf-3.1.1/docs/adr/0004-extent-of-OOP-in-metadata-model.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0005-use-google-python-style-guide.md` & `tuf-3.1.1/docs/adr/0005-use-google-python-style-guide.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0006-where-to-implemenent-model-serialization.md` & `tuf-3.1.1/docs/adr/0006-where-to-implemenent-model-serialization.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0008-accept-unrecognised-fields.md` & `tuf-3.1.1/docs/adr/0008-accept-unrecognised-fields.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0009-what-is-a-reference-implementation.md` & `tuf-3.1.1/docs/adr/0009-what-is-a-reference-implementation.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/0010-repository-library-design.md` & `tuf-3.1.1/docs/adr/0010-repository-library-design.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/index.md` & `tuf-3.1.1/docs/adr/index.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/adr/template.md` & `tuf-3.1.1/docs/adr/template.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/api/api-reference.rst` & `tuf-3.1.1/docs/api/api-reference.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/api/tuf.api.metadata.supporting.rst` & `tuf-3.1.1/docs/api/tuf.api.metadata.supporting.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/docs/api/tuf.ngclient.rst` & `tuf-3.1.1/docs/api/tuf.ngclient.rst`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/client/README.md` & `tuf-3.1.1/examples/client/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/client/client` & `tuf-3.1.1/examples/client/client`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/manual_repo/basic_repo.py` & `tuf-3.1.1/examples/manual_repo/basic_repo.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/manual_repo/hashed_bin_delegation.py` & `tuf-3.1.1/examples/manual_repo/hashed_bin_delegation.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/manual_repo/succinct_hash_bin_delegations.py` & `tuf-3.1.1/examples/manual_repo/succinct_hash_bin_delegations.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/repository/README.md` & `tuf-3.1.1/examples/repository/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/repository/_simplerepo.py` & `tuf-3.1.1/examples/repository/_simplerepo.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/repository/repo` & `tuf-3.1.1/examples/repository/repo`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/uploader/README.md` & `tuf-3.1.1/examples/uploader/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/uploader/_localrepo.py` & `tuf-3.1.1/examples/uploader/_localrepo.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/examples/uploader/uploader` & `tuf-3.1.1/examples/uploader/uploader`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/aggregate_tests.py` & `tuf-3.1.1/tests/aggregate_tests.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_simulator.py` & `tuf-3.1.1/tests/repository_simulator.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/simple_server.py` & `tuf-3.1.1/tests/simple_server.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_api.py` & `tuf-3.1.1/tests/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1004,12 +1004,39 @@
         self.assertEqual(succinct_roles.suffix_len, expected_suffix_length)
         for bin_numer, role_name in enumerate(succinct_roles.get_roles()):
             # This adds zero-padding if the bin_numer is represented by a hex
             # number with a length less than expected_suffix_length.
             expected_bin_suffix = f"{bin_numer:0{expected_suffix_length}x}"
             self.assertEqual(role_name, f"bin-{expected_bin_suffix}")
 
+    def test_delegations_get_delegated_role(self) -> None:
+        delegations = Delegations({}, {})
+        targets = Targets(delegations=delegations)
+
+        with self.assertRaises(ValueError):
+            targets.get_delegated_role("abc")
+
+        # test "normal" delegated role (path or path_hash_prefix)
+        role = DelegatedRole("delegated", [], 1, False, [])
+        delegations.roles = {"delegated": role}
+        with self.assertRaises(ValueError):
+            targets.get_delegated_role("not-delegated")
+        self.assertEqual(targets.get_delegated_role("delegated"), role)
+        delegations.roles = None
+
+        # test succinct delegation
+        bit_len = 3
+        role2 = SuccinctRoles([], 1, bit_len, "prefix")
+        delegations.succinct_roles = role2
+        for name in ["prefix-", "prefix--1", f"prefix-{2**bit_len:0x}"]:
+            with self.assertRaises(ValueError, msg=f"role name '{name}'"):
+                targets.get_delegated_role(name)
+        for i in range(0, 2**bit_len):
+            self.assertEqual(
+                targets.get_delegated_role(f"prefix-{i:0x}"), role2
+            )
+
 
 # Run unit test.
 if __name__ == "__main__":
     utils.configure_test_logging(sys.argv)
     unittest.main()
```

### Comparing `tuf-3.1.0/tests/test_examples.py` & `tuf-3.1.1/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_fetcher_ng.py` & `tuf-3.1.1/tests/test_fetcher_ng.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_metadata_eq_.py` & `tuf-3.1.1/tests/test_metadata_eq_.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_metadata_generation.py` & `tuf-3.1.1/tests/test_metadata_generation.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_metadata_serialization.py` & `tuf-3.1.1/tests/test_metadata_serialization.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_trusted_metadata_set.py` & `tuf-3.1.1/tests/test_trusted_metadata_set.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_consistent_snapshot.py` & `tuf-3.1.1/tests/test_updater_consistent_snapshot.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_delegation_graphs.py` & `tuf-3.1.1/tests/test_updater_delegation_graphs.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_fetch_target.py` & `tuf-3.1.1/tests/test_updater_fetch_target.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_key_rotations.py` & `tuf-3.1.1/tests/test_updater_key_rotations.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_ng.py` & `tuf-3.1.1/tests/test_updater_ng.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_top_level_update.py` & `tuf-3.1.1/tests/test_updater_top_level_update.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_updater_validation.py` & `tuf-3.1.1/tests/test_updater_validation.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/test_utils.py` & `tuf-3.1.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/utils.py` & `tuf-3.1.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/generated_data/generate_md.py` & `tuf-3.1.1/tests/generated_data/generate_md.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/generated_data/ed25519_metadata/root_with_ed25519.json` & `tuf-3.1.1/tests/generated_data/ed25519_metadata/root_with_ed25519.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/README.md` & `tuf-3.1.1/tests/repository_data/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/1.root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/role1.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/snapshot.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/targets.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/current/timestamp.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/1.root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/role1.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/targets.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json` & `tuf-3.1.1/tests/repository_data/client/test_repository1/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/1.root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/role1.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/snapshot.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/targets.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/current/timestamp.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/current/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/1.root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/role1.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/root.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/targets.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json` & `tuf-3.1.1/tests/repository_data/client/test_repository2/metadata/previous/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1.root.json` & `tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/1.targets.json` & `tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/1.targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json` & `tuf-3.1.1/tests/repository_data/fishy_rolenames/metadata/2.snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/delegation_key` & `tuf-3.1.1/tests/repository_data/keystore/delegation_key`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/root_key` & `tuf-3.1.1/tests/repository_data/keystore/root_key`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/root_key.pub` & `tuf-3.1.1/tests/repository_data/keystore/root_key.pub`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/root_key2` & `tuf-3.1.1/tests/repository_data/keystore/root_key2`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/root_key3` & `tuf-3.1.1/tests/repository_data/keystore/root_key3`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/snapshot_key` & `tuf-3.1.1/tests/repository_data/keystore/snapshot_key`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/targets_key` & `tuf-3.1.1/tests/repository_data/keystore/targets_key`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/keystore/timestamp_key` & `tuf-3.1.1/tests/repository_data/keystore/timestamp_key`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/1.root.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/1.root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/role1.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/role1.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/root.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/root.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/snapshot.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/snapshot.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/targets.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/targets.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tests/repository_data/repository/metadata/timestamp.json` & `tuf-3.1.1/tests/repository_data/repository/metadata/timestamp.json`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/api/exceptions.py` & `tuf-3.1.1/tuf/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/api/metadata.py` & `tuf-3.1.1/tuf/api/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -2040,18 +2040,21 @@
         """Return the role object for the given delegated role.
 
         Raises ValueError if delegated_role is not actually delegated.
         """
         if self.delegations is None:
             raise ValueError("No delegations found")
 
+        role: Optional[Role] = None
         if self.delegations.roles is not None:
-            role: Optional[Role] = self.delegations.roles.get(delegated_role)
-        else:
-            role = self.delegations.succinct_roles
+            role = self.delegations.roles.get(delegated_role)
+        elif self.delegations.succinct_roles is not None:
+            succinct = self.delegations.succinct_roles
+            if succinct.is_delegated_role(delegated_role):
+                role = succinct
 
         if not role:
             raise ValueError(f"Delegated role {delegated_role} not found")
 
         return role
 
     def get_key(self, keyid: str) -> Key:  # noqa: D102
```

### Comparing `tuf-3.1.0/tuf/api/serialization/__init__.py` & `tuf-3.1.1/tuf/api/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/api/serialization/json.py` & `tuf-3.1.1/tuf/api/serialization/json.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/README.md` & `tuf-3.1.1/tuf/ngclient/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/__init__.py` & `tuf-3.1.1/tuf/ngclient/__init__.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/config.py` & `tuf-3.1.1/tuf/ngclient/config.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/fetcher.py` & `tuf-3.1.1/tuf/ngclient/fetcher.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/updater.py` & `tuf-3.1.1/tuf/ngclient/updater.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/_internal/requests_fetcher.py` & `tuf-3.1.1/tuf/ngclient/_internal/requests_fetcher.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/ngclient/_internal/trusted_metadata_set.py` & `tuf-3.1.1/tuf/ngclient/_internal/trusted_metadata_set.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/tuf/repository/_repository.py` & `tuf-3.1.1/tuf/repository/_repository.py`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/LICENSE` & `tuf-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/LICENSE-MIT` & `tuf-3.1.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/README.md` & `tuf-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/pyproject.toml` & `tuf-3.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tuf-3.1.0/PKG-INFO` & `tuf-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuf
-Version: 3.1.0
+Version: 3.1.1
 Summary: A secure updater framework for Python
 Project-URL: Documentation, https://theupdateframework.readthedocs.io/en/stable/
 Project-URL: Homepage, https://www.updateframework.com
 Project-URL: Issues, https://github.com/theupdateframework/python-tuf/issues
 Project-URL: Source, https://github.com/theupdateframework/python-tuf
 Author-email: theupdateframework@googlegroups.com
 License: MIT OR Apache-2.0
```

