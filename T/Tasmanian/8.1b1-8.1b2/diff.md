# Comparing `tmp/Tasmanian-8.1b1.tar.gz` & `tmp/Tasmanian-8.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tasmanian-8.1b1.tar", last modified: Sun Mar 31 19:07:59 2024, max compression
+gzip compressed data, was "Tasmanian-8.1b2.tar", last modified: Thu Apr  4 00:34:31 2024, max compression
```

## Comparing `Tasmanian-8.1b1.tar` & `Tasmanian-8.1b2.tar`

### file list

```diff
@@ -1,333 +1,333 @@
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.629363 Tasmanian-8.1b1/Addons/
--rw-r--r--   0 miz      (15155) users      (100)     4885 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/CMakeLists.txt
--rw-r--r--   0 miz      (15155) users      (100)     3271 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/TasmanianAddons.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5279 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testAddons.cpp
--rw-r--r--   0 miz      (15155) users      (100)    16777 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testConstructSurrogate.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5197 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testCustomTabulated.hpp
--rw-r--r--   0 miz      (15155) users      (100)    11181 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testExoticQuadrature.hpp
--rw-r--r--   0 miz      (15155) users      (100)    14262 2024-03-21 14:58:59.000000 Tasmanian-8.1b1/Addons/testLoadUnstructured.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5770 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testMPI.cpp
--rw-r--r--   0 miz      (15155) users      (100)    13010 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testMPI.hpp
--rw-r--r--   0 miz      (15155) users      (100)     9052 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/testMPIDream.hpp
--rw-r--r--   0 miz      (15155) users      (100)     3061 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgAddonsCommon.hpp
--rw-r--r--   0 miz      (15155) users      (100)    15507 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgCConstructSurrogate.cpp
--rw-r--r--   0 miz      (15155) users      (100)     3429 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgCExoticQuadrature.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4217 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgCLoadNeededValues.cpp
--rw-r--r--   0 miz      (15155) users      (100)     2843 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgCLoadUnstructuredPoints.cpp
--rw-r--r--   0 miz      (15155) users      (100)    11725 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgCandidateManager.hpp
--rw-r--r--   0 miz      (15155) users      (100)    29345 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgConstructSurrogate.hpp
--rw-r--r--   0 miz      (15155) users      (100)    20151 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgExoticQuadrature.hpp
--rw-r--r--   0 miz      (15155) users      (100)    10163 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgLoadNeededValues.hpp
--rw-r--r--   0 miz      (15155) users      (100)    17488 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgLoadUnstructuredPoints.hpp
--rw-r--r--   0 miz      (15155) users      (100)    23836 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgMPIConstructGrid.hpp
--rw-r--r--   0 miz      (15155) users      (100)    11321 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgMPISampleDream.hpp
--rw-r--r--   0 miz      (15155) users      (100)     9514 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgMPIScatterDream.hpp
--rw-r--r--   0 miz      (15155) users      (100)    14622 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Addons/tsgMPIScatterGrid.hpp
--rw-r--r--   0 miz      (15155) users      (100)    13343 2024-03-21 18:19:22.000000 Tasmanian-8.1b1/CHANGELOG.md
--rw-r--r--   0 miz      (15155) users      (100)     9953 2024-02-22 19:21:36.000000 Tasmanian-8.1b1/CMakeLists.txt
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.629363 Tasmanian-8.1b1/Config/
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.629363 Tasmanian-8.1b1/Config/AltBuildSystems/
--rw-r--r--   0 miz      (15155) users      (100)     2526 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/AltBuildSystems/HeaderConvert.py
--rw-r--r--   0 miz      (15155) users      (100)     2757 2024-02-22 19:21:36.000000 Tasmanian-8.1b1/Config/AltBuildSystems/TasmanianConfig.hpp
--rw-r--r--   0 miz      (15155) users      (100)      555 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/AltBuildSystems/testConfigureData.py
--rw-r--r--   0 miz      (15155) users      (100)      496 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/AltBuildSystems/tsgGetPaths.m
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.633363 Tasmanian-8.1b1/Config/CMakeIncludes/
--rw-r--r--   0 miz      (15155) users      (100)     5004 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/CMakeLists.txt
--rw-r--r--   0 miz      (15155) users      (100)     2596 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/FindTasmanianDpcpp.cmake
--rw-r--r--   0 miz      (15155) users      (100)     4387 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/FindTasmanianMagma.cmake
--rw-r--r--   0 miz      (15155) users      (100)      304 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/PythonImportTest.py
--rw-r--r--   0 miz      (15155) users      (100)     4479 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/add_dependencies_target.cmake
--rw-r--r--   0 miz      (15155) users      (100)     4363 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/all_examples.cmake
--rw-r--r--   0 miz      (15155) users      (100)     4773 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/exports.cmake
--rw-r--r--   0 miz      (15155) users      (100)     9817 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/helper_macros.cmake
--rw-r--r--   0 miz      (15155) users      (100)     1542 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/master_targets.cmake
--rw-r--r--   0 miz      (15155) users      (100)    11270 2024-02-15 19:27:55.000000 Tasmanian-8.1b1/Config/CMakeIncludes/sanity_check_and_xsdk.cmake
--rw-r--r--   0 miz      (15155) users      (100)     2678 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeIncludes/setup_message.cmake
--rw-r--r--   0 miz      (15155) users      (100)     4318 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/CMakeLists.examples.cmake
--rw-r--r--   0 miz      (15155) users      (100)     2790 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/Tasmanian.h
--rw-r--r--   0 miz      (15155) users      (100)     3120 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/Tasmanian.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5596 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/TasmanianConfig.in.cmake
--rw-r--r--   0 miz      (15155) users      (100)     3324 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/TasmanianConfig.in.hpp
--rwxr-xr-x   0 miz      (15155) users      (100)      625 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/TasmanianENVsetup.in.sh
--rw-r--r--   0 miz      (15155) users      (100)      261 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/TasmanianMakefile.in
--rw-r--r--   0 miz      (15155) users      (100)    16889 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Config/magma_cmake.patch
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.633363 Tasmanian-8.1b1/DREAM/
--rw-r--r--   0 miz      (15155) users      (100)     5216 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/CMakeLists.txt
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.637363 Tasmanian-8.1b1/DREAM/Examples/
--rw-r--r--   0 miz      (15155) users      (100)     1541 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4962 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream_01.cpp
--rw-r--r--   0 miz      (15155) users      (100)     7815 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream_02.cpp
--rw-r--r--   0 miz      (15155) users      (100)     7745 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream_03.cpp
--rw-r--r--   0 miz      (15155) users      (100)     8075 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream_04.cpp
--rw-r--r--   0 miz      (15155) users      (100)    10993 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_dream_05.cpp
--rw-r--r--   0 miz      (15155) users      (100)     1049 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_optimization.cpp
--rw-r--r--   0 miz      (15155) users      (100)     5987 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_optimization_01.cpp
--rw-r--r--   0 miz      (15155) users      (100)     6404 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Examples/example_optimization_02.cpp
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.637363 Tasmanian-8.1b1/DREAM/Optimization/
--rw-r--r--   0 miz      (15155) users      (100)     4235 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/TasmanianOptimization.hpp
--rw-r--r--   0 miz      (15155) users      (100)    15645 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/TasmanianOptimizationWrapC.cpp
--rw-r--r--   0 miz      (15155) users      (100)    16618 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tasdreamOptimizationTests.cpp
--rw-r--r--   0 miz      (15155) users      (100)     6545 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tsgGradientDescent.cpp
--rw-r--r--   0 miz      (15155) users      (100)    11249 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tsgGradientDescent.hpp
--rw-r--r--   0 miz      (15155) users      (100)     9080 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tsgOptimizationUtils.hpp
--rw-r--r--   0 miz      (15155) users      (100)    12670 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tsgParticleSwarm.cpp
--rw-r--r--   0 miz      (15155) users      (100)    16669 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/Optimization/tsgParticleSwarm.hpp
--rw-r--r--   0 miz      (15155) users      (100)     4272 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/TasmanianDREAM.hpp
--rw-r--r--   0 miz      (15155) users      (100)     4551 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/dreamtest_main.cpp
--rw-r--r--   0 miz      (15155) users      (100)    26656 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tasdreamExternalTests.cpp
--rw-r--r--   0 miz      (15155) users      (100)    10668 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tasdreamExternalTests.hpp
--rw-r--r--   0 miz      (15155) users      (100)     6470 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamCorePDF.hpp
--rw-r--r--   0 miz      (15155) users      (100)     7814 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamCoreRandom.hpp
--rw-r--r--   0 miz      (15155) users      (100)     6998 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamEnumerates.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5640 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamLikelihoodCore.hpp
--rw-r--r--   0 miz      (15155) users      (100)     7183 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamLikelyGaussian.cpp
--rw-r--r--   0 miz      (15155) users      (100)    11026 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamLikelyGaussian.hpp
--rw-r--r--   0 miz      (15155) users      (100)    28502 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamSample.hpp
--rw-r--r--   0 miz      (15155) users      (100)    11318 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamSampleWrapC.cpp
--rw-r--r--   0 miz      (15155) users      (100)     8750 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamState.cpp
--rw-r--r--   0 miz      (15155) users      (100)    10549 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/DREAM/tsgDreamState.hpp
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.637363 Tasmanian-8.1b1/Doxygen/
--rw-r--r--   0 miz      (15155) users      (100)     8809 2023-10-17 16:07:31.000000 Tasmanian-8.1b1/Doxygen/CMakeLists.txt
--rw-r--r--   0 miz      (15155) users      (100)     1201 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/Contributors.md
--rw-r--r--   0 miz      (15155) users      (100)     4114 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/CustomRuleFileFormat.md
--rw-r--r--   0 miz      (15155) users      (100)      557 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/DevNotes.md
--rw-r--r--   0 miz      (15155) users      (100)    21998 2024-03-21 18:19:22.000000 Tasmanian-8.1b1/Doxygen/Installation.md
--rw-r--r--   0 miz      (15155) users      (100)     8714 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/InterfaceCLI.md
--rw-r--r--   0 miz      (15155) users      (100)     7933 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/InterfaceFortran2003.md
--rw-r--r--   0 miz      (15155) users      (100)     3515 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/InterfaceLibEnsemble.md
--rw-r--r--   0 miz      (15155) users      (100)     9902 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/InterfaceMATLAB.md
--rw-r--r--   0 miz      (15155) users      (100)     5715 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/InterfacePython.md
--rw-r--r--   0 miz      (15155) users      (100)      738 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/footer.html
--rw-r--r--   0 miz      (15155) users      (100)     2285 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/header.html
--rw-r--r--   0 miz      (15155) users      (100)     7981 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Doxygen/tasmanian.css
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.637363 Tasmanian-8.1b1/InterfaceFortran/
--rw-r--r--   0 miz      (15155) users      (100)     2952 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/CMakeLists.txt
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.637363 Tasmanian-8.1b1/InterfaceFortran/Examples/
--rw-r--r--   0 miz      (15155) users      (100)    35422 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/Examples/example_sparse_grids.f90
--rw-r--r--   0 miz      (15155) users      (100)    33420 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/TasmanianSG.f90
--rw-r--r--   0 miz      (15155) users      (100)    61071 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/fortester.f90
--rw-r--r--   0 miz      (15155) users      (100)     4364 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/mpitester.f90
--rw-r--r--   0 miz      (15155) users      (100)    14518 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/tsgC2Fortran.cpp
--rw-r--r--   0 miz      (15155) users      (100)     3869 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceFortran/tsgC2FortranBridge.f90
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.645363 Tasmanian-8.1b1/InterfaceMATLAB/
--rw-r--r--   0 miz      (15155) users      (100)     6104 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/CMakeLists.txt
--rw-r--r--   0 miz      (15155) users      (100)      793 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgCancelRefine.m
--rw-r--r--   0 miz      (15155) users      (100)     2525 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgCleanTempFiles.m
--rw-r--r--   0 miz      (15155) users      (100)     1182 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgCopyGrid.m
--rw-r--r--   0 miz      (15155) users      (100)    46014 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgCoreTests.m
--rw-r--r--   0 miz      (15155) users      (100)      499 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgDeleteGrid.m
--rw-r--r--   0 miz      (15155) users      (100)      538 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgDeleteGridByName.m
--rw-r--r--   0 miz      (15155) users      (100)     2159 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgDifferentiate.m
--rw-r--r--   0 miz      (15155) users      (100)     1598 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgEstimateAnisotropicCoefficients.m
--rw-r--r--   0 miz      (15155) users      (100)     1934 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgEvaluate.m
--rw-r--r--   0 miz      (15155) users      (100)     2758 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgEvaluateHierarchy.m
--rw-r--r--   0 miz      (15155) users      (100)    23609 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgExample.m
--rw-r--r--   0 miz      (15155) users      (100)     3964 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetCandidateConstructionAnisotropic.m
--rw-r--r--   0 miz      (15155) users      (100)     4292 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetCandidateConstructionSurplus.m
--rw-r--r--   0 miz      (15155) users      (100)     2240 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetDifferentiationWeights.m
--rw-r--r--   0 miz      (15155) users      (100)     1197 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetHCoefficients.m
--rw-r--r--   0 miz      (15155) users      (100)      994 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetHSupport.m
--rw-r--r--   0 miz      (15155) users      (100)     1546 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetInterpolationWeights.m
--rw-r--r--   0 miz      (15155) users      (100)     1020 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetNeededIndexes.m
--rw-r--r--   0 miz      (15155) users      (100)     1138 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetNeededPoints.m
--rw-r--r--   0 miz      (15155) users      (100)      391 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPaths.build.m
--rw-r--r--   0 miz      (15155) users      (100)      391 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPaths.install.m
--rw-r--r--   0 miz      (15155) users      (100)      942 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPoints.m
--rw-r--r--   0 miz      (15155) users      (100)     1020 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPointsIndexes.m
--rw-r--r--   0 miz      (15155) users      (100)     1395 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPolynomialSpaces.m
--rw-r--r--   0 miz      (15155) users      (100)     1061 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgGetQuadrature.m
--rw-r--r--   0 miz      (15155) users      (100)      938 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgIntegrate.m
--rw-r--r--   0 miz      (15155) users      (100)      567 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgListGridsByName.m
--rw-r--r--   0 miz      (15155) users      (100)     1513 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadConstructedPoints.m
--rw-r--r--   0 miz      (15155) users      (100)     1870 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadGridFromFile.m
--rw-r--r--   0 miz      (15155) users      (100)     1458 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadHCoefficients.m
--rw-r--r--   0 miz      (15155) users      (100)     1199 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadValues.m
--rw-r--r--   0 miz      (15155) users      (100)     2175 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeExoticQuadrature.m
--rw-r--r--   0 miz      (15155) users      (100)     1123 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeFilenames.m
--rw-r--r--   0 miz      (15155) users      (100)     8047 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeFourier.m
--rw-r--r--   0 miz      (15155) users      (100)    11945 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeGlobal.m
--rw-r--r--   0 miz      (15155) users      (100)      361 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeGridFilename.m
--rw-r--r--   0 miz      (15155) users      (100)     6027 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeLocalPolynomial.m
--rw-r--r--   0 miz      (15155) users      (100)    12020 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeQuadrature.m
--rw-r--r--   0 miz      (15155) users      (100)     7277 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeSequence.m
--rw-r--r--   0 miz      (15155) users      (100)     5659 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeWavelet.m
--rw-r--r--   0 miz      (15155) users      (100)      772 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgMergeRefine.m
--rw-r--r--   0 miz      (15155) users      (100)      760 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgPlotPoints2D.m
--rw-r--r--   0 miz      (15155) users      (100)     1378 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgReadCustomRuleFile.m
--rw-r--r--   0 miz      (15155) users      (100)      872 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgReadMatrix.m
--rw-r--r--   0 miz      (15155) users      (100)     3202 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgRefineAnisotropic.m
--rw-r--r--   0 miz      (15155) users      (100)     4156 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgRefineSurplus.m
--rw-r--r--   0 miz      (15155) users      (100)     1801 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgReloadGrid.m
--rw-r--r--   0 miz      (15155) users      (100)      660 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgSummary.m
--rw-r--r--   0 miz      (15155) users      (100)      891 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgUsingConstruction.m
--rw-r--r--   0 miz      (15155) users      (100)     2711 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgWriteCustomRuleFile.m
--rw-r--r--   0 miz      (15155) users      (100)      991 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceMATLAB/tsgWriteMatrix.m
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.653363 Tasmanian-8.1b1/InterfacePython/
--rw-r--r--   0 miz      (15155) users      (100)    15865 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/CMakeLists.txt
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.653363 Tasmanian-8.1b1/InterfacePython/PipInstaller/
--rw-r--r--   0 miz      (15155) users      (100)      430 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/PipInstaller/MANIFEST.in
--rw-r--r--   0 miz      (15155) users      (100)     4326 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/PipInstaller/README.md
--rw-r--r--   0 miz      (15155) users      (100)      472 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/PipInstaller/make_tarball.sh
--rw-r--r--   0 miz      (15155) users      (100)       87 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/PipInstaller/pyproject.toml
--rw-r--r--   0 miz      (15155) users      (100)     3106 2024-03-31 19:07:52.000000 Tasmanian-8.1b1/InterfacePython/PipInstaller/setup.py
--rw-r--r--   0 miz      (15155) users      (100)     3874 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/Tasmanian.py
--rw-r--r--   0 miz      (15155) users      (100)    23721 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianAddons.py
--rw-r--r--   0 miz      (15155) users      (100)     4289 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/TasmanianConfig.in.py
--rw-r--r--   0 miz      (15155) users      (100)     2803 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/TasmanianDREAM.py
--rw-r--r--   0 miz      (15155) users      (100)     6636 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianDreamLikely.py
--rw-r--r--   0 miz      (15155) users      (100)    29258 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianDreamSampler.py
--rw-r--r--   0 miz      (15155) users      (100)     8090 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianDreamState.py
--rw-r--r--   0 miz      (15155) users      (100)    17345 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianGradientDescent.py
--rw-r--r--   0 miz      (15155) users      (100)     2553 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/TasmanianOPT.py
--rw-r--r--   0 miz      (15155) users      (100)    17715 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/TasmanianParticleSwarm.py
--rw-r--r--   0 miz      (15155) users      (100)   124558 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/TasmanianSG.py
--rwxr-xr-x   0 miz      (15155) users      (100)     3393 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream.in.py
--rw-r--r--   0 miz      (15155) users      (100)     5050 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream_01.py
--rw-r--r--   0 miz      (15155) users      (100)     6783 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream_02.py
--rw-r--r--   0 miz      (15155) users      (100)     6477 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream_03.py
--rw-r--r--   0 miz      (15155) users      (100)     6752 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream_04.py
--rw-r--r--   0 miz      (15155) users      (100)     7124 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_dream_05.py
--rwxr-xr-x   0 miz      (15155) users      (100)     3177 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_optimization.in.py
--rw-r--r--   0 miz      (15155) users      (100)     6127 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_optimization_01.py
--rw-r--r--   0 miz      (15155) users      (100)     7283 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_optimization_02.py
--rwxr-xr-x   0 miz      (15155) users      (100)     3911 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids.in.py
--rw-r--r--   0 miz      (15155) users      (100)     4285 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_01.py
--rw-r--r--   0 miz      (15155) users      (100)     4710 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_02.py
--rw-r--r--   0 miz      (15155) users      (100)     4602 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_03.py
--rw-r--r--   0 miz      (15155) users      (100)     4070 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_04.py
--rw-r--r--   0 miz      (15155) users      (100)     6738 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_05.py
--rw-r--r--   0 miz      (15155) users      (100)     4622 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_06.py
--rw-r--r--   0 miz      (15155) users      (100)     3084 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_07.py
--rw-r--r--   0 miz      (15155) users      (100)     5550 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_08.py
--rw-r--r--   0 miz      (15155) users      (100)     5980 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_09.py
--rw-r--r--   0 miz      (15155) users      (100)     4882 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_10.py
--rw-r--r--   0 miz      (15155) users      (100)     4859 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/example_sparse_grids_11.py
--rwxr-xr-x   0 miz      (15155) users      (100)      796 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/sandbox.py
--rw-r--r--   0 miz      (15155) users      (100)     7102 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/testAcceleration.py
--rw-r--r--   0 miz      (15155) users      (100)     9604 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testAddons.py
--rw-r--r--   0 miz      (15155) users      (100)    21512 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testBasicIO.py
--rw-r--r--   0 miz      (15155) users      (100)     9245 2024-03-31 18:45:29.000000 Tasmanian-8.1b1/InterfacePython/testCommon.py
--rw-r--r--   0 miz      (15155) users      (100)      801 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testConfigureData.in.py
--rw-r--r--   0 miz      (15155) users      (100)     5264 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testDream.py
--rw-r--r--   0 miz      (15155) users      (100)    34228 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testExceptions.py
--rw-r--r--   0 miz      (15155) users      (100)    20655 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testMakeUpdate.py
--rw-r--r--   0 miz      (15155) users      (100)     8216 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testMisc.py
--rw-r--r--   0 miz      (15155) users      (100)     8528 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testOptimization.py
--rw-r--r--   0 miz      (15155) users      (100)    12423 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testRefinement.py
--rwxr-xr-x   0 miz      (15155) users      (100)     2407 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testTSG.py
--rw-r--r--   0 miz      (15155) users      (100)    12297 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfacePython/testUnstructuredData.py
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.653363 Tasmanian-8.1b1/InterfaceTPL/
--rw-r--r--   0 miz      (15155) users      (100)     4009 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgBlasNull.hpp
--rw-r--r--   0 miz      (15155) users      (100)    22145 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgBlasWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)    34665 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgCudaWrappers.cpp
--rw-r--r--   0 miz      (15155) users      (100)    12174 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgCudaWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)    18800 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgDpcppWrappers.cpp
--rw-r--r--   0 miz      (15155) users      (100)     5953 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgDpcppWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)    13496 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgGpuNull.cpp
--rw-r--r--   0 miz      (15155) users      (100)     7511 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgGpuWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)    22391 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgHipWrappers.cpp
--rw-r--r--   0 miz      (15155) users      (100)     8686 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgHipWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)     8657 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgMagmaWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)     3410 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/InterfaceTPL/tsgTPLWrappers.hpp
--rw-r--r--   0 miz      (15155) users      (100)     2227 2021-05-26 18:15:42.000000 Tasmanian-8.1b1/LICENSE
--rw-r--r--   0 miz      (15155) users      (100)     5631 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/PKG-INFO
--rw-r--r--   0 miz      (15155) users      (100)     5256 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/README.md
--rw-r--r--   0 miz      (15155) users      (100)       81 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SUPPORT.md
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/SparseGrids/
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/SparseGrids/Benchmarks/
--rw-r--r--   0 miz      (15155) users      (100)     8749 2024-03-21 14:34:22.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchCommon.hpp
--rw-r--r--   0 miz      (15155) users      (100)     1718 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchDifferentiate.hpp
--rw-r--r--   0 miz      (15155) users      (100)     2145 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchEvaluate.hpp
--rw-r--r--   0 miz      (15155) users      (100)     1595 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchInterpolationWeights.hpp
--rw-r--r--   0 miz      (15155) users      (100)     1781 2024-02-22 16:43:25.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchLoadNeeded.hpp
--rw-r--r--   0 miz      (15155) users      (100)     1445 2024-02-20 21:15:48.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchMakeGrid.hpp
--rw-r--r--   0 miz      (15155) users      (100)     1883 2024-03-21 14:34:22.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/benchRefine.hpp
--rw-r--r--   0 miz      (15155) users      (100)     8737 2024-03-21 14:34:22.000000 Tasmanian-8.1b1/SparseGrids/Benchmarks/bench_main.cpp
--rw-r--r--   0 miz      (15155) users      (100)     9872 2024-03-21 14:34:22.000000 Tasmanian-8.1b1/SparseGrids/CMakeLists.txt
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/SparseGrids/Examples/
--rw-r--r--   0 miz      (15155) users      (100)     3957 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids.cpp
--rw-r--r--   0 miz      (15155) users      (100)     2718 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_01.cpp
--rw-r--r--   0 miz      (15155) users      (100)     3158 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_02.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4599 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_03.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4081 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_04.cpp
--rw-r--r--   0 miz      (15155) users      (100)     6147 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_05.cpp
--rw-r--r--   0 miz      (15155) users      (100)     5651 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_06.cpp
--rw-r--r--   0 miz      (15155) users      (100)     6219 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_07.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4848 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_08.cpp
--rw-r--r--   0 miz      (15155) users      (100)     5882 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_09.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4591 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_10.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4781 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_11.cpp
--rw-r--r--   0 miz      (15155) users      (100)    55377 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/GaussPattersonRule.table
--rw-r--r--   0 miz      (15155) users      (100)    95905 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.cpp
--rw-r--r--   0 miz      (15155) users      (100)    10330 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.h
--rw-r--r--   0 miz      (15155) users      (100)   126030 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.hpp
--rw-r--r--   0 miz      (15155) users      (100)    33108 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/TasmanianSparseGridWrapC.cpp
--rw-r--r--   0 miz      (15155) users      (100)     5770 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestCLICommon.hpp
--rw-r--r--   0 miz      (15155) users      (100)   130177 2024-03-31 18:45:20.000000 Tasmanian-8.1b1/SparseGrids/gridtestExternalTests.cpp
--rw-r--r--   0 miz      (15155) users      (100)     8095 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestExternalTests.hpp
--rw-r--r--   0 miz      (15155) users      (100)    27756 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestTestFunctions.cpp
--rw-r--r--   0 miz      (15155) users      (100)    14436 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestTestFunctions.hpp
--rw-r--r--   0 miz      (15155) users      (100)    10155 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestTestHelpers.hpp
--rw-r--r--   0 miz      (15155) users      (100)     8895 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestTestInterfaceC.cpp
--rw-r--r--   0 miz      (15155) users      (100)    36788 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestUnitTests.cpp
--rw-r--r--   0 miz      (15155) users      (100)     3513 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtestUnitTests.hpp
--rw-r--r--   0 miz      (15155) users      (100)     4088 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/gridtest_main.cpp
--rw-r--r--   0 miz      (15155) users      (100)     9141 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgAcceleratedDataStructures.cpp
--rw-r--r--   0 miz      (15155) users      (100)    40354 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgAcceleratedDataStructures.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5693 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgAcceleratedHandles.hpp
--rw-r--r--   0 miz      (15155) users      (100)     9942 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCacheLagrange.hpp
--rw-r--r--   0 miz      (15155) users      (100)    29251 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCoreOneDimensional.cpp
--rw-r--r--   0 miz      (15155) users      (100)    14976 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCoreOneDimensional.hpp
--rw-r--r--   0 miz      (15155) users      (100)    29102 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCudaBasisEvaluations.hpp
--rw-r--r--   0 miz      (15155) users      (100)    24125 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCudaKernels.cu
--rw-r--r--   0 miz      (15155) users      (100)    13839 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCudaLinearAlgebra.hpp
--rw-r--r--   0 miz      (15155) users      (100)     6463 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgCudaLoadStructures.hpp
--rw-r--r--   0 miz      (15155) users      (100)     9707 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgDConstructGridGlobal.cpp
--rw-r--r--   0 miz      (15155) users      (100)    15450 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgDConstructGridGlobal.hpp
--rw-r--r--   0 miz      (15155) users      (100)    20939 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgDpcppBasisEvaluations.hpp
--rw-r--r--   0 miz      (15155) users      (100)    18700 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgDpcppKernels.cpp
--rw-r--r--   0 miz      (15155) users      (100)    33380 2024-02-22 19:21:36.000000 Tasmanian-8.1b1/SparseGrids/tsgEnumerates.hpp
--rw-r--r--   0 miz      (15155) users      (100)     7785 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridCore.hpp
--rw-r--r--   0 miz      (15155) users      (100)    50202 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridFourier.cpp
--rw-r--r--   0 miz      (15155) users      (100)    11656 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridFourier.hpp
--rw-r--r--   0 miz      (15155) users      (100)    41549 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridGlobal.cpp
--rw-r--r--   0 miz      (15155) users      (100)    11771 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridGlobal.hpp
--rw-r--r--   0 miz      (15155) users      (100)    76290 2024-03-31 18:45:20.000000 Tasmanian-8.1b1/SparseGrids/tsgGridLocalPolynomial.cpp
--rw-r--r--   0 miz      (15155) users      (100)    22424 2024-03-31 18:45:20.000000 Tasmanian-8.1b1/SparseGrids/tsgGridLocalPolynomial.hpp
--rw-r--r--   0 miz      (15155) users      (100)    40023 2024-02-15 21:55:13.000000 Tasmanian-8.1b1/SparseGrids/tsgGridSequence.cpp
--rw-r--r--   0 miz      (15155) users      (100)    12039 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridSequence.hpp
--rw-r--r--   0 miz      (15155) users      (100)    45354 2024-03-21 18:32:24.000000 Tasmanian-8.1b1/SparseGrids/tsgGridWavelet.cpp
--rw-r--r--   0 miz      (15155) users      (100)     9275 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgGridWavelet.hpp
--rw-r--r--   0 miz      (15155) users      (100)    50527 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgHardCodedTabulatedRules.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4544 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgHardCodedTabulatedRules.hpp
--rw-r--r--   0 miz      (15155) users      (100)    13069 2024-02-22 16:49:04.000000 Tasmanian-8.1b1/SparseGrids/tsgHierarchyManipulator.cpp
--rw-r--r--   0 miz      (15155) users      (100)    13517 2024-03-21 14:58:59.000000 Tasmanian-8.1b1/SparseGrids/tsgHierarchyManipulator.hpp
--rw-r--r--   0 miz      (15155) users      (100)    22477 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgHipKernels.hip.cpp
--rw-r--r--   0 miz      (15155) users      (100)    15963 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgIOHelpers.hpp
--rw-r--r--   0 miz      (15155) users      (100)    28104 2024-03-21 18:32:24.000000 Tasmanian-8.1b1/SparseGrids/tsgIndexManipulator.cpp
--rw-r--r--   0 miz      (15155) users      (100)    26026 2024-02-15 21:55:13.000000 Tasmanian-8.1b1/SparseGrids/tsgIndexManipulator.hpp
--rw-r--r--   0 miz      (15155) users      (100)    11776 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgIndexSets.cpp
--rw-r--r--   0 miz      (15155) users      (100)    20915 2024-03-21 14:58:59.000000 Tasmanian-8.1b1/SparseGrids/tsgIndexSets.hpp
--rw-r--r--   0 miz      (15155) users      (100)    36519 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgLinearSolvers.cpp
--rw-r--r--   0 miz      (15155) users      (100)    12646 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgLinearSolvers.hpp
--rw-r--r--   0 miz      (15155) users      (100)     5320 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgMathUtils.hpp
--rw-r--r--   0 miz      (15155) users      (100)    17803 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgOneDimensionalWrapper.hpp
--rw-r--r--   0 miz      (15155) users      (100)    39690 2024-03-31 18:45:20.000000 Tasmanian-8.1b1/SparseGrids/tsgRuleLocalPolynomial.hpp
--rw-r--r--   0 miz      (15155) users      (100)    23153 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgRuleWavelet.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4997 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgRuleWavelet.hpp
--rw-r--r--   0 miz      (15155) users      (100)    23040 2024-03-21 14:58:59.000000 Tasmanian-8.1b1/SparseGrids/tsgSequenceOptimizer.cpp
--rw-r--r--   0 miz      (15155) users      (100)     4675 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgSequenceOptimizer.hpp
--rw-r--r--   0 miz      (15155) users      (100)     6432 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/SparseGrids/tsgUtils.hpp
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/Tasgrid/
--rw-r--r--   0 miz      (15155) users      (100)     2725 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Tasgrid/CMakeLists.txt
--rw-r--r--   0 miz      (15155) users      (100)     5469 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Tasgrid/tasgridLogs.in.hpp
--rw-r--r--   0 miz      (15155) users      (100)    44908 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Tasgrid/tasgridWrapper.cpp
--rw-r--r--   0 miz      (15155) users      (100)     8534 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Tasgrid/tasgridWrapper.hpp
--rw-r--r--   0 miz      (15155) users      (100)    57027 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Tasgrid/tasgrid_main.cpp
-drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-03-31 19:07:59.661363 Tasmanian-8.1b1/Testing/
--rw-r--r--   0 miz      (15155) users      (100)     1666 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Testing/CMakeLists.test.cmake
--rw-r--r--   0 miz      (15155) users      (100)     3171 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Testing/tasmanian_version.cpp
--rwxr-xr-x   0 miz      (15155) users      (100)      758 2023-10-16 21:44:16.000000 Tasmanian-8.1b1/Testing/test_post_install.in.sh
--rw-r--r--   0 miz      (15155) users      (100)       87 2024-03-31 19:07:59.000000 Tasmanian-8.1b1/pyproject.toml
--rw-r--r--   0 miz      (15155) users      (100)     3106 2024-03-31 19:07:59.000000 Tasmanian-8.1b1/setup.py
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.253499 Tasmanian-8.1b2/Addons/
+-rw-r--r--   0 miz      (15155) users      (100)     4885 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/CMakeLists.txt
+-rw-r--r--   0 miz      (15155) users      (100)     3271 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/TasmanianAddons.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5279 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testAddons.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    16777 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testConstructSurrogate.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5197 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testCustomTabulated.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    11181 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testExoticQuadrature.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    14262 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testLoadUnstructured.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5770 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testMPI.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    13010 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testMPI.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     9052 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/testMPIDream.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     3061 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgAddonsCommon.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    15507 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgCConstructSurrogate.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     3429 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgCExoticQuadrature.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4217 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgCLoadNeededValues.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     2843 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgCLoadUnstructuredPoints.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    11725 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgCandidateManager.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    29345 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgConstructSurrogate.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    20151 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgExoticQuadrature.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    10163 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgLoadNeededValues.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    17488 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgLoadUnstructuredPoints.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    23836 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgMPIConstructGrid.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    11321 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgMPISampleDream.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     9514 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgMPIScatterDream.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    14622 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Addons/tsgMPIScatterGrid.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    13461 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/CHANGELOG.md
+-rw-r--r--   0 miz      (15155) users      (100)     9953 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/CMakeLists.txt
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.257499 Tasmanian-8.1b2/Config/
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.257499 Tasmanian-8.1b2/Config/AltBuildSystems/
+-rw-r--r--   0 miz      (15155) users      (100)     2526 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/AltBuildSystems/HeaderConvert.py
+-rw-r--r--   0 miz      (15155) users      (100)     2757 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/AltBuildSystems/TasmanianConfig.hpp
+-rw-r--r--   0 miz      (15155) users      (100)      555 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/AltBuildSystems/testConfigureData.py
+-rw-r--r--   0 miz      (15155) users      (100)      496 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/AltBuildSystems/tsgGetPaths.m
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.257499 Tasmanian-8.1b2/Config/CMakeIncludes/
+-rw-r--r--   0 miz      (15155) users      (100)     5004 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/CMakeLists.txt
+-rw-r--r--   0 miz      (15155) users      (100)     2596 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/FindTasmanianDpcpp.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     4387 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/FindTasmanianMagma.cmake
+-rw-r--r--   0 miz      (15155) users      (100)      304 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/PythonImportTest.py
+-rw-r--r--   0 miz      (15155) users      (100)     4479 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/add_dependencies_target.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     4363 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/all_examples.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     4773 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/exports.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     9817 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/helper_macros.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     1542 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/master_targets.cmake
+-rw-r--r--   0 miz      (15155) users      (100)    11270 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/sanity_check_and_xsdk.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     2678 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeIncludes/setup_message.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     4318 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/CMakeLists.examples.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     2790 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/Tasmanian.h
+-rw-r--r--   0 miz      (15155) users      (100)     3120 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/Tasmanian.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5596 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/TasmanianConfig.in.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     3324 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/TasmanianConfig.in.hpp
+-rwxr-xr-x   0 miz      (15155) users      (100)      625 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/TasmanianENVsetup.in.sh
+-rw-r--r--   0 miz      (15155) users      (100)      261 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/TasmanianMakefile.in
+-rw-r--r--   0 miz      (15155) users      (100)    16889 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Config/magma_cmake.patch
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.257499 Tasmanian-8.1b2/DREAM/
+-rw-r--r--   0 miz      (15155) users      (100)     5216 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/CMakeLists.txt
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.261499 Tasmanian-8.1b2/DREAM/Examples/
+-rw-r--r--   0 miz      (15155) users      (100)     1541 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4962 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream_01.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     7815 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream_02.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     7745 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream_03.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     8075 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream_04.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    10993 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_dream_05.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     1049 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_optimization.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     5987 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_optimization_01.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     6404 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Examples/example_optimization_02.cpp
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.261499 Tasmanian-8.1b2/DREAM/Optimization/
+-rw-r--r--   0 miz      (15155) users      (100)     4235 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/TasmanianOptimization.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    15645 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/TasmanianOptimizationWrapC.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    16618 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tasdreamOptimizationTests.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     6545 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tsgGradientDescent.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    11249 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tsgGradientDescent.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     9080 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tsgOptimizationUtils.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    12670 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tsgParticleSwarm.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    16669 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/Optimization/tsgParticleSwarm.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     4272 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/TasmanianDREAM.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     4551 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/dreamtest_main.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    26656 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tasdreamExternalTests.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    10668 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tasdreamExternalTests.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     6470 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamCorePDF.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     7814 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamCoreRandom.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     6998 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamEnumerates.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5640 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamLikelihoodCore.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     7183 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamLikelyGaussian.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    11026 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamLikelyGaussian.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    28502 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamSample.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    11318 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamSampleWrapC.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     8750 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamState.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    10549 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/DREAM/tsgDreamState.hpp
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.261499 Tasmanian-8.1b2/Doxygen/
+-rw-r--r--   0 miz      (15155) users      (100)     8809 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/CMakeLists.txt
+-rw-r--r--   0 miz      (15155) users      (100)     1201 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/Contributors.md
+-rw-r--r--   0 miz      (15155) users      (100)     4114 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/CustomRuleFileFormat.md
+-rw-r--r--   0 miz      (15155) users      (100)      557 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/DevNotes.md
+-rw-r--r--   0 miz      (15155) users      (100)    22656 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/Installation.md
+-rw-r--r--   0 miz      (15155) users      (100)     8714 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/InterfaceCLI.md
+-rw-r--r--   0 miz      (15155) users      (100)     7933 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/InterfaceFortran2003.md
+-rw-r--r--   0 miz      (15155) users      (100)     3515 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/InterfaceLibEnsemble.md
+-rw-r--r--   0 miz      (15155) users      (100)     9902 2024-04-04 00:31:35.000000 Tasmanian-8.1b2/Doxygen/InterfaceMATLAB.md
+-rw-r--r--   0 miz      (15155) users      (100)     5715 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Doxygen/InterfacePython.md
+-rw-r--r--   0 miz      (15155) users      (100)      738 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Doxygen/footer.html
+-rw-r--r--   0 miz      (15155) users      (100)     2285 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Doxygen/header.html
+-rw-r--r--   0 miz      (15155) users      (100)     7981 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Doxygen/tasmanian.css
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.261499 Tasmanian-8.1b2/InterfaceFortran/
+-rw-r--r--   0 miz      (15155) users      (100)     2952 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/CMakeLists.txt
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.261499 Tasmanian-8.1b2/InterfaceFortran/Examples/
+-rw-r--r--   0 miz      (15155) users      (100)    35422 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/Examples/example_sparse_grids.f90
+-rw-r--r--   0 miz      (15155) users      (100)    33420 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/TasmanianSG.f90
+-rw-r--r--   0 miz      (15155) users      (100)    61071 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/fortester.f90
+-rw-r--r--   0 miz      (15155) users      (100)     4364 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/mpitester.f90
+-rw-r--r--   0 miz      (15155) users      (100)    14518 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/tsgC2Fortran.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     3869 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceFortran/tsgC2FortranBridge.f90
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.269499 Tasmanian-8.1b2/InterfaceMATLAB/
+-rw-r--r--   0 miz      (15155) users      (100)     6104 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/CMakeLists.txt
+-rw-r--r--   0 miz      (15155) users      (100)      793 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgCancelRefine.m
+-rw-r--r--   0 miz      (15155) users      (100)     2525 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgCleanTempFiles.m
+-rw-r--r--   0 miz      (15155) users      (100)     1182 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgCopyGrid.m
+-rw-r--r--   0 miz      (15155) users      (100)    46014 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgCoreTests.m
+-rw-r--r--   0 miz      (15155) users      (100)      499 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgDeleteGrid.m
+-rw-r--r--   0 miz      (15155) users      (100)      538 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgDeleteGridByName.m
+-rw-r--r--   0 miz      (15155) users      (100)     2159 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgDifferentiate.m
+-rw-r--r--   0 miz      (15155) users      (100)     1598 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgEstimateAnisotropicCoefficients.m
+-rw-r--r--   0 miz      (15155) users      (100)     1934 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgEvaluate.m
+-rw-r--r--   0 miz      (15155) users      (100)     2758 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgEvaluateHierarchy.m
+-rw-r--r--   0 miz      (15155) users      (100)    23609 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgExample.m
+-rw-r--r--   0 miz      (15155) users      (100)     3964 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetCandidateConstructionAnisotropic.m
+-rw-r--r--   0 miz      (15155) users      (100)     4292 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetCandidateConstructionSurplus.m
+-rw-r--r--   0 miz      (15155) users      (100)     2240 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetDifferentiationWeights.m
+-rw-r--r--   0 miz      (15155) users      (100)     1197 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetHCoefficients.m
+-rw-r--r--   0 miz      (15155) users      (100)      994 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetHSupport.m
+-rw-r--r--   0 miz      (15155) users      (100)     1546 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetInterpolationWeights.m
+-rw-r--r--   0 miz      (15155) users      (100)     1020 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetNeededIndexes.m
+-rw-r--r--   0 miz      (15155) users      (100)     1138 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetNeededPoints.m
+-rw-r--r--   0 miz      (15155) users      (100)      391 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPaths.build.m
+-rw-r--r--   0 miz      (15155) users      (100)      391 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPaths.install.m
+-rw-r--r--   0 miz      (15155) users      (100)      942 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPoints.m
+-rw-r--r--   0 miz      (15155) users      (100)     1020 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPointsIndexes.m
+-rw-r--r--   0 miz      (15155) users      (100)     1395 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPolynomialSpaces.m
+-rw-r--r--   0 miz      (15155) users      (100)     1061 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgGetQuadrature.m
+-rw-r--r--   0 miz      (15155) users      (100)      938 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgIntegrate.m
+-rw-r--r--   0 miz      (15155) users      (100)      567 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgListGridsByName.m
+-rw-r--r--   0 miz      (15155) users      (100)     1513 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadConstructedPoints.m
+-rw-r--r--   0 miz      (15155) users      (100)     1870 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadGridFromFile.m
+-rw-r--r--   0 miz      (15155) users      (100)     1458 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadHCoefficients.m
+-rw-r--r--   0 miz      (15155) users      (100)     1199 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadValues.m
+-rw-r--r--   0 miz      (15155) users      (100)     2175 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeExoticQuadrature.m
+-rw-r--r--   0 miz      (15155) users      (100)     1123 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeFilenames.m
+-rw-r--r--   0 miz      (15155) users      (100)     8047 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeFourier.m
+-rw-r--r--   0 miz      (15155) users      (100)    11945 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeGlobal.m
+-rw-r--r--   0 miz      (15155) users      (100)      361 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeGridFilename.m
+-rw-r--r--   0 miz      (15155) users      (100)     6027 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeLocalPolynomial.m
+-rw-r--r--   0 miz      (15155) users      (100)    12020 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeQuadrature.m
+-rw-r--r--   0 miz      (15155) users      (100)     7277 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeSequence.m
+-rw-r--r--   0 miz      (15155) users      (100)     5659 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeWavelet.m
+-rw-r--r--   0 miz      (15155) users      (100)      772 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgMergeRefine.m
+-rw-r--r--   0 miz      (15155) users      (100)      760 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgPlotPoints2D.m
+-rw-r--r--   0 miz      (15155) users      (100)     1378 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgReadCustomRuleFile.m
+-rw-r--r--   0 miz      (15155) users      (100)      872 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgReadMatrix.m
+-rw-r--r--   0 miz      (15155) users      (100)     3202 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgRefineAnisotropic.m
+-rw-r--r--   0 miz      (15155) users      (100)     4156 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgRefineSurplus.m
+-rw-r--r--   0 miz      (15155) users      (100)     1801 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgReloadGrid.m
+-rw-r--r--   0 miz      (15155) users      (100)      660 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgSummary.m
+-rw-r--r--   0 miz      (15155) users      (100)      891 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgUsingConstruction.m
+-rw-r--r--   0 miz      (15155) users      (100)     2711 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgWriteCustomRuleFile.m
+-rw-r--r--   0 miz      (15155) users      (100)      991 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceMATLAB/tsgWriteMatrix.m
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.273499 Tasmanian-8.1b2/InterfacePython/
+-rw-r--r--   0 miz      (15155) users      (100)    15865 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/CMakeLists.txt
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.273499 Tasmanian-8.1b2/InterfacePython/PipInstaller/
+-rw-r--r--   0 miz      (15155) users      (100)      430 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/PipInstaller/MANIFEST.in
+-rw-r--r--   0 miz      (15155) users      (100)     4326 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/PipInstaller/README.md
+-rw-r--r--   0 miz      (15155) users      (100)      472 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/PipInstaller/make_tarball.sh
+-rw-r--r--   0 miz      (15155) users      (100)       87 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/PipInstaller/pyproject.toml
+-rw-r--r--   0 miz      (15155) users      (100)     3106 2024-04-04 00:34:19.000000 Tasmanian-8.1b2/InterfacePython/PipInstaller/setup.py
+-rw-r--r--   0 miz      (15155) users      (100)     3874 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/Tasmanian.py
+-rw-r--r--   0 miz      (15155) users      (100)    23721 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianAddons.py
+-rw-r--r--   0 miz      (15155) users      (100)     4289 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianConfig.in.py
+-rw-r--r--   0 miz      (15155) users      (100)     2803 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianDREAM.py
+-rw-r--r--   0 miz      (15155) users      (100)     6636 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianDreamLikely.py
+-rw-r--r--   0 miz      (15155) users      (100)    29258 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianDreamSampler.py
+-rw-r--r--   0 miz      (15155) users      (100)     8090 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianDreamState.py
+-rw-r--r--   0 miz      (15155) users      (100)    17345 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianGradientDescent.py
+-rw-r--r--   0 miz      (15155) users      (100)     2553 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianOPT.py
+-rw-r--r--   0 miz      (15155) users      (100)    17715 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianParticleSwarm.py
+-rw-r--r--   0 miz      (15155) users      (100)   124558 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/TasmanianSG.py
+-rwxr-xr-x   0 miz      (15155) users      (100)     3393 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream.in.py
+-rw-r--r--   0 miz      (15155) users      (100)     5050 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream_01.py
+-rw-r--r--   0 miz      (15155) users      (100)     6783 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream_02.py
+-rw-r--r--   0 miz      (15155) users      (100)     6477 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream_03.py
+-rw-r--r--   0 miz      (15155) users      (100)     6752 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream_04.py
+-rw-r--r--   0 miz      (15155) users      (100)     7124 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_dream_05.py
+-rwxr-xr-x   0 miz      (15155) users      (100)     3177 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_optimization.in.py
+-rw-r--r--   0 miz      (15155) users      (100)     6127 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_optimization_01.py
+-rw-r--r--   0 miz      (15155) users      (100)     7283 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_optimization_02.py
+-rwxr-xr-x   0 miz      (15155) users      (100)     3911 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids.in.py
+-rw-r--r--   0 miz      (15155) users      (100)     4285 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_01.py
+-rw-r--r--   0 miz      (15155) users      (100)     4710 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_02.py
+-rw-r--r--   0 miz      (15155) users      (100)     4602 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_03.py
+-rw-r--r--   0 miz      (15155) users      (100)     4070 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_04.py
+-rw-r--r--   0 miz      (15155) users      (100)     6738 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_05.py
+-rw-r--r--   0 miz      (15155) users      (100)     4622 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_06.py
+-rw-r--r--   0 miz      (15155) users      (100)     3084 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_07.py
+-rw-r--r--   0 miz      (15155) users      (100)     5550 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_08.py
+-rw-r--r--   0 miz      (15155) users      (100)     5980 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_09.py
+-rw-r--r--   0 miz      (15155) users      (100)     4882 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_10.py
+-rw-r--r--   0 miz      (15155) users      (100)     4859 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/example_sparse_grids_11.py
+-rwxr-xr-x   0 miz      (15155) users      (100)      796 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/sandbox.py
+-rw-r--r--   0 miz      (15155) users      (100)     7102 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testAcceleration.py
+-rw-r--r--   0 miz      (15155) users      (100)     9604 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testAddons.py
+-rw-r--r--   0 miz      (15155) users      (100)    21512 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testBasicIO.py
+-rw-r--r--   0 miz      (15155) users      (100)     9245 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testCommon.py
+-rw-r--r--   0 miz      (15155) users      (100)      801 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testConfigureData.in.py
+-rw-r--r--   0 miz      (15155) users      (100)     5264 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testDream.py
+-rw-r--r--   0 miz      (15155) users      (100)    34228 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testExceptions.py
+-rw-r--r--   0 miz      (15155) users      (100)    20655 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testMakeUpdate.py
+-rw-r--r--   0 miz      (15155) users      (100)     8216 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testMisc.py
+-rw-r--r--   0 miz      (15155) users      (100)     8528 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testOptimization.py
+-rw-r--r--   0 miz      (15155) users      (100)    12423 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testRefinement.py
+-rwxr-xr-x   0 miz      (15155) users      (100)     2407 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testTSG.py
+-rw-r--r--   0 miz      (15155) users      (100)    12297 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfacePython/testUnstructuredData.py
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.273499 Tasmanian-8.1b2/InterfaceTPL/
+-rw-r--r--   0 miz      (15155) users      (100)     4009 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgBlasNull.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    22145 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgBlasWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    34665 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgCudaWrappers.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    12174 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgCudaWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    18800 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgDpcppWrappers.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     5953 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgDpcppWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    13496 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgGpuNull.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     7511 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgGpuWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    22391 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgHipWrappers.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     8686 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgHipWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     8657 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgMagmaWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     3410 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/InterfaceTPL/tsgTPLWrappers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     2227 2021-05-26 18:15:42.000000 Tasmanian-8.1b2/LICENSE
+-rw-r--r--   0 miz      (15155) users      (100)     5631 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/PKG-INFO
+-rw-r--r--   0 miz      (15155) users      (100)     5256 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/README.md
+-rw-r--r--   0 miz      (15155) users      (100)       81 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SUPPORT.md
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/SparseGrids/
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/SparseGrids/Benchmarks/
+-rw-r--r--   0 miz      (15155) users      (100)     8749 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchCommon.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     1718 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchDifferentiate.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     2145 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchEvaluate.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     1595 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchInterpolationWeights.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     1781 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchLoadNeeded.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     1445 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchMakeGrid.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     1883 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/benchRefine.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     8737 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Benchmarks/bench_main.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     9872 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/CMakeLists.txt
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/SparseGrids/Examples/
+-rw-r--r--   0 miz      (15155) users      (100)     3957 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     2718 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_01.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     3158 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_02.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4599 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_03.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4081 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_04.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     6147 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_05.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     5651 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_06.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     6219 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_07.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4848 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_08.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     5882 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_09.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4591 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_10.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4781 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_11.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    55377 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/GaussPattersonRule.table
+-rw-r--r--   0 miz      (15155) users      (100)    95905 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    10330 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.h
+-rw-r--r--   0 miz      (15155) users      (100)   126030 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    33108 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/TasmanianSparseGridWrapC.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     5770 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestCLICommon.hpp
+-rw-r--r--   0 miz      (15155) users      (100)   130197 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestExternalTests.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     8095 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestExternalTests.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    27756 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestTestFunctions.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    14436 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestTestFunctions.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    10155 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestTestHelpers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     8895 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestTestInterfaceC.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    36788 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestUnitTests.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     3513 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtestUnitTests.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     4088 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/gridtest_main.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     9141 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgAcceleratedDataStructures.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    40354 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgAcceleratedDataStructures.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5693 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgAcceleratedHandles.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     9942 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCacheLagrange.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    29251 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCoreOneDimensional.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    14976 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCoreOneDimensional.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    29102 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCudaBasisEvaluations.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    24125 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCudaKernels.cu
+-rw-r--r--   0 miz      (15155) users      (100)    13839 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCudaLinearAlgebra.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     6463 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgCudaLoadStructures.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     9707 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgDConstructGridGlobal.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    16083 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgDConstructGridGlobal.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    20939 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgDpcppBasisEvaluations.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    18700 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgDpcppKernels.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    33380 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgEnumerates.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     7785 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridCore.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    50202 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridFourier.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    11656 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridFourier.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    41549 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridGlobal.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    11771 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridGlobal.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    91861 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridLocalPolynomial.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    27808 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridLocalPolynomial.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    40023 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridSequence.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    12039 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridSequence.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    45354 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridWavelet.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     9275 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgGridWavelet.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    50527 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgHardCodedTabulatedRules.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4544 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgHardCodedTabulatedRules.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    17135 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgHierarchyManipulator.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    14269 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgHierarchyManipulator.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    22477 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgHipKernels.hip.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    15963 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgIOHelpers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    28494 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgIndexManipulator.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    26026 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgIndexManipulator.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    11776 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgIndexSets.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    20915 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgIndexSets.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    36519 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgLinearSolvers.cpp
+-rw-r--r--   0 miz      (15155) users      (100)    12646 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgLinearSolvers.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     5320 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgMathUtils.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    17803 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgOneDimensionalWrapper.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    49284 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgRuleLocalPolynomial.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    23153 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgRuleWavelet.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4997 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgRuleWavelet.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    23040 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgSequenceOptimizer.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     4675 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgSequenceOptimizer.hpp
+-rw-r--r--   0 miz      (15155) users      (100)     6432 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/SparseGrids/tsgUtils.hpp
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/Tasgrid/
+-rw-r--r--   0 miz      (15155) users      (100)     2725 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Tasgrid/CMakeLists.txt
+-rw-r--r--   0 miz      (15155) users      (100)     5469 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Tasgrid/tasgridLogs.in.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    44908 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Tasgrid/tasgridWrapper.cpp
+-rw-r--r--   0 miz      (15155) users      (100)     8534 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Tasgrid/tasgridWrapper.hpp
+-rw-r--r--   0 miz      (15155) users      (100)    57027 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Tasgrid/tasgrid_main.cpp
+drwxr-xr-x   0 miz      (15155) users      (100)        0 2024-04-04 00:34:31.281499 Tasmanian-8.1b2/Testing/
+-rw-r--r--   0 miz      (15155) users      (100)     1666 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Testing/CMakeLists.test.cmake
+-rw-r--r--   0 miz      (15155) users      (100)     3171 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Testing/tasmanian_version.cpp
+-rwxr-xr-x   0 miz      (15155) users      (100)      758 2024-04-04 00:31:36.000000 Tasmanian-8.1b2/Testing/test_post_install.in.sh
+-rw-r--r--   0 miz      (15155) users      (100)       87 2024-04-04 00:34:30.000000 Tasmanian-8.1b2/pyproject.toml
+-rw-r--r--   0 miz      (15155) users      (100)     3106 2024-04-04 00:34:30.000000 Tasmanian-8.1b2/setup.py
```

### Comparing `Tasmanian-8.1b1/Addons/CMakeLists.txt` & `Tasmanian-8.1b2/Addons/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/TasmanianAddons.hpp` & `Tasmanian-8.1b2/Addons/TasmanianAddons.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testAddons.cpp` & `Tasmanian-8.1b2/Addons/testAddons.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testConstructSurrogate.hpp` & `Tasmanian-8.1b2/Addons/testConstructSurrogate.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testCustomTabulated.hpp` & `Tasmanian-8.1b2/Addons/testCustomTabulated.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testExoticQuadrature.hpp` & `Tasmanian-8.1b2/Addons/testExoticQuadrature.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testLoadUnstructured.hpp` & `Tasmanian-8.1b2/Addons/testLoadUnstructured.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testMPI.cpp` & `Tasmanian-8.1b2/Addons/testMPI.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testMPI.hpp` & `Tasmanian-8.1b2/Addons/testMPI.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/testMPIDream.hpp` & `Tasmanian-8.1b2/Addons/testMPIDream.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgAddonsCommon.hpp` & `Tasmanian-8.1b2/Addons/tsgAddonsCommon.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgCConstructSurrogate.cpp` & `Tasmanian-8.1b2/Addons/tsgCConstructSurrogate.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgCExoticQuadrature.cpp` & `Tasmanian-8.1b2/Addons/tsgCExoticQuadrature.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgCLoadNeededValues.cpp` & `Tasmanian-8.1b2/Addons/tsgCLoadNeededValues.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgCLoadUnstructuredPoints.cpp` & `Tasmanian-8.1b2/Addons/tsgCLoadUnstructuredPoints.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgCandidateManager.hpp` & `Tasmanian-8.1b2/Addons/tsgCandidateManager.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgConstructSurrogate.hpp` & `Tasmanian-8.1b2/Addons/tsgConstructSurrogate.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgExoticQuadrature.hpp` & `Tasmanian-8.1b2/Addons/tsgExoticQuadrature.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgLoadNeededValues.hpp` & `Tasmanian-8.1b2/Addons/tsgLoadNeededValues.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgLoadUnstructuredPoints.hpp` & `Tasmanian-8.1b2/Addons/tsgLoadUnstructuredPoints.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgMPIConstructGrid.hpp` & `Tasmanian-8.1b2/Addons/tsgMPIConstructGrid.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgMPISampleDream.hpp` & `Tasmanian-8.1b2/Addons/tsgMPISampleDream.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgMPIScatterDream.hpp` & `Tasmanian-8.1b2/Addons/tsgMPIScatterDream.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Addons/tsgMPIScatterGrid.hpp` & `Tasmanian-8.1b2/Addons/tsgMPIScatterGrid.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/CHANGELOG.md` & `Tasmanian-8.1b2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 Changelog for version 8.1
 --------------
 
