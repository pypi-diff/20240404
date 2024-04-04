# Comparing `tmp/altrios-0.1.8.tar.gz` & `tmp/altrios-0.2.0.tar.gz`

## Comparing `altrios-0.1.8.tar` & `altrios-0.2.0.tar`

### file list

```diff
@@ -1,204 +1,202 @@
--rw-r--r--   0     1001      127     1236 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/Cargo.toml
--rw-r--r--   0     1001      127      784 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/README.md
--rw-r--r--   0     1001      127     2475 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/combo_error.rs
--rw-r--r--   0     1001      127    22741 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/consist_model.rs
--rw-r--r--   0     1001      127     4095 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/consist_sim.rs
--rw-r--r--   0     1001      127    11016 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/consist_utils.rs
--rw-r--r--   0     1001      127     3176 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
--rw-r--r--   0     1001      127     3605 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
--rw-r--r--   0     1001      127    12008 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
--rw-r--r--   0     1001      127    13285 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/loco_sim.rs
--rw-r--r--   0     1001      127    37832 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
--rw-r--r--   0     1001      127      991 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/mod.rs
--rw-r--r--   0     1001      127      430 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
--rw-r--r--   0     1001      127    14859 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
--rw-r--r--   0     1001      127     1034 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
--rw-r--r--   0     1001      127    13478 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
--rw-r--r--   0     1001      127      348 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
--rw-r--r--   0     1001      127    14475 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
--rw-r--r--   0     1001      127      213 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
--rw-r--r--   0     1001      127      938 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
--rw-r--r--   0     1001      127     9907 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
--rw-r--r--   0     1001      127    30918 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
--rw-r--r--   0     1001      127      200 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
--rw-r--r--   0     1001      127     2790 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/locomotive/tests.rs
--rw-r--r--   0     1001      127      752 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/mod.rs
--rw-r--r--   0     1001      127     1039 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/consist/tests.rs
--rw-r--r--   0     1001      127     1299 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/imports.rs
--rw-r--r--   0     1001      127     1142 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/lib.rs
--rw-r--r--   0     1001      127     1602 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/lin_search_hint.rs
--rw-r--r--   0     1001      127     8028 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/macros.rs
--rw-r--r--   0     1001      127      482 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/disp_imports.rs
--rw-r--r--   0     1001      127     5431 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/disp_structs.rs
--rw-r--r--   0     1001      127    11583 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/dispatch.rs
--rw-r--r--   0     1001      127     2661 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
--rw-r--r--   0     1001      127    29630 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/mod.rs
--rw-r--r--   0     1001      127     9721 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/update_times.rs
--rw-r--r--   0     1001      127      281 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/mod.rs
--rw-r--r--   0     1001      127    25666 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
--rw-r--r--   0     1001      127    36649 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
--rw-r--r--   0     1001      127     9716 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/mod.rs
--rw-r--r--   0     1001      127     1961 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/prelude.rs
--rw-r--r--   0     1001      127      255 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/pyo3.rs
--rw-r--r--   0     1001      127     1039 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/si.rs
--rw-r--r--   0     1001      127     2613 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/testing.rs
--rw-r--r--   0     1001      127     2129 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/cat_power.rs
--rw-r--r--   0     1001      127     3743 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/elev.rs
--rw-r--r--   0     1001      127     4158 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/heading.rs
--rw-r--r--   0     1001      127     4718 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/link_idx.rs
--rw-r--r--   0     1001      127    19359 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/link_impl.rs
--rw-r--r--   0     1001      127     1241 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/link_old.rs
--rw-r--r--   0     1001      127     1900 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/location.rs
--rw-r--r--   0     1001      127      246 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/locations.csv
--rw-r--r--   0     1001      127      301 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/mod.rs
--rw-r--r--   0     1001      127     4792 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_limit.rs
--rw-r--r--   0     1001      127     3242 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_param.rs
--rw-r--r--   0     1001      127     5971 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_set.rs
--rw-r--r--   0     1001      127      120 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/link/speed.rs
--rw-r--r--   0     1001      127      120 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/mod.rs
--rw-r--r--   0     1001      127     6079 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/link_point.rs
--rw-r--r--   0     1001      127      182 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/mod.rs
--rw-r--r--   0     1001      127     2826 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/path_res_coeff.rs
--rw-r--r--   0     1001      127    19968 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/path_tpc.rs
--rw-r--r--   0     1001      127     7804 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/speed_point.rs
--rw-r--r--   0     1001      127     3842 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/track/path_track/train_params.rs
--rw-r--r--   0     1001      127     6200 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/braking_point.rs
--rw-r--r--   0     1001      127     3503 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/friction_brakes.rs
--rw-r--r--   0     1001      127      344 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/mod.rs
--rw-r--r--   0     1001      127     3605 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/rail_vehicle.rs
--rw-r--r--   0     1001      127     1124 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
--rw-r--r--   0     1001      127      324 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/bearing.rs
--rw-r--r--   0     1001      127      438 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/davis_b.rs
--rw-r--r--   0     1001      127       90 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/mod.rs
--rw-r--r--   0     1001      127     3834 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/path_res.rs
--rw-r--r--   0     1001      127      397 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/rolling.rs
--rw-r--r--   0     1001      127       75 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/method/mod.rs
--rw-r--r--   0     1001      127     2276 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/method/point.rs
--rw-r--r--   0     1001      127     2683 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/method/strap.rs
--rw-r--r--   0     1001      127     1247 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/resistance/mod.rs
--rw-r--r--   0     1001      127    12652 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/set_speed_train_sim.rs
--rw-r--r--   0     1001      127    24523 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/speed_limit_train_sim.rs
--rw-r--r--   0     1001      127      443 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/test_rail_vehicles.csv
--rw-r--r--   0     1001      127      182 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/timed_path.rs
--rw-r--r--   0     1001      127    40485 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/train_config.rs
--rw-r--r--   0     1001      127      317 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/train_imports.rs
--rw-r--r--   0     1001      127     6786 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/train/train_state.rs
--rw-r--r--   0     1001      127    10138 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/traits.rs
--rw-r--r--   0     1001      127     2849 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/uc.rs
--rw-r--r--   0     1001      127    13949 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     2455 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/utils/val_range.rs
--rw-r--r--   0     1001      127     7292 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/src/validate.rs
--rw-r--r--   0     1001      127      578 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/Cargo.toml
--rw-r--r--   0     1001      127      707 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/README.md
--rw-r--r--   0     1001      127    10749 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
--rw-r--r--   0     1001      127    13787 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/altrios_api.rs
--rw-r--r--   0     1001      127     4077 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
--rw-r--r--   0     1001      127     2741 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
--rw-r--r--   0     1001      127      367 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/imports.rs
--rw-r--r--   0     1001      127     1192 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/lib.rs
--rw-r--r--   0     1001      127      571 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
--rw-r--r--   0     1001      127     3154 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/utilities.rs
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 altrios-0.1.8/rust/altrios-py/Cargo.toml
--rw-r--r--   0     1001      127      586 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-py/README.md
--rw-r--r--   0     1001      127     3016 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/altrios-py/src/lib.rs
--rw-r--r--   0     1001      127    59381 2024-03-25 20:55:48.000000 altrios-0.1.8/rust/Cargo.lock
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 altrios-0.1.8/rust/Cargo.toml
--rw-r--r--   0     1001      127     2197 2024-03-25 20:55:48.000000 altrios-0.1.8/pyproject.toml
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/fuel_converters/__init__.py
--rw-r--r--   0     1001      127      999 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
--rw-r--r--   0     1001      127    25350 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
--rw-r--r--   0     1001      127     9907 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/trains/__init__.py
--rw-r--r--   0     1001      127      568 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/trains/train_res_temp.yaml
--rw-r--r--   0     1001      127      350 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/demo_data/link_points_idx.csv
--rw-r--r--   0     1001      127       15 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
--rw-r--r--   0     1001      127      191 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/demo_data/README.md
--rw-r--r--   0     1001      127     2279 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/demo_data/speed_trace.csv
--rw-r--r--   0     1001      127      274 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/__init__.py
--rw-r--r--   0     1001      127      390 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/default_locations.csv
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/__init__.py
--rw-r--r--   0     1001      127     1153 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/links_test.yaml
--rw-r--r--   0     1001      127  2550221 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/Taconite.yaml
--rw-r--r--   0     1001      127     8946 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/simple_corridor_two_segment_network.yaml
--rw-r--r--   0     1001      127     3595 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/simple_corridor_network.yaml
--rw-r--r--   0     1001      127      214 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/simple_corridor_locations.csv
--rw-r--r--   0     1001      127  2499520 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/Taconite-NoBalloon.yaml
--rw-r--r--   0     1001      127     8823 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/two_segment_network.yaml
--rw-r--r--   0     1001      127      548 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
--rw-r--r--   0     1001      127      136 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/networks/network_charging_guidelines.csv
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/powertrain_model_input_example.csv
--rw-r--r--   0     1001      127      695 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/Default Demand StoBar.csv
--rw-r--r--   0     1001      127      253 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/Default Demand.csv
--rw-r--r--   0     1001      127       50 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/tpc_input_example.csv
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/__init__.py
--rw-r--r--   0     1001      127      498 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
--rw-r--r--   0     1001      127      501 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Unit.yaml
--rw-r--r--   0     1001      127      492 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Intermodal.yaml
--rw-r--r--   0     1001      127      496 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
--rw-r--r--   0     1001      127      641 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/rail_vehicles.csv
--rw-r--r--   0     1001      127      492 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Unit_Empty.yaml
--rw-r--r--   0     1001      127      511 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/rolling_stock/Manifest.yaml
--rw-r--r--   0     1001      127   128287 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
--rw-r--r--   0     1001      127      994 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
--rw-r--r--   0     1001      127  1237826 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
--rw-r--r--   0     1001      127     2025 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
--rw-r--r--   0     1001      127    10562 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
--rw-r--r--   0     1001      127     1616 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
--rw-r--r--   0     1001      127    67018 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/resources/TimedPaths.csv
--rw-r--r--   0     1001      127     1078 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/objectives.py
--rw-r--r--   0     1001      127     4178 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/speed_limit_train_sim_demo.py
--rw-r--r--   0     1001      127      111 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/__init__.py
--rw-r--r--   0     1001      127     2351 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/conv_demo.py
--rw-r--r--   0     1001      127     3482 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/rollout_demo.py
--rw-r--r--   0     1001      127      278 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/demo_logging.py
--rw-r--r--   0     1001      127     2371 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/bel_demo.py
--rw-r--r--   0     1001      127     3600 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/set_speed_simple_corr_demo.py
--rw-r--r--   0     1001      127     4030 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/set_speed_train_sim_demo.py
--rw-r--r--   0     1001      127     4214 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/speed_limit_simple_corr_demo.py
--rw-r--r--   0     1001      127      578 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/test_demos.py
--rw-r--r--   0     1001      127     5586 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/demos/sim_manager_demo.py
--rw-r--r--   0     1001      127      386 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/plot.py
--rw-r--r--   0     1001      127     2074 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/defaults.py
--rw-r--r--   0     1001      127    52841 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/output_12072022.csv
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/loaders/__init__.py
--rw-r--r--   0     1001      127     3448 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/loaders/powertrain_components.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/py.typed
--rw-r--r--   0     1001      127    53858 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/train_planner.py
--rw-r--r--   0     1001      127      766 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/stringline_old.py
--rw-r--r--   0     1001      127    41804 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/metric_calculator.py
--rw-r--r--   0     1001      127    16755 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/stringline.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/fuel_grid.py
--rw-r--r--   0     1001      127     5693 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/sim_manager.py
--rw-r--r--   0     1001      127    29289 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/altrios_pyo3.pyi
--rw-r--r--   0     1001      127     6896 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/rollout.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/user_interface.py
--rw-r--r--   0     1001      127     1754 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_powertrain_res.py
--rw-r--r--   0     1001      127     1279 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_powertrain_fuel_conv.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/__init__.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_multi_obj_opt.py
--rw-r--r--   0     1001      127      689 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_locomotive_simulation.py
--rw-r--r--   0     1001      127      928 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_metric_calculator.py
--rw-r--r--   0     1001      127      603 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_consist.py
--rw-r--r--   0     1001      127     2351 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_multi_obj_cal_and_val.py
--rw-r--r--   0     1001      127      386 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_train_simulation.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_objectives.py
--rw-r--r--   0     1001      127        0 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_fuel_grid.py
--rw-r--r--   0     1001      127      675 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_consist_sim.py
--rw-r--r--   0     1001      127      747 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_powertrain_generator.py
--rw-r--r--   0     1001      127     1019 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_utilities.py
--rw-r--r--   0     1001      127      229 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_train_planner.py
--rw-r--r--   0     1001      127     1533 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_locomotive.py
--rw-r--r--   0     1001      127      874 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_powertrain_edrive.py
--rw-r--r--   0     1001      127     7941 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/mock_resources.py
--rw-r--r--   0     1001      127      652 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/tests/test_rail_vehicles.py
--rw-r--r--   0     1001      127       25 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/optimization/__init__.py
--rw-r--r--   0     1001      127    24471 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/optimization/cal_and_val.py
--rw-r--r--   0     1001      127       91 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/optimization/multi_obj_opt.py
--rw-r--r--   0     1001      127     8741 2024-03-25 20:55:48.000000 altrios-0.1.8/python/altrios/utilities.py
--rw-r--r--   0     1001      127     7492 2024-03-25 20:55:48.000000 altrios-0.1.8/README.md
--rw-r--r--   0     1001      127     1660 2024-03-25 20:55:48.000000 altrios-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 altrios-0.1.8/PKG-INFO
+-rw-r--r--   0     1001      127      578 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/Cargo.toml
+-rw-r--r--   0     1001      127      707 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/README.md
+-rw-r--r--   0     1001      127    10749 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs
+-rw-r--r--   0     1001      127    13309 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/altrios_api.rs
+-rw-r--r--   0     1001      127     4077 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs
+-rw-r--r--   0     1001      127     2741 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs
+-rw-r--r--   0     1001      127      367 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/imports.rs
+-rw-r--r--   0     1001      127     1192 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/lib.rs
+-rw-r--r--   0     1001      127      571 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs
+-rw-r--r--   0     1001      127     3154 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/utilities.rs
+-rw-r--r--   0     1001      127     1212 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/Cargo.toml
+-rw-r--r--   0     1001      127      784 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/README.md
+-rw-r--r--   0     1001      127     2475 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/combo_error.rs
+-rw-r--r--   0     1001      127    22741 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/consist_model.rs
+-rw-r--r--   0     1001      127     4095 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/consist_sim.rs
+-rw-r--r--   0     1001      127    12088 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/consist_utils.rs
+-rw-r--r--   0     1001      127     3176 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs
+-rw-r--r--   0     1001      127     3606 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/conventional_loco.rs
+-rw-r--r--   0     1001      127    12008 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs
+-rw-r--r--   0     1001      127    13285 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/loco_sim.rs
+-rw-r--r--   0     1001      127    39926 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/locomotive_model.rs
+-rw-r--r--   0     1001      127      991 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/mod.rs
+-rw-r--r--   0     1001      127      430 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.default.yaml
+-rw-r--r--   0     1001      127    14859 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs
+-rw-r--r--   0     1001      127     1034 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml
+-rw-r--r--   0     1001      127    13407 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs
+-rw-r--r--   0     1001      127      348 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/generator.default.yaml
+-rw-r--r--   0     1001      127    14475 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs
+-rw-r--r--   0     1001      127      213 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/mod.rs
+-rw-r--r--   0     1001      127      938 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs
+-rw-r--r--   0     1001      127     9907 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml
+-rw-r--r--   0     1001      127    30918 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs
+-rw-r--r--   0     1001      127      200 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/test.rs
+-rw-r--r--   0     1001      127     2790 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/locomotive/tests.rs
+-rw-r--r--   0     1001      127      752 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/mod.rs
+-rw-r--r--   0     1001      127     1039 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/consist/tests.rs
+-rw-r--r--   0     1001      127     1254 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/imports.rs
+-rw-r--r--   0     1001      127     1142 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/lib.rs
+-rw-r--r--   0     1001      127     1602 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/lin_search_hint.rs
+-rw-r--r--   0     1001      127     8028 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/macros.rs
+-rw-r--r--   0     1001      127      482 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/disp_imports.rs
+-rw-r--r--   0     1001      127     5431 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/disp_structs.rs
+-rw-r--r--   0     1001      127    11567 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/dispatch.rs
+-rw-r--r--   0     1001      127     2661 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs
+-rw-r--r--   0     1001      127    29031 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/mod.rs
+-rw-r--r--   0     1001      127     9721 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/update_times.rs
+-rw-r--r--   0     1001      127      281 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/mod.rs
+-rw-r--r--   0     1001      127    25666 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs
+-rw-r--r--   0     1001      127    36649 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/free_path.rs
+-rw-r--r--   0     1001      127     9684 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/mod.rs
+-rw-r--r--   0     1001      127     1940 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/prelude.rs
+-rw-r--r--   0     1001      127      255 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/pyo3.rs
+-rw-r--r--   0     1001      127     1039 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/si.rs
+-rw-r--r--   0     1001      127     2613 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/testing.rs
+-rw-r--r--   0     1001      127     2129 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/cat_power.rs
+-rw-r--r--   0     1001      127     3743 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/elev.rs
+-rw-r--r--   0     1001      127     4947 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/heading.rs
+-rw-r--r--   0     1001      127     4752 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/link_idx.rs
+-rw-r--r--   0     1001      127    20637 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/link_impl.rs
+-rw-r--r--   0     1001      127     1387 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/link_old.rs
+-rw-r--r--   0     1001      127     1900 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/location.rs
+-rw-r--r--   0     1001      127      246 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/locations.csv
+-rw-r--r--   0     1001      127      301 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/mod.rs
+-rw-r--r--   0     1001      127     4792 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_limit.rs
+-rw-r--r--   0     1001      127     3242 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_param.rs
+-rw-r--r--   0     1001      127     5971 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_set.rs
+-rw-r--r--   0     1001      127      120 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/link/speed.rs
+-rw-r--r--   0     1001      127      120 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/mod.rs
+-rw-r--r--   0     1001      127     6079 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/link_point.rs
+-rw-r--r--   0     1001      127      182 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/mod.rs
+-rw-r--r--   0     1001      127     2826 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/path_res_coeff.rs
+-rw-r--r--   0     1001      127    19995 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/path_tpc.rs
+-rw-r--r--   0     1001      127     7804 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/speed_point.rs
+-rw-r--r--   0     1001      127     3842 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/track/path_track/train_params.rs
+-rw-r--r--   0     1001      127     6200 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/braking_point.rs
+-rw-r--r--   0     1001      127     3503 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/friction_brakes.rs
+-rw-r--r--   0     1001      127      344 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/mod.rs
+-rw-r--r--   0     1001      127     3605 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/rail_vehicle.rs
+-rw-r--r--   0     1001      127     1124 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs
+-rw-r--r--   0     1001      127      324 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/bearing.rs
+-rw-r--r--   0     1001      127      438 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/davis_b.rs
+-rw-r--r--   0     1001      127       90 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/path_res.rs
+-rw-r--r--   0     1001      127      397 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/rolling.rs
+-rw-r--r--   0     1001      127      133 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/method/mod.rs
+-rw-r--r--   0     1001      127     2253 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/method/point.rs
+-rw-r--r--   0     1001      127     2684 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/method/strap.rs
+-rw-r--r--   0     1001      127     1780 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/resistance/mod.rs
+-rw-r--r--   0     1001      127    13755 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/set_speed_train_sim.rs
+-rw-r--r--   0     1001      127    24586 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/speed_limit_train_sim.rs
+-rw-r--r--   0     1001      127      443 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/test_rail_vehicles.csv
+-rw-r--r--   0     1001      127      182 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/timed_path.rs
+-rw-r--r--   0     1001      127    40485 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/train_config.rs
+-rw-r--r--   0     1001      127      338 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/train_imports.rs
+-rw-r--r--   0     1001      127     8167 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/train/train_state.rs
+-rw-r--r--   0     1001      127    10138 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/traits.rs
+-rw-r--r--   0     1001      127     2849 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/uc.rs
+-rw-r--r--   0     1001      127    13949 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     2455 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/utils/val_range.rs
+-rw-r--r--   0     1001      127     7292 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-core/src/validate.rs
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 altrios-0.2.0/rust/altrios-py/Cargo.toml
+-rw-r--r--   0     1001      127      586 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-py/README.md
+-rw-r--r--   0     1001      127     2954 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/altrios-py/src/lib.rs
+-rw-r--r--   0     1001      127    59363 2024-04-04 17:55:26.000000 altrios-0.2.0/rust/Cargo.lock
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 altrios-0.2.0/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2197 2024-04-04 17:55:26.000000 altrios-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/fuel_converters/__init__.py
+-rw-r--r--   0     1001      127      999 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/reversible_energy_storages/__init__.py
+-rw-r--r--   0     1001      127    25350 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx
+-rw-r--r--   0     1001      127     9907 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/trains/__init__.py
+-rw-r--r--   0     1001      127      568 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/trains/train_res_temp.yaml
+-rw-r--r--   0     1001      127      350 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/demo_data/link_points_idx.csv
+-rw-r--r--   0     1001      127       15 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/demo_data/link_points_idx_simple_corridor.csv
+-rw-r--r--   0     1001      127      191 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/demo_data/README.md
+-rw-r--r--   0     1001      127     2279 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/demo_data/speed_trace.csv
+-rw-r--r--   0     1001      127      274 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/demo_data/speed_trace_simple_corridor.csv
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/__init__.py
+-rw-r--r--   0     1001      127      390 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/default_locations.csv
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/__init__.py
+-rw-r--r--   0     1001      127     1153 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/links_test.yaml
+-rw-r--r--   0     1001      127  3192802 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/Taconite.yaml
+-rw-r--r--   0     1001      127     3595 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/simple_corridor_network.yaml
+-rw-r--r--   0     1001      127      214 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/simple_corridor_locations.csv
+-rw-r--r--   0     1001      127  3119913 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/Taconite-NoBalloon.yaml
+-rw-r--r--   0     1001      127      548 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv
+-rw-r--r--   0     1001      127      136 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/networks/network_charging_guidelines.csv
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/powertrain_model_input_example.csv
+-rw-r--r--   0     1001      127      695 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/Default Demand StoBar.csv
+-rw-r--r--   0     1001      127      253 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/Default Demand.csv
+-rw-r--r--   0     1001      127       50 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/tpc_input_example.csv
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/__init__.py
+-rw-r--r--   0     1001      127      498 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Intermodal_Empty.yaml
+-rw-r--r--   0     1001      127      501 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Unit.yaml
+-rw-r--r--   0     1001      127      492 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Intermodal.yaml
+-rw-r--r--   0     1001      127      496 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Manifest_Empty.yaml
+-rw-r--r--   0     1001      127      641 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/rail_vehicles.csv
+-rw-r--r--   0     1001      127      492 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Unit_Empty.yaml
+-rw-r--r--   0     1001      127      511 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/rolling_stock/Manifest.yaml
+-rw-r--r--   0     1001      127   128287 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv
+-rw-r--r--   0     1001      127      994 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv
+-rw-r--r--   0     1001      127  1237826 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv
+-rw-r--r--   0     1001      127     2025 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv
+-rw-r--r--   0     1001      127    10562 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv
+-rw-r--r--   0     1001      127     1616 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv
+-rw-r--r--   0     1001      127    67018 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/resources/TimedPaths.csv
+-rw-r--r--   0     1001      127     1078 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/objectives.py
+-rw-r--r--   0     1001      127     5988 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/speed_limit_train_sim_demo.py
+-rw-r--r--   0     1001      127      111 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/__init__.py
+-rw-r--r--   0     1001      127     2357 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/conv_demo.py
+-rw-r--r--   0     1001      127     3488 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/rollout_demo.py
+-rw-r--r--   0     1001      127      278 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/demo_logging.py
+-rw-r--r--   0     1001      127     2377 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/bel_demo.py
+-rw-r--r--   0     1001      127     3410 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/set_speed_simple_corr_demo.py
+-rw-r--r--   0     1001      127     3860 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/set_speed_train_sim_demo.py
+-rw-r--r--   0     1001      127     4220 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/speed_limit_simple_corr_demo.py
+-rw-r--r--   0     1001      127      578 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/test_demos.py
+-rw-r--r--   0     1001      127     5592 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/demos/sim_manager_demo.py
+-rw-r--r--   0     1001      127      386 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/plot.py
+-rw-r--r--   0     1001      127     2074 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/defaults.py
+-rw-r--r--   0     1001      127    52841 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/output_12072022.csv
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/loaders/__init__.py
+-rw-r--r--   0     1001      127     3448 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/loaders/powertrain_components.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/py.typed
+-rw-r--r--   0     1001      127    53858 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/train_planner.py
+-rw-r--r--   0     1001      127      766 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/stringline_old.py
+-rw-r--r--   0     1001      127    41804 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/metric_calculator.py
+-rw-r--r--   0     1001      127    16755 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/stringline.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/fuel_grid.py
+-rw-r--r--   0     1001      127     5693 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/sim_manager.py
+-rw-r--r--   0     1001      127    29495 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/altrios_pyo3.pyi
+-rw-r--r--   0     1001      127     6896 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/rollout.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/user_interface.py
+-rw-r--r--   0     1001      127     1754 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_powertrain_res.py
+-rw-r--r--   0     1001      127     1279 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_powertrain_fuel_conv.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_multi_obj_opt.py
+-rw-r--r--   0     1001      127      689 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_locomotive_simulation.py
+-rw-r--r--   0     1001      127      928 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_metric_calculator.py
+-rw-r--r--   0     1001      127      603 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_consist.py
+-rw-r--r--   0     1001      127     2351 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_multi_obj_cal_and_val.py
+-rw-r--r--   0     1001      127      386 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_train_simulation.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_objectives.py
+-rw-r--r--   0     1001      127        0 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_fuel_grid.py
+-rw-r--r--   0     1001      127      675 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_consist_sim.py
+-rw-r--r--   0     1001      127      747 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_powertrain_generator.py
+-rw-r--r--   0     1001      127     1019 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_utilities.py
+-rw-r--r--   0     1001      127      229 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_train_planner.py
+-rw-r--r--   0     1001      127     1533 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_locomotive.py
+-rw-r--r--   0     1001      127      874 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_powertrain_edrive.py
+-rw-r--r--   0     1001      127     7941 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/mock_resources.py
+-rw-r--r--   0     1001      127      652 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/tests/test_rail_vehicles.py
+-rw-r--r--   0     1001      127       25 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/optimization/__init__.py
+-rw-r--r--   0     1001      127    24477 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/optimization/cal_and_val.py
+-rw-r--r--   0     1001      127       91 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/optimization/multi_obj_opt.py
+-rw-r--r--   0     1001      127     8741 2024-04-04 17:55:26.000000 altrios-0.2.0/python/altrios/utilities.py
+-rw-r--r--   0     1001      127     7492 2024-04-04 17:55:26.000000 altrios-0.2.0/README.md
+-rw-r--r--   0     1001      127     1660 2024-04-04 17:55:26.000000 altrios-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     9102 1970-01-01 00:00:00.000000 altrios-0.2.0/PKG-INFO
```

