# Comparing `tmp/hiperwalk-2.0b1.tar.gz` & `tmp/hiperwalk-2.0b11.tar.gz`

## Comparing `hiperwalk-2.0b1.tar` & `hiperwalk-2.0b11.tar`

### file list

```diff
@@ -1,136 +1,160 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/.readthedocs.yaml
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/build_and_upload_to_pypi
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/deleteme.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/fit.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/generator.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/oriented_lat.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/plot_max_success_probability.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/plot_optimal_runtime.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/prob_test.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/renato.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/ring_of_donuts.py
--rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/test_state.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/test_t_opt.py
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/.github/workflows/rebuild_project_page.yml
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/README.md
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/conf.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/go
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/test_docs
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/development/index.rst
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/documentation/graph.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/documentation/index.rst
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/documentation/plot.rst
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/cycle-arcs.dot
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/graph-arcs.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/graph-example.dot
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/line-arcs.dot
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/bounded-diagonal.dot
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/bounded-diagonal.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/bounded-natural.dot
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/bounded-natural.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/diagonal-directions.dot
--rw-r--r--   0        0        0     9307 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/even-dim-diagonal.dot
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/even-dim-diagonal.py
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/go
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/natural-directions.dot
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/periodic-diagonal.dot
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/periodic-diagonal.py
--rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/periodic-natural.dot
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/graphviz/grid/periodic-natural.py
--rw-r--r--   0        0        0     8252 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/install/index.rst
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/tutorial/graphs.rst
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/tutorial/index.rst
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/tutorial/plotting.rst
--rw-r--r--   0        0        0    17540 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/docs/tutorial/quantum_walk_models.rst
--rw-r--r--   0        0        0   348577 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled-Copy1.ipynb
--rw-r--r--   0        0        0  1644954 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled.ipynb
--rw-r--r--   0        0        0   765630 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled1.ipynb
--rw-r--r--   0        0        0  1234252 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled2.ipynb
--rw-r--r--   0        0        0   429871 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled3.ipynb
--rw-r--r--   0        0        0   541540 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/Untitled4.ipynb
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/coined-complete-search.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/coined-diagonal-grid.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/coined-grid-search.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/coined-hypercube.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/continuous-cycle.py
--rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/deleteme.py
--rw-r--r--   0        0        0    43772 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/exemplo1.ipynb
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/examples/issue13.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/_constants.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/complete.py
--rw-r--r--   0        0        0     4589 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/complete_bipartite.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/grid.py
--rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/hypercube.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/lattice.py
--rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/graph/line.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    31994 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/plot/refactor.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    33144 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/quantum_walk/coined.py
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/quantum_walk/continuous_time.py
--rw-r--r--   0        0        0    19253 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/__init__.py
--rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/run_all.sh
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/run_nonhpc.sh
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/test_constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/__init__.py
--rw-r--r--   0        0        0     3842 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/coined_cycle.py
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/coined_line.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/complete.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/complete_bipartite.py
--rw-r--r--   0        0        0     4169 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/continuous_graph.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/graph.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/tests/unit/hypercube.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/pyproject.toml
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0b1/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.readthedocs.yaml
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/build_and_upload_to_pypi
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/deleteme.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/fit.py
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hypercube.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/memory_test.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/oriented_lat.py
+-rw-r--r--   0        0        0   180930 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/output.txt
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/paulomotta.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/plot_max_success_probability.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/plot_optimal_runtime.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/prob_test.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/renato.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/ring_of_donuts.py
+-rw-r--r--   0        0        0      892 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/test_state.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/test_t_opt.py
+-rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.github/workflows/rebuild_project_page.yml
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/README.md
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/conf.py
+-rwxr-xr-x   0        0        0      104 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/go
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/test_docs
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/development/index.rst
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/hpc.rst
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/index.rst
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/complete.rst
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/complete_bipartite.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/cycle.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/grid.rst
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/hypercube.rst
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/integer_lattice.rst
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/documentation/graph_constructors/line.rst
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/examples/index.rst
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/graph-arcs.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/graph-example.dot
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.dot
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.dot
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/diagonal-grid-neigh-order.dot
+-rw-r--r--   0        0        0     5932 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.dot
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.py
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/go
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/natural-grid-neigh-order.dot
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.dot
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.dot
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.py
+-rw-r--r--   0        0        0     9009 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/install/index.rst
+-rw-r--r--   0        0        0     2085 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/graph_constructors.rst
+-rw-r--r--   0        0        0     6196 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/graphs.rst
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/index.rst
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/plotting.rst
+-rw-r--r--   0        0        0    23410 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/docs/tutorial/quantum_walk_models.rst
+-rw-r--r--   0        0        0   348577 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled-Copy1.ipynb
+-rw-r--r--   0        0        0  1644954 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled.ipynb
+-rw-r--r--   0        0        0   765630 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled1.ipynb
+-rw-r--r--   0        0        0  1234252 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled2.ipynb
+-rw-r--r--   0        0        0   429871 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled3.ipynb
+-rw-r--r--   0        0        0   541540 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/Untitled4.ipynb
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-bipartite-search.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-complete-search.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-diagonal-grid.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-grid-search.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/coined-hypercube.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/continuous-cycle.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/deleteme.py
+-rw-r--r--   0        0        0    43772 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/exemplo1.ipynb
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/grid-search.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/grovers-algorithm.py
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/hipercubo-multimarcados.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/hypercube-search.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/issue13.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/new_hypercube.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/square_lattice.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/CoinedDiagonalLattice.ipynb
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/ContinuousCycle.ipynb
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/examples/notebooks/test_load_numpy_matrix.ipynb
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/_constants.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/_sym_dir_multigraph.py
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/complete.py
+-rw-r--r--   0        0        0     4565 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/complete_bipartite.py
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0    15634 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/grid.py
+-rw-r--r--   0        0        0     4860 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/hypercube.py
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/integer_lattice.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/multigraph.py
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/graph/weighted_graph.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    36244 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    12866 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    39685 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/coined.py
+-rw-r--r--   0        0        0    17212 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/continuous_time.py
+-rw-r--r--   0        0        0    27148 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/__init__.py
+-rwxr-xr-x   0        0        0      120 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_all.sh
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      121 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/__init__.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/binary_search_test.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/coined_cycle.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/coined_line.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/complete.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/complete_bipartite.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/continuous_time.py
+-rw-r--r--   0        0        0     5370 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/graph.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/hypercube.py
+-rw-r--r--   0        0        0     6517 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/tests/unit/multigraph.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/README.md
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/pyproject.toml
+-rw-r--r--   0        0        0    11957 2020-02-02 00:00:00.000000 hiperwalk-2.0b11/PKG-INFO
```

### Comparing `hiperwalk-2.0b1/fit.py` & `hiperwalk-2.0b11/fit.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/ring_of_donuts.py` & `hiperwalk-2.0b11/ring_of_donuts.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/test_state.py` & `hiperwalk-2.0b11/test_state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/test_t_opt.py` & `hiperwalk-2.0b11/test_t_opt.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/.github/workflows/rebuild_project_page.yml` & `hiperwalk-2.0b11/.github/workflows/rebuild_project_page.yml`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/config.py` & `hiperwalk-2.0b11/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/custom.nbl` & `hiperwalk-2.0b11/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/custom.py` & `hiperwalk-2.0b11/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/distance.py` & `hiperwalk-2.0b11/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/dtqw1d.nbl` & `hiperwalk-2.0b11/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/dtqw1d.py` & `hiperwalk-2.0b11/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/dtqw2d.nbl` & `hiperwalk-2.0b11/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/dtqw2d.py` & `hiperwalk-2.0b11/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/gnuplot.py` & `hiperwalk-2.0b11/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/hiperwalk.py` & `hiperwalk-2.0b11/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/install.sh` & `hiperwalk-2.0b11/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/ioFunctions.py` & `hiperwalk-2.0b11/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/neblina.py` & `hiperwalk-2.0b11/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/operators.py` & `hiperwalk-2.0b11/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/parsing.py` & `hiperwalk-2.0b11/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/run.py` & `hiperwalk-2.0b11/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/staggered1d.nbl` & `hiperwalk-2.0b11/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/staggered1d.py` & `hiperwalk-2.0b11/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/staggered2d.nbl` & `hiperwalk-2.0b11/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/staggered2d.py` & `hiperwalk-2.0b11/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/standardDeviation.py` & `hiperwalk-2.0b11/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/state.py` & `hiperwalk-2.0b11/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/testmode.py` & `hiperwalk-2.0b11/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/Archive/walks.py` & `hiperwalk-2.0b11/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/Makefile` & `hiperwalk-2.0b11/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/conf.py` & `hiperwalk-2.0b11/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 sys.path.append(os.path.abspath('../'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Hiperwalk'
-copyright = '2023'
+copyright = '2024'
 author = 'Gustavo Bezerra'
 
 # The full version, including alpha/beta/rc tags
 release = 'stable'
 version = 'stable'
```

### Comparing `hiperwalk-2.0b1/docs/index.rst` & `hiperwalk-2.0b11/docs/index.rst`

 * *Files 15% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 .. toctree::
    :maxdepth: 3
    :caption: Contents:
 
    install/index
    tutorial/index
+   examples/index
    documentation/index
    development/index
 
 
 Indices and tables
 ==================
```

### Comparing `hiperwalk-2.0b1/docs/make.bat` & `hiperwalk-2.0b11/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/_templates/automodule.rst` & `hiperwalk-2.0b11/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/development/index.rst` & `hiperwalk-2.0b11/docs/development/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,21 @@
 If you installed the standalone version (without HPC support), 
 execute:
 
 .. code-block:: shell
 
     ./run_nonhpc.sh
 
+Bug Report and Contact
+======================
+
+To send a bug report or
+contribute to Hiperwalk or contact the developers, 
+write an email to hiperwalk@gmail.com.
+
 Documentation
 =============
 
 There are likely to be new features in the ``main`` branch. 
 These features are documented online in the  **latest** version.
 
 Install Requirements
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/graph-arcs.dot` & `hiperwalk-2.0b11/docs/graphviz/graph-arcs.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/bounded-diagonal.dot` & `hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.dot`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,32 @@
 	"(0, 1)" [pos="0.0,1.75!" width=0.75 height=0.75 fixedsize=True]
 	"(1, 1)" [pos="1.75,1.75!" width=0.75 height=0.75 fixedsize=True]
 	"(2, 1)" [pos="3.5,1.75!" width=0.75 height=0.75 fixedsize=True]
 	"(0, 2)" [pos="0.0,3.5!" width=0.75 height=0.75 fixedsize=True]
 	"(1, 2)" [pos="1.75,3.5!" width=0.75 height=0.75 fixedsize=True]
 	"(2, 2)" [pos="3.5,3.5!" width=0.75 height=0.75 fixedsize=True]
 
-	 "(0, 0)" -> "(1, 1)"[headlabel=0 labeldistance=2 labelangle=-50];
-	 "(1, 0)" -> "(2, 1)"[headlabel=1 labeldistance=2 labelangle=-50];
-	 "(1, 0)" -> "(0, 1)"[headlabel=2 labeldistance=2 labelangle=-50];
-	 "(2, 0)" -> "(1, 1)"[headlabel=3 labeldistance=2 labelangle=-50];
-	 "(0, 1)" -> "(1, 2)"[headlabel=4 labeldistance=2 labelangle=-50];
-	 "(0, 1)" -> "(1, 0)"[headlabel=5 labeldistance=2 labelangle=-50];
-	 "(1, 1)" -> "(2, 2)"[headlabel=6 labeldistance=2 labelangle=-50];
-	 "(1, 1)" -> "(2, 0)"[headlabel=7 labeldistance=2 labelangle=-50];
-	 "(1, 1)" -> "(0, 2)"[headlabel=8 labeldistance=2 labelangle=-50];
-	 "(1, 1)" -> "(0, 0)"[headlabel=9 labeldistance=2 labelangle=-50];
-	 "(2, 1)" -> "(1, 2)"[headlabel=10 labeldistance=2 labelangle=-50];
-	 "(2, 1)" -> "(1, 0)"[headlabel=11 labeldistance=2 labelangle=-50];
-	 "(0, 2)" -> "(1, 1)"[headlabel=12 labeldistance=2 labelangle=-50];
-	 "(1, 2)" -> "(2, 1)"[headlabel=13 labeldistance=2 labelangle=-50];
-	 "(1, 2)" -> "(0, 1)"[headlabel=14 labeldistance=2 labelangle=-50];
-	 "(2, 2)" -> "(1, 1)"[headlabel=15 labeldistance=2 labelangle=-50];
+	 "(0, 0)" -> "(1, 0)"[headlabel=0 labeldistance=4 labelangle=-20];
+	 "(0, 0)" -> "(0, 1)"[headlabel=1 labeldistance=4 labelangle=-20];
+	 "(1, 0)" -> "(2, 0)"[headlabel=2 labeldistance=4 labelangle=-20];
+	 "(1, 0)" -> "(0, 0)"[headlabel=3 labeldistance=4 labelangle=-20];
+	 "(1, 0)" -> "(1, 1)"[headlabel=4 labeldistance=4 labelangle=-20];
+	 "(2, 0)" -> "(1, 0)"[headlabel=5 labeldistance=4 labelangle=-20];
+	 "(2, 0)" -> "(2, 1)"[headlabel=6 labeldistance=4 labelangle=-20];
+	 "(0, 1)" -> "(1, 1)"[headlabel=7 labeldistance=4 labelangle=-20];
+	 "(0, 1)" -> "(0, 2)"[headlabel=8 labeldistance=4 labelangle=-20];
+	 "(0, 1)" -> "(0, 0)"[headlabel=9 labeldistance=4 labelangle=-20];
+	 "(1, 1)" -> "(2, 1)"[headlabel=10 labeldistance=4 labelangle=-20];
+	 "(1, 1)" -> "(0, 1)"[headlabel=11 labeldistance=4 labelangle=-20];
+	 "(1, 1)" -> "(1, 2)"[headlabel=12 labeldistance=4 labelangle=-20];
+	 "(1, 1)" -> "(1, 0)"[headlabel=13 labeldistance=4 labelangle=-20];
+	 "(2, 1)" -> "(1, 1)"[headlabel=14 labeldistance=4 labelangle=-20];
+	 "(2, 1)" -> "(2, 2)"[headlabel=15 labeldistance=4 labelangle=-20];
+	 "(2, 1)" -> "(2, 0)"[headlabel=16 labeldistance=4 labelangle=-20];
+	 "(0, 2)" -> "(1, 2)"[headlabel=17 labeldistance=4 labelangle=-20];
+	 "(0, 2)" -> "(0, 1)"[headlabel=18 labeldistance=4 labelangle=-20];
+	 "(1, 2)" -> "(2, 2)"[headlabel=19 labeldistance=4 labelangle=-20];
+	 "(1, 2)" -> "(0, 2)"[headlabel=20 labeldistance=4 labelangle=-20];
+	 "(1, 2)" -> "(1, 1)"[headlabel=21 labeldistance=4 labelangle=-20];
+	 "(2, 2)" -> "(1, 2)"[headlabel=22 labeldistance=4 labelangle=-20];
+	 "(2, 2)" -> "(2, 1)"[headlabel=23 labeldistance=4 labelangle=-20];
 }
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/bounded-diagonal.py` & `hiperwalk-2.0b11/docs/graphviz/grid/even-dim-diagonal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,61 @@
-print('digraph {')
+print('graph {')
 
-dim = 3
+dim = 4
 
-def out_of_bounds(axis):
-    return axis < 0 or axis >= dim 
+def out_of_bounds(vertex):
+    return (vertex[0] < 0 or vertex[0] >= dim
+            or
+            vertex[1] < 0 or vertex[1] >= dim)
 
-for y in range(dim):
-    for x in range(dim):
-        out_x = out_of_bounds(x)
-        out_y = out_of_bounds(y)
+for y in range(-1, dim + 1):
+    for x in range(-1, dim + 1):
 
         node_str = ('\t"' + str((x, y)) + '" ['
                     + 'pos="' + str(1.75*x) + ',' + str(1.75*y) + '!" '
                     + 'width=0.75 height=0.75 fixedsize=True')
-        if out_x or out_y:
+
+        out = out_of_bounds((x, y))
+        if out:
             node_str += (' style="dashed" label="' +
                          str((x % dim, y % dim)) + '"')
+
+        if (x % dim + y % dim) % 2:
+            node_str += ' fontcolor="white" fillcolor="darkgray" style="filled'
+            #node_str += ',dashed" penwidth=2' if out else '"'
+            node_str += ',dashed"' if out else '"'
+
         node_str += ']'
 
         print(node_str)
 
 print()
 
 arc_count = 0
-for y in range(dim):
-    for x in range(dim):
-        tail = str((x, y))
-        for d in range(4):
+for y in range(-1, dim + 1):
+    for x in range(-1, dim + 1):
+        for d in [0, 2]:
+            tail = (x, y)
+
             x_shift = 1 if d // 2 == 0 else -1
             y_shift = 1 if d % 2 == 0 else -1
             head = (x + x_shift, y + y_shift)
 
-            if out_of_bounds(head[0]) or out_of_bounds(head[1]):
+            if out_of_bounds(head) and out_of_bounds(tail):
                 continue
 
-            arc_str = '\t "' + str(tail) + '" -> "' + str(head) + '"'
-            arc_str += '[headlabel=' + str(arc_count)
-            arc_str += ' labeldistance=2'
-            arc_str += ' labelangle=-50'
+            tail = str(tail)
+            head = str(head)
+
+            arc_str = '\t "' + tail + '" -- "' + head + '"'
+            arc_str += '['
+            #arc_str += 'headlabel=' + str(arc_count)
+            if (x % dim + y % dim) % 2:
+                arc_str += ' color="black"'
+                arc_str += ' style="dashed"'
+            # arc_str += ' penwidth=2'
             arc_str += '];'
 
             print(arc_str)
             arc_count += 1
 
 print('}')
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/bounded-natural.py` & `hiperwalk-2.0b11/docs/graphviz/grid/bounded-natural.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/diagonal-directions.dot` & `hiperwalk-2.0b11/docs/graphviz/grid/diagonal-grid-neigh-order.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/even-dim-diagonal.py` & `hiperwalk-2.0b11/docs/graphviz/grid/periodic-natural.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,49 @@
-print('digraph {')
+print('graph {')
 
-dim = 4
+dim = 3
 
 def out_of_bounds(axis):
     return axis < 0 or axis >= dim 
 
 for y in range(-1, dim + 1):
     for x in range(-1, dim + 1):
         out_x = out_of_bounds(x)
         out_y = out_of_bounds(y)
+        if out_x and out_y:
+            continue
 
         node_str = ('\t"' + str((x, y)) + '" ['
                     + 'pos="' + str(1.75*x) + ',' + str(1.75*y) + '!" '
                     + 'width=0.75 height=0.75 fixedsize=True')
         if out_x or out_y:
             node_str += (' style="dashed" label="' +
                          str((x % dim, y % dim)) + '"')
-
-        if (x % dim + y % dim) % 2:
-            node_str += ' fontcolor="white" fillcolor="red" style="filled'
-            node_str += ',dashed" penwidth=2' if out_x or out_y else '"'
-
         node_str += ']'
 
         print(node_str)
 
 print()
 
-arc_count = 0
 for y in range(dim):
     for x in range(dim):
         tail = str((x, y))
-        for d in range(4):
-            x_shift = 1 if d // 2 == 0 else -1
-            y_shift = 1 if d % 2 == 0 else -1
-            head = str((x + x_shift, y + y_shift))
-
-            arc_str = '\t "' + tail + '" -> "' + head + '"'
-            arc_str += '['
-            #arc_str += 'headlabel=' + str(arc_count)
-            if (x % dim + y % dim) % 2:
-                arc_str += ' color="red"'
-                arc_str += ' style="dashed"'
-            arc_str += ' labeldistance=2'
-            arc_str += ' labelangle=-50'
-            arc_str += ' penwidth=2'
-            arc_str += '];'
+        for d in [0, 2]:
+            y_axis = d // 2
+            shift = 1 if d % 2 == 0 else -1
+            head = (str((x + shift, y)) if not y_axis else
+                    str((x, y + shift)))
+
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
 
             print(arc_str)
-            arc_count += 1
+
+        if x == 0:
+            head = str((-1, y))
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
+            print(arc_str)
+        if y == 0:
+            head = str((x, -1))
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
+            print(arc_str)
 
 print('}')
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/natural-directions.dot` & `hiperwalk-2.0b11/docs/graphviz/grid/natural-grid-neigh-order.dot`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-digraph {
+graph {
 	4 [pos="0,0!" label="(x, y)" width=1 height=1 fixedsize=True;]
 	0 [pos="2,0!" label="(x + 1, y)" width=1 height=1 fixedsize=True;]
 	1 [pos="-2,0!" label="(x - 1, y)" width=1 height=1 fixedsize=True;]
 	2 [pos="0,2!" label="(x, y + 1)" width=1 height=1 fixedsize=True;]
 	3 [pos="0,-2!" label="(x, y - 1)" width=1 height=1 fixedsize=True;]
 
-	4 -> 0 [headlabel=0 labeldistance=4 labelangle=-10];
-	4 -> 1 [headlabel=1 labeldistance=4 labelangle=10];
-	4 -> 2 [headlabel=2 labeldistance=4 labelangle=10];
-	4 -> 3 [headlabel=3 labeldistance=4 labelangle=-10];
+	4 -- 0 [headlabel=0 labeldistance=4 labelangle=-10];
+	4 -- 1 [headlabel=1 labeldistance=4 labelangle=10];
+	4 -- 2 [headlabel=2 labeldistance=4 labelangle=10];
+	4 -- 3 [headlabel=3 labeldistance=4 labelangle=-10];
 }
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/periodic-diagonal.py` & `hiperwalk-2.0b11/docs/graphviz/grid/bounded-diagonal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-print('digraph {')
+print('graph {')
 
 dim = 3
 
 def out_of_bounds(axis):
     return axis < 0 or axis >= dim 
 
-for y in range(-1, dim + 1):
-    for x in range(-1, dim + 1):
+for y in range(dim):
+    for x in range(dim):
         out_x = out_of_bounds(x)
         out_y = out_of_bounds(y)
 
         node_str = ('\t"' + str((x, y)) + '" ['
                     + 'pos="' + str(1.75*x) + ',' + str(1.75*y) + '!" '
                     + 'width=0.75 height=0.75 fixedsize=True')
         if out_x or out_y:
@@ -18,26 +18,23 @@
                          str((x % dim, y % dim)) + '"')
         node_str += ']'
 
         print(node_str)
 
 print()
 
