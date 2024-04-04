# Comparing `tmp/nucliadb_node_binding-2.46.1.post1078.tar.gz` & `tmp/nucliadb_node_binding-2.46.1.post1079.tar.gz`

## Comparing `nucliadb_node_binding-2.46.1.post1078.tar` & `nucliadb_node_binding-2.46.1.post1079.tar`

### file list

```diff
@@ -1,312 +1,312 @@
--rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12250 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    19361 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    12611 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1405 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    11778 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2722 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127    10271 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    22479 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127     8043 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     4762 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
--rw-r--r--   0     1001      127     1087 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/indexset/state.rs
--rw-r--r--   0     1001      127     2172 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    18388 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    24262 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     2884 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/reader.rs
--rw-r--r--   0     1001      127     4221 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/schema.rs
--rw-r--r--   0     1001      127    21255 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
--rw-r--r--   0     1001      127    17196 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43068 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11380 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18507 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/Cargo.toml
--rw-r--r--   0     1001      127     9354 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/bfs_engine.rs
--rw-r--r--   0     1001      127     1761 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/errors.rs
--rw-r--r--   0     1001      127    21119 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/graph_db.rs
--rw-r--r--   0     1001      127     1784 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
--rw-r--r--   0     1001      127    10531 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/index.rs
--rw-r--r--   0     1001      127     1003 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/lib.rs
--rw-r--r--   0     1001      127     5550 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/node_dictionary.rs
--rw-r--r--   0     1001      127     5249 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/relations_io.rs
--rw-r--r--   0     1001      127     2658 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/bfs.rs
--rw-r--r--   0     1001      127      970 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/mod.rs
--rw-r--r--   0     1001      127     9828 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/reader.rs
--rw-r--r--   0     1001      127    10781 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/tests.rs
--rw-r--r--   0     1001      127     3071 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/utils.rs
--rw-r--r--   0     1001      127     7110 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/writer.rs
--rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2681 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     4869 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2990 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15365 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2069 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8399 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2603 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3806 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2155 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    27030 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127     9078 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    77192 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    10215 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    43211 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    18949 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    32720 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127     5528 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17053 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     8279 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9435 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     4192 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    17730 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      941 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     6724 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py
--rw-r--r--   0     1001      127     2424 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    10762 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13788 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2461 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     4963 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py
--rw-r--r--   0     1001      127     2361 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12553 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     4989 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2323 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      276 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5083 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8259 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1816 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     2566 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18837 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    17048 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2490 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1467 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1473 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2770 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13613 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1937 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2421 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127      997 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14059 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11702 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127     7945 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/inner_settings.rs
--rw-r--r--   0     1001      127     7559 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/mod.rs
--rw-r--r--   0     1001      127     6920 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/providers.rs
--rw-r--r--   0     1001      127     1345 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/mod.rs
--rw-r--r--   0     1001      127     2860 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs
--rw-r--r--   0     1001      127    10693 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1111 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    10834 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1137 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    24437 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    20778 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127    10251 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/versions.rs
--rw-r--r--   0     1001      127     9377 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6383 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12856 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8173 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     7024 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     6862 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22604 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10377 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3391 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2046 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     8881 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3460 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/query_io.rs
--rw-r--r--   0     1001      127    21119 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/reader.rs
--rw-r--r--   0     1001      127     2761 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/schema.rs
--rw-r--r--   0     1001      127     8676 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/search_query.rs
--rw-r--r--   0     1001      127     9257 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/writer.rs
--rw-r--r--   0     1001      127     3389 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/common/mod.rs
--rw-r--r--   0     1001      127     2044 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_reader.rs
--rw-r--r--   0     1001      127     8063 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3458 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_writer.rs
--rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/Makefile
--rw-r--r--   0     1001      127       52 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/README.md
--rwxr-xr-x   0     1001      127      978 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/cov.sh
--rw-r--r--   0     1001      127     1309 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/pyproject.toml
--rw-r--r--   0     1001      127     2203 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/lib.rs
--rw-r--r--   0     1001      127     9575 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/reader.rs
--rw-r--r--   0     1001      127     2162 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/update.rs
--rw-r--r--   0     1001      127    12083 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-04-03 20:41:37.000000 nucliadb_node_binding-2.46.1.post1078/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1078/PKG-INFO
+-rw-r--r--   0        0        0      398 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/query_io.rs
+-rw-r--r--   0     1001      127    21119 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/reader.rs
+-rw-r--r--   0     1001      127     2761 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/schema.rs
+-rw-r--r--   0     1001      127     8676 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/search_query.rs
+-rw-r--r--   0     1001      127     9257 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/writer.rs
+-rw-r--r--   0     1001      127     3389 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2044 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8063 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3458 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_writer.rs
+-rw-r--r--   0        0        0      628 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/reader.rs
+-rw-r--r--   0     1001      127     4221 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/schema.rs
+-rw-r--r--   0     1001      127    21255 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/stop_words.rs
+-rw-r--r--   0     1001      127    17196 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tr.json
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43068 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11380 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18507 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0     3325 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     4192 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    17730 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      941 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     6724 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py
+-rw-r--r--   0     1001      127     2424 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    10762 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13788 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2461 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     4963 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py
+-rw-r--r--   0     1001      127     2361 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12553 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     4989 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2323 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      276 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5083 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8259 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1816 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     2566 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18837 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    17047 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2490 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1467 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1473 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2770 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13613 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1937 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2421 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127      997 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14059 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11702 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127     7945 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/inner_settings.rs
+-rw-r--r--   0     1001      127     7559 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/mod.rs
+-rw-r--r--   0     1001      127     6920 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/providers.rs
+-rw-r--r--   0     1001      127     1345 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/mod.rs
+-rw-r--r--   0     1001      127     2860 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    10693 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1111 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    10834 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1137 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    24437 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    21502 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127    10251 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/versions.rs
+-rw-r--r--   0     1001      127     9377 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6383 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12856 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8173 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     7024 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     6862 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17053 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     8279 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9435 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22604 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10377 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3391 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2046 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     8881 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3460 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      703 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12250 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    19361 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    12611 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1405 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    11778 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2722 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127    10271 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    22479 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127     8043 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     4762 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/mod.rs
+-rw-r--r--   0     1001      127     1087 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/state.rs
+-rw-r--r--   0     1001      127     2172 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    18388 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    24262 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     2884 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      931 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2681 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     4869 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2990 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15365 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2069 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8399 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2603 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3806 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      838 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/Cargo.toml
+-rw-r--r--   0     1001      127     9354 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/bfs_engine.rs
+-rw-r--r--   0     1001      127     1761 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/errors.rs
+-rw-r--r--   0     1001      127    21119 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_db.rs
+-rw-r--r--   0     1001      127     1784 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_test_utils.rs
+-rw-r--r--   0     1001      127    10531 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/index.rs
+-rw-r--r--   0     1001      127     1003 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/lib.rs
+-rw-r--r--   0     1001      127     5550 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/node_dictionary.rs
+-rw-r--r--   0     1001      127     5249 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/relations_io.rs
+-rw-r--r--   0     1001      127     2658 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/bfs.rs
+-rw-r--r--   0     1001      127      970 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/mod.rs
+-rw-r--r--   0     1001      127     9828 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/reader.rs
+-rw-r--r--   0     1001      127    10781 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/tests.rs
+-rw-r--r--   0     1001      127     3071 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/utils.rs
+-rw-r--r--   0     1001      127     7110 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/writer.rs
+-rw-r--r--   0        0        0      501 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2155 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    27030 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127     9078 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    77192 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    10215 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    43211 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    18949 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    32720 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127     5528 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/Makefile
+-rw-r--r--   0     1001      127       52 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/README.md
+-rwxr-xr-x   0     1001      127      978 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/cov.sh
+-rw-r--r--   0     1001      127     1309 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/pyproject.toml
+-rw-r--r--   0     1001      127     2203 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/lib.rs
+-rw-r--r--   0     1001      127     9575 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/reader.rs
+-rw-r--r--   0     1001      127     2162 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/update.rs
+-rw-r--r--   0     1001      127    12082 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-04-04 09:00:21.000000 nucliadb_node_binding-2.46.1.post1079/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 nucliadb_node_binding-2.46.1.post1079/PKG-INFO
```

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/indexset/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/indexset/state.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/indexset/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/search_response.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/stop_words.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ar.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/az.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/bn.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ca.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ch.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/da.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/de.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/el.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/en.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/es.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/eu.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/extract.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/fi.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/fr.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/he.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/hu.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/id.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/it.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/kk.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ne.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/nl.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/no.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/pt.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ro.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/ru.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/sl.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/sv.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs/stop_words/tg.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/bfs_engine.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/bfs_engine.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/errors.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/graph_db.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_db.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/graph_test_utils.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/graph_test_utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/index.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/index.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/node_dictionary.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/node_dictionary.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/relations_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/relations_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/bfs.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/bfs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/tests.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/utils.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations/src/service/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/gc_scheduler.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_gc_scheduler.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         let shard_id = resource.shard_id.clone();
         let shards = Arc::clone(&self.shards);
         let shard_id_clone = shard_id.clone();
         let info = info_span!(parent: &span, "set resource");
         let write_task = || {
             run_with_telemetry(info, move || {
                 let shard = obtain_shard(shards, shard_id_clone)?;
-                shard.set_resource(&resource).and_then(|()| shard.get_opstatus())
+                shard.set_resource(resource).and_then(|()| shard.get_opstatus())
             })
         };
         let status = tokio::task::spawn_blocking(write_task)
             .await
             .map_err(|error| tonic::Status::internal(format!("Blocking task panicked: {error:?}")))?;
         match status {
             Ok(mut status) => {
```

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/inner_settings.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/inner_settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/settings/providers.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/settings/providers.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,37 @@
 use crate::disk_structure::*;
 use crate::shards::metadata::ShardMetadata;
 use crate::shards::versions::Versions;
 use crate::telemetry::run_with_telemetry;
 
 pub struct BlockingToken<'a>(MutexGuard<'a, ()>);
 
+const MAX_LABEL_LENGTH: usize = 32768; // Tantivy max is 2^16 - 4
+
+fn remove_invalid_labels(resource: &mut Resource) {
+    resource.labels.retain(|l| {
+        if l.len() > MAX_LABEL_LENGTH {
+            warn!("Label length ({}) longer than maximum, it will not be indexed", l.len());
+            false
+        } else {
+            true
+        }
+    });
+    for text in resource.texts.values_mut() {
+        text.labels.retain(|l| {
+            if l.len() > MAX_LABEL_LENGTH {
+                warn!("Label length ({}) longer than maximum, it will not be indexed", l.len());
+                false
+            } else {
+                true
+            }
+        });
+    }
+}
+
 #[derive(Debug)]
 pub struct ShardWriter {
     pub metadata: Arc<ShardMetadata>,
     pub id: String,
     pub path: PathBuf,
     text_writer: TextsWriterPointer,
     paragraph_writer: ParagraphsWriterPointer,
@@ -208,17 +231,19 @@
         };
 
         ShardWriter::initialize(metadata, tsc, psc, vsc, rsc)
     }
 
     #[measure(actor = "shard", metric = "set_resource")]
     #[tracing::instrument(skip_all)]
-    pub fn set_resource(&self, resource: &Resource) -> NodeResult<()> {
+    pub fn set_resource(&self, mut resource: Resource) -> NodeResult<()> {
         let span = tracing::Span::current();
 
+        remove_invalid_labels(&mut resource);
+
         let text_writer_service = self.text_writer.clone();
         let field_resource = resource.clone();
         let text_task = move || {
             debug!("Field service starts set_resource");
             let mut writer = write_rw_lock(&text_writer_service);
             let result = writer.set_resource(&field_resource);
             debug!("Field service ends set_resource");
```

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/shards/versions.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/shards/versions.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/query_io.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/schema.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/search_query.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/common/mod.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_reader.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_search.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_streaming.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/local_dependencies/nucliadb_texts/tests/test_writer.rs` & `nucliadb_node_binding-2.46.1.post1079/local_dependencies/nucliadb_texts/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/Cargo.toml` & `nucliadb_node_binding-2.46.1.post1079/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "2.46.1-post1078"
+version = "2.46.1-post1079"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-2.46.1.post1078/CHANGELOG.md` & `nucliadb_node_binding-2.46.1.post1079/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/Makefile` & `nucliadb_node_binding-2.46.1.post1079/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/cov.sh` & `nucliadb_node_binding-2.46.1.post1079/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/pyproject.toml` & `nucliadb_node_binding-2.46.1.post1079/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/collect_garbage.rs` & `nucliadb_node_binding-2.46.1.post1079/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/errors.rs` & `nucliadb_node_binding-2.46.1.post1079/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/lib.rs` & `nucliadb_node_binding-2.46.1.post1079/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/reader.rs` & `nucliadb_node_binding-2.46.1.post1079/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/update.rs` & `nucliadb_node_binding-2.46.1.post1079/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/src/writer.rs` & `nucliadb_node_binding-2.46.1.post1079/src/writer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         ))
     }
 
     pub fn set_resource<'p>(&mut self, resource: RawProtos, py: Python<'p>) -> PyResult<&'p PyAny> {
         let resource = Resource::decode(&mut Cursor::new(resource)).expect("Error decoding arguments");
         let shard_id = resource.shard_id.clone();
         let shard = self.obtain_shard(shard_id.clone())?;
-        let status = shard.set_resource(&resource).and_then(|()| shard.get_opstatus());
+        let status = shard.set_resource(resource).and_then(|()| shard.get_opstatus());
         match status {
             Ok(mut status) => {
                 status.status = 0;
                 status.detail = "Success!".to_string();
                 Ok(PyList::new(py, status.encode_to_vec()))
             }
             Err(error) => {
```

### Comparing `nucliadb_node_binding-2.46.1.post1078/tests/__init__.py` & `nucliadb_node_binding-2.46.1.post1079/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/tests/conftest.py` & `nucliadb_node_binding-2.46.1.post1079/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-2.46.1.post1078/tests/integration/test_indexing.py` & `nucliadb_node_binding-2.46.1.post1079/tests/integration/test_indexing.py`

 * *Files identical despite different names*