### Comparing `altrios-0.1.8/rust/altrios-core/Cargo.toml` & `altrios-0.2.0/rust/altrios-core/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [package]
 name = "altrios-core"
 authors = { workspace = true }
 edition = { workspace = true }
 license = { workspace = true }
 homepage = { workspace = true }
 repository = { workspace = true }
-version = "0.1.5"
+version = "0.1.7"
 description = "ALTRIOS Core model for train simulation"
 readme = "README.md"
 
 [dependencies]
 csv = "1.1.6"
 serde = { version = "1.0.136", features = ["derive"] }
 serde_yaml = "0.8.23"
 serde_json = "1.0"
 uom = { workspace = true }
 paste = "1.0.7"
 easy-ext = "1.0.0"
 altrios-proc-macros = { version = "0.1.5", path = "altrios-proc-macros" }
 argmin = "0.5.1"
-enum_dispatch = "0.3.8"
 rayon = "1.5.3"
 bincode = "1.3.3"
 log = "0.4.17"
 anyhow = { workspace = true }
 readonly = "0.2.3"
 duplicate = "0.4.1"
 nohash-hasher = "0.2.0"
```

### Comparing `altrios-0.1.8/rust/altrios-core/README.md` & `altrios-0.2.0/rust/altrios-core/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/combo_error.rs` & `altrios-0.2.0/rust/altrios-core/src/combo_error.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/consist_model.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/consist_model.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/consist_sim.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/consist_sim.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/consist_utils.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/consist_utils.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-use super::locomotive::{BatteryElectricLoco, ConventionalLoco, DummyLoco, HybridLoco};
 use super::*;
 
 /// Trait for ensuring consistency among locomotives and consists