-arc_count = 0
 for y in range(dim):
     for x in range(dim):
         tail = str((x, y))
-        for d in range(4):
+        for d in [0, 2]:
             x_shift = 1 if d // 2 == 0 else -1
             y_shift = 1 if d % 2 == 0 else -1
-            head = str((x + x_shift, y + y_shift))
+            head = (x + x_shift, y + y_shift)
+
+            if out_of_bounds(head[0]) or out_of_bounds(head[1]):
+                continue
 
-            arc_str = '\t "' + tail + '" -> "' + head + '"'
-            arc_str += '[headlabel=' + str(arc_count)
-            arc_str += ' labeldistance=2'
-            arc_str += ' labelangle=-50'
-            arc_str += '];'
+            arc_str = '\t "' + str(tail) + '" -- "' + str(head) + '";'
 
             print(arc_str)
-            arc_count += 1
 
 print('}')
```

### Comparing `hiperwalk-2.0b1/docs/graphviz/grid/periodic-natural.py` & `hiperwalk-2.0b11/docs/graphviz/grid/periodic-diagonal.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-print('digraph {')
+print('graph {')
 
 dim = 3
 
 def out_of_bounds(axis):
     return axis < 0 or axis >= dim 
 
 for y in range(-1, dim + 1):
     for x in range(-1, dim + 1):
         out_x = out_of_bounds(x)
         out_y = out_of_bounds(y)
-        if out_x and out_y:
-            continue
 
         node_str = ('\t"' + str((x, y)) + '" ['
                     + 'pos="' + str(1.75*x) + ',' + str(1.75*y) + '!" '
                     + 'width=0.75 height=0.75 fixedsize=True')
         if out_x or out_y:
             node_str += (' style="dashed" label="' +
                          str((x % dim, y % dim)) + '"')
         node_str += ']'
 
         print(node_str)
 
 print()
 
-arc_count = 0
 for y in range(dim):
     for x in range(dim):
         tail = str((x, y))
-        for d in range(4):
-            y_axis = d // 2
-            shift = 1 if d % 2 == 0 else -1
-            head = (str((x + shift, y)) if not y_axis else
-                    str((x, y + shift)))
-
-            arc_str = '\t "' + tail + '" -> "' + head + '"'
-            arc_str += '[headlabel=' + str(arc_count)
-            arc_str += ' labeldistance=4'
-            arc_str += ' labelangle=-20'
-            arc_str += '];'
+        for d in [0, 2]:
+            x_shift = 1 if d // 2 == 0 else -1
+            y_shift = 1 if d % 2 == 0 else -1
+            head = str((x + x_shift, y + y_shift))
 
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
+            print(arc_str)
+
+        if x == 0 or y == 0:
+            head = str((x -1, y - 1))
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
+            print(arc_str)
+
+        if y == 0 or x == dim - 1:
+            head = str((x + 1, y - 1))
+            arc_str = '\t "' + tail + '" -- "' + head + '";'
             print(arc_str)
-            arc_count += 1
 
 print('}')
```

### Comparing `hiperwalk-2.0b1/docs/install/index.rst` & `hiperwalk-2.0b11/docs/install/index.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,54 @@
 =======
 Install
 =======
 
+You can install Hiperwalk locally or its docker distribution.
+We recommend to use Hiperwalk's docker distribution.
+
+-------------------
+Docker Installation
+-------------------
+
+Using Hiperwalk on its Docker distribution offers
+numerous benefits to users.
+Docker provides a lightweight, portable, and scalable environment,
+ensuring seamless deployment across
+different operating systems and environments.
+With Docker, users can easily manage dependencies,
+streamline updates, and replicate configurations,
+leading to improved consistency and reliability.
+Additionally, Docker enables efficient resource utilization,
+facilitating faster development cycles and easier collaboration
+among team members.
+Overall, opting for Hiperwalk on its Docker distribution
+empowers users with enhanced flexibility, efficiency,
+and agility in their development and deployment processes.
+
+.. todo::
+
+   Add installation guidelines
+
+------------------
+Local Installation
+------------------
+
 Hiperwalk relies on a number of Python libraries.
 However, installing these Python libraries alone does not enable
 Hiperwalk to leverage High-Performance Computing (HPC).
 If you desire to install Hiperwalk with HPC support, please refer
 to :ref:`docs_install_hpc_prerequisites` before proceeding
 with the Hiperwalk installation.
 
 On this page, we outline the process for installing Hiperwalk on
 a newly installed Ubuntu 20.04 operating system. The steps will
 cover identifying the GPU, installing the GPU drivers,
 neblina-core, neblina-opencl-bridge, pyneblina, and
 all necessary Python libraries.
 
-.. warning::
-
-   While currently only Ubuntu 20.04 is supported, we are working
-   diligently to extend support to other distributions as soon as
-   possible.
-
-   We are developing support for Ubuntu 22.04 with the main challenge
-   being the adaptation of plotting features, which currently work well
-   in Jupyter notebooks.
-
 .. _docs_install_hiperwalk:
 
 Hiperwalk
 =========
 
 Hiperwalk can be conveniently installed using pip.
 To begin, ensure that pip is installed on your system.
@@ -57,14 +77,20 @@
 
 To verify the success of the installation,
 you can execute any code found in the
 `examples directory of the repository
 <https://github.com/hiperwalk/hiperwalk/tree/master/examples>`_
 or proceed to the :ref:`docs_tutorial`.
 
+To update an older version of the hiperwalk package:
+
+.. code-block:: shell
+
+   pip3 install hiperwalk --upgrade
+
 .. _docs_install_hpc_prerequisites:
 
 HPC Prerequisites
 =================
 
 Before proceeding, it's advisable to update and upgrade your
 Ubuntu packages. Execute the following commands:
```

### Comparing `hiperwalk-2.0b1/docs/tutorial/index.rst` & `hiperwalk-2.0b11/docs/tutorial/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -53,16 +53,16 @@
 
 Before running the simulation, we need to specify the initial state. 
 One way to accomplish this is by using the
 :meth:`hiperwalk.Coined.ket` method,
 which generates a state of the computational basis.
 
 >>> vertex = N // 2
->>> initial_state = qw.ket(vertex, vertex + 1)
->>> initial_state
+>>> state = qw.ket((vertex, vertex + 1))
+>>> state
 array([0., 0., 0., 0., 0., 0., 0., 0., 0., 1., 0., 0., 0., 0., 0., 0., 0.,
        0., 0., 0.])
 
 This state corresponds to the walker on
 vertex 5 with the coin pointing to vertex 6
 (keep in mind that the vertex numbers range from 0 to 10).
 
@@ -72,15 +72,15 @@
 When specifying only the final time,
 the output will be the final state.
 If everything was installed correctly,
 the :meth:`hiperwalk.Coined.simulate` method will automatically use
 high-performance computing to perform the matrix-vector multiplications.
 
 >>> final_state = qw.simulate(time=N//2,
-...                           initial_state=initial_state)
+...                           state=state)
 
 
 
 Display the results
 -------------------
 
 Presenting the results can be as straightforward as printing them.
@@ -123,9 +123,10 @@
 
 The remainder of the tutorial is split into the following sections.
 
 .. toctree::
     :maxdepth: 1
 
     graphs.rst
+    graph_constructors.rst
     quantum_walk_models.rst
     plotting.rst
