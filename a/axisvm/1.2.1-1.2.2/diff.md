# Comparing `tmp/axisvm-1.2.1.tar.gz` & `tmp/axisvm-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axisvm-1.2.1.tar", last modified: Thu Oct  5 06:54:29 2023, max compression
+gzip compressed data, was "axisvm-1.2.2.tar", last modified: Tue Apr  2 12:20:24 2024, max compression
```

## Comparing `axisvm-1.2.1.tar` & `axisvm-1.2.2.tar`

### file list

```diff
@@ -1,260 +1,115 @@
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.749621 axisvm-1.2.1/
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.415837 axisvm-1.2.1/.circleci/
--rw-rw-rw-   0        0        0     2672 2022-06-07 21:27:15.000000 axisvm-1.2.1/.circleci/config.yml
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.375833 axisvm-1.2.1/.github/
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.438580 axisvm-1.2.1/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      872 2021-11-29 17:14:48.000000 axisvm-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      615 2021-11-29 17:14:48.000000 axisvm-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-rw-rw-   0        0        0     2165 2023-09-29 09:00:49.000000 axisvm-1.2.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.439571 axisvm-1.2.1/.vscode/
--rw-rw-rw-   0        0        0      224 2022-10-11 06:56:58.000000 axisvm-1.2.1/.vscode/settings.json
--rw-rw-rw-   0        0        0     1095 2021-11-29 09:51:27.000000 axisvm-1.2.1/LICENSE
--rw-rw-rw-   0        0        0    10078 2023-10-05 06:54:29.747622 axisvm-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6590 2023-09-29 09:00:49.000000 axisvm-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.477571 axisvm-1.2.1/docs/
--rw-rw-rw-   0        0        0      638 2022-06-08 18:13:41.000000 axisvm-1.2.1/docs/Makefile
--rwxrwxrwx   0        0        0      804 2022-06-08 18:13:41.000000 axisvm-1.2.1/docs/make.bat
--rw-rw-rw-   0        0        0      249 2022-11-03 14:13:56.000000 axisvm-1.2.1/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.747571 axisvm-1.2.1/docs/source/
--rw-rw-rw-   0        0        0  2094454 2022-09-29 18:15:11.000000 axisvm-1.2.1/docs/source/AxisVM_logo.bmp
--rw-rw-rw-   0        0        0   413507 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/IAxisVMNodes.png
--rw-rw-rw-   0        0        0   169233 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/IAxisVMNodes_AddWithDof.png
--rw-rw-rw-   0        0        0   133114 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/IAxisVMNodes_Functions.png
--rw-rw-rw-   0        0        0   267991 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/IAxisVMNodes_Properties.png
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.781572 axisvm-1.2.1/docs/source/_notebooks/
--rw-rw-rw-   0        0        0       52 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/_notebooks/console.nblink
--rw-rw-rw-   0        0        0       61 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/_notebooks/membrane.nblink
--rw-rw-rw-   0        0        0       60 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/_notebooks/plate1.nblink
--rw-rw-rw-   0        0        0       60 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/_notebooks/plate2.nblink
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.844570 axisvm-1.2.1/docs/source/_static/
--rw-rw-rw-   0        0        0  2094454 2022-06-09 19:45:41.000000 axisvm-1.2.1/docs/source/_static/AxisVM_logo.bmp
--rw-rw-rw-   0        0        0    29461 2022-06-10 10:08:11.000000 axisvm-1.2.1/docs/source/_static/AxisVM_logo_dark.png
--rw-rw-rw-   0        0        0    30404 2022-06-10 10:08:10.000000 axisvm-1.2.1/docs/source/_static/AxisVM_logo_light.png
--rw-rw-rw-   0        0        0       80 2022-10-24 15:28:08.000000 axisvm-1.2.1/docs/source/api.rst
--rw-rw-rw-   0        0        0     1031 2022-09-29 19:00:43.000000 axisvm-1.2.1/docs/source/api_axisvm.rst
--rw-rw-rw-   0        0        0      180 2022-09-13 22:09:14.000000 axisvm-1.2.1/docs/source/api_client.rst
--rw-rw-rw-   0        0        0       90 2022-09-13 07:36:49.000000 axisvm-1.2.1/docs/source/api_python.rst
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.137621 axisvm-1.2.1/docs/source/auto_examples/
--rw-rw-rw-   0        0        0     8326 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/auto_examples_jupyter.zip
--rw-rw-rw-   0        0        0     3571 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/auto_examples_python.zip
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.314623 axisvm-1.2.1/docs/source/auto_examples/images/
--rw-rw-rw-   0        0        0    22301 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_0_grid1_001.png
--rw-rw-rw-   0        0        0    47359 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_0_grid1_001_2_0x.png
--rw-rw-rw-   0        0        0    81648 2022-09-29 18:36:02.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_1_domain_results_001.png
--rw-rw-rw-   0        0        0   190619 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_1_domain_results_001_2_0x.png
--rw-rw-rw-   0        0        0    81648 2022-09-29 18:32:14.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_1_surface_stresses_001.png
--rw-rw-rw-   0        0        0   190619 2022-09-29 18:32:14.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_1_surface_stresses_001_2_0x.png
--rw-rw-rw-   0        0        0   312454 2022-09-29 20:28:18.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_2_domain_stresses_001.png
--rw-rw-rw-   0        0        0   755682 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/images/sphx_glr_plot_2_domain_stresses_001_2_0x.png
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.354620 axisvm-1.2.1/docs/source/auto_examples/images/thumb/
--rw-rw-rw-   0        0        0    14864 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/images/thumb/sphx_glr_plot_0_grid1_thumb.png
--rw-rw-rw-   0        0        0    15811 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/images/thumb/sphx_glr_plot_1_domain_results_thumb.png
--rw-rw-rw-   0        0        0    15811 2022-09-29 18:32:15.000000 axisvm-1.2.1/docs/source/auto_examples/images/thumb/sphx_glr_plot_1_surface_stresses_thumb.png
--rw-rw-rw-   0        0        0    27606 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/images/thumb/sphx_glr_plot_2_domain_stresses_thumb.png
--rw-rw-rw-   0        0        0     2111 2023-03-15 23:32:29.000000 axisvm-1.2.1/docs/source/auto_examples/index.rst
--rw-rw-rw-   0        0        0     1858 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/plot_0_grid1.ipynb
--rw-rw-rw-   0        0        0      669 2023-09-29 09:00:49.000000 axisvm-1.2.1/docs/source/auto_examples/plot_0_grid1.py
--rw-rw-rw-   0        0        0       32 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/plot_0_grid1.py.md5
--rw-rw-rw-   0        0        0     2336 2022-09-13 10:55:33.000000 axisvm-1.2.1/docs/source/auto_examples/plot_0_grid1.rst
--rw-rw-rw-   0        0        0     1948 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_domain_results.ipynb
--rw-rw-rw-   0        0        0      842 2023-09-29 09:00:49.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_domain_results.py
--rw-rw-rw-   0        0        0       32 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_domain_results.py.md5
--rw-rw-rw-   0        0        0     2416 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_domain_results.rst
--rw-rw-rw-   0        0        0     3524 2022-09-29 18:36:03.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_domain_results_codeobj.pickle
--rw-rw-rw-   0        0        0     2049 2022-09-29 18:32:15.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_surface_stresses.ipynb
--rw-rw-rw-   0        0        0      830 2023-09-29 09:00:49.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_surface_stresses.py
--rw-rw-rw-   0        0        0       32 2022-09-29 18:32:15.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_surface_stresses.py.md5
--rw-rw-rw-   0        0        0     2475 2022-09-29 18:32:15.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_surface_stresses.rst
--rw-rw-rw-   0        0        0     3524 2022-09-29 18:32:15.000000 axisvm-1.2.1/docs/source/auto_examples/plot_1_surface_stresses_codeobj.pickle
--rw-rw-rw-   0        0        0     1941 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/plot_2_domain_stresses.ipynb
--rw-rw-rw-   0        0        0      830 2023-09-29 09:00:49.000000 axisvm-1.2.1/docs/source/auto_examples/plot_2_domain_stresses.py
--rw-rw-rw-   0        0        0       32 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/plot_2_domain_stresses.py.md5
--rw-rw-rw-   0        0        0     2425 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/plot_2_domain_stresses.rst
--rw-rw-rw-   0        0        0     3524 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/plot_2_domain_stresses_codeobj.pickle
--rw-rw-rw-   0        0        0      510 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_examples/searchindex.bak
--rw-rw-rw-   0        0        0   129903 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_examples/searchindex.dat
--rw-rw-rw-   0        0        0      510 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_examples/searchindex.dir
--rw-rw-rw-   0        0        0      951 2022-09-29 20:28:19.000000 axisvm-1.2.1/docs/source/auto_examples/sg_execution_times.rst
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.429624 axisvm-1.2.1/docs/source/auto_pyvista_examples/
--rw-rw-rw-   0        0        0       22 2022-09-13 10:58:08.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/auto_pyvista_examples_jupyter.zip
--rw-rw-rw-   0        0        0       22 2022-09-13 10:58:08.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/auto_pyvista_examples_python.zip
--rw-rw-rw-   0        0        0      783 2022-09-13 10:58:08.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/index.rst
--rw-rw-rw-   0        0        0      510 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/searchindex.bak
--rw-rw-rw-   0        0        0   129903 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/searchindex.dat
--rw-rw-rw-   0        0        0      510 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/auto_pyvista_examples/searchindex.dir
--rw-rw-rw-   0        0        0    15129 2023-09-29 09:00:49.000000 axisvm-1.2.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      104 2022-09-13 08:18:24.000000 axisvm-1.2.1/docs/source/downloads.rst
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.381838 axisvm-1.2.1/docs/source/gen_modules/
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.559620 axisvm-1.2.1/docs/source/gen_modules/backreferences/
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.ApplicationClose.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.AskCloseOnLastReleased.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.AskSaveOnLastReleased.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.AxisVMPlatform.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.BringToFront.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.Catalog.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.ChangeUnitSystem.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.CustomFunction.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.DisableMainForm.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.EnableMainForm.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.HandleMessages.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.MessageDlg.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.Models.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.Quit.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.UnLoadCOMclients.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.app.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.model.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axapp.IAxisVMApplication.new_model.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:06:33.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axcalculation.IAxisVMCalculation.LinearAnalysis.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:01:09.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axcalculation.IAxisVMCalculation.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.ABDS.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:25:44.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.IsXLAM.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.coordinates.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.detach_mesh.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.plot.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.plot_dof_solution.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:36:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.plot_forces.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:41:04.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.plot_stresses.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:25:44.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.record.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.surface_coordinates.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:21:53.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.topology.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:25:44.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.tr.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 19:25:44.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.transformation_matrix.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 20:48:06.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomain.xlam_surface_stresses.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axdomain.IAxisVMDomains.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axline.IAxisVMLine.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axline.IAxisVMLines.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmember.IAxisVMMember.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmember.IAxisVMMembers.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Calculation.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Domains.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Lines.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Materials.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Members.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.MeshSurfaceIds.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Nodes.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Results.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Surfaces.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.Windows.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.coordinates.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.critical_xlam_data.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.dof_solution.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.generalized_surface_forces.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:31.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axmodel.IAxisVMModel.surface_stresses.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.connected_surfaces.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_IDs.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_connected_surfaceIDs.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_indices.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:34:51.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_record.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_selected.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_selected_IDs.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.get_selected_indices.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.select.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:55.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.select_IDs.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axnode.IAxisVMNodes.select_indices.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.attributes.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.critical_xlam_efficiency.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.normal.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.record.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.surface_attributes.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.topology.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.tr.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.transformation_matrix.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurface.xlam_stresses.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.attributes.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.frames.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.n.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.surface_attributes.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.t.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:59:01.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.axsurface.IAxisVMSurfaces.tr.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:10:14.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.client.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:10:14.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.client.start_AxisVM.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:10:18.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.tlb.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:10:18.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.tlb.find_axisvm_tlb.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:10:18.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.com.tlb.wrap_axisvm_tlb.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.delete_downloads.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_bernoulli_grid.examples
--rw-rw-rw-   0        0        0        0 2022-09-29 18:31:47.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_plate_ss.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_sample_001.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_stand_stl.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_stand_vtk.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_stem_stl.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.download_tetrahedra.examples
--rw-rw-rw-   0        0        0        0 2022-09-13 22:16:59.000000 axisvm-1.2.1/docs/source/gen_modules/backreferences/axisvm.examples.downloads.examples
--rw-rw-rw-   0        0        0     4499 2022-11-08 08:58:46.000000 axisvm-1.2.1/docs/source/getting_started.md
--rw-rw-rw-   0        0        0   307075 2022-09-29 18:03:37.000000 axisvm-1.2.1/docs/source/gt40.PNG
--rw-rw-rw-   0        0        0     1618 2022-11-08 09:06:53.000000 axisvm-1.2.1/docs/source/index.rst
--rw-rw-rw-   0        0        0       75 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/notebooks.rst
--rw-rw-rw-   0        0        0     3905 2022-06-09 19:36:16.000000 axisvm-1.2.1/docs/source/tips_and_tricks.md
--rw-rw-rw-   0        0        0      155 2023-03-16 17:13:47.000000 axisvm-1.2.1/docs/source/tutorials.rst
--rw-rw-rw-   0        0        0      107 2022-09-29 17:49:19.000000 axisvm-1.2.1/docs/source/verification.rst
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.571623 axisvm-1.2.1/examples/
--rw-rw-rw-   0        0        0       34 2022-08-15 17:39:56.000000 axisvm-1.2.1/examples/README.txt
--rw-rw-rw-   0        0        0      669 2023-09-29 09:00:49.000000 axisvm-1.2.1/examples/plot_0_grid1.py
--rw-rw-rw-   0        0        0      842 2023-09-29 09:00:49.000000 axisvm-1.2.1/examples/plot_1_domain_results.py
--rw-rw-rw-   0        0        0      830 2023-09-29 09:00:49.000000 axisvm-1.2.1/examples/plot_2_domain_stresses.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.663620 axisvm-1.2.1/notebooks/
--rw-rw-rw-   0        0        0    21809 2023-10-05 02:13:46.000000 axisvm-1.2.1/notebooks/connected_members.ipynb
--rw-rw-rw-   0        0        0   388406 2023-09-29 09:00:49.000000 axisvm-1.2.1/notebooks/console.ipynb
--rw-rw-rw-   0        0        0     3252 2023-09-29 09:00:49.000000 axisvm-1.2.1/notebooks/gen_tlb.ipynb
--rw-rw-rw-   0        0        0    75542 2023-10-05 02:13:46.000000 axisvm-1.2.1/notebooks/membrane_example.ipynb
--rw-rw-rw-   0        0        0  1232016 2023-10-05 02:13:46.000000 axisvm-1.2.1/notebooks/plate_example_1.ipynb
--rw-rw-rw-   0        0        0   102334 2023-10-05 02:13:46.000000 axisvm-1.2.1/notebooks/plate_example_2.ipynb
--rw-rw-rw-   0        0        0   142642 2023-10-05 02:13:46.000000 axisvm-1.2.1/notebooks/pyvista.ipynb
--rw-rw-rw-   0        0        0   110233 2023-09-29 09:00:49.000000 axisvm-1.2.1/notebooks/tetrahedra.ipynb
--rw-rw-rw-   0        0        0     1651 2023-10-05 02:13:46.000000 axisvm-1.2.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.670622 axisvm-1.2.1/pyvista_examples/
--rw-rw-rw-   0        0        0       44 2022-08-15 17:39:34.000000 axisvm-1.2.1/pyvista_examples/README.txt
--rw-rw-rw-   0        0        0       17 2023-09-29 09:00:49.000000 axisvm-1.2.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       19 2023-09-29 09:00:49.000000 axisvm-1.2.1/requirements-test.txt
--rw-rw-rw-   0        0        0      212 2023-10-05 06:52:35.000000 axisvm-1.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-10-05 06:54:29.749621 axisvm-1.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:28.384835 axisvm-1.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.672622 axisvm-1.2.1/src/axisvm/
--rw-rw-rw-   0        0        0     2058 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.726621 axisvm-1.2.1/src/axisvm/com/
--rw-rw-rw-   0        0        0       25 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/__init__.py
--rw-rw-rw-   0        0        0      620 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/attr.py
--rw-rw-rw-   0        0        0    10121 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axapp.py
--rw-rw-rw-   0        0        0     2088 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axcalculation.py
--rw-rw-rw-   0        0        0      209 2023-10-05 02:13:46.000000 axisvm-1.2.1/src/axisvm/com/axcatalog.py
--rw-rw-rw-   0        0        0    32807 2023-10-05 02:13:46.000000 axisvm-1.2.1/src/axisvm/com/axdomain.py
--rw-rw-rw-   0        0        0    11863 2023-10-05 02:13:46.000000 axisvm-1.2.1/src/axisvm/com/axline.py
--rw-rw-rw-   0        0        0     2189 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axloadcombinations.py
--rw-rw-rw-   0        0        0     2584 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axmaterial.py
--rw-rw-rw-   0        0        0    10705 2023-10-05 02:13:46.000000 axisvm-1.2.1/src/axisvm/com/axmember.py
--rw-rw-rw-   0        0        0    14584 2023-09-29 09:44:47.000000 axisvm-1.2.1/src/axisvm/com/axmodel.py
--rw-rw-rw-   0        0        0     1907 2023-09-29 09:44:47.000000 axisvm-1.2.1/src/axisvm/com/axnodalsupports.py
--rw-rw-rw-   0        0        0    10306 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axnode.py
--rw-rw-rw-   0        0        0     4068 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axresult.py
--rw-rw-rw-   0        0        0    27827 2023-10-05 02:13:46.000000 axisvm-1.2.1/src/axisvm/com/axsurface.py
--rw-rw-rw-   0        0        0     1199 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/axwindow.py
--rw-rw-rw-   0        0        0     3799 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/client.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.733622 axisvm-1.2.1/src/axisvm/com/core/
--rw-rw-rw-   0        0        0       25 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/core/__init__.py
--rw-rw-rw-   0        0        0      947 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/core/abc.py
--rw-rw-rw-   0        0        0    12893 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/core/utils.py
--rw-rw-rw-   0        0        0     7757 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/core/wrap.py
--rw-rw-rw-   0        0        0     2390 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/com/tlb.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.735622 axisvm-1.2.1/src/axisvm/docs/
--rw-rw-rw-   0        0        0       25 2022-08-09 11:31:16.000000 axisvm-1.2.1/src/axisvm/docs/__init__.py
--rw-rw-rw-   0        0        0     1408 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/docs/utils.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.738622 axisvm-1.2.1/src/axisvm/examples/
--rw-rw-rw-   0        0        0       51 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/examples/__init__.py
--rw-rw-rw-   0        0        0     7506 2023-09-29 09:00:49.000000 axisvm-1.2.1/src/axisvm/examples/downloads.py
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.703619 axisvm-1.2.1/src/axisvm.egg-info/
--rw-rw-rw-   0        0        0    10078 2023-10-05 06:54:28.000000 axisvm-1.2.1/src/axisvm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14225 2023-10-05 06:54:28.000000 axisvm-1.2.1/src/axisvm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-05 06:54:28.000000 axisvm-1.2.1/src/axisvm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      405 2023-10-05 06:54:28.000000 axisvm-1.2.1/src/axisvm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-10-05 06:54:28.000000 axisvm-1.2.1/src/axisvm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-10-05 06:54:29.741622 axisvm-1.2.1/tests/
--rw-rw-rw-   0        0        0        0 2022-06-02 18:26:52.000000 axisvm-1.2.1/tests/__init__.py
--rw-rw-rw-   0        0        0      309 2023-09-29 09:00:49.000000 axisvm-1.2.1/tests/test_client.py
--rw-rw-rw-   0        0        0     4001 2023-03-15 23:26:33.000000 axisvm-1.2.1/tips_and_tricks.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.208159 axisvm-1.2.2/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.752266 axisvm-1.2.2/.circleci/
+-rw-rw-rw-   0        0        0     2672 2022-06-07 21:27:15.000000 axisvm-1.2.2/.circleci/config.yml
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.708258 axisvm-1.2.2/.github/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.774292 axisvm-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      872 2021-11-29 17:14:48.000000 axisvm-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      615 2021-11-29 17:14:48.000000 axisvm-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-rw-rw-   0        0        0     2165 2023-09-29 09:00:49.000000 axisvm-1.2.2/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.775260 axisvm-1.2.2/.vscode/
+-rw-rw-rw-   0        0        0      224 2023-12-21 15:21:56.000000 axisvm-1.2.2/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1095 2021-11-29 09:51:27.000000 axisvm-1.2.2/LICENSE
+-rw-rw-rw-   0        0        0     7714 2024-04-02 12:20:24.207189 axisvm-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3824 2023-12-21 15:09:38.000000 axisvm-1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.783261 axisvm-1.2.2/docs/
+-rw-rw-rw-   0        0        0      638 2022-06-08 18:13:41.000000 axisvm-1.2.2/docs/Makefile
+-rwxrwxrwx   0        0        0      804 2022-06-08 18:13:41.000000 axisvm-1.2.2/docs/make.bat
+-rw-rw-rw-   0        0        0      614 2023-12-18 15:41:14.000000 axisvm-1.2.2/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.791259 axisvm-1.2.2/docs/source/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.953483 axisvm-1.2.2/docs/source/_static/
+-rw-rw-rw-   0        0        0  2094454 2022-06-09 19:45:41.000000 axisvm-1.2.2/docs/source/_static/AxisVM_logo.bmp
+-rw-rw-rw-   0        0        0    29461 2022-06-10 10:08:11.000000 axisvm-1.2.2/docs/source/_static/AxisVM_logo_dark.png
+-rw-rw-rw-   0        0        0    30404 2022-06-10 10:08:10.000000 axisvm-1.2.2/docs/source/_static/AxisVM_logo_light.png
+-rw-rw-rw-   0        0        0   413507 2022-09-29 17:49:19.000000 axisvm-1.2.2/docs/source/_static/IAxisVMNodes.png
+-rw-rw-rw-   0        0        0   169233 2022-09-29 17:49:19.000000 axisvm-1.2.2/docs/source/_static/IAxisVMNodes_AddWithDof.png
+-rw-rw-rw-   0        0        0   133114 2022-09-29 17:49:19.000000 axisvm-1.2.2/docs/source/_static/IAxisVMNodes_Functions.png
+-rw-rw-rw-   0        0        0   267991 2022-09-29 17:49:19.000000 axisvm-1.2.2/docs/source/_static/IAxisVMNodes_Properties.png
+-rw-rw-rw-   0        0        0     2322 2023-12-18 20:39:49.000000 axisvm-1.2.2/docs/source/_static/custom.css
+-rw-rw-rw-   0        0        0      143 2023-10-05 02:24:33.000000 axisvm-1.2.2/docs/source/_static/custom.js
+-rw-rw-rw-   0        0        0   307075 2022-09-29 18:03:37.000000 axisvm-1.2.2/docs/source/_static/gt40.PNG
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.040067 axisvm-1.2.2/docs/source/_static/index-images/
+-rw-rw-rw-   0        0        0      856 2023-09-27 18:07:10.000000 axisvm-1.2.2/docs/source/_static/index-images/api.svg
+-rw-rw-rw-   0        0        0     1342 2023-09-27 17:50:06.000000 axisvm-1.2.2/docs/source/_static/index-images/gallery.svg
+-rw-rw-rw-   0        0        0      791 2023-09-27 18:06:20.000000 axisvm-1.2.2/docs/source/_static/index-images/getting_started.svg
+-rw-rw-rw-   0        0        0     4237 2023-09-27 18:04:33.000000 axisvm-1.2.2/docs/source/_static/index-images/user_guide.svg
+-rw-rw-rw-   0        0        0    17493 2023-10-05 02:24:33.000000 axisvm-1.2.2/docs/source/_static/require.min.js
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.043064 axisvm-1.2.2/docs/source/api/
+-rw-rw-rw-   0        0        0     1031 2022-09-29 19:00:43.000000 axisvm-1.2.2/docs/source/api/api_axisvm.rst
+-rw-rw-rw-   0        0        0      170 2023-12-18 16:42:44.000000 axisvm-1.2.2/docs/source/api/api_client.rst
+-rw-rw-rw-   0        0        0      104 2023-12-18 16:42:52.000000 axisvm-1.2.2/docs/source/api/api_downloads.rst
+-rw-rw-rw-   0        0        0      394 2023-12-18 16:43:56.000000 axisvm-1.2.2/docs/source/api.rst
+-rw-rw-rw-   0        0        0     7312 2023-12-18 20:22:32.000000 axisvm-1.2.2/docs/source/conf.py
+-rw-rw-rw-   0        0        0     1092 2024-02-27 09:00:25.000000 axisvm-1.2.2/docs/source/doc_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.047088 axisvm-1.2.2/docs/source/examples/
+-rw-rw-rw-   0        0        0    86521 2023-12-18 15:51:17.000000 axisvm-1.2.2/docs/source/examples/plot_domain_results.ipynb
+-rw-rw-rw-   0        0        0   396275 2023-12-18 15:52:27.000000 axisvm-1.2.2/docs/source/examples/plot_domain_stresses.ipynb
+-rw-rw-rw-   0        0        0    29160 2023-12-18 15:49:37.000000 axisvm-1.2.2/docs/source/examples/screenshot.ipynb
+-rw-rw-rw-   0        0        0      184 2024-04-02 12:11:07.000000 axisvm-1.2.2/docs/source/examples_gallery.rst
+-rw-rw-rw-   0        0        0     6774 2023-12-18 19:45:19.000000 axisvm-1.2.2/docs/source/getting_started.md
+-rw-rw-rw-   0        0        0     3461 2023-12-18 19:02:58.000000 axisvm-1.2.2/docs/source/index.rst
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.057093 axisvm-1.2.2/docs/source/notebooks/
+-rw-rw-rw-   0        0        0    88041 2024-02-27 14:36:33.000000 axisvm-1.2.2/docs/source/notebooks/_concrete_beam_design.ipynb
+-rw-rw-rw-   0        0        0    16861 2024-01-29 11:21:18.000000 axisvm-1.2.2/docs/source/notebooks/adding_cross_sections.ipynb
+-rw-rw-rw-   0        0        0   388406 2023-09-29 09:00:49.000000 axisvm-1.2.2/docs/source/notebooks/console.ipynb
+-rw-rw-rw-   0        0        0    75542 2023-10-05 02:13:46.000000 axisvm-1.2.2/docs/source/notebooks/membrane_example.ipynb
+-rw-rw-rw-   0        0        0    34414 2023-12-21 14:01:06.000000 axisvm-1.2.2/docs/source/notebooks/moving_loads_on_a_beam.ipynb
+-rw-rw-rw-   0        0        0  1232016 2023-10-05 02:13:46.000000 axisvm-1.2.2/docs/source/notebooks/plate_example_1.ipynb
+-rw-rw-rw-   0        0        0   102334 2023-10-05 02:13:46.000000 axisvm-1.2.2/docs/source/notebooks/plate_example_2.ipynb
+-rw-rw-rw-   0        0        0     3927 2023-12-18 19:03:01.000000 axisvm-1.2.2/docs/source/tips_and_tricks.md
+-rw-rw-rw-   0        0        0      559 2023-12-18 18:44:46.000000 axisvm-1.2.2/docs/source/user_guide.rst
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.143260 axisvm-1.2.2/notebooks/
+-rw-rw-rw-   0        0        0    21809 2023-10-05 02:13:46.000000 axisvm-1.2.2/notebooks/connected_members.ipynb
+-rw-rw-rw-   0        0        0     3252 2023-09-29 09:00:49.000000 axisvm-1.2.2/notebooks/gen_tlb.ipynb
+-rw-rw-rw-   0        0        0   142642 2023-10-05 02:13:46.000000 axisvm-1.2.2/notebooks/pyvista.ipynb
+-rw-rw-rw-   0        0        0   110233 2023-09-29 09:00:49.000000 axisvm-1.2.2/notebooks/tetrahedra.ipynb
+-rw-rw-rw-   0        0        0     1652 2024-02-27 11:31:03.000000 axisvm-1.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       17 2023-09-29 09:00:49.000000 axisvm-1.2.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       40 2023-12-21 13:59:45.000000 axisvm-1.2.2/requirements-test.txt
+-rw-rw-rw-   0        0        0      220 2024-02-27 14:14:07.000000 axisvm-1.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:20:24.208159 axisvm-1.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:23.713258 axisvm-1.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.144259 axisvm-1.2.2/src/axisvm/
+-rw-rw-rw-   0        0        0     2227 2023-12-18 20:11:52.000000 axisvm-1.2.2/src/axisvm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.190226 axisvm-1.2.2/src/axisvm/com/
+-rw-rw-rw-   0        0        0       25 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/__init__.py
+-rw-rw-rw-   0        0        0      620 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/attr.py
+-rw-rw-rw-   0        0        0    10121 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axapp.py
+-rw-rw-rw-   0        0        0     2088 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axcalculation.py
+-rw-rw-rw-   0        0        0      209 2023-10-05 02:13:46.000000 axisvm-1.2.2/src/axisvm/com/axcatalog.py
+-rw-rw-rw-   0        0        0    32867 2023-12-18 19:50:51.000000 axisvm-1.2.2/src/axisvm/com/axdomain.py
+-rw-rw-rw-   0        0        0    11863 2023-10-05 02:13:46.000000 axisvm-1.2.2/src/axisvm/com/axline.py
+-rw-rw-rw-   0        0        0     2189 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axloadcombinations.py
+-rw-rw-rw-   0        0        0     2584 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axmaterial.py
+-rw-rw-rw-   0        0        0    10705 2023-10-05 02:13:46.000000 axisvm-1.2.2/src/axisvm/com/axmember.py
+-rw-rw-rw-   0        0        0    14859 2023-12-17 19:23:14.000000 axisvm-1.2.2/src/axisvm/com/axmodel.py
+-rw-rw-rw-   0        0        0     1907 2023-09-29 09:44:47.000000 axisvm-1.2.2/src/axisvm/com/axnodalsupports.py
+-rw-rw-rw-   0        0        0    10306 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axnode.py
+-rw-rw-rw-   0        0        0     3144 2023-12-17 20:30:51.000000 axisvm-1.2.2/src/axisvm/com/axrcbeamdesign.py
+-rw-rw-rw-   0        0        0     4068 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axresult.py
+-rw-rw-rw-   0        0        0    27827 2023-10-05 02:13:46.000000 axisvm-1.2.2/src/axisvm/com/axsurface.py
+-rw-rw-rw-   0        0        0     1199 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/axwindow.py
+-rw-rw-rw-   0        0        0     3799 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/client.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.194230 axisvm-1.2.2/src/axisvm/com/core/
+-rw-rw-rw-   0        0        0       25 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/core/__init__.py
+-rw-rw-rw-   0        0        0      947 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/core/abc.py
+-rw-rw-rw-   0        0        0    12893 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/core/utils.py
+-rw-rw-rw-   0        0        0     7757 2023-12-17 19:22:51.000000 axisvm-1.2.2/src/axisvm/com/core/wrap.py
+-rw-rw-rw-   0        0        0     2390 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/com/tlb.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.196251 axisvm-1.2.2/src/axisvm/docs/
+-rw-rw-rw-   0        0        0       25 2022-08-09 11:31:16.000000 axisvm-1.2.2/src/axisvm/docs/__init__.py
+-rw-rw-rw-   0        0        0     1408 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/docs/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.198161 axisvm-1.2.2/src/axisvm/examples/
+-rw-rw-rw-   0        0        0       51 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/examples/__init__.py
+-rw-rw-rw-   0        0        0     7506 2023-09-29 09:00:49.000000 axisvm-1.2.2/src/axisvm/examples/downloads.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.204161 axisvm-1.2.2/src/axisvm.egg-info/
+-rw-rw-rw-   0        0        0     7714 2024-04-02 12:20:23.000000 axisvm-1.2.2/src/axisvm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2803 2024-04-02 12:20:23.000000 axisvm-1.2.2/src/axisvm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:20:23.000000 axisvm-1.2.2/src/axisvm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      526 2024-04-02 12:20:23.000000 axisvm-1.2.2/src/axisvm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 12:20:23.000000 axisvm-1.2.2/src/axisvm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 12:20:24.202159 axisvm-1.2.2/tests/
+-rw-rw-rw-   0        0        0        0 2022-06-02 18:26:52.000000 axisvm-1.2.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-12-21 14:23:00.000000 axisvm-1.2.2/tests/conftest.py
+-rw-rw-rw-   0        0        0     1062 2023-12-21 15:05:36.000000 axisvm-1.2.2/tests/test_doc_notebooks.py
+-rw-rw-rw-   0        0        0      475 2023-12-21 15:03:34.000000 axisvm-1.2.2/tests/utils.py
+-rw-rw-rw-   0        0        0     4001 2023-03-15 23:26:33.000000 axisvm-1.2.2/tips_and_tricks.md
```

### Comparing `axisvm-1.2.1/.circleci/config.yml` & `axisvm-1.2.2/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `axisvm-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `axisvm-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/.gitignore` & `axisvm-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/LICENSE` & `axisvm-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/README.md` & `axisvm-1.2.2/docs/source/getting_started.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,412 +1,424 @@
-00000000: 2320 2a2a 5079 4178 6973 564d 2a2a 202d  # **PyAxisVM** -
-00000010: 2054 6865 206f 6666 6963 6961 6c20 7079   The official py
-00000020: 7468 6f6e 2070 6163 6b61 6765 2066 6f72  thon package for
-00000030: 202a 2a41 7869 7356 4d2a 2a0d 0a0d 0a21   **AxisVM**....!
-00000040: 5b61 6c74 2074 6578 745d 2868 7474 7073  [alt text](https
-00000050: 3a2f 2f67 6974 6875 622e 636f 6d2f 4178  ://github.com/Ax
-00000060: 6973 564d 2f44 796e 616d 6f54 6f41 7869  isVM/DynamoToAxi
-00000070: 7356 4d2f 626c 6f62 2f6d 6173 7465 722f  sVM/blob/master/
-00000080: 446f 6375 6d65 6e74 6174 696f 6e2f 696d  Documentation/im
-00000090: 6167 6573 2f41 7869 7356 4d25 3230 6c6f  ages/AxisVM%20lo
-000000a0: 676f 2e62 6d70 290d 0a0d 0a3c 7461 626c  go.bmp)....<tabl
-000000b0: 653e 0d0a 2020 2020 3c74 723e 0d0a 2020  e>..    <tr>..  
-000000c0: 2020 2020 2020 3c74 643e 4c61 7465 7374        <td>Latest
-000000d0: 2052 656c 6561 7365 3c2f 7464 3e0d 0a20   Release</td>.. 
-000000e0: 2020 2020 2020 203c 7464 3e0d 0a20 2020         <td>..   
-000000f0: 2020 2020 2020 2020 203c 6120 6872 6566           <a href
-00000100: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
-00000110: 7267 2f70 726f 6a65 6374 2f61 7869 7376  rg/project/axisv
-00000120: 6d2f 222f 3e0d 0a20 2020 2020 2020 2020  m/"/>..         
-00000130: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-00000140: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
-00000150: 696f 2f70 792f 6178 6973 766d 2e73 7667  io/py/axisvm.svg
-00000160: 222f 3e0d 0a20 2020 2020 2020 203c 2f74  "/>..        </t
-00000170: 643e 0d0a 2020 2020 3c2f 7472 3e0d 0a20  d>..    </tr>.. 
-00000180: 2020 203c 7472 3e0d 0a20 2020 2020 2020     <tr>..       
-00000190: 203c 7464 3e4c 6963 656e 7365 3c2f 7464   <td>License</td
-000001a0: 3e0d 0a20 2020 2020 2020 203c 7464 3e0d  >..        <td>.
-000001b0: 0a20 2020 2020 2020 2020 2020 203c 6120  .            <a 
-000001c0: 6872 6566 3d22 6874 7470 733a 2f2f 6f70  href="https://op
-000001d0: 656e 736f 7572 6365 2e6f 7267 2f6c 6963  ensource.org/lic
-000001e0: 656e 7365 732f 4d49 5422 2f3e 0d0a 2020  enses/MIT"/>..  
-000001f0: 2020 2020 2020 2020 2020 3c69 6d67 2073            <img s
-00000200: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000210: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000220: 2f4c 6963 656e 7365 2d4d 4954 2d79 656c  /License-MIT-yel
-00000230: 6c6f 772e 7376 6722 2f3e 0d0a 2020 2020  low.svg"/>..    
-00000240: 2020 2020 3c2f 7464 3e0d 0a20 2020 203c      </td>..    <
-00000250: 2f74 723e 0d0a 3c2f 7461 626c 653e 0d0a  /tr>..</table>..
-00000260: 0d0a 2323 204f 7665 7276 6965 770d 0a0d  ..## Overview...
-00000270: 0a54 6865 202a 2a50 7941 7869 7356 4d2a  .The **PyAxisVM*
-00000280: 2a20 7072 6f6a 6563 7420 6f66 6665 7273  * project offers
-00000290: 2061 2068 6967 682d 6c65 7665 6c20 696e   a high-level in
-000002a0: 7465 7266 6163 6520 746f 202a 2a41 7869  terface to **Axi
-000002b0: 7356 4d2a 2a2c 206d 616b 696e 6720 6974  sVM**, making it
-000002c0: 7320 6f70 6572 6174 696f 6e73 2061 7661  s operations ava
-000002d0: 696c 6162 6c65 2064 6972 6563 746c 7920  ilable directly 
-000002e0: 6672 6f6d 2050 7974 686f 6e2e 2049 7420  from Python. It 
-000002f0: 6275 696c 6473 206f 6e20 746f 7020 6f66  builds on top of
-00000300: 204d 6963 726f 736f 6674 2773 2043 4f4d   Microsoft's COM
-00000310: 2074 6563 686e 6f6c 6f67 7920 616e 6420   technology and 
-00000320: 7375 7070 6f72 7473 2061 6c6c 2074 6865  supports all the
-00000330: 2066 6561 7475 7265 7320 6f66 2074 6865   features of the
-00000340: 206f 7269 6769 6e61 6c20 2a2a 4178 6973   original **Axis
-00000350: 564d 2a2a 2043 4f4d 2074 7970 6520 6c69  VM** COM type li
-00000360: 6272 6172 792c 206d 616b 696e 6720 796f  brary, making yo
-00000370: 7520 6162 6c65 2074 6f0d 0a20 200d 0a2a  u able to..  ..*
-00000380: 2062 7569 6c64 2c20 6d61 6e69 7075 6c61   build, manipula
-00000390: 7465 2061 6e64 2061 6e61 6c79 7365 202a  te and analyse *
-000003a0: 2a41 7869 7356 4d2a 2a20 6d6f 6465 6c73  *AxisVM** models
-000003b0: 0d0a 0d0a 2a20 6669 6e64 2062 6574 7465  ....* find bette
-000003c0: 7220 736f 6c75 7469 6f6e 7320 7769 7468  r solutions with
-000003d0: 2069 7465 7261 7469 7665 206d 6574 686f   iterative metho
-000003e0: 6473 0d0a 0d0a 2a20 636f 6d62 696e 6520  ds....* combine 
-000003f0: 7468 6520 706f 7765 7220 6f66 202a 2a41  the power of **A
-00000400: 7869 7356 4d2a 2a20 7769 7468 2074 6869  xisVM** with thi
-00000410: 7264 2d70 6172 7479 2050 7974 686f 6e20  rd-party Python 
-00000420: 6c69 6272 6172 6965 730d 0a0d 0a2a 2062  libraries....* b
-00000430: 7569 6c64 2065 7874 656e 7369 6f6e 206d  uild extension m
-00000440: 6f64 756c 6573 0d0a 0d0a 4f6e 2074 6f70  odules....On top
-00000450: 206f 6620 7468 6174 2c20 2a2a 5079 4178   of that, **PyAx
-00000460: 6973 564d 2a2a 2065 6e68 616e 6365 7320  isVM** enhances 
-00000470: 7468 6520 7479 7065 206c 6962 7261 7279  the type library
-00000480: 2077 6974 6820 5079 7468 6f6e 2773 2073   with Python's s
-00000490: 6c69 6369 6e67 206d 6563 6861 6e69 736d  licing mechanism
-000004a0: 2c20 636f 6e74 6578 7420 6d61 6e61 6765  , context manage
-000004b0: 6d65 6e74 2061 6e64 206d 6f72 652c 2074  ment and more, t
-000004c0: 6861 7420 656e 6162 6c65 7320 7772 6974  hat enables writ
-000004d0: 696e 6720 636c 6561 6e2c 2063 6f6e 6369  ing clean, conci
-000004e0: 7365 2c20 616e 6420 7265 6164 6162 6c65  se, and readable
-000004f0: 2063 6f64 652e 0d0a 0d0a 2323 2049 6e73   code.....## Ins
-00000500: 7461 6c6c 6174 696f 6e0d 0a0d 0a54 6869  tallation....Thi
-00000510: 7320 6973 206f 7074 696f 6e61 6c2c 2062  s is optional, b
-00000520: 7574 2077 6520 7375 6767 6573 7420 796f  ut we suggest yo
-00000530: 7520 746f 2063 7265 6174 6520 6120 6465  u to create a de
-00000540: 6469 6361 7465 6420 7669 7274 7561 6c20  dicated virtual 
-00000550: 656e 7669 726f 6d65 6e74 2061 7420 616c  enviroment at al
-00000560: 6c20 7469 6d65 7320 746f 2061 766f 6964  l times to avoid
-00000570: 2063 6f6e 666c 6963 7473 2077 6974 6820   conflicts with 
-00000580: 796f 7572 206f 7468 6572 2070 726f 6a65  your other proje
-00000590: 6374 732e 2043 7265 6174 6520 6120 666f  cts. Create a fo
-000005a0: 6c64 6572 2c20 6f70 656e 2061 2063 6f6d  lder, open a com
-000005b0: 6d61 6e64 2073 6865 6c6c 2069 6e20 7468  mand shell in th
-000005c0: 6174 2066 6f6c 6465 7220 616e 6420 7573  at folder and us
-000005d0: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-000005e0: 636f 6d6d 616e 640d 0a0d 0a60 6060 636f  command....```co
-000005f0: 6e73 6f6c 650d 0a3e 3e3e 2070 7974 686f  nsole..>>> pytho
-00000600: 6e20 2d6d 2076 656e 7620 7665 6e76 5f6e  n -m venv venv_n
-00000610: 616d 650d 0a60 6060 0d0a 0d0a 4f6e 6365  ame..```....Once
-00000620: 2074 6865 2065 6e76 6972 6f6d 656e 7420   the enviroment 
-00000630: 6973 2063 7265 6174 6564 2c20 6163 7469  is created, acti
-00000640: 7661 7465 2069 7420 7669 6120 7479 7069  vate it via typi
-00000650: 6e67 0d0a 0d0a 6060 6063 6f6e 736f 6c65  ng....```console
-00000660: 0d0a 3e3e 3e20 2e5c 7665 6e76 5f6e 616d  ..>>> .\venv_nam
-00000670: 655c 5363 7269 7074 735c 6163 7469 7661  e\Scripts\activa
-00000680: 7465 0d0a 6060 600d 0a0d 0a54 6865 202a  te..```....The *
-00000690: 2a41 7869 7356 4d2a 2a20 7079 7468 6f6e  *AxisVM** python
-000006a0: 2070 6163 6b61 6765 2063 616e 2062 6520   package can be 
-000006b0: 696e 7374 616c 6c65 6420 2865 6974 6865  installed (eithe
-000006c0: 7220 696e 2061 2076 6972 7475 616c 2065  r in a virtual e
-000006d0: 6e76 6972 6f6d 656e 7420 6f72 2067 6c6f  nviroment or glo
-000006e0: 6261 6c6c 7929 2066 726f 6d20 5079 5049  bally) from PyPI
-000006f0: 2075 7369 6e67 2060 7069 7060 206f 6e20   using `pip` on 
-00000700: 5079 7468 6f6e 203e 3d20 332e 3720 3c3d  Python >= 3.7 <=
-00000710: 2033 2e31 303a 0d0a 0d0a 6060 6063 6f6e   3.10:....```con
-00000720: 736f 6c65 0d0a 3e3e 3e20 7069 7020 696e  sole..>>> pip in
-00000730: 7374 616c 6c20 6178 6973 766d 0d0a 6060  stall axisvm..``
-00000740: 600d 0a0d 0a6f 7220 6368 6563 686b 6f75  `....or chechkou
-00000750: 7420 7769 7468 2074 6865 2066 6f6c 6c6f  t with the follo
-00000760: 7769 6e67 2063 6f6d 6d61 6e64 206f 7665  wing command ove
-00000770: 7220 4854 5450 5320 7669 6120 3c68 7474  r HTTPS via <htt
-00000780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000790: 4178 6973 564d 2f70 7961 7869 7376 6d2e  AxisVM/pyaxisvm.
-000007a0: 6769 743e 206f 7220 6279 2075 7369 6e67  git> or by using
-000007b0: 2074 6865 2047 6974 4875 6220 434c 490d   the GitHub CLI.
-000007c0: 0a0d 0a60 6060 636f 6e73 6f6c 650d 0a67  ...```console..g
-000007d0: 6820 7265 706f 2063 6c6f 6e65 2041 7869  h repo clone Axi
-000007e0: 7356 4d2f 7079 6178 6973 766d 0d0a 6060  sVM/pyaxisvm..``
-000007f0: 600d 0a0d 0a61 6e64 2069 6e73 7461 6c6c  `....and install
-00000800: 2066 726f 6d20 736f 7572 6365 2062 7920   from source by 
-00000810: 7479 7069 6e67 0d0a 0d0a 6060 6063 6f6e  typing....```con
-00000820: 736f 6c65 0d0a 3e3e 3e20 7069 7020 696e  sole..>>> pip in
-00000830: 7374 616c 6c20 2e0d 0a60 6060 0d0a 0d0a  stall ...```....
-00000840: 4966 2079 6f75 2077 616e 7420 746f 2072  If you want to r
-00000850: 756e 2074 6865 2074 6573 7473 2c20 796f  un the tests, yo
-00000860: 7520 6361 6e20 696e 7374 616c 6c20 7468  u can install th
-00000870: 6520 7061 636b 6167 6520 616c 6f6e 6720  e package along 
-00000880: 7769 7468 2074 6865 206e 6563 6573 7361  with the necessa
-00000890: 7279 206f 7074 696f 6e61 6c20 6465 7065  ry optional depe
-000008a0: 6e64 656e 6369 6573 206c 696b 6520 7468  ndencies like th
-000008b0: 6973 0d0a 0d0a 6060 6063 6f6e 736f 6c65  is....```console
-000008c0: 0d0a 3e3e 3e20 7069 7020 696e 7374 616c  ..>>> pip instal
-000008d0: 6c20 222e 5b74 6573 745d 220d 0a60 6060  l ".[test]"..```
-000008e0: 0d0a 0d0a 2323 2320 4465 7665 6c6f 706d  ....### Developm
-000008f0: 656e 7420 6d6f 6465 0d0a 0d0a 4966 2079  ent mode....If y
-00000900: 6f75 2061 7265 2061 2064 6576 656c 6f70  ou are a develop
-00000910: 6572 2061 6e64 2077 616e 7420 746f 2069  er and want to i
-00000920: 6e73 7461 6c6c 2074 6865 206c 6962 7261  nstall the libra
-00000930: 7279 2069 6e20 6465 7665 6c6f 706d 656e  ry in developmen
-00000940: 7420 6d6f 6465 2c20 7468 6520 7375 6767  t mode, the sugg
-00000950: 6573 7465 6420 7761 7920 6973 2062 7920  ested way is by 
-00000960: 7573 696e 6720 7468 6973 2063 6f6d 6d61  using this comma
-00000970: 6e64 3a0d 0a0d 0a60 6060 636f 6e73 6f6c  nd:....```consol
-00000980: 650d 0a3e 3e3e 2070 6970 2069 6e73 7461  e..>>> pip insta
-00000990: 6c6c 2022 2d65 202e 5b74 6573 742c 2064  ll "-e .[test, d
-000009a0: 6576 5d22 0d0a 6060 600d 0a0d 0a49 6620  ev]"..```....If 
-000009b0: 796f 7520 706c 616e 2074 6f20 746f 7563  you plan to touc
-000009c0: 6820 7468 6520 646f 6373 2c20 796f 7520  h the docs, you 
-000009d0: 6361 6e20 696e 7374 616c 6c20 7468 6520  can install the 
-000009e0: 7265 7175 6972 656d 656e 7473 2066 6f72  requirements for
-000009f0: 2074 6861 7420 6173 2077 656c 6c3a 0d0a   that as well:..
-00000a00: 0d0a 6060 6063 6f6e 736f 6c65 0d0a 3e3e  ..```console..>>
-00000a10: 3e20 7069 7020 696e 7374 616c 6c20 222d  > pip install "-
-00000a20: 6520 2e5b 7465 7374 2c20 6465 762c 2064  e .[test, dev, d
-00000a30: 6f63 735d 220d 0a60 6060 0d0a 0d0a 2323  ocs]"..```....##
-00000a40: 202a 2a44 6f63 756d 656e 7461 7469 6f6e   **Documentation
-00000a50: 2061 6e64 2049 7373 7565 732a 2a0d 0a0d   and Issues**...
-00000a60: 0a54 6865 202a 2a2a 4178 6973 564d 2041  .The ***AxisVM A
-00000a70: 5049 2052 6566 6572 656e 6365 2047 7569  PI Reference Gui
-00000a80: 6465 2a2a 2a20 6973 2061 7661 696c 6162  de*** is availab
-00000a90: 6c65 2069 6e20 7064 6620 666f 726d 6174  le in pdf format
-00000aa0: 2c20 2079 6f75 2063 616e 2064 6f77 6e6c  ,  you can downl
-00000ab0: 6f61 6420 6974 205b 2a2a 2a68 6572 652a  oad it [***here*
-00000ac0: 2a2a 5d28 6874 7470 733a 2f2f 6178 6973  **](https://axis
-00000ad0: 766d 2e65 752f 6178 6973 766d 2d64 6f77  vm.eu/axisvm-dow
-00000ae0: 6e6c 6f61 6473 2f23 6170 706c 6963 6174  nloads/#applicat
-00000af0: 696f 6e29 2e0d 0a0d 0a54 6865 2064 6f63  ion).....The doc
-00000b00: 756d 656e 7461 7469 6f6e 206f 6620 7468  umentation of th
-00000b10: 6973 206c 6962 7261 7279 2069 7320 6176  is library is av
-00000b20: 6169 6c61 626c 6520 5b2a 2a2a 6865 7265  ailable [***here
-00000b30: 2a2a 2a5d 2868 7474 7073 3a2f 2f61 7869  ***](https://axi
-00000b40: 7376 6d2e 6769 7468 7562 2e69 6f2f 7079  svm.github.io/py
-00000b50: 6178 6973 766d 2d64 6f63 732f 292e 0d0a  axisvm-docs/)...
-00000b60: 0d0a 506c 6561 7365 2066 6565 6c20 6672  ..Please feel fr
-00000b70: 6565 2074 6f20 706f 7374 2069 7373 7565  ee to post issue
-00000b80: 7320 616e 6420 6f74 6865 7220 7175 6573  s and other ques
-00000b90: 7469 6f6e 7320 6174 202a 2a50 7941 7869  tions at **PyAxi
-00000ba0: 7356 4d2a 2a20 4973 7375 6573 2e20 5468  sVM** Issues. Th
-00000bb0: 6973 2069 7320 7468 6520 6265 7374 2070  is is the best p
-00000bc0: 6c61 6365 2074 6f20 706f 7374 2071 7565  lace to post que
-00000bd0: 7374 696f 6e73 2061 6e64 2063 6f64 6520  stions and code 
-00000be0: 7265 6c61 7465 6420 746f 2069 7373 7565  related to issue
-00000bf0: 7320 7769 7468 2074 6869 7320 7072 6f6a  s with this proj
-00000c00: 6563 742e 0d0a 0d0a 2323 2044 6570 656e  ect.....## Depen
-00000c10: 6465 6e63 6965 730d 0a0d 0a59 6f75 2077  dencies....You w
-00000c20: 696c 6c20 6e65 6564 2061 206c 6f63 616c  ill need a local
-00000c30: 206c 6963 656e 6365 6420 636f 7079 206f   licenced copy o
-00000c40: 6620 2a2a 4178 6973 564d 2a2a 2076 6572  f **AxisVM** ver
-00000c50: 7369 6f6e 203e 3d20 3133 7232 2e20 546f  sion >= 13r2. To
-00000c60: 2067 6574 2061 2063 6f70 7920 6f66 202a   get a copy of *
-00000c70: 2a41 7869 7356 4d2a 2a2c 2070 6c65 6173  *AxisVM**, pleas
-00000c80: 6520 7669 7369 7420 6f75 7220 5b2a 2a2a  e visit our [***
-00000c90: 686f 6d65 7061 6765 2a2a 2a5d 2868 7474  homepage***](htt
-00000ca0: 7073 3a2f 2f61 7869 7376 6d2e 6575 2f29  ps://axisvm.eu/)
-00000cb0: 2e0d 0a0d 0a23 2320 4765 7474 696e 6720  .....## Getting 
-00000cc0: 5374 6172 7465 640d 0a0d 0a23 2323 2052  Started....### R
-00000cd0: 6567 6973 7465 7220 7468 6520 4178 6973  egister the Axis
-00000ce0: 564d 2054 7970 6520 4c69 6272 6172 790d  VM Type Library.
-00000cf0: 0a0d 0a49 6620 7468 6973 2069 7320 6e6f  ...If this is no
-00000d00: 7420 796f 7572 2066 6972 7374 2074 696d  t your first tim
-00000d10: 6520 7573 696e 6720 2a2a 4178 6973 564d  e using **AxisVM
-00000d20: 2a2a 2074 6872 6f75 6768 2061 2043 4f4d  ** through a COM
-00000d30: 2069 6e74 6572 6661 6365 206f 6e20 796f   interface on yo
-00000d40: 7572 206d 6163 6869 6e65 2c20 796f 7520  ur machine, you 
-00000d50: 7368 6f75 6c64 2061 6c72 6561 6479 2068  should already h
-00000d60: 6176 6520 6120 7265 6769 7374 6572 6564  ave a registered
-00000d70: 2074 7970 6520 6c69 6272 6172 7920 616e   type library an
-00000d80: 6420 796f 7520 6361 6e20 736b 6970 2074  d you can skip t
-00000d90: 6869 7320 7374 6570 2e20 4f74 6865 7277  his step. Otherw
-00000da0: 6973 652c 2066 6f6c 6c6f 7720 7468 6520  ise, follow the 
-00000db0: 696e 7374 7275 6374 696f 6e73 2061 7420  instructions at 
-00000dc0: 7468 6520 6265 6769 6e6e 696e 6720 6f66  the beginning of
-00000dd0: 2074 6865 202a 2a2a 4178 6973 564d 2041   the ***AxisVM A
-00000de0: 5049 2052 6566 6572 656e 6365 2047 7569  PI Reference Gui
-00000df0: 6465 2a2a 2a2e 0d0a 0d0a 2323 2320 4c61  de***.....### La
-00000e00: 756e 6368 2041 7869 7356 4d0d 0a0d 0a54  unch AxisVM....T
-00000e10: 6865 2060 6178 6973 766d 2e63 6f6d 2e63  he `axisvm.com.c
-00000e20: 6c69 656e 7460 2073 7562 6d6f 6475 6c65  lient` submodule
-00000e30: 2069 6d70 6c65 6d65 6e74 7320 7661 7269   implements vari
-00000e40: 6f75 7320 746f 6f6c 7320 746f 2068 616e  ous tools to han
-00000e50: 646c 6520 7468 6520 636c 6965 6e74 2073  dle the client s
-00000e60: 6964 6520 6f70 6572 6174 696f 6e73 206f  ide operations o
-00000e70: 6620 6372 6561 7469 6e67 2061 2043 4f4d  f creating a COM
-00000e80: 2063 6f6e 6e65 6374 696f 6e2e 2049 6d70   connection. Imp
-00000e90: 6f72 7420 7468 6520 6d6f 6475 6c65 2061  ort the module a
-00000ea0: 6e64 2073 7461 7274 2061 206e 6577 2061  nd start a new a
-00000eb0: 7070 6c69 6361 7469 6f6e 2069 6e73 7461  pplication insta
-00000ec0: 6e63 6520 7769 7468 2074 6865 2060 7374  nce with the `st
-00000ed0: 6172 745f 4178 6973 564d 6020 6d65 7468  art_AxisVM` meth
-00000ee0: 6f64 3a0d 0a0d 0a60 6060 7079 7468 6f6e  od:....```python
-00000ef0: 0d0a 6672 6f6d 2061 7869 7376 6d2e 636f  ..from axisvm.co
-00000f00: 6d2e 636c 6965 6e74 2069 6d70 6f72 7420  m.client import 
-00000f10: 7374 6172 745f 4178 6973 564d 0d0a 6178  start_AxisVM..ax
-00000f20: 6170 7020 3d20 7374 6172 745f 4178 6973  app = start_Axis
-00000f30: 564d 2876 6973 6962 6c65 3d54 7275 6529  VM(visible=True)
-00000f40: 0d0a 6060 600d 0a0d 0a54 6f20 7465 7374  ..```....To test
-00000f50: 2074 6865 2063 6f6e 6e65 6374 696f 6e2c   the connection,
-00000f60: 2079 6f75 2063 616e 2071 7565 7279 2074   you can query t
-00000f70: 6865 2070 6174 6820 6f66 2074 6865 2065  he path of the e
-00000f80: 7865 6375 7461 626c 6520 6265 696e 6720  xecutable being 
-00000f90: 7275 6e20 6279 2074 7970 696e 6720 6061  run by typing `a
-00000fa0: 7861 7070 2e46 756c 6c45 7865 5061 7468  xapp.FullExePath
-00000fb0: 602e 0d0a 0d0a 2323 2320 4261 7369 6320  `.....### Basic 
-00000fc0: 5573 6167 650d 0a0d 0a49 6620 7468 6520  Usage....If the 
-00000fd0: 636f 6e6e 6563 7469 6f6e 2069 7320 636f  connection is co
-00000fe0: 6d70 6c65 7465 2c20 6372 6561 7465 2061  mplete, create a
-00000ff0: 206e 6577 206d 6f64 656c 2061 6e64 2067   new model and g
-00001000: 6574 2061 6e20 696e 7465 7266 6163 6520  et an interface 
-00001010: 746f 2069 743a 0d0a 0d0a 6060 6070 7974  to it:....```pyt
-00001020: 686f 6e0d 0a6d 6f64 656c 4964 203d 2061  hon..modelId = a
-00001030: 7861 7070 2e4d 6f64 656c 732e 4e65 7728  xapp.Models.New(
-00001040: 290d 0a61 786d 6f64 656c 203d 2061 7861  )..axmodel = axa
-00001050: 7070 2e4d 6f64 656c 732e 4974 656d 5b6d  pp.Models.Item[m
-00001060: 6f64 656c 4964 5d0d 0a60 6060 0d0a 0d0a  odelId]..```....
-00001070: 4576 6572 7920 7469 6d65 2079 6f75 2063  Every time you c
-00001080: 7265 6174 6520 6120 6e65 7720 2a2a 4178  reate a new **Ax
-00001090: 6973 564d 2a2a 2069 6e73 7461 6e63 6520  isVM** instance 
-000010a0: 7769 7468 2074 6865 2060 7374 6172 745f  with the `start_
-000010b0: 4178 6973 564d 6020 636f 6d6d 616e 642c  AxisVM` command,
-000010c0: 2061 6e20 6174 7465 6d70 7420 6973 206d   an attempt is m
-000010d0: 6164 6520 746f 2069 6d70 6f72 7420 7468  ade to import th
-000010e0: 6520 7479 7065 206c 6962 7261 7279 2061  e type library a
-000010f0: 7320 6120 7079 7468 6f6e 206d 6f64 756c  s a python modul
-00001100: 652c 206f 7220 746f 2067 656e 6572 6174  e, or to generat
-00001110: 6520 6f6e 6520 6966 206e 6563 6573 7361  e one if necessa
-00001120: 7279 2e20 5468 6520 6765 6e65 7261 7465  ry. The generate
-00001130: 6420 6d6f 6475 6c65 2069 7320 7468 656e  d module is then
-00001140: 2061 6363 6573 7369 626c 6520 6173 2060   accessible as `
-00001150: 6178 6973 766d 2e63 6f6d 2e74 6c62 602e  axisvm.com.tlb`.
-00001160: 0d0a 0d0a 5468 6520 6e65 7874 2062 6c6f  ....The next blo
-00001170: 636b 206f 6620 636f 6d6d 616e 6473 2061  ck of commands a
-00001180: 6464 7320 6120 6c69 6e65 2074 6f20 7468  dds a line to th
-00001190: 6520 7363 656e 653a 0d0a 0d0a 6060 6070  e scene:....```p
-000011a0: 7974 686f 6e0d 0a66 726f 6d20 6178 6973  ython..from axis
-000011b0: 766d 2e63 6f6d 2e74 6c62 2069 6d70 6f72  vm.com.tlb impor
-000011c0: 7420 6c67 7453 7472 6169 6768 744c 696e  t lgtStraightLin
-000011d0: 652c 2052 4c69 6e65 4765 6f6d 4461 7461  e, RLineGeomData
-000011e0: 0d0a 6e31 203d 2061 786d 6f64 656c 2e4e  ..n1 = axmodel.N
-000011f0: 6f64 6573 2e41 6464 2830 2c20 302c 2030  odes.Add(0, 0, 0
-00001200: 290d 0a6e 3220 3d20 6178 6d6f 6465 6c2e  )..n2 = axmodel.
-00001210: 4e6f 6465 732e 4164 6428 312c 2031 2c20  Nodes.Add(1, 1, 
-00001220: 3129 0d0a 6c31 203d 2061 786d 6f64 656c  1)..l1 = axmodel
-00001230: 2e4c 696e 6573 2e41 6464 286e 312c 206e  .Lines.Add(n1, n
-00001240: 322c 206c 6774 5374 7261 6967 6874 4c69  2, lgtStraightLi
-00001250: 6e65 2c20 524c 696e 6547 656f 6d44 6174  ne, RLineGeomDat
-00001260: 6128 2929 0d0a 6060 600d 0a0d 0a50 7574  a())..```....Put
-00001270: 202a 2a41 7869 7356 4d2a 2a20 6f6e 2074   **AxisVM** on t
-00001280: 6f70 2061 6e64 2073 6361 6c65 206d 6f64  op and scale mod
-00001290: 656c 2074 6f20 6669 6c6c 2075 7020 7468  el to fill up th
-000012a0: 6520 6375 7272 656e 7420 7669 6577 3a0d  e current view:.
-000012b0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6178  ...```python..ax
-000012c0: 6170 702e 4272 696e 6754 6f46 726f 6e74  app.BringToFront
-000012d0: 2829 0d0a 6178 6d6f 6465 6c2e 4669 7449  ()..axmodel.FitI
-000012e0: 6e56 6965 7728 290d 0a60 6060 0d0a 0d0a  nView()..```....
-000012f0: 4174 2074 6865 2065 6e64 206f 6620 796f  At the end of yo
-00001300: 7572 2073 6573 7369 6f6e 2c20 7265 6c65  ur session, rele
-00001310: 6173 6520 7468 6520 636f 6e6e 6563 7469  ase the connecti
-00001320: 6f6e 2061 6e64 2063 6c6f 7365 2074 6865  on and close the
-00001330: 2061 7070 6c69 6361 7469 6f6e 2073 696d   application sim
-00001340: 706c 7920 6279 2074 7970 696e 670d 0a0d  ply by typing...
-00001350: 0a60 6060 7079 7468 6f6e 0d0a 6178 6170  .```python..axap
-00001360: 702e 556e 4c6f 6164 434f 4d43 6c69 656e  p.UnLoadCOMClien
-00001370: 7473 2829 0d0a 6178 6170 702e 5175 6974  ts()..axapp.Quit
-00001380: 2829 0d0a 6060 600d 0a0d 0a54 616b 6520  ()..```....Take 
-00001390: 6120 6c6f 6f6b 2061 7420 7468 6520 6a75  a look at the ju
-000013a0: 7079 7465 7220 6e6f 7465 626f 6f6b 7320  pyter notebooks 
-000013b0: 696e 2074 6865 205b 2a2a 2a65 7861 6d70  in the [***examp
-000013c0: 6c65 732a 2a2a 5d28 6874 7470 733a 2f2f  les***](https://
-000013d0: 6769 7468 7562 2e63 6f6d 2f41 7869 7356  github.com/AxisV
-000013e0: 4d2f 7079 6178 6973 766d 2f74 7265 652f  M/pyaxisvm/tree/
-000013f0: 6d61 696e 2f65 7861 6d70 6c65 7329 2066  main/examples) f
-00001400: 6f6c 6465 7220 6f66 2074 6869 7320 7265  older of this re
-00001410: 706f 7369 746f 7279 2066 6f72 206d 6f72  pository for mor
-00001420: 6520 7573 6520 6361 7365 732e 0d0a 0d0a  e use cases.....
-00001430: 2323 2054 6970 7320 616e 6420 5472 6963  ## Tips and Tric
-00001440: 6b73 0d0a 0d0a 2a2a 5079 4178 6973 564d  ks....**PyAxisVM
-00001450: 2a2a 2077 7261 7073 2075 7020 7468 6520  ** wraps up the 
-00001460: 434f 4d20 7479 7065 206c 6962 7261 7279  COM type library
-00001470: 2c20 616c 6c6f 7769 6e67 2075 7365 7273  , allowing users
-00001480: 2074 6f20 6578 706c 6f69 7420 7468 6520   to exploit the 
-00001490: 656c 6567 616e 7420 616e 6420 636f 6e63  elegant and conc
-000014a0: 6973 6520 7379 6e74 6178 2074 6861 7420  ise syntax that 
-000014b0: 5079 7468 6f6e 2070 726f 7669 6465 732c  Python provides,
-000014c0: 2077 6869 6c65 2073 7469 6c6c 206c 6561   while still lea
-000014d0: 7669 6e67 2065 7665 7279 7468 696e 6720  ving everything 
-000014e0: 6f6e 2074 6865 2074 6162 6c65 2066 6f72  on the table for
-000014f0: 206c 6567 6163 7920 636f 6465 2e20 4966   legacy code. If
-00001500: 2066 6f72 2065 7861 6d70 6c65 2c20 7765   for example, we
-00001510: 2077 616e 7465 6420 746f 2063 616c 6375   wanted to calcu
-00001520: 6c61 7465 2061 7265 6173 206f 6620 7375  late areas of su
-00001530: 7266 6163 6520 656c 656d 656e 7473 2c20  rface elements, 
-00001540: 7468 6520 6f75 7420 6f66 2062 6f78 2073  the out of box s
-00001550: 6f6c 7574 696f 6e20 776f 756c 6420 6265  olution would be
-00001560: 2073 6f6d 6574 6869 6e67 206c 696b 650d   something like.
-00001570: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6172  ...```python..ar
-00001580: 6561 7320 3d20 5b5d 0d0a 666f 7220 6920  eas = []..for i 
-00001590: 696e 2072 616e 6765 2861 786d 6f64 656c  in range(axmodel
-000015a0: 2e53 7572 6661 6365 732e 436f 756e 7429  .Surfaces.Count)
-000015b0: 3a0d 0a20 2020 2061 7265 6173 2e61 7070  :..    areas.app
-000015c0: 656e 6428 6178 6d6f 6465 6c2e 5375 7266  end(axmodel.Surf
-000015d0: 6163 6573 2e49 7465 6d5b 692b 315d 2e41  aces.Item[i+1].A
-000015e0: 7265 6129 0d0a 6060 600d 0a0d 0a6f 7220  rea)..```....or 
-000015f0: 7573 696e 6720 6120 6c69 7374 2063 6f6d  using a list com
-00001600: 7072 6568 656e 7369 6f6e 0d0a 0d0a 6060  prehension....``
-00001610: 6070 7974 686f 6e0d 0a61 7265 6173 203d  `python..areas =
-00001620: 205b 6178 6d6f 6465 6c2e 5375 7266 6163   [axmodel.Surfac
-00001630: 6573 2e49 7465 6d5b 692b 315d 2e41 7265  es.Item[i+1].Are
-00001640: 6120 666f 7220 6920 696e 2072 616e 6765  a for i in range
-00001650: 2861 786d 6f64 656c 2e53 7572 6661 6365  (axmodel.Surface
-00001660: 732e 436f 756e 7429 5d0d 0a60 6060 0d0a  s.Count)]..```..
-00001670: 0d0a 5769 7468 202a 2a50 7941 7869 7356  ..With **PyAxisV
-00001680: 4d2a 2a2c 2065 7661 6c75 6174 696f 6e20  M**, evaluation 
-00001690: 6f66 2073 696e 676c 6520 6974 656d 2070  of single item p
-000016a0: 726f 7065 7274 6965 7320 6f76 6572 2063  roperties over c
-000016b0: 6f6c 6c65 6374 696f 6e73 2069 7320 6173  ollections is as
-000016c0: 2065 6173 7920 6173 0d0a 0d0a 6060 6070   easy as....```p
-000016d0: 7974 686f 6e0d 0a61 7265 6173 203d 205b  ython..areas = [
-000016e0: 732e 4172 6561 2066 6f72 2073 2069 6e20  s.Area for s in 
-000016f0: 6178 6d6f 6465 6c2e 5375 7266 6163 6573  axmodel.Surfaces
-00001700: 5d0d 0a60 6060 0d0a 0d0a 6f72 2073 696d  ]..```....or sim
-00001710: 706c 790d 0a0d 0a60 6060 7079 7468 6f6e  ply....```python
-00001720: 0d0a 6172 6561 7320 3d20 6178 6d6f 6465  ..areas = axmode
-00001730: 6c2e 5375 7266 6163 6573 5b3a 5d2e 4172  l.Surfaces[:].Ar
-00001740: 6561 0d0a 6060 600d 0a0d 0a43 6c69 636b  ea..```....Click
-00001750: 205b 2a2a 2a68 6572 652a 2a2a 5d28 6874   [***here***](ht
-00001760: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001770: 2f41 7869 7356 4d2f 7079 6178 6973 766d  /AxisVM/pyaxisvm
-00001780: 2f62 6c6f 622f 3661 6266 6562 6466 6432  /blob/6abfebdfd2
-00001790: 3661 3736 3732 3138 3336 6531 6234 3930  6a76721836e1b490
-000017a0: 3436 3564 3166 3561 3437 3461 3833 2f74  465d1f5a474a83/t
-000017b0: 6970 735f 616e 645f 7472 6963 6b73 2e6d  ips_and_tricks.m
-000017c0: 6429 2074 6f20 6765 7420 6120 6675 6c6c  d) to get a full
-000017d0: 206f 7665 7276 6965 7720 6162 6f75 7420   overview about 
-000017e0: 7468 6520 7079 7468 6f6e 6963 2075 7361  the pythonic usa
-000017f0: 6765 206f 6620 7468 6520 6c69 6272 6172  ge of the librar
-00001800: 792e 0d0a 0d0a 2323 204c 6963 656e 7365  y.....## License
-00001810: 0d0a 0d0a 2a2a 5079 4178 6973 564d 2a2a  ....**PyAxisVM**
-00001820: 2069 7320 6c69 6365 6e73 6564 2075 6e64   is licensed und
-00001830: 6572 2074 6865 205b 4d49 5420 6c69 6365  er the [MIT lice
-00001840: 6e73 655d 2868 7474 7073 3a2f 2f6f 7065  nse](https://ope
-00001850: 6e73 6f75 7263 652e 6f72 672f 6c69 6365  nsource.org/lice
-00001860: 6e73 652f 6d69 742f 292e 0d0a 0d0a 5468  nse/mit/).....Th
-00001870: 6973 206d 6f64 756c 652c 202a 2a50 7941  is module, **PyA
-00001880: 7869 7356 4d2a 2a20 6d61 6b65 7320 6e6f  xisVM** makes no
-00001890: 2063 6f6d 6d65 7263 6961 6c20 636c 6169   commercial clai
-000018a0: 6d20 6f76 6572 2041 7869 7356 4d20 7768  m over AxisVM wh
-000018b0: 6174 736f 6576 6572 2e20 5468 6973 2074  atsoever. This t
-000018c0: 6f6f 6c20 6578 7465 6e64 7320 7468 6520  ool extends the 
-000018d0: 6675 6e63 7469 6f6e 616c 6974 7920 6f66  functionality of
-000018e0: 202a 2a41 7869 7356 4d2a 2a20 6279 2061   **AxisVM** by a
-000018f0: 6464 696e 6720 6120 5079 7468 6f6e 2069  dding a Python i
-00001900: 6e74 6572 6661 6365 2074 6f20 7468 6520  nterface to the 
-00001910: 2a2a 4178 6973 564d 2a2a 2043 4f4d 2073  **AxisVM** COM s
-00001920: 6572 7669 6365 2077 6974 686f 7574 2063  ervice without c
-00001930: 6861 6e67 696e 6720 7468 6520 636f 7265  hanging the core
-00001940: 2062 6568 6176 696f 7220 6f72 206c 6963   behavior or lic
-00001950: 656e 7365 206f 6620 7468 6520 6f72 6967  ense of the orig
-00001960: 696e 616c 2073 6f66 7477 6172 652e 2054  inal software. T
-00001970: 6865 2075 7365 206f 6620 2a2a 5079 4178  he use of **PyAx
-00001980: 6973 564d 2a2a 2072 6571 7569 7265 7320  isVM** requires 
-00001990: 6120 6c65 6761 6c6c 7920 6c69 6365 6e73  a legally licens
-000019a0: 6564 206c 6f63 616c 2063 6f70 7920 6f66  ed local copy of
-000019b0: 202a 2a41 7869 7356 4d2a 2a2e 0d0a        **AxisVM**...
+00000000: 2320 4765 7474 696e 6720 5374 6172 7465  # Getting Starte
+00000010: 640d 0a0d 0a54 6865 2067 6574 7469 6e67  d....The getting
+00000020: 2073 7461 7274 6564 206c 6962 7261 7279   started library
+00000030: 2068 656c 7073 2079 6f75 2074 6f20 6d61   helps you to ma
+00000040: 6b65 2074 6865 2066 6972 7374 2073 7465  ke the first ste
+00000050: 7073 206f 6620 796f 7572 206a 6f75 726e  ps of your journ
+00000060: 6579 2065 7870 6c6f 7269 6e67 2074 6865  ey exploring the
+00000070: 206c 6962 7261 7279 2e20 5765 2067 7569   library. We gui
+00000080: 6465 2079 6f75 2074 6872 6f75 6768 2074  de you through t
+00000090: 6865 2069 6e73 7461 6c6c 6174 696f 6e20  he installation 
+000000a0: 7072 6f63 6573 7320 616e 6420 7465 6163  process and teac
+000000b0: 6820 796f 7520 686f 7720 746f 2065 6666  h you how to eff
+000000c0: 6963 6965 6e74 6c79 2075 7365 2074 6865  iciently use the
+000000d0: 2064 6f63 756d 656e 7461 7469 6f6e 2c20   documentation, 
+000000e0: 686f 7065 6675 6c6c 7920 6d69 6e69 6d69  hopefully minimi
+000000f0: 7a69 6e67 2079 6f75 7220 6c65 6172 6e69  zing your learni
+00000100: 6e67 2063 7572 7665 2e0d 0a0d 0a23 2320  ng curve.....## 
+00000110: 5072 6572 6571 7569 7369 7465 730d 0a0d  Prerequisites...
+00000120: 0a49 6e20 6f72 6465 7220 746f 2075 7365  .In order to use
+00000130: 2050 7974 686f 6e20 7769 7468 2041 7869   Python with Axi
+00000140: 7356 4d2c 2079 6f75 206e 6565 6420 746f  sVM, you need to
+00000150: 2068 6176 650d 0a0d 0a2d 2041 206c 6963   have....- A lic
+00000160: 656e 7365 6420 7665 7273 696f 6e20 6f66  ensed version of
+00000170: 2041 7869 7356 4d20 696e 7374 616c 6c65   AxisVM installe
+00000180: 6420 6f6e 2079 6f75 7220 636f 6d70 7574  d on your comput
+00000190: 6572 0d0a 2d20 5079 7468 6f6e 203e 3d20  er..- Python >= 
+000001a0: 332e 3820 616e 6420 3c3d 2033 2e31 300d  3.8 and <= 3.10.
+000001b0: 0a2d 2054 6869 7320 6c69 6272 6172 7920  .- This library 
+000001c0: 2873 6565 2069 6e73 7461 6c6c 6174 696f  (see installatio
+000001d0: 6e20 6c61 7465 7229 0d0a 2d20 5468 6520  n later)..- The 
+000001e0: 4178 6973 564d 2043 4f4d 2041 5049 2052  AxisVM COM API R
+000001f0: 4546 4552 454e 4345 2047 5549 452e 2054  EFERENCE GUIE. T
+00000200: 6869 7320 6973 2061 2070 6466 2064 6f63  his is a pdf doc
+00000210: 756d 656e 742c 2061 7661 6c69 6162 6c65  ument, avaliable
+00000220: 2061 7420 7468 6520 5b64 6f77 6e6c 6f61   at the [downloa
+00000230: 6473 5d28 6874 7470 733a 2f2f 6178 6973  ds](https://axis
+00000240: 766d 2e65 752f 6178 6973 766d 2d64 6f77  vm.eu/axisvm-dow
+00000250: 6e6c 6f61 6473 2f29 206f 6620 4178 6973  nloads/) of Axis
+00000260: 564d 2773 2068 6f6d 6570 6167 652e 0d0a  VM's homepage...
+00000270: 0d0a 2323 2049 6e73 7461 6c6c 6174 696f  ..## Installatio
+00000280: 6e0d 0a0d 0a23 2323 2052 6567 6973 7465  n....### Registe
+00000290: 7220 4178 6973 564d 2773 2054 7970 6520  r AxisVM's Type 
+000002a0: 4c69 6272 6172 790d 0a0d 0a49 6620 7468  Library....If th
+000002b0: 6973 2069 7320 6e6f 7420 796f 7572 2066  is is not your f
+000002c0: 6972 7374 2074 696d 6520 7573 696e 6720  irst time using 
+000002d0: 2a2a 4178 6973 564d 2a2a 2074 6872 6f75  **AxisVM** throu
+000002e0: 6768 2061 2043 4f4d 2069 6e74 6572 6661  gh a COM interfa
+000002f0: 6365 206f 6e20 796f 7572 206d 6163 6869  ce on your machi
+00000300: 6e65 2c20 796f 7520 7368 6f75 6c64 2061  ne, you should a
+00000310: 6c72 6561 6479 2068 6176 6520 6120 7265  lready have a re
+00000320: 6769 7374 6572 6564 2074 7970 6520 6c69  gistered type li
+00000330: 6272 6172 7920 616e 6420 796f 7520 6361  brary and you ca
+00000340: 6e20 736b 6970 2074 6869 7320 7374 6570  n skip this step
+00000350: 2e20 4f74 6865 7277 6973 652c 2079 6f75  . Otherwise, you
+00000360: 2068 6176 6520 746f 2072 6567 6973 7465   have to registe
+00000370: 7220 7468 6520 7479 7065 206c 6962 7261  r the type libra
+00000380: 7279 206f 6620 796f 7572 2041 7869 7356  ry of your AxisV
+00000390: 4d20 6170 706c 6963 6174 696f 6e2e 2044  M application. D
+000003a0: 6966 6665 7265 6e74 2076 6572 7369 6f6e  ifferent version
+000003b0: 7320 636f 6d65 2077 6974 6820 6469 6666  s come with diff
+000003c0: 6572 656e 7420 7479 7065 206c 6962 7261  erent type libra
+000003d0: 7269 6573 2c20 736f 2079 6f75 206d 6967  ries, so you mig
+000003e0: 6874 2072 6564 6f20 7468 6973 2073 7465  ht redo this ste
+000003f0: 7020 7768 656e 2079 6f75 2075 7064 6174  p when you updat
+00000400: 6520 746f 2061 206e 6577 2076 6572 7369  e to a new versi
+00000410: 6f6e 2e20 4174 2061 6c6c 2074 696d 6573  on. At all times
+00000420: 2c20 2a2a 6f6c 6465 7220 7665 7273 696f  , **older versio
+00000430: 6e73 206d 7573 7420 6265 2075 6e72 6567  ns must be unreg
+00000440: 6973 7465 7265 6420 6672 6f6d 2074 6865  istered from the
+00000450: 2057 696e 646f 7773 2072 6567 6973 7472   Windows registr
+00000460: 7920 6265 666f 7265 206e 6577 2072 6567  y before new reg
+00000470: 6973 7472 6174 696f 6e73 212a 2a0d 0a0d  istrations!**...
+00000480: 0a54 6f20 6861 7665 2079 6f75 7220 4178  .To have your Ax
+00000490: 6973 564d 2072 6567 6973 7465 7265 642c  isVM registered,
+000004a0: 206c 6f63 6174 6520 7468 6520 666f 6c64   locate the fold
+000004b0: 6572 206f 6e20 796f 7572 2066 696c 6573  er on your files
+000004c0: 7973 7465 6d20 4178 6973 564d 2069 7320  ystem AxisVM is 
+000004d0: 696e 7374 616c 6c65 6420 696e 746f 2e20  installed into. 
+000004e0: 496e 2074 6861 7420 666f 6c64 6572 2079  In that folder y
+000004f0: 6f75 2073 686f 756c 6420 7365 6520 6120  ou should see a 
+00000500: 6669 6c65 2063 616c 6c65 6420 2a21 5245  file called *!RE
+00000510: 4749 5354 4552 5f41 5849 5356 4d5f 5836  GISTER_AXISVM_X6
+00000520: 342a 2061 6e64 202a 2152 4547 4953 5445  4* and *!REGISTE
+00000530: 525f 4158 4953 564d 2a2e 2044 6f75 626c  R_AXISVM*. Doubl
+00000540: 6520 636c 6963 6b20 6f6e 2074 6865 2066  e click on the f
+00000550: 6972 7374 2066 6f72 2061 2036 342d 6269  irst for a 64-bi
+00000560: 742c 206f 7220 7468 6520 7365 636f 6e64  t, or the second
+00000570: 206f 6e65 2066 6f72 2061 2033 322d 6269   one for a 32-bi
+00000580: 7420 696e 7374 616c 6c61 7469 6f6e 2e20  t installation. 
+00000590: 2a2a 4974 2069 7320 696d 706f 7274 616e  **It is importan
+000005a0: 7420 746f 2072 6567 6973 7465 7220 6f6e  t to register on
+000005b0: 6c79 2074 6865 2076 6572 7369 6f6e 2074  ly the version t
+000005c0: 6861 7420 6973 2072 6571 7569 7265 6420  hat is required 
+000005d0: 616e 6420 6d61 7463 6865 7320 7769 7468  and matches with
+000005e0: 2074 6865 2076 6572 7369 6f6e 206f 6620   the version of 
+000005f0: 696e 7374 616c 6c65 6420 4178 6973 564d  installed AxisVM
+00000600: 2a2a 2e0d 0a0d 0a54 6f20 756e 7265 6769  **.....To unregi
+00000610: 7374 6572 2061 2074 7970 6520 6c69 6272  ster a type libr
+00000620: 6172 792c 2074 6865 2073 7465 7020 6973  ary, the step is
+00000630: 2073 696d 696c 6172 2c20 6275 7420 6e6f   similar, but no
+00000640: 7720 796f 7520 7573 6520 7468 6520 6669  w you use the fi
+00000650: 6c65 7320 2a21 554e 5245 4749 5354 4552  les *!UNREGISTER
+00000660: 5f41 5849 5356 4d5f 5836 342a 2061 6e64  _AXISVM_X64* and
+00000670: 202a 2155 4e52 4547 4953 5445 525f 4158   *!UNREGISTER_AX
+00000680: 4953 564d 2a2e 0d0a 0d0a 2323 2320 496e  ISVM*.....### In
+00000690: 7374 616c 6c20 7468 6520 5079 7468 6f6e  stall the Python
+000006a0: 2070 6163 6b61 6765 2066 6f72 2041 7869   package for Axi
+000006b0: 7356 4d0d 0a0d 0a54 6869 7320 6973 206f  sVM....This is o
+000006c0: 7074 696f 6e61 6c2c 2062 7574 2077 6520  ptional, but we 
+000006d0: 7375 6767 6573 7420 796f 7520 746f 2063  suggest you to c
+000006e0: 7265 6174 6520 6120 6465 6469 6361 7465  reate a dedicate
+000006f0: 6420 7669 7274 7561 6c20 656e 7669 726f  d virtual enviro
+00000700: 6d65 6e74 2061 7420 616c 6c20 7469 6d65  ment at all time
+00000710: 7320 746f 2061 766f 6964 2063 6f6e 666c  s to avoid confl
+00000720: 6963 7473 2077 6974 6820 796f 7572 206f  icts with your o
+00000730: 7468 6572 2070 726f 6a65 6374 732e 2043  ther projects. C
+00000740: 7265 6174 6520 6120 666f 6c64 6572 2c20  reate a folder, 
+00000750: 6f70 656e 2061 2063 6f6d 6d61 6e64 2073  open a command s
+00000760: 6865 6c6c 2069 6e20 7468 6174 2066 6f6c  hell in that fol
+00000770: 6465 7220 616e 6420 7573 6520 7468 6520  der and use the 
+00000780: 666f 6c6c 6f77 696e 6720 636f 6d6d 616e  following comman
+00000790: 640d 0a0d 0a60 6060 636f 6e73 6f6c 650d  d....```console.
+000007a0: 0a3e 3e3e 2070 7974 686f 6e20 2d6d 2076  .>>> python -m v
+000007b0: 656e 7620 7665 6e76 5f6e 616d 650d 0a60  env venv_name..`
+000007c0: 6060 0d0a 0d0a 4f6e 6365 2074 6865 2065  ``....Once the e
+000007d0: 6e76 6972 6f6d 656e 7420 6973 2063 7265  nviroment is cre
+000007e0: 6174 6564 2c20 6163 7469 7661 7465 2069  ated, activate i
+000007f0: 7420 7669 6120 7479 7069 6e67 0d0a 0d0a  t via typing....
+00000800: 6060 6063 6f6e 736f 6c65 0d0a 3e3e 3e20  ```console..>>> 
+00000810: 2e5c 7665 6e76 5f6e 616d 655c 5363 7269  .\venv_name\Scri
+00000820: 7074 735c 6163 7469 7661 7465 0d0a 6060  pts\activate..``
+00000830: 600d 0a0d 0a54 6865 202a 2a41 7869 7356  `....The **AxisV
+00000840: 4d2a 2a20 7079 7468 6f6e 2070 6163 6b61  M** python packa
+00000850: 6765 2063 616e 2062 6520 696e 7374 616c  ge can be instal
+00000860: 6c65 6420 2865 6974 6865 7220 696e 2061  led (either in a
+00000870: 2076 6972 7475 616c 2065 6e76 6972 6f6d   virtual envirom
+00000880: 656e 7420 6f72 2067 6c6f 6261 6c6c 7929  ent or globally)
+00000890: 2066 726f 6d20 5079 5049 2075 7369 6e67   from PyPI using
+000008a0: 2060 7069 7060 206f 6e20 5079 7468 6f6e   `pip` on Python
+000008b0: 203e 3d33 2e38 203c 3d33 2e31 303a 0d0a   >=3.8 <=3.10:..
+000008c0: 0d0a 6060 6063 6f6e 736f 6c65 0d0a 3e3e  ..```console..>>
+000008d0: 3e20 7069 7020 696e 7374 616c 6c20 6178  > pip install ax
+000008e0: 6973 766d 0d0a 6060 600d 0a0d 0a23 2323  isvm..```....###
+000008f0: 204c 6175 6e63 6820 4178 6973 564d 2066   Launch AxisVM f
+00000900: 726f 6d20 5079 7468 6f6e 0d0a 0d0a 5468  rom Python....Th
+00000910: 6520 6061 7869 7376 6d2e 636f 6d2e 636c  e `axisvm.com.cl
+00000920: 6965 6e74 6020 7375 626d 6f64 756c 6520  ient` submodule 
+00000930: 696d 706c 656d 656e 7473 2076 6172 696f  implements vario
+00000940: 7573 2074 6f6f 6c73 2074 6f20 6861 6e64  us tools to hand
+00000950: 6c65 2074 6865 2063 6c69 656e 7420 7369  le the client si
+00000960: 6465 206f 7065 7261 7469 6f6e 7320 6f66  de operations of
+00000970: 2063 7265 6174 696e 6720 6120 434f 4d20   creating a COM 
+00000980: 636f 6e6e 6563 7469 6f6e 2e20 496d 706f  connection. Impo
+00000990: 7274 2074 6865 206d 6f64 756c 6520 616e  rt the module an
+000009a0: 6420 7374 6172 7420 6120 6e65 7720 6170  d start a new ap
+000009b0: 706c 6963 6174 696f 6e20 696e 7374 616e  plication instan
+000009c0: 6365 2077 6974 6820 7468 6520 6073 7461  ce with the `sta
+000009d0: 7274 5f41 7869 7356 4d60 206d 6574 686f  rt_AxisVM` metho
+000009e0: 643a 0d0a 0d0a 6060 6070 7974 686f 6e0d  d:....```python.
+000009f0: 0a66 726f 6d20 6178 6973 766d 2e63 6f6d  .from axisvm.com
+00000a00: 2e63 6c69 656e 7420 696d 706f 7274 2073  .client import s
+00000a10: 7461 7274 5f41 7869 7356 4d0d 0a61 7861  tart_AxisVM..axa
+00000a20: 7070 203d 2073 7461 7274 5f41 7869 7356  pp = start_AxisV
+00000a30: 4d28 7669 7369 626c 653d 5472 7565 290d  M(visible=True).
+00000a40: 0a60 6060 0d0a 0d0a 546f 2074 6573 7420  .```....To test 
+00000a50: 7468 6520 636f 6e6e 6563 7469 6f6e 2c20  the connection, 
+00000a60: 796f 7520 6361 6e20 7175 6572 7920 7468  you can query th
+00000a70: 6520 7061 7468 206f 6620 7468 6520 6578  e path of the ex
+00000a80: 6563 7574 6162 6c65 2062 6569 6e67 2072  ecutable being r
+00000a90: 756e 2062 7920 7479 7069 6e67 2060 6178  un by typing `ax
+00000aa0: 6170 702e 4675 6c6c 4578 6550 6174 6860  app.FullExePath`
+00000ab0: 2e0d 0a0d 0a23 2323 2043 6f6e 6e65 6374  .....### Connect
+00000ac0: 696e 6720 746f 2061 2072 756e 6e69 6e67  ing to a running
+00000ad0: 2069 6e73 7461 6e63 6520 6f66 2041 7869   instance of Axi
+00000ae0: 7356 4d0d 0a0d 0a49 6620 796f 7520 7761  sVM....If you wa
+00000af0: 6e74 2074 6f20 6265 2061 626c 6520 746f  nt to be able to
+00000b00: 2063 6f6e 6e65 6374 2074 6f20 616e 2061   connect to an a
+00000b10: 6c72 6561 6479 2072 756e 6e69 6e67 2069  lready running i
+00000b20: 6e73 7461 6e63 6520 6f66 2041 7869 7356  nstance of AxisV
+00000b30: 4d2c 2079 6f75 206e 6565 6420 746f 2073  M, you need to s
+00000b40: 7461 7274 2074 6865 2065 7865 6375 7461  tart the executa
+00000b50: 626c 6520 7769 7468 2074 6865 2060 2f4d  ble with the `/M
+00000b60: 554c 5449 494e 5354 414e 4345 434f 4d43  ULTIINSTANCECOMC
+00000b70: 4c49 454e 5453 6020 7061 7261 6d65 7465  LIENTS` paramete
+00000b80: 722e 2054 6865 2073 696d 706c 6573 7420  r. The simplest 
+00000b90: 7761 7920 6f66 2061 6368 6965 7669 6e67  way of achieving
+00000ba0: 2074 6869 7320 6973 2074 6f20 6c6f 6361   this is to loca
+00000bb0: 7465 2074 6865 2069 636f 6e20 6f66 2041  te the icon of A
+00000bc0: 7869 7356 4d20 6f6e 2079 6f75 7220 6465  xisVM on your de
+00000bd0: 736b 746f 7020 2849 2061 7373 756d 6520  sktop (I assume 
+00000be0: 796f 7520 6861 7665 206f 6e65 2920 616e  you have one) an
+00000bf0: 6420 6d6f 6469 6679 2074 6865 2074 6172  d modify the tar
+00000c00: 6765 7420 6f66 2069 7420 746f 2065 6e64  get of it to end
+00000c10: 2077 6974 6820 602f 4d55 4c54 4949 4e53   with `/MULTIINS
+00000c20: 5441 4e43 4543 4f4d 434c 4945 4e54 5360  TANCECOMCLIENTS`
+00000c30: 2e20 5468 6520 7461 7267 6574 206f 6620  . The target of 
+00000c40: 796f 7572 2073 686f 7274 6375 7420 7368  your shortcut sh
+00000c50: 6f75 6c64 206c 6f6f 6b20 6c69 6b65 0d0a  ould look like..
+00000c60: 0d0a 2243 3a5c 4178 6973 564d 5c41 7869  .."C:\AxisVM\Axi
+00000c70: 7356 4d58 375c 4178 6973 564d 5f78 3634  sVMX7\AxisVM_x64
+00000c80: 2e65 7865 2220 2f4d 554c 5449 494e 5354  .exe" /MULTIINST
+00000c90: 414e 4345 434f 4d43 4c49 454e 5453 0d0a  ANCECOMCLIENTS..
+00000ca0: 0d0a 6f72 2073 6f6d 6574 6869 6e67 2063  ..or something c
+00000cb0: 6c6f 7365 2074 6f20 6974 2e20 5468 656e  lose to it. Then
+00000cc0: 2c20 796f 7520 6361 6e20 636f 6e6e 6563  , you can connec
+00000cd0: 7420 746f 2061 2072 756e 6e69 6e67 2041  t to a running A
+00000ce0: 7869 7356 4d20 696e 7374 616e 6365 2062  xisVM instance b
+00000cf0: 7920 7573 696e 6720 6120 736c 6967 6874  y using a slight
+00000d00: 6c79 2064 6966 6665 7265 6e74 2076 6572  ly different ver
+00000d10: 7369 6f6e 206f 6620 7468 6520 7072 6576  sion of the prev
+00000d20: 696f 7573 2063 6f64 6520 736e 6970 7065  ious code snippe
+00000d30: 743a 0d0a 0d0a 6060 6070 7974 686f 6e0d  t:....```python.
+00000d40: 0a66 726f 6d20 6178 6973 766d 2e63 6f6d  .from axisvm.com
+00000d50: 2e63 6c69 656e 7420 696d 706f 7274 2073  .client import s
+00000d60: 7461 7274 5f41 7869 7356 4d0d 0a61 7861  tart_AxisVM..axa
+00000d70: 7070 203d 2073 7461 7274 5f41 7869 7356  pp = start_AxisV
+00000d80: 4d28 7669 7369 626c 653d 5472 7565 2c20  M(visible=True, 
+00000d90: 6a6f 696e 3d54 7275 6529 0d0a 6060 600d  join=True)..```.
+00000da0: 0a0d 0a48 6572 652c 2074 6865 2060 6a6f  ...Here, the `jo
+00000db0: 696e 3d54 7275 6560 2070 6172 616d 6574  in=True` paramet
+00000dc0: 6572 2074 656c 6c73 2074 6865 206c 6962  er tells the lib
+00000dd0: 7261 7279 2074 6861 7420 6966 2079 6f75  rary that if you
+00000de0: 2764 2070 7265 6665 7220 746f 206a 6f69  'd prefer to joi
+00000df0: 6e20 6120 7275 6e6e 696e 6720 696e 7374  n a running inst
+00000e00: 616e 6365 2c20 6966 2074 6865 7265 2069  ance, if there i
+00000e10: 7320 616e 792e 2049 6620 7468 6572 6520  s any. If there 
+00000e20: 6973 206e 6f20 7275 6e6e 696e 6720 696e  is no running in
+00000e30: 7374 616e 6365 2c20 6120 6e65 7720 696e  stance, a new in
+00000e40: 7374 616e 6365 206f 6620 4178 6973 564d  stance of AxisVM
+00000e50: 2069 7320 6372 6561 7465 642e 0d0a 0d0a   is created.....
+00000e60: 2323 2048 6f77 2074 6f20 7573 6520 7468  ## How to use th
+00000e70: 6520 4150 490d 0a0d 0a54 6865 2050 7974  e API....The Pyt
+00000e80: 686f 6e20 6c69 6272 6172 7920 6861 7320  hon library has 
+00000e90: 7477 6f20 6c61 7965 7273 2e20 5468 6520  two layers. The 
+00000ea0: 6669 7273 7420 6f6e 6520 6973 2074 6865  first one is the
+00000eb0: 2072 6177 2074 7970 6520 6c69 6272 6172   raw type librar
+00000ec0: 7920 6578 7472 6163 7465 6420 6672 6f6d  y extracted from
+00000ed0: 2041 7869 7356 4d20 7573 696e 6720 7468   AxisVM using th
+00000ee0: 6520 6063 6f6d 7074 7970 6573 6020 7061  e `comptypes` pa
+00000ef0: 636b 6167 652e 2057 6520 6172 6520 776f  ckage. We are wo
+00000f00: 726b 696e 6720 6f6e 2061 6e20 6f6e 6c69  rking on an onli
+00000f10: 6e65 2076 6572 7369 6f6e 206f 6620 6974  ne version of it
+00000f20: 2c20 756e 7469 6c20 7468 6174 2074 6865  , until that the
+00000f30: 2064 6f63 756d 656e 7461 7469 6f6e 206f   documentation o
+00000f40: 6620 7468 6973 206c 6179 6572 2069 7320  f this layer is 
+00000f50: 6f6e 6c79 2061 7661 696c 6162 6c65 2069  only available i
+00000f60: 6e20 7064 6620 666f 726d 6174 2c20 7468  n pdf format, th
+00000f70: 6174 2079 6f75 2073 686f 756c 6420 616c  at you should al
+00000f80: 7265 6164 7920 706f 7365 7373 2061 7420  ready posess at 
+00000f90: 7468 6520 6d6f 6d65 6e74 206f 6620 7265  the moment of re
+00000fa0: 6164 696e 6720 7468 6973 206e 6f74 6562  ading this noteb
+00000fb0: 6f6f 6b2e 2049 6620 796f 7520 646f 6e27  ook. If you don'
+00000fc0: 7420 6861 7665 2069 7420 7965 742c 2067  t have it yet, g
+00000fd0: 6f20 746f 206f 7572 2077 6562 7369 7465  o to our website
+00000fe0: 2c20 616e 6420 6c6f 6f6b 2066 6f72 2069  , and look for i
+00000ff0: 7420 756e 6465 7220 5b64 6f77 6e6c 6f61  t under [downloa
+00001000: 6473 5d28 6874 7470 733a 2f2f 6178 6973  ds](https://axis
+00001010: 766d 2e65 752f 6178 6973 766d 2d64 6f77  vm.eu/axisvm-dow
+00001020: 6e6c 6f61 6473 2f29 2e20 4974 2069 7320  nloads/). It is 
+00001030: 696d 706f 7274 616e 7420 7468 6174 2074  important that t
+00001040: 6869 7320 646f 6375 6d65 6e74 6174 696f  his documentatio
+00001050: 6e20 6973 206c 616e 6775 6167 6520 6167  n is language ag
+00001060: 6e6f 7374 6963 2c20 616e 6420 796f 7520  nostic, and you 
+00001070: 776f 6e27 7420 6669 6e64 2074 6865 2050  won't find the P
+00001080: 7974 686f 6e69 6320 7665 7273 696f 6e73  ythonic versions
+00001090: 206f 6620 7468 6520 6675 6e63 7469 6f6e   of the function
+000010a0: 2063 616c 6c73 2064 6972 6563 746c 7920   calls directly 
+000010b0: 696e 2069 742c 2062 7574 2064 6f6e 2774  in it, but don't
+000010c0: 2077 6f72 7279 2c20 7468 6520 5b75 7365   worry, the [use
+000010d0: 7220 6775 6964 655d 2875 7365 725f 6775  r guide](user_gu
+000010e0: 6964 652e 7273 7429 2068 6173 2073 6576  ide.rst) has sev
+000010f0: 6572 616c 2065 7861 6d70 6c65 7320 746f  eral examples to
+00001100: 2068 656c 7020 796f 7520 6765 7420 7468   help you get th
+00001110: 6520 6861 6e67 206f 6620 6974 2e20 4166  e hang of it. Af
+00001120: 7465 7220 6c69 7474 6c65 2070 7261 6374  ter little pract
+00001130: 6963 696e 672c 2079 6f75 2077 696c 6c20  icing, you will 
+00001140: 6b6e 6f77 2068 6f77 2074 6f20 6361 6c6c  know how to call
+00001150: 2061 6e79 206f 6620 7468 6520 4150 4920   any of the API 
+00001160: 656e 6470 6f69 6e74 7320 6c69 7374 6564  endpoints listed
+00001170: 2069 6e20 7468 6520 7064 6620 646f 6375   in the pdf docu
+00001180: 6d65 6e74 2e0d 0a0d 0a23 2323 2042 6173  ment.....### Bas
+00001190: 6963 2041 5049 2075 7361 6765 0d0a 0d0a  ic API usage....
+000011a0: 4669 7274 7320 6f66 2061 6c6c 2c20 7765  Firts of all, we
+000011b0: 206e 6565 6420 6120 7275 6e6e 6e69 6e67   need a runnning
+000011c0: 2041 7869 7356 4d20 6569 7468 6572 2069   AxisVM either i
+000011d0: 6e20 7468 6520 6261 636b 6772 6f75 6e64  n the background
+000011e0: 2c20 6f72 2077 6974 6820 7468 6520 6772  , or with the gr
+000011f0: 6170 6869 6361 6c20 696e 7465 7266 6163  aphical interfac
+00001200: 652e 0d0a 0d0a 6060 6070 7974 686f 6e0d  e.....```python.
+00001210: 0a66 726f 6d20 6178 6973 766d 2e63 6f6d  .from axisvm.com
+00001220: 2e63 6c69 656e 7420 696d 706f 7274 2073  .client import s
+00001230: 7461 7274 5f41 7869 7356 4d0d 0a61 7876  tart_AxisVM..axv
+00001240: 6d20 3d20 7374 6172 745f 4178 6973 564d  m = start_AxisVM
+00001250: 2876 6973 6962 6c65 3d54 7275 652c 2064  (visible=True, d
+00001260: 6165 6d6f 6e3d 5472 7565 290d 0a60 6060  aemon=True)..```
+00001270: 0d0a 0d0a 4173 2061 2063 6f6e 7365 7175  ....As a consequ
+00001280: 656e 6365 206f 6620 7468 6520 6869 6572  ence of the hier
+00001290: 6172 6368 6963 616c 2073 7472 7563 7475  archical structu
+000012a0: 7265 206f 6620 7468 6520 6d6f 6465 6c73  re of the models
+000012b0: 2069 6e20 4178 6973 564d 2c20 6576 6572   in AxisVM, ever
+000012c0: 7920 6d6f 6465 6c20 6372 6561 7469 6f6e  y model creation
+000012d0: 2070 726f 6363 6573 7320 7374 6172 7473   proccess starts
+000012e0: 2077 6974 6820 6e6f 6465 732e 2054 6f20   with nodes. To 
+000012f0: 6372 6561 7465 206e 6f64 6573 2077 6520  create nodes we 
+00001300: 6e65 6564 2061 6e20 696e 7465 7266 6163  need an interfac
+00001310: 6520 746f 2074 6865 206e 6f64 6573 206f  e to the nodes o
+00001320: 6620 7468 6520 6170 706c 6963 6174 696f  f the applicatio
+00001330: 6e2e 2054 6869 7320 6973 2061 6368 6965  n. This is achie
+00001340: 7665 6420 6279 2074 6865 2060 4941 7869  ved by the `IAxi
+00001350: 7356 4d4e 6f64 6573 6020 636c 6173 7320  sVMNodes` class 
+00001360: 6f66 2074 6865 2074 7970 6520 6c69 6272  of the type libr
+00001370: 6172 792e 2049 6620 796f 7520 6c6f 6f6b  ary. If you look
+00001380: 2069 7420 7570 2069 6e20 7468 6520 7064   it up in the pd
+00001390: 6620 646f 6375 6d65 6e74 2c20 796f 7520  f document, you 
+000013a0: 7769 6c6c 2073 6565 2074 6869 733a 0d0a  will see this:..
+000013b0: 0d0a 215b 4941 7869 7356 4d4e 6f64 6573  ..![IAxisVMNodes
+000013c0: 5d28 5f73 7461 7469 632f 4941 7869 7356  ](_static/IAxisV
+000013d0: 4d4e 6f64 6573 2e70 6e67 290d 0a0d 0a4a  MNodes.png)....J
+000013e0: 7573 7420 6c69 6b65 206f 7468 6572 2069  ust like other i
+000013f0: 6e74 6572 6661 6365 732c 2074 6865 2064  nterfaces, the d
+00001400: 6f63 756d 656e 7461 7469 6f6e 206f 6620  ocumentation of 
+00001410: 6049 4178 6973 564d 4e6f 6465 7360 2062  `IAxisVMNodes` b
+00001420: 6567 696e 7320 7769 7468 206c 6973 7469  egins with listi
+00001430: 6e67 2074 6865 2065 6e75 6d65 7261 7469  ng the enumerati
+00001440: 6f6e 7320 616e 6420 7265 636f 7264 7320  ons and records 
+00001450: 7370 6563 6966 6963 2074 6f20 6e6f 6465  specific to node
+00001460: 732e 2042 656c 6f77 2074 6865 7365 2c20  s. Below these, 
+00001470: 796f 7520 6361 6e20 7365 6520 7468 6520  you can see the 
+00001480: 6675 6e63 7469 6f6e 7320 6f66 2074 6865  functions of the
+00001490: 2069 6e74 6572 6661 6365 2e0d 0a0d 0a21   interface.....!
+000014a0: 5b46 756e 6374 696f 6e73 5d28 5f73 7461  [Functions](_sta
+000014b0: 7469 632f 4941 7869 7356 4d4e 6f64 6573  tic/IAxisVMNodes
+000014c0: 5f46 756e 6374 696f 6e73 2e70 6e67 290d  _Functions.png).
+000014d0: 0a0d 0a41 6674 6572 2061 6c6c 2074 6865  ...After all the
+000014e0: 2066 756e 6374 696f 6e73 2c20 7468 6520   functions, the 
+000014f0: 646f 6375 6d65 6e74 6174 696f 6e20 6f66  documentation of
+00001500: 2074 6865 2069 6e74 6572 6661 6365 2069   the interface i
+00001510: 7320 6669 6e69 7368 6564 2062 7920 6c69  s finished by li
+00001520: 7374 696e 6720 7468 6520 7072 6f70 6572  sting the proper
+00001530: 7469 6573 206f 6620 7468 6520 696e 7465  ties of the inte
+00001540: 7266 6163 652e 0d0a 0d0a 215b 5072 6f70  rface.....![Prop
+00001550: 6572 7469 6573 5d28 5f73 7461 7469 632f  erties](_static/
+00001560: 4941 7869 7356 4d4e 6f64 6573 5f50 726f  IAxisVMNodes_Pro
+00001570: 7065 7274 6965 732e 706e 6729 0d0a 0d0a  perties.png)....
+00001580: 6060 6070 7974 686f 6e0d 0a66 726f 6d20  ```python..from 
+00001590: 6178 6973 766d 2e63 6f6d 2e63 6c69 656e  axisvm.com.clien
+000015a0: 7420 696d 706f 7274 2073 7461 7274 5f41  t import start_A
+000015b0: 7869 7356 4d0d 0a61 7876 6d20 3d20 7374  xisVM..axvm = st
+000015c0: 6172 745f 4178 6973 564d 2876 6973 6962  art_AxisVM(visib
+000015d0: 6c65 3d54 7275 652c 2064 6165 6d6f 6e3d  le=True, daemon=
+000015e0: 5472 7565 290d 0a0d 0a6d 6f64 656c 4964  True)....modelId
+000015f0: 203d 2061 7876 6d2e 4d6f 6465 6c73 2e4e   = axvm.Models.N
+00001600: 6577 2829 0d0a 6d6f 6465 6c20 3d20 6178  ew()..model = ax
+00001610: 766d 2e4d 6f64 656c 735b 6d6f 6465 6c49  vm.Models[modelI
+00001620: 645d 0d0a 6060 600d 0a0d 0a52 6967 6874  d]..```....Right
+00001630: 2062 656c 6f77 2074 6865 2060 4164 6460   below the `Add`
+00001640: 2066 756e 6374 696f 6e2c 2074 6865 7265   function, there
+00001650: 2069 7320 7468 6520 6041 6464 5769 7468   is the `AddWith
+00001660: 444f 4660 2c20 7769 7468 2074 6865 2066  DOF`, with the f
+00001670: 6f6c 6c6f 7769 6e67 2064 6f63 756d 656e  ollowing documen
+00001680: 7461 7469 6f6e 3a0d 0a0d 0a21 5b50 726f  tation:....![Pro
+00001690: 7065 7274 6965 735d 285f 7374 6174 6963  perties](_static
+000016a0: 2f49 4178 6973 564d 4e6f 6465 735f 4164  /IAxisVMNodes_Ad
+000016b0: 6457 6974 6844 6f66 2e70 6e67 290d 0a0d  dWithDof.png)...
+000016c0: 0a49 7420 7465 6c6c 732c 2074 6861 7420  .It tells, that 
+000016d0: 7468 6520 6675 6e63 7469 6f6e 206e 6565  the function nee
+000016e0: 6473 2074 6f20 6265 2063 616c 6c65 6420  ds to be called 
+000016f0: 7769 7468 2073 7065 6369 6679 696e 6720  with specifying 
+00001700: 7468 7265 6520 7363 616c 6172 2076 616c  three scalar val
+00001710: 7565 7320 616e 6420 6120 666f 7572 7468  ues and a fourth
+00001720: 206f 6e65 2073 7065 6369 6679 696e 6720   one specifying 
+00001730: 6120 444f 4620 636f 6d70 6f6e 656e 742e  a DOF component.
+00001740: 2054 6865 2065 6e75 6d65 7261 7469 6f6e   The enumeration
+00001750: 2060 4544 6567 7265 654f 6646 7265 6564   `EDegreeOfFreed
+00001760: 6f6d 6020 7761 7320 6c69 7374 6564 2061  om` was listed a
+00001770: 7420 7468 6520 6265 6769 6e6e 696e 6720  t the beginning 
+00001780: 6f66 2074 6865 2064 6f63 756d 656e 7461  of the documenta
+00001790: 7469 6f6e 206f 6620 7468 6520 696e 7465  tion of the inte
+000017a0: 7266 6163 652e 0d0a 0d0a 6060 6070 7974  rface.....```pyt
+000017b0: 686f 6e0d 0a66 726f 6d20 6178 6973 766d  hon..from axisvm
+000017c0: 2e63 6f6d 2e74 6c62 2069 6d70 6f72 7420  .com.tlb import 
+000017d0: 646f 6646 7265 650d 0a69 6431 203d 206d  dofFree..id1 = m
+000017e0: 6f64 656c 2e4e 6f64 6573 2e41 6464 5769  odel.Nodes.AddWi
+000017f0: 7468 444f 4628 2d31 2c20 2d31 2c20 302c  thDOF(-1, -1, 0,
+00001800: 2064 6f66 4672 6565 290d 0a69 6432 203d   dofFree)..id2 =
+00001810: 206d 6f64 656c 2e4e 6f64 6573 2e41 6464   model.Nodes.Add
+00001820: 5769 7468 444f 4628 312c 202d 312c 2030  WithDOF(1, -1, 0
+00001830: 2c20 646f 6646 7265 6529 0d0a 6964 3320  , dofFree)..id3 
+00001840: 3d20 6d6f 6465 6c2e 4e6f 6465 732e 4164  = model.Nodes.Ad
+00001850: 6457 6974 6844 4f46 2831 2c20 312c 2030  dWithDOF(1, 1, 0
+00001860: 2c20 646f 6646 7265 6529 0d0a 6964 3420  , dofFree)..id4 
+00001870: 3d20 6d6f 6465 6c2e 4e6f 6465 732e 4164  = model.Nodes.Ad
+00001880: 6457 6974 6844 4f46 282d 312c 2031 2c20  dWithDOF(-1, 1, 
+00001890: 302c 2064 6f66 4672 6565 290d 0a60 6060  0, dofFree)..```
+000018a0: 0d0a 0d0a 4166 7465 7220 7468 6520 7365  ....After the se
+000018b0: 7373 696f 6e20 6861 7320 656e 6465 642c  ssion has ended,
+000018c0: 2063 6c6f 7365 2074 6865 2061 7070 6c69   close the appli
+000018d0: 6361 7469 6f6e 2062 790d 0a0d 0a60 6060  cation by....```
+000018e0: 7079 7468 6f6e 0d0a 6178 766d 2e51 7569  python..axvm.Qui
+000018f0: 7428 290d 0a60 6060 0d0a 0d0a 2323 2320  t()..```....### 
+00001900: 4d6f 7265 2061 6476 616e 6365 6420 6578  More advanced ex
+00001910: 616d 706c 6573 0d0a 0d0a 4966 2079 6f75  amples....If you
+00001920: 2077 616e 7420 6d6f 7265 2c20 6368 6563   want more, chec
+00001930: 6b20 6f75 7420 7468 6520 5b75 7365 7220  k out the [user 
+00001940: 6775 6964 655d 2875 7365 725f 6775 6964  guide](user_guid
+00001950: 652e 7273 7429 2c20 7768 6572 6520 796f  e.rst), where yo
+00001960: 7520 7769 6c6c 2066 696e 6420 6120 6772  u will find a gr
+00001970: 6f77 696e 6720 7365 7420 6f66 2065 7861  owing set of exa
+00001980: 6d70 6c65 7320 746f 2073 756f 7070 6f72  mples to suoppor
+00001990: 7420 796f 7520 696e 2079 6f75 7220 6c65  t you in your le
+000019a0: 6172 6e69 6e67 2070 726f 6365 7373 2e20  arning process. 
+000019b0: 5765 2073 7567 6765 7374 2079 6f75 2074  We suggest you t
+000019c0: 6f20 636f 6e74 696e 7565 2077 6861 7420  o continue what 
+000019d0: 796f 7527 7665 2064 6f6e 6520 696e 2074  you've done in t
+000019e0: 6865 2070 7265 7669 6f75 7320 7365 6374  he previous sect
+000019f0: 696f 6e20 6f66 2074 6869 7320 7061 6765  ion of this page
+00001a00: 2e20 4861 7665 2074 6865 2041 7869 7356  . Have the AxisV
+00001a10: 4d20 4150 4920 5245 4645 5245 4e43 4520  M API REFERENCE 
+00001a20: 7064 6620 646f 6375 6d65 6e74 206f 7065  pdf document ope
+00001a30: 6e65 642c 2061 6e64 2073 6565 2066 6f72  ned, and see for
+00001a40: 2079 6f75 7273 656c 6620 686f 7720 656e   yourself how en
+00001a50: 6470 6f69 6e74 7320 616e 6420 7265 7475  dpoints and retu
+00001a60: 726e 6564 2064 6174 6120 7765 7265 2075  rned data were u
+00001a70: 7365 642e 0d0a                           sed...
```

### Comparing `axisvm-1.2.1/docs/Makefile` & `axisvm-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/make.bat` & `axisvm-1.2.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/AxisVM_logo.bmp` & `axisvm-1.2.2/docs/source/_static/AxisVM_logo.bmp`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/IAxisVMNodes.png` & `axisvm-1.2.2/docs/source/_static/IAxisVMNodes.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/IAxisVMNodes_AddWithDof.png` & `axisvm-1.2.2/docs/source/_static/IAxisVMNodes_AddWithDof.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/IAxisVMNodes_Functions.png` & `axisvm-1.2.2/docs/source/_static/IAxisVMNodes_Functions.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/IAxisVMNodes_Properties.png` & `axisvm-1.2.2/docs/source/_static/IAxisVMNodes_Properties.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/_static/AxisVM_logo_dark.png` & `axisvm-1.2.2/docs/source/_static/AxisVM_logo_dark.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/_static/AxisVM_logo_light.png` & `axisvm-1.2.2/docs/source/_static/AxisVM_logo_light.png`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/api_axisvm.rst` & `axisvm-1.2.2/docs/source/api/api_axisvm.rst`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/gt40.PNG` & `axisvm-1.2.2/docs/source/_static/gt40.PNG`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/docs/source/tips_and_tricks.md` & `axisvm-1.2.2/docs/source/tips_and_tricks.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+(tips-and-tricks)=
 # Tips and Tricks
 
 This page sums up the changes in syntax, compared to the 'raw' usage of the COM type library. Everything the API provides out of the box is still available and is working as ever, but the syntax of Python provides a few shortcuts to make coding easier.
 
 ## Collections and Slicing
 
 When accessing items of collection-like COM classes (like `IAxisVMDomains`, `IAxisVMSurfaces`, anything having an `Item` method), you can use the slicing mechanism of Python. Suppose that we have an `IAxisVMModel`  instance called `axm`. The model has several domains, each of them having the property `Weight`. Let say we want to calculate the weight of all domains. The out of box solution for this would be something like
   
 ```python
 weights=[]
 for i in range(axm.Surfaces.Count):
     weights.append(axm.Surfaces.Item[i+1].Weight)
 weight = sum(weights)
 ```
+
 or using a list comprehension
 
 ```python
 weight = sum([axm.Surfaces.Item[i+1].Weight for i in range(axm.Surfaces.Count)])
 ```
 
 or maybe even this
@@ -40,15 +42,15 @@
 
 or maybe
 
 ```python
 weight = sum(map(lambda s : s.Weight, axm.Surfaces))
 ```
 
-Notice how the loops here are carried out over the collection object itself. This is because collection types implement the so-called iterator protocol. 
+Notice how the loops here are carried out over the collection object itself. This is because collection types implement the so-called iterator protocol.
 
 It is also possible to provide negative indices:
 
 ```python
 axm.Surfaces[-1].Weight # equivalent to axm.Surfaces[axm.Surfaces.Count].Weight
 axm.Surfaces[-2].Weight # equivalent to axm.Surfaces[axm.Surfaces.Count - 1].Weight
 ```
@@ -89,15 +91,15 @@
 When creating a new interface, you can do it like
 
 ```python
 from axisvm.com.client import start_AxisVM
 axvm = start_AxisVM(visible=True, daemon=True)
 ```
 
-The keyword argument `daemon=True` is a simple shortcut, equivalent to 
+The keyword argument `daemon=True` is a simple shortcut, equivalent to
 
 ```python
 from axisvm.com.client import start_AxisVM
 import axisvm.com.tlb as axtlb
 axapp = start_AxisVM(visible=True, daemon=False)
 axapp.CloseOnLastReleased = True
 axapp.AskCloseOnLastReleased = False
@@ -105,8 +107,8 @@
 axapp.ApplicationClose = axtlb.acEnableNoWarning
 ```
 
 As a result of these settings, if the COM server is shut down, AxisVM shuts down either, hence the term `daemon`. Shutting down the COM server can be done with typing
 
 ```python
 axapp.Quit()
-```
+```
```

### Comparing `axisvm-1.2.1/notebooks/connected_members.ipynb` & `axisvm-1.2.2/notebooks/connected_members.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/console.ipynb` & `axisvm-1.2.2/docs/source/notebooks/console.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/gen_tlb.ipynb` & `axisvm-1.2.2/notebooks/gen_tlb.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/membrane_example.ipynb` & `axisvm-1.2.2/docs/source/notebooks/membrane_example.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/plate_example_1.ipynb` & `axisvm-1.2.2/docs/source/notebooks/plate_example_1.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/plate_example_2.ipynb` & `axisvm-1.2.2/docs/source/notebooks/plate_example_2.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/pyvista.ipynb` & `axisvm-1.2.2/notebooks/pyvista.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/notebooks/tetrahedra.ipynb` & `axisvm-1.2.2/notebooks/tetrahedra.ipynb`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/pyproject.toml` & `axisvm-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel>=0.38.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axisvm"
-version = "1.2.1"
+version = "1.2.2"
 description = "A Python package for AxisVM."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
@@ -29,15 +29,15 @@
     { name = "InterCAD Ltd.", email = "gbokor@axisvm.eu" }
 ]
 license = { file = "LICENSE" }
 keywords = [
     "engineering", "mechanics", "finite element method", "AxisVM", "civil engineering",
     "steel design", "concrete design", "timber design"
 ]