-#[enum_dispatch]
 pub trait LocoTrait {
     /// returns current max power, current max power rate, and current max regen
     /// power that can be absorbed by the RES/battery
     fn set_cur_pwr_max_out(
         &mut self,
         pwr_aux: Option<si::Power>,
         dt: si::Time,
@@ -24,15 +22,14 @@
 }
 
 #[altrios_api]
 #[derive(Default, Serialize, Deserialize, Clone, PartialEq, SerdeAPI)]
 /// Wrapper struct for `Vec<Locomotive>` to expose various methods to Python.
 pub struct Pyo3VecLocoWrapper(pub Vec<Locomotive>);
 
-#[enum_dispatch]
 pub trait SolvePower {
     /// Returns vector of locomotive tractive powers during positive traction events
     fn solve_positive_traction(
         &mut self,
         loco_vec: &[Locomotive],
         state: &ConsistState,
     ) -> anyhow::Result<Vec<si::Power>>;
@@ -261,20 +258,48 @@
         _state: &ConsistState,
     ) -> anyhow::Result<Vec<si::Power>> {
         todo!() // not needed urgently
     }
 }
 /// Variants of this enum are used to determine what control strategy gets used for distributing
 /// power required from or delivered to during negative tractive power each locomotive.
-#[enum_dispatch(SolvePower)]
 #[derive(PartialEq, Clone, Deserialize, Serialize, Debug, SerdeAPI)]
 pub enum PowerDistributionControlType {
-    RESGreedy,
-    Proportional,
-    GoldenSectionSearch,
-    FrontAndBack,
+    RESGreedy(RESGreedy),
+    Proportional(Proportional),
+    GoldenSectionSearch(GoldenSectionSearch),
+    FrontAndBack(FrontAndBack),
 }
+
+impl SolvePower for PowerDistributionControlType {
+    fn solve_negative_traction(
+        &mut self,
+        loco_vec: &[Locomotive],
+        state: &ConsistState,
+    ) -> anyhow::Result<Vec<si::Power>> {
+        match self {
+            Self::RESGreedy(res_greedy) => res_greedy.solve_negative_traction(loco_vec, state),
+            Self::Proportional(prop) => prop.solve_negative_traction(loco_vec, state),
+            Self::GoldenSectionSearch(gss) => gss.solve_negative_traction(loco_vec, state),
+            Self::FrontAndBack(fab) => fab.solve_negative_traction(loco_vec, state),
+        }
+    }
+
+    fn solve_positive_traction(
+        &mut self,
+        loco_vec: &[Locomotive],
+        state: &ConsistState,
+    ) -> anyhow::Result<Vec<si::Power>> {
+        match self {
+            Self::RESGreedy(res_greedy) => res_greedy.solve_positive_traction(loco_vec, state),
+            Self::Proportional(prop) => prop.solve_positive_traction(loco_vec, state),
+            Self::GoldenSectionSearch(gss) => gss.solve_positive_traction(loco_vec, state),
+            Self::FrontAndBack(fab) => fab.solve_positive_traction(loco_vec, state),
+        }
+    }
+}
+
 impl Default for PowerDistributionControlType {
     fn default() -> Self {
         Self::RESGreedy(RESGreedy)
     }
 }
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/battery_electric_loco.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/conventional_loco.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/conventional_loco.rs`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         &mut self,
         pwr_aux: Option<si::Power>,
         dt: si::Time,
     ) -> anyhow::Result<()> {
         self.fc.set_cur_pwr_out_max(dt)?;
         self.gen.set_cur_pwr_max_out(
             self.fc.state.pwr_out_max,
-            Some(pwr_aux.ok_or(anyhow!(format_dbg!("`pwr_aux` not provided")))?),
+            Some(pwr_aux.with_context(|| format_dbg!("`pwr_aux` not provided"))?),
         )?;
         self.edrv
             .set_cur_pwr_max_out(self.gen.state.pwr_elec_prop_out_max, None)?;
         self.gen
             .set_pwr_rate_out_max(self.fc.pwr_out_max / self.fc.pwr_ramp_lag);
         self.edrv
             .set_pwr_rate_out_max(self.gen.state.pwr_rate_out_max);
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/hybrid_loco.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/loco_sim.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/loco_sim.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/locomotive_model.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/locomotive_model.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,87 @@
 use super::*;
 
-#[enum_dispatch(LocoTrait)]
 #[derive(Clone, Debug, Serialize, Deserialize, PartialEq, SerdeAPI)]
 pub enum PowertrainType {
-    ConventionalLoco,
+    ConventionalLoco(ConventionalLoco),
     HybridLoco(Box<HybridLoco>),
-    BatteryElectricLoco,
-    DummyLoco,
+    BatteryElectricLoco(BatteryElectricLoco),
+    DummyLoco(DummyLoco),
+}
+
+impl LocoTrait for PowertrainType {
+    fn set_cur_pwr_max_out(
+        &mut self,
+        pwr_aux: Option<si::Power>,
+        dt: si::Time,
+    ) -> anyhow::Result<()> {
+        match self {
+            PowertrainType::ConventionalLoco(conv) => conv.set_cur_pwr_max_out(pwr_aux, dt),
+            PowertrainType::HybridLoco(hel) => hel.set_cur_pwr_max_out(pwr_aux, dt),
+            PowertrainType::BatteryElectricLoco(bel) => bel.set_cur_pwr_max_out(pwr_aux, dt),
+            PowertrainType::DummyLoco(dummy) => dummy.set_cur_pwr_max_out(pwr_aux, dt),
+        }
+    }
+
+    fn save_state(&mut self) {
+        match self {
+            PowertrainType::ConventionalLoco(conv) => conv.save_state(),
+            PowertrainType::HybridLoco(hel) => hel.save_state(),
+            PowertrainType::BatteryElectricLoco(bel) => bel.save_state(),
+            PowertrainType::DummyLoco(dummy) => dummy.save_state(),
+        }
+    }
+
+    fn step(&mut self) {
+        match self {
+            PowertrainType::ConventionalLoco(conv) => conv.step(),
+            PowertrainType::HybridLoco(hel) => hel.step(),
+            PowertrainType::BatteryElectricLoco(bel) => bel.step(),
+            PowertrainType::DummyLoco(dummy) => dummy.step(),
+        }
+    }
+
+    fn get_energy_loss(&self) -> si::Energy {
+        match self {
+            PowertrainType::ConventionalLoco(conv) => conv.get_energy_loss(),
+            PowertrainType::HybridLoco(hel) => hel.get_energy_loss(),
+            PowertrainType::BatteryElectricLoco(bel) => bel.get_energy_loss(),
+            PowertrainType::DummyLoco(dummy) => dummy.get_energy_loss(),
+        }
+    }
+}
+
+impl From<ConventionalLoco> for PowertrainType {
+    fn from(value: ConventionalLoco) -> Self {
+        Self::ConventionalLoco(value)
+    }
 }
 
 impl From<HybridLoco> for PowertrainType {
     fn from(value: HybridLoco) -> Self {
-        Self::from(Box::new(value))
+        Self::HybridLoco(Box::new(value))
+    }
+}
+
+impl From<BatteryElectricLoco> for PowertrainType {
+    fn from(value: BatteryElectricLoco) -> Self {
+        Self::BatteryElectricLoco(value)
+    }
+}
+
+impl From<DummyLoco> for PowertrainType {
+    fn from(value: DummyLoco) -> Self {
+        Self::DummyLoco(value)
     }
 }
 
 #[cfg(feature = "pyo3")]
 impl TryFrom<&PyAny> for PowertrainType {
     type Error = PyErr;
-    /// This allows us to construct PowertrainType any struct that can be converted into PowertrainType
+    /// This allows us to construct PowertrainType from any struct that can be converted into PowertrainType
     fn try_from(value: &PyAny) -> std::result::Result<Self, Self::Error> {
         value
             .extract::<ConventionalLoco>()
             .map(PowertrainType::from)
             .or_else(|_| {
                 value
                     .extract::<HybridLoco>()
@@ -92,14 +151,15 @@
     pub force_max: si::Force,
     #[api(skip_get, skip_set)]
     /// [Locomotive::mass]
     pub mass: Option<si::Mass>,
 }
 
 impl LocoParams {
+    #[allow(unused)]
     fn from_hash(mut params: HashMap<&str, f64>) -> anyhow::Result<Self> {
         let pwr_aux_offset_watts = params
             .remove("pwr_aux_offset_watts")
             .ok_or_else(|| anyhow!("Must provide 'pwr_aux_offset_watts'."))?;
         let pwr_aux_traction_coeff_ratio = params
             .remove("pwr_aux_traction_coeff_ratio")
             .ok_or_else(|| anyhow!("Must provide 'pwr_aux_traction_coeff_ratio'."))?;
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/electric_drivetrain.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/fuel_converter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,15 @@
     #[serde(rename = "pwr_out_max_watts")]
     /// max rated brake output power
     pub pwr_out_max: si::Power,
     /// starting/baseline transient power limit
     #[serde(default)]
     pub pwr_out_max_init: si::Power,
     // TODO: consider a ramp down rate, which may be needed for fuel cells
-    #[serde(rename(
-        serialize = "pwr_ramp_lag_seconds",
-        deserialize = "pwr_ramp_lag_seconds"
-    ))]
+    #[serde(rename = "pwr_ramp_lag_seconds")]
     /// lag time for ramp up
     pub pwr_ramp_lag: si::Time,
     /// Fuel converter brake power fraction array at which efficiencies are evaluated.
     /// This fuel converter efficiency model assumes that speed and load (or voltage and current) will
     /// always be controlled for operating at max possible efficiency for the power demand
     pub pwr_out_frac_interp: Vec<f64>,
     /// fuel converter efficiency array
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/generator.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/powertrain_traits.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.default.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/powertrain/reversible_energy_storage.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/locomotive/tests.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/locomotive/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/consist/tests.rs` & `altrios-0.2.0/rust/altrios-core/src/consist/tests.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/imports.rs` & `altrios-0.2.0/rust/altrios-core/src/imports.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 pub(crate) use crate::utils::{almost_eq, interp1d, interp3d, is_sorted, DIRECT_SET_ERR};
 pub(crate) use crate::utils::{Pyo3Vec2Wrapper, Pyo3Vec3Wrapper, Pyo3VecWrapper};
 pub(crate) use crate::validate::*;
 pub(crate) use altrios_proc_macros::{altrios_api, HistoryMethods, HistoryVec, SerdeAPI};
 
 pub(crate) use duplicate::duplicate_item;
 pub(crate) use easy_ext::ext;
-pub(crate) use enum_dispatch::enum_dispatch;
 
 pub(crate) use bincode::{deserialize, serialize};
 pub(crate) use serde::{Deserialize, Serialize};
 pub(crate) use std::cmp::{self, Ordering};
 pub(crate) use std::collections::{BinaryHeap, HashMap, HashSet, VecDeque};
 pub(crate) use std::error::Error;
 pub(crate) use std::ffi::OsStr;
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/lib.rs` & `altrios-0.2.0/rust/altrios-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/lin_search_hint.rs` & `altrios-0.2.0/rust/altrios-core/src/lin_search_hint.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/macros.rs` & `altrios-0.2.0/rust/altrios-core/src/macros.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/disp_structs.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/disp_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/dispatch.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/dispatch.rs`

 * *Files 1% similar despite different names*