```

### Comparing `hiperwalk-2.0b1/docs/tutorial/plotting.rst` & `hiperwalk-2.0b11/docs/tutorial/plotting.rst`

 * *Files 6% similar despite different names*

```diff
@@ -51,32 +51,36 @@
 
 >>> import hiperwalk as hpw
 >>> dim = 7
 >>> lat = hpw.Grid(dim)
 >>> center = (dim//2, dim//2)
 >>> right = (center[0] + 1, center[1])
 >>> qw = hpw.Coined(lat, shift='persistent', coin='grover')
->>> psi0 = qw.state([0.5, (center, right)],
-...                 [0.5, (right, center)])
->>> psi = qw.simulate(time=dim//2, initial_state=psi0)
+>>> psi0 = qw.state([[0.5, (center, right)],
+...                  [0.5, (right, center)]])
+>>> psi = qw.simulate(time=dim//2, state=psi0)
 >>> prob = qw.probability_distribution(psi)
 >>> prob
-array([[0.       , 0.       , 0.       , 0.0078125, 0.0078125, 0.       ,
-        0.       , 0.       , 0.       , 0.0078125, 0.0390625, 0.0390625,
-        0.0078125, 0.       , 0.       , 0.0078125, 0.0390625, 0.0390625,
-        0.0390625, 0.0390625, 0.0078125, 0.015625 , 0.0078125, 0.1953125,
-        0.0078125, 0.0078125, 0.1953125, 0.0078125, 0.       , 0.0078125,
-        0.0390625, 0.0390625, 0.0390625, 0.0390625, 0.0078125, 0.       ,
-        0.       , 0.0078125, 0.0390625, 0.0390625, 0.0078125, 0.       ,
-        0.       , 0.       , 0.       , 0.0078125, 0.0078125, 0.       ,
+array([[0.       , 0.       , 0.       , 0.015625 , 0.       , 0.       ,
+        0.       , 0.       , 0.       , 0.0078125, 0.0078125, 0.0078125,
+        0.       , 0.       , 0.       , 0.0078125, 0.0390625, 0.1953125,
+        0.0390625, 0.0078125, 0.       , 0.0078125, 0.0390625, 0.0390625,
+        0.0078125, 0.0390625, 0.0390625, 0.0078125, 0.0078125, 0.0390625,
+        0.0390625, 0.0078125, 0.0390625, 0.0390625, 0.0078125, 0.       ,
+        0.0078125, 0.0390625, 0.1953125, 0.0390625, 0.0078125, 0.       ,
+        0.       , 0.       , 0.0078125, 0.0078125, 0.0078125, 0.       ,
         0.       ]])
 
 Bar Plot
 ''''''''
 
+.. todo::
+
+   Fix plots
+
 The vertices are represented on the x-axis.
 The respective probabilities are represented on the y-axis.
 Each vertex is associated with a bar.
 
 >>> hpw.plot_probability_distribution(prob, plot='bar') #doctest: +SKIP
 
 .. image:: bar.png
@@ -95,14 +99,18 @@
 
 Histogram Plot
 ''''''''''''''
 
 This is essentially the same as the bar plot
 but the ``width`` kwarg is *overriden* so the bars are not separated.
 
+>>> hpw.plot_probability_distribution(prob,
+...                                   plot='histogram') #doctest: +SKIP
+
+
 .. image:: histogram.png
 
 Line Plot
 '''''''''
 
 The vertices are represented on the x-axis.
 The respective probabilities are represented on the y-axis.
@@ -113,19 +121,14 @@
 
 .. image:: line.png
 
 It is built on top of :obj:`matplotlib.pyplot.plot`.
 The respective valid matplotlib keywords can be used to customize the plot.
 
 >>> hpw.plot_probability_distribution(
-...     prob, plot='bar', color='red', edgecolor='black', linewidth=3,
-...     tick_label=[str((x, y)) for x in range(dim) for y in range(dim)]
-... ) #doctest: +SKIP
-
->>> hpw.plot_probability_distribution(
 ...     prob, plot='line', linewidth=3, color='black', linestyle='--',
 ...     marker='X', markerfacecolor='yellow', markersize=15,
 ...     markeredgewidth=2, markeredgecolor='red') #doctest: +SKIP
 
 .. image:: custom_line.png
 
 Plane Plot
@@ -211,15 +214,15 @@
 * ``max_node_size``
 
 In this tutorial, only two keywords are detailed:
 ``animate`` and ``rescale``.
 For better comprehension and visualization,
 the probabilities of the intermediate simulation steps are saved.
 
->>> psi = qw.simulate(time=(dim//2, 1), initial_state=psi0)
+>>> psi = qw.simulate(time=(dim//2, 1), state=psi0)
 >>> prob = qw.probability_distribution(psi)
 
 ``animate``
 '''''''''''
 
 If multiple probabilites are stored,
 the ``animate`` keyword can be used to generate an animation.
@@ -241,8 +244,11 @@
 the walker (and the probabilities) tend to spread.
 Consequently, in later simulation steps,
 it may be hard to visualize the probabilities.
 If ``rescale`` is set to ``True``, each plot is rescaled such that
 the maximum probability of the current plot corresponds to
 the maximum value on the axis.
 
+>>> hpw.plot_probability_distribution(
+...     prob, graph=lat, animate=True, rescale=True) #doctest: +SKIP
+
 .. image:: rescale.gif
```

### Comparing `hiperwalk-2.0b1/examples/Untitled-Copy1.ipynb` & `hiperwalk-2.0b11/examples/Untitled-Copy1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/Untitled.ipynb` & `hiperwalk-2.0b11/examples/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/Untitled1.ipynb` & `hiperwalk-2.0b11/examples/Untitled1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/Untitled2.ipynb` & `hiperwalk-2.0b11/examples/Untitled2.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/Untitled3.ipynb` & `hiperwalk-2.0b11/examples/Untitled3.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/Untitled4.ipynb` & `hiperwalk-2.0b11/examples/Untitled4.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/coined-diagonal-grid.py` & `hiperwalk-2.0b11/examples/coined-diagonal-grid.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import hiperwalk as hpw
 import numpy as np
 
 dim = 121
-grid = hpw.Grid(dim, diagonal=True)
-center = np.array([dim // 2, dim // 2])
+grid = hpw.Grid(dim, diagonal=True, periodic=False)
 dtqw = hpw.Coined(grid, shift='persistent', coin='grover')
-psi0 = dtqw.state([0.5, (center, center + (1, 1))],
-                  [-0.5, (center, center + (1, -1))],
-                  [-0.5, (center, center + (-1, 1))],
-                  [0.5, (center, center + (-1, -1))])
-psi_final = dtqw.simulate(time=dim // 2, initial_state=psi0, hpc=False)
+center = np.array([dim // 2, dim // 2])
+psi0 = dtqw.state([[0.5, (center, center + (1, 1))],
+                   [-0.5, (center, center + (1, -1))],
+                   [-0.5, (center, center + (-1, 1))],
+                   [0.5, (center, center + (-1, -1))]])
+psi_final = dtqw.simulate(time=dim // 2, state=psi0)
 prob = dtqw.probability_distribution(psi_final)
 hpw.plot_probability_distribution(prob, graph=grid)
```

### Comparing `hiperwalk-2.0b1/examples/deleteme.py` & `hiperwalk-2.0b11/examples/deleteme.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/exemplo1.ipynb` & `hiperwalk-2.0b11/examples/exemplo1.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/examples/issue13.py` & `hiperwalk-2.0b11/examples/issue13.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/hiperwalk/graph/graph.py` & `hiperwalk-2.0b11/hiperwalk/graph/integer_lattice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,344 +1,362 @@
+from abc import ABC, abstractmethod
 import numpy as np
-from scipy.sparse import issparse, csr_array
+from scipy.sparse import csr_array
+from scipy.sparse import eye as sparse_eye
+from .graph import Graph
+from types import MethodType
+
+def __generate_valid_basis(euc_dim, basis=None):
+    if basis is None:
+        basis = np.arange(1, euc_dim + 1)
+
+    try:
+        basis.shape
+    except AttributeError:
+        basis = np.array(basis)
+
+    if basis.shape[0] == euc_dim:
+        # add negative arrays to basis
+        # this explicits the neighbor order
+        basis = np.concatenate((basis, -basis))
+
+    if basis.shape[0] != 2*euc_dim:
+        raise ValueError("Invalid number of basis vectors. "
+                         + str(euc_dim)
+                         + " or "
+                         + str(2*euc_dim)
+                         + " were expected.")
+
+    if len(basis.shape) == 1:
+        # generate standard basis
+        valid_basis = np.zeros((basis.shape[0], euc_dim), dtype=np.int8)
+
+        for i in range(basis.shape[0]):
+            entry = basis[i]
+            positive = entry > 0
+            entry = entry if positive else -entry
+            entry = entry - 1
+            valid_basis[i, entry] = 1 if positive else - 1
+
+        basis = valid_basis
+
+    return basis
+
+def __create_adj_matrix(graph):
+    num_vert = graph.number_of_vertices()
+
+    indices = [[]]*num_vert
+    indptr = np.zeros(num_vert + 1, dtype=np.int32)
+
+    for v in range(num_vert):
+        coord = graph.vertex_coordinates(v)
+
+        neigh = np.array([coord + graph._basis[i]
+                          for i in range(len(graph._basis))])
+
+        if not graph._periodic:
+            adj = [graph._valid_vertex(n, exception=False)
+                   for n in neigh]
+            neigh = neigh[adj]
+
+        indices[v] = [graph.vertex_number(n) for n in neigh]
+        indptr[v + 1] = indptr[v] + len(neigh)
+
+    if graph._periodic:
+        indices = np.reshape(indices, indptr[-1])
+    else:
+        indices = np.array([elem for l in indices for elem in l],
+                           dtype=np.int32)
+    data = np.ones(indptr[-1], dtype=np.int8)
+
+    adj_matrix = csr_array((data, indices, indptr), copy=False)
+    return adj_matrix
+
+def _valid_vertex(self, vertex, exception=False):
+    try:
+        # coordinates
+        if len(vertex) != self._euc_dim:
+            if not exception:
+                return False
+            raise ValueError("Vertex is not a "
+                             + str(self._euc_dim)
+                             + "-tuple.")
+
+        if self._periodic:
+            return True
+
+        for i in range(self._euc_dim):
+            if vertex[i] < 0 or vertex[i] >= self._dim[i]:
+                if not exception:
+                    return False
+                raise ValueError("Inexistent vertex"
+                                 + str(vertex) + ". "
+                                 + "Lattice is not periodic.")
+
+    except TypeError:
+        # number
+        if vertex < 0 or vertex >= self.number_of_vertices():
+            if not exception:
+                return False
+            raise ValueError("Inexistent vertex " + str(vertex))
+
+    return True
+
+def vertex_number(self, coordinates):
+    self._valid_vertex(coordinates, exception=True)
+    # number
+    try:
+        len(coordinates)
+    except TypeError:
+        return coordinates
+
+    # coordinates
+    coordinates = list(coordinates)
+    dim = self._dim
+    mult = 1
+    number = 0
+    for i in range(self._euc_dim - 1, -1, -1):
+        if self._periodic:
+            coordinates[i] = coordinates[i] % self._dim[i]
 
-def _binary_search(v, elem, start=0, end=None):
+        number += mult*coordinates[i]
+        mult *= dim[i]
+
+    return number
+
+def vertex_coordinates(self, vertex):
     r"""
-    This function expects a sorted array and performs a binary search on the subarray 
-    v[start:end], looking for the element 'elem'. 
-    If the element is found, the function returns the index of the element. 
-    If the element is not found, the function returns -1.    
-    This is an implementation of binary search following Cormen's algorithm. 
-    It is used to improve the time complexity of the search process.
+    Return the coordinates of the given vertex.
+
+    Given the number of a vertex,
+    return the corresponding coordinates in the integer lattice.
+
+    Returns
+    -------
+    :class:`numpy.ndarray`
+
+    See Also
+    --------
+    hiperwalk.Graph.vertex_number
+
+    Notes
+    -----
+    The vertex number depends on its coordinates and the
+    dimension of the lattice ``dim``.
+    If the coordinates of a vertex are ``(v[0], ..., v[n-1])``,
+    its number is
+    ``v[n-1] + dim[n-1]*v[n-2] + ... + dim[n-1]*...*dim[1]*v[0]``.
+
+    Examples
+    --------
+    .. testsetup::
+
+        import hiperwalk as hpw
+
+    The methods ``vertex_coordinates`` is the inverse of
+    ``vertex_number``, and vice versa.
+
+    .. doctest::
+
+        >>> g = hpw.IntegerLattice((3, 3, 3))
+        >>> tuple(g.vertex_coordinates(0))
+        (0, 0, 0)
+        >>> g.vertex_number((0, 0, 0))
+        0
+        >>> tuple(g.vertex_coordinates(13))
+        (1, 1, 1)
+        >>> g.vertex_number((1, 1, 1))
+        13
     """
+    self._valid_vertex(vertex, exception=True)
+
+    dim = self._dim.copy()
+
+    # coordinates
+    try:
+        len(vertex)
+        if self._periodic:
+            for i in range(self._euc_dim):
+                vertex[i] = vertex[i] % dim[i]
+
+        return vertex
+
+    except TypeError:
+        pass
 
-    if end == None:
-        end = len(v)
-    
-    while start < end:
-        mid = int((start + end)/2)
-        if elem <= v[mid]:
-            end = mid
-        else:
-            start = mid + 1
+    # input is number
+    mult = np.prod(dim, dtype=np.int64)
+    coordinates = np.zeros(self._euc_dim, dtype=np.int32)
+    for i in range(self._euc_dim - 1):
+        mult = mult // dim[i]
+        coordinates[i] = vertex // mult
 
-    return end if v[end] == elem else -1
+        # TODO: check which one is more efficient
+        vertex = vertex % mult
+        # vertex -= coordinates[i]*mult
 
-class Graph():
+    coordinates[-1] = vertex
+
+    return coordinates
+
+def dimensions(self):
     r"""
-    Arbitrary graph.
+    Dimensions of integer lattice.
+
+    Returns
+    -------
+    dim : tuple of int
+        ``dim[i]`` is the number of vertices in the ``i``-th axis.
+    """
+    return self._dim
+
+def neighbors(self, vertex):
+    v_num = self.vertex_number(vertex)
+    start = self._adj_matrix.indptr[v_num]
+    end = self._adj_matrix.indptr[v_num + 1]
+    neighs = self._adj_matrix.indices[start:end]
+
+    if hasattr(vertex, '__iter__'):
+        neighs = np.array([self.vertex_coordinates(n) for n in neighs],
+                           dtype=neighs.dtype)
 
-    The graph on which a quantum walk takes place.
+    return neighs
+
+def IntegerLattice(dim, basis=None, periodic=True,
+                  multiedges=None, weights=None):
+    r"""
+    Integer lattice graph.
+
+    An integer lattice is a lattice in an euclidean space
+    such that every point is a tuple of integers.
+    In the integer lattice graph,
+    every vertex corresponds to a lattice point.
 
     Parameters
     ----------
-    adj_matrix : :class:`scipy.sparse.csr_array` or :class:`numpy.ndarray`
-        Adjacency matrix of the graph on
-        which the quantum walk takes place.
-
-    Raises
-    ------
-    TypeError
-        if ``adj_matrix`` is not an square matrix.
+    dim : tuple of int
+        Lattice dimensions where
+        ``dim[i]`` is the number of vertices in the ``i``-th-axis.
+
+    basis : list of int or matrix, default=None
+        Vectors used to determine the graph adjacency and
+        the corresponding order of neighbors.
+        ``basis`` can be specified in three different ways.
+        Let ``n = len(dim)``.
+
+        * ``None``
+            Equivalent to the argument ``[1, ..., n]``.
+
+        * list of int
+            Adjacency is described by the standard basis where
+            ``i`` corresponds to the array with all entries
+            equal to ``0`` and the ``i-1``-th entry equal to ``1``.
+            Analogously, ``-i`` corresponds to the same array
+            but in the opposite direction (``-1`` instead of ``1``).
+
+            The values of ``basis`` must satisfy
+            ``1 <= abs(basis) <= n``.
+            Note that 0 is not a valid value because
+            ``-0 == 0``.
+
+            It is expected that ``len(basis) == 2*n`` or
+            ``len(basis) == n``.
+            If ``len(basis) == n``,
+            the equivalent argument is
+
+            .. code-block:: python
+
+                [basis[0], ..., basis[n - 1],
+                 -basis[0], ..., -basis[n - 1]]
+
+        * matrix
+            A matrix with ``2*n`` rows and ``n`` columns.
+            The ``i``-th neighbor of the
+            vertex with coordinates ``(v[0], ..., v[n-1])`` is
+            ``(v[0] + basis[i][0], ..., v[n-1] + basis[i][n-1])``.
+
+
+    periodic : bool, default=True
+        ``True`` if the grid has cyclic boundary conditions,
+        ``False`` if it has borders.
+
+    multiedges, weights: scipy.sparse.csr_array, default=None
+        See :ref:`graph_constructors`.
+
+    Returns
+    -------
+    :class:`hiperwalk.Graph`
+        See :ref:`graph_constructors` for details.
+
+    See Also
+    --------
+    :ref:`graph_constructors`.
 
     Notes
     -----
-    .. todo::
-        Check if it is more efficient to store the adjacency matrix as
-        sparse or dense.
-
-    A wide range of methods are available. 
-    These methods can be used by a quantum walk model 
-    to generate a valid quantum walk.
-    
-    This class can be passed as an argument to plotting functions.
-    In this case,
-    the default representation for the graph will be displayed.
-
-    The recommended parameter type is
-    :class:`scipy.sparse.csr_array` with ``dtype=np.int8``,
-    where 1 denotes adjacency and 0 denotes non-adjacency.
-    If any entry differs from 0 or 1,
-    some methods may not operate as expected.
-
-    Each edge of a given graph :math:`G(V, E)` is associated with
-    two arcs in the symmetric digraph :math:`\vec{G}(V, A)`,
-    where
-
-    .. math::
-        \begin{align*}
-            A = \bigcup_{(v,u) \in E} \{(v, u), (u, v)\}.
-        \end{align*}
-
-    An arc can be described either in the arc notation as (tail,head) 
-    or through a numerical label. The ordering of the labels in 
-    the :obj:`Graph` class is as follows: 
-    Consider two arcs, :math:`(v_1, u_1)` and :math:`(v_2, u_2')`, 
-    with numerical labels :math:`a_1` and :math:`a_2` respectively. 
-    Then, :math:`a_1 < a_2` if and only if either :math:`v_1 < v_2` 
-    or :math:`v_1 = v_2` and :math:`u_1 < u_2`.
+    The **order of neighbors** depends on the value of ``basis``.
 
-    .. note::
-        The arc ordering may change for graphs defined using specific classes.
+    The vertex number depends on its coordinates and ``dim``.
+    If the coordinates of a vertex are ``(v[0], ..., v[n-1])``,
+    its number is
+    ``v[n-1] + dim[n-1]*v[n-2] + ... + dim[n-1]*...*dim[1]*v[0]``.
 
-    For example, the graph :math:`G(V, E)` shown in
-    Figure 1 has an adjacency matrix ``adj_matrix``.
+    Examples
+    --------
 
     .. testsetup::
 
-        import numpy as np
+        import hiperwalk as hpw
 
-    >>> adj_matrix = np.array([
-    ...     [0, 1, 0, 0],
-    ...     [1, 0, 1, 1],
-    ...     [0, 1, 0, 1],
-    ...     [0, 1, 1, 0]])
-    >>> adj_matrix
-    array([[0, 1, 0, 0],
-           [1, 0, 1, 1],
-           [0, 1, 0, 1],
-           [0, 1, 1, 0]])
-
-    .. graphviz:: ../../graphviz/graph-example.dot
-        :align: center
-        :layout: neato
-        :caption: Figure 1
-
-    The arcs of the associated digraph in the arc notation are
-
-    >>> arcs = [(i, j) for i in range(4)
-    ...                for j in range(4) if adj_matrix[i,j] == 1]
-    >>> arcs
-    [(0, 1), (1, 0), (1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2)]
-
-    Note that ``arcs`` is already sorted, hence the associated 
-    numeric labels are
-
-    >>> arcs_labels = {arcs[i]: i for i in range(len(arcs))}
-    >>> arcs_labels
-    {(0, 1): 0, (1, 0): 1, (1, 2): 2, (1, 3): 3, (2, 1): 4, (2, 3): 5, (3, 1): 6, (3, 2): 7}
-
-    The numeric labels are depicted in Figure 2.
-
-    .. graphviz:: ../../graphviz/graph-arcs.dot
-        :align: center
-        :layout: neato
-        :caption: Figure 2
-
-    If we insert the labels of the arcs into the adjacency matrix,
-    we obtain matrix ``adj_labels`` as follows:
-
-    >>> adj_labels = [[arcs_labels[(i,j)] if (i,j) in arcs_labels
-    ...                                   else '' for j in range(4)]
-    ...               for i in range(4)]
-    >>> adj_labels = np.matrix(adj_labels)
-    >>> adj_labels
-    matrix([['', '0', '', ''],
-            ['1', '', '2', '3'],
-            ['', '4', '', '5'],
-            ['', '6', '7', '']], dtype='<U21')
+    .. doctest::
 
-    Note that, intuitively,
-    the arcs are labeled in left-to-right and top-to-bottom fashion.
-    """
+        >>> g = hpw.IntegerLattice((3, 3), basis=None)
+        >>> neigh = g.neighbors((1, 1))
+        >>> [tuple(g.vertex_coordinates(v)) for v in neigh]
+        [(2, 1), (1, 2), (0, 1), (1, 0)]
 
-    def __init__(self, adj_matrix):
-        # TODO:
-        # * Check if valid adjacency matrix
-        # * Add option: numpy dense matrix as parameters.
-        # * Add option: networkx graph as parameter.
-        if not issparse(adj_matrix):
-            adj_matrix = csr_array(adj_matrix, dtype=np.int8)
-
-        if adj_matrix.shape[0] != adj_matrix.shape[1]:
-            raise TypeError("Adjacency matrix is not square.")
-
-        # the following is commented because the current way to
-        # implement Laplacian in ContinuousTime quantum walks is by
-        # passing the Laplacian as adjacency matrix
-        # if adj_matrix.data.min() != 1 or adj_matrix.data.max() != 1:
-        #     raise ValueError("Adjacency matrix must only have 0's "
-        #                      + "and 1's as entries.")
-
-        self._adj_matrix = adj_matrix
-        self._coloring = None
-
-    def arc_number(self, *args):
-        r"""
-        Returns the numerical label of the arc.
-
-        Parameters
-        ----------
-        *args:
-            int:
-                The numerical arc label itself is passed
-                as argument.
-            (tail, head):
-                Arc in arc notation.
-            tail, head:
-                Arc in arc notation,
-                but ``tail`` and ``head`` are passed as
-                different arguments, not as a tuple.
-
-        Returns
-        -------
-        label: int
-            Arc label.
-
-        Examples
-        --------
-        If arc ``(0, 1)`` exists, the following commands return
-        the same result.
-
-        .. testsetup::
-
-            import networkx as nx
-            from sys import path
-            path.append('../..')
-            import hiperwalk as hpw
-            nxg = nx.cycle_graph(10)
-            adj_matrix = nx.adjacency_matrix(nxg)
-            graph = hpw.Graph(adj_matrix)
+    .. doctest::
 
-        >>> graph.arc_number(0) #arc number 0
-        0
-        >>> graph.arc_number((0, 1)) #arc as tuple
-        0
-        >>> graph.arc_number(0, 1) #tail and head in separate arguments
-        0
-        """
-        arc = (args[0], args[1]) if len(args) == 2 else args[0]
+        >>> g = hpw.IntegerLattice((3, 3), basis=[-1, -2])
+        >>> neigh = g.neighbors((1, 1))
+        >>> [tuple(g.vertex_coordinates(v)) for v in neigh]
+        [(0, 1), (1, 0), (2, 1), (1, 2)]
 
-        if not hasattr(arc, '__iter__'):
-            num_arcs = self.number_of_arcs()
-            if arc < 0 and arc >= num_arcs:
-                raise ValueError("Arc value out of range. "
-                                 + "Expected arc value from 0 to "
-                                 + str(num_arcs - 1))
-            return int(arc)
-
-        tail, head = arc
-        arc_number = _binary_search(self._adj_matrix.indices, head,
-                                   start = self._adj_matrix.indptr[tail],
-                                   end = self._adj_matrix.indptr[tail + 1])
-        if arc_number == -1:
-            raise ValueError("Inexistent arc " + str(arc) + ".")
-        return arc_number
-
-    def arc(self, number):
-        r"""
-        Converts the arc number to arc notation.
-
-        Given the arc number,
-        returns the arc in the ``(tail, head)`` notation.
-
-        Parameters
-        ----------
-        number: int
-            The arc number
-
-        Returns
-        -------
-        (int, int)
-            Arc in the arc notation ``(tail, head)``.
-        """
-        adj_matrix = self._adj_matrix
-        head = adj_matrix.indices[number]
-        #TODO: binary search
-        for tail in range(len(adj_matrix.indptr)):
-            if adj_matrix.indptr[tail + 1] > number:
-                break
-        return (tail, head)
-
-    def neighbors(self, vertex):
-        r"""
-        Returns all neighbors of the given vertex.
-        """
-        start = self._adj_matrix.indptr[vertex]
-        end = self._adj_matrix.indptr[vertex + 1]
-        return self._adj_matrix.indices[start:end]
-
-    def arcs_with_tail(self, tail):
-        r"""
-        Returns all arcs that have the given tail.
-        """
-        arcs_lim = self._adj_matrix.indptr
-        return np.arange(arcs_lim[tail], arcs_lim[tail + 1])
-
-    def number_of_vertices(self):
-        r"""
-        Cardinality of vertex set.
-        """
-        return self._adj_matrix.shape[0]
-
-    def number_of_arcs(self):
-        r"""
-        Cardinality of arc set.
-
-        For simple graphs, the cardinality is twice the number of edges.
-        """
-        return self._adj_matrix.sum()
-
-    def number_of_edges(self):
-        r"""
-        Cardinality of edge set.
-        """
-        return self._adj_matrix.sum() >> 1
-
-    def degree(self, vertex):
-        r"""
-        Degree of given vertex.
-        """
-        indptr = self._adj_matrix.indptr
-        return indptr[vertex + 1] - indptr[vertex]
-
-    def vertex_number(self, vertex):
-        r"""
-        Returns vertex number given any vertex representation.
-
-        By invoking this method,
-        the vertex number is returned regardless of its representation.
-        There are some graphs in which a vertex may have multiple
-        representations.
-        For example, coordinates in a grid.
-        For general graphs,
-        this function returns the argument itself if valid.
-
-        Parameters
-        ----------
-        vertex: int
-            The vertex in any of its representation.
-            For general graphs,
-            only its label is accepted.
-
-        Returns
-        -------
-        int
-            Vertex number.
-
-        Notes
-        -----
-        It is useful to have this function implemented for general graphs
-        to simplify the implementation of some quantum walk methods.
-        """
-        vertex = int(vertex)
-        num_vert = self.number_of_vertices()
-        if vertex < 0 or vertex >= num_vert:
-            raise ValueError("Vertex label out of range. " +
-                             "Expected integer value from 0 to" +
-                             str(num_vert - 1))
-        return vertex
+    .. doctest::
+
+        >>> basis = [[0, 1], [-1, 1], [1, -1], [0, -1]]
+        >>> g = hpw.IntegerLattice((3, 3), basis=basis)
+        >>> neigh = g.neighbors((1, 1))
+        >>> [tuple(g.vertex_coordinates(v)) for v in neigh]
+        [(1, 2), (0, 2), (2, 0), (1, 0)]
+
+    """
+    if weights is not None or multiedges is not None:
+        raise NotImplementedError()
+
+    if not hasattr(dim, '__iter__'):
+        dim = [dim]
+    dim = np.array(dim)
+    num_vert = np.prod(dim)
+
+    # create toy graph
+    g = Graph(sparse_eye(num_vert).tocsr())
+
+    # modify toy graph to IntegerLattice
+    g._dim = dim
+    g._periodic = periodic
+    g._euc_dim = len(g._dim) # euclidian space dimension
+    g._num_loops = 0
+
+    # use provided (or generated) basis
+    g._basis = __generate_valid_basis(g._euc_dim, basis)
+
+    # bind methods before updating adjacency matrix
+    g._valid_vertex = MethodType(_valid_vertex, g)
+    g.vertex_number = MethodType(vertex_number, g)
+    g.vertex_coordinates = MethodType(vertex_coordinates, g)
+    g.dimensions = MethodType(dimensions, g)
+
+    #create adjacency matrix
+    g._set_adj_matrix(__create_adj_matrix(g))
 
-    def adjacency_matrix(self):
-        r"""
-        Returns the graph adjacency matrix.
-
-        Returns
-        -------
-        :class:`scipy.sparse.csr_array`.
-
-        Notes
-        -----
-        .. todo::
-            Add other return types depending on the stored matrix type.
-        """
-        return self._adj_matrix
+    return g
```

### Comparing `hiperwalk-2.0b1/hiperwalk/plot/_plot.py` & `hiperwalk-2.0b11/hiperwalk/plot/_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,42 +2,38 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from PIL import Image
 from .._constants import __DEBUG__
 from ..graph import *
 from ..quantum_walk import QuantumWalk
 from matplotlib.animation import FuncAnimation
+from scipy.sparse import csr_array
 
 if __DEBUG__:
     from time import time
 
-# TODO: move to constants
-plt.rcParams["figure.figsize"] = (12, 10)
-plt.rcParams["figure.dpi"] = 100
-
-
-# TODO: add option for changing figsize and dpi
 # histogram is alias for bar width=1
 def plot_probability_distribution(
         probabilities, plot=None, animate=False, show=True,
-        filename=None, interval=250, **kwargs):
+        filename=None, interval=250, figsize=(12, 10), dpi=100, **kwargs):
     """
-    Plots probability distribution of quantum walk.
+    Plot the probability distributions of quantum walk states.
 
-    The probability distribution of multiple steps of a quantum walk
-    may be plotted.
-    The generated figures may be shown step-by-step,
-    saved in multiple files, animated or saved as animation.
+    This function allows plotting the probability distributions 
+    for multiple steps of a quantum walk evolution.
+    The generated figures can be displayed step-by-step, 
+    saved as individual files, or used to create and save animations.
 
     Parameters
     ----------
     probabilities : :class:`numpy.ndarray`
-        The probabilities of the walker to be found on each step
-        of the quantum walk.
-        Columns represent vertices and rows represent the walk steps.
+        An array representing the probabilities of the walker being 
+        found at each vertex during the quantum walk evolution.
+        Each column corresponds to a vertex, 
+        while each row represents a step in the walk.
     plot : str, default=None
         The plot type.
         The valid options are
         ``{'bar', 'line', 'graph', 'histogram', 'plane'}``.
         If ``None``, uses default plotting. Usually ``bar``,
         but default plotting changes according to ``graph``.
     show : bool, default=True
@@ -59,24 +55,24 @@
         the plot(s) will be saved.
         If ``None`` no file is saved.
         Otherwise, if ``animate==False``,
         the j-step is saved in the ``filename-j.png`` file;
         if ``animate==True``,
         the entire walk is saved in the ``filename.fig`` file.
     graph : optional
-        The structure of the graph on which the walk occurs.
+        The structure of the graph on which the walk takes place.
         The graph labels are used as plotting labels.
         **Important**: check Graph Plots subsection in other parameters.
 
         The following types are acceptable.
         
         * :class:`hiperwalk.Graph`
             Hiperwalk Graph.
             It is used to generate default plotting for specific graphs.
-            Does not override values explicited by the user.
+            User-specified values are not overridden.
         * :class:`networkx.classes.graph`,
             NetworkX Graph
         * :class:`scipy.sparse.csr_matrix`
             Adjacency matrix.
     rescale : bool, optional
         If ``False`` or omitted, the reference maximum probability
         is the global one.
@@ -92,14 +88,19 @@
         the step maximum node size shown is 3000.
     animate : bool, default=False
         Whether or not to animate multiple plots.
         If ``False``, each quantum walk step generates an image.
         If ``True``, each quantum walk step is used as an animation frame.
     interval : int, default=250
         Time in milliseconds that each frame is shown if ``animate==True``.
+    figsize : tuple, default=(12, 10)
+        Figure size in inches. Must be a tuple in the format (WIDTH, HEIGHT).
+    dpi : float, default=100
+        Figure resolution in dots-per-inch.
+
     **kwargs : dict, optional
         Extra arguments to further customize plotting.
         Valid arguments depend on ``plot``.
         Check Other Parameters Section for details.
 
     Other Parameters
     ----------------
@@ -192,14 +193,23 @@
         - Implement GTK 4.0 support.
 
     Examples
     --------
     .. todo::
         probabilities expects numpy array or matrix
     """
+    # Figure size
+
+    if len(figsize) == 2:
+        fig_width, fig_height = figsize
+    else:
+        raise ValueError(
+            'figsize must be a tuple in the format (WIDTH, HEIGHT)'
+        )
+
     # passes kwargs by reference to be updated accordingly
 
     if 'graph' in kwargs:
         plot = _default_graph_kwargs(kwargs, plot)
 
     if plot is None:
         plot = 'bar'
@@ -242,41 +252,46 @@
         valid_plots[2]: _update_animation_graph,
         valid_plots[3]: _update_animation_bars,
         valid_plots[4]: None
     }
 
     # preparing probabilities to shape requested by called functions
     if len(probabilities.shape) == 1:
-        probabilities = [probabilities]
+        probabilities = np.array([probabilities])
 
     # passes kwargs by reference to be updated accordingly
     preconfigs[plot](probabilities, kwargs)
 
     if not animate:
         for i in range(len(probabilities)):
             # TODO: set figure size according to graph dimensions
             # TODO: check for kwargs
-            fig, ax = configs[plot](probabilities.shape[1]) 
+            fig, ax = configs[plot](fig_width=fig_width,
+                                    fig_height=fig_height,
+                                    dpi=dpi)
 
             plot_funcs[plot](probabilities[i], ax, **kwargs)
 
             plt.tight_layout()
 
             # saves or shows image (or both)
             if filename is not None:
                 filename_suffix = str(i).zfill(
                         len(str(len(probabilities) - 1)))
-                plt.savefig(filename + '-' + filename_suffix)
+                plt.savefig(filename if len(probabilities) == 1
+                            else filename + '-' + filename_suffix)
                 if not show:
                     plt.close()
             if show:
                 plt.show()
 
     else:
-        fig, ax = configs[plot](probabilities.shape[1]) 
+        fig, ax = configs[plot](fig_width=fig_width,
+                                fig_height=fig_height,
+                                dpi=dpi)
 
         if plot == 'plane':
             from functools import partial
             surf, cbar = plot_funcs[plot](probabilities[0], ax,
                                           **kwargs)
 
             anim = FuncAnimation(
@@ -308,15 +323,15 @@
         if filename is not None:
             anim.save(filename)
         if show:
             if _is_in_notebook():
                 from IPython import display
 
                 # embedding animation in jupyter notebook
-                video = anim.to_html5_video()
+                video = anim.to_jshtml()
                 html = display.HTML(video)
                 display.display(html)
 
                 plt.close()
             else:
                 plt.show()
 
@@ -328,41 +343,47 @@
 
     if 'cmap' in kwargs:
         if kwargs['cmap'] == 'default':
             kwargs['cmap'] = 'viridis'
 
     graph = kwargs['graph']
 
-    # hiperwalk graph
-    if isinstance(graph, Grid):
+    # Hiperwalk Grid
+    if hasattr(graph, '_euc_dim') and graph._euc_dim == 2:
         if plot is None:
             plot = 'plane'
         if plot == 'plane' and 'dimensions' not in kwargs:
             kwargs['dimensions'] = graph.dimensions()
         return plot
 
-    if isinstance(graph, Hypercube):
-        if plot is None:
-            plot = 'graph'
-
-            nx_graph = nx.from_scipy_sparse_array(graph.adjacency_matrix())
-            for v in nx_graph:
-                try:
-                    nx_graph.nodes[v]["subset"] = v.bit_count()
-                except AttributeError:
-                    nx_graph.nodes[v]["subset"] = bin(v).count('1')
-
-            kwargs['pos'] = nx.multipartite_layout(nx_graph)
-            dim = graph.dimension()
-            kwargs['graph'] = nx_graph
-            kwargs['edge_color'] = (0, 0, 0, max(0.002, 2**(-dim/2)))
-            kwargs['labels'] = {0: 0, 2**dim - 1 : 2**dim - 1}
-            kwargs['min_node_size'] = 1
-            kwargs['max_node_size'] = 1000
-            kwargs['edgecolors'] = None
+    # Hiperwalk Hypercube
+    is_hypercube = False
+    try:
+        is_hypercube = graph.degree(0) == graph.dimension()
+    except AttributeError:
+        pass
+
+    if is_hypercube and plot is None:
+        plot = 'graph'
+
+        nx_graph = nx.from_scipy_sparse_array(graph.adjacency_matrix())
+        for v in nx_graph:
+            try:
+                nx_graph.nodes[v]["subset"] = v.bit_count()
+            except AttributeError:
+                nx_graph.nodes[v]["subset"] = bin(v).count('1')
+
+        kwargs['pos'] = nx.multipartite_layout(nx_graph)
+        dim = graph.dimension()
+        kwargs['graph'] = nx_graph
+        kwargs['edge_color'] = (0, 0, 0, max(0.002, 2**(-dim/2)))
+        kwargs['labels'] = {0: 0, 2**dim - 1 : 2**dim - 1}
+        kwargs['min_node_size'] = 1
+        kwargs['max_node_size'] = 1000
+        kwargs['edgecolors'] = None
 
     return 'graph' if plot is None else plot
 
 
 def _preconfigure_plot(probabilities, kwargs):
     """
     Configure static parameters for matplotlib plot.
@@ -411,15 +432,15 @@
         kwargs['max_prob'] = probabilities.max() #max_prob
         kwargs['rescale'] = False
 
     if 'graph' not in kwargs:
         raise KeyError("'graph' kwarg not provided.")
 
     graph = kwargs['graph']
-    if isinstance(graph, scipy.sparse.csr_array):
+    if isinstance(graph, csr_array):
         kwargs['graph'] = nx.from_scipy_sparse_array(graph)
     elif isinstance(graph, Graph):
         adj_matrix = graph.adjacency_matrix()
         kwargs['graph'] = nx.from_scipy_sparse_array(adj_matrix)
 
     if 'min_node_size' not in kwargs:
         kwargs['min_node_size'] = None
@@ -429,15 +450,15 @@
     # setting static kwargs for plotting
     # kwargs dictionary is updated by reference
     # TODO: change ConfigureNodes parameters
     # (remove G and use information from kwargs)
     _configure_nodes(kwargs['graph'], probabilities, kwargs)
 
 
-def _configure_figure(num_vert, fig_width=None, fig_height=None):
+def _configure_figure(fig_width, fig_height, dpi):
     """
     Set basic figure configuration.
 
     Creates a figure with size depending on the parameters.
 
     Parameters
     ----------
@@ -450,56 +471,49 @@
 
     Returns
     -------
     fig : current figure
     ax : current figure axes
     """
 
-    #TODO: set figure size according to graph dimensions
-    if fig_width is None:
-        fig_width = plt.rcParams["figure.figsize"][0]
-    if fig_height is None:
-        fig_height = plt.rcParams["figure.figsize"][1]
-
-    fig = plt.figure(figsize=(fig_width, fig_height))
+    fig = plt.figure(figsize=(fig_width, fig_height), dpi=dpi)
     ax = plt.gca()
 
     return fig, ax
 
 
-def _configure_plot_figure(num_vert, fig_width=None, fig_height=None):
+def _configure_plot_figure(fig_width, fig_height, dpi):
     """
     Set basic figure configuration for matplotlib plots.
     """
     
-    fig, ax = _configure_figure(num_vert, fig_width, fig_height)
+    fig, ax = _configure_figure(fig_width, fig_height, dpi)
 
     plt.xlabel("Vertex", size=18)
     plt.ylabel("Probability", size=18)
 
     plt.tick_params(length=7, labelsize=14)
 
     return fig, ax
 
 
-def _configure_graph_figure(num_vert=None, fig_width=None,
-                            fig_height=None):
-    return _configure_figure(num_vert, fig_width, fig_height)
-
-def _configure_plane_figure(num_vert=None, fig_width=None,
-                           fig_height=None):
-    if fig_width is None:
-        fig_width = plt.rcParams["figure.figsize"][0]
-    if fig_height is None:
-        fig_height = plt.rcParams["figure.figsize"][1]
+def _configure_graph_figure(fig_width,
+                            fig_height,
+                            dpi):
+    return _configure_figure(fig_width, fig_height, dpi)
+
+def _configure_plane_figure(fig_width,
+                            fig_height,
+                            dpi):
 
     #fig, ax =_configure_figure(num_vert, fig_width, fig_height) 
     #ax = fig.add_subplot(projection='3d')
     fig, ax = plt.subplots(figsize=(fig_width, fig_height),
-                           subplot_kw={"projection": "3d"})
+                           subplot_kw={"projection": "3d"},
+                           dpi=dpi)
 
     ax.tick_params(length=10, width=1, labelsize=16, pad=10)
     ax.set_xlabel('Vertex X', labelpad=15, fontsize=18)
     ax.set_ylabel('Vertex Y', labelpad=15, fontsize=18)
     ax.set_zlabel('Probability', labelpad=30, fontsize=18)
     return fig, ax
 
@@ -879,15 +893,15 @@
     """
     Plots probability distribution on the plane.
     """
     x_dim, y_dim = dimensions
 
     X = np.arange(0, x_dim, 1)
     Y = np.arange(0, y_dim, 1)
-    X, Y = np.meshgrid(X, Y)
+    Y, X = np.meshgrid(Y, X)
     Z = np.reshape(probabilities, (x_dim, y_dim))
 
     _default_plane_kwargs(kwargs)
 
     cmap = kwargs.pop('cmap')
     mappable = plt.cm.ScalarMappable(cmap=cmap)
     mappable.set_array(Z)
@@ -900,70 +914,91 @@
     mappable.set_clim(vmin, vmax)
 
     # division by 4 apparently normalize the colors
     if surf is None:
         surf = [0]
     else:
         surf[0].remove()
+
     surf[0] = ax.plot_surface(X, Y, Z, cmap=mappable.cmap,
                            vmin=vmin/4, vmax=vmax/4,
                            **kwargs)
     ax.set_zlim(vmin, vmax)
-    kwargs['cmap'] = cmap # reinserts into kwargs
 
+    kwargs['cmap'] = cmap # reinserts into kwargs
     if cbar is None:
         cbar = plt.colorbar(mappable,
                             shrink=0.4, aspect=20,
-                            pad=0.15)
+                            pad=0.15, ax=ax)
     else:
         cbar.update_normal(mappable)
 
     cbar.ax.tick_params(length=10, width=1, labelsize=16)
 
     return [[surf[0]], cbar]
 
 def _is_in_notebook():
+    ipython_shells = (
+        'XPythonShell',        # jupyterlite-xeus-python
+        'Interpreter',         # jupyterlite-pyodide-kernel
+        'ZMQInteractiveShell', # ipykernel
+    )
     try:
         shell = get_ipython().__class__.__name__
-        if shell == 'ZMQInteractiveShell':
+        if shell in ipython_shells:
             return True
         return False
     except:
         return False
 
 ##########################################################################
 
-def plot_success_probability(time, probabilities, **kwargs):
+def plot_success_probability(time, probabilities, figsize=(12, 10), dpi=100, **kwargs):
     r"""
-    Plots the success probability with respect to time.
-
-    The probabilities must have been calculated previously.
+    Plot the success probability over time.
 
+    Assumes that the probabilities have already been calculated.
+    
     Parameters
     ----------
     time:
         Time used for the quantum walk simulation.
         See :meth:`QuantumWalk.simulate` for details.
 
     probabilities:
         Success probabilities with respect to ``time``,
         such that ``probabilities[i]`` corresponds to ``i``-th
         timestamp described by ``time``.
+    figsize : tuple, default=(12, 10)
+        Figure size in inches. Must be a tuple in the format (WIDTH, HEIGHT).
+    dpi : float, default=100
+        Figure resolution in dots-per-inch.
 
     **kwargs:
         Additional arguments to customize plot.
         See :obj:`matplotlib.pyplot.plot` for the optional keywords.
 
     See Also
     --------
     QuantumWalk.simulate
     QuantumWalk.success_probability
     matplotlib.pyplot.plot
     """
 
+    # Figure size
+
+    if len(figsize) == 2:
+        fig_width, fig_height = figsize
+    else:
+        raise ValueError(
+            'figsize must be a tuple in the format (WIDTH, HEIGHT)'
+        )
+
+    _configure_figure(fig_width, fig_height, dpi)
+
     time = QuantumWalk._time_to_tuple(time)
     time[1] += time[2]
     time = np.arange(*time)
 
 
     if 'marker' not in kwargs:
         kwargs['marker'] = 'o'
@@ -975,9 +1010,119 @@
 
     ax = plt.gca()
     ax.set_ylim(0, 1.05*max(probabilities))
 
     plt.plot(time, probabilities, **kwargs)
     plt.show()
 
+def plot_function(qw_iter, x_label, y_label, x_vals, function,
+                  figsize=(12, 10), dpi=100, *args, **kwargs):
+    # TODO: any situation where *y_args and **y_kwargs are iterable?
+
+    # y_vals = [y_func(qw, *y_args, **y_kwargs) for qw in qw_gen]
+    # plt.plot(x_arg, y_vals)
+    # plt.show()
+    #######################################
+    # Figure size
+
+    if len(figsize) == 2:
+        fig_width, fig_height = figsize
+    else:
+        raise ValueError(
+            'figsize must be a tuple in the format (WIDTH, HEIGHT)'
+        )
+
+    _configure_figure(fig_width, fig_height, dpi)
+
+    if hasattr(x_vals, '__iter__'):
+        x_vals = iter(x_vals)
+
+    valid_function_kwargs = QuantumWalk._get_valid_kwargs(function)
+    function_kwargs = QuantumWalk._pop_valid_kwargs(kwargs,
+            valid_function_kwargs)
+    del valid_function_kwargs
+
+    x = []
+    y = []
+
+    for qw in qw_iter:
+        x.append(x_vals(qw)
+                 if callable(x_vals)
+                 else next(x_vals))
+
+        y.append(function(qw, *args, **function_kwargs))
+
+    plt.plot(x, y, marker='o')
+    plt.xlabel(x_label)
+    plt.ylabel(y_label)
+    plt.show()
+
+def plot_optimal_runtime(qw_iter, x_label, x_vals, state=None,
+                         **kwargs):
+    r"""
+    Parameters
+    ----------
+    qw_iter : iterable of :class:`QuantumWalk`
+        The code will be execute for each quantum walk in
+        the iterable.
+
+    x_vals :
+        The values to be plotted in the x-axis.
+        Iterable or callable.
+
+    state:
+        The initial state of the simulation.
+        If ``None`` uses default argument.
+        There are two types allowed.
+
+        iterable :
+            An array of states or an iterable.
+            The ``i``-th entry will be used as the inital state
+            of the ``i``-th quantum walk.
+
+        callable :
+            A function that receives a :class:`QuantumWalk` as argument
+            and returns a state.
+
+            .. todo::
+                Should the function accept ``*args`` and ``**kwargs``?
+    """
+    if hasattr(state, '__iter__'):
+        state = iter(state)
+
+    def function(qw, state=None, delta_time=1):
+        psi0 = None
+        if state is not None:
+            psi0 = (state(qw)
+                    if callable(state)
+                    else next(state))
+
+        return qw.optimal_runtime(state=psi0,
+                                  delta_time=delta_time)
+
+    plot_function(qw_iter, x_label, 'Optimal runtime', x_vals, function,
+                  state=state, **kwargs)
+
+def plot_max_success_probability(qw_iter, x_label, x_vals,
+        state=None, **kwargs):
+    r"""
+    TODO
+    """
+    if hasattr(state, '__iter__'):
+        state = iter(state)
+
+    def function(qw, state=None, delta_time=1):
+        psi0 = None
+        if state is not None:
+            psi0 = (state(qw)
+                    if callable(state)
+                    else next(state))
+
+        return qw.max_success_probability(state=psi0,
+                                          delta_time=delta_time)
+
+    plot_function(qw_iter, x_label, 'Max success probability',
+                  x_vals, function, state=state, **kwargs)
+
+
 if __DEBUG__:
     start = time()
```

### Comparing `hiperwalk-2.0b1/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0b11/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,76 @@
-import neblina
+try:
+    import neblina
+except ModuleNotFoundError:
+    pass
 import numpy as np
 import scipy.sparse
 from warnings import warn
 from .._constants import *
 from .._constants import __DEBUG__
 
 ############################################
 # used for automatically stopping the engine
 import atexit
 
 __engine_initiated = False
+__hpc_type = None
+
+def set_hpc(hpc):
+    r"""
+    Indicates which HPC platform is going to be used.
+
+    After executing the ``set_hpc`` command,
+    all subsequent hiperwalk commands will
+    utilize the dsignated HPC platform.
+
+    Parameters
+    ----------
+    hpc : {None, 'cpu', 'gpu'}
+        Indicates whether to utilize HPC
+        for matrix multiplication using CPU or GPU.
+        If ``hpc=None``, it will use standalone Python.
+    """
+    new_hpc = hpc
+
+    if hpc is not None:
+        hpc = hpc.lower()
+        hpc = hpc.strip()
+
+        if hpc == 'cpu':
+            new_hpc = 0
+        elif hpc == 'gpu':
+            new_hpc = 1
+        else:
+            raise ValueError(
+                    'Unexpected value of `hpc`: '
+                    + new_hpc + '. Expected a value in '
+                    + "[None, 'cpu', 'gpu'].")
+
+    global __hpc_type
+    if __hpc_type != new_hpc:
+        exit_handler()
+        __hpc_type = new_hpc
+        _init_engine()
+
+def get_hpc():
+    global __hpc_type
+
+    if __hpc_type == 0:
+        return 'cpu'
+    if __hpc_type == 1:
+        return 'gpu'
+
+    return None
 
 def exit_handler():
     global __engine_initiated
     if __engine_initiated:
         neblina.stop_engine()
+        __engine_initiated = False
 
 atexit.register(exit_handler)
 ############################################
 
 # "abstract"
 class PyNeblinaObject:
     def __init__(self, nbl_obj, shape, is_complex):
@@ -39,16 +91,27 @@
 def _init_engine():
     r"""
     Initiates neblina-core engine.
 
     Initiates the engine if it was not previously initiated
     """
     global __engine_initiated
-    if not __engine_initiated:
-        neblina.init_engine(neblina.CPU, 0)
+    global __hpc_type
+    if not __engine_initiated and __hpc_type is not None:
+        # TODO: if not 'neblina' in sys.modules raise ModuleNotFoundError
+        neblina_imported = True
+        try:
+            neblina.init_engine(__hpc_type, 0)
+        except NameError:
+            neblina_imported = False
+        if not neblina_imported:
+            raise ModuleNotFoundError(
+                "Module neblina was not imported. "
+                + "Do you have neblina-core and pyneblina installed?"
+            )
         __engine_initiated = True
 
 def send_vector(v):
     r"""
     Transfers a vector (v) to Neblina-core, and moves it
     to the device to be used.
     Returns a pointer to this vector
@@ -58,15 +121,14 @@
     TransferVector(v, False);
     this saves half the memory that would be used.
     TODO: is there a way to move the vector to the device directly?
     I think an auxiliary vector is beign created,
     thus twice the memory needed is being used
     """
 
-    _init_engine()
     # TODO: check if complex automatically?
     is_complex = isinstance(v.dtype, complex)
 
     if not is_complex:
         warn(
             "Real multiplication not implemented. "
             + "Treating entries as complex."
@@ -82,24 +144,27 @@
     # there should be a way to return a vector and automatically
     # convert to an array of float or of complex numbers accordingly.
     # 
     # vec = (neblina.vector_new(n, neblina.COMPLEX)
     #        if is_complex else neblina.vector_new(n, neblina.FLOAT))
     vec = neblina.vector_new(n, neblina.COMPLEX)
 
-    if is_complex:
+    try:
+        # TODO: Pyneblina needs to accept 3 only arguments
+        # instead of 4?
+        # TODO: check if neblina.vector_set is idetifying
+        # the vector type right (i.e. real and not complex)
         for i in range(n):
             neblina.vector_set(vec, i, v[i].real, v[i].imag)
-    else:
-        for i in range(n):
-            # TODO: Pyneblina needs to accept 3 only arguments
-            # instead of 4?
-            # TODO: check if neblina.vector_set is idetifying
-            # the vector type right (i.e. real and not complex)
-            neblina.vector_set(vec, i, v[i], 0)
+    except AttributeError:
+        print("Error: vector entries must have real and imaginary parts.")
+    except TypeError:
+        print("Error: vector entries must be numbers.")
+    except Exception as e:
+        print("Error: ", e)
 
     # suppose that the vector is going to be used
     # immediately after being transferred
     # TODO: check if this is the case
     neblina.move_vector_device(vec)
     return PyNeblinaVector(vec, is_complex, n)
 
@@ -144,16 +209,14 @@
     TODO: Add tests
       - Transfer and check real Matrix
       - Transfer and check complex Matrix
     TODO: isn't there a way for neblina-core to use the csr matrix directly?
       In order to avoid double memory usage
     """
     
-    _init_engine()
-
     # TODO: check if complex automatically?
     n = M.shape[0]
 
     # creates neblina sparse matrix structure
     # TODO: needs better support from pyneblina to
     #   use next instruction (commented).
     #   For example: neblina.sparse_matrix_set works, but in the real case,
@@ -187,16 +250,14 @@
 
     neblina.sparse_matrix_pack(smat) # TODO: is this needed?
     neblina.move_sparse_matrix_device(smat)
 
     return PyNeblinaMatrix(smat, M.shape, is_complex, True)
 
 def _send_dense_matrix(M, is_complex):
-    _init_engine()
-
     num_rows, num_cols = M.shape
     mat = (neblina.matrix_new(num_rows, num_cols, neblina.COMPLEX)
            if is_complex
            else neblina.matrix_new(num_rows, num_cols, neblina.FLOAT))
     
     # inserts elements into neblina matrix
     # TODO: Check if there really is a difference between real and complex
@@ -207,17 +268,15 @@
             neblina.matrix_set(mat, i, j, M[i, j].real, M[i, j].imag)
 
     neblina.move_matrix_device(mat)
 
     return PyNeblinaMatrix(mat, M.shape, is_complex, False)
 
 def send_matrix(M):
-    is_complex = isinstance(M.dtype, complex)
-
-    if not is_complex:
+    if not isinstance(M.dtype, complex):
         warn(
             "Real multiplication not implemented. "
             + "Treating entries as complex."
         )
     is_complex = True
 
     if scipy.sparse.issparse(M):
@@ -330,15 +389,14 @@
     if scipy.sparse.issparse(A):
         A = np.array(A.todense())
         warn(
             "Sparse matrix multiplication not implemented. "
             + "Converting to dense."
         )
 
-    _init_engine()
     pynbl_A = send_matrix(A)
     pynbl_Term = send_matrix(np.eye(A.shape[0], dtype=A.dtype))
     pynbl_M = send_matrix(np.eye(A.shape[0], dtype=A.dtype))
 
     for i in range(1, n+1):
         pynbl_Term.nbl_obj = neblina.mat_mul(
                 pynbl_Term.nbl_obj, pynbl_A.nbl_obj
```

### Comparing `hiperwalk-2.0b1/hiperwalk/quantum_walk/coined.py` & `hiperwalk-2.0b11/hiperwalk/quantum_walk/coined.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,172 @@
 import numpy as np
 import scipy
 import scipy.sparse
 import networkx as nx
 from .quantum_walk import QuantumWalk
-from .._constants import __DEBUG__, PYNEBLINA_IMPORT_ERROR_MSG
+from ..graph import SDMultigraph
+from .._constants import __DEBUG__
 from scipy.linalg import hadamard, dft
-try:
-    from . import _pyneblina_interface as nbl
-except:
-    pass
+from . import _pyneblina_interface as nbl
 
 if __DEBUG__:
     from time import time as now
 
 class Coined(QuantumWalk):
     r"""
-    Manage an instance of a coined quantum walk on
-    any simple graph.
+    Manage instances of coined quantum walks on arbitrary graphs.
 
-    This class provides methods for handling, simulating, and generating
-    operators within the coined quantum walk model for
-    various types of graphs.
+    The class provides methods to handle and generate operators in the 
+    coined quantum walk model. It also facilitates the simulation of 
+    coined quantum walks on graphs.
     
     For additional details about coined quantum walks,
     refer to the Notes Section.
 
     Parameters
     ----------
     graph
         Graph on which the quantum walk takes place.
-        It can be the graph itself (:class:`hiperwalk.graph.Graph`) or
-        its adjacency matrix (:class:`scipy.sparse.csr_array`).
+        Two types of entries are accepted:
+
+        * Simple graph (:class:`hiperwalk.Graph`);
+        * Multigraph (:class:`hiperwalk.Multigraph`);
+
+        A symmetric directed multigraph is created based on the input.
 
     **kwargs : optional
         Optional arguments for setting the non-default evolution operator.
         See :meth:`set_evolution`.
 
     Raises
     ------
     TypeError
         if ``adj_matrix`` is not an instance of
         :class:`scipy.sparse.csr_array`.
 
     See Also
     --------
     set_evolution
+    set_shift
+    set_coin
 
     Notes
     -----
 
-    The computational basis is spanned by the set of arcs.
-    The cardinality is :math:`2|E|`, where :math:`E`
-    represents the edge set of the graph.
-    For further information regarding the order of the arcs,
-    consult the respective graph descriptions.
-    The Hilbert space of a coined quantum walk is denoted by
-    :math:`\mathcal{H}^{2|E|}`.
+    The coined quantum walk model is a quantum analog of 
+    classical random walks, incorporating an additional 
+    quantum coin-toss mechanism. It uses an extra quantum 
+    internal degree of freedom, represented by the coin state,
+    to determine the direction of the walker's movement 
+    on a graph.
+
+    In the coined model, the graph is interpreted
+    as a directed graph as follows:
+    Each edge in :math:`G(V, E)` connecting two distinct vertices
+    translates into a pair of arcs in the directed graph
+    :math:`\vec{G}(V, \mathcal{A})`, where
+
+    .. math::
+        \begin{align*}
+            \mathcal{A} = \bigcup_{v_k v_\ell\, \in E} \{(v_k, v_\ell), (v_\ell, v_k)\}.
+        \end{align*}
+
+    .. note::
+        The order of arcs depends on the order of neighbors.
+
+    Arcs are represented using either
+    the (tail,head) notation or numerical labels.
+    In the :obj:`Graph` class, the arc labels are ordered such that for two arcs,
+    :math:`(v_i, v_j)` and :math:`(v_k, v_\ell)`, with labels :math:`a_1` and
+    :math:`a_2` respectively, :math:`a_1 < a_2` if and only if :math:`i < k` or
+    (:math:`i = k` and :math:`j < \ell`).
+    Loops are depicted as single arcs,
+    affecting the dimension of the associated Hilbert space.
+    In coined quantum walks, the weights of arcs do not influence the dynamics.
+
+    The computational basis is composed of the graph's arc set.
+    For simple graphs, the cardinality of the computational
+    basis is :math:`2|E|`, where :math:`E`
+    represents the graph's edge set.
+    When a loop is added to the graph, the cardinality of the 
+    computational basis increases by one for each loop.
+    
+    The arcs are arranged within the computational basis 
+    to ensure that the coin operator adopts a block-diagonal 
+    matrix form.
+    For additional information on the arc ordering,
+    please consult the respective graph descriptions.
 
     For a more detailed understanding of coined quantum walks,
     refer to Section 7.2: Coined Walks on Arbitrary Graphs,
     found in the book  'Quantum Walks and Search Algorithms' [1]_.
 
+    For example, the graph :math:`G(V, E)` shown in
+    Figure 1 has an adjacency matrix ``adj_matrix``.
+
+    .. testsetup::
+
+        import numpy as np
+
+    >>> adj_matrix = np.array([
+    ...     [0, 1, 0, 0],
+    ...     [1, 0, 1, 1],
+    ...     [0, 1, 0, 1],
+    ...     [0, 1, 1, 0]])
+    >>> adj_matrix
+    array([[0, 1, 0, 0],
+           [1, 0, 1, 1],
+           [0, 1, 0, 1],
+           [0, 1, 1, 0]])
+
+    .. graphviz:: ../../graphviz/graph-example.dot
+        :align: center
+        :layout: neato
+        :caption: Figure 1
+
+    Suppose that, for this graph,
+    the neighbors are given in ascending order.
+    Then,
+    the arcs of the associated digraph in the arc notation are
+
+    >>> arcs = [(i, j) for i in range(4)
+    ...                for j in range(4) if adj_matrix[i,j] == 1]
+    >>> arcs
+    [(0, 1), (1, 0), (1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2)]
+
+    Note that ``arcs`` is already sorted, hence the associated
+    numeric labels are
+
+    >>> arcs_labels = {arcs[i]: i for i in range(len(arcs))}
+    >>> arcs_labels
+    {(0, 1): 0, (1, 0): 1, (1, 2): 2, (1, 3): 3, (2, 1): 4, (2, 3): 5, (3, 1): 6, (3, 2): 7}
+
+    The numeric labels are depicted in Figure 2.
+
+    .. graphviz:: ../../graphviz/graph-arcs.dot
+        :align: center
+        :layout: neato
+        :caption: Figure 2
+
+    If we insert the labels of the arcs into the adjacency matrix,
+    we obtain matrix ``adj_labels`` as follows:
+
+    >>> adj_labels = [[arcs_labels[(i,j)] if (i,j) in arcs_labels
+    ...                                   else '' for j in range(4)]
+    ...               for i in range(4)]
+    >>> adj_labels = np.matrix(adj_labels)
+    >>> adj_labels
+    matrix([['', '0', '', ''],
+            ['1', '', '2', '3'],
+            ['', '4', '', '5'],
+            ['', '6', '7', '']], dtype='<U21')
+
+    Note that, intuitively,
+    the arcs are labeled in left-to-right and top-to-bottom fashion.
+
     References
     ----------
     .. [1] R. Portugal. "Quantum walks and search algorithms", 2nd edition,
         Springer, 2018.
     """
 
     # static attributes.
@@ -72,30 +174,33 @@
     # The class must be instantiated so the interpreter knows
     # the memory location for the function pointers.
     _coin_funcs = dict()
     _valid_kwargs = dict()
 
     def __init__(self, graph=None, **kwargs):
 
+        # create symmetric directed multigraph from input
+        sdmg = SDMultigraph(graph)
+
+        super().__init__(graph=sdmg)
+        self.hilb_dim = self._graph.number_of_arcs()
+
+        # Specific coined quantum walk attributes
         self._shift = None
         self._coin = None
         self._oracle_coin = []
-        super().__init__(graph=graph)
-
-        # Expects adjacency matrix with only 0 and 1 as entries
-        self.hilb_dim = self._graph.number_of_arcs()
 
+        # create static dicts
         if not bool(Coined._valid_kwargs):
-            # assign static attribute
             Coined._valid_kwargs = {
-                'shift': Coined._get_valid_kwargs(self._update_shift),
-                'coin': Coined._get_valid_kwargs(self._update_coin),
-                'marked': Coined._get_valid_kwargs(self._update_marked),
+                'shift': Coined._get_valid_kwargs(self._set_shift),
+                'coin': Coined._get_valid_kwargs(self._set_coin),
+                'marked': Coined._get_valid_kwargs(self._set_marked),
                 'evolution': Coined._get_valid_kwargs(
-                    self._update_evolution)
+                    self._set_evolution)
             }
 
         # dict with valid coins as keys and the respective
         # function pointers.
         if not bool(Coined._coin_funcs):
             # assign static attribute
             Coined._coin_funcs = {
@@ -117,62 +222,68 @@
                         for p in self._valid_kwargs[m]]
             if len(params) != len(set(params)):
                 raise AssertionError
 
 
     def _set_flipflop_shift(self):
         r"""
-        Create the flipflop shift operator (:math:`S`) based on
+        Creates the flipflop shift operator (:math:`S`) based on
         the ``_graph`` attribute.
 
         The operator is configured for future use. If an evolution
         operator was set earlier, it will be unset to maintain coherence.
         """
-
-        num_vert = self._graph.number_of_vertices()
-        num_arcs = self._graph.number_of_arcs()
-
-        S_cols = [self._graph.arc_number((j, i))
-                  for i in range(num_vert)
-                  for j in self._graph.neighbors(i)]
+        g = self._graph
+        num_vert = g.number_of_vertices()
+        num_arcs = g.number_of_arcs()
+
+        if g.is_underlying_simple():
+            S_cols = [g.arc_number((j, i))
+                      for i in range(num_vert)
+                      for j in g.neighbors(i)]
+        else:
+            S_cols = [g.arc_number((j, i, e))
+                      for i in range(num_vert)
+                      for j in g.neighbors(i)
+                      for e in range(g.number_of_edges(j, i))]
 
         # Using csr_array((data, indices, indptr), shape)
         # Note that there is only one entry per row and column
         S = scipy.sparse.csr_array(
             ( np.ones(num_arcs, dtype=np.int8),
               S_cols, np.arange(num_arcs+1) ),
             shape=(num_arcs, num_arcs)
         )
 
         self._shift = S
 
     def has_persistent_shift(self):
         r"""
-        Checks whether the persistent shift operator is defined
+        Check whether the persistent shift operator is defined
         for the current graph.
 
         Returns
         -------
         bool
 
         Notes
         -----
         The persistent shift is sometimes called *moving shift*.
 
         The persistent shift operator can only be defined in a
         meaningful way for certain specific graphs. For instance,
-        for graphs that can be embedded onto a plane,
+        for graphs that can be embedded onto a plane so that
         directions such as left, right, up, and down
         can be referred to naturally.
         """
-        return 'previous_arc' in dir(self._graph)
+        return self._graph.previous_arc(0) is not None
 
     def _set_persistent_shift(self):
         r"""
-        Create the persistent shift operator (:math:`S`) based on
+        Creates the persistent shift operator (:math:`S`) based on
         the ``_graph`` attribute.
 
         The operator is set for future usage.
         If an evolution operator was set previously,
         it is unset for coherence.
         """
         num_arcs = self._graph.number_of_arcs()
@@ -185,62 +296,82 @@
             ( np.ones(num_arcs, dtype=np.int8),
               S_cols, np.arange(num_arcs+1) ),
             shape=(num_arcs, num_arcs)
         )
 
         self._shift = S
 
-    def _update_shift(self, shift='default'):
+    def _set_shift(self, shift='default'):
         valid_vals = ['default', 'flipflop', 'persistent', 'ff', 'p']
-        if shift not in valid_vals:
-            raise ValueError(
-                "Invalid `shift` value. Expected one of "
-                + str(valid_vals) + ". But received '"
-                + str(shift) + "' instead."
-            )
 
-        if shift == 'default':
-            shift = 'p' if self.has_persistent_shift() else 'ff'
+        # check if string
+        try:
+            shift = shift.lower()
 
-        if shift == 'ff':
-            shift = 'flipflop'
-        elif shift == 'p':
-            shift = 'persistent'
+            if shift not in valid_vals:
+                raise ValueError(
+                    "Invalid `shift` value. Expected one of "
+                    + str(valid_vals) + ". But received '"
+                    + str(shift) + "' instead."
+                )
+
+            if shift == 'default':
+                shift = 'p' if self.has_persistent_shift() else 'ff'
+
+            if shift == 'ff':
+                shift = 'flipflop'
+            elif shift == 'p':
+                shift = 'persistent'
+
+            if str(self._shift) != shift:
+                if shift == 'flipflop':
+                    self._set_flipflop_shift()
+                else:
+                    self._set_persistent_shift()
+                return True
 
-        
-        if shift == 'flipflop':
-            self._set_flipflop_shift()
-        else:
-            self._set_persistent_shift()
+            return False
 
-        if __DEBUG__:
-            if self._shift is None: raise AssertionError
+        except AttributeError:
+            pass
 
-    def set_shift(self, shift='default', **kwargs):
+        # check if explict matrix
+        try:
+            shift[0][0] #if this works, then shift is numpy or list of list
+            # convert to sparse
+            shift = scipy.sparse.csr_array(shift)
+        except NotImplementedError:
+            # already sparse
+            pass
+
+        if (len(shift.shape) != 2 or shift.shape[0] != shift.shape[1]):
+            raise TypeError('Explicit coin is not a square matrix.')
+
+        if (id(self._shift) != id(shift)):
+            self._shift = shift
+            return True
+
+        return False
+
+    def set_shift(self, shift='default'):
         r"""
         Set the shift operator.
 
-        Sets either the flipflop or the persistent shift operator.
-        Afterwards, the evolution operator is updated accordingly.
+        Defines either the flipflop or the persistent shift operator.
+        Following this, the evolution operator updates accordingly.
 
         Parameters
         ----------
         shift: {'default', 'flipflop', 'persistent', 'ff', 'p'}
             Whether to create the flip flop or the persistent shift.
             By default, creates the persistent shift if it is defined;
             otherwise creates the flip flop shift.
             Argument ``'ff'`` is an alias for ``'flipflop'``.
             Argument ``'p'`` is an alias for ``'persistent'``.
 
-        **kwargs:
-            Additional arguments.
-            Used for determining the procedure for
-            updating the evolution operator.
-            See :meth:`hiperwalk.Coined.set_evolution` for valid options.
-
         Raises
         ------
         AttributeError
             If ``shift='persistent'`` and
             the persistent shift operator cannot be defined.
 
         See Also
@@ -250,29 +381,33 @@
 
         Notes
         -----
         .. note::
             Check :class:`Coined` Notes for details
             about the computational basis.
 
-        The persistent shift is sometimes called *moving shift*.
-
-        The flip-flop shift operator :math:`S` is defined such that
+        The flip-flop shift operator :math:`S` is defined as
 
         .. math::
-            \begin{align*}
-                S \ket{(v, u)} &= \ket{(u, v)} \\
-                \implies S\ket i &= \ket j
-            \end{align*}
-
-        where :math:`i` is the label of the edge :math:`(v, u)` and
-        :math:`j` is the label of the edge :math:`(u, v)`.
-
+            S \ket{v, u} = \ket{u, v},
 
-        For a more comprehensive understanding of the flipflop
+        in the context of arc notation, where :math:`(v, u)` and
+        :math:`(u, v)` represent opposite arcs. This can be equivalently 
+        expressed as :math:`S\ket{i} = \ket{j}`, where :math:`i` is the 
+        label of the arc :math:`(v, u)` and :math:`j` is the label of 
+        the arc :math:`(u, v)`. The flip-flop shift satisfies the 
+        property :math:`S^2 = I`.
+
+        The persistent shift, also known as the *moving shift*, 
+        is defined for graphs with a clear notion of direction or rotation.
+        When the shift operator is applied repeatedly, it causes the walker 
+        to continue moving persistently in the same direction. Unlike the 
+        flip-flop shift, the persistent shift does not satisfy :math:`S^2 = I`.
+        
+        For a more comprehensive understanding of the 
         shift operator, refer to Section 7.2: Coined Walks on Arbitrary
         Graphs in the book "Quantum Walks and Search Algorithms" [1]_.
         
 
         References
         ----------
         .. [1] R. Portugal. "Quantum walks and search algorithms",
@@ -284,23 +419,25 @@
         :class:`Graph` Notes Section example.
         The corresponding flip-flop shift operator is
 
         .. testsetup::
 
             import numpy as np
             import scipy.sparse
+            from sys import path
+            path.append('../..')
 
         .. doctest::
 
             >>> import hiperwalk as hpw
             >>> A = scipy.sparse.csr_array([[0, 1, 0, 0],
             ...                             [1, 0, 1, 1],
             ...                             [0, 1, 0, 1],
             ...                             [0, 1, 1, 0]])
-            >>> qw = hpw.Coined(A)
+            >>> qw = hpw.Coined(hpw.Graph(A))
             >>> qw.set_shift(shift='flipflop')
             >>> S = qw.get_shift().todense()
             >>> S
             array([[0, 1, 0, 0, 0, 0, 0, 0],
                    [1, 0, 0, 0, 0, 0, 0, 0],
                    [0, 0, 0, 0, 1, 0, 0, 0],
                    [0, 0, 0, 0, 0, 0, 1, 0],
@@ -326,30 +463,35 @@
             >>> S @ np.array([0, 0, 0, 0, 1, 0, 0, 0]) # S|4> = |2>
             array([0, 0, 1, 0, 0, 0, 0, 0])
 
         .. todo::
             
             Add persistent example.
         """
-        self._update_shift(shift=shift)
-        self._update_evolution(**kwargs)
+        self.set_evolution(shift=shift,
+                           coin=self._coin,
+                           marked=self._marked)
 
     def get_shift(self):
         r"""
-        Return the shift operator.
+        Retrieve the shift operator.
 
         Shift operator used for constructing the evolution operator.
 
         Returns
         -------
         scipy.sparse.csr_array
+
+        See Also
+        --------
+        set_shift
         """
         return self._shift
 
-    def _update_coin(self, coin='default'):
+    def _set_coin(self, coin='default'):
         try:
             if len(coin.shape) != 2:
                 raise TypeError('Explicit coin is not a matrix.')
 
             # explicit coin
             if not scipy.sparse.issparse(coin):
                 coin = scipy.sparse.csr_array(coin)
@@ -365,22 +507,22 @@
             raise ValueError('Coin was not specified for all vertices.')
 
         self._coin = coin_list
 
         if __DEBUG__:
             if self._coin is None: raise AssertionError
 
-    def set_coin(self, coin='default', **kwargs):
+    def set_coin(self, coin='default'):
         """
-        Generate a coin operator based on the graph structure.
+        Set the coin operator based on the graph's structure.
 
-        Constructs a coin operator based on the degree of each vertex.
-        A single type of coin may be applied to
-        all vertices or a subset thereof.
-        Once the coin operator is set,
+        Builds a coin operator considering the degree of each vertex.
+        The same coin can be applied to all vertices, or multiple 
+        coins can be assigned, each to a specific subset of vertices. 
+        After setting the coin operator,
         the evolution operator is updated accordingly.
 
         Parameters
         ----------
         coin
             Coin to be used.
             Several types of arguments are acceptable.
@@ -411,43 +553,41 @@
                 If ``list_of_vertices = []``,
                 the respective ``coin_type`` is applied to all vertices
                 that were not explicitly listed.
 
             * :class:`scipy.sparse.csr_array`
                 The explicit coin operator.
 
-        **kwargs:
-            Additional arguments.
-            Used for determining the procedure for
-            updating the evolution operator.
-            See :meth:`hiperwalk.Coined.set_evolution` for valid options.
-
         See Also
         --------
         set_evolution
 
+            
         Notes
         -----
-        Owing to the selected computational basis (refer to the
-        Notes in the :class:`Coined`),
-        the outcome is a block diagonal operator.
-        Each block is a :math:`\deg(v)`-dimensional ``coin``.
+        
+        The output of this method is a block-diagonal 
+        operator, which results from the specific ordering of arcs 
+        in the computational basis 
+        (refer to the Notes in :class:`Coined` for more details).        
+        Each block is associated with a :math:`\deg(v)`-dimensional ``coin``.
         As a result, there are :math:`|V|` blocks in total.
+        Note that a loop at a vertex :math:`u` is treated
+        as the arc :math:`(u,u)`, contributing an additional 
+        one to the degree of :math:`u`.
+        
 
         .. todo::
 
             Check if explicit coin is valid.
 
         """
-        for key in kwargs:
-            if key not in Coined._valid_kwargs['evolution']:
-                kwargs.pop(key)
-
-        self._update_coin(coin=coin)
-        self._update_evolution(**kwargs)
+        self.set_evolution(shift=self._shift,
+                           coin=coin,
+                           marked=self._marked)
 
     def default_coin(self):
         r"""
         Returns the default coin name.
 
         The default coin name depends on the graph on
         which the quantum walk occurs.
@@ -574,42 +714,47 @@
     def _minus_hadamard_coin(dim):
         return -Coined._hadamard_coin(dim)
 
     @staticmethod
     def _minus_identity_coin(dim):
         return -np.identity(dim)
 
-    def _update_marked(self, marked=[]):
-        coin_list = []
+    def _set_marked(self, marked=[]):
+        try:
+            marked.get(0) #throws exception if list
+        except AttributeError:
+            # list
+            if len(marked) > 0:
+                marked = {'-I': marked}
+            else:
+                marked = {}
 
-        if isinstance(marked, dict):
-            coin_list, _ = self._coin_to_list(marked)
+        coin_list, _ = self._coin_to_list(marked)
 
-            dict_values = marked.values()
-            vertices = [vlist if hasattr(vlist, '__iter__') else [vlist]
-                        for vlist in dict_values]
-            vertices = [v for vlist in vertices for v in vlist ]
-            marked = vertices
+        dict_values = marked.values()
+        vertices = [vlist if hasattr(vlist, '__iter__') else [vlist]
+                    for vlist in dict_values]
+        vertices = [v for vlist in vertices for v in vlist ]
+        marked = vertices
 
-        super()._update_marked(marked=marked)
+        super()._set_marked(marked=marked)
         self._oracle_coin = coin_list
 
-    def set_marked(self, marked=[], **kwargs):
+    def set_marked(self, marked=[]):
         r"""
-        Set marked vertices.
+        Set the marked vertices.
 
-        If a list of vertices is provided, those vertices are
-        deemed as marked.
+        When a set or list of vertices is provided, they 
+        are set as marked.
         The evolution operator is updated accordingly.
 
-        If a dictionary is passed,
-        the coin of those vertices are substituted
-        only for generating the evolution operator.
-        This can only be done if the set coin operator is
-        not a explicit matrix.
+        If a dictionary is passed, the coin of those vertices is
+        replaced solely for the purpose of generating the evolution 
+        operator. This can only be done if the set coin operator is
+        not an explicit matrix.
 
         Parameters
         ----------
         marked : list of vertices or dict
             list of vertices to be marked and
             how they are going to be marked.
             
@@ -618,86 +763,66 @@
                 The coin for those vertices is '-I'.
 
             * dict
                 A dictionary with structure
                 ``{coin_type : list_of_vertices}``.
                 Analogous to the one accepted by :meth:`set_coin`.
 
-        **kwargs:
-            Additional arguments.
-            Used for determining the procedure for
-            updating the evolution operator.
-            See :meth:`hiperwalk.Coined.set_evolution` for valid options.
-
         See Also
         --------
         set_coin
         set_evolution
         """
-        super().set_marked(marked=marked, **kwargs)
+        self.set_evolution(shift=self._shift,
+                           coin=self._coin,
+                           marked=marked)
 
     def _coin_list_to_explicit_coin(self, coin_list):
         num_vert = self._graph.number_of_vertices()
         degree = self._graph.degree
         blocks = [self._coin_funcs[coin_list[v]](degree(v))
                   for v in range(num_vert)]
         C = scipy.sparse.block_diag(blocks, format='csr')
         return scipy.sparse.csr_array(C)
 
     def get_coin(self):
         r"""
-        Return coin used for creating the evolution operator.
+        Retrieve the coin used in the creation of the evolution operator.
 
         Returns
         -------
         :class:`scipy.sparse.csr_array`
 
         See Also
         --------
         set_coin
-        
-        Notes
-        -----
-        The final coin :math:`C'` is obtained by multiplying the
-        coin operator :math:`C` and the oracle :math:`R`.
-        That is,
-
-        .. math::
-            
-            C' = CR .
-
-        The oracle is not explicitly saved.
-        Instead, the oracle coins are saved -- i.e.
-        which coin is going to be applied to each marked vertices.
-        To generate :math:`C'` we simply substitute the original coin
-        by the oracle coin in all marked vertices.
-
-        Examples
-        --------
-        .. todo::
-            examples
         """
         if scipy.sparse.issparse(self._coin):
             if not bool(self._oracle_coin):
                 return self._coin
 
             # if coin was explicitly set,
             # and there are different coins for the marked vertices,
             # change them.
             def get_block(vertex):
                 g = self._graph
                 neighbors = g.neighbors(vertex)
-                start = g.arc_number((vertex, neighbors[0]))
-                end = g.arc_number((vertex, neighbors[-1])) + 1
+                # TODO: this technique wont work after the behavior of
+                # neighbors() change.
+                a1 = g.arc_number((vertex, neighbors[0]))
+                a2 = g.arc_number((vertex, neighbors[-1]))
+                # arc order may change
+                start = min(a1, a2)
+                end = max(a1, a2) + 1
 
                 return scipy.sparse.csr_array(self._coin[start:end,
                                                          start:end])
 
-            num_vert = self.number_of_vertices()
-            degree = self.degree
+            num_vert = self._graph.number_of_vertices()
+            degree = self._graph.degree
             oracle_coin = self._oracle_coin
             coin_funcs = Coined._coin_funcs
             blocks = [coin_funcs[oracle_coin[v]](degree(v))
                       if oracle_coin[v] != ''
                       else get_block(v)
                       for v in range(num_vert)]
             C = scipy.sparse.block_diag(blocks, format='csr')
@@ -711,24 +836,24 @@
                          else coin[i]
                          for i in range(len(coin))]
         else:
             coin_list = self._coin
 
         return self._coin_list_to_explicit_coin(coin_list)
 
-    def _update_evolution(self, hpc=True):
+    def _set_evolution(self):
+        # TODO: Check if matrix is sparse in pynelibna interface
+        # TODO: Check if matrices are deleted from memory and GPU.
         U = None
-        if hpc and not self._pyneblina_imported():
-            hpc = False
 
         S = self.get_shift()
         C = self.get_coin()
 
-        if hpc:
-
+        if nbl.get_hpc() is not None:
+            # TODO: implement sparse matrix multiplication with hpc
             S = S.todense()
             C = C.todense()
 
             nbl_S = nbl.send_matrix(S)
             del S
             nbl_C = nbl.send_matrix(C)
             del C
@@ -742,71 +867,71 @@
 
         else:
             U = S @ C
 
         self._evolution = U
         return U
 
-    def set_evolution(self, hpc=True, **kwargs):
+    def set_evolution(self, **kwargs):
         """
-        Create evolution operator.
+        Set the evolution operator.
 
-        Sets shift, coin and marked vertices.
+        Establishes the shift operator, coin operator,
+        and the marked vertices.
         They are set using the appropriate ``**kwargs``.
         If ``**kwargs`` is empty, the default arguments are used.
 
-        Then, creates evolution operator by multiplying the
-        shift operator and coin operator.
-        If the coin operator is not an explicit matrix,
-        and the coin for marked vertices was specified,
-        the coin of each marked vertex is substituted.
+        Subsequently, the evolution operator is constructed by 
+        multiplying the shift and coin operators. 
+        If the coin operator is given as an explicit matrix, 
+        its definition remains unaltered 
+        even in the presence of marked vertices. However, if the coin 
+        operator is defined using coin names, any marked vertices will 
+        prompt an update to the coin operator. Specifically, the coin names 
+        for each marked vertex will default to a replacement with -I, 
+        unless an alternative substitution is provided.
 
         Parameters
         ----------
         **kwargs : dict, optional
             Arguments for setting the evolution operator.
             Accepts any valid keywords from
             :meth:`set_shift` :meth:`set_coin`, and :meth:`set_marked`.
 
-        hpc : bool, default=True
-            Whether or not the evolution operator should be
-            constructed using nelina's high-performance computing.
-
         See Also
         --------
         set_shift
         set_coin
         set_marked
         get_evolution
 
         Notes
         -----
         The evolution operator is given by
 
         .. math::
-           U = SC'
+           U = SC
 
-        where :math`S` is the shift operator, and
-        :math:`C'` is the coin operator (probably) modified by
-        the marked vertices [1]_.
-
-        If the coin operator was set as an explicit matrix,
-        the marked vertices to not alter it.
-        If the coin operator was not set as an explicit matrix
-        (e.g. as a list of coins),
-        the coin of each marked vertex is substituted as specified by
-        the last :meth:`set_marked` call.
-
-        .. todo::
-            * Sparse matrix multipliation is not supported yet.
-              Converting all matrices to dense.
-              Then converting back to sparse.
-              This uses unnecessary memory and computational time.
-            * Check if matrix is sparse in pynelibna interface
-            * Check if matrices are deleted from memory and GPU.
+        where :math:`S` is the shift operator, and
+        :math:`C` is the coin operator. If there are
+        any marked vertices, the coin operator is
+        modified accordingly [1]_.
+
+        When the coin operator is set as an explicit matrix, it remains 
+        unaltered by marked vertices. However, if it's not provided in 
+        matrix form (e.g., as a list of coins), the coin for each marked 
+        vertex will be substituted based on the most recent 
+        :meth:`set_marked` invocation.
+
+
+        .. warning::
+            Sparse matrix multipliation is not supported yet.
+            Converting all matrices to dense.
+            Then converting back to sparse.
+            This uses unnecessary memory and computational time.
 
 
         References
         ----------
         .. [1] R. Portugal. "Quantum walks and search algorithms",
             2nd edition, Springer, 2018.
 
@@ -823,18 +948,18 @@
         C_kwargs = Coined._filter_valid_kwargs(
                               kwargs,
                               Coined._valid_kwargs['coin'])
         R_kwargs = Coined._filter_valid_kwargs(
                               kwargs,
                               Coined._valid_kwargs['marked'])
 
-        self._update_shift(**S_kwargs)
-        self._update_coin(**C_kwargs)
-        self._update_marked(**R_kwargs)
-        self._update_evolution(hpc=hpc)
+        self._set_shift(**S_kwargs)
+        self._set_coin(**C_kwargs)
+        self._set_marked(**R_kwargs)
+        self._set_evolution()
 
     def probability_distribution(self, states):
         r"""
         Compute the probability distribution of given state(s).
 
         The probability of the walker being found on each vertex
         for the given state(s).
@@ -854,77 +979,89 @@
 
             If ``states`` is a list of states,
             ``probabilities[i][v]`` is the probability of the
             walker beign found at vertex ``v`` in ``states[i]``.
 
         See Also
         --------
+        probability
         simulate
 
         Notes
         -----
-        The probability for a given vertex :math:`u` is the sum of the
-        absolute square of the amplitudes of the arcs with tail :math:`u`.
-        That is, for an arbitrary superposition
-
+        The probability for a given vertex :math:`u` is calculated as the sum of the
+        absolute squares of the amplitudes of the arcs originating from :math:`u`.
+        More precisely, if the state of the walker is
+        
         .. math::
-            \sum_{(u, v) \in A(\vec G)} \alpha_{u,v} \ket{u,v},
-
-        -- where :math:`\vec G` is the graph :math:`G` with each
-        edge substituted by two arcs (one for each direction) --
-        the probability associated with vertex :math:`u` is
-
+            \sum_{(v, w) \in \mathcal{A}(\vec G)} \alpha_{v,w} \ket{v,w},
+        
+        where :math:`\mathcal{A}(\vec G)` is the set of arcs of
+        the symmetric directed graph formed by
+        replacing each edge in :math:`G` with two arcs, one for each direction,
+        then the probability associated with vertex :math:`u` is given by
+        
         .. math::
             \sum_{v \in N(u)}|\alpha_{u, v}|^2,
-
-        where :math:`N(u)` is the set of neighbors of :math:`u`.
+        
+        with :math:`N(u)` being the set of out neighbors of :math:`u`.
+        A loop at :math:`u` is the arc :math:`(u,u)`. 
+        
+        The probability distribution, which is returned by this
+        method as a ``numpy.ndarray``, is the collection of these
+        probabilities for all vertices.
         """
         if __DEBUG__:
             start = now()
 
+        try:
+            states.shape == 1
+        except:
+            states = np.array(states, copy=False)
+
         if len(states.shape) == 1:
-            states = [states]
+            states = np.array([states], copy=False)
+
 
         graph = self._graph
         num_vert = graph.number_of_vertices()
         prob = np.array([[Coined._elementwise_probability(
                               states[i, graph.arcs_with_tail(v)]).sum()
                           for v in range(num_vert)]
                          for i in range(len(states))])
 
         return prob
 
-    def state(self, *args):
+    def state(self, entries):
         """
         Generates a valid state.
 
         The state corresponds to the walker being in a superposition
         of the ``entries``.
         For instance, click on :meth:`qwalk.coined.Graph`.
         The final state is normalized in order to be a unit vector.
 
         Parameters
         ----------
-        *args
+        entries : list of entry
             Each entry is a tuple (or array).
-            An entry can be specified in three different ways:
-            ``(amplitude, (tail, head))``,
-            ``(amplitude, tail, head)``, and
+            An entry can be specified in two different ways:
+            ``(amplitude, (tail, head))``, and
             ``(amplitude, arc_number)``.
 
             amplitude
                 The amplitude of the given entry.
             tail
                 The vertex corresponding to the position of the walker
                 in the superposition.
                 In other words, the tail of the arc.
+                The tuple ``(tail, head)`` must be a valid arc.
             head
                 The vertex to which the coin is pointing.
-                That is, the tuple
-                ``(tail, head)`` must be a valid arc.
+                The tuple ``(tail, head)`` must be a valid arc.
             arc_number
                 The numerical arc label with respect to the arc ordering
                 given by the computational basis.
 
         Notes
         -----
         If there are repeated arcs,
@@ -941,97 +1078,127 @@
             path.append('../..')
             import hiperwalk as hpw
             import numpy as np
             dim = 10
             g = hpw.Grid((dim, dim))
             qw = hpw.Coined(graph=g)
 
-        >>> psi = qw.state((1, (0, 1)), [1, 1], (1, 2))
-        >>> psi1 = qw.state((1, ([0, 0], [1, 0])),
-        ...                 [[1, (0, dim - 1)],
-        ...                  (1, [(0, 0), [0, 1]])])
-        >>> psi2 = qw.state([(1, [0, 0], [1, 0]),
-        ...                  [1, 0, dim - 1]],
-        ...                 (1, (0, 0), [0, 1]))
+        >>> psi = qw.state([(1, (0, 1)), [1, 1], (1, 2)])
+        >>> psi1 = qw.state([(1, ([0, 0], [0, 1])),
+        ...                  [1, [(0, 0), (dim - 1, 0)]],
+        ...                  (1, (0, 1))])
+        >>> psi2 = qw.state([(1, [[0, 0], [0, 1]]),
+        ...                  [1, ((0, 0), (dim - 1, 0))],
+        ...                  (1, [0, 1])])
         >>> np.all(psi == psi1)
         True
         >>> np.all(psi1 == psi2)
         True
         """
-        if len(args) == 0:
+        if len(entries) == 0:
             raise TypeError("Entries were not specified.")
 
-        state = [0] * self.hilb_dim
+        state = np.zeros(self.hilb_dim)
 
-        def add_entry(entry):
-            ampl = entry[0]
-            arc = entry[1:]
-            if len(arc) == 1:
-                arc = arc[0]
+        for ampl, arc in entries:
             state[self._graph.arc_number(arc)] = ampl
 
-        for arg in args:
-            if hasattr(arg[0],'__iter__'):
-                for entry in arg:
-                    add_entry(entry)
-            else:
-                add_entry(arg)
-
-        state = np.array(state)
         return self._normalize(state)
 
-    def ket(self, *args):
+    def ket(self, arc):
         r"""
         Create a computational basis state.
 
         Parameters
         ----------
-        *args
+        arc: int or tuple of int
             The ket label.
-            There are three different labels acceptable.
+            There are two different labels acceptable.
 
             (tail, head)
                 The arc notation.
-            tail, head
-                The arc notation with ``tail`` and ``head`` as
-                separate arguments.
             arc_number
                 The label of the arc.
-                Its number according to the computational basis order.
+                The number according to the computational basis order.
 
         Examples
         --------
         .. todo::
             valid examples
         """
         ket = np.zeros(self.hilb_dim, dtype=float)
-        ket[self._graph.arc_number(*args)] = 1
+        ket[self._graph.arc_number(arc)] = 1
 
         return ket
 
-    def _prepare_engine(self, initial_state, hpc):
-        if hpc:
+    def _prepare_engine(self, state, hpc):
+        if hpc is not None:
             S = nbl.send_matrix(self.get_shift())
             C = nbl.send_matrix(self.get_coin())
             self._simul_mat = (C, S)
-            self._simul_vec = nbl.send_vector(initial_state)
+            self._simul_vec = nbl.send_vector(state)
 
             dtype = (complex if (S.is_complex or C.is_complex
-                                 or np.iscomplex(initial_state.dtype))
+                                 or np.iscomplex(state.dtype))
                      else np.double)
 
             return dtype
 
-        else:
-            return super()._prepare_engine(initial_state, hpc)
+        return super()._prepare_engine(state, hpc)
 
 
     def _simulate_step(self, step, hpc):
-        if hpc:
+        if hpc is not None:
             for i in range(step):
                 self._simul_vec = nbl.multiply_matrix_vector(
                     self._simul_mat[0], self._simul_vec)
 
                 self._simul_vec = nbl.multiply_matrix_vector(
                     self._simul_mat[1], self._simul_vec)
         else:
             super()._simulate_step(step, hpc)
+
+    def probability(self, states, vertices):
+        r"""
+        Computes the sum of probabilities for the specified vertices.
+        
+        Computes the probability of the walker being located on a
+        vertex within the set of provided vertices, given that the walk 
+        is on specified states.
+        
+        Parameters
+        ----------
+        states : :class:`numpy.ndarray`
+            The state(s) used to compute the probability.
+            ``states`` can be a single state or a list of states.
+        
+        vertices: list of int
+           The subset of vertices. 
+        
+        Returns
+        -------
+        probabilities : float or :class:`numpy.ndarray`
+            float:
+                If ``states`` is a single state.
+            :class:`numpy.ndarray`:
+                If ``states`` is a list of states,
+                ``probabilities[i]`` is the probability
+                corresponding to the ``i``-th state.
+        
+        See Also
+        --------
+        simulate
+        
+        Notes
+        -----
+        
+        The probability of finding the walker on vertex 
+        :math:`v`, given the state of the walk
+        :math:`|\psi \rangle`, is calculated as
+
+        .. math::
+            \sum_{\substack{a\in{\mathcal{A}}\\ \operatorname{tail}(a)=v}} \, 
+            \left|{\langle a} | {\psi \rangle}\right|^2,
+
+        where :math:`\mathcal{A}` denotes the set of arcs.        
+        """
+        return super().probability(states, vertices)
```

### Comparing `hiperwalk-2.0b1/hiperwalk/quantum_walk/continuous_time.py` & `hiperwalk-2.0b11/hiperwalk/quantum_walk/continuous_time.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,264 +1,364 @@
 import numpy as np
 import scipy.sparse
 import scipy.linalg
 from .quantum_walk import QuantumWalk
-from .._constants import PYNEBLINA_IMPORT_ERROR_MSG
-try:
-    from . import _pyneblina_interface as nbl
-except:
-    pass
+from . import _pyneblina_interface as nbl
 
 class ContinuousTime(QuantumWalk):
     r"""
-    Manage an instance of a continuous-time quantum walk
-    on any simple graph.
-
-    For further implementation details, refer to the Notes Section.
+    Manage instances of continuous-time quantum walks on graphs.
+    
+    For further implementation details and theoretical background, 
+    refer to the Notes Section.
 
     Parameters
     ----------
     graph :
         Graph on which the quantum walk takes place.
         There are two acceptable inputs:
 
-        :class:`hiperwalk.graph.Graph` :
-            The graph itself.
-
-        :class:`class:scipy.sparse.csr_array`:
-            The adjacency matrix of the graph.
-
-    gamma : float
-        Gamma value for setting Hamiltonian.
+        * Simple graph (:class:`hiperwalk.Graph`);
+        * Weighted graph (:class:`hiperwalk.WeightedGraph`);
 
     **kwargs : optional
-        Arguments to set the Hamiltonian and evolution operator.
+        Additional arguments to set the Hamiltonian and evolution operator.
 
     See Also
     --------
     set_hamiltonian
     set_evolution
 
     Notes
     -----
-    The adjacency matrix of a graph :math:`G(V, E)` is
-    the :math:`|V| \times |V|`-dimensional matrix :math:`A` such that
+    The continuous-time quantum walk model represents quantum particles 
+    evolving on a graph in continuous time, as directed by the Schrödinger 
+    equation. The Hamiltonian is usually chosen as the adjacency matrix 
+    or the Laplacian of the graph. A positive parameter gamma acts 
+    as a weighting factor for the Hamiltonian, adjusting the walk's 
+    spreading rate. When marked vertices are present, 
+    the Hamiltonian is suitably modified.
+    
+    The computational basis associated with a graph 
+    :math:`G(V, E)` comprising :math:`n` vertices
+    :math:`v_0, \ldots, v_{n-1}` is spanned by the states 
+    :math:`\ket{i}` for
+    :math:`0 \leq i < n`, where
+    :math:`\ket{i}` describes the walker's position
+    as vertex :math:`v_i`.
+    
+    The adjacency matrix of :math:`G(V, E)` is the 
+    :math:`n`-dimensional matrix :math:`A` such that
     
     .. math::
         A_{i,j} = \begin{cases}
-            1, \text{ if } (i,j) \in E(G),\\
+            1, \text{ if } v_i \text{ is adjacent to } v_j,\\
+            0, \text{ otherwise.}
+        \end{cases}
+        
+    Similarly, the Laplacian matrix is defined as
+    
+    .. math::
+        L_{i,j} = \begin{cases}
+            \text{degree}(v_i), \text{ if } i=j,\\
+            -1, \text{ if } i\neq j \text{ and }
+                v_i \text{ is adjacent to } v_j,\\
             0, \text{ otherwise.}
         \end{cases}
 
-    The Hamiltonian, which depends on the adjacency matrix and the location of 
-    the marked vertices, is described in the
-    :meth:`hiperwalk.ContinuousTime.set_hamiltonian` method.
-
-    The states of the computational basis are :math:`\ket{i}` for
-    :math:`0 \leq i < |V|`, where
-    :math:`\ket i` is associated with the :math:`i`-th vertex.
-
-    This class can also facilitate the simulation of any Hamiltonian
-    evolution. To do this, simply pass the desired Hamiltonian in place
-    of the adjacency matrix.
+    The Hamiltonian's formulation is detailed in 
+    :meth:`hiperwalk.ContinuousTime.set_hamiltonian`, 
+    depending on the choice between the adjacency 
+    or Laplacian matrix, along with the positioning 
+    of the marked vertices.
+
+    The :class:`hiperwalk.ContinuousTime` class enables the simulation of
+    real Hamiltonians.
+    A particular Hamiltonian :math:`H`,
+    can be simulated by creating a :class:`hiperwalk.WeightedGraph`
+    with adjacency matrix :math:`C` such that :math:`H = -\gamma C`.
+    Additionally, the Laplacian matrix is computed 
+    as :math:`D - A`, with :math:`D` being 
+    the degree matrix. 
+    See :meth:`hiperwalk.Graph.adjacency_matrix`
+    and :meth:`hiperwalk.Graph.laplacian_matrix`.
+    
+    For a comprehensive understanding of continuous-time quantum 
+    walks, consult reference [1]_. 
+    To examine the differences between utilizing 
+    the adjacency matrix and the Laplacian matrix, 
+    refer to reference [2]_.
+    
+    References
+    ----------
+    .. [1] E. Farhi and S. Gutmann. "Quantum computation and decision trees". 
+        Physical Review A, 58(2):915–928, 1998. ArXiv:quant-ph/9706062.
+        
+    .. [2] T. G. Wong, L. Tarrataca, and N. Nahimov. Laplacian versus adjacency 
+    	matrix in quantum walk search. Quantum Inf Process 15, 4029-4048, 2016.
     """
 
     _valid_kwargs = dict()
 
-    def __init__(self, graph=None, gamma=None, **kwargs):
+    def __init__(self, graph=None, **kwargs):
 
         super().__init__(graph=graph)
 
         # create attributes
         self.hilb_dim = self._graph.number_of_vertices()
+
         self._gamma = None
+        self._hamil_type = None
+        self._terms = None
         self._hamiltonian = None
-        self._evolution = None
-        self._evolution_time = None
+
+        self._time = None
 
         # import inspect
 
         if not bool(ContinuousTime._valid_kwargs):
             # assign static attribute
             ContinuousTime._valid_kwargs = {
                 'gamma': ContinuousTime._get_valid_kwargs(
-                    self._update_gamma),
+                    self._set_gamma),
                 'marked': ContinuousTime._get_valid_kwargs(
-                    self._update_marked),
+                    self._set_marked),
                 'evolution': ContinuousTime._get_valid_kwargs(
-                    self._update_evolution),
+                    self._set_evolution),
                 'time': ContinuousTime._get_valid_kwargs(
-                    self._update_time),
+                    self._set_time),
                 }
 
-        if not 'time' in kwargs:
-            kwargs['time'] = 0
+        self.set_evolution(**kwargs)
 
-        self.set_evolution(gamma=gamma, **kwargs)
-
-    def _update_gamma(self, gamma=None):
+    def _set_gamma(self, gamma=0.1):
         if gamma is None or gamma.imag != 0:
             raise TypeError("Value of 'gamma' is not float.")
 
         if self._gamma != gamma:
             self._gamma = gamma
             return True
         return False
 
-    def set_gamma(self, gamma=None, **kwargs):
+    def set_gamma(self, gamma=0.1):
         r"""
-        Sets the gamma parameter.
+        Set gamma.
         
-        The gamma parameter is used in the definition of the Hamiltonian.
-        By setting gamma,
-        both the Hamiltonian and evolution operator are updated.
+        Parameter gamma is used in the definition of the
+        Hamiltonian to determine the hopping probability per unit 
+        of time. Upon setting gamma, both the Hamiltonian and evolution 
+        operators are updated.
 
         Parameters
         ----------
-        gamma : float
-            Gamma value.
-
-        ** kwargs :
-            Additional arguments for updating the evolution operator.
-            For example, whether to use neblina HPC or not.
-            See :meth:`set_evolution` for more options.
+        gamma : float, default=0.1
+            The value of gamma.
 
         Raises
         ------
         TypeError
             If ``gamma`` is ``None`` or complex.
         ValueError
             If ``gamma < 0``.
         """
-        if self._update_gamma(gamma=gamma):
-            self._update_hamiltonian()
-            self._update_evolution(**kwargs)
+        self.set_hamiltonian(gamma=gamma,
+                             type=self._hamil_type,
+                             marked=self._marked)
 
     def get_gamma(self):
         r"""
-        Retrieves the gamma value used in
+        Retrieve the value of gamma used in
         the definition of the Hamiltonian.
 
         Returns
         -------
         float
+        
+        See Also
+        --------
+        set_gamma
         """
         return self._gamma
 
-    def set_marked(self, marked=[], **kwargs):
-        self._update_marked(marked=marked)
-        self._update_hamiltonian()
-        self._update_evolution(**kwargs)
+    def set_marked(self, marked=[]):
+        self.set_hamiltonian(gamma=self._gamma,
+                             type=self._hamil_type,
+                             marked=marked)
+
+    def _set_hamiltonian(self, gamma=0.1, type='adjacency', marked=[]):
+        update = self._set_gamma(gamma)
+        update = self._set_hamiltonian_type(type) or update
+        update = self._set_marked(marked) or update
+
+        if update:
+            if self._hamil_type == 'adjacency':
+                H = -self._gamma * self._graph.adjacency_matrix()
+            else:
+                H = -self._gamma * self._graph.laplacian_matrix()
 
-    def _update_hamiltonian(self):
-        r"""
-        If this method is invoked,
-        the hamiltonian is recalculated
-        """
-        self._hamiltonian = -self._gamma * self._graph.adjacency_matrix()
+            # creating oracle
+            if len(self._marked) > 0:
+                data = np.ones(len(self._marked), dtype=np.int8)
+                oracle = scipy.sparse.csr_array(
+                        (data, (self._marked, self._marked)),
+                        shape=(self.hilb_dim, self.hilb_dim))
+
+                H -= oracle
 
-        # creating oracle
-        if len(self._marked) > 0:
-            data = np.ones(len(self._marked), dtype=np.int8)
-            oracle = scipy.sparse.csr_array(
-                    (data, (self._marked, self._marked)),
-                    shape=(self.hilb_dim, self.hilb_dim))
+            self._hamiltonian = H
 
-            self._hamiltonian -= oracle
+        return update
 
-    def set_hamiltonian(self, gamma=None, **kwargs):
+    def set_hamiltonian(self, gamma=0.1, type="adjacency", marked=[]):
         r"""
-        Creates the Hamiltonian.
+        Set the Hamiltonian.
 
-        If no marked vertices is specified,
-        the default value is used.
-        After the Hamiltonian is created,
-        the evolution operator is updated accordingly.
+        The Hamiltonian takes the form of ``-gamma*C`` wheres
+        ``C`` is either the adjacency matrix or the Laplacian matrix.
+        If marked vertices are specified, the Hamiltonian 
+        is modified as described in the Notes section. 
+        Once the Hamiltonian has been established, 
+        the evolution operator is updated accordingly. 
 
         Parameters
         ----------
-        gamma : float
-            Gamma value.
+        gamma : float, default=0.1
+            The value of gamma.
 
-        **kwargs :
-            Used for determining the marked vertices, and
-            the procedure for updating the evolution operator.
-            See :meth:`hiperwalk.ContinuousTime.set_marked`, and
-            See :meth:`hiperwalk.ContinuousTime.set_evolution`.
+        type: {'adjacency', 'laplacian'}
+            Two types of Hamiltonian are used:
+            ``'A'`` is shorthand for ``'adjacency'`` (default).
+            ``'L'`` is shorthand for ``'laplacian'``.
+
+        marked : list of vertices, default=[]
+            List of vertices to be marked.
+            If empty list, no vertex is marked.
 
         Raises
         ------
         TypeError
             If ``gamma`` is ``None`` or complex.
         ValueError
             If ``gamma < 0``.
 
         See Also
         --------
         set_gamma
+        set_hamiltonian_type
         set_marked
         set_evolution
 
         Notes
         -----
-        The Hamiltonian is given by
+        The Hamiltonian is given by [1]_ [2]_
 
         .. math::
-            H = -\gamma A  - \sum_{m \in M} \ket m \bra m,
+            H = -\gamma C  - \sum_{m \in M} \ket m \bra m,
 
-        where :math:`A` is the adjacency matrix, and
-        :math:`M` is the set of marked vertices.
+        where :math:`C` is either the adjacency matrix or
+        the Laplacian matrix.
+        The set :math:`M` specifies the marked vertices via
+        the argument ``marked=M``. For instance, ``marked={0}``
+        specifies that :math:`v_0` is the marked vertex.
+        The default is :math:`M=\emptyset`.
+        
+        References
+        ----------
+        .. [1] E. Farhi and S. Gutmann.
+            "Quantum computation and decision trees". 
+            Physical Review A, 58(2):915–928, 1998.
+            ArXiv:quant-ph/9706062.
+        
+        .. [2] A. M. Childs and J. Goldstone.
+            "Spatial search by quantum walk",
+            Phys. Rev. A 70, 022314, 2004.
         """
-        self._update_gamma(gamma=gamma)
-
-        marked_kwargs = ContinuousTime._pop_valid_kwargs(kwargs,
-                ContinuousTime._valid_kwargs['marked'])
-        self._update_marked(**marked_kwargs)
-
-        self._update_hamiltonian()
-        self._update_evolution(**kwargs)
+        self.set_evolution(time=self._time,
+                           terms=self._terms,
+                           gamma=gamma,
+                           type=type,
+                           marked=marked)
 
     def get_hamiltonian(self):
         r"""
-        Returns the Hamiltonian.
+        Retrieve the Hamiltonian.
 
         Returns
         -------
         :class:`scipy.sparse.csr_array`
-        """
 
+        See Also
+        --------
+        set_hamiltonian
+        """
         return self._hamiltonian
 
-    def _update_time(self, time=None):
+    def _set_hamiltonian_type(self, type='adjacency'):
+        if type.upper() == 'A':
+            type = 'adjacency'
+        elif type.upper() == 'L':
+            type = 'laplacian'
+
+        if type != self._hamil_type:
+            self._hamil_type = type
+            return True
+
+        return False
+
+    def set_hamiltonian_type(self, type='adjacency'):
+        r"""
+        Set the type of the Hamiltonian.
+        
+        Parameters
+        ----------
+        type: {'adjacency', 'laplacian'}
+            Two types of Hamiltonian are used:
+            ``'A'`` is shorthand for ``'adjacency'``.
+            ``'L'`` is shorthand for ``'laplacian'``.
+        """
+        self.set_hamiltonian(gamma=self._gamma,
+                             type=type,
+                             marked=self._marked)
+
+    def get_hamiltonian_type():
+        r"""
+        Retrieve the type of the Hamiltonian.
+        
+        See Also
+        --------
+        set_hamiltonian_type
+        
+        Returns
+        -------
+        type: {'adjacency', 'laplacian'}
+        """
+        return self._hamil_type
+
+
+    def _set_time(self, time=1):
         if time is None or time < 0:
             raise ValueError(
                 "Expected non-negative `time` value."
             )
 
-        if time != self._evolution_time:
-            self._evolution_time = time
+        if time != self._time:
+            self._time = time
             return True
         return False
 
-    def set_time(self, time=None, **kwargs):
+    def set_time(self, time=1):
         r"""
-        Sets time.
+        Set a time instant.
 
-        Sets time and
-        generates the evolution operator corresponding to
-        the specified time.
+        Defines a time t and calculates the evolution operator U(t) at
+        the specified time (see Notes).
 
         Parameters
         ----------
-        time : float
-
-        ** kwargs :
-            Additional arguments for updating the evolution operator.
-            For example, whether to use neblina HPC or not.
-            See :meth:`set_evolution` for more options.
+        time : float, default=1
 
         Raises
         ------
         ValueError
             If ``time < 0``.
 
         See Also
@@ -266,38 +366,82 @@
         set_evolution
 
         Notes
         -----
         The evolution operator is given by
 
         .. math::
-            U(t) = e^{-\text{i}tH},
+            U(t) = 	\text{e}^{-\text{i}tH},
 
         where :math:`H` is the Hamiltonian, and
         :math:`t` is the time.
         """
-        if self._update_time(time=time):
-            self._update_evolution(**kwargs)
+        self.set_evolution(time=time,
+                           terms=self._terms,
+                           gamma=self._gamma,
+                           type=self._hamil_type,
+                           marked=self._marked)
+
+    def _set_terms(self, terms=21):
+        if self._terms != terms:
+            self._terms = terms
+            return True
+        return False
+
+    def set_terms(self, terms=21):
+        r"""
+        Set the number of terms used to calculate the
+        evolution operator as a power series.
+
+        Parameters
+        ----------
+        terms : int, default=20
+            Number of terms in the truncated Taylor series expansion.
+
+        See Also
+        --------
+        set_evolution
+        """
+        self.set_evolution(time=self._time,
+                           terms=terms,
+                           gamma=self._gamma,
+                           type=self._hamil_type,
+                           marked=self._marked)
 
-    def _update_evolution(self, hpc=True, terms=21):
+    def get_terms(self):
+        r"""
+        Retrieve the number of terms in the power series used to
+        calculate the evolution operator.
+
+        Returns
+        -------
+        int
+
+        See Also
+        --------
+        set_terms
+        set_evolution
+        """
+        return self._terms
+
+    def _set_evolution(self, terms=21):
         r"""
         If this method is invoked,
         the evolution is recalculated
         """
-        time = self._evolution_time
+        time = self._time
 
         if time == 0:
             self._evolution = np.eye(self.hilb_dim)
             return
 
         n = terms - 1
         H = self.get_hamiltonian()
 
-        if hpc and not self._pyneblina_imported():
-            hpc = False
+        hpc = nbl.get_hpc()
 
         #TODO: when scipy issue 18086 is solved,
         # invoke scipy.linalg.expm to calculate power series
         def numpy_matrix_power_series(A, n):
             """
             I + A + A^2/2 + A^3/3! + ... + A^n/n!
             """
@@ -308,15 +452,15 @@
                 U += curr_term
 
             return U
 
         # determining the number of terms in power series
         max_val = np.max(np.abs(H))
         if max_val*time <= 1:
-            if hpc:
+            if hpc is not None:
                 nbl_U = nbl.matrix_power_series(-1j*time*H, n)
             else:
                 U = numpy_matrix_power_series(-1j*time*H.todense(), n)
 
         else:
             # if the order of magnitude is very large,
             # float point errors may occur
@@ -328,136 +472,95 @@
             else:
                 # TODO: assert precision
                 new_time = max_val*time
                 order = np.ceil(np.math.log(new_time, n))
                 new_time /= 10**order
                 num_mult = int(np.round(time/new_time)) - 1
 
-            if hpc:
+            if hpc is not None:
                 new_nbl_U = nbl.matrix_power_series(
                         -1j*new_time*H, n)
                 nbl_U = nbl.multiply_matrices(new_nbl_U, new_nbl_U)
                 for i in range(num_mult - 1):
                     nbl_U = nbl.multiply_matrices(nbl_U, new_nbl_U)
             else:
                 U = numpy_matrix_power_series(
                         -1j*new_time*H.todense(), n)
                 U = np.linalg.matrix_power(U, num_mult + 1)
 
-        if hpc:
+        if hpc is not None:
             U = nbl.retrieve_matrix(nbl_U)
 
         self._evolution = U
 
-    def set_evolution(self, hpc=True, terms=21, **kwargs):
+    def set_evolution(self, **kwargs):
         r"""
-        Sets the evolution operator.
+        Set the evolution operator.
 
-        Sets Hamiltonian and time.
-        They are set using the appropriate ``**kwargs``.
-        If ``**kwargs`` is empty, the default arguments are used.
-        Then, the evolution operator is constructed using
-        a Taylor series expansion.
+        This method defines the evolution operator for a specified 
+        ``time``.
+        It first determines the 
+        Hamiltonian and subsequently derives the evolution operator 
+        via a truncated Taylor series. The default number of terms 
+        in this series is set to ``terms=21``, which is adequate 
+        when the Hamiltonian is derived from the adjacency matrix 
+        and gamma is less than 1.
 
         Parameters
         ----------
-        hpc : bool, default = True
-            Determines whether or not to use neblina HPC 
-            functions to generate the evolution operator.
-
-        terms : int
-            Number of terms in Taylor series expansion.
-
         **kwargs :
             Additional arguments for setting Hamiltonian and time.
-            See :meth:`hiperwalk.ContinuousTime.set_hamiltonian`, and
-            :meth:`hiperwalk.ContinuousTime.set_time`.
             If omitted, the default arguments are used.
+            See :meth:`hiperwalk.ContinuousTime.set_hamiltonian`,
+            :meth:`hiperwalk.ContinuousTime.set_time`, and
+            :meth:`hiperwalk.ContinuousTime.set_terms`.
 
         See Also
         --------
         set_hamiltonian
         set_time
+        set_terms
 
         Notes
         -----
         The evolution operator is given by
 
         .. math::
-            U(t) = e^{-\text{i}tH},
+            U(t) = 	\text{e}^{-\text{i}tH},
 
         where :math:`H` is the Hamiltonian, and
         :math:`t` is the time.
 
-        The Taylor series expansion is given by
-
+        The :math:`n\text{th}` partial sum of
+        the Taylor series expansion is given by
+        
         .. math::
-            e^{-\text{i}tH} &= \sum_{j = 0}^{n} (\text{i}tH)^j / j!
+            \text{e}^{-\text{i}tH} \approx
+            \sum_{j = 0}^{n-1} (-\text{i}tH)^j / j!
 
-        where :math:`n` is the number of terms minus 1
-        (i.e. ``terms - 1``).
+        where ``terms``:math:`=n`.
+        This choice reflects default Python loops over integers,
+        such as ``range`` and ``np.arange``.
 
         .. warning::
             For non-integer time (floating number),
             the result is approximate. It is recommended 
             to select a small time interval and perform 
             multiple matrix multiplications to minimize 
             rounding errors.
 
         .. todo::
-            Use ``scipy.linalg.expm`` when ``hpc=False`` once the
+            Use ``scipy.linalg.expm`` when ``hpc=None`` once the
             `scipy issue 18086
             <https://github.com/scipy/scipy/issues/18086>`_
             is solved.
         """
-        self._update_time(**ContinuousTime._pop_valid_kwargs(
-            kwargs,
-            ContinuousTime._valid_kwargs['time']))
-        self.set_hamiltonian(**kwargs)
-
-    def simulate(self, time=None, initial_state=None, hpc=True):
-        r"""
-        Analogous to :meth:`hiperwalk.QuantumWalk.simulate`,
-        which accepts float entries for the ``time`` parameter.
-
-        Parameters
-        ----------
-        time : float or tuple of floats
-            This parameter is analogous to those in
-            :meth:`hiperwalk.QuantumWalk.simulate`,
-            with the distinction that it accepts float inputs.
-            The ``step`` parameter is used to construct the evolution operator.
-            The states within the interval
-            **[** ``start/step``, ``end/step`` **]** are stored.
-            The values describing this interval are
-            rounded up if the decimal part exceeds ``1 - 1e-5``,
-            and rounded down otherwise.
-
-        Other Parameters
-        ----------------
-        See `hiperwalk.QuantumWalk.simulate`.
-
-        See Also
-        --------
-        set_evolution
-        get_evolution
-        """
-        if time is None:
-            raise ValueError(
-                "Invalid `time_range`. Expected a float, 2-tuple, "
-                + "or 3-tuple of float."
-            )
-
-        time = np.array(QuantumWalk._time_to_tuple(time))
-
-        self.set_time(time=time[2])
-
-        # cleaning time_range to int
-        tol = 1e-5
-        time = [int(val/time[2])
-                if int(val/time[2])
-                   <= np.ceil(val/time[2]) - tol
-                else int(np.ceil(val/time[2]))
-                for val in time]
-
-        states = super().simulate(time, initial_state, hpc)
-        return states
+        def filter_and_call(method, update):
+            valid = self._get_valid_kwargs(method)
+            filtered = self._filter_valid_kwargs(kwargs, valid)
+            return method(**filtered) or update
+
+        update = filter_and_call(self._set_time, False)
+        update = filter_and_call(self._set_hamiltonian, update)
+        update = filter_and_call(self._set_terms, update)
+        if (update):
+            filter_and_call(self._set_evolution, update)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hiperwalk-2.0b1/tests/unit/coined_cycle.py` & `hiperwalk-2.0b11/tests/unit/coined_cycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,51 +5,52 @@
 from test_constants import *
 import hiperwalk as hpw
 import unittest
 
 class TestCoinedCycle(unittest.TestCase):
 
     def setUp(self):
+        hpw.set_hpc(None)
         self.num_vert = 10
         self.cycle = hpw.Cycle(self.num_vert)
         self.qw = hpw.Coined(self.cycle)
 
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_clockwise_roundabout(self):
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
-        init_state = self.qw.state([1, (0, 1)])
+        init_state = self.qw.state([[1, (0, 1)]])
 
         num_steps = self.num_vert
-        final_state = self.qw.simulate(num_steps, init_state, hpc=False)[0]
+        final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_anticlockwise_roundabout(self):
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
-        init_state = self.qw.state([1, (0, self.num_vert - 1)])
+        init_state = self.qw.state([[1, (0, self.num_vert - 1)]])
 
         num_steps = self.num_vert
-        final_state = self.qw.simulate(num_steps, init_state, hpc=False)[0]
+        final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_hadamard_evolution_operator(self):
-        init_state = self.qw.state((1, (0, 1)))
+        init_state = self.qw.state([(1, (0, 1))])
 
         num_steps = 2*self.num_vert
-        states = self.qw.simulate((num_steps, 1), init_state, hpc=False)
+        states = self.qw.simulate((num_steps, 1), init_state)
         states = states.real
 
         def recursive_expression():
             states = np.zeros((num_steps + 1, init_state.shape[0]))
             states[0] = np.copy(init_state)
             num_arcs = 2*self.num_vert
 
@@ -69,43 +70,53 @@
         rec_states = recursive_expression()
         
         self.assertTrue(np.allclose(states, rec_states,
                                     rtol=1e-15, atol=1e-15))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_clockwise_roundabout(self):
+        hpw.set_hpc('cpu')
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
         init_state = self.qw.state([1, (0, 1)])
 
         num_steps = self.num_vert
-        final_state = self.qw.simulate(num_steps, init_state, hpc=True)[0]
+        final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_anticlockwise_roundabout(self):
+        hpw.set_hpc('cpu')
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
         init_state = self.qw.state([1, (0, self.num_vert - 1)])
 
         num_steps = self.num_vert
-        final_state = self.qw.simulate(num_steps, init_state, hpc=True)[0]
+        final_state = self.qw.simulate(num_steps, init_state)[0]
 
         self.assertTrue(np.all(init_state == final_state))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_evolution_operator_matches_nonhpc(self):
         init_state = self.qw.state([1, (0, 1)])
         num_steps = 2*self.num_vert
 
-        states = self.qw.simulate(
-            (num_steps, 1), init_state, hpc=False)
-        hpc_states = self.qw.simulate(
-            (num_steps, 1), init_state, hpc=True)
+        hpw.set_hpc(None)
+        states = self.qw.simulate((num_steps, 1), init_state)
+
+        hpw.set_hpc('cpu')
+        hpc_states = self.qw.simulate((num_steps, 1), init_state)
         
         self.assertTrue(np.allclose(states, hpc_states,
                                     rtol=1e-15, atol=1e-15))
+
+    @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
+    def test_set_explicit_coin(self):
+        C = self.qw.get_coin()
+        self.qw.set_coin(coin=C)
+        C2 = self.qw.get_coin()
+        self.assertTrue((C - C2).nnz == 0)
```

### Comparing `hiperwalk-2.0b1/tests/unit/coined_line.py` & `hiperwalk-2.0b11/tests/unit/coined_line.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 import hiperwalk as hpw
 import unittest
 from test_constants import *
 
 class TestCoinedLine(unittest.TestCase):
 
     def setUp(self):
+        hpw.set_hpc(None)
         self.num_vert = 41
         self.line = hpw.Line(self.num_vert)
         self.qw = hpw.Coined(self.line)
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_persistent_shift_right_state_transfer(self):
         # initial state in leftmost vertex
         # final state in rightmost vertex
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
-        init_state = self.qw.state([1, (0, 1)])
+        init_state = self.qw.state([[1, (0, 1)]])
 
         num_steps = self.num_vert - 1
-        final_state = self.qw.simulate(num_steps, init_state, hpc=False)
+        final_state = self.qw.simulate(num_steps, init_state)
         final_state = final_state[0]
 
         self.assertTrue(
             final_state[-1] == 1 and np.all(final_state[:-1] == 0)
         )
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
@@ -36,18 +37,18 @@
         # initial state in leftmost vertex
         # final state in rightmost vertex
         self.qw.set_shift('persistent')
         self.qw.set_coin('I')
         self.qw.set_marked([])
 
         init_state = self.qw.state(
-            [1, (self.num_vert - 1, self.num_vert - 2)])
+            [[1, (self.num_vert - 1, self.num_vert - 2)]])
 
         num_steps = self.num_vert - 1
-        final_state = self.qw.simulate(num_steps, init_state, hpc=False)
+        final_state = self.qw.simulate(num_steps, init_state)
         final_state = final_state[0]
 
         self.assertTrue(
             final_state[0] == 1 and np.all(final_state[1:] == 0)
         )
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
@@ -55,13 +56,22 @@
 
         num_steps = self.num_vert // 2
         center = self.num_vert // 2
         entries = [[1, (center, center + 1)],
                    [-1j, (center, center - 1)]]
         init_state = self.qw.state(*entries)
 
-        states = self.qw.simulate((num_steps, 1), init_state, hpc=False)
-        hpc_states = self.qw.simulate((num_steps, 1), init_state, hpc=True)
+        hpw.set_hpc(None)
+        states = self.qw.simulate((num_steps, 1), init_state)
+        hpw.set_hpc('cpu')
+        hpc_states = self.qw.simulate((num_steps, 1), init_state)
 
         self.assertTrue(
             np.allclose(states, hpc_states, rtol=1e-15, atol=1e-15)
         )
+
+    @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
+    def test_set_explicit_coin(self):
+        C = self.qw.get_coin()
+        self.qw.set_coin(coin=C)
+        C2 = self.qw.get_coin()
+        self.assertTrue((C - C2).nnz == 0)
```

### Comparing `hiperwalk-2.0b1/tests/unit/complete_bipartite.py` & `hiperwalk-2.0b11/tests/unit/hypercube.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,37 +2,33 @@
 from sys import path as sys_path
 sys_path.append('../')
 sys_path.append('../../')
 from test_constants import *
 import hiperwalk as hpw
 import unittest
 
-class TestCompleteBipartite(unittest.TestCase):
+class TestHypercube(unittest.TestCase):
     
     def setUp(self):
-        self.n1 = 20
-        self.n2 = 30
-        self.g = hpw.CompleteBipartite(self.n1, self.n2)
+        self.dim = 10
+        hypercube = hpw.Hypercube(self.dim)
+        self.g = hpw.SDMultigraph(hypercube)
 
     def tearDown(self):
         del self.g
 
+    def test_arc_direction(self):
+        array = [self.g._neighbor_index(*self.g.arc(a))
+                 for a in range(self.g.number_of_arcs())]
+        num_vert = self.g.number_of_vertices()
+        self.assertTrue(array == list(range(self.dim))*num_vert)
+
     def test_arc_number(self):
-        array = [self.g.arc_number((u, v))
-                 for u in range(self.g.number_of_vertices())
-                 for v in self.g.neighbors(u)]
-        self.assertTrue(np.all(
-            array == list(range(self.g.number_of_arcs()))))
+        array = [self.g.arc_number((v, v ^ 1 << direction))
+                 for v in range(self.g.number_of_vertices())
+                 for direction in range(self.dim)]
+        self.assertTrue(array == list(range(self.g.number_of_arcs())))
 
     def test_arc(self):
         array = [self.g.arc_number((self.g.arc(a)[0], self.g.arc(a)[1]))
                  for a in range(self.g.number_of_arcs())]
         self.assertTrue(array == list(range(self.g.number_of_arcs())))
-
-    def test_invertibility_of_arc_and_arc_number(self):
-        arc_number1 = np.arange(self.g.number_of_arcs())
-        arc_notation1 = list(map(self.g.arc, arc_number1))
-        arc_number2 = list(map(self.g.arc_number, arc_notation1))
-        arc_notation2 = list(map(self.g.arc, arc_number1))
-
-        self.assertTrue(np.all(arc_number1 == arc_number2))
-        self.assertTrue(np.all(arc_notation1 == arc_notation2))
```

### Comparing `hiperwalk-2.0b1/tests/unit/continuous_graph.py` & `hiperwalk-2.0b11/tests/unit/continuous_time.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 from sys import path as sys_path
 sys_path.append('../')
 sys_path.append('../../')
 from test_constants import *
 import hiperwalk as hpw
 import unittest
 
-class TestContinuousGraph(unittest.TestCase):
+class TestContinuousTime(unittest.TestCase):
 
     def setUp(self):
+        hpw.set_hpc(None)
         self.num_vert = 40
         nx_graph = nx.ladder_graph(self.num_vert // 2)
         self.adj = nx.adjacency_matrix(nx_graph)
-        self.g = hpw.Graph(self.adj)
+        self.g = hpw.Graph(self.adj, copy=True)
         self.gamma = 1/2
         self.qw = hpw.ContinuousTime(self.g, gamma=self.gamma)
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_hamiltonian_default(self):
         H = self.qw.get_hamiltonian()
         self.assertTrue((H - (-self.gamma*self.adj) != 0).nnz == 0)
@@ -48,62 +49,61 @@
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_evolution_operator_invalid_time(self):
         marked = self.qw._marked
         H = self.qw._hamiltonian
         U = self.qw._evolution
 
         self.assertRaises(ValueError, self.qw.set_evolution,
-                          time=-1, gamma=self.qw.get_gamma(),
-                          hpc=False)
+                          time=-1, gamma=self.qw.get_gamma())
 
         self.assertTrue(id(marked) == id(self.qw._marked))
         self.assertTrue(id(H) == id(self.qw._hamiltonian))
         self.assertTrue(id(U) == id(self.qw._evolution))
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_evolution_operator_set_hamiltonian_no_marked(self):
         prev_marked = self.qw._marked
         prev_H = self.qw._hamiltonian
         prev_U = self.qw._evolution
 
-        self.qw.set_evolution(time=1, hpc=False, gamma=1, marked=[])
+        self.qw.set_evolution(time=1, gamma=1, marked=[])
         U = self.qw.get_evolution()
 
         self.assertTrue(U is not None)
         self.assertTrue(self.qw._evolution is not None)
         self.assertTrue(id(prev_marked) != id(self.qw._marked))
         self.assertTrue(id(prev_H) != id(self.qw._hamiltonian))
         self.assertTrue(id(prev_U) != id(self.qw._evolution))
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_evolution_operator_set_hamiltonian_and_marked(self):
         prev_marked = self.qw._marked
         prev_H = self.qw._hamiltonian
         prev_U = self.qw._evolution
 
-        self.qw.set_evolution(time=1, gamma=1, marked=[0], hpc=False)
+        self.qw.set_evolution(time=1, gamma=1, marked=[0])
         U = self.qw.get_evolution()
 
         self.assertTrue(U is not None)
         self.assertTrue(self.qw._evolution is not None)
         self.assertTrue(id(prev_marked) != id(self.qw._marked))
         self.assertTrue(id(prev_H) != id(self.qw._hamiltonian))
         self.assertTrue(id(prev_U) != id(self.qw._evolution))
 
     @unittest.skipIf(not TEST_NONHPC, 'Skipping nonhpc tests.')
     def test_evolution_unitary(self):
-        U = self.qw.set_evolution(gamma=self.qw.get_gamma(),
-                time=1, hpc=False)
+        U = self.qw.set_evolution(gamma=self.qw.get_gamma(), time=1)
         U = self.qw.get_evolution()
 
         self.assertTrue(np.allclose(
             U@U.T.conjugate(), np.eye(U.shape[0])
         ))
 
     @unittest.skipIf(not TEST_HPC, 'Skipping hpc tests.')
     def test_hpc_evolution_unitary(self):
-        self.qw.set_time(time=1, hpc=True)
+        hpw.set_hpc('cpu')
+        self.qw.set_time(time=1)
         U = self.qw.get_evolution()
 
         self.assertTrue(np.allclose(
             U@U.T.conjugate(), np.eye(U.shape[0])
         ))
```

### Comparing `hiperwalk-2.0b1/.gitignore` & `hiperwalk-2.0b11/.gitignore`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,20 @@
 
 # PyBuilder
 target/
 
 # Text Editors / IDE extra files
 .ipynb_checkpoints/
 *.swp
+.vscode/
 
 # Output files
 *.png
 *.gif
 *.mp4
 
 # Documentation autogenerated files
 docs/documentation/generated/
+docs/documentation/graph_constructors/generated/
+
+# Test constants
+tests/test_constants.py
```

### Comparing `hiperwalk-2.0b1/LICENSE` & `hiperwalk-2.0b11/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/README.md` & `hiperwalk-2.0b11/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0b1/pyproject.toml` & `hiperwalk-2.0b11/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0b1"
+version = "2.0b11"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
```

### Comparing `hiperwalk-2.0b1/PKG-INFO` & `hiperwalk-2.0b11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hiperwalk
-Version: 2.0b1
+Version: 2.0b11
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
```