+* added support for Apple silicon M chips
+    * python required some work-arounds and bug-fixes, C++ was good before
+
 * added more multicore cpu support
     * parallelized setting surplus refinement
     * compatibility with gcc parallel STL algorithms
 
 * implemented a new algorithm for global sparse Kronecker
     * significant speedup when loading needed values
```

### Comparing `Tasmanian-8.1b1/CMakeLists.txt` & `Tasmanian-8.1b2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/AltBuildSystems/HeaderConvert.py` & `Tasmanian-8.1b2/Config/AltBuildSystems/HeaderConvert.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/AltBuildSystems/TasmanianConfig.hpp` & `Tasmanian-8.1b2/Config/AltBuildSystems/TasmanianConfig.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/AltBuildSystems/testConfigureData.py` & `Tasmanian-8.1b2/Config/AltBuildSystems/testConfigureData.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/CMakeLists.txt` & `Tasmanian-8.1b2/Config/CMakeIncludes/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/FindTasmanianDpcpp.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/FindTasmanianDpcpp.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/FindTasmanianMagma.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/FindTasmanianMagma.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/add_dependencies_target.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/add_dependencies_target.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/all_examples.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/all_examples.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/exports.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/exports.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/helper_macros.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/helper_macros.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/master_targets.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/master_targets.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/sanity_check_and_xsdk.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/sanity_check_and_xsdk.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeIncludes/setup_message.cmake` & `Tasmanian-8.1b2/Config/CMakeIncludes/setup_message.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/CMakeLists.examples.cmake` & `Tasmanian-8.1b2/Config/CMakeLists.examples.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/Tasmanian.h` & `Tasmanian-8.1b2/Config/Tasmanian.h`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/Tasmanian.hpp` & `Tasmanian-8.1b2/Config/Tasmanian.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/TasmanianConfig.in.cmake` & `Tasmanian-8.1b2/Config/TasmanianConfig.in.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/TasmanianConfig.in.hpp` & `Tasmanian-8.1b2/Config/TasmanianConfig.in.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/TasmanianENVsetup.in.sh` & `Tasmanian-8.1b2/Config/TasmanianENVsetup.in.sh`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Config/magma_cmake.patch` & `Tasmanian-8.1b2/Config/magma_cmake.patch`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/CMakeLists.txt` & `Tasmanian-8.1b2/DREAM/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream_01.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream_01.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream_02.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream_02.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream_03.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream_03.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream_04.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream_04.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_dream_05.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_dream_05.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_optimization.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_optimization.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_optimization_01.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_optimization_01.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Examples/example_optimization_02.cpp` & `Tasmanian-8.1b2/DREAM/Examples/example_optimization_02.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/TasmanianOptimization.hpp` & `Tasmanian-8.1b2/DREAM/Optimization/TasmanianOptimization.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/TasmanianOptimizationWrapC.cpp` & `Tasmanian-8.1b2/DREAM/Optimization/TasmanianOptimizationWrapC.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tasdreamOptimizationTests.cpp` & `Tasmanian-8.1b2/DREAM/Optimization/tasdreamOptimizationTests.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tsgGradientDescent.cpp` & `Tasmanian-8.1b2/DREAM/Optimization/tsgGradientDescent.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tsgGradientDescent.hpp` & `Tasmanian-8.1b2/DREAM/Optimization/tsgGradientDescent.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tsgOptimizationUtils.hpp` & `Tasmanian-8.1b2/DREAM/Optimization/tsgOptimizationUtils.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tsgParticleSwarm.cpp` & `Tasmanian-8.1b2/DREAM/Optimization/tsgParticleSwarm.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/Optimization/tsgParticleSwarm.hpp` & `Tasmanian-8.1b2/DREAM/Optimization/tsgParticleSwarm.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/TasmanianDREAM.hpp` & `Tasmanian-8.1b2/DREAM/TasmanianDREAM.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/dreamtest_main.cpp` & `Tasmanian-8.1b2/DREAM/dreamtest_main.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tasdreamExternalTests.cpp` & `Tasmanian-8.1b2/DREAM/tasdreamExternalTests.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tasdreamExternalTests.hpp` & `Tasmanian-8.1b2/DREAM/tasdreamExternalTests.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamCorePDF.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamCorePDF.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamCoreRandom.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamCoreRandom.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamEnumerates.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamEnumerates.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamLikelihoodCore.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamLikelihoodCore.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamLikelyGaussian.cpp` & `Tasmanian-8.1b2/DREAM/tsgDreamLikelyGaussian.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamLikelyGaussian.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamLikelyGaussian.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamSample.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamSample.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamSampleWrapC.cpp` & `Tasmanian-8.1b2/DREAM/tsgDreamSampleWrapC.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamState.cpp` & `Tasmanian-8.1b2/DREAM/tsgDreamState.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/DREAM/tsgDreamState.hpp` & `Tasmanian-8.1b2/DREAM/tsgDreamState.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/CMakeLists.txt` & `Tasmanian-8.1b2/Doxygen/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/Contributors.md` & `Tasmanian-8.1b2/Doxygen/Contributors.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/CustomRuleFileFormat.md` & `Tasmanian-8.1b2/Doxygen/CustomRuleFileFormat.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/DevNotes.md` & `Tasmanian-8.1b2/Doxygen/DevNotes.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/Installation.md` & `Tasmanian-8.1b2/Doxygen/Installation.md`

 * *Files 5% similar despite different names*