```diff
@@ -299,16 +299,15 @@
         assert!(output.is_empty());
     }
 
     #[test]
     fn test_simple_dispatch() {
         let mut network_file_path = project_root::get_project_root().unwrap();
         network_file_path.push("../python/altrios/resources/networks/Taconite.yaml");
-        let network =
-            Vec::<Link>::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
+        let network = Network::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
         network.validate().unwrap();
 
         let train_sims = vec![
             crate::train::speed_limit_train_sim_fwd(),
             crate::train::speed_limit_train_sim_rev(),
         ];
         // &vec![
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/est_time_structs.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -736,25 +736,14 @@
                 || idx == est_times.len() - 1
         );
     }
 
     update_times_forward(&mut est_times, time_depart);
     update_times_backward(&mut est_times);
 
-    // TODO: Write complete network validation function!
-    // This could entail (some may already be complete):
-    // - [ ] checking that final offset in each vec is same as Link length
-    // - [ ] checking that starting offset in each vec is zero
-    // - [ ] checking that reverse-forward nodal symmetry is correct
-    // - [ ] check graph structure consistency
-    // - [ ] verify that link headind and elevation actually meet up reasonably (with some tolerance)
-    //   for adjecent links
-    // - [x] check that `idx_*` and `idx_*_alt` are different unless both are zero
-    // - [ ] ???
-
     let est_time_net = EstTimeNet::new(est_times);
     ensure!(
         !est_time_net.val.iter().all(|x| x.time_sched == 0. * uc::S),
         "All times are 0.0 so something went wrong.\n{}",
         format_dbg!()
     );
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/est_times/update_times.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/est_times/update_times.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/advance_rewind.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/free_path.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/free_path.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/meet_pass/train_disp/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/meet_pass/train_disp/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -218,16 +218,15 @@
 mod test_train_disp {
     use super::*;
 
     #[test]
     fn test_make_train_fwd() {
         let mut network_file_path = project_root::get_project_root().unwrap();
         network_file_path.push("../python/altrios/resources/networks/Taconite.yaml");
-        let network =
-            Vec::<Link>::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
+        let network = Network::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
         network.validate().unwrap();
 
         let speed_limit_train_sim = crate::train::speed_limit_train_sim_fwd();
         let est_times = make_est_times(&speed_limit_train_sim, &network).unwrap().0;
         TrainDisp::new(
             speed_limit_train_sim.train_id.clone(),
             NonZeroU16::new(1),
@@ -242,16 +241,15 @@
     }
 
     #[test]
     fn test_make_train_rev() {
         // TODO: Make this test depend on a better file
         let mut network_file_path = project_root::get_project_root().unwrap();
         network_file_path.push("../python/altrios/resources/networks/Taconite.yaml");
-        let network =
-            Vec::<Link>::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
+        let network = Network::from_file(network_file_path.as_os_str().to_str().unwrap()).unwrap();
 
         network.validate().unwrap();
         let speed_limit_train_sim = crate::train::speed_limit_train_sim_rev();
         let est_times = make_est_times(&speed_limit_train_sim, &network).unwrap().0;
         TrainDisp::new(
             speed_limit_train_sim.train_id.clone(),
             NonZeroU16::new(1),
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/prelude.rs` & `altrios-0.2.0/rust/altrios-core/src/prelude.rs`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 pub use crate::utils::{Pyo3Vec2Wrapper, Pyo3Vec3Wrapper, Pyo3VecBoolWrapper, Pyo3VecWrapper};
 
 #[cfg(feature = "pyo3")]
 pub use crate::meet_pass::{
     dispatch::run_dispatch_py, est_times::check_od_pair_valid, est_times::make_est_times_py,
 };
 #[cfg(feature = "pyo3")]
-pub use crate::track::{import_locations_py, import_network_py};
+pub use crate::track::import_locations_py;
 #[cfg(feature = "pyo3")]
 pub use crate::train::{
     build_speed_limit_train_sims, import_rail_vehicles_py, run_speed_limit_train_sims,
 };
 
 pub use crate::meet_pass::est_times::{make_est_times, EstTimeNet};
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/si.rs` & `altrios-0.2.0/rust/altrios-core/src/si.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/testing.rs` & `altrios-0.2.0/rust/altrios-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/cat_power.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/cat_power.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/elev.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/elev.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/heading.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/heading.rs`

 * *Files 22% similar despite different names*

```diff
@@ -4,14 +4,26 @@
 #[derive(Clone, Copy, Default, Debug, PartialEq, PartialOrd, Serialize, Deserialize, SerdeAPI)]
 #[altrios_api]
 pub struct Heading {
     #[api(skip_set)]
     pub offset: si::Length,
     #[api(skip_set)]
     pub heading: si::Angle,
+    /// Optional latitude at `self.offset`.  No checks are currently performed to ensure consistency
+    /// between headind and lat/lon, and this is not actually used in the code.  
+    #[api(skip_set)]
+    #[serde(rename = "Lat")]
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub lat: Option<f64>,
+    /// Optional longitude at `self.offset`.  No checks are currently performed to ensure
+    /// consistency between headind and lat/lon, and this is not actually used in the code.
+    #[api(skip_set)]
+    #[serde(rename = "Lon")]
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub lon: Option<f64>,
 }
 
 impl Valid for Heading {}
 
 impl ObjState for Heading {
     fn validate(&self) -> ValidationResults {
         let mut errors = ValidationErrors::new();
@@ -31,18 +43,22 @@
     fn valid() -> Self {
         let offset_end = uc::M * 10000.0;
         vec![
             Heading::valid(),
             Heading {
                 offset: offset_end * 0.5,
                 heading: si::Angle::ZERO,
+                lat: Default::default(),
+                lon: Default::default(),
             },
             Heading {
                 offset: offset_end,
                 heading: uc::RAD,
+                lat: Default::default(),
+                lon: Default::default(),
             },
         ]
     }
 }
 
 impl ObjState for [Heading] {
     fn is_fake(&self) -> bool {
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/link_idx.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/link_idx.rs`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         } else {
             Ok(Self(lp))
         }
     }
 
     /// Load from csv file
     pub fn to_csv_file<P: AsRef<Path>>(&self, filepath: P) -> anyhow::Result<()> {
-        let file = File::open(filepath)?;
+        let file = std::fs::OpenOptions::new().write(true).open(filepath)?;
         let mut wrtr = csv::WriterBuilder::new()
             .has_headers(true)
             .from_writer(file);
         for elem in &self.0 {
             wrtr.serialize(elem)?;
         }
         wrtr.flush()?;
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/link_impl.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/link_impl.rs`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     /// if it does not exist, it should be `LinkIdx{idx: 0}`
     pub idx_next_alt: LinkIdx,
     /// see [EstTime::idx_prev]
     pub idx_prev: LinkIdx,
     /// see [EstTime::idx_prev_alt]  
     /// if it does not exist, it should be `LinkIdx{idx: 0}`
     pub idx_prev_alt: LinkIdx,
+    /// Optional OpenStreetMap ID -- not used in simulation
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub osm_id: Option<String>,
 
     /// Spatial vector of elevation values and corresponding positions along track
     pub elevs: Vec<Elev>,
     #[serde(default)]
     /// Spatial vector of compass heading values and corresponding positions along track
     pub headings: Vec<Heading>,
     /// Map of train types and corresponding speed sets
@@ -40,14 +43,19 @@
     pub speed_set: Option<SpeedSet>,
     #[serde(default)]
     /// Spatial vector of catenary power limit values and corresponding positions along track
     pub cat_power_limits: Vec<CatPowerLimit>,
     pub length: si::Length,
 
     #[serde(default)]
+    /// Prevents provided links from being occupied when the current link has a train on it. An
+    /// example would be at a switch, where there would be foul links running from the switch points
+    /// to the clearance point. Due to the geometric overlap of the foul links, only one may be
+    /// occupied at a given time. For further explanation, see the [graphical
+    /// example](https://nrel.github.io/altrios/api-doc/rail-network.html?highlight=network#link-lockout).
     pub link_idxs_lockout: Vec<LinkIdx>,
 }
 
 impl Link {
     fn is_linked_prev(&self, idx: LinkIdx) -> bool {
         self.idx_curr.is_fake() || self.idx_prev == idx || self.idx_prev_alt == idx
     }
@@ -79,14 +87,15 @@
             length: l.length,
             idx_next: l.idx_next,
             idx_next_alt: l.idx_next_alt,
             idx_prev: l.idx_prev,
             idx_prev_alt: l.idx_prev_alt,
             idx_curr: l.idx_curr,
             idx_flip: l.idx_flip,
+            osm_id: l.osm_id,
             link_idxs_lockout: l.link_idxs_lockout,
         }
     }
 }
 
 impl Valid for Link {
     fn valid() -> Self {
@@ -128,15 +137,22 @@
             }
         } else {
             si_chk_num_gtz(&mut errors, &self.length, "Link length");
             validate_field_real(&mut errors, &self.elevs, "Elevations");
             if !self.headings.is_empty() {
                 validate_field_real(&mut errors, &self.headings, "Headings");
             }
-            validate_field_real(&mut errors, &self.speed_sets, "Speed sets");
+            match &self.speed_set {
+                Some(speed_set) => {
+                    validate_field_real(&mut errors, speed_set, "Speed sets");
+                }
+                None => {
+                    validate_field_real(&mut errors, &self.speed_sets, "Speed sets");
+                }
+            }
             validate_field_real(&mut errors, &self.cat_power_limits, "Catenary power limits");
 
             early_err!(errors, "Link");
 
             if self.idx_flip.is_real() {
                 for (var, name) in [
                     (self.idx_curr, "curr"),
@@ -166,42 +182,48 @@
                 errors.push(anyhow!(
                     "Link index prev = {:?} must be real when link index prev alt = {:?} is real!",
                     self.idx_prev,
                     self.idx_prev_alt
                 ));
             }
 
+            // verify that first offset is zero
             if self.elevs.first().unwrap().offset != si::Length::ZERO {
                 errors.push(anyhow!(
                     "First elevation offset = {:?} is invalid, must equal zero!",
                     self.elevs.first().unwrap().offset
                 ));
             }
+            // verify that last offset is equal to length
             if self.elevs.last().unwrap().offset != self.length {
                 errors.push(anyhow!(
                     "Last elevation offset = {:?} is invalid, must equal length = {:?}!",
                     self.elevs.last().unwrap().offset,
                     self.length
                 ));
             }
             if !self.headings.is_empty() {
+                // verify that first offset is zero
                 if self.headings.first().unwrap().offset != si::Length::ZERO {
                     errors.push(anyhow!(
                         "First heading offset = {:?} is invalid, must equal zero!",
                         self.headings.first().unwrap().offset
                     ));
                 }
+                // verify that last offset is equal to length
                 if self.headings.last().unwrap().offset != self.length {
                     errors.push(anyhow!(
                         "Last heading offset = {:?} is invalid, must equal length = {:?}!",
                         self.headings.last().unwrap().offset,
                         self.length
                     ));
                 }
             }
+            // if cat power limits are not specified for entire length of link, assume that no cat
+            // power is available
             if !self.cat_power_limits.is_empty() {
                 if self.cat_power_limits.first().unwrap().offset_start < si::Length::ZERO {
                     errors.push(anyhow!(
                         "First cat power limit offset start = {:?} is invalid, must be greater than or equal to zero!",
                         self.cat_power_limits.first().unwrap().offset_start
                     ));
                 }
@@ -220,38 +242,54 @@
 
 #[altrios_api]
 #[derive(Debug, Default, Clone, PartialEq, Serialize, Deserialize)]
 /// Struct that contains a `Vec<Link>` for the purpose of providing `SerdeAPI` for `Vec<Link>` in
 /// Python
 pub struct Network(pub Vec<Link>);
 
+impl ObjState for Network {
+    fn is_fake(&self) -> bool {
+        self.0.is_fake()
+    }
+    fn validate(&self) -> ValidationResults {
+        self.0.validate()
+    }
+}
+
 impl SerdeAPI for Network {
     fn from_file<P: AsRef<Path>>(filepath: P) -> anyhow::Result<Self> {
         let filepath = filepath.as_ref();
         let extension = filepath
             .extension()
             .and_then(OsStr::to_str)
             .with_context(|| format!("File extension could not be parsed: {filepath:?}"))?;
         let file = File::open(filepath).with_context(|| {
             if !filepath.exists() {
                 format!("File not found: {filepath:?}")
             } else {
                 format!("Could not open file: {filepath:?}")
             }
         })?;
-        match Self::from_reader(file, extension) {
-            Ok(network) => Ok(network),
-            Err(err) => Ok(NetworkOld::from_file(filepath).with_context(|| err)?.into()),
-        }
+        let mut network = match Self::from_reader(file, extension) {
+            Ok(network) => network,
+            Err(err) => NetworkOld::from_file(filepath).with_context(|| err)?.into(),
+        };
+        network.init()?;
+
+        Ok(network)
+    }
+
+    fn init(&mut self) -> anyhow::Result<()> {
+        Ok(self.as_ref().validate()?)
     }
 }
 
 impl From<NetworkOld> for Network {
-    fn from(value: NetworkOld) -> Self {
-        Network(value.0.iter().map(|l| Link::from(l.clone())).collect())
+    fn from(old: NetworkOld) -> Self {
+        Network(old.0.iter().map(|l| Link::from(l.clone())).collect())
     }
 }
 
 #[altrios_api]
 #[derive(Debug, Default, Clone, PartialEq, Serialize, Deserialize, SerdeAPI)]
 /// Struct that contains a `Vec<Link>` for the purpose of providing `SerdeAPI` for `Vec<Link>` in
 /// Python
@@ -268,22 +306,14 @@
 
 impl From<&Vec<Link>> for Network {
     fn from(value: &Vec<Link>) -> Self {
         Self(value.to_vec())
     }
 }
 
-#[cfg(feature = "pyo3")]
-#[cfg_attr(feature = "pyo3", pyfunction(name = "import_network"))]
-pub fn import_network_py(filepath: &PyAny) -> anyhow::Result<Vec<Link>> {
-    let network = Vec::<Link>::from_file(PathBuf::extract(filepath)?)?;
-    network.validate()?;
-    Ok(network)
-}
-
 impl Valid for Vec<Link> {
     fn valid() -> Self {
         vec![Link::default(), Link::valid()]
     }
 }
 
 impl ObjState for [Link] {
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/link_old.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/link_old.rs`

 * *Files 20% similar despite different names*

```diff
@@ -32,10 +32,13 @@
     /// see [EstTime::idx_prev_alt]  
     /// if it does not exist, it should be `LinkIdx{idx: 0}`
     pub idx_prev_alt: LinkIdx,
     /// Index of current link
     pub idx_curr: LinkIdx,
     /// Index of adjacent link in reverse direction
     pub idx_flip: LinkIdx,
+    /// Optional OpenStreetMap ID -- not used in simulation
+    #[serde(skip_serializing_if = "Option::is_none")]
+    pub osm_id: Option<String>,
     #[serde(default)]
     pub link_idxs_lockout: Vec<LinkIdx>,
 }
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/location.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/location.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_limit.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_limit.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_param.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_param.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/link/speed/speed_set.rs` & `altrios-0.2.0/rust/altrios-core/src/track/link/speed/speed_set.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/path_track/link_point.rs` & `altrios-0.2.0/rust/altrios-core/src/track/path_track/link_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/path_track/path_res_coeff.rs` & `altrios-0.2.0/rust/altrios-core/src/track/path_track/path_res_coeff.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/path_track/path_tpc.rs` & `altrios-0.2.0/rust/altrios-core/src/track/path_track/path_tpc.rs`

 * *Files 1% similar despite different names*

```diff
@@ -367,29 +367,29 @@
             }
         }
         Ok(())
     }
 }
 
 /// If provided, returns `speed_set`.  Otherwise, finds speed_set appropriate for