-requires-python = ">=3.7, <3.11"
+requires-python = ">=3.10, <3.12"
 dynamic = ["dependencies", "optional-dependencies"]
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
```

### Comparing `axisvm-1.2.1/src/axisvm/__init__.py` & `axisvm-1.2.2/src/axisvm/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.9"
-
 import os
 import appdirs
 import warnings
 from typing import Optional
+from importlib.metadata import metadata
+
+__pkg_metadata__ = metadata("axisvm")
+__version__ = __pkg_metadata__["version"]
+__description__ = __pkg_metadata__["summary"]
+del __pkg_metadata__
 
 # catch annoying numpy/vtk future warning:
 warnings.simplefilter(action="ignore", category=FutureWarning)
 
 # If available, a local vtk-data instance will be used for examples
 AXISVM_DATA_PATH: Optional[str] = None
 if "AXISVM_DATA_PATH" in os.environ:
```

### Comparing `axisvm-1.2.1/src/axisvm/com/attr.py` & `axisvm-1.2.2/src/axisvm/com/attr.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axapp.py` & `axisvm-1.2.2/src/axisvm/com/axapp.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axcalculation.py` & `axisvm-1.2.2/src/axisvm/com/axcalculation.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axdomain.py` & `axisvm-1.2.2/src/axisvm/com/axdomain.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
     def plot(self, *_, **mpl_kw) -> None:
         """
         Plots the surface using `matplotlib`.
 
         Parameters
         ----------
         **mpl_kw: dict, Optional
-            Parameters to pass to :func:`sigmaepsilon.plotting.mpl.triplot`
+            Parameters to pass to :func:`~sigmaepsilon.mesh.plotting.mpl.triplot_mpl_mesh`
         """
         coords, topo, _ = self.detach_mesh(return_indices=True, triangulate=True)
         triobj = tri.Triangulation(coords[:, 0], coords[:, 1], triangles=topo)
         if mpl_kw is None:
             mpl_kw = dict(axis="on")
         triplot_mpl_mesh(triobj, **mpl_kw)
 