```diff
@@ -278,14 +278,25 @@
   cmake --build . --config Release
   ctest -C Release
   cmake --build . --config Release --target install
 ```
 * Both Debug and Release are supported config modes, but do not use them simultaneously,
   pick only one Release or Debug.
 
+### Install on Mac platform
+
+Apple with Intel CPU will handle Tasmanian in the same way as Linux.
+
+Using Apple silicon M chips, the python interface is broken prior to 8.1, which is still in development.
+The development version can be downloaded from the main branch on github
+or a beta pre-release is available through Python PIP:
+```
+  python -m pip install Tasmanian==8.1b1 --user
+```
+
 ### Install folder structure
 
 Tasmanian follows standard Linux conventions, the install path could
 be set to `/usr/local/`, although it is recommended to install in
 a location inside the user home folder to avoid potential system-wide conflicts.
 
 * Install folder structure:
@@ -352,24 +363,27 @@
 ```
 The modules correspond to shared and static libraries and the cmake options used during build.
 
 All available components will be included even if the component is not explicitly requested.
 Requesting components can help catch errors early in the build process
 and/or print useful log messages. For example:
 ```
-  find_package(Tasmanian 7.0 REQUIRED SHARED PYTHON CUDA OPTIONAL_COMPONENTS OPENMP)
+  find_package(Tasmanian 8.0 REQUIRED SHARED PYTHON CUDA OPTIONAL_COMPONENTS OPENMP)
 ```
 In the above example:
 * an error will be generated if Tasmanian was build with static libraries, no CUDA or no Python support
 * a status message will report whether Tasmanian was build with OpenMP support
 * requesting incompatible components will always fail, e.g., CUDA with ROCM or SHARED and STATIC
 
 ### Known Issues
 
 Several known issues and work-around fixes:
+* Apple OSX has poor support for OpenMP, especially when using M-chips (apple silicon)
+    * OpenMP is not supported by the default compiler (xcode)
+    * gcc with OpenMP support can be installed through Homebrew, but the performance gains from multi-threading are low
 * the automated MAGMA download reports the wrong GPU architecture enabled
     * ignore the MAGMA message the build correctly respects `CMAKE_CUDA_ARCHITECTURES`
 * The addon tests sometime fail due to thread scheduling
     * The overhead associated with thread scheduling is much larger than the simple test models used,
     which leads to unrealistically large fluctuations in sample run-time, which in turn leads to
     randomness in the results, most notably on machines with few cpu cores.
     * Rerun the tests and/or installation to see if the problem is persistent
```