-/// `train_params.train_type
+/// `train_params.train_type`
 fn extract_speed_set<'a>(
     speed_sets: &'a HashMap<TrainType, SpeedSet>,
     speed_set: &'a Option<SpeedSet>,
     train_params: &'a TrainParams,
 ) -> Result<&'a SpeedSet, argmin::prelude::Error> {
     let speed_set = match speed_set {
         Some(s) => s,
         None => {
             speed_sets
                 .iter()
                 .find(|&sps| sps.0 == &train_params.train_type)
                 .ok_or_else(|| {
                     anyhow!(
-                        "`train_params.train_type` {:?} not found in `speed_sets.keys()` {:?}",
+                        "`speed_set` is `None` and `train_params.train_type` {:?} not found in `speed_sets.keys()` {:?}",
                         train_params.train_type,
                         speed_sets.keys()
                     )
                 })?
                 .1
         }
     };
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/path_track/speed_point.rs` & `altrios-0.2.0/rust/altrios-core/src/track/path_track/speed_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/track/path_track/train_params.rs` & `altrios-0.2.0/rust/altrios-core/src/track/path_track/train_params.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/braking_point.rs` & `altrios-0.2.0/rust/altrios-core/src/train/braking_point.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/friction_brakes.rs` & `altrios-0.2.0/rust/altrios-core/src/train/friction_brakes.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/rail_vehicle.rs` & `altrios-0.2.0/rust/altrios-core/src/train/rail_vehicle.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs` & `altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/aerodynamic.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/resistance/kind/path_res.rs` & `altrios-0.2.0/rust/altrios-core/src/train/resistance/kind/path_res.rs`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,38 @@
 }
 impl Point {
     pub fn new(vals: &[PathResCoeff], state: &TrainState) -> anyhow::Result<Self> {
         Ok(Self {
             idx: vals.calc_idx(state.offset - state.length * 0.5, 0, &Dir::Fwd)?,
         })
     }
+
     pub fn calc_res(
         &mut self,
         vals: &[PathResCoeff],
         state: &TrainState,
         dir: &Dir,
     ) -> anyhow::Result<si::Force> {
         self.idx = vals.calc_idx(state.offset - state.length * 0.5, self.idx, dir)?;
         Ok(calc_res_val(vals[self.idx].res_coeff, state))
     }
+
     pub fn res_coeff_front(&self, vals: &[PathResCoeff]) -> si::Ratio {
         vals[self.idx].res_coeff
     }
+
     pub fn res_net_front(&self, vals: &[PathResCoeff], state: &TrainState) -> si::Length {
         vals[self.idx].calc_res_val(state.offset)
     }
+
+    /// Returns index of current element containing front of train within `PathTPC`
+    pub fn path_tpc_idx_front(&self) -> usize {
+        self.idx
+    }
+
     pub fn fix_cache(&mut self, idx_sub: usize) {
         self.idx -= idx_sub;
     }
 }
 
 #[ext(CalcResStrap)]
 impl [PathResCoeff] {
@@ -104,15 +113,22 @@
         };
 
         Ok(calc_res_val(res_coeff, state))
     }
     pub fn res_coeff_front(&self, vals: &[PathResCoeff]) -> si::Ratio {
         vals[self.idx_front].res_coeff
     }
+
     pub fn res_net_front(&self, vals: &[PathResCoeff], state: &TrainState) -> si::Length {
         vals[self.idx_front].calc_res_val(state.offset)
     }
+
+    /// Returns index of current element containing front of train within `PathTPC`
+    pub fn path_tpc_idx_front(&self) -> usize {
+        self.idx_front
+    }
+
     pub fn fix_cache(&mut self, idx_sub: usize) {
         self.idx_back -= idx_sub;
         self.idx_front -= idx_sub;
     }
 }
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/resistance/method/point.rs` & `altrios-0.2.0/rust/altrios-core/src/train/resistance/method/point.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use super::super::kind::*;
 use super::super::ResMethod;
+use super::*;
 use crate::imports::*;
-use crate::track::{LinkPoint, PathResCoeff, PathTpc};
-use crate::train::TrainState;
+use crate::track::{LinkPoint, PathResCoeff};
 
 #[altrios_api]
 #[derive(Debug, Clone, Serialize, Deserialize, Default, PartialEq, SerdeAPI)]
 pub struct Point {
     bearing: bearing::Basic,
     rolling: rolling::Basic,
     davis_b: davis_b::Basic,
@@ -28,22 +28,24 @@
         state.res_rolling = self.rolling.calc_res(state);
         state.res_davis_b = self.davis_b.calc_res(state);
         state.res_aero = self.aerodynamic.calc_res(state);
         state.res_grade = self.grade.calc_res(path_tpc.grades(), state, dir)?;
         state.res_curve = self.curve.calc_res(path_tpc.curves(), state, dir)?;
         state.grade_front = self.grade.res_coeff_front(path_tpc.grades());
         state.elev_front = self.grade.res_net_front(path_tpc.grades(), state);
+
         Ok(())
     }
 
     fn fix_cache(&mut self, link_point_del: &LinkPoint) {
         self.grade.fix_cache(link_point_del.grade_count);
         self.curve.fix_cache(link_point_del.curve_count);
     }
 }
+
 impl Valid for Point {
     fn valid() -> Self {
         Self {
             bearing: bearing::Basic::new(40.0 * 100.0 * uc::LBF),
             rolling: rolling::Basic::new(1.5 * uc::LB / uc::TON),
             davis_b: davis_b::Basic::new(0.03 / uc::MPH * uc::LB / uc::TON),
             aerodynamic: aerodynamic::Basic::new(
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/resistance/method/strap.rs` & `altrios-0.2.0/rust/altrios-core/src/train/resistance/method/strap.rs`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
         state.res_aero = self.aerodynamic.calc_res(state);
         state.res_grade = self.grade.calc_res(path_tpc.grades(), state, dir)?;
         state.res_curve = self.curve.calc_res(path_tpc.curves(), state, dir)?;
         state.grade_front = self.grade.res_coeff_front(path_tpc.grades());
         state.elev_front = self.grade.res_net_front(path_tpc.grades(), state);
         Ok(())
     }
+
     fn fix_cache(&mut self, link_point_del: &LinkPoint) {
         self.grade.fix_cache(link_point_del.grade_count);
         self.curve.fix_cache(link_point_del.curve_count);
     }
 }
 impl Valid for Strap {
     fn valid() -> Self {
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/resistance/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/train/resistance/mod.rs`

 * *Files 17% similar despite different names*

```diff
@@ -2,35 +2,53 @@
 pub mod method;
 
 use crate::imports::*;
 use crate::track::LinkPoint;
 use crate::track::PathTpc;
 use crate::train::TrainState;
 
-#[enum_dispatch]
 pub trait ResMethod {
     fn update_res(
         &mut self,
         state: &mut TrainState,
         path_tpc: &PathTpc,
         dir: &Dir,
     ) -> anyhow::Result<()>;
     fn fix_cache(&mut self, link_point_del: &LinkPoint);
 }
 
 /// Train resistance calculator that calculates resistive powers due to rolling, curvature, flange,
 /// grade, and bearing resistances.  
 // TODO: May also include inertial -- figure this out and modify doc string above
-#[enum_dispatch(ResMethod)]
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq, SerdeAPI)]
 pub enum TrainRes {
     Point(method::Point),
     Strap(method::Strap),
 }
 