@@ -279,15 +279,15 @@
             * 'fz' or 'rotz' : rotation around Z
 
             Default is 'ez'.
         displacement_system: Union[str, int], Optional
             Sets the displacement system in which results are to be returned. Possible values
             are 1 (or 'global) and 0 (or 'local'). Default is 1, which means the global system.
         **mpl_kw : dict, Optional
-            Parameters to pass to :func:`sigmaepsilon.plotting.mpl.triplot`
+            Parameters to pass to :func:`~sigmaepsilon.mesh.plotting.mpl.triplot_mpl_data`
         *args
             Forwarded to :function:`~axisvm.com.axmodel.IAxisVMModel.dof_solution`.
         **kwargs
             Forwarded to :function:`~axisvm.com.axmodel.IAxisVMModel.dof_solution`.
 
         Notes
         -----
@@ -383,15 +383,15 @@
             * 'vx' or 'vxz' : :math:`v_x` shear force
             * 'vy' or 'vyz' : :math:`v_y` shear force
 
             Default is 'nx'.
         smoothen: int, Optional
             If the values should be smoothened or not. Default is False.
         **mpl_kw: dict, Optional
-            Parameters to pass to :func:`sigmaepsilon.plotting.mpl.triplot`
+            Parameters to pass to :func:`~sigmaepsilon.mesh.plotting.mpl.triplot_mpl_data`
         """
         assert not smoothen, "Smoothing is not available at the moment."
         axm = self.model
         sids = np.array(self.MeshSurfaceIds) - 1
         forces = axm.generalized_surface_forces(*args, **kwargs)[sids]
         coords, topo = self.detach_mesh(triangulate=False)
         topo, forces = triang(topo, data=forces)  # triangulate with data
@@ -449,15 +449,15 @@
             Default is None.
         z: str, Optional
             Specifies the location along the thickness. Possible values are
             't' for top, 'b' for bottom, 'm' for middle and 'max' for the location
             where the value takes its maximum (only for shear stresses).
             Default is None.
         **mpl_kw: dict, Optional
-            Parameters to pass to :func:`sigmaepsilon.plotting.mpl.triplot`
+            Parameters to pass to :func:`~sigmaepsilon.mesh.plotting.mpl.triplot_mpl_data`
 
         Import the necessary stuff,
 
         Examples
         --------
         >>> from axisvm.com.client import start_AxisVM
         >>> from axisvm import examples
```

### Comparing `axisvm-1.2.1/src/axisvm/com/axline.py` & `axisvm-1.2.2/src/axisvm/com/axline.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axloadcombinations.py` & `axisvm-1.2.2/src/axisvm/com/axloadcombinations.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axmaterial.py` & `axisvm-1.2.2/src/axisvm/com/axmaterial.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axmember.py` & `axisvm-1.2.2/src/axisvm/com/axmember.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axmodel.py` & `axisvm-1.2.2/src/axisvm/com/axmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .axline import IAxisVMLines
 from .axwindow import IAxisVMWindows
 from .axresult import IAxisVMResults
 from .axmaterial import IAxisVMMaterials
 from .axcalculation import IAxisVMCalculation
 from .axloadcombinations import IAxisVMLoadCombinations
 from .axnodalsupports import IAxisVMNodalSupports
+from .axrcbeamdesign import IAxisVMRCBeamDesign
 
 __all__ = ["IAxisVMModels", "IAxisVMModel"]
 
 
 class IAxisVMModel(AxWrapper):
     """Wrapper for the `IAxisVMModel` COM interface."""
 
@@ -105,14 +106,19 @@
 
     @property
     def NodalSupports(self) -> IAxisVMNodalSupports:
         """Returns a pointer object to the `IAxisVMNodalSupports` COM interface."""
         return IAxisVMNodalSupports(model=self, wrap=self._wrapped.NodalSupports)
     
     @property
+    def RCBeamDesign(self) -> IAxisVMRCBeamDesign:
+        """Returns a pointer object to the `IAxisVMRCBeamDesign` COM interface."""
+        return IAxisVMRCBeamDesign(wrap=self._wrapped.RCBeamDesign)
+    
+    @property
     def MeshSurfaceIds(self) -> ndarray:
         """Returns the indices of the surfaces of all domains in the model
         as a NumPy array."""
         d = self.Domains
         dc = d.Count
 
         def fnc(i):
```

### Comparing `axisvm-1.2.1/src/axisvm/com/axnodalsupports.py` & `axisvm-1.2.2/src/axisvm/com/axnodalsupports.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axnode.py` & `axisvm-1.2.2/src/axisvm/com/axnode.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axresult.py` & `axisvm-1.2.2/src/axisvm/com/axresult.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axsurface.py` & `axisvm-1.2.2/src/axisvm/com/axsurface.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/axwindow.py` & `axisvm-1.2.2/src/axisvm/com/axwindow.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/client.py` & `axisvm-1.2.2/src/axisvm/com/client.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/core/abc.py` & `axisvm-1.2.2/src/axisvm/com/core/abc.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/core/utils.py` & `axisvm-1.2.2/src/axisvm/com/core/utils.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/core/wrap.py` & `axisvm-1.2.2/src/axisvm/com/core/wrap.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/com/tlb.py` & `axisvm-1.2.2/src/axisvm/com/tlb.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/docs/utils.py` & `axisvm-1.2.2/src/axisvm/docs/utils.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/src/axisvm/examples/downloads.py` & `axisvm-1.2.2/src/axisvm/examples/downloads.py`

 * *Files identical despite different names*

### Comparing `axisvm-1.2.1/tips_and_tricks.md` & `axisvm-1.2.2/tips_and_tricks.md`

 * *Files identical despite different names*