### Comparing `Tasmanian-8.1b1/Doxygen/InterfaceCLI.md` & `Tasmanian-8.1b2/Doxygen/InterfaceCLI.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/InterfaceFortran2003.md` & `Tasmanian-8.1b2/Doxygen/InterfaceFortran2003.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/InterfaceLibEnsemble.md` & `Tasmanian-8.1b2/Doxygen/InterfaceLibEnsemble.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/InterfaceMATLAB.md` & `Tasmanian-8.1b2/Doxygen/InterfaceMATLAB.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/InterfacePython.md` & `Tasmanian-8.1b2/Doxygen/InterfacePython.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/footer.html` & `Tasmanian-8.1b2/Doxygen/footer.html`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/header.html` & `Tasmanian-8.1b2/Doxygen/header.html`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Doxygen/tasmanian.css` & `Tasmanian-8.1b2/Doxygen/tasmanian.css`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/CMakeLists.txt` & `Tasmanian-8.1b2/InterfaceFortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/Examples/example_sparse_grids.f90` & `Tasmanian-8.1b2/InterfaceFortran/Examples/example_sparse_grids.f90`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/TasmanianSG.f90` & `Tasmanian-8.1b2/InterfaceFortran/TasmanianSG.f90`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/fortester.f90` & `Tasmanian-8.1b2/InterfaceFortran/fortester.f90`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/mpitester.f90` & `Tasmanian-8.1b2/InterfaceFortran/mpitester.f90`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/tsgC2Fortran.cpp` & `Tasmanian-8.1b2/InterfaceFortran/tsgC2Fortran.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceFortran/tsgC2FortranBridge.f90` & `Tasmanian-8.1b2/InterfaceFortran/tsgC2FortranBridge.f90`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/CMakeLists.txt` & `Tasmanian-8.1b2/InterfaceMATLAB/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgCancelRefine.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgCancelRefine.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgCleanTempFiles.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgCleanTempFiles.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgCopyGrid.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgCopyGrid.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgCoreTests.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgCoreTests.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgDeleteGridByName.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgDeleteGridByName.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgDifferentiate.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgDifferentiate.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgEstimateAnisotropicCoefficients.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgEstimateAnisotropicCoefficients.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgEvaluate.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgEvaluate.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgEvaluateHierarchy.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgEvaluateHierarchy.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgExample.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgExample.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetCandidateConstructionAnisotropic.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetCandidateConstructionAnisotropic.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetCandidateConstructionSurplus.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetCandidateConstructionSurplus.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetDifferentiationWeights.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetDifferentiationWeights.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetHCoefficients.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetHCoefficients.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetHSupport.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetHSupport.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetInterpolationWeights.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetInterpolationWeights.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetNeededIndexes.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetNeededIndexes.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetNeededPoints.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetNeededPoints.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPoints.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPoints.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPointsIndexes.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPointsIndexes.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetPolynomialSpaces.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetPolynomialSpaces.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgGetQuadrature.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgGetQuadrature.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgIntegrate.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgIntegrate.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgListGridsByName.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgListGridsByName.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadConstructedPoints.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadConstructedPoints.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadGridFromFile.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadGridFromFile.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadHCoefficients.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadHCoefficients.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgLoadValues.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgLoadValues.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeExoticQuadrature.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeExoticQuadrature.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeFilenames.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeFilenames.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeFourier.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeFourier.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeGlobal.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeGlobal.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeLocalPolynomial.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeLocalPolynomial.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeQuadrature.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeQuadrature.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeSequence.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeSequence.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMakeWavelet.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMakeWavelet.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgMergeRefine.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgMergeRefine.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgPlotPoints2D.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgPlotPoints2D.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgReadCustomRuleFile.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgReadCustomRuleFile.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgReadMatrix.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgReadMatrix.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgRefineAnisotropic.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgRefineAnisotropic.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgRefineSurplus.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgRefineSurplus.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgReloadGrid.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgReloadGrid.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgSummary.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgSummary.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgUsingConstruction.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgUsingConstruction.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgWriteCustomRuleFile.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgWriteCustomRuleFile.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceMATLAB/tsgWriteMatrix.m` & `Tasmanian-8.1b2/InterfaceMATLAB/tsgWriteMatrix.m`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/CMakeLists.txt` & `Tasmanian-8.1b2/InterfacePython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/PipInstaller/README.md` & `Tasmanian-8.1b2/InterfacePython/PipInstaller/README.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/PipInstaller/setup.py` & `Tasmanian-8.1b2/InterfacePython/PipInstaller/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 if isosxframework:
     cmake_args.append('-DTasmanian_osx_framework:BOOL=ON')
 
 
 # call the actual package setup command
 setup(
     name='Tasmanian',
-    version='8.1b1',
+    version='8.1b2',
     author='Miroslav Stoyanov',
     author_email='stoyanovmk@ornl.gov',
     description='UQ library for sparse grids, optimization and Bayesian inference',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://tasmanian.ornl.gov',
     classifiers=[
```

### Comparing `Tasmanian-8.1b1/InterfacePython/Tasmanian.py` & `Tasmanian-8.1b2/InterfacePython/Tasmanian.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianAddons.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianAddons.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianConfig.in.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianConfig.in.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianDREAM.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianDREAM.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianDreamLikely.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianDreamLikely.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianDreamSampler.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianDreamSampler.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianDreamState.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianDreamState.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianGradientDescent.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianGradientDescent.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianOPT.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianOPT.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianParticleSwarm.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianParticleSwarm.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/TasmanianSG.py` & `Tasmanian-8.1b2/InterfacePython/TasmanianSG.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream.in.py` & `Tasmanian-8.1b2/InterfacePython/example_dream.in.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream_01.py` & `Tasmanian-8.1b2/InterfacePython/example_dream_01.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream_02.py` & `Tasmanian-8.1b2/InterfacePython/example_dream_02.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream_03.py` & `Tasmanian-8.1b2/InterfacePython/example_dream_03.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream_04.py` & `Tasmanian-8.1b2/InterfacePython/example_dream_04.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_dream_05.py` & `Tasmanian-8.1b2/InterfacePython/example_dream_05.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_optimization.in.py` & `Tasmanian-8.1b2/InterfacePython/example_optimization.in.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_optimization_01.py` & `Tasmanian-8.1b2/InterfacePython/example_optimization_01.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_optimization_02.py` & `Tasmanian-8.1b2/InterfacePython/example_optimization_02.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids.in.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids.in.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_01.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_01.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_02.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_02.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_03.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_03.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_04.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_04.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_05.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_05.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_06.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_06.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_07.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_07.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_08.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_08.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_09.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_09.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_10.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_10.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/example_sparse_grids_11.py` & `Tasmanian-8.1b2/InterfacePython/example_sparse_grids_11.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/sandbox.py` & `Tasmanian-8.1b2/InterfacePython/sandbox.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testAcceleration.py` & `Tasmanian-8.1b2/InterfacePython/testAcceleration.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testAddons.py` & `Tasmanian-8.1b2/InterfacePython/testAddons.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testBasicIO.py` & `Tasmanian-8.1b2/InterfacePython/testBasicIO.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testCommon.py` & `Tasmanian-8.1b2/InterfacePython/testCommon.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testConfigureData.in.py` & `Tasmanian-8.1b2/InterfacePython/testConfigureData.in.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testDream.py` & `Tasmanian-8.1b2/InterfacePython/testDream.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testExceptions.py` & `Tasmanian-8.1b2/InterfacePython/testExceptions.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testMakeUpdate.py` & `Tasmanian-8.1b2/InterfacePython/testMakeUpdate.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testMisc.py` & `Tasmanian-8.1b2/InterfacePython/testMisc.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testOptimization.py` & `Tasmanian-8.1b2/InterfacePython/testOptimization.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testRefinement.py` & `Tasmanian-8.1b2/InterfacePython/testRefinement.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testTSG.py` & `Tasmanian-8.1b2/InterfacePython/testTSG.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfacePython/testUnstructuredData.py` & `Tasmanian-8.1b2/InterfacePython/testUnstructuredData.py`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgBlasNull.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgBlasNull.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgBlasWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgBlasWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgCudaWrappers.cpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgCudaWrappers.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgCudaWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgCudaWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgDpcppWrappers.cpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgDpcppWrappers.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgDpcppWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgDpcppWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgGpuNull.cpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgGpuNull.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgGpuWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgGpuWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgHipWrappers.cpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgHipWrappers.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgHipWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgHipWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgMagmaWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgMagmaWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/InterfaceTPL/tsgTPLWrappers.hpp` & `Tasmanian-8.1b2/InterfaceTPL/tsgTPLWrappers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/LICENSE` & `Tasmanian-8.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/PKG-INFO` & `Tasmanian-8.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tasmanian
-Version: 8.1b1
+Version: 8.1b2
 Summary: UQ library for sparse grids, optimization and Bayesian inference
 Home-page: https://tasmanian.ornl.gov
 Author: Miroslav Stoyanov
 Author-email: stoyanovmk@ornl.gov
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Tasmanian-8.1b1/README.md` & `Tasmanian-8.1b2/README.md`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchCommon.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchCommon.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchDifferentiate.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchDifferentiate.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchEvaluate.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchEvaluate.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchInterpolationWeights.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchInterpolationWeights.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchLoadNeeded.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchLoadNeeded.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchMakeGrid.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchMakeGrid.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/benchRefine.hpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/benchRefine.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Benchmarks/bench_main.cpp` & `Tasmanian-8.1b2/SparseGrids/Benchmarks/bench_main.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/CMakeLists.txt` & `Tasmanian-8.1b2/SparseGrids/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_01.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_01.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_02.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_02.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_03.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_03.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_04.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_04.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_05.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_05.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_06.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_06.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_07.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_07.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_08.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_08.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_09.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_09.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_10.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_10.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/Examples/example_sparse_grids_11.cpp` & `Tasmanian-8.1b2/SparseGrids/Examples/example_sparse_grids_11.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/GaussPattersonRule.table` & `Tasmanian-8.1b2/SparseGrids/GaussPattersonRule.table`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.cpp` & `Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.h` & `Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.h`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/TasmanianSparseGrid.hpp` & `Tasmanian-8.1b2/SparseGrids/TasmanianSparseGrid.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/TasmanianSparseGridWrapC.cpp` & `Tasmanian-8.1b2/SparseGrids/TasmanianSparseGridWrapC.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestCLICommon.hpp` & `Tasmanian-8.1b2/SparseGrids/gridtestCLICommon.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestExternalTests.cpp` & `Tasmanian-8.1b2/SparseGrids/gridtestExternalTests.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1481,15 +1481,15 @@
         }
     }{
         const BaseFunction *f = &f21curved;
         grid.makeGlobalGrid(f->getNumInputs(), f->getNumOutputs(), 3, type_iptotal, rule_leja);
         int np[10] = { 10, 12, 17, 24, 32, 34, 41, 42, 57, 59 };
         double errs[10] = { 9.48e-03, 9.50e-03, 6.85e-03, 5.11e-04, 6.26e-05, 7.11e-06, 5.07e-06, 5.19e-06, 1.17e-08, 1.86e-08 };
         if (!testAnisotropicRefinement(f, grid, type_ipcurved, 1, np, errs, 7)){
-            cout << "ERROR: failed anisotropic refinement using leja ipcurved nodes for " << f->getDescription() << endl;  pass2 = false;
+            cout << "ERROR: failed anisotropic refinement (global) using leja ipcurved nodes for " << f->getDescription() << endl;  pass2 = false;
         }
     }{
         const BaseFunction *f = &f21curved;
         grid.makeGlobalGrid(f->getNumInputs(), f->getNumOutputs(), 3, type_iptotal, rule_clenshawcurtis);
         int np[3] = { 13, 21, 29 };
         double errs[3] = { 6.12e-04, 6.05e-04, 1.33e-08 };
         if (!testAnisotropicRefinement(f, grid, type_ipcurved, 1, np, errs, 3)){
@@ -1498,15 +1498,15 @@
     }{
         const BaseFunction *f = &f21curved;
         grid.makeSequenceGrid(f->getNumInputs(), f->getNumOutputs(), 3, type_iptotal, rule_leja);
         grid.enableAcceleration(accel_none);
         int np[10] = { 10, 12, 17, 24, 32, 34, 41, 42, 57, 59 };
         double errs[10] = { 9.48e-03, 9.50e-03, 6.85e-03, 5.11e-04, 6.26e-05, 7.11e-06, 5.07e-06, 5.19e-06, 1.17e-08, 1.86e-08 };
         if (!testAnisotropicRefinement(f, grid, type_ipcurved, 1, np, errs, 7)){
-            cout << "ERROR: failed anisotropic refinement using leja ipcurved nodes for " << f->getDescription() << endl;  pass2 = false;
+            cout << "ERROR: failed anisotropic refinement (sequence) using leja ipcurved nodes for " << f->getDescription() << endl;  pass2 = false;
         }
     }{
         const BaseFunction *f = &f21c1c2periodic;
         grid.makeFourierGrid(f->getNumInputs(), f->getNumOutputs(), 3, type_hyperbolic);
         grid.setDomainTransform({-1.0, -1.0}, {1.0, 1.0});
         int np[5] = { 17, 35, 111, 273, 759 };
         double errs[5] = { 1.28e-2, 2.80e-3, 1.97e-4, 6.78e-5, 5.65e-5 };
```

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestExternalTests.hpp` & `Tasmanian-8.1b2/SparseGrids/gridtestExternalTests.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestTestFunctions.cpp` & `Tasmanian-8.1b2/SparseGrids/gridtestTestFunctions.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestTestFunctions.hpp` & `Tasmanian-8.1b2/SparseGrids/gridtestTestFunctions.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestTestHelpers.hpp` & `Tasmanian-8.1b2/SparseGrids/gridtestTestHelpers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestTestInterfaceC.cpp` & `Tasmanian-8.1b2/SparseGrids/gridtestTestInterfaceC.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestUnitTests.cpp` & `Tasmanian-8.1b2/SparseGrids/gridtestUnitTests.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtestUnitTests.hpp` & `Tasmanian-8.1b2/SparseGrids/gridtestUnitTests.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/gridtest_main.cpp` & `Tasmanian-8.1b2/SparseGrids/gridtest_main.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgAcceleratedDataStructures.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgAcceleratedDataStructures.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgAcceleratedDataStructures.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgAcceleratedDataStructures.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgAcceleratedHandles.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgAcceleratedHandles.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCacheLagrange.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgCacheLagrange.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCoreOneDimensional.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgCoreOneDimensional.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCoreOneDimensional.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgCoreOneDimensional.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCudaBasisEvaluations.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgCudaBasisEvaluations.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCudaKernels.cu` & `Tasmanian-8.1b2/SparseGrids/tsgCudaKernels.cu`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCudaLinearAlgebra.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgCudaLinearAlgebra.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgCudaLoadStructures.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgCudaLoadStructures.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgDConstructGridGlobal.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgDConstructGridGlobal.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgDConstructGridGlobal.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgDConstructGridGlobal.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -197,14 +197,29 @@
 std::vector<double> listToNodes(std::forward_list<NodeData> const &node_list, size_t num_dimensions, RuleLike const &rule){
     std::vector<double> result(Utils::size_mult(std::distance(node_list.begin(), node_list.end()), num_dimensions));
     auto ix = result.begin();
     for(auto const &t : node_list)
         ix = MultiIndexManipulations::indexesToNodes(t.point, rule, ix);
     return result;
 }
+/*!
+ * \internal
+ * \ingroup TasmanianRefinement
+ * \brief Using MultiIndexManipulations::indexesToNodes() convert the \b node_list to actual points according to the rule.
+ *
+ * \endinternal
+ */
+template<typename callable_method>
+std::vector<double> listToLocalNodes(std::forward_list<NodeData> const &node_list, size_t num_dimensions, callable_method rule){
+    std::vector<double> result(Utils::size_mult(std::distance(node_list.begin(), node_list.end()), num_dimensions));
+    auto ix = result.begin();
+    for(auto const &t : node_list)
+        ix = std::transform(t.point.begin(), t.point.end(), ix, rule);
+    return result;
+}
 
 /*!
  * \internal
  * \ingroup TasmanianRefinement
  * \brief Helper class that stores data from dynamic construction of a Global grid.
  *
  * The class stores candidate tensors with corresponding weights
```

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgDpcppBasisEvaluations.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgDpcppBasisEvaluations.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgDpcppKernels.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgDpcppKernels.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgEnumerates.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgEnumerates.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridCore.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridCore.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridFourier.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridFourier.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridFourier.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridFourier.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridGlobal.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridGlobal.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridGlobal.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridGlobal.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridLocalPolynomial.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridLocalPolynomial.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 #include "tsgTPLWrappers.hpp"
 
 namespace TasGrid{
 
 template<bool iomode> void GridLocalPolynomial::write(std::ostream &os) const{
     if (iomode == mode_ascii){ os << std::scientific; os.precision(17); }
     IO::writeNumbers<iomode, IO::pad_line>(os, num_dimensions, num_outputs, order, top_level);
-    IO::writeRule<iomode>(rule->getType(), os);
+    IO::writeRule<iomode>(RuleLocal::getRule(effective_rule), os);
     IO::writeFlag<iomode, IO::pad_auto>(!points.empty(), os);
     if (!points.empty()) points.write<iomode>(os);
     if (iomode == mode_ascii){ // backwards compatible: surpluses and needed, or needed and surpluses
         IO::writeFlag<iomode, IO::pad_auto>((surpluses.getNumStrips() != 0), os);
         if (!surpluses.empty()) surpluses.writeVector<iomode, IO::pad_line>(os);
         IO::writeFlag<iomode, IO::pad_auto>(!needed.empty(), os);
         if (!needed.empty()) needed.write<iomode>(os);
@@ -68,73 +68,135 @@
 
 template void GridLocalPolynomial::write<mode_ascii>(std::ostream &) const;
 template void GridLocalPolynomial::write<mode_binary>(std::ostream &) const;
 
 GridLocalPolynomial::GridLocalPolynomial(AccelerationContext const *acc, int cnum_dimensions, int cnum_outputs, int depth, int corder, TypeOneDRule crule, const std::vector<int> &level_limits)
     : BaseCanonicalGrid(acc, cnum_dimensions, cnum_outputs, MultiIndexSet(), MultiIndexSet(), StorageSet()),
       order(corder),
-      rule(makeRuleLocalPolynomial(((crule == rule_semilocalp) && (order < 2)) ? rule_localp : crule, corder))
-      {
+      effective_rule(RuleLocal::getEffectiveRule(order, (crule == rule_semilocalp and order < 2) ? rule_localp : crule))
+    {
 
     MultiIndexSet tensors = MultiIndexManipulations::selectTensors((size_t) num_dimensions, depth, type_level, [&](int i) -> int{ return i; }, std::vector<int>(), level_limits);
 
-    needed = MultiIndexManipulations::generateNestedPoints(tensors, [&](int l) -> int{ return rule->getNumPoints(l); });
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            needed = MultiIndexManipulations::generateNestedPoints(tensors,
+                [&](int l) -> int{ return RuleLocal::getNumPoints<RuleLocal::erule::pwc>(l); });
+            break;
+        case RuleLocal::erule::localp:
+            needed = MultiIndexManipulations::generateNestedPoints(tensors,
+                [&](int l) -> int{ return RuleLocal::getNumPoints<RuleLocal::erule::localp>(l); });
+            break;
+        case RuleLocal::erule::semilocalp:
+            needed = MultiIndexManipulations::generateNestedPoints(tensors,
+                [&](int l) -> int{ return RuleLocal::getNumPoints<RuleLocal::erule::semilocalp>(l); });
+            break;
+        case RuleLocal::erule::localp0:
+            needed = MultiIndexManipulations::generateNestedPoints(tensors,
+                [&](int l) -> int{ return RuleLocal::getNumPoints<RuleLocal::erule::localp0>(l); });
+            break;
+        default: // case RuleLocal::erule::localpb:
+            needed = MultiIndexManipulations::generateNestedPoints(tensors,
+                [&](int l) -> int{ return RuleLocal::getNumPoints<RuleLocal::erule::localpb>(l); });
+            break;
+    };
 
     buildTree();
 
     if (num_outputs == 0){
         points = std::move(needed);
         needed = MultiIndexSet();
-        parents = HierarchyManipulations::computeDAGup(points, rule.get());
+        parents = HierarchyManipulations::computeDAGup(points, effective_rule);
     }else{
         values.resize(num_outputs, needed.getNumIndexes());
     }
 }
 
 GridLocalPolynomial::GridLocalPolynomial(AccelerationContext const *acc, GridLocalPolynomial const *pwpoly, int ibegin, int iend) :
     BaseCanonicalGrid(acc, *pwpoly, ibegin, iend),
     order(pwpoly->order),
     top_level(pwpoly->top_level),
     surpluses((num_outputs == pwpoly->num_outputs) ? pwpoly->surpluses : pwpoly->surpluses.splitData(ibegin, iend)),
     parents(pwpoly->parents),
     roots(pwpoly->roots),
     pntr(pwpoly->pntr),
     indx(pwpoly->indx),
-    rule(makeRuleLocalPolynomial(pwpoly->rule->getType(), pwpoly->order)){
+    effective_rule(pwpoly->effective_rule){
 
     if (pwpoly->dynamic_values){
         dynamic_values = Utils::make_unique<SimpleConstructData>(*pwpoly->dynamic_values);
         if (num_outputs != pwpoly->num_outputs) dynamic_values->restrictData(ibegin, iend);
     }
 }
 
 GridLocalPolynomial::GridLocalPolynomial(AccelerationContext const *acc, int cnum_dimensions, int cnum_outputs, int corder, TypeOneDRule crule,
                                          std::vector<int> &&pnts, std::vector<double> &&vals, std::vector<double> &&surps)
     : BaseCanonicalGrid(acc, cnum_dimensions, cnum_outputs, MultiIndexSet(cnum_dimensions, std::move(pnts)), MultiIndexSet(),
                         StorageSet(cnum_outputs, static_cast<int>(vals.size() / cnum_outputs), std::move(vals))),
     order(corder),
     surpluses(Data2D<double>(cnum_outputs, points.getNumIndexes(), std::move(surps))),
-    rule(makeRuleLocalPolynomial(crule, corder)){
+    effective_rule(RuleLocal::getEffectiveRule(order, crule)){
 
     buildTree();
 }
 
-void GridLocalPolynomial::getLoadedPoints(double *x) const{
-    int num_points = points.getNumIndexes();
+struct localp_loaded{};
+struct localp_needed{};
+
+template<RuleLocal::erule eff_rule, typename points_mode>
+void GridLocalPolynomial::getPoints(double *x) const {
+    int num_points = (std::is_same<points_mode, localp_loaded>::value) ? points.getNumIndexes() : needed.getNumIndexes();
     Utils::Wrapper2D<double> split(num_dimensions, x);
     #pragma omp parallel for schedule(static)
-    for(int i=0; i<num_points; i++)
-        MultiIndexManipulations::indexesToNodes(points.getIndex(i), num_dimensions, *rule, split.getStrip(i));
+    for(int i=0; i<num_points; i++) {
+        int const *p = (std::is_same<points_mode, localp_loaded>::value) ? points.getIndex(i) : needed.getIndex(i);
+        double *s = split.getStrip(i);
+        for(int j=0; j<num_dimensions; j++)
+            s[j] = RuleLocal::getNode<eff_rule>(p[j]);
+    }
+}
+void GridLocalPolynomial::getLoadedPoints(double *x) const{
+    using pmode = localp_loaded;
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            getPoints<RuleLocal::erule::pwc, pmode>(x);
+            break;
+        case RuleLocal::erule::localp:
+            getPoints<RuleLocal::erule::localp, pmode>(x);
+            break;
+        case RuleLocal::erule::semilocalp:
+            getPoints<RuleLocal::erule::semilocalp, pmode>(x);
+            break;
+        case RuleLocal::erule::localp0:
+            getPoints<RuleLocal::erule::localp0, pmode>(x);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            getPoints<RuleLocal::erule::localpb, pmode>(x);
+            break;
+    };
 }
 void GridLocalPolynomial::getNeededPoints(double *x) const{
-    int num_points = needed.getNumIndexes();
-    Utils::Wrapper2D<double> split(num_dimensions, x);
-    #pragma omp parallel for schedule(static)
-    for(int i=0; i<num_points; i++)
-        MultiIndexManipulations::indexesToNodes(needed.getIndex(i), num_dimensions, *rule, split.getStrip(i));
+    using pmode = localp_needed;
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            getPoints<RuleLocal::erule::pwc, pmode>(x);
+            break;
+        case RuleLocal::erule::localp:
+            getPoints<RuleLocal::erule::localp, pmode>(x);
+            break;
+        case RuleLocal::erule::semilocalp:
+            getPoints<RuleLocal::erule::semilocalp, pmode>(x);
+            break;
+        case RuleLocal::erule::localp0:
+            getPoints<RuleLocal::erule::localp0, pmode>(x);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            getPoints<RuleLocal::erule::localpb, pmode>(x);
+            break;
+    };
 }
 void GridLocalPolynomial::getPoints(double *x) const{
     if (points.empty()){ getNeededPoints(x); }else{ getLoadedPoints(x); }
 }
 
 void GridLocalPolynomial::evaluate(const double x[], double y[]) const{
     std::fill_n(y, num_outputs, 0.0);
@@ -216,15 +278,15 @@
         }
     }
 }
 
 void GridLocalPolynomial::loadNeededValuesGPU(const double *vals){
     updateValues(vals);
 
-    std::vector<int> levels = HierarchyManipulations::computeLevels(points, rule.get());
+    std::vector<int> levels = HierarchyManipulations::computeLevels(points, effective_rule);
 
     std::vector<Data2D<int>> lpnts = HierarchyManipulations::splitByLevels(points, levels);
     std::vector<Data2D<double>> lvals = HierarchyManipulations::splitByLevels(values, levels);
 
     Data2D<double> allx(num_dimensions, points.getNumIndexes());
     getPoints(allx.data());
 
@@ -304,67 +366,61 @@
     evaluateBatchGPUtempl(gpu_x, cpu_num_x, gpu_y);
 }
 void GridLocalPolynomial::evaluateBatchGPU(const float gpu_x[], int cpu_num_x, float gpu_y[]) const{
     evaluateBatchGPUtempl(gpu_x, cpu_num_x, gpu_y);
 }
 void GridLocalPolynomial::evaluateHierarchicalFunctionsGPU(const double gpu_x[], int cpu_num_x, double *gpu_y) const{
     loadGpuBasis<double>();
-    TasGpu::devalpwpoly(acceleration, order, rule->getType(), num_dimensions, cpu_num_x, getNumPoints(), gpu_x, gpu_cache->nodes.data(), gpu_cache->support.data(), gpu_y);
+    TasGpu::devalpwpoly(acceleration, order, RuleLocal::getRule(effective_rule), num_dimensions, cpu_num_x, getNumPoints(), gpu_x, gpu_cache->nodes.data(), gpu_cache->support.data(), gpu_y);
 }
 void GridLocalPolynomial::buildSparseBasisMatrixGPU(const double gpu_x[], int cpu_num_x, GpuVector<int> &gpu_spntr, GpuVector<int> &gpu_sindx, GpuVector<double> &gpu_svals) const{
     loadGpuBasis<double>();
     loadGpuHierarchy<double>();
-    TasGpu::devalpwpoly_sparse(acceleration, order, rule->getType(), num_dimensions, cpu_num_x, gpu_x,
+    TasGpu::devalpwpoly_sparse(acceleration, order, RuleLocal::getRule(effective_rule), num_dimensions, cpu_num_x, gpu_x,
                                gpu_cache->nodes, gpu_cache->support,
                                gpu_cache->hpntr, gpu_cache->hindx, gpu_cache->hroots, gpu_spntr, gpu_sindx, gpu_svals);
 }
 void GridLocalPolynomial::evaluateHierarchicalFunctionsGPU(const float gpu_x[], int cpu_num_x, float *gpu_y) const{
     loadGpuBasis<float>();
-    TasGpu::devalpwpoly(acceleration, order, rule->getType(), num_dimensions, cpu_num_x, getNumPoints(), gpu_x, gpu_cachef->nodes.data(), gpu_cachef->support.data(), gpu_y);
+    TasGpu::devalpwpoly(acceleration, order, RuleLocal::getRule(effective_rule), num_dimensions, cpu_num_x, getNumPoints(), gpu_x, gpu_cachef->nodes.data(), gpu_cachef->support.data(), gpu_y);
 }
 void GridLocalPolynomial::buildSparseBasisMatrixGPU(const float gpu_x[], int cpu_num_x, GpuVector<int> &gpu_spntr, GpuVector<int> &gpu_sindx, GpuVector<float> &gpu_svals) const{
     loadGpuBasis<float>();
     loadGpuHierarchy<float>();
-    TasGpu::devalpwpoly_sparse(acceleration, order, rule->getType(), num_dimensions, cpu_num_x, gpu_x,
+    TasGpu::devalpwpoly_sparse(acceleration, order, RuleLocal::getRule(effective_rule), num_dimensions, cpu_num_x, gpu_x,
                                gpu_cachef->nodes, gpu_cachef->support,
                                gpu_cachef->hpntr, gpu_cachef->hindx, gpu_cachef->hroots, gpu_spntr, gpu_sindx, gpu_svals);
 }
 template<typename T> void GridLocalPolynomial::loadGpuBasis() const{
     auto& ccache = getGpuCache<T>();
     if (!ccache) ccache = Utils::make_unique<CudaLocalPolynomialData<T>>();
     if (!ccache->nodes.empty()) return;
 
     Data2D<double> cpu_nodes(num_dimensions, getNumPoints());
     getPoints(cpu_nodes.getStrip(0));
     ccache->nodes.load(acceleration, cpu_nodes.begin(), cpu_nodes.end());
 
     Data2D<T> cpu_support = [&](void)->Data2D<T>{
             const MultiIndexSet &work = (points.empty()) ? needed : points;
-            if (rule->getType() == rule_localp){
-                switch(order){
-                case 0: return encodeSupportForGPU<0, rule_localp, T>(work);
-                case 2: return encodeSupportForGPU<2, rule_localp, T>(work);
-                default:
-                    return encodeSupportForGPU<1, rule_localp, T>(work);
-                }
-            }else if (rule->getType() == rule_semilocalp){
-                return encodeSupportForGPU<2, rule_semilocalp, T>(work);
-            }else if (rule->getType() == rule_localpb){
-                switch(order){
-                case 2: return encodeSupportForGPU<2, rule_localpb, T>(work);
-                default:
-                    return encodeSupportForGPU<1, rule_localpb, T>(work);
-                }
-            }else{
-                switch(order){
-                case 2: return encodeSupportForGPU<2, rule_localp0, T>(work);
-                default:
-                    return encodeSupportForGPU<1, rule_localp0, T>(work);
-                }
-            }
+            switch(effective_rule) {
+                case RuleLocal::erule::pwc:
+                    return encodeSupportForGPU<0, rule_localp, T>(work);
+                case RuleLocal::erule::localp:
+                    return (order == 1) ? encodeSupportForGPU<1, rule_localp, T>(work)
+                                        : encodeSupportForGPU<2, rule_localp, T>(work);
+                case RuleLocal::erule::semilocalp:
+                    return (order == 1) ? encodeSupportForGPU<1, rule_semilocalp, T>(work)
+                                        : encodeSupportForGPU<2, rule_semilocalp, T>(work);
+                case RuleLocal::erule::localp0:
+                    return (order == 1) ? encodeSupportForGPU<1, rule_localp0, T>(work)
+                                        : encodeSupportForGPU<2, rule_localp0, T>(work);
+                default: // case RuleLocal::erule::localpb:
+                    return (order == 1) ? encodeSupportForGPU<1, rule_localpb, T>(work)
+                                        : encodeSupportForGPU<2, rule_localpb, T>(work);
+            };
         }();
     ccache->support.load(acceleration, cpu_support.begin(), cpu_support.end());
 }
 void GridLocalPolynomial::clearGpuBasisHierarchy(){
     if (gpu_cache) gpu_cache->clearBasisHierarchy();
     if (gpu_cachef) gpu_cachef->clearBasisHierarchy();
 }
@@ -448,18 +504,19 @@
 }
 void GridLocalPolynomial::readConstructionData(std::istream &is, bool iomode){
     if (iomode == mode_ascii)
         dynamic_values = Utils::make_unique<SimpleConstructData>(is, num_dimensions, num_outputs, IO::mode_ascii_type());
     else
         dynamic_values = Utils::make_unique<SimpleConstructData>(is, num_dimensions, num_outputs, IO::mode_binary_type());
 }
+template<RuleLocal::erule effrule>
 std::vector<double> GridLocalPolynomial::getCandidateConstructionPoints(double tolerance, TypeRefinement criteria, int output,
                                                                         std::vector<int> const &level_limits, double const *scale_correction){
     // combine the initial points with negative weights and the refinement candidates with surplus weights (no need to normalize, the sort uses relative values)
-    MultiIndexSet refine_candidates = getRefinementCanidates(tolerance, criteria, output, level_limits, scale_correction);
+    MultiIndexSet refine_candidates = getRefinementCanidates<effrule>(tolerance, criteria, output, level_limits, scale_correction);
     MultiIndexSet new_points = (dynamic_values->initial_points.empty()) ? std::move(refine_candidates) : refine_candidates - dynamic_values->initial_points;
 
     // compute the weights for the new_points points
     std::vector<double> norm = getNormalization();
 
     int active_outputs = (output == -1) ? num_outputs : 1;
     Utils::Wrapper2D<double const> scale(active_outputs, scale_correction);
@@ -484,190 +541,243 @@
     std::vector<double> refine_weights(new_points.getNumIndexes());
 
     #pragma omp parallel for
     for(int i=0; i<new_points.getNumIndexes(); i++){
         double weight = 0.0;
         std::vector<int> p = new_points.copyIndex(i);
 
-        HierarchyManipulations::touchAllImmediateRelatives(p, points, rule.get(),
-                                                            [&](int relative)->void{ weight = std::max(weight, getDominantSurplus(relative)); });
+        HierarchyManipulations::touchAllImmediateRelatives<effrule>(p, points,
+                [&](int relative)->void{ weight = std::max(weight, getDominantSurplus(relative)); });
         refine_weights[i] = weight; // those will be inverted
     }
 
     // if using stable refinement, ensure the weight of the parents is never less than the children
     if (!new_points.empty() && ((criteria == refine_parents_first) || (criteria == refine_fds))){
-        auto rlevels = HierarchyManipulations::computeLevels(new_points, rule.get());
+        auto rlevels = HierarchyManipulations::computeLevels<effrule>(new_points);
         auto split = HierarchyManipulations::splitByLevels(new_points, rlevels);
         for(auto is = split.rbegin(); is != split.rend(); is++){
             for(int i=0; i<is->getNumStrips(); i++){
                 std::vector<int> parent(is->getStrip(i), is->getStrip(i) + num_dimensions);
                 double correction = refine_weights[new_points.getSlot(parent)]; // will never be missing
                 for(auto &p : parent){
                     int r = p;
-                    p = rule->getParent(r);
+                    p = RuleLocal::getParent<effrule>(r);
                     int ip = (p == -1) ? -1 : new_points.getSlot(parent); // if parent is among the refined
                     if (ip != -1) refine_weights[ip] += correction;
-                    p = rule->getStepParent(r);
+                    p = RuleLocal::getStepParent<effrule>(r);
                     ip = (p == -1) ? -1 : new_points.getSlot(parent); // if parent is among the refined
                     if (ip != -1) refine_weights[ip] += correction;
                     p = r;
                 }
             }
         }
     }else if (!new_points.empty() && (criteria == refine_stable)){
         // stable refinement, ensure that if level[i] < level[j] then weight[i] > weight[j]
-        auto rlevels = HierarchyManipulations::computeLevels(new_points, rule.get());
+        auto rlevels = HierarchyManipulations::computeLevels<effrule>(new_points);
         auto split = HierarchyManipulations::splitByLevels(new_points, rlevels);
         double max_weight = 0.0;
         for(auto is = split.rbegin(); is != split.rend(); is++){ // loop backwards in levels
             double correction = max_weight;
             for(int i=0; i<is->getNumStrips(); i++){
                 int idx = new_points.getSlot(std::vector<int>(is->getStrip(i), is->getStrip(i) + num_dimensions));
                 refine_weights[idx] += correction;
                 max_weight = std::max(max_weight, refine_weights[idx]);
             }
         }
     }
 
     // compute the weights for the initial points
-    std::vector<int> initial_levels = HierarchyManipulations::computeLevels(dynamic_values->initial_points, rule.get());
+    std::vector<int> initial_levels = HierarchyManipulations::computeLevels<effrule>(dynamic_values->initial_points);
 
     std::forward_list<NodeData> weighted_points;
     for(int i=0; i<dynamic_values->initial_points.getNumIndexes(); i++)
         weighted_points.push_front({dynamic_values->initial_points.copyIndex(i), {-1.0 / ((double) initial_levels[i])}});
     for(int i=0; i<new_points.getNumIndexes(); i++)
         weighted_points.push_front({new_points.copyIndex(i), {1.0 / refine_weights[i]}});
 
     // sort and return the sorted list
     weighted_points.sort([&](const NodeData &a, const NodeData &b)->bool{ return (a.value[0] < b.value[0]); });
 
-    return listToNodes(weighted_points, num_dimensions, *rule);
+    return listToLocalNodes(weighted_points, num_dimensions, [&](int i)->double{ return RuleLocal::getNode<effrule>(i); });
 }
+std::vector<double> GridLocalPolynomial::getCandidateConstructionPoints(double tolerance, TypeRefinement criteria, int output,
+                                                                        std::vector<int> const &level_limits, double const *scale_correction) {
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            return getCandidateConstructionPoints<RuleLocal::erule::pwc>(tolerance, criteria, output, level_limits, scale_correction);
+        case RuleLocal::erule::localp:
+            return getCandidateConstructionPoints<RuleLocal::erule::localp>(tolerance, criteria, output, level_limits, scale_correction);
+        case RuleLocal::erule::semilocalp:
+            return getCandidateConstructionPoints<RuleLocal::erule::semilocalp>(tolerance, criteria, output, level_limits, scale_correction);
+        case RuleLocal::erule::localp0:
+            return getCandidateConstructionPoints<RuleLocal::erule::localp0>(tolerance, criteria, output, level_limits, scale_correction);
+        default: // case RuleLocal::erule::localpb:
+            return getCandidateConstructionPoints<RuleLocal::erule::localpb>(tolerance, criteria, output, level_limits, scale_correction);
+    };
+}
+
+template<RuleLocal::erule effrule>
 std::vector<int> GridLocalPolynomial::getMultiIndex(const double x[]){
     std::vector<int> p(num_dimensions); // convert x to p, maybe expensive
     for(int j=0; j<num_dimensions; j++){
         int i = 0;
-        while(std::abs(rule->getNode(i) - x[j]) > Maths::num_tol) i++;
+        while(std::abs(RuleLocal::getNode<effrule>(i) - x[j]) > Maths::num_tol) i++;
         p[j] = i;
     }
     return p;
 }
+
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::loadConstructedPoint(const double x[], const std::vector<double> &y){
-    auto p = getMultiIndex(x);
+    auto p = getMultiIndex<effrule>(x);
 
     dynamic_values->initial_points.removeIndex(p);
 
     bool isConnected = false;
-    HierarchyManipulations::touchAllImmediateRelatives(p, points, rule.get(),
-                                                       [&](int)->void{ isConnected = true; });
-    int lvl = rule->getLevel(p[0]);
-    for(int j=1; j<num_dimensions; j++) lvl += rule->getLevel(p[j]);
+    HierarchyManipulations::touchAllImmediateRelatives<effrule>(p, points, [&](int)->void{ isConnected = true; });
+    int lvl = RuleLocal::getLevel<effrule>(p[0]);
+    for(int j=1; j<num_dimensions; j++) lvl += RuleLocal::getLevel<effrule>(p[j]);
 
     if (isConnected || (lvl == 0)){
-        expandGrid(p, y);
-        loadConstructedPoints();
+        expandGrid<effrule>(p, y);
+        loadConstructedPoints<effrule>();
     }else{
         dynamic_values->data.push_front({p, y});
     }
 }
+void GridLocalPolynomial::loadConstructedPoint(const double x[], const std::vector<double> &y){
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            return loadConstructedPoint<RuleLocal::erule::pwc>(x, y);
+        case RuleLocal::erule::localp:
+            return loadConstructedPoint<RuleLocal::erule::localp>(x, y);
+        case RuleLocal::erule::semilocalp:
+            return loadConstructedPoint<RuleLocal::erule::semilocalp>(x, y);
+        case RuleLocal::erule::localp0:
+            return loadConstructedPoint<RuleLocal::erule::localp0>(x, y);
+        default: // case RuleLocal::erule::localpb:
+            return loadConstructedPoint<RuleLocal::erule::localpb>(x, y);
+    };
+}
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::expandGrid(const std::vector<int> &point, const std::vector<double> &value){
     if (points.empty()){ // only one point
         points = MultiIndexSet((size_t) num_dimensions, std::vector<int>(point));
         values = StorageSet(num_outputs, 1, std::vector<double>(value));
         surpluses = Data2D<double>(num_outputs, 1, std::vector<double>(value)); // one value is its own surplus
     }else{ // merge with existing points
         // compute the surplus for the point
-        std::vector<double> xnode = MultiIndexManipulations::getIndexesToNodes(point, *rule);
+        std::vector<double> xnode(num_dimensions);
+        for(int j=0; j<num_dimensions; j++)
+            xnode[j] = RuleLocal::getNode<effrule>(point[j]);
+
         std::vector<double> approximation(num_outputs), surp(num_outputs);
         evaluate(xnode.data(), approximation.data());
         std::transform(approximation.begin(), approximation.end(), value.begin(), surp.begin(), [&](double e, double v)->double{ return v - e; });
 
-        std::vector<int> graph = getSubGraph(point); // get the descendant nodes that must be updated later
+        std::vector<int> graph = getSubGraph<effrule>(point); // get the descendant nodes that must be updated later
 
         values.addValues(points, MultiIndexSet(num_dimensions, std::vector<int>(point)), value.data()); // added the value
 
         points.addSortedIndexes(point); // add the point
         int newindex = points.getSlot(point);
         surpluses.appendStrip(newindex, surp); // find the index of the new point
 
         for(auto &g : graph) if (g >= newindex) g++; // all points belowe the newindex have been shifted down by one spot
 
         std::vector<int> levels(points.getNumIndexes(), 0); // compute the levels, but only for the new indexes
         for(auto &g : graph){
             int const *pnt = points.getIndex(g);
-            int l = rule->getLevel(pnt[0]);
-            for(int j=1; j<num_dimensions; j++) l += rule->getLevel(pnt[j]);
+            int l = RuleLocal::getLevel<effrule>(pnt[0]);
+            for(int j=1; j<num_dimensions; j++) l += RuleLocal::getLevel<effrule>(pnt[j]);
             levels[g] = l;
 
             std::copy_n(values.getValues(g), num_outputs, surpluses.getStrip(g)); // reset the surpluses to the values (will be updated)
         }
 
         // compute the current DAG and update the surplused for the descendants
-        updateSurpluses(points, top_level + 1, levels, HierarchyManipulations::computeDAGup(points, rule.get()));
+        updateSurpluses<effrule>(points, top_level + 1, levels, HierarchyManipulations::computeDAGup<effrule>(points));
     }
     buildTree(); // the tree is needed for evaluate(), must be rebuild every time the points set is updated
 }
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::loadConstructedPoint(const double x[], int numx, const double y[]){
     Utils::Wrapper2D<const double> wrapx(num_dimensions, x);
     std::vector<std::vector<int>> pnts(numx);
     #pragma omp parallel for
     for(int i=0; i<numx; i++)
-        pnts[i] = getMultiIndex(wrapx.getStrip(i));
+        pnts[i] = getMultiIndex<effrule>(wrapx.getStrip(i));
 
     if (!dynamic_values->initial_points.empty()){
         Data2D<int> combined_pnts(num_dimensions, numx);
         for(int i=0; i<numx; i++)
             std::copy_n(pnts[i].begin(), num_dimensions, combined_pnts.getIStrip(i));
         dynamic_values->initial_points = dynamic_values->initial_points - combined_pnts;
     }
 
     Utils::Wrapper2D<const double> wrapy(num_outputs, y);
     for(int i=0; i<numx; i++)
         dynamic_values->data.push_front({std::move(pnts[i]), std::vector<double>(wrapy.getStrip(i), wrapy.getStrip(i) + num_outputs)});
 
-    loadConstructedPoints();
+    loadConstructedPoints<effrule>();
 }
+void GridLocalPolynomial::loadConstructedPoint(const double x[], int numx, const double y[]){
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            return loadConstructedPoint<RuleLocal::erule::pwc>(x, numx, y);
+        case RuleLocal::erule::localp:
+            return loadConstructedPoint<RuleLocal::erule::localp>(x, numx, y);
+        case RuleLocal::erule::semilocalp:
+            return loadConstructedPoint<RuleLocal::erule::semilocalp>(x, numx, y);
+        case RuleLocal::erule::localp0:
+            return loadConstructedPoint<RuleLocal::erule::localp0>(x, numx, y);
+        default: // case RuleLocal::erule::localpb:
+            return loadConstructedPoint<RuleLocal::erule::localpb>(x, numx, y);
+    };
+}
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::loadConstructedPoints(){
     Data2D<int> candidates(num_dimensions, (int) std::distance(dynamic_values->data.begin(), dynamic_values->data.end()));
     for(struct{ int i; std::forward_list<NodeData>::iterator d; } p = {0, dynamic_values->data.begin()};
         p.d != dynamic_values->data.end(); p.i++, p.d++){
         std::copy_n(p.d->point.begin(), num_dimensions, candidates.getIStrip(p.i));
     }
-    auto new_points = HierarchyManipulations::getLargestConnected(points, MultiIndexSet(candidates), rule.get());
+    auto new_points = HierarchyManipulations::getLargestConnected<effrule>(points, MultiIndexSet(candidates));
     if (new_points.empty()) return;
 
     clearGpuBasisHierarchy(); // the points will change, clear the cache
     clearGpuSurpluses();
 
     auto vals = dynamic_values->extractValues(new_points);
     if (points.empty()){
         points = std::move(new_points);
         values.setValues(std::move(vals));
     }else{
         values.addValues(points, new_points, vals.data());
         points += new_points;
     }
     buildTree();
-    recomputeSurpluses(); // costly, but the only option under the circumstances
+    recomputeSurpluses<effrule>(); // costly, but the only option under the circumstances
 }
 void GridLocalPolynomial::finishConstruction(){ dynamic_values.reset(); }
 
+template<RuleLocal::erule effrule>
 std::vector<int> GridLocalPolynomial::getSubGraph(std::vector<int> const &point) const{
     std::vector<int> graph, p = point;
     std::vector<bool> used(points.getNumIndexes(), false);
-    int max_1d_kids = rule->getMaxNumKids();
+    int max_1d_kids = RuleLocal::getMaxNumKids<effrule>();
     int max_kids = max_1d_kids * num_dimensions;
 
     std::vector<int> monkey_count(1, 0), monkey_tail;
 
     while(monkey_count[0] < max_kids){
         if (monkey_count.back() < max_kids){
             int dim = monkey_count.back() / max_1d_kids;
             monkey_tail.push_back(p[dim]);
-            p[dim] = rule->getKid(monkey_tail.back(), monkey_count.back() % max_1d_kids);
+            p[dim] = RuleLocal::getKid<effrule>(monkey_tail.back(), monkey_count.back() % max_1d_kids);
             int slot = points.getSlot(p);
             if ((slot == -1) || used[slot]){ // this kid is missing
                 p[dim] = monkey_tail.back();
                 monkey_tail.pop_back();
                 monkey_count.back()++;
             }else{ // found kid, go deeper in the graph
                 graph.push_back(slot);
@@ -717,25 +827,70 @@
 }
 
 void GridLocalPolynomial::evaluateHierarchicalFunctions(const double x[], int num_x, double y[]) const{
     const MultiIndexSet &work = (points.empty()) ? needed : points;
     int num_points = work.getNumIndexes();
     Utils::Wrapper2D<double const> xwrap(num_dimensions, x);
     Utils::Wrapper2D<double> ywrap(num_points, y);
-    #pragma omp parallel for
-    for(int i=0; i<num_x; i++){
-        double const *this_x = xwrap.getStrip(i);
-        double *this_y = ywrap.getStrip(i);
-        bool dummy;
-        for(int j=0; j<num_points; j++)
-            this_y[j] = evalBasisSupported(work.getIndex(j), this_x, dummy);
-    }
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            #pragma omp parallel for
+            for(int i=0; i<num_x; i++){
+                double const *this_x = xwrap.getStrip(i);
+                double *this_y = ywrap.getStrip(i);
+                bool dummy;
+                for(int j=0; j<num_points; j++)
+                    this_y[j] = evalBasisSupported<RuleLocal::erule::pwc>(work.getIndex(j), this_x, dummy);
+            }
+            break;
+        case RuleLocal::erule::localp:
+            #pragma omp parallel for
+            for(int i=0; i<num_x; i++){
+                double const *this_x = xwrap.getStrip(i);
+                double *this_y = ywrap.getStrip(i);
+                bool dummy;
+                for(int j=0; j<num_points; j++)
+                    this_y[j] = evalBasisSupported<RuleLocal::erule::localp>(work.getIndex(j), this_x, dummy);
+            }
+            break;
+        case RuleLocal::erule::semilocalp:
+            #pragma omp parallel for
+            for(int i=0; i<num_x; i++){
+                double const *this_x = xwrap.getStrip(i);
+                double *this_y = ywrap.getStrip(i);
+                bool dummy;
+                for(int j=0; j<num_points; j++)
+                    this_y[j] = evalBasisSupported<RuleLocal::erule::semilocalp>(work.getIndex(j), this_x, dummy);
+            }
+            break;
+        case RuleLocal::erule::localp0:
+            #pragma omp parallel for
+            for(int i=0; i<num_x; i++){
+                double const *this_x = xwrap.getStrip(i);
+                double *this_y = ywrap.getStrip(i);
+                bool dummy;
+                for(int j=0; j<num_points; j++)
+                    this_y[j] = evalBasisSupported<RuleLocal::erule::localp0>(work.getIndex(j), this_x, dummy);
+            }
+            break;
+        default: // case RuleLocal::erule::localpb:
+            #pragma omp parallel for
+            for(int i=0; i<num_x; i++){
+                double const *this_x = xwrap.getStrip(i);
+                double *this_y = ywrap.getStrip(i);
+                bool dummy;
+                for(int j=0; j<num_points; j++)
+                    this_y[j] = evalBasisSupported<RuleLocal::erule::localpb>(work.getIndex(j), this_x, dummy);
+            }
+            break;
+    };
 }
 
-void GridLocalPolynomial::recomputeSurpluses(){
+template<RuleLocal::erule effrule>
+void GridLocalPolynomial::recomputeSurpluses() {
     surpluses = Data2D<double>(num_outputs, points.getNumIndexes(), std::vector<double>(values.begin(), values.end()));
 
     // There are two available algorithms here:
     // - global sparse Kronecker (kron), implemented here in recomputeSurpluses()
     // - sparse matrix in matrix-free form (mat), implemented in updateSurpluses()
     //
     // (kron) has the additional restriction that it will only work when the hierarchy is complete
@@ -759,35 +914,35 @@
     //            the breaking point depends on n, the order and system
     // for d = 4 and above, the (kron) algorithm is much faster
     //           it is possible that for sufficiently large n (mat) will win again
     //           but tested on 12 cores CPUs (Intel and AMD) up to n = 3.5 million, the (kron) method is over 2x faster
     // higher dimensions will favor (kron) even more
 
     if (num_dimensions <= 2 or (num_dimensions == 3 and points.getNumIndexes() > 2000000)) {
-        Data2D<int> dagUp = HierarchyManipulations::computeDAGup(points, rule.get());
-        std::vector<int> level = HierarchyManipulations::computeLevels(points, rule.get());
-        updateSurpluses(points, top_level, level, dagUp);
+        Data2D<int> dagUp = HierarchyManipulations::computeDAGup<effrule>(points);
+        std::vector<int> level = HierarchyManipulations::computeLevels<effrule>(points);
+        updateSurpluses<effrule>(points, top_level, level, dagUp);
         return;
     }
 
     bool is_complete = true;
-    Data2D<int> dagUp = HierarchyManipulations::computeDAGup(points, rule.get(), is_complete);
+    Data2D<int> dagUp = HierarchyManipulations::computeDAGup<effrule>(points, is_complete);
 
     if (not is_complete) {
         // incomplete hierarchy, must use the slow algorithm
-        std::vector<int> level = HierarchyManipulations::computeLevels(points, rule.get());
-        updateSurpluses(points, top_level, level, dagUp);
+        std::vector<int> level = HierarchyManipulations::computeLevels<effrule>(points);
+        updateSurpluses<effrule>(points, top_level, level, dagUp);
         return;
     }
 
     int num_nodes = 1 + *std::max_element(points.begin(), points.end());
 
     std::vector<int> vpntr, vindx;
     std::vector<double> vvals;
-    rule->van_matrix(num_nodes, vpntr, vindx, vvals);
+    RuleLocal::van_matrix<effrule>(order, num_nodes, vpntr, vindx, vvals);
 
     std::vector<std::vector<int>> map;
     std::vector<std::vector<int>> lines1d;
     MultiIndexManipulations::resortIndexes(points, map, lines1d);
 
     for(int d=num_dimensions-1; d>=0; d--) {
         #pragma omp parallel for schedule(dynamic)
@@ -819,108 +974,143 @@
                     }
                 }
             }
         }
     }
 }
 
+void GridLocalPolynomial::recomputeSurpluses() {
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            recomputeSurpluses<RuleLocal::erule::pwc>();
+            break;
+        case RuleLocal::erule::localp:
+            recomputeSurpluses<RuleLocal::erule::localp>();
+            break;
+        case RuleLocal::erule::semilocalp:
+            recomputeSurpluses<RuleLocal::erule::semilocalp>();
+            break;
+        case RuleLocal::erule::localp0:
+            recomputeSurpluses<RuleLocal::erule::localp0>();
+            break;
+        default: // case RuleLocal::erule::localpb:
+            recomputeSurpluses<RuleLocal::erule::localpb>();
+            break;
+    };
+}
+
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::updateSurpluses(MultiIndexSet const &work, int max_level, std::vector<int> const &level, Data2D<int> const &dagUp){
     int num_points = work.getNumIndexes();
-    int max_parents = num_dimensions * rule->getMaxNumParents();
+    int max_parents = num_dimensions * RuleLocal::getMaxNumParents<effrule>();
 
     std::vector<std::vector<int>> indexses_for_levels((size_t) max_level+1);
     for(int i=0; i<num_points; i++)
         if (level[i] > 0) indexses_for_levels[level[i]].push_back(i);
 
     for(int l=1; l<=max_level; l++){
         int level_size = (int) indexses_for_levels[l].size();
-        #pragma omp parallel for schedule(dynamic)
-        for(int s=0; s<level_size; s++){
-            int i = indexses_for_levels[l][s];
-
-            std::vector<double> x = MultiIndexManipulations::getIndexesToNodes(work.getIndex(i), num_dimensions, *rule);
-            double *surpi = surpluses.getStrip(i);
+        #pragma omp parallel
+        {
+            std::vector<double> x(num_dimensions);
 
             std::vector<int> monkey_count(max_level + 1);
             std::vector<int> monkey_tail(max_level + 1);
             std::vector<bool> used(num_points, false);
 
-            int current = 0;
+            #pragma omp for schedule(dynamic)
+            for(int s=0; s<level_size; s++){
+                int i = indexses_for_levels[l][s];
+
+                int const *pnt = work.getIndex(i);
+                for(int j=0; j<num_dimensions; j++)
+                    x[j] = RuleLocal::getNode<effrule>(pnt[j]);
 
-            monkey_count[0] = 0;
-            monkey_tail[0] = i;
+                std::fill(used.begin(), used.end(), false);
 
-            while(monkey_count[0] < max_parents){
-                if (monkey_count[current] < max_parents){
-                    int branch = dagUp.getStrip(monkey_tail[current])[monkey_count[current]];
-                    if ((branch == -1) || (used[branch])){
-                        monkey_count[current]++;
-                    }else{
-                        const double *branch_surp = surpluses.getStrip(branch);
-                        double basis_value = evalBasisRaw(work.getIndex(branch), x.data());
-                        for(int k=0; k<num_outputs; k++)
-                            surpi[k] -= basis_value * branch_surp[k];
-                        used[branch] = true;
+                double *surpi = surpluses.getStrip(i);
+
+                int current = 0;
 
-                        monkey_count[++current] = 0;
-                        monkey_tail[current] = branch;
+                monkey_count[0] = 0;
+                monkey_tail[0] = i;
+
+                while(monkey_count[0] < max_parents){
+                    if (monkey_count[current] < max_parents){
+                        int branch = dagUp.getStrip(monkey_tail[current])[monkey_count[current]];
+                        if ((branch == -1) || (used[branch])){
+                            monkey_count[current]++;
+                        }else{
+                            const double *branch_surp = surpluses.getStrip(branch);
+                            double basis_value = evalBasisRaw<effrule>(work.getIndex(branch), x.data());
+                            for(int k=0; k<num_outputs; k++)
+                                surpi[k] -= basis_value * branch_surp[k];
+                            used[branch] = true;
+
+                            monkey_count[++current] = 0;
+                            monkey_tail[current] = branch;
+                        }
+                    }else{
+                        monkey_count[--current]++;
                     }
-                }else{
-                    monkey_count[--current]++;
                 }
-            }
-        }
-    }
+            } // for-loop
+        } // omp parallel
+    } // level loop
 }
 
-template<int mode>
+template<int mode, RuleLocal::erule effrule>
 void GridLocalPolynomial::applyTransformationTransposed(double weights[], const MultiIndexSet &work, const std::vector<int> &active_points) const {
     Data2D<int> lparents = (parents.getNumStrips() != work.getNumIndexes()) ? // if the current dag loaded in parents does not reflect the indexes in work
-                            HierarchyManipulations::computeDAGup(work, rule.get()) :
+                            HierarchyManipulations::computeDAGup<effrule>(work) :
                             Data2D<int>();
 
     const Data2D<int> &dagUp = (parents.getNumStrips() != work.getNumIndexes()) ? lparents : parents;
 
     std::vector<int> level(active_points.size());
     int active_top_level = 0;
     for(size_t i=0; i<active_points.size(); i++){
         const int *p = work.getIndex(active_points[i]);
-        int current_level = rule->getLevel(p[0]);
+        int current_level = RuleLocal::getLevel<effrule>(p[0]);
         for(int j=1; j<num_dimensions; j++){
-            current_level += rule->getLevel(p[j]);
+            current_level += RuleLocal::getLevel<effrule>(p[j]);
         }
         if (active_top_level < current_level) active_top_level = current_level;
         level[i] = current_level;
     }
 
     std::vector<int> monkey_count(top_level+1);
     std::vector<int> monkey_tail(top_level+1);
     std::vector<bool> used(work.getNumIndexes());
-    int max_parents = rule->getMaxNumParents() * num_dimensions;
+    int max_parents = RuleLocal::getMaxNumParents<effrule>() * num_dimensions;
+
+    std::vector<double> node(num_dimensions);
 
     for(int l=active_top_level; l>0; l--){
         for(size_t i=0; i<active_points.size(); i++){
             if (level[i] == l){
-                std::vector<double> node = MultiIndexManipulations::getIndexesToNodes(work.getIndex(active_points[i]), num_dimensions, *rule);
+                int const *pnt = work.getIndex(active_points[i]);
+                for(int j=0; j<num_dimensions; j++)
+                    node[j] = RuleLocal::getNode<effrule>(pnt[j]);
 
                 std::fill(used.begin(), used.end(), false);
 
                 monkey_count[0] = 0;
                 monkey_tail[0] = active_points[i];
                 int current = 0;
 
                 while(monkey_count[0] < max_parents){
                     if (monkey_count[current] < max_parents){
                         int branch = dagUp.getStrip(monkey_tail[current])[monkey_count[current]];
                         if ((branch == -1) || used[branch]){
                             monkey_count[current]++;
                         }else{
                             const int *func = work.getIndex(branch);
-                            double basis_value = rule->evalRaw(func[0], node[0]);
-                            for(int j=1; j<num_dimensions; j++) basis_value *= rule->evalRaw(func[j], node[j]);
+                            double basis_value = RuleLocal::evalRaw<effrule>(order, func[0], node[0]);
+                            for(int j=1; j<num_dimensions; j++) basis_value *= RuleLocal::evalRaw<effrule>(order, func[j], node[j]);
 
                             if (mode == 0) {
                                 weights[branch] -= weights[active_points[i]] * basis_value;
                             } else {
                                 for (int d=0; d<num_dimensions; d++)
                                     weights[branch * num_dimensions + d] -=
                                             weights[active_points[i] * num_dimensions + d] * basis_value;
@@ -935,43 +1125,33 @@
                     }
                 }
             }
         }
     }
 }
 
-double GridLocalPolynomial::evalBasisRaw(const int point[], const double x[]) const{
-    double f = rule->evalRaw(point[0], x[0]);
-    for(int j=1; j<num_dimensions; j++) f *= rule->evalRaw(point[j], x[j]);
-    return f;
-}
-double GridLocalPolynomial::evalBasisSupported(const int point[], const double x[], bool &isSupported) const{
-    double f = rule->evalSupport(point[0], x[0], isSupported);
-    if (!isSupported) return 0.0;
-    for(int j=1; j<num_dimensions; j++){
-        f *= rule->evalSupport(point[j], x[j], isSupported);
-        if (!isSupported) return 0.0;
-    }
-    return f;
-}
-
-void GridLocalPolynomial::diffBasisSupported(const int point[], const double x[], double diff_values[], bool &isSupported) const{
-    isSupported = false;
-    for(int i=0; i<num_dimensions; i++) diff_values[i] = 1.0;
-    bool isDimSupported = false;
-    for(int k=0; k<num_dimensions; k++) {
-        double fval = rule->evalSupport(point[k], x[k], isDimSupported);
-        isSupported = isDimSupported or isSupported;
-        for(int j=0; j<k; j++) diff_values[j] *= fval;
-        for(int j=k+1; j<num_dimensions; j++) diff_values[j] *= fval;
-    }
-    for (int k=0; k<num_dimensions; k++) {
-        diff_values[k] *= rule->diffSupport(point[k], x[k], isDimSupported);
-        isSupported = isDimSupported or isSupported;
-    }
+template<int mode>
+void GridLocalPolynomial::applyTransformationTransposed(double weights[], const MultiIndexSet &work, const std::vector<int> &active_points) const {
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            applyTransformationTransposed<mode, RuleLocal::erule::pwc>(weights, work, active_points);
+            break;
+        case RuleLocal::erule::localp:
+            applyTransformationTransposed<mode, RuleLocal::erule::localp>(weights, work, active_points);
+            break;
+        case RuleLocal::erule::semilocalp:
+            applyTransformationTransposed<mode, RuleLocal::erule::semilocalp>(weights, work, active_points);
+            break;
+        case RuleLocal::erule::localp0:
+            applyTransformationTransposed<mode, RuleLocal::erule::localp0>(weights, work, active_points);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            applyTransformationTransposed<mode, RuleLocal::erule::localpb>(weights, work, active_points);
+            break;
+    };
 }
 
 void GridLocalPolynomial::buildSpareBasisMatrix(const double x[], int num_x, int num_chunk, std::vector<int> &spntr, std::vector<int> &sindx, std::vector<double> &svals) const{
     std::vector<std::vector<int>> tindx;
     std::vector<std::vector<double>> tvals;
     std::vector<int> numnz;
     buildSparseMatrixBlockForm(x, num_x, num_chunk, numnz, tindx, tvals);
@@ -1054,18 +1234,40 @@
     }
 }
 
 void GridLocalPolynomial::buildTree(){
     const MultiIndexSet &work = (points.empty()) ? needed : points;
     int num_points = work.getNumIndexes();
 
-    std::vector<int> level = HierarchyManipulations::computeLevels(work, rule.get());
-    top_level = *std::max_element(level.begin(), level.end());
+    Data2D<int> kids;
+    std::vector<int> level;
 
-    Data2D<int> kids = HierarchyManipulations::computeDAGDown(work, rule.get());
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            kids = HierarchyManipulations::computeDAGDown<RuleLocal::erule::pwc>(work);
+            level = HierarchyManipulations::computeLevels<RuleLocal::erule::pwc>(work);
+            break;
+        case RuleLocal::erule::localp:
+            kids = HierarchyManipulations::computeDAGDown<RuleLocal::erule::localp>(work);
+            level = HierarchyManipulations::computeLevels<RuleLocal::erule::localp>(work);
+            break;
+        case RuleLocal::erule::semilocalp:
+            kids = HierarchyManipulations::computeDAGDown<RuleLocal::erule::semilocalp>(work);
+            level = HierarchyManipulations::computeLevels<RuleLocal::erule::semilocalp>(work);
+            break;
+        case RuleLocal::erule::localp0:
+            kids = HierarchyManipulations::computeDAGDown<RuleLocal::erule::localp0>(work);
+            level = HierarchyManipulations::computeLevels<RuleLocal::erule::localp0>(work);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            kids = HierarchyManipulations::computeDAGDown<RuleLocal::erule::localpb>(work);
+            level = HierarchyManipulations::computeLevels<RuleLocal::erule::localpb>(work);
+            break;
+    };
+    top_level = *std::max_element(level.begin(), level.end());
 
     int max_kids = (int) kids.getStride();
 
     Data2D<int> tree(max_kids, num_points, -1);
     std::vector<bool> free(num_points, true);
 
     std::vector<int> monkey_count((size_t) (top_level + 1));
@@ -1116,78 +1318,144 @@
     std::copy_if(tree.begin(), tree.end(), indx.begin(), [](int t)->bool{ return (t > -1); });
 }
 
 void GridLocalPolynomial::integrateHierarchicalFunctions(double integrals[]) const{
     const MultiIndexSet &work = (points.empty()) ? needed : points;
 
     std::vector<double> w, x;
-    if ((rule->getMaxOrder() == -1) || (rule->getMaxOrder() > 3) )
-        OneDimensionalNodes::getGaussLegendre(((rule->getMaxOrder() == -1) ? top_level : rule->getMaxOrder()) / 2 + 1, w, x);
+    if (order == -1 or order > 3)
+        OneDimensionalNodes::getGaussLegendre(((order == -1) ? top_level : order) / 2 + 1, w, x);
 
-    for(int i=0; i<work.getNumIndexes(); i++){
-        const int* p = work.getIndex(i);
-        integrals[i] = rule->getArea(p[0], w, x);
-        for(int j=1; j<num_dimensions; j++)
-            integrals[i] *= rule->getArea(p[j], w, x);
-    }
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            #pragma omp parallel for
+            for(int i=0; i<work.getNumIndexes(); i++){
+                const int* p = work.getIndex(i);
+                integrals[i] = RuleLocal::getArea<RuleLocal::erule::pwc>(order, p[0], w, x);
+                for(int j=1; j<num_dimensions; j++)
+                    integrals[i] *= RuleLocal::getArea<RuleLocal::erule::pwc>(order, p[j], w, x);
+            }
+            break;
+        case RuleLocal::erule::localp:
+            #pragma omp parallel for
+            for(int i=0; i<work.getNumIndexes(); i++){
+                const int* p = work.getIndex(i);
+                integrals[i] = RuleLocal::getArea<RuleLocal::erule::localp>(order, p[0], w, x);
+                for(int j=1; j<num_dimensions; j++)
+                    integrals[i] *= RuleLocal::getArea<RuleLocal::erule::localp>(order, p[j], w, x);
+            }
+            break;
+        case RuleLocal::erule::semilocalp:
+            #pragma omp parallel for
+            for(int i=0; i<work.getNumIndexes(); i++){
+                const int* p = work.getIndex(i);
+                integrals[i] = RuleLocal::getArea<RuleLocal::erule::semilocalp>(order, p[0], w, x);
+                for(int j=1; j<num_dimensions; j++)
+                    integrals[i] *= RuleLocal::getArea<RuleLocal::erule::semilocalp>(order, p[j], w, x);
+            }
+            break;
+        case RuleLocal::erule::localp0:
+            #pragma omp parallel for
+            for(int i=0; i<work.getNumIndexes(); i++){
+                const int* p = work.getIndex(i);
+                integrals[i] = RuleLocal::getArea<RuleLocal::erule::localp0>(order, p[0], w, x);
+                for(int j=1; j<num_dimensions; j++)
+                    integrals[i] *= RuleLocal::getArea<RuleLocal::erule::localp0>(order, p[j], w, x);
+            }
+            break;
+        default: // case RuleLocal::erule::localpb:
+            #pragma omp parallel for
+            for(int i=0; i<work.getNumIndexes(); i++){
+                const int* p = work.getIndex(i);
+                integrals[i] = RuleLocal::getArea<RuleLocal::erule::localpb>(order, p[0], w, x);
+                for(int j=1; j<num_dimensions; j++)
+                    integrals[i] *= RuleLocal::getArea<RuleLocal::erule::localpb>(order, p[j], w, x);
+            }
+            break;
+    };
 }
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::getQuadratureWeights(double *weights) const{
     const MultiIndexSet &work = (points.empty()) ? needed : points;
     integrateHierarchicalFunctions(weights);
 
     std::vector<int> monkey_count(top_level+1);
     std::vector<int> monkey_tail(top_level+1);
 
     double basis_value;
 
     Data2D<int> lparents;
     if (parents.getNumStrips() != work.getNumIndexes())
-        lparents = HierarchyManipulations::computeDAGup(work, rule.get());
+        lparents = HierarchyManipulations::computeDAGup<effrule>(work);
 
     const Data2D<int> &dagUp = (parents.getNumStrips() != work.getNumIndexes()) ? lparents : parents;
 
     int num_points = work.getNumIndexes();
-    std::vector<int> level = HierarchyManipulations::computeLevels(work, rule.get());
+    std::vector<int> level = HierarchyManipulations::computeLevels<effrule>(work);
 
-    int max_parents = rule->getMaxNumParents() * num_dimensions;
+    int max_parents = RuleLocal::getMaxNumParents<effrule>() * num_dimensions;
+
+    std::vector<double> node(num_dimensions);
+    std::vector<bool> used(work.getNumIndexes(), false);
 
     for(int l=top_level; l>0; l--){
         for(int i=0; i<num_points; i++){
             if (level[i] == l){
-                std::vector<double> node = MultiIndexManipulations::getIndexesToNodes(work.getIndex(i), num_dimensions, *rule);
+                int const *pnt = work.getIndex(i);
+                for(int j=0; j<num_dimensions; j++)
+                    node[j] = RuleLocal::getNode<effrule>(pnt[j]);
 
-                std::vector<bool> used(work.getNumIndexes(), false);
+                std::fill(used.begin(), used.end(), false);
 
                 monkey_count[0] = 0;
                 monkey_tail[0] = i;
                 int current = 0;
 
                 while(monkey_count[0] < max_parents){
                     if (monkey_count[current] < max_parents){
                         int branch = dagUp.getStrip(monkey_tail[current])[monkey_count[current]];
                         if ((branch == -1) || used[branch]){
                             monkey_count[current]++;
                         }else{
                             const int *func = work.getIndex(branch);
-                            basis_value = rule->evalRaw(func[0], node[0]);
-                            for(int j=1; j<num_dimensions; j++) basis_value *= rule->evalRaw(func[j], node[j]);
+                            basis_value = RuleLocal::evalRaw<effrule>(order, func[0], node[0]);
+                            for(int j=1; j<num_dimensions; j++) basis_value *= RuleLocal::evalRaw<effrule>(order, func[j], node[j]);
                             weights[branch] -= weights[i] * basis_value;
                             used[branch] = true;
 
                             monkey_count[++current] = 0;
                             monkey_tail[current] = branch;
                         }
                     }else{
                         monkey_count[--current]++;
                     }
                 }
             }
         }
     }
 }
+void GridLocalPolynomial::getQuadratureWeights(double *weights) const{
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            getQuadratureWeights<RuleLocal::erule::pwc>(weights);
+            break;
+        case RuleLocal::erule::localp:
+            getQuadratureWeights<RuleLocal::erule::localp>(weights);
+            break;
+        case RuleLocal::erule::semilocalp:
+            getQuadratureWeights<RuleLocal::erule::semilocalp>(weights);
+            break;
+        case RuleLocal::erule::localp0:
+            getQuadratureWeights<RuleLocal::erule::localp0>(weights);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            getQuadratureWeights<RuleLocal::erule::localpb>(weights);
+            break;
+    };
+}
 
 void GridLocalPolynomial::integrate(double q[], double *conformal_correction) const{
     int num_points = points.getNumIndexes();
     std::fill(q, q + num_outputs, 0.0);
 
     if (conformal_correction == 0){
         std::vector<double> integrals(num_points);
@@ -1223,14 +1491,15 @@
         for(int j=0; j<num_outputs; j++){
             if (norms[j] < std::abs(v[j])) norms[j] = std::abs(v[j]);
         }
     }
     return norms;
 }
 
+template<RuleLocal::erule effrule>
 Data2D<int> GridLocalPolynomial::buildUpdateMap(double tolerance, TypeRefinement criteria, int output, const double *scale_correction) const{
     int num_points = points.getNumIndexes();
     Data2D<int> pmap(num_dimensions, num_points,
                      std::vector<int>(Utils::size_mult(num_dimensions, num_points),
                                       (tolerance == 0.0) ? 1 : 0) // tolerance 0 means "refine everything"
                     );
     if (tolerance == 0.0) return pmap;
@@ -1257,17 +1526,17 @@
                 small = ((c[0] * std::abs(s[output]) / norm[output]) <= tolerance);
             }
             if (!small)
                 std::fill_n(pmap.getStrip(i), num_dimensions, 1);
         }
     }else{
         // construct a series of 1D interpolants and use a refinement criteria that is a combination of the two hierarchical coefficients
-        Data2D<int> dagUp = HierarchyManipulations::computeDAGup(points, rule.get());
+        Data2D<int> dagUp = HierarchyManipulations::computeDAGup<effrule>(points);
 
-        int max_1D_parents = rule->getMaxNumParents();
+        int max_1D_parents = RuleLocal::getMaxNumParents<effrule>();
 
         HierarchyManipulations::SplitDirections split(points);
 
         #pragma omp parallel
         {
             int max_nump = split.getMaxNumPoints();
             std::vector<int> global_to_pnts(num_points);
@@ -1292,64 +1561,64 @@
 
                 Data2D<double> vals(active_outputs, nump);
 
                 if (output == -1) {
                     for(int i=0; i<nump; i++){
                         std::copy_n(values.getValues(pnts[i]), num_outputs, vals.getStrip(i));
                         global_to_pnts[pnts[i]] = i;
-                        levels[i] = rule->getLevel(points.getIndex(pnts[i])[d]);
+                        levels[i] = RuleLocal::getLevel<effrule>(points.getIndex(pnts[i])[d]);
                         if (max_level < levels[i]) max_level = levels[i];
                     }
                 } else {
                     for(int i=0; i<nump; i++){
                         vals.getStrip(i)[0] = values.getValues(pnts[i])[output];
                         global_to_pnts[pnts[i]] = i;
-                        levels[i] = rule->getLevel(points.getIndex(pnts[i])[d]);
+                        levels[i] = RuleLocal::getLevel<effrule>(points.getIndex(pnts[i])[d]);
                         if (max_level < levels[i]) max_level = levels[i];
                     }
                 }
 
                 if (max_1D_parents == 1) {
                     for(int l=1; l<=max_level; l++){
                         for(int i=0; i<nump; i++){
                             if (levels[i] == l){
-                                double x = rule->getNode(points.getIndex(pnts[i])[d]);
+                                double x = RuleLocal::getNode<effrule>(points.getIndex(pnts[i])[d]);
                                 double *valsi = vals.getStrip(i);
 
                                 int branch = dagUp.getStrip(pnts[i])[d];
                                 while(branch != -1) {
                                     const int *branch_point = points.getIndex(branch);
-                                    double basis_value = rule->evalRaw(branch_point[d], x);
+                                    double basis_value = RuleLocal::evalRaw<effrule>(order, branch_point[d], x);
                                     const double *branch_vals = vals.getStrip(global_to_pnts[branch]);
                                     for(int k=0; k<active_outputs; k++) valsi[k] -= basis_value * branch_vals[k];
                                     branch = dagUp.getStrip(branch)[d];
                                 }
                             }
                         }
                     }
                 } else {
                     for(int l=1; l<=max_level; l++){
                         for(int i=0; i<nump; i++){
                             if (levels[i] == l){
-                                double x = rule->getNode(points.getIndex(pnts[i])[d]);
+                                double x = RuleLocal::getNode<effrule>(points.getIndex(pnts[i])[d]);
                                 double *valsi = vals.getStrip(i);
 
                                 int current = 0;
                                 monkey_count[0] = d * max_1D_parents;
                                 monkey_tail[0] = pnts[i]; // uses the global indexes
                                 std::fill_n(used.begin(), nump, false);
 
                                 while(monkey_count[0] < (d+1) * max_1D_parents){
                                     if (monkey_count[current] < (d+1) * max_1D_parents){
                                         int branch = dagUp.getStrip(monkey_tail[current])[monkey_count[current]];
                                         if ((branch == -1) || (used[global_to_pnts[branch]])){
                                             monkey_count[current]++;
                                         }else{
                                             const int *branch_point = points.getIndex(branch);
-                                            double basis_value = rule->evalRaw(branch_point[d], x);
+                                            double basis_value = RuleLocal::evalRaw<effrule>(order, branch_point[d], x);
                                             const double *branch_vals = vals.getStrip(global_to_pnts[branch]);
                                             for(int k=0; k<active_outputs; k++) valsi[k] -= basis_value * branch_vals[k];
 
                                             used[global_to_pnts[branch]] = true;
                                             monkey_count[++current] = d * max_1D_parents;
                                             monkey_tail[current] = branch;
                                         }
@@ -1378,16 +1647,17 @@
                     pmap.getStrip(pnts[i])[d] = (small) ? 0 : 1;;
                 }
             }
         }
     }
     return pmap;
 }
+template<RuleLocal::erule effrule>
 MultiIndexSet GridLocalPolynomial::getRefinementCanidates(double tolerance, TypeRefinement criteria, int output, const std::vector<int> &level_limits, const double *scale_correction) const{
-    Data2D<int> pmap = buildUpdateMap(tolerance, criteria, output, scale_correction);
+    Data2D<int> pmap = buildUpdateMap<effrule>(tolerance, criteria, output, scale_correction);
 
     bool useParents = (criteria == refine_fds) || (criteria == refine_parents_first);
 
     Data2D<int> refined(num_dimensions, 0);
 
     int num_points = points.getNumIndexes();
 
@@ -1398,28 +1668,28 @@
 
         if (level_limits.empty()){
             #pragma omp for
             for(int i=0; i<num_points; i++){
                 const int *map = pmap.getStrip(i);
                 for(int j=0; j<num_dimensions; j++){
                     if (map[j] == 1){ // if this dimension needs to be refined
-                        if (!(useParents && addParent(points.getIndex(i), j, points, lrefined))){
-                            addChild(points.getIndex(i), j, points, lrefined);
+                        if (!(useParents && addParent<effrule>(points.getIndex(i), j, points, lrefined))){
+                            addChild<effrule>(points.getIndex(i), j, points, lrefined);
                         }
                     }
                 }
             }
         }else{
             #pragma omp for
             for(int i=0; i<num_points; i++){
                 const int *map = pmap.getStrip(i);
                 for(int j=0; j<num_dimensions; j++){
                     if (map[j] == 1){ // if this dimension needs to be refined
-                        if (!(useParents && addParent(points.getIndex(i), j, points, lrefined))){
-                            addChildLimited(points.getIndex(i), j, points, level_limits, lrefined);
+                        if (!(useParents && addParent<effrule>(points.getIndex(i), j, points, lrefined))){
+                            addChildLimited<effrule>(points.getIndex(i), j, points, level_limits, lrefined);
                         }
                     }
                 }
             }
         }
 
         #pragma omp critical
@@ -1429,72 +1699,76 @@
     }
     #else
     if (level_limits.empty()){
         for(int i=0; i<num_points; i++){
             const int *map = pmap.getStrip(i);
             for(int j=0; j<num_dimensions; j++){
                 if (map[j] == 1){ // if this dimension needs to be refined
-                    if (!(useParents && addParent(points.getIndex(i), j, points, refined))){
-                        addChild(points.getIndex(i), j, points, refined);
+                    if (!(useParents && addParent<effrule>(points.getIndex(i), j, points, refined))){
+                        addChild<effrule>(points.getIndex(i), j, points, refined);
                     }
                 }
             }
         }
     }else{
         for(int i=0; i<num_points; i++){
             const int *map = pmap.getStrip(i);
             for(int j=0; j<num_dimensions; j++){
                 if (map[j] == 1){ // if this dimension needs to be refined
-                    if (!(useParents && addParent(points.getIndex(i), j, points, refined))){
-                        addChildLimited(points.getIndex(i), j, points, level_limits, refined);
+                    if (!(useParents && addParent<effrule>(points.getIndex(i), j, points, refined))){
+                        addChildLimited<effrule>(points.getIndex(i), j, points, level_limits, refined);
                     }
                 }
             }
         }
     }
     #endif
 
     MultiIndexSet result(refined);
     if (criteria == refine_stable)
-        HierarchyManipulations::completeToLower(points, result, rule.get());
+        HierarchyManipulations::completeToLower<effrule>(points, result);
+
     return result;
 }
 
+template<RuleLocal::erule effrule>
 bool GridLocalPolynomial::addParent(const int point[], int direction, const MultiIndexSet &exclude, Data2D<int> &destination) const{
     std::vector<int> dad(point, point + num_dimensions);
     bool added = false;
-    dad[direction] = rule->getParent(point[direction]);
+    dad[direction] = RuleLocal::getParent<effrule>(point[direction]);
     if ((dad[direction] != -1) && exclude.missing(dad)){
         destination.appendStrip(dad);
         added = true;
     }
-    dad[direction] = rule->getStepParent(point[direction]);
+    dad[direction] = RuleLocal::getStepParent<effrule>(point[direction]);
     if ((dad[direction] != -1) && exclude.missing(dad)){
         destination.appendStrip(dad);
         added = true;
     }
     return added;
 }
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::addChild(const int point[], int direction, const MultiIndexSet &exclude, Data2D<int> &destination) const{
     std::vector<int> kid(point, point + num_dimensions);
-    int max_1d_kids = rule->getMaxNumKids();
+    int max_1d_kids = RuleLocal::getMaxNumKids<effrule>();
     for(int i=0; i<max_1d_kids; i++){
-        kid[direction] = rule->getKid(point[direction], i);
+        kid[direction] = RuleLocal::getKid<effrule>(point[direction], i);
         if ((kid[direction] != -1) && exclude.missing(kid)){
             destination.appendStrip(kid);
         }
     }
 }
+template<RuleLocal::erule effrule>
 void GridLocalPolynomial::addChildLimited(const int point[], int direction, const MultiIndexSet &exclude, const std::vector<int> &level_limits, Data2D<int> &destination) const{
     std::vector<int> kid(point, point + num_dimensions);
-    int max_1d_kids = rule->getMaxNumKids();
+    int max_1d_kids = RuleLocal::getMaxNumKids<effrule>();
     for(int i=0; i<max_1d_kids; i++){
-        kid[direction] = rule->getKid(point[direction], i);
+        kid[direction] = RuleLocal::getKid<effrule>(point[direction], i);
         if ((kid[direction] != -1)
-            && ((level_limits[direction] == -1) || (rule->getLevel(kid[direction]) <= level_limits[direction]))
+            && ((level_limits[direction] == -1) || (RuleLocal::getLevel<effrule>(kid[direction]) <= level_limits[direction]))
             && exclude.missing(kid)){
             destination.appendStrip(kid);
         }
     }
 }
 
 void GridLocalPolynomial::clearRefinement(){ needed = MultiIndexSet(); }
@@ -1504,22 +1778,61 @@
 const int* GridLocalPolynomial::getNeededIndexes() const{
     return (needed.empty()) ? 0 : needed.getIndex(0);
 }
 std::vector<double> GridLocalPolynomial::getSupport() const{
     MultiIndexSet const &work = (points.empty()) ? needed : points;
 
     std::vector<double> support(Utils::size_mult(work.getNumIndexes(), work.getNumDimensions()));
-    std::transform(work.begin(), work.end(), support.begin(), [&](int p)->double{ return rule->getSupport(p); });
+
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            std::transform(work.begin(), work.end(), support.begin(),
+                           [&](int p)->double{ return RuleLocal::getSupport<RuleLocal::erule::pwc>(p); });
+            break;
+        case RuleLocal::erule::localp:
+            std::transform(work.begin(), work.end(), support.begin(),
+                           [&](int p)->double{ return RuleLocal::getSupport<RuleLocal::erule::localp>(p); });
+            break;
+        case RuleLocal::erule::semilocalp:
+            std::transform(work.begin(), work.end(), support.begin(),
+                           [&](int p)->double{ return RuleLocal::getSupport<RuleLocal::erule::semilocalp>(p); });
+            break;
+        case RuleLocal::erule::localp0:
+            std::transform(work.begin(), work.end(), support.begin(),
+                           [&](int p)->double{ return RuleLocal::getSupport<RuleLocal::erule::localp0>(p); });
+            break;
+        default: // case RuleLocal::erule::localpb:
+            std::transform(work.begin(), work.end(), support.begin(),
+                           [&](int p)->double{ return RuleLocal::getSupport<RuleLocal::erule::localpb>(p); });
+            break;
+    };
     return support;
 }
 
 void GridLocalPolynomial::setSurplusRefinement(double tolerance, TypeRefinement criteria, int output, const std::vector<int> &level_limits, const double *scale_correction){
     clearRefinement();
 
-    needed = getRefinementCanidates(tolerance, criteria, output, level_limits, scale_correction);
+    switch(effective_rule) {
+        case RuleLocal::erule::pwc:
+            needed = getRefinementCanidates<RuleLocal::erule::pwc>(tolerance, criteria, output, level_limits, scale_correction);
+            break;
+        case RuleLocal::erule::localp:
+            needed = getRefinementCanidates<RuleLocal::erule::localp>(tolerance, criteria, output, level_limits, scale_correction);
+            break;
+        case RuleLocal::erule::semilocalp:
+            needed = getRefinementCanidates<RuleLocal::erule::semilocalp>(tolerance, criteria, output, level_limits, scale_correction);
+            break;
+        case RuleLocal::erule::localp0:
+            needed = getRefinementCanidates<RuleLocal::erule::localp0>(tolerance, criteria, output, level_limits, scale_correction);
+            break;
+        default: // case RuleLocal::erule::localpb:
+            needed = getRefinementCanidates<RuleLocal::erule::localpb>(tolerance, criteria, output, level_limits, scale_correction);
+            break;
+    };
+
 }
 std::vector<double> GridLocalPolynomial::getScaledCoefficients(int output, const double *scale_correction){
     int num_points = points.getNumIndexes();
     std::vector<double> norm = getNormalization();
     int active_outputs = (output == -1) ? num_outputs : 1;
     Utils::Wrapper2D<double const> scale(active_outputs, scale_correction);
```

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridLocalPolynomial.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridLocalPolynomial.hpp`

 * *Files 20% similar despite different names*

```diff
@@ -46,21 +46,25 @@
 
     bool isLocalPolynomial() const override{ return true; }
 
     void write(std::ostream &os, bool iomode) const override{ if (iomode == mode_ascii) write<mode_ascii>(os); else write<mode_binary>(os); }
 
     template<bool iomode> void write(std::ostream &os) const;
 
-    TypeOneDRule getRule() const override{ return rule->getType(); }
+    TypeOneDRule getRule() const override{ return RuleLocal::getRule(effective_rule); }
     int getOrder() const{ return order; }
 
+    template<RuleLocal::erule, typename points_mode>
+    void getPoints(double *x) const;
     void getLoadedPoints(double *x) const override;
     void getNeededPoints(double *x) const override;
     void getPoints(double *x) const override; // returns the loaded points unless no points are loaded, then returns the needed points
 
+    template<RuleLocal::erule effrule>
+    void getQuadratureWeights(double weights[]) const;
     void getQuadratureWeights(double weights[]) const override;
     void getInterpolationWeights(const double x[], double weights[]) const override;
     void getDifferentiationWeights(const double x[], double weights[]) const override;
 
     void loadNeededValues(const double *vals) override;
 
     void evaluate(const double x[], double y[]) const override;
@@ -98,16 +102,22 @@
      * \param pmap is a vector with size equal to the loaded points and flags as \b false each point that should be removed.
      */
     int removeMappedPoints(std::vector<bool> const &pmap);
 
     void beginConstruction() override;
     void writeConstructionData(std::ostream &os, bool) const override;
     void readConstructionData(std::istream &is, bool) override;
+    template<RuleLocal::erule effrule>
     std::vector<double> getCandidateConstructionPoints(double tolerance, TypeRefinement criteria, int output, std::vector<int> const &level_limits, double const *scale_correction);
+    std::vector<double> getCandidateConstructionPoints(double tolerance, TypeRefinement criteria, int output, std::vector<int> const &level_limits, double const *scale_correction);
+    template<RuleLocal::erule effrule>
+    void loadConstructedPoint(const double x[], const std::vector<double> &y);
     void loadConstructedPoint(const double x[], const std::vector<double> &y) override;
+    template<RuleLocal::erule effrule>
+    void loadConstructedPoint(const double x[], int numx, const double y[]);
     void loadConstructedPoint(const double x[], int numx, const double y[]) override;
     void finishConstruction() override;
 
     void evaluateHierarchicalFunctions(const double x[], int num_x, double y[]) const override;
     std::vector<double> getSupport() const override final;
     void setHierarchicalCoefficients(const double c[]) override;
     void integrateHierarchicalFunctions(double integrals[]) const override;
@@ -127,26 +137,33 @@
 
     //! \brief Used as part of the loadNeededPoints() algorithm, updates the values and cuda cache, but does not touch the surpluses.
     void updateValues(double const *vals);
 
     void buildTree();
 
     //! \brief Returns a list of indexes of the nodes in \b points that are descendants of the \b point.
+    template<RuleLocal::erule effrule>
     std::vector<int> getSubGraph(std::vector<int> const &point) const;
 
     //! \brief Add the \b point to the grid using the \b values.
+    template<RuleLocal::erule effrule>
     void expandGrid(std::vector<int> const &point, std::vector<double> const &value);
 
     //! \brief Return the multi-index of canonical point \b x.
+    template<RuleLocal::erule effrule>
     std::vector<int> getMultiIndex(const double x[]);
 
     //! \brief Looks for a batch of constructed points and processes all that will result in a connected graph.
+    template<RuleLocal::erule effrule>
     void loadConstructedPoints();
 
     //! \brief Fast algorithm, uses global Kronecker algorithm to recompute all surpluses
+    template<RuleLocal::erule effrule>
+    void recomputeSurpluses();
+
     void recomputeSurpluses();
 
     /*!
      * \brief Update the surpluses for a portion of the graph.
      *
      * Updates the surpluses (i.e., hierarchical coefficients) for a portion of the DAG graph.
      * - \b work is the point set to consider
@@ -156,22 +173,53 @@
      * - \b dagUp must have been computed using \b MultiIndexManipulations::computeDAGup(\b work, \b rule, \b dagUp)
      *
      * Note: adjusting the \b level vector allows to update the surpluses for only a portion of the graph.
      *
      * Note: see the comments inside recomputeSurpluses() for the performance comparison between different algorithms
      *       also note that this method can be used to partially update, i.e., update the surpluses for some of the indexes
      */
+    template<RuleLocal::erule effrule>
     void updateSurpluses(MultiIndexSet const &work, int max_level, std::vector<int> const &level, Data2D<int> const &dagUp);
 
     // Same idea as in GridSequence::applyTransformationTransposed().
-    template<int mode> void applyTransformationTransposed(double weights[], const MultiIndexSet &work, const std::vector<int> &active_points) const;
+    template<int mode>
+    void applyTransformationTransposed(double weights[], const MultiIndexSet &work, const std::vector<int> &active_points) const;
+    template<int mode, RuleLocal::erule effrule>
+    void applyTransformationTransposed(double weights[], const MultiIndexSet &work, const std::vector<int> &active_points) const;
 
     void buildSparseMatrixBlockForm(const double x[], int num_x, int num_chunk, std::vector<int> &numnz,
                                     std::vector<std::vector<int>> &tindx, std::vector<std::vector<double>> &tvals) const;
 
+    template<RuleLocal::erule eff_rule>
+    double evalBasisSupported(const int point[], const double x[], bool &isSupported) const{
+        double f = RuleLocal::evalSupport<eff_rule>(order, point[0], x[0], isSupported);
+        if (!isSupported) return 0.0;
+        for(int j=1; j<num_dimensions; j++){
+            f *= RuleLocal::evalSupport<eff_rule>(order, point[j], x[j], isSupported);
+            if (!isSupported) return 0.0;
+        }
+        return f;
+    }
+    template<RuleLocal::erule effrule>
+    void diffBasisSupported(const int point[], const double x[], double diff_values[], bool &isSupported) const{
+        isSupported = false;
+        for(int i=0; i<num_dimensions; i++) diff_values[i] = 1.0;
+        bool isDimSupported = false;
+        for(int k=0; k<num_dimensions; k++) {
+            double fval = RuleLocal::evalSupport<effrule>(order, point[k], x[k], isDimSupported);
+            isSupported = isDimSupported or isSupported;
+            for(int j=0; j<k; j++) diff_values[j] *= fval;
+            for(int j=k+1; j<num_dimensions; j++) diff_values[j] *= fval;
+        }
+        for (int k=0; k<num_dimensions; k++) {
+            diff_values[k] *= RuleLocal::diffSupport<effrule>(order, point[k], x[k], isDimSupported);
+            isSupported = isDimSupported or isSupported;
+        }
+    }
+
     /*!
      * \brief Walk through all the nodes of the tree and touches only the nodes supported at \b x.
      *
      * The template is instantiated in different modes:
      * - \b mode \b 0, ignore \b sindx and \b svals, find the non-zero basis functions multiply them by the surpluses and add to \b y
      * - \b mode \b 1, ignore \b y, form a sparse vector by std::vector::push_back() to the \b sindx and \b svals
      * - \b mode \b 2, same as \b mode \b 1 but it also sorts the entries within the vector (requirement of Nvidia cusparseDgemvi)
@@ -179,25 +227,29 @@
      * - \b mode \b 4, same as \b mode \b 1, but replaces the non-zero basis function values with their gradient vectors
      *
      * For mode 4, the i-th entry of sindx maps to the set of num_dimension values in svals at index (i * num_dimension). Hence,
      * we have (sindx.size() * num_dimensions == svals.size()).
      *
      * In all cases, \b work is the \b points or \b needed set that has been used to construct the tree.
      */
-    template<int mode>
+    template<int mode, RuleLocal::erule effrule>
     void walkTree(const MultiIndexSet &work, const double x[], std::vector<int> &sindx, std::vector<double> &svals, double *y) const{
         std::vector<int> monkey_count(top_level+1); // traverse the tree, counts the branches of the current node
         std::vector<int> monkey_tail(top_level+1); // traverse the tree, keeps track of the previous node (history)
 
+        bool isSupported;
+        double basis_value;
+        std::vector<double> basis_derivative(num_dimensions);
+
         for(const auto &r : roots){
-            bool isSupported;
-            double basis_value = (mode == 3 or mode == 4) ? 0.0 : evalBasisSupported(work.getIndex(r), x, isSupported);
-            std::vector<double> basis_derivative(num_dimensions);
-            if (mode == 3 or mode == 4)
-                diffBasisSupported(work.getIndex(r), x, basis_derivative.data(), isSupported);
+            if (mode == 3 or mode == 4) {
+                diffBasisSupported<effrule>(work.getIndex(r), x, basis_derivative.data(), isSupported);
+            } else {
+                basis_value = evalBasisSupported<effrule>(work.getIndex(r), x, isSupported);
+            }
 
             if (isSupported){
                 if (mode == 0){
                     double const *s = surpluses.getStrip(r);
                     for(int k=0; k<num_outputs; k++)
                         y[k] += basis_value * s[k];
                 }else if (mode == 1 or mode == 2){
@@ -218,17 +270,17 @@
                 monkey_tail[0] = r;
                 monkey_count[0] = pntr[r];
 
                 while(monkey_count[0] < pntr[monkey_tail[0]+1]){
                     if (monkey_count[current] < pntr[monkey_tail[current]+1]){
                         int p = indx[monkey_count[current]];
                         if (mode == 3 or mode == 4){
-                            diffBasisSupported(work.getIndex(p), x, basis_derivative.data(), isSupported);
+                            diffBasisSupported<effrule>(work.getIndex(p), x, basis_derivative.data(), isSupported);
                         }else{
-                            basis_value = evalBasisSupported(work.getIndex(p), x, isSupported);
+                            basis_value = evalBasisSupported<effrule>(work.getIndex(p), x, isSupported);
                         }
                         if (isSupported){
                             if (mode == 0){
                                 double const *s = surpluses.getStrip(p);
                                 for(int k=0; k<num_outputs; k++)
                                     y[k] += basis_value * s[k];
                             }else if (mode == 1 or mode == 2){
@@ -267,26 +319,55 @@
 
             std::vector<int> idx = sindx;
             std::vector<double> vls = svals;
             std::transform(map.begin(), map.end(), sindx.begin(), [&](int i)->int{ return idx[i]; });
             std::transform(map.begin(), map.end(), svals.begin(), [&](int i)->double{ return vls[i]; });
         }
     }
+    // Explicitly instantiates based on the effective_rule
+    template<int mode>
+    void walkTree(const MultiIndexSet &work, const double x[], std::vector<int> &sindx, std::vector<double> &svals, double *y) const{
+        switch(effective_rule) {
+            case RuleLocal::erule::pwc:
+                walkTree<mode, RuleLocal::erule::pwc>(work,x, sindx, svals, y);
+                break;
+            case RuleLocal::erule::localp:
+                walkTree<mode, RuleLocal::erule::localp>(work,x, sindx, svals, y);
+                break;
+            case RuleLocal::erule::semilocalp:
+                walkTree<mode, RuleLocal::erule::semilocalp>(work,x, sindx, svals, y);
+                break;
+            case RuleLocal::erule::localp0:
+                walkTree<mode, RuleLocal::erule::localp0>(work,x, sindx, svals, y);
+                break;
+            default: // case RuleLocal::erule::localpb:
+                walkTree<mode, RuleLocal::erule::localpb>(work,x, sindx, svals, y);
+                break;
+        };
+    }
 
-    double evalBasisRaw(const int point[], const double x[]) const;
-    double evalBasisSupported(const int point[], const double x[], bool &isSupported) const;
-    void diffBasisSupported(const int point[], const double x[], double diff_values[], bool &isSupported) const;
+    template<RuleLocal::erule effrule>
+    double evalBasisRaw(const int point[], const double x[]) const {
+        double f = RuleLocal::evalRaw<effrule>(order, point[0], x[0]);
+        for(int j=1; j<num_dimensions; j++) f *= RuleLocal::evalRaw<effrule>(order, point[j], x[j]);
+        return f;
+    }
 
     std::vector<double> getNormalization() const;
 
+    template<RuleLocal::erule effrule>
     Data2D<int> buildUpdateMap(double tolerance, TypeRefinement criteria, int output, const double *scale_correction) const;
+    template<RuleLocal::erule effrule>
     MultiIndexSet getRefinementCanidates(double tolerance, TypeRefinement criteria, int output, const std::vector<int> &level_limits, const double *scale_correction) const;
 
+    template<RuleLocal::erule effrule>
     bool addParent(const int point[], int direction, const MultiIndexSet &exclude, Data2D<int> &destination) const;
+    template<RuleLocal::erule effrule>
     void addChild(const int point[], int direction, const MultiIndexSet &exclude, Data2D<int> &destination) const;
+    template<RuleLocal::erule effrule>
     void addChildLimited(const int point[], int direction, const MultiIndexSet &exclude, const std::vector<int> &level_limits, Data2D<int> &destination) const;
 
     void clearGpuSurpluses();
     void clearGpuBasisHierarchy();
 
 private:
     int order, top_level;
@@ -296,28 +377,43 @@
     Data2D<int> parents;
 
     // tree for evaluation
     std::vector<int> roots;
     std::vector<int> pntr;
     std::vector<int> indx;
 
-    std::unique_ptr<BaseRuleLocalPolynomial> rule;
+    RuleLocal::erule effective_rule;
 
     std::unique_ptr<SimpleConstructData> dynamic_values;
 
     // synchronize with tasgpu_devalpwpoly_feval
     template<int ord, TypeOneDRule crule, typename T>
     Data2D<T> encodeSupportForGPU(const MultiIndexSet &work) const{
         Data2D<T> cpu_support(num_dimensions, work.getNumIndexes());
         for(int i=0; i<work.getNumIndexes(); i++){
             const int* p = work.getIndex(i);
             T *s = cpu_support.getStrip(i);
             for(int j=0; j<num_dimensions; j++){
-                s[j] = static_cast<T>(rule->getSupport(p[j]));
-                if (ord != 0){
+                if (ord == 0){
+                    s[j] = static_cast<T>(RuleLocal::getSupport<RuleLocal::erule::pwc>(p[j]));
+                } else {
+                    switch(crule) {
+                        case rule_localp:
+                            s[j] = static_cast<T>(RuleLocal::getSupport<RuleLocal::erule::localp>(p[j]));
+                            break;
+                        case rule_semilocalp:
+                            s[j] = static_cast<T>(RuleLocal::getSupport<RuleLocal::erule::semilocalp>(p[j]));
+                            break;
+                        case rule_localp0:
+                            s[j] = static_cast<T>(RuleLocal::getSupport<RuleLocal::erule::localp0>(p[j]));
+                            break;
+                        case rule_localpb:
+                            s[j] = static_cast<T>(RuleLocal::getSupport<RuleLocal::erule::localpb>(p[j]));
+                            break;
+                    };
                     if (ord == 2) s[j] *= s[j];
                     if ((crule == rule_localp) || (crule == rule_semilocalp)) if (p[j] == 0) s[j] = static_cast<T>(-1.0); // constant function
                     if ((crule == rule_localp) && (ord == 2)){
                         if (p[j] == 1) s[j] = static_cast<T>(-2.0);
                         else if (p[j] == 2) s[j] = static_cast<T>(-3.0);
                     }
                     if ((crule == rule_semilocalp) && (ord == 2)){
@@ -350,28 +446,39 @@
         std::unique_ptr<GridLocalPolynomial> grid = Utils::make_unique<GridLocalPolynomial>(acc);
 
             grid->num_dimensions = IO::readNumber<iomode, int>(is);
             grid->num_outputs = IO::readNumber<iomode, int>(is);
             grid->order = IO::readNumber<iomode, int>(is);
             grid->top_level = IO::readNumber<iomode, int>(is);
             TypeOneDRule rule = IO::readRule<iomode>(is);
-            grid->rule = makeRuleLocalPolynomial(rule, grid->order);
+            grid->effective_rule = RuleLocal::getEffectiveRule(grid->order, rule);
 
             if (IO::readFlag<iomode>(is)) grid->points = MultiIndexSet(is, iomode());
             if (std::is_same<iomode, IO::mode_ascii_type>::value){ // backwards compatible: surpluses and needed, or needed and surpluses
                 if (IO::readFlag<iomode>(is))
                     grid->surpluses = IO::readData2D<iomode, double>(is, grid->num_outputs, grid->points.getNumIndexes());
                 if (IO::readFlag<iomode>(is)) grid->needed = MultiIndexSet(is, iomode());
             }else{
                 if (IO::readFlag<iomode>(is)) grid->needed = MultiIndexSet(is, iomode());
                 if (IO::readFlag<iomode>(is))
                     grid->surpluses = IO::readData2D<iomode, double>(is, grid->num_outputs, grid->points.getNumIndexes());
             }
+            int max_parents = [&]()->int {
+                    switch(grid->effective_rule) {
+                        case RuleLocal::erule::pwc: return RuleLocal::getMaxNumParents<RuleLocal::erule::pwc>();
+                        case RuleLocal::erule::localp: return RuleLocal::getMaxNumParents<RuleLocal::erule::localp>();
+                        case RuleLocal::erule::semilocalp: return RuleLocal::getMaxNumParents<RuleLocal::erule::semilocalp>();
+                        case RuleLocal::erule::localp0: return RuleLocal::getMaxNumParents<RuleLocal::erule::localp0>();
+                        default: // case RuleLocal::erule::localpb:
+                            return RuleLocal::getMaxNumParents<RuleLocal::erule::localpb>();
+                    };
+                }();
+
             if (IO::readFlag<iomode>(is))
-                grid->parents = IO::readData2D<iomode, int>(is, grid->rule->getMaxNumParents() * grid->num_dimensions, grid->points.getNumIndexes());
+                grid->parents = IO::readData2D<iomode, int>(is, max_parents * grid->num_dimensions, grid->points.getNumIndexes());
 
             size_t num_points = (size_t) ((grid->points.empty()) ? grid->needed.getNumIndexes() : grid->points.getNumIndexes());
             grid->roots = std::vector<int>((size_t) IO::readNumber<iomode, int>(is));
             if (grid->roots.size() > 0){
                 IO::readVector<iomode>(is, grid->roots);
                 grid->pntr = IO::readVector<iomode, int>(is, num_points + 1);
                 if (grid->pntr[num_points] > 0){
```

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridSequence.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridSequence.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridSequence.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridSequence.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridWavelet.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridWavelet.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgGridWavelet.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgGridWavelet.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgHardCodedTabulatedRules.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgHardCodedTabulatedRules.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgHardCodedTabulatedRules.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgHardCodedTabulatedRules.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgHierarchyManipulator.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgHierarchyManipulator.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -80,84 +80,106 @@
  *
  * Each node defined by a multi-index in \b mset can have one or more parents in each direction,
  * where the parent-offspring relation is defined by the \b rule. For each index in \b mset, the
  * Data2D structure \b parents will hold a strip with the location of each parent in \b mset
  * (or -1 if the parent is missing from \b mset).
  * \endinternal
  */
-Data2D<int> computeDAGup(MultiIndexSet const &mset, const BaseRuleLocalPolynomial *rule);
+template<RuleLocal::erule effrule>
+Data2D<int> computeDAGup(MultiIndexSet const &mset);
+/*!
+ * \internal
+ * \ingroup TasmanianHierarchyManipulations
+ * \brief Cache the indexes slot numbers of the parents of the multi-indexes in \b mset.
+ *
+ * The effective rule is passed in at runtime and a switch statement finds the correct template.
+ * \endinternal
+ */
+Data2D<int> computeDAGup(MultiIndexSet const &mset, RuleLocal::erule effrule);
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Variant that also check if all points have all parents
  *
  * This is merged together so it will do only one pass over the data.
  *
  * On exit, \b is_complete will indicate whether there are points with missing parents.
  * \endinternal
  */
-Data2D<int> computeDAGup(MultiIndexSet const &mset, const BaseRuleLocalPolynomial *rule, bool &is_complete);
+template<RuleLocal::erule effrule>
+Data2D<int> computeDAGup(MultiIndexSet const &mset, bool &is_complete);
 
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Cache the indexes slot numbers of the children of the multi-indexes in \b mset.
  *
  * Each node defined by a multi-index in \b mset can have one or more children in each direction,
  * where the parent-offspring relation is defined by the \b rule. For each index in \b mset, the
  * returned Data2D structure will hold a strip with the location of each child in \b mset
  * (or -1 if the kid is missing from \b mset).
  * \endinternal
  */
-Data2D<int> computeDAGDown(MultiIndexSet const &mset, const BaseRuleLocalPolynomial *rule);
+template<RuleLocal::erule effrule>
+Data2D<int> computeDAGDown(MultiIndexSet const &mset);
 
 /*!
  * \internal
  * \brief Returns a vector that is the sum of the one dimensional levels of each multi-index in the set.
  * \ingroup TasmanianHierarchyManipulations
  * \endinternal
  */
-std::vector<int> computeLevels(MultiIndexSet const &mset, BaseRuleLocalPolynomial const *rule);
+template<RuleLocal::erule effrule>
+std::vector<int> computeLevels(MultiIndexSet const &mset);
+/*!
+ * \internal
+ * \brief Overload that turns switch statement into template instantiations
+ * \ingroup TasmanianHierarchyManipulations
+ * \endinternal
+ */
+std::vector<int> computeLevels(MultiIndexSet const &mset, RuleLocal::erule effrule);
 
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Complete \b refined so that the union of \b refined and \b mset is lower w.r.t. the \b rule.
  * \endinternal
  */
-void completeToLower(MultiIndexSet const &mset, MultiIndexSet &refined, BaseRuleLocalPolynomial const *rule);
+template<RuleLocal::erule effrule>
+void completeToLower(MultiIndexSet const &mset, MultiIndexSet &refined);
 
 /*!
  * \internal
  * \brief Will call \b apply() with the slot index in \b mset of each parent/child of \b point.
  * \ingroup TasmanianHierarchyManipulations
  * \endinternal
  */
-inline void touchAllImmediateRelatives(std::vector<int> &point, MultiIndexSet const &mset, BaseRuleLocalPolynomial const *rule, std::function<void(int i)> apply){
-    int max_kids = rule->getMaxNumKids();
+template<RuleLocal::erule effrule, typename callable_method>
+void touchAllImmediateRelatives(std::vector<int> &point, MultiIndexSet const &mset, callable_method apply){
+    int max_kids = RuleLocal::getMaxNumKids<effrule>();
     for(auto &v : point){
         int save = v; // replace one by one each index of p with either parent or kid
 
         // check the parents
-        v = rule->getParent(save);
+        v = RuleLocal::getParent<effrule>(save);
         if (v > -1){
             int parent_index = mset.getSlot(point);
             if (parent_index > -1)
                 apply(parent_index);
         }
 
-        v = rule->getStepParent(save);
+        v = RuleLocal::getStepParent<effrule>(save);
         if (v > -1){
             int parent_index = mset.getSlot(point);
             if (parent_index > -1)
                 apply(parent_index);
         }
 
         for(int k=0; k<max_kids; k++){
-            v = rule->getKid(save, k);
+            v = RuleLocal::getKid<effrule>(save, k);
             if (v > -1){
                 int kid_index = mset.getSlot(point);
                 if (kid_index > -1)
                     apply(kid_index);
             }
         }
 
@@ -168,33 +190,35 @@
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Return the tensor set of all points that sit on level zero (i.e., have no parents).
  *
  * \endinternal
  */
-inline MultiIndexSet getLevelZeroPoints(size_t num_dimensions, BaseRuleLocalPolynomial const *rule){
+template<RuleLocal::erule effrule>
+MultiIndexSet getLevelZeroPoints(size_t num_dimensions){
     int num_parents = 0;
-    while(rule->getParent(num_parents) == -1) num_parents++;
+    while(RuleLocal::getParent<effrule>(num_parents) == -1) num_parents++;
     return MultiIndexManipulations::generateFullTensorSet(std::vector<int>(num_dimensions, num_parents));
 }
 
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Return the largest subset of \b candidates such that adding it to \b current will result in a connected graph.
  *
  * \endinternal
  */
-inline MultiIndexSet getLargestConnected(MultiIndexSet const &current, MultiIndexSet const &candidates, BaseRuleLocalPolynomial const *rule){
+template<RuleLocal::erule effrule>
+MultiIndexSet getLargestConnected(MultiIndexSet const &current, MultiIndexSet const &candidates){
     if (candidates.empty()) return MultiIndexSet();
     auto num_dimensions = candidates.getNumDimensions();
 
     // always consider the points without parents
-    MultiIndexSet level_zero = getLevelZeroPoints(num_dimensions, rule);
+    MultiIndexSet level_zero = getLevelZeroPoints<effrule>(num_dimensions);
 
     MultiIndexSet result; // keep track of the cumulative result
     MultiIndexSet total = current; // forms a working copy of the entire merged graph
 
     // do not consider the points already included in total, complexity is level_zero.getNumIndexes()
     if (!total.empty()) level_zero = level_zero - total;
 
@@ -208,26 +232,27 @@
 
         result = MultiIndexSet(roots);
         total += result;
     }
 
     if (total.empty()) return MultiIndexSet(); // current was empty and no roots could be added
 
-    int max_kids      = rule->getMaxNumKids();
-    int max_relatives = rule->getMaxNumParents() + max_kids;
+    int max_kids      = RuleLocal::getMaxNumKids<effrule>();
+    int max_relatives = RuleLocal::getMaxNumParents<effrule>() + max_kids;
     Data2D<int> update;
     do{
         update = Data2D<int>(num_dimensions, 0);
 
         for(int i=0; i<total.getNumIndexes(); i++){
             std::vector<int> relative(total.getIndex(i), total.getIndex(i) + num_dimensions);
             for(auto &r : relative){
                 int k = r; // save the value
                 for(int j=0; j<max_relatives; j++){
-                    r = (j < max_kids) ? rule->getKid(k, j) : ((j - max_kids == 0) ? rule->getParent(k) : rule->getStepParent(k));
+                    r = (j < max_kids) ? RuleLocal::getKid<effrule>(k, j)
+                                       : ((j - max_kids == 0) ? RuleLocal::getParent<effrule>(k) : RuleLocal::getStepParent<effrule>(k));
                     if ((r != -1) && !candidates.missing(relative) && total.missing(relative))
                         update.appendStrip(relative);
                 }
                 r = k;
             }
         }
 
@@ -237,14 +262,15 @@
             total  += update_set;
         }
     }while(update.getNumStrips() > 0);
 
     return result;
 }
 
+
 /*!
  * \internal
  * \ingroup TasmanianHierarchyManipulations
  * \brief Split the range between \b ibegin and \b iend into strips of \b stride and orders those by levels according to the level index in \b ilevels.
  *
  * \endinternal
  */
```

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgHipKernels.hip.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgHipKernels.hip.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgIOHelpers.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgIOHelpers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgIndexManipulator.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgIndexManipulator.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -51,27 +51,40 @@
 template<bool use_parents_direction>
 void repeatAddIndexes(std::function<bool(const std::vector<int> &index)> inside, std::vector<MultiIndexSet> &level_sets){
     size_t num_dimensions = level_sets.back().getNumDimensions();
     bool adding = true;
     while(adding){
         Data2D<int> level((int) num_dimensions, 0);
         int num_indexes = level_sets.back().getNumIndexes();
-        #pragma omp parallel for
-        for(int i=0; i<num_indexes; i++){
+        #pragma omp parallel
+        {
             std::vector<int> point(num_dimensions);
-            std::copy_n(level_sets.back().getIndex(i), num_dimensions, point.data());
-            for(auto &p : point){
-                p += (use_parents_direction) ? -1 : 1; // parents have lower index, children have higher indexes
-                if ( (not use_parents_direction or p >= 0) and inside(point) ){
-                    #pragma omp critical
-                    {
-                        level.appendStrip(point);
+            Data2D<int> mlevel((int) num_dimensions, 0);
+
+            #pragma omp for
+            for(int i=0; i<num_indexes; i++){
+                std::copy_n(level_sets.back().getIndex(i), num_dimensions, point.data());
+                for(auto &p : point){
+                    p += (use_parents_direction) ? -1 : 1; // parents have lower index, children have higher indexes
+                    if (not use_parents_direction or p >= 0) {
+                        bool is_inside = false;
+                        #pragma omp critical(level_append)
+                        {
+                            is_inside = inside(point);
+                        }
+                        if (is_inside)
+                            mlevel.appendStrip(point);
                     }
+                    p -= (use_parents_direction) ? -1 : 1; // restore p
                 }
-                p -= (use_parents_direction) ? -1 : 1; // restore p
+            }
+
+            #pragma omp critical
+            {
+                level.append(mlevel);
             }
         }
 
         adding = (level.getNumStrips() > 0);
         if (adding)
             level_sets.push_back(MultiIndexSet(level));
     }
```

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgIndexManipulator.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgIndexManipulator.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgIndexSets.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgIndexSets.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgIndexSets.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgIndexSets.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgLinearSolvers.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgLinearSolvers.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgLinearSolvers.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgLinearSolvers.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgMathUtils.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgMathUtils.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgOneDimensionalWrapper.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgOneDimensionalWrapper.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgRuleWavelet.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgRuleWavelet.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgRuleWavelet.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgRuleWavelet.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgSequenceOptimizer.cpp` & `Tasmanian-8.1b2/SparseGrids/tsgSequenceOptimizer.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgSequenceOptimizer.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgSequenceOptimizer.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/SparseGrids/tsgUtils.hpp` & `Tasmanian-8.1b2/SparseGrids/tsgUtils.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Tasgrid/CMakeLists.txt` & `Tasmanian-8.1b2/Tasgrid/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Tasgrid/tasgridLogs.in.hpp` & `Tasmanian-8.1b2/Tasgrid/tasgridLogs.in.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Tasgrid/tasgridWrapper.cpp` & `Tasmanian-8.1b2/Tasgrid/tasgridWrapper.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Tasgrid/tasgridWrapper.hpp` & `Tasmanian-8.1b2/Tasgrid/tasgridWrapper.hpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Tasgrid/tasgrid_main.cpp` & `Tasmanian-8.1b2/Tasgrid/tasgrid_main.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Testing/CMakeLists.test.cmake` & `Tasmanian-8.1b2/Testing/CMakeLists.test.cmake`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Testing/tasmanian_version.cpp` & `Tasmanian-8.1b2/Testing/tasmanian_version.cpp`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/Testing/test_post_install.in.sh` & `Tasmanian-8.1b2/Testing/test_post_install.in.sh`

 * *Files identical despite different names*

### Comparing `Tasmanian-8.1b1/setup.py` & `Tasmanian-8.1b2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 if isosxframework:
     cmake_args.append('-DTasmanian_osx_framework:BOOL=ON')
 
 
 # call the actual package setup command
 setup(
     name='Tasmanian',
-    version='8.1b1',
+    version='8.1b2',
     author='Miroslav Stoyanov',
     author_email='stoyanovmk@ornl.gov',
     description='UQ library for sparse grids, optimization and Bayesian inference',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://tasmanian.ornl.gov',
     classifiers=[
```