+impl ResMethod for TrainRes {
+    fn update_res(
+        &mut self,
+        state: &mut TrainState,
+        path_tpc: &PathTpc,
+        dir: &Dir,
+    ) -> anyhow::Result<()> {
+        match self {
+            TrainRes::Point(p) => p.update_res(state, path_tpc, dir),
+            TrainRes::Strap(s) => s.update_res(state, path_tpc, dir),
+        }
+    }
+    fn fix_cache(&mut self, link_point_del: &LinkPoint) {
+        match self {
+            TrainRes::Point(p) => p.fix_cache(link_point_del),
+            TrainRes::Strap(s) => s.fix_cache(link_point_del),
+        }
+    }
+}
+
 impl Default for TrainRes {
     fn default() -> Self {
         Self::Strap(method::Strap::default())
     }
 }
 
 impl Valid for TrainRes {
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/set_speed_train_sim.rs` & `altrios-0.2.0/rust/altrios-core/src/train/set_speed_train_sim.rs`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,19 @@
     fn from_csv_file_py(filepath: &PyAny) -> anyhow::Result<Self> {
         Self::from_csv_file(PathBuf::extract(filepath)?)
     }
 
     fn __len__(&self) -> usize {
         self.len()
     }
+
+    #[pyo3(name = "to_csv_file")]
+    fn to_csv_file_py(&self, filepath: &PyAny) -> anyhow::Result<()> {
+        self.to_csv_file(PathBuf::extract(filepath)?)
+    }
 )]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize, SerdeAPI)]
 pub struct SpeedTrace {
     /// simulation time
     pub time: Vec<si::Time>,
     /// simulation speed
     pub speed: Vec<si::Velocity>,
@@ -116,14 +121,38 @@
         ensure!(
             !st.is_empty(),
             "Invalid SpeedTrace file {:?}; SpeedTrace is empty",
             filepath
         );
         Ok(st)
     }
+
+    /// Save speed trace to csv file
+    pub fn to_csv_file<P: AsRef<Path>>(&self, filepath: P) -> anyhow::Result<()> {
+        let file = std::fs::OpenOptions::new().write(true).open(filepath)?;
+        let mut wrtr = csv::WriterBuilder::new()
+            .has_headers(true)
+            .from_writer(file);
+        let engine_on: Vec<Option<bool>> = match &self.engine_on {
+            Some(eo_vec) => eo_vec
+                .iter()
+                .map(|eo| Some(*eo))
+                .collect::<Vec<Option<bool>>>(),
+            None => vec![None; self.len()],
+        };
+        for ((time, speed), engine_on) in self.time.iter().zip(&self.speed).zip(engine_on) {
+            wrtr.serialize(SpeedTraceElement {
+                time: *time,
+                speed: *speed,
+                engine_on,
+            })?;
+        }
+        wrtr.flush()?;
+        Ok(())
+    }
 }
 
 impl Default for SpeedTrace {
     fn default() -> Self {
         let mut speed_mps: Vec<f64> = Vec::linspace(0.0, 20.0, 800);
         speed_mps.append(&mut [20.0; 100].to_vec());
         speed_mps.append(&mut Vec::linspace(20.0, 0.0, 200));
@@ -321,14 +350,15 @@
             self.speed_trace.dt(self.state.i),
             Some(true),
         )?;
 
         self.state.time = self.speed_trace.time[self.state.i];
         self.state.speed = self.speed_trace.speed[self.state.i];
         self.state.offset += self.speed_trace.mean(self.state.i) * self.state.dt;
+        set_link_and_offset(&mut self.state, &self.path_tpc)?;
         self.state.total_dist += (self.speed_trace.mean(self.state.i) * self.state.dt).abs();
         Ok(())
     }
 
     /// Saves current time step for self and nested `loco_con`.
     fn save_state(&mut self) {
         if let Some(interval) = self.save_interval {
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/speed_limit_train_sim.rs` & `altrios-0.2.0/rust/altrios-core/src/train/speed_limit_train_sim.rs`

 * *Files 0% similar despite different names*

```diff
@@ -295,14 +295,15 @@
             .update_res(&mut self.state, &self.path_tpc, &Dir::Fwd)?;
         self.solve_required_pwr()?;
         self.loco_con.solve_energy_consumption(
             self.state.pwr_whl_out,
             self.state.dt,
             Some(true),
         )?;
+        set_link_and_offset(&mut self.state, &self.path_tpc)?;
         Ok(())
     }
 
     fn save_state(&mut self) {
         if let Some(interval) = self.save_interval {
             if self.state.i % interval == 0 || 1 == self.state.i {
                 self.history.push(self.state);
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/train_config.rs` & `altrios-0.2.0/rust/altrios-core/src/train/train_config.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/train/train_state.rs` & `altrios-0.2.0/rust/altrios-core/src/train/train_state.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 use crate::imports::*;
+use crate::track::PathTpc;
 
 #[derive(Debug, Clone, Copy, PartialEq, Serialize, Deserialize, HistoryVec)]
 #[altrios_api(
     #[new]
     fn __new__(
         time_seconds: Option<f64>,
         offset_meters: Option<f64>,
@@ -68,19 +69,26 @@
     }
 )]
 pub struct TrainState {
     /// time since user-defined datum
     pub time: si::Time,
     /// index for time steps
     pub i: usize,
+    /// Linear-along-track, directional distance from initial starting position.
+    ///
     /// If this is provided in [InitTrainState::new], it gets set as the train length or the value,
     /// whichever is larger, and if it is not provided, then it defaults to the train length.
     pub offset: si::Length,
     pub offset_back: si::Length,
+    /// Linear-along-track, cumulative, absolute distance from initial starting position.
     pub total_dist: si::Length,
+    /// Current link containing head end (i.e. pulling locomotives) of train
+    pub link_idx_front: u32,
+    /// Offset from start of current link
+    pub offset_in_link: si::Length,
     /// Achieved speed based on consist capabilities and train resistance
     pub speed: si::Velocity,
     /// Speed limit
     pub speed_limit: si::Velocity,
     /// Speed target from meet-pass planner
     pub speed_target: si::Velocity,
     pub dt: si::Time,
@@ -118,14 +126,16 @@
     fn default() -> Self {
         Self {
             time: Default::default(),
             i: 1,
             offset: Default::default(),
             offset_back: Default::default(),
             total_dist: si::Length::ZERO,
+            link_idx_front: Default::default(),
+            offset_in_link: Default::default(),
             speed: Default::default(),
             speed_limit: Default::default(),
             dt: uc::S,
             length: Default::default(),
             mass_static: Default::default(),
             mass_adj: Default::default(),
             mass_freight: Default::default(),
@@ -211,7 +221,34 @@
         si_chk_num_gtz_fin(&mut errors, &self.length, "Length");
         // si_chk_num_gtz_fin(&mut errors, &self.res_bearing, "Resistance bearing");
         // si_chk_num_fin(&mut errors, &self.res_davis_b, "Resistance Davis B");
         // si_chk_num_gtz_fin(&mut errors, &self.drag_area, "Drag area");
         errors.make_err()
     }
 }
+
+/// Sets `link_idx_front` and `offset_in_link` based on `state` and `path_tpc`
+///
+/// Assumes that `offset` in `link_points()` is monotically increasing, which may not always be true.
+pub fn set_link_and_offset(state: &mut TrainState, path_tpc: &PathTpc) -> anyhow::Result<()> {
+    let idx_curr_link = path_tpc
+        .link_points()
+        .iter()
+        .position(|&lp| lp.offset >= state.offset)
+        // if None, assume that it's the last element
+        .unwrap_or_else(|| path_tpc.link_points().len())
+        - 1;
+    state.link_idx_front = path_tpc
+        .link_points()
+        .get(idx_curr_link)
+        .with_context(|| format_dbg!())?
+        .link_idx
+        .idx() as u32;
+    state.offset_in_link = state.offset
+        - path_tpc
+            .link_points()
+            .get(idx_curr_link)
+            .with_context(|| format_dbg!())?
+            .offset;
+
+    Ok(())
+}
```

### Comparing `altrios-0.1.8/rust/altrios-core/src/traits.rs` & `altrios-0.2.0/rust/altrios-core/src/traits.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/uc.rs` & `altrios-0.2.0/rust/altrios-core/src/uc.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/utils/mod.rs` & `altrios-0.2.0/rust/altrios-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/utils/val_range.rs` & `altrios-0.2.0/rust/altrios-core/src/utils/val_range.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/src/validate.rs` & `altrios-0.2.0/rust/altrios-core/src/validate.rs`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use uom::si::Quantity;
 use uom::ConstZero;
 
 pub type ValidationError = anyhow::Error;
 pub type ValidationErrors = ComboErrors<ValidationError>;
 pub type ValidationResults = Result<(), ValidationErrors>;
 
-///Generate valid default like input for use in other objects
+///Generate valid default-like input for use in other objects
 pub trait Valid: Sized + Default {
     fn valid() -> Self {
         Default::default()
     }
 }
 
 ///Specify when an object is valid, real, and fake
```

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/Cargo.toml` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/README.md` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/altrios_api/altrios_api_utils.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/altrios_api.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/altrios_api.rs`

 * *Files 2% similar despite different names*

```diff
@@ -73,88 +73,82 @@
                 .unzip();
             field.attrs = new_attrs.0.iter().cloned().cloned().collect();
 
             impl_getters_and_setters(&mut py_impl_block, ident, &opts, &ftype);
         }
     } else if let syn::Fields::Unnamed(syn::FieldsUnnamed { unnamed, .. }) = &mut ast.fields {
         // tuple struct
-        let ident_str = ast.ident.to_string();
-        if ["Vec", "Network", "Path"]
-            .iter()
-            .any(|&x| ident_str.contains(x))
-        {
-            assert!(unnamed.len() == 1);
-            for field in unnamed.iter() {
-                let ftype = field.ty.clone();
-                if let syn::Type::Path(type_path) = ftype.clone() {
-                    let type_str = type_path.clone().into_token_stream().to_string();
-                    if type_str.contains("Vec") {
-                        let re = Regex::new(r"Vec < (.+) >").unwrap();
-                        // println!("{}", type_str);
-                        // println!("{}", &re.captures(&type_str).unwrap()[1]);
-                        let contained_dtype: TokenStream2 = re.captures(&type_str).unwrap()[1]
-                            .to_string()
-                            .parse()
-                            .unwrap();
-                        py_impl_block.extend::<TokenStream2>(
-                            quote! {
-                                #[new]
-                                /// Rust-defined `__new__` magic method for Python used exposed via PyO3.
-                                fn __new__(v: Vec<#contained_dtype>) -> Self {
-                                    Self(v)
-                                }
-                                /// Rust-defined `__repr__` magic method for Python used exposed via PyO3.
-                                fn __repr__(&self) -> String {
-                                    format!("Pyo3Vec({:?})", self.0)
-                                }
-                                /// Rust-defined `__str__` magic method for Python used exposed via PyO3.
-                                fn __str__(&self) -> String {
-                                    format!("{:?}", self.0)
-                                }
-                                /// Rust-defined `__getitem__` magic method for Python used exposed via PyO3.
-                                /// Prevents the Python user getting item directly using indexing.
-                                fn __getitem__(&self, _idx: usize) -> anyhow::Result<()> {
-                                    bail!(PyNotImplementedError::new_err(
-                                        "Getting Rust vector value at index is not implemented.
-                                        Run `tolist` method to convert to standalone Python list.",
-                                    ))
-                                }
-                                /// Rust-defined `__setitem__` magic method for Python used exposed via PyO3.
-                                /// Prevents the Python user setting item using indexing.
-                                fn __setitem__(&mut self, _idx: usize, _new_value: #contained_dtype) -> anyhow::Result<()> {
-                                    bail!(PyNotImplementedError::new_err(
-                                        "Setting list value at index is not implemented.
-                                        Run `tolist` method, modify value at index, and
-                                        then set entire list.",
-                                    ))
-                                }
-                                /// PyO3-exposed method to convert vec-containing struct to Python list. 
-                                fn tolist(&self) -> anyhow::Result<Vec<#contained_dtype>> {
-                                    Ok(self.0.clone())
-                                }
-                                /// Rust-defined `__len__` magic method for Python used exposed via PyO3.
-                                /// Returns the length of the Rust vector.
-                                fn __len__(&self) -> usize {
-                                    self.0.len()
-                                }
-                                /// PyO3-exposed method to check if the vec-containing struct is empty.
-                                fn is_empty(&self) -> bool {
-                                    self.0.is_empty()
-                                }
-                            }
-                        );
-                        impl_block.extend::<TokenStream2>(quote! {
-                            impl #ident{
-                                /// Implement the non-Python `new` method.
-                                pub fn new(value: Vec<#contained_dtype>) -> Self {
-                                    Self(value)
-                                }
+        assert!(unnamed.len() == 1);
+        for field in unnamed.iter() {
+            let ftype = field.ty.clone();
+            if let syn::Type::Path(type_path) = ftype.clone() {
+                let type_str = type_path.clone().into_token_stream().to_string();
+                if type_str.contains("Vec") {
+                    let re = Regex::new(r"Vec < (.+) >").unwrap();
+                    // println!("{}", type_str);
+                    // println!("{}", &re.captures(&type_str).unwrap()[1]);
+                    let contained_dtype: TokenStream2 = re.captures(&type_str).unwrap()[1]
+                        .to_string()
+                        .parse()
+                        .unwrap();
+                    py_impl_block.extend::<TokenStream2>(
+                        quote! {
+                            #[new]
+                            /// Rust-defined `__new__` magic method for Python used exposed via PyO3.
+                            fn __new__(v: Vec<#contained_dtype>) -> Self {
+                                Self(v)
                             }
-                        });
-                    }
+                            /// Rust-defined `__repr__` magic method for Python used exposed via PyO3.
+                            fn __repr__(&self) -> String {
+                                format!("Pyo3Vec({:?})", self.0)
+                            }
+                            /// Rust-defined `__str__` magic method for Python used exposed via PyO3.
+                            fn __str__(&self) -> String {
+                                format!("{:?}", self.0)
+                            }
+                            /// Rust-defined `__getitem__` magic method for Python used exposed via PyO3.
+                            /// Prevents the Python user getting item directly using indexing.
+                            fn __getitem__(&self, _idx: usize) -> anyhow::Result<()> {
+                                bail!(PyNotImplementedError::new_err(
+                                    "Getting Rust vector value at index is not implemented.
+                            Run `tolist` method to convert to standalone Python list.",
+                                ))
+                            }
+                            /// Rust-defined `__setitem__` magic method for Python used exposed via PyO3.
+                            /// Prevents the Python user setting item using indexing.
+                            fn __setitem__(&mut self, _idx: usize, _new_value: #contained_dtype) -> anyhow::Result<()> {
+                                bail!(PyNotImplementedError::new_err(
+                                    "Setting list value at index is not implemented.
+                            Run `tolist` method, modify value at index, and
+                            then set entire list.",
+                                ))
+                            }
+                            /// PyO3-exposed method to convert vec-containing struct to Python list. 
+                            fn tolist(&self) -> anyhow::Result<Vec<#contained_dtype>> {
+                                Ok(self.0.clone())
+                            }
+                            /// Rust-defined `__len__` magic method for Python used exposed via PyO3.
+                            /// Returns the length of the Rust vector.
+                            fn __len__(&self) -> usize {
+                                self.0.len()
+                            }
+                            /// PyO3-exposed method to check if the vec-containing struct is empty.
+                            fn is_empty(&self) -> bool {
+                                self.0.is_empty()
+                            }
+                        }
+                    );
+                    impl_block.extend::<TokenStream2>(quote! {
+                        impl #ident{
+                            /// Implement the non-Python `new` method.
+                            pub fn new(value: Vec<#contained_dtype>) -> Self {
+                                Self(value)
+                            }
+                        }
+                    });
                 }
             }
         }
     } else {
         abort_call_site!(
             "Invalid use of `altrios_api` macro.  Expected tuple struct or C-style struct."
         );
```

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/history_vec_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/hm_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/lib.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/lib.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/serde_api_derive.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-core/altrios-proc-macros/src/utilities.rs` & `altrios-0.2.0/rust/altrios-core/altrios-proc-macros/src/utilities.rs`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-py/Cargo.toml` & `altrios-0.2.0/rust/altrios-py/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-py/README.md` & `altrios-0.2.0/rust/altrios-py/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/rust/altrios-py/src/lib.rs` & `altrios-0.2.0/rust/altrios-py/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     m.add_class::<TrainParams>()?;
     m.add_class::<RailVehicle>()?;
     m.add_class::<TrainSimBuilder>()?;
     m.add_class::<SpeedLimitTrainSimVec>()?;
     m.add_class::<EstTimeNet>()?;
     m.add_function(wrap_pyfunction!(import_rail_vehicles_py, m)?)?;
     m.add_function(wrap_pyfunction!(import_locations_py, m)?)?;
-    m.add_function(wrap_pyfunction!(import_network_py, m)?)?;
     m.add_function(wrap_pyfunction!(make_est_times_py, m)?)?;
     m.add_function(wrap_pyfunction!(run_dispatch_py, m)?)?;
     m.add_function(wrap_pyfunction!(check_od_pair_valid, m)?)?;
     m.add_function(wrap_pyfunction!(build_speed_limit_train_sims, m)?)?;
     m.add_function(wrap_pyfunction!(run_speed_limit_train_sims, m)?)?;
 
     m.add_class::<Pyo3VecWrapper>()?;
```

### Comparing `altrios-0.1.8/rust/Cargo.lock` & `altrios-0.2.0/rust/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -42,26 +42,25 @@
 name = "allocator-api2"
 version = "0.2.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0942ffc6dcaadf03badf6e6a2d0228460359d5e34b57ccdc720b7382dfbd5ec5"
 
 [[package]]
 name = "altrios-core"
-version = "0.1.5"
+version = "0.1.7"
 dependencies = [
  "altrios-proc-macros",
  "anyhow",
  "argmin",
  "bincode",
  "csv",
  "directories",
  "duplicate",
  "easy-ext",
  "eng_fmt",
- "enum_dispatch",
  "log",
  "nohash-hasher",
  "paste",
  "polars",
  "polars-lazy",
  "project-root",
  "pyo3",
```

### Comparing `altrios-0.1.8/rust/Cargo.toml` & `altrios-0.2.0/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/pyproject.toml` & `altrios-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0"]
 build-backend = "maturin"
 
 [project]
 name = "altrios"
-version = "0.1.8"
+version = "0.2.0"
 authors = [
     { name = "ALTRIOS Team", email = "altrios@nrel.gov" },
     { name = "Chad Baker, Lead Developer" },
     { name = "Nick Reinicke, Developer" },
     { name = "Matt Bruchon, Developer" },
     { name = "Saad Akhtar, Developer" },
     { name = "Steven Shi, Developer" },
```

### Comparing `altrios-0.1.8/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml` & `altrios-0.2.0/python/altrios/resources/powertrains/fuel_converters/wabtec_tier4.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx` & `altrios-0.2.0/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah.xlsx`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml` & `altrios-0.2.0/python/altrios/resources/powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/trains/train_res_temp.yaml` & `altrios-0.2.0/python/altrios/resources/trains/train_res_temp.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/demo_data/speed_trace.csv` & `altrios-0.2.0/python/altrios/resources/demo_data/speed_trace.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/networks/links_test.yaml` & `altrios-0.2.0/python/altrios/resources/networks/links_test.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/networks/simple_corridor_network.yaml` & `altrios-0.2.0/python/altrios/resources/networks/simple_corridor_network.yaml`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv` & `altrios-0.2.0/python/altrios/resources/networks/simple_corridor_two_segment_locations.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/Default Demand StoBar.csv` & `altrios-0.2.0/python/altrios/resources/Default Demand StoBar.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/rolling_stock/rail_vehicles.csv` & `altrios-0.2.0/python/altrios/resources/rolling_stock/rail_vehicles.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/Cambium22_MidCase_annual_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/EIA_Electricity_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/Cambium22_MidCase_tod_gea.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/GREET-CA_Emissions_Factors.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/NREL_ATB_Battery_Cost_Forecasts.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv` & `altrios-0.2.0/python/altrios/resources/metrics_inputs/EIA_Liquid_Fuel_Prices.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/resources/TimedPaths.csv` & `altrios-0.2.0/python/altrios/resources/TimedPaths.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/__init__.py` & `altrios-0.2.0/python/altrios/__init__.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/demos/speed_limit_train_sim_demo.py` & `altrios-0.2.0/python/altrios/demos/speed_limit_simple_corr_demo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 # %%
-import altrios as alt
+"""
+SetSpeedTrainSim over a simple, hypothetical corridor
+"""
+
 import time
 import matplotlib.pyplot as plt
 import numpy as np
-import seaborn as sns
 import pandas as pd
-sns.set()
+import seaborn as sns
 
-SHOW_PLOTS = alt.utils.show_plots()
+import altrios as alt 
+sns.set_theme()
 
-SAVE_INTERVAL = 100
+SHOW_PLOTS = alt.utils.show_plots()
 
+SAVE_INTERVAL = 1
+res = alt.ReversibleEnergyStorage.from_file(
+    alt.resources_root() / "powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml"
+)
+# https://docs.rs/altrios-core/latest/altrios_core/train/struct.TrainConfig.html
 train_config = alt.TrainConfig(
     cars_empty=50,
     cars_loaded=50,
     rail_vehicle_type="Manifest",
-    train_type=alt.TrainType.Freight,
+    train_type=None, 
     train_length_meters=None,
     train_mass_kilograms=None,
 )
 
-# instantiate battery model
-res = alt.ReversibleEnergyStorage.from_file(
-    alt.resources_root() / "powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml"
-)
-# instantiate electric drivetrain (motors and any gearboxes)
 edrv = alt.ElectricDrivetrain(
     pwr_out_frac_interp=[0., 1.],
     eta_interp=[0.98, 0.98],
     pwr_out_max_watts=5e9,
     save_interval=SAVE_INTERVAL,
 )
 
-bel = alt.Locomotive.build_battery_electric_loco(
+bel: alt.Locomotive = alt.Locomotive.build_battery_electric_loco(
     reversible_energy_storage=res,
     drivetrain=edrv,
     loco_params=alt.LocoParams.from_dict(dict(
         pwr_aux_offset_watts=8.55e3,
         pwr_aux_traction_coeff_ratio=540.e-6,
         force_max_newtons=667.2e3,
 )))
 
 # construct a vector of one BEL and several conventional locomotives
 loco_vec = [bel.clone()] + [alt.Locomotive.default()] * 7
 # instantiate consist
 loco_con = alt.Consist(
-    loco_vec,
+    loco_vec
 )
 
+
 tsb = alt.TrainSimBuilder(
     train_id="0",
-    origin_id="Minneapolis",
-    destination_id="Superior",
+    origin_id="A",
+    destination_id="B",
     train_config=train_config,
     loco_con=loco_con,
 )
 
-# make sure rail_vehicle_map can be constructed from yaml file and such
-rail_vehicle_file = "rolling_stock/" + train_config.rail_vehicle_type + ".yaml"
-rail_vehicle = alt.RailVehicle.from_file(alt.resources_root() / rail_vehicle_file)
-
-network = alt.Network.from_file(alt.resources_root() / "networks/Taconite-NoBalloon.yaml")
+rail_vehicle_file = "rolling_stock/rail_vehicles.csv"
+rail_vehicle_map = alt.import_rail_vehicles(alt.resources_root() / rail_vehicle_file)
+rail_vehicle = rail_vehicle_map[train_config.rail_vehicle_type]
 
-location_map = alt.import_locations(alt.resources_root() / "networks/default_locations.csv")
+network = alt.Network.from_file(
+    alt.resources_root() / 'networks/simple_corridor_network.yaml')
 
-train_sim: alt.SpeedLimitTrainSim = tsb.make_speed_limit_train_sim(
+location_map = alt.import_locations(alt.resources_root() / "networks/simple_corridor_locations.csv")
+train_sim: alt.SetSpeedTrainSim = tsb.make_speed_limit_train_sim(
     rail_vehicle=rail_vehicle,
     location_map=location_map,
     save_interval=1,
 )
 train_sim.set_save_interval(SAVE_INTERVAL)
-
 est_time_net, _consist = alt.make_est_times(train_sim, network)
 
 timed_link_path = alt.run_dispatch(
     network,
     alt.SpeedLimitTrainSimVec([train_sim]),
     [est_time_net],
     False,
@@ -86,14 +89,15 @@
     network=network,
     timed_path=timed_link_path,
 )
 t1 = time.perf_counter()
 print(f'Time to simulate: {t1 - t0:.5g}')
 assert len(train_sim.history) > 1
 
+# pull out solved locomotive for plotting convenience
 loco0:alt.Locomotive = train_sim.loco_con.loco_vec.tolist()[0]
 
 fig, ax = plt.subplots(4, 1, sharex=True)
 ax[0].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
     np.array(train_sim.history.pwr_whl_out_watts) / 1e6,
     label="tract pwr",
@@ -150,10 +154,9 @@
 ax[-1].set_xlabel('Time [hr]')
 ax[-1].set_ylabel('Speed [m/s]')
 ax[-1].legend()
 plt.suptitle("Speed Limit Train Sim Demo")
 if SHOW_PLOTS:
     plt.tight_layout()
     plt.show()
-# Impact of sweep of battery capacity
 
 # %%
```

### Comparing `altrios-0.1.8/python/altrios/demos/conv_demo.py` & `altrios-0.2.0/python/altrios/demos/conv_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import altrios as alt
 import numpy as np
 import matplotlib.pyplot as plt
 import time
 import os
 import seaborn as sns
 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 
 # %%
 SAVE_INTERVAL = 1
 # load hybrid consist
 t0 = time.perf_counter()
```

### Comparing `altrios-0.1.8/python/altrios/demos/rollout_demo.py` & `altrios-0.2.0/python/altrios/demos/rollout_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from altrios import rollout, defaults, train_planner
 
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
 from pathlib import Path
 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 
 # %
 
 # %%
```

### Comparing `altrios-0.1.8/python/altrios/demos/bel_demo.py` & `altrios-0.2.0/python/altrios/demos/bel_demo.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import altrios as alt
 import numpy as np
 import matplotlib.pyplot as plt
 import time
 import os
 import seaborn as sns
 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 
 
 SAVE_INTERVAL = 1
```

### Comparing `altrios-0.1.8/python/altrios/demos/set_speed_train_sim_demo.py` & `altrios-0.2.0/python/altrios/demos/set_speed_train_sim_demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 import altrios as alt 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 
 SAVE_INTERVAL = 1
 
 # https://docs.rs/altrios-core/latest/altrios_core/train/struct.TrainConfig.html
 train_config = alt.TrainConfig(
@@ -21,16 +21,15 @@
     train_length_meters=None,
     train_mass_kilograms=None,
 )
 
 # instantiate battery model
 # https://docs.rs/altrios-core/latest/altrios_core/consist/locomotive/powertrain/reversible_energy_storage/struct.ReversibleEnergyStorage.html#
 res = alt.ReversibleEnergyStorage.from_file(
-    alt.resources_root() / 
-        "powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml"
+    alt.resources_root() / "powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml"
 )
 # instantiate electric drivetrain (motors and any gearboxes)
 # https://docs.rs/altrios-core/latest/altrios_core/consist/locomotive/powertrain/electric_drivetrain/struct.ElectricDrivetrain.html
 edrv = alt.ElectricDrivetrain(
     pwr_out_frac_interp=[0., 1.],
     eta_interp=[0.98, 0.98],
     pwr_out_max_watts=5e9,
@@ -57,40 +56,37 @@
 
 tsb = alt.TrainSimBuilder(
     train_id="0",
     train_config=train_config,
     loco_con=loco_con,
 )
 
-rail_vehicle_file = "rolling_stock/rail_vehicles.csv"
-rail_vehicle_map = alt.import_rail_vehicles(alt.resources_root() / rail_vehicle_file)
-rail_vehicle = rail_vehicle_map[train_config.rail_vehicle_type]
-
-network = alt.Network.from_file(alt.resources_root() / "networks/Taconite.yaml")
-# This data in this file were generated by running 
-# ```python
-# [lp.link_idx.idx for lp in sim0.path_tpc.link_points]
-# ``` 
-# in sim_manager_demo.py.
-link_path = alt.LinkPath.from_csv_file(alt.resources_root() / "demo_data/link_points_idx.csv")
-
+rail_vehicle_file = "rolling_stock/" + train_config.rail_vehicle_type + ".yaml"
+rail_vehicle = alt.RailVehicle.from_file(
+    alt.resources_root() / rail_vehicle_file)
+
+network = alt.Network.from_file(
+    alt.resources_root() / "networks/Taconite.yaml")
+link_path = alt.LinkPath.from_csv_file(
+    alt.resources_root() / "demo_data/link_points_idx.csv"
+)
 
 speed_trace = alt.SpeedTrace.from_csv_file(
     alt.resources_root() / "demo_data/speed_trace.csv"
 )
 
 train_sim: alt.SetSpeedTrainSim = tsb.make_set_speed_train_sim(
     rail_vehicle=rail_vehicle,
     network=network,
     link_path=link_path,
     speed_trace=speed_trace,
     save_interval=SAVE_INTERVAL,
 )
 
-train_sim.set_save_interval(1)
+train_sim.set_save_interval(SAVE_INTERVAL)
 t0 = time.perf_counter()
 train_sim.walk()
 t1 = time.perf_counter()
 print(f'Time to simulate: {t1 - t0:.5g}')
 
 fig, ax = plt.subplots(3, 1, sharex=True)
 ax[0].plot(
```

### Comparing `altrios-0.1.8/python/altrios/demos/speed_limit_simple_corr_demo.py` & `altrios-0.2.0/python/altrios/demos/set_speed_simple_corr_demo.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,157 +6,134 @@
 import time
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 
 import altrios as alt 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 
 SAVE_INTERVAL = 1
-res = alt.ReversibleEnergyStorage.from_file(
-    alt.resources_root() / "powertrains/reversible_energy_storages/Kokam_NMC_75Ah_flx_drive.yaml"
-)
+
 # https://docs.rs/altrios-core/latest/altrios_core/train/struct.TrainConfig.html
 train_config = alt.TrainConfig(
     cars_empty=50,
     cars_loaded=50,
     rail_vehicle_type="Manifest",
-    train_type=None, 
+    train_type=None,
     train_length_meters=None,
     train_mass_kilograms=None,
 )
 
-edrv = alt.ElectricDrivetrain(
-    pwr_out_frac_interp=[0., 1.],
-    eta_interp=[0.98, 0.98],
-    pwr_out_max_watts=5e9,
-    save_interval=SAVE_INTERVAL,
-)
-
-bel: alt.Locomotive = alt.Locomotive.build_battery_electric_loco(
-    reversible_energy_storage=res,
-    drivetrain=edrv,
-    loco_params=alt.LocoParams.from_dict(dict(
-        pwr_aux_offset_watts=8.55e3,
-        pwr_aux_traction_coeff_ratio=540.e-6,
-        force_max_newtons=667.2e3,
-)))
+bel: alt.Locomotive = alt.Locomotive.default_battery_electric_loco()
 
 # construct a vector of one BEL and several conventional locomotives
-loco_vec = [bel.clone()] + [alt.Locomotive.default()] * 7
+loco_vec = [bel] + [alt.Locomotive.default()] * 7
 # instantiate consist
 loco_con = alt.Consist(
-    loco_vec
+    loco_vec,
+    SAVE_INTERVAL,
 )
 
-
 tsb = alt.TrainSimBuilder(
     train_id="0",
-    origin_id="A",
-    destination_id="B",
     train_config=train_config,
     loco_con=loco_con,
 )
 
 rail_vehicle_file = "rolling_stock/rail_vehicles.csv"
 rail_vehicle_map = alt.import_rail_vehicles(alt.resources_root() / rail_vehicle_file)
 rail_vehicle = rail_vehicle_map[train_config.rail_vehicle_type]
 
 network = alt.Network.from_file(
     alt.resources_root() / 'networks/simple_corridor_network.yaml')
+# This data in this file were generated by running 
+# ```python
+# [lp.link_idx.idx for lp in sim0.path_tpc.link_points]
+# ``` 
+# in sim_manager_demo.py.
+link_path = alt.LinkPath.from_csv_file(
+    alt.resources_root() / "demo_data/link_points_idx_simple_corridor.csv")
 
-location_map = alt.import_locations(alt.resources_root() / "networks/simple_corridor_locations.csv")
-train_sim: alt.SetSpeedTrainSim = tsb.make_speed_limit_train_sim(
-    rail_vehicle=rail_vehicle,
-    location_map=location_map,
-    save_interval=1,
-)
-train_sim.set_save_interval(SAVE_INTERVAL)
-est_time_net, _consist = alt.make_est_times(train_sim, network)
 
-timed_link_path = alt.run_dispatch(
-    network,
-    alt.SpeedLimitTrainSimVec([train_sim]),
-    [est_time_net],
-    False,
-    False,
-)[0]
+speed_trace = alt.SpeedTrace.from_csv_file(
+    alt.resources_root() / "demo_data/speed_trace_simple_corridor.csv"
+)
 
-t0 = time.perf_counter()
-train_sim.walk_timed_path(
+train_sim: alt.SetSpeedTrainSim = tsb.make_set_speed_train_sim(
+    rail_vehicle=rail_vehicle,
     network=network,
-    timed_path=timed_link_path,
+    link_path=link_path,
+    speed_trace=speed_trace,
+    save_interval=SAVE_INTERVAL,
 )
+
+train_sim.set_save_interval(1)
+t0 = time.perf_counter()
+train_sim.walk()
 t1 = time.perf_counter()
 print(f'Time to simulate: {t1 - t0:.5g}')
-assert len(train_sim.history) > 1
 
 # pull out solved locomotive for plotting convenience
 loco0:alt.Locomotive = train_sim.loco_con.loco_vec.tolist()[0]
 
 fig, ax = plt.subplots(4, 1, sharex=True)
 ax[0].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.pwr_whl_out_watts) / 1e6,
+    train_sim.history.pwr_whl_out_watts,
     label="tract pwr",
 )
-ax[0].set_ylabel('Power [MW]')
+ax[0].set_ylabel('Power')
 ax[0].legend()
 
 ax[1].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.res_aero_newtons) / 1e3,
+    train_sim.history.res_aero_newtons,
     label='aero',
 )
 ax[1].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.res_rolling_newtons) / 1e3,
+    train_sim.history.res_rolling_newtons,
     label='rolling',
 )
 ax[1].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.res_curve_newtons) / 1e3,
+    train_sim.history.res_curve_newtons,
     label='curve',
 )
 ax[1].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.res_bearing_newtons) / 1e3,
+    train_sim.history.res_bearing_newtons,
     label='bearing',
 )
 ax[1].plot(
     np.array(train_sim.history.time_seconds) / 3_600,
-    np.array(train_sim.history.res_grade_newtons) / 1e3,
+    train_sim.history.res_grade_newtons,
     label='grade',
 )
-ax[1].set_ylabel('Force [MN]')
+ax[1].set_ylabel('Force [N]')
 ax[1].legend()
 
+ax[-1].plot(
+    np.array(train_sim.history.time_seconds) / 3_600,
+    train_sim.speed_trace.speed_meters_per_second,
+)
+ax[-1].set_xlabel('Time [hr]')
+ax[-1].set_ylabel('Speed [m/s]')
+
 ax[2].plot(
     np.array(train_sim.history.time_seconds) / 3_600, 
     np.array(loco0.res.history.soc)
 )
 
 ax[2].set_ylabel('SOC')
 ax[2].legend()
 
-ax[-1].plot(
-    np.array(train_sim.history.time_seconds) / 3_600,
-    train_sim.history.speed_meters_per_second,
-    label='achieved'
-)
-ax[-1].plot(
-    np.array(train_sim.history.time_seconds) / 3_600,
-    train_sim.history.speed_limit_meters_per_second,
-    label='limit'
-)
-ax[-1].set_xlabel('Time [hr]')
-ax[-1].set_ylabel('Speed [m/s]')
-ax[-1].legend()
-plt.suptitle("Speed Limit Train Sim Demo")
+plt.suptitle("Set Speed Train Sim Demo")
+plt.tight_layout()
+
 if SHOW_PLOTS:
-    plt.tight_layout()
-    plt.show()
+    fig.show()
 
 # %%
```

### Comparing `altrios-0.1.8/python/altrios/demos/test_demos.py` & `altrios-0.2.0/python/altrios/demos/test_demos.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/demos/sim_manager_demo.py` & `altrios-0.2.0/python/altrios/demos/sim_manager_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import altrios as alt
 import numpy as np
 import matplotlib.pyplot as plt
 import time
 import seaborn as sns
 from pathlib import Path
 
-sns.set()
+sns.set_theme()
 
 SHOW_PLOTS = alt.utils.show_plots()
 # %
 
 plot_dir = Path() / "plots"
 # make the dir if it doesn't exist
 plot_dir.mkdir(exist_ok=True)
```

### Comparing `altrios-0.1.8/python/altrios/defaults.py` & `altrios-0.2.0/python/altrios/defaults.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/output_12072022.csv` & `altrios-0.2.0/python/altrios/output_12072022.csv`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/loaders/powertrain_components.py` & `altrios-0.2.0/python/altrios/loaders/powertrain_components.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/train_planner.py` & `altrios-0.2.0/python/altrios/train_planner.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/stringline_old.py` & `altrios-0.2.0/python/altrios/stringline_old.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/metric_calculator.py` & `altrios-0.2.0/python/altrios/metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/stringline.py` & `altrios-0.2.0/python/altrios/stringline.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/sim_manager.py` & `altrios-0.2.0/python/altrios/sim_manager.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/altrios_pyo3.pyi` & `altrios-0.2.0/python/altrios/altrios_pyo3.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -609,22 +609,26 @@
     engine_on: Optional[list[bool]]
     def clone(self) -> Self: ...
     @classmethod
     def default(cls) -> Self: ...
     def __copy__(self) -> Any: ...
     def __len__(self) -> int: ...
     def from_csv_file(pathstr: str) -> Self: ...
+    def to_csv_file(self, pathstr: str): ...
 
 
 class TrainState:
     time_seconds: float
     i: int
     offset_meters: float
     offset_back_meters: float
     total_dist_meters: float
+    link_idx_front: int
+    offset_in_link_meters: float
+    grade_front: float
     speed_meters_per_second: float
     speed_limit_meters_per_second: float
     speed_target_meters_per_second: float
     dt_seconds: float
     length_meters: float
     mass_static_kilograms: float
     mass_adj_kilograms: float
@@ -664,14 +668,18 @@
     def clone(self) -> TrainState: ...
     def reset_orphaned(self) -> None: ...
 
 
 class TrainStateHistoryVec(SerdeAPI):
     time_seconds: list[float]
     offset_meters: list[float]
+    offset_back_meters: list[float]
+    link_idx_front: list[int]
+    offset_in_link_meters: list[float]
+    grade_front: list[float]
     speed_meters_per_second: list[float]
     speed_limit_meters_per_second: list[float]
     speed_target_meters_per_second: list[float]
     dt_seconds: list[float]
     length_meters: list[float]
     mass_static_kilograms: list[float]
     mass_adj_kilograms: list[float]
@@ -956,15 +964,14 @@
 
 class Link(SerdeAPI):
     length_meters: float
     @classmethod
     def default(cls) -> Self: ...
 
 
-def import_network(filename: str) -> List[Link]: ...
 def import_locations(filename: str) -> Dict[str, List[Location]]: ...
 def import_rail_vehicles(filename: str) -> Dict[str, RailVehicle]: ...
 
 
 def build_speed_limit_train_sims(
     train_sim_builders: List[TrainSimBuilder],
     rail_veh_map: Dict[str, RailVehicle],
```

### Comparing `altrios-0.1.8/python/altrios/rollout.py` & `altrios-0.2.0/python/altrios/rollout.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_powertrain_res.py` & `altrios-0.2.0/python/altrios/tests/test_powertrain_res.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_powertrain_fuel_conv.py` & `altrios-0.2.0/python/altrios/tests/test_powertrain_fuel_conv.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_locomotive_simulation.py` & `altrios-0.2.0/python/altrios/tests/test_locomotive_simulation.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_metric_calculator.py` & `altrios-0.2.0/python/altrios/tests/test_metric_calculator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_consist.py` & `altrios-0.2.0/python/altrios/tests/test_consist.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_multi_obj_cal_and_val.py` & `altrios-0.2.0/python/altrios/tests/test_multi_obj_cal_and_val.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_consist_sim.py` & `altrios-0.2.0/python/altrios/tests/test_consist_sim.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_powertrain_generator.py` & `altrios-0.2.0/python/altrios/tests/test_powertrain_generator.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_utilities.py` & `altrios-0.2.0/python/altrios/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_locomotive.py` & `altrios-0.2.0/python/altrios/tests/test_locomotive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_powertrain_edrive.py` & `altrios-0.2.0/python/altrios/tests/test_powertrain_edrive.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/mock_resources.py` & `altrios-0.2.0/python/altrios/tests/mock_resources.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/tests/test_rail_vehicles.py` & `altrios-0.2.0/python/altrios/tests/test_rail_vehicles.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/python/altrios/optimization/cal_and_val.py` & `altrios-0.2.0/python/altrios/optimization/cal_and_val.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from matplotlib.figure import Figure
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 import seaborn as sns
 import json
 import numpy.typing as npt
 import re
-sns.set()
+sns.set_theme()
 
 # local
 from altrios import SetSpeedTrainSim, ConsistSimulation, LocomotiveSimulation
 import altrios as alt
 
 def get_delta_seconds(ds: pd.Series) -> pd.Series:
     """
```

### Comparing `altrios-0.1.8/python/altrios/utilities.py` & `altrios-0.2.0/python/altrios/utilities.py`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/README.md` & `altrios-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/LICENSE.md` & `altrios-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `altrios-0.1.8/PKG-INFO` & `altrios-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: altrios
-Version: 0.1.8
+Version: 0.2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Dist: pandas >=2
 Requires-Dist: numpy
```

