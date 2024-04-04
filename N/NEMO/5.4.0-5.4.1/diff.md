# Comparing `tmp/NEMO-5.4.0.tar.gz` & `tmp/NEMO-5.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NEMO-5.4.0.tar", last modified: Wed Apr  3 17:49:49 2024, max compression
+gzip compressed data, was "NEMO-5.4.1.tar", last modified: Thu Apr  4 15:56:30 2024, max compression
```

## Comparing `NEMO-5.4.0.tar` & `NEMO-5.4.1.tar`

### file list

```diff
@@ -1,588 +1,588 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.653196 NEMO-5.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1865 2024-03-06 04:03:19.000000 NEMO-5.4.0/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-06 04:03:19.000000 NEMO-5.4.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.554195 NEMO-5.4.0/NEMO/
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7689 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    64058 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/admin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.557195 NEMO-5.4.0/NEMO/apps/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.557195 NEMO-5.4.0/NEMO/apps/area_access/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.537195 NEMO-5.4.0/NEMO/apps/area_access/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.558195 NEMO-5.4.0/NEMO/apps/area_access/static/area_access/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/area_access/static/area_access/area_access.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.537195 NEMO-5.4.0/NEMO/apps/area_access/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.561195 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/alerts.html
--rw-rw-rw-   0 root         (0) root         (0)     1910 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/badge_not_found.html
--rw-rw-rw-   0 root         (0) root         (0)     9831 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/base.html
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/choose_area.html
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/door_is_open.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/farewell_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/inactive.html
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/login_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/logout_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/logout_warning.html
--rw-rw-rw-   0 root         (0) root         (0)      240 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/not_logged_in.html
--rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/welcome_screen.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/area_access/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    15349 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/apps/area_access/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.563195 NEMO-5.4.0/NEMO/apps/contracts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4294 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/customization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.563195 NEMO-5.4.0/NEMO/apps/contracts/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.564195 NEMO-5.4.0/NEMO/apps/contracts/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.564195 NEMO-5.4.0/NEMO/apps/contracts/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     7784 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/migrations/0002_increase_document_path_length.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5550 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.538195 NEMO-5.4.0/NEMO/apps/contracts/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.566195 NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/contractors.html
--rw-rw-rw-   0 root         (0) root         (0)     4746 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     3744 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/procurements.html
--rw-rw-rw-   0 root         (0) root         (0)     5178 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/service_contracts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.566195 NEMO-5.4.0/NEMO/apps/contracts/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     3577 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
--rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/contracts/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.566195 NEMO-5.4.0/NEMO/apps/contracts/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11009 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/contracts/views/contracts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.567196 NEMO-5.4.0/NEMO/apps/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.538195 NEMO-5.4.0/NEMO/apps/kiosk/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.568195 NEMO-5.4.0/NEMO/apps/kiosk/static/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/kiosk/static/kiosk/kiosk.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.539195 NEMO-5.4.0/NEMO/apps/kiosk/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.571195 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/
--rw-rw-rw-   0 root         (0) root         (0)     1336 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html
--rw-rw-rw-   0 root         (0) root         (0)     2362 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/choices.html
--rw-rw-rw-   0 root         (0) root         (0)     1223 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/error.html
--rw-rw-rw-   0 root         (0) root         (0)     3786 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)    15451 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/success.html
--rw-rw-rw-   0 root         (0) root         (0)    23584 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html
--rw-rw-rw-   0 root         (0) root         (0)     1628 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
--rw-rw-rw-   0 root         (0) root         (0)     4111 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     2071 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation_extra.html
--rw-rw-rw-   0 root         (0) root         (0)     2023 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/apps/kiosk/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    17507 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/apps/kiosk/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.573196 NEMO-5.4.0/NEMO/apps/sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10252 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/apps/sensors/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      968 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/customizations.py
--rw-rw-rw-   0 root         (0) root         (0)     2767 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/apps/sensors/evaluators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.574195 NEMO-5.4.0/NEMO/apps/sensors/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.574195 NEMO-5.4.0/NEMO/apps/sensors/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/management/commands/manage_sensor_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.575195 NEMO-5.4.0/NEMO/apps/sensors/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     9355 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14350 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/apps/sensors/models.py
--rw-rw-rw-   0 root         (0) root         (0)     8703 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/apps/sensors/sensors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.539195 NEMO-5.4.0/NEMO/apps/sensors/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.577196 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/
--rw-rw-rw-   0 root         (0) root         (0)   408236 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chart.js
--rw-rw-rw-   0 root         (0) root         (0)   195090 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chart.min.js
--rw-rw-rw-   0 root         (0) root         (0)     1376 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
--rw-rw-rw-   0 root         (0) root         (0)     7659 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/daterangepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    66305 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/daterangepicker.js
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/static/sensors/sensors.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.540195 NEMO-5.4.0/NEMO/apps/sensors/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.577196 NEMO-5.4.0/NEMO/apps/sensors/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     8089 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.578196 NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
--rw-rw-rw-   0 root         (0) root         (0)    16375 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/sensor_data.html
--rw-rw-rw-   0 root         (0) root         (0)     4202 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/sensors.html
--rw-rw-rw-   0 root         (0) root         (0)      829 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/urls.py
--rw-rw-rw-   0 root         (0) root         (0)     6227 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/apps/sensors/views.py
--rw-rw-rw-   0 root         (0) root         (0)     4434 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/context_processors.py
--rw-rw-rw-   0 root         (0) root         (0)     7067 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     4757 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/evaluators.py
--rw-rw-rw-   0 root         (0) root         (0)     4927 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4342 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    16617 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/forms.py
--rw-rw-rw-   0 root         (0) root         (0)    22250 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/interlocks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.578196 NEMO-5.4.0/NEMO/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.581196 NEMO-5.4.0/NEMO/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/area_auto_logout_users.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/cancel_unused_reservations.py
--rw-rw-rw-   0 root         (0) root         (0)      415 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/create_closure_alerts.py
--rw-rw-rw-   0 root         (0) root         (0)      409 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/manage_recurring_charges.py
--rw-rw-rw-   0 root         (0) root         (0)      464 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/manage_tool_qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_reservation_ending_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_reservation_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_usage_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_user_access_expiration_reminders.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/management/commands/send_email_weekend_access_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     6338 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.594196 NEMO-5.4.0/NEMO/migrations/
--rw-rw-rw-   0 root         (0) root         (0)    64745 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0001_version_1_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)    39249 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0002_version_1_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)     8947 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0012_version_2_0_0_squashed.py
--rw-rw-rw-   0 root         (0) root         (0)    11366 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0020_version_3_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0021_version_3_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0022_version_3_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1220 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0023_badgereader.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0024_contactinformation_user.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0025_version_3_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)     6944 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0026_version_3_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0027_version_3_8_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2665 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0028_version_3_9_0.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0030_version_3_9_2.py
--rw-rw-rw-   0 root         (0) root         (0)     3190 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0031_version_3_10_0.py
--rw-rw-rw-   0 root         (0) root         (0)     3972 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0032_version_3_11_0.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0033_version_3_12_0.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0034_version_3_13_0.py
--rw-rw-rw-   0 root         (0) root         (0)     8846 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0035_version_3_14_0.py
--rw-rw-rw-   0 root         (0) root         (0)     9890 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0036_version_3_15_0.py
--rw-rw-rw-   0 root         (0) root         (0)     4101 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0037_version_3_16_0.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0038_version_4_0_0.py
--rw-rw-rw-   0 root         (0) root         (0)     4010 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0039_version_4_1_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2896 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0040_version_4_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0041_version_4_2_1.py
--rw-rw-rw-   0 root         (0) root         (0)    20584 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0042_version_4_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      570 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0043_version_4_3_2.py
--rw-rw-rw-   0 root         (0) root         (0)     6333 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0044_version_4_4_0.py
--rw-rw-rw-   0 root         (0) root         (0)    16787 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0045_version_4_5_0.py
--rw-rw-rw-   0 root         (0) root         (0)     2606 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0045_version_4_5_5.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0046_version_4_6_0.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0047_version_4_6_1.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0048_version_4_6_3.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0049_version_4_7_0.py
--rw-rw-rw-   0 root         (0) root         (0)      765 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0050_consumable_add_self_checkout_and_notes.py
--rw-rw-rw-   0 root         (0) root         (0)     7273 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0051_request_reviewers_in_tool_and_area.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0052_area_add_auto_logout_time.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0053_consumable_withdraw_add_usage_event_link.py
--rw-rw-rw-   0 root         (0) root         (0)     1712 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0054_documents_update_max_length.py
--rw-rw-rw-   0 root         (0) root         (0)     7122 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0055_reservationconfigurationoption.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0056_version_5_2_0.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0057_version_5_3_0.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0058_reservation_confirmation_override_prefs.py
--rw-rw-rw-   0 root         (0) root         (0)      801 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0059_tool_pre_usage_questions.py
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0060_add_impersonate_permission.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0061_alter_interlock_unique_together.py
--rw-rw-rw-   0 root         (0) root         (0)     1047 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0062_migrate_email_upcoming_reservation.py
--rw-rw-rw-   0 root         (0) root         (0)     6993 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations/0063_knowledge_base.py
--rw-rw-rw-   0 root         (0) root         (0)      641 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/migrations/0064_consumable_self_checkout_only_users.py
--rw-rw-rw-   0 root         (0) root         (0)      769 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/migrations/0065_door_adjacent_area.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/migrations/0066_tool_ask_to_leave_area_when_done_using.py
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/migrations/0067_project_allow_staff_charges.py
--rw-rw-rw-   0 root         (0) root         (0)     2040 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/migrations/0068_door_multiple_areas.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/migrations_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    13219 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     4632 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/model_tree.py
--rw-rw-rw-   0 root         (0) root         (0)   183416 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1654 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)    50755 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/policy.py
--rw-rw-rw-   0 root         (0) root         (0)    10709 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/provisioning.py
--rw-rw-rw-   0 root         (0) root         (0)     6697 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/rates.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/rest_filter_backend.py
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/rest_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)    17749 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.600196 NEMO-5.4.0/NEMO/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.600196 NEMO-5.4.0/NEMO/static/admin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.601196 NEMO-5.4.0/NEMO/static/admin/dynamic_form_preview/
--rw-rw-rw-   0 root         (0) root         (0)     4209 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.css
--rw-rw-rw-   0 root         (0) root         (0)     2586 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.601196 NEMO-5.4.0/NEMO/static/admin/physical_access_level/
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/admin/physical_access_level/access_level.js
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/admin/time_options_override.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.601196 NEMO-5.4.0/NEMO/static/admin/tool/
--rw-rw-rw-   0 root         (0) root         (0)     1300 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/admin/tool/tool.js
--rw-rw-rw-   0 root         (0) root         (0)     1615 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/static/badge_reader.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.541195 NEMO-5.4.0/NEMO/static/bootstrap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.603196 NEMO-5.4.0/NEMO/static/bootstrap/css/
--rw-rw-rw-   0 root         (0) root         (0)    22608 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.css
--rw-rw-rw-   0 root         (0) root         (0)    43339 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map
--rw-rw-rw-   0 root         (0) root         (0)    19963 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css
--rw-rw-rw-   0 root         (0) root         (0)   141622 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.css
--rw-rw-rw-   0 root         (0) root         (0)   380986 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.css.map
--rw-rw-rw-   0 root         (0) root         (0)   117305 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.604196 NEMO-5.4.0/NEMO/static/bootstrap/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    20127 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
--rw-rw-rw-   0 root         (0) root         (0)   108738 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
--rw-rw-rw-   0 root         (0) root         (0)    45404 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)    23424 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
--rw-rw-rw-   0 root         (0) root         (0)    18028 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.604196 NEMO-5.4.0/NEMO/static/bootstrap/js/
--rw-rw-rw-   0 root         (0) root         (0)    67546 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/js/bootstrap.js
--rw-rw-rw-   0 root         (0) root         (0)    35951 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/bootstrap/js/bootstrap.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.604196 NEMO-5.4.0/NEMO/static/datetimepicker/
--rw-rw-rw-   0 root         (0) root         (0)     9020 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
--rw-rw-rw-   0 root         (0) root         (0)   105978 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.606196 NEMO-5.4.0/NEMO/static/fullcalendar/
--rw-rw-rw-   0 root         (0) root         (0)    28531 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   358115 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)    13687 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.min.css
--rw-rw-rw-   0 root         (0) root         (0)   166724 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.607196 NEMO-5.4.0/NEMO/static/icons/
--rw-rw-rw-   0 root         (0) root         (0)    24065 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/icons/agreement.png
--rw-rw-rw-   0 root         (0) root         (0)    16685 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/icons/caution.png
--rw-rw-rw-   0 root         (0) root         (0)     4664 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/icons/preferences.png
--rw-rw-rw-   0 root         (0) root         (0)   247387 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    84320 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/jquery.min.js
--rw-rw-rw-   0 root         (0) root         (0)  1183392 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/jumbotron_watermark.bmp
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/mobile.js
--rw-rw-rw-   0 root         (0) root         (0)   174603 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/moment.js
--rw-rw-rw-   0 root         (0) root         (0)    58102 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/moment.min.js
--rw-rw-rw-   0 root         (0) root         (0)    86041 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/moment.min.js.map
--rw-rw-rw-   0 root         (0) root         (0)    19266 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/nemo.css
--rw-rw-rw-   0 root         (0) root         (0)    24034 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/static/nemo.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.607196 NEMO-5.4.0/NEMO/static/numpad/
--rw-rw-rw-   0 root         (0) root         (0)    12285 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/numpad/custom_numpad.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/numpad/numpad.jquery.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.608196 NEMO-5.4.0/NEMO/static/pickadate/
--rw-rw-rw-   0 root         (0) root         (0)     3795 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/default.css
--rw-rw-rw-   0 root         (0) root         (0)     6040 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/default.date.css
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/default.time.css
--rw-rw-rw-   0 root         (0) root         (0)    48215 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/picker.date.js
--rw-rw-rw-   0 root         (0) root         (0)    36941 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/picker.js
--rw-rw-rw-   0 root         (0) root         (0)    31899 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/pickadate/picker.time.js
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/robots.txt
--rw-rw-rw-   0 root         (0) root         (0)    48446 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/typeahead.jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    20748 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/typeahead.jquery.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.610196 NEMO-5.4.0/NEMO/static/virtualkeyboard/
--rw-rw-rw-   0 root         (0) root         (0)   113008 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/virtualkeyboard/jquery.keyboard.js
--rw-rw-rw-   0 root         (0) root         (0)    47325 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
--rw-rw-rw-   0 root         (0) root         (0)     7848 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/virtualkeyboard/keyboard-basic.css
--rw-rw-rw-   0 root         (0) root         (0)     5889 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.612196 NEMO-5.4.0/NEMO/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.613196 NEMO-5.4.0/NEMO/templates/abuse/
--rw-rw-rw-   0 root         (0) root         (0)     5236 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/abuse/abuse.html
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/abuse/user_drill_down.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.614196 NEMO-5.4.0/NEMO/templates/accounts_and_projects/
--rw-rw-rw-   0 root         (0) root         (0)     9016 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/account_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     3388 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/create_account.html
--rw-rw-rw-   0 root         (0) root         (0)     7972 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/create_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/documents_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/projects.html
--rw-rw-rw-   0 root         (0) root         (0)    10628 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/transfer_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/accounts_and_projects/users_for_project.html
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/acknowledgement.html
--rw-rw-rw-   0 root         (0) root         (0)     6537 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/alerts.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.615196 NEMO-5.4.0/NEMO/templates/area_access/
--rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/area_access.html
--rw-rw-rw-   0 root         (0) root         (0)     2172 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/calendar_self_login.html
--rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/change_project.html
--rw-rw-rw-   0 root         (0) root         (0)     1608 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/login_areas.html
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/new_area_access_record.html
--rw-rw-rw-   0 root         (0) root         (0)     2536 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/new_area_access_record_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/area_access/self_login.html
--rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/authorization_failed.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.616196 NEMO-5.4.0/NEMO/templates/base/
--rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base/footer.html
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base/impersonate_header.html
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base/navbar.html
--rw-rw-rw-   0 root         (0) root         (0)    12140 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base/navbar_base.html
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base/popup.html
--rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.618196 NEMO-5.4.0/NEMO/templates/calendar/
--rw-rw-rw-   0 root         (0) root         (0)    37109 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/calendar.html
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/configuration.html
--rw-rw-rw-   0 root         (0) root         (0)     1060 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/configuration_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     3720 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/configuration_helper.html
--rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/policy_dialog.html
--rw-rw-rw-   0 root         (0) root         (0)     1525 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/project_choice.html
--rw-rw-rw-   0 root         (0) root         (0)     1611 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/proxy_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     2756 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/reservation_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     1782 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/reservation_questions.html
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/reservation_warning.html
--rw-rw-rw-   0 root         (0) root         (0)     5313 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/scheduled_outage_information.html
--rw-rw-rw-   0 root         (0) root         (0)     2029 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/specific_user_feed.html
--rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/calendar/usage_event_feed.html
--rw-rw-rw-   0 root         (0) root         (0)    10209 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/configuration_agenda.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.618196 NEMO-5.4.0/NEMO/templates/consumables/
--rw-rw-rw-   0 root         (0) root         (0)    11089 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/consumables/consumables.html
--rw-rw-rw-   0 root         (0) root         (0)     1617 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/consumables/consumables_order.html
--rw-rw-rw-   0 root         (0) root         (0)    13475 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/consumables/recurring_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/consumables/recurring_charges.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.619196 NEMO-5.4.0/NEMO/templates/contact/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/contact/contact_staff.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.621196 NEMO-5.4.0/NEMO/templates/customizations/
--rw-rw-rw-   0 root         (0) root         (0)     1853 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations.html
--rw-rw-rw-   0 root         (0) root         (0)    11038 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_application.html
--rw-rw-rw-   0 root         (0) root         (0)    14374 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_calendar.html
--rw-rw-rw-   0 root         (0) root         (0)    11917 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4641 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_emails.html
--rw-rw-rw-   0 root         (0) root         (0)     2806 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_interlock.html
--rw-rw-rw-   0 root         (0) root         (0)     2647 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_knowledge_base.html
--rw-rw-rw-   0 root         (0) root         (0)     7799 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_projects_and_accounts.html
--rw-rw-rw-   0 root         (0) root         (0)     2535 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_rates.html
--rw-rw-rw-   0 root         (0) root         (0)     4133 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_recurring_charges.html
--rw-rw-rw-   0 root         (0) root         (0)     2907 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)    20124 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     5071 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_safety.html
--rw-rw-rw-   0 root         (0) root         (0)    30060 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_templates.html
--rw-rw-rw-   0 root         (0) root         (0)    19946 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_tool.html
--rw-rw-rw-   0 root         (0) root         (0)     2047 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_training.html
--rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_upload.html
--rw-rw-rw-   0 root         (0) root         (0)     6186 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/customizations/customizations_user.html
--rw-rw-rw-   0 root         (0) root         (0)      508 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/display_success_and_redirect.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.622196 NEMO-5.4.0/NEMO/templates/email/
--rw-rw-rw-   0 root         (0) root         (0)    11342 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/email/compose_email.html
--rw-rw-rw-   0 root         (0) root         (0)     4906 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/email/email_broadcast.html
--rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/email/email_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.623196 NEMO-5.4.0/NEMO/templates/event_details/
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/event_details/area_access_details.html
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/event_details/outage_details.html
--rw-rw-rw-   0 root         (0) root         (0)    13988 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/event_details/reservation_details.html
--rw-rw-rw-   0 root         (0) root         (0)      623 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/event_details/usage_details.html
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/facility_rules.html
--rw-rw-rw-   0 root         (0) root         (0)     1452 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/feedback.html
--rw-rw-rw-   0 root         (0) root         (0)     1190 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/history.html
--rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/impersonate.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.623196 NEMO-5.4.0/NEMO/templates/jumbotron/
--rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/jumbotron/jumbotron.html
--rw-rw-rw-   0 root         (0) root         (0)     5819 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/jumbotron/jumbotron_content.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.623196 NEMO-5.4.0/NEMO/templates/knowledge_base/
--rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base.html
--rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base_base.html
--rw-rw-rw-   0 root         (0) root         (0)     3317 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base_items.html
--rw-rw-rw-   0 root         (0) root         (0)    11635 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/landing.html
--rw-rw-rw-   0 root         (0) root         (0)     4656 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.624196 NEMO-5.4.0/NEMO/templates/maintenance/
--rw-rw-rw-   0 root         (0) root         (0)     2182 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/maintenance/closed_task_details.html
--rw-rw-rw-   0 root         (0) root         (0)     7551 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/maintenance/maintenance.html
--rw-rw-rw-   0 root         (0) root         (0)    10855 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/maintenance/pending_task_details.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.625196 NEMO-5.4.0/NEMO/templates/mobile/
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/cancellation_result.html
--rw-rw-rw-   0 root         (0) root         (0)     2535 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/choose_item.html
--rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/error.html
--rw-rw-rw-   0 root         (0) root         (0)     1224 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/individual_outage.html
--rw-rw-rw-   0 root         (0) root         (0)     4128 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/individual_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)     4814 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/new_reservation.html
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/no_active_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/reservation_extra.html
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/reservation_success.html
--rw-rw-rw-   0 root         (0) root         (0)     1666 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/mobile/view_calendar.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.626196 NEMO-5.4.0/NEMO/templates/news/
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/news/archived_news.html
--rw-rw-rw-   0 root         (0) root         (0)     1319 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/news/new_news_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1363 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/news/news_update_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/news/recent_news.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/no_project.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.627196 NEMO-5.4.0/NEMO/templates/occupancy/
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/occupancy/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)     2700 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/occupancy/occupancy_content.html
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/occupancy/occupancy_count.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.627196 NEMO-5.4.0/NEMO/templates/pagination/
--rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/pagination/pagination_base.html
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/pagination/pagination_column.html
--rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/pagination/pagination_pages.html
--rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/pagination/pagination_selector.html
--rw-rw-rw-   0 root         (0) root         (0)     3267 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/qualifications.html
--rw-rw-rw-   0 root         (0) root         (0)     5832 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/refresh_sidebar_icons.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.628196 NEMO-5.4.0/NEMO/templates/remote_work/
--rw-rw-rw-   0 root         (0) root         (0)    13396 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/remote_work/remote_work.html
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/remote_work/remote_work_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.628196 NEMO-5.4.0/NEMO/templates/requests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.628196 NEMO-5.4.0/NEMO/templates/requests/access_requests/
--rw-rw-rw-   0 root         (0) root         (0)     9117 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/access_requests/access_request.html
--rw-rw-rw-   0 root         (0) root         (0)     3845 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/access_requests/access_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     3784 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/access_requests/access_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.629196 NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/
--rw-rw-rw-   0 root         (0) root         (0)     9867 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html
--rw-rw-rw-   0 root         (0) root         (0)     4033 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     7649 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.629196 NEMO-5.4.0/NEMO/templates/requests/buddy_requests/
--rw-rw-rw-   0 root         (0) root         (0)     4779 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/buddy_requests/buddy_request.html
--rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/buddy_requests/buddy_requests.html
--rw-rw-rw-   0 root         (0) root         (0)     4418 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/requests/user_requests.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.630196 NEMO-5.4.0/NEMO/templates/resources/
--rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/resources/modify_resource.html
--rw-rw-rw-   0 root         (0) root         (0)     5358 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/resources/resource_details.html
--rw-rw-rw-   0 root         (0) root         (0)     1642 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/resources/resources.html
--rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/resources/scheduled_outage.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.630196 NEMO-5.4.0/NEMO/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     2941 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/rest_framework/api.html
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/rest_framework/custom_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.631196 NEMO-5.4.0/NEMO/templates/safety/
--rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety.html
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_base.html
--rw-rw-rw-   0 root         (0) root         (0)     9496 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_data_sheets.html
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_issues.html
--rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_issues_create.html
--rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_issues_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     2282 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_issues_update.html
--rw-rw-rw-   0 root         (0) root         (0)     2307 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/safety/safety_items.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.632196 NEMO-5.4.0/NEMO/templates/snippets/
--rw-rw-rw-   0 root         (0) root         (0)      519 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/snippets/button.html
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/snippets/contact_person.html
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/snippets/document_list.html
--rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/snippets/embedded_document.html
--rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/snippets/tool_info.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.633196 NEMO-5.4.0/NEMO/templates/staff_charges/
--rw-rw-rw-   0 root         (0) root         (0)      948 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/change_status.html
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/choose_project.html
--rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/end_area_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1284 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/new_staff_charge.html
--rw-rw-rw-   0 root         (0) root         (0)     1049 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/reminder.html
--rw-rw-rw-   0 root         (0) root         (0)     2145 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/staff_charges/staff_charges_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.634196 NEMO-5.4.0/NEMO/templates/status_dashboard/
--rw-rw-rw-   0 root         (0) root         (0)     2333 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/status_dashboard/occupancy.html
--rw-rw-rw-   0 root         (0) root         (0)    11703 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/status_dashboard/staff.html
--rw-rw-rw-   0 root         (0) root         (0)     8559 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/status_dashboard/staff_absence.html
--rw-rw-rw-   0 root         (0) root         (0)     7477 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/status_dashboard/status_dashboard.html
--rw-rw-rw-   0 root         (0) root         (0)     4927 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/status_dashboard/tools.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.634196 NEMO-5.4.0/NEMO/templates/tasks/
--rw-rw-rw-   0 root         (0) root         (0)     3107 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tasks/resolve.html
--rw-rw-rw-   0 root         (0) root         (0)     6800 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tasks/update.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.636196 NEMO-5.4.0/NEMO/templates/tool_control/
--rw-rw-rw-   0 root         (0) root         (0)      820 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/config_history.html
--rw-rw-rw-   0 root         (0) root         (0)     1009 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)      771 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/interlock_error.html
--rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/logout_user.html
--rw-rw-rw-   0 root         (0) root         (0)     5162 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/past_tasks_and_comments.html
--rw-rw-rw-   0 root         (0) root         (0)     3079 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/qualified_users.html
--rw-rw-rw-   0 root         (0) root         (0)    16755 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/tool_control.html
--rw-rw-rw-   0 root         (0) root         (0)    55529 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/tool_status.html
--rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/usage_data.html
--rw-rw-rw-   0 root         (0) root         (0)      422 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/tool_control/use_tool_for_other.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.636196 NEMO-5.4.0/NEMO/templates/training/
--rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/training/get_projects.html
--rw-rw-rw-   0 root         (0) root         (0)     5757 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/training/training.html
--rw-rw-rw-   0 root         (0) root         (0)     5695 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/training/training_entry.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.637196 NEMO-5.4.0/NEMO/templates/usage/
--rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/usage/adjustment_request_button.html
--rw-rw-rw-   0 root         (0) root         (0)     5458 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/usage/billing.html
--rw-rw-rw-   0 root         (0) root         (0)    11290 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/usage/usage.html
--rw-rw-rw-   0 root         (0) root         (0)    10462 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/usage/usage_base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.637196 NEMO-5.4.0/NEMO/templates/users/
--rw-rw-rw-   0 root         (0) root         (0)    29353 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/users/create_or_modify_user.html
--rw-rw-rw-   0 root         (0) root         (0)    21255 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/users/preferences.html
--rw-rw-rw-   0 root         (0) root         (0)     5399 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/users/safe_deactivation.html
--rw-rw-rw-   0 root         (0) root         (0)     5563 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templates/users/users.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.638196 NEMO-5.4.0/NEMO/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9466 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/templatetags/custom_tags_and_filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.640196 NEMO-5.4.0/NEMO/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.640196 NEMO-5.4.0/NEMO/tests/test_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/test_api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/tests/test_api/test_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     5747 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_api/test_crud.py
--rw-rw-rw-   0 root         (0) root         (0)    29763 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/tests/test_area_access.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.642196 NEMO-5.4.0/NEMO/tests/test_calendar/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/test_calendar/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33680 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_area_reservation.py
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_calendar.py
--rw-rw-rw-   0 root         (0) root         (0)    22955 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_outage.py
--rw-rw-rw-   0 root         (0) root         (0)    11729 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_freed_time.py
--rw-rw-rw-   0 root         (0) root         (0)    18987 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_qualification_expiration.py
--rw-rw-rw-   0 root         (0) root         (0)    30268 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_reservation.py
--rw-rw-rw-   0 root         (0) root         (0)    10126 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_closures.py
--rw-rw-rw-   0 root         (0) root         (0)    24973 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/tests/test_consumables.py
--rw-rw-rw-   0 root         (0) root         (0)    15018 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     3680 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/tests/test_evaluators.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_formats.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.642196 NEMO-5.4.0/NEMO/tests/test_interlocks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/test_interlocks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3597 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_interlocks/test_modbus_interlock.py
--rw-rw-rw-   0 root         (0) root         (0)    11445 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_interlocks/test_stanford_interlock.py
--rw-rw-rw-   0 root         (0) root         (0)     7059 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_interlocks/test_web_relay_interlock.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.643196 NEMO-5.4.0/NEMO/tests/test_requests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/test_requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9460 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_requests/test_adjustment_requests.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.643196 NEMO-5.4.0/NEMO/tests/test_sensors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/tests/test_sensors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2229 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/tests/test_sensors/test_modbus_sensors.py
--rw-rw-rw-   0 root         (0) root         (0)     5067 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/tests/test_staff_charges.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2024-03-20 03:03:10.000000 NEMO-5.4.0/NEMO/tests/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)    18834 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_urls.py
--rw-rw-rw-   0 root         (0) root         (0)     3390 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/tests/test_utilities.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/typing.py
--rw-rw-rw-   0 root         (0) root         (0)    32325 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    27428 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/utilities.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.651196 NEMO-5.4.0/NEMO/views/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5483 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/abuse.py
--rw-rw-rw-   0 root         (0) root         (0)    12996 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/access_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    14108 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/accounts_and_projects.py
--rw-rw-rw-   0 root         (0) root         (0)    18838 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/adjustment_requests.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/alerts.py
--rw-rw-rw-   0 root         (0) root         (0)    22064 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/api.py
--rw-rw-rw-   0 root         (0) root         (0)    13969 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/api_billing.py
--rw-rw-rw-   0 root         (0) root         (0)     2700 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/api_file_import.py
--rw-rw-rw-   0 root         (0) root         (0)    21857 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/area_access.py
--rw-rw-rw-   0 root         (0) root         (0)    13996 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     7251 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/buddy_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    55977 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     2334 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/charge_validation.py
--rw-rw-rw-   0 root         (0) root         (0)     2705 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/configuration_agenda.py
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    12946 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/views/consumables.py
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/contact_staff.py
--rw-rw-rw-   0 root         (0) root         (0)    25225 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/customization.py
--rw-rw-rw-   0 root         (0) root         (0)     3763 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/documents.py
--rw-rw-rw-   0 root         (0) root         (0)    14607 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/email.py
--rw-rw-rw-   0 root         (0) root         (0)     2129 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/event_details.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/feedback.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-14 03:03:20.000000 NEMO-5.4.0/NEMO/views/get_projects.py
--rw-rw-rw-   0 root         (0) root         (0)     4745 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/history.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/jumbotron.py
--rw-rw-rw-   0 root         (0) root         (0)     3967 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/knowledge_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3631 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/landing.py
--rw-rw-rw-   0 root         (0) root         (0)     3007 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/maintenance.py
--rw-rw-rw-   0 root         (0) root         (0)     9060 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/mobile.py
--rw-rw-rw-   0 root         (0) root         (0)     3793 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/news.py
--rw-rw-rw-   0 root         (0) root         (0)     5628 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/notifications.py
--rw-rw-rw-   0 root         (0) root         (0)     1542 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     5650 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/qualifications.py
--rw-rw-rw-   0 root         (0) root         (0)    11231 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/remote_work.py
--rw-rw-rw-   0 root         (0) root         (0)     4095 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     9657 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/safety.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/sidebar.py
--rw-rw-rw-   0 root         (0) root         (0)    23435 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/status_dashboard.py
--rw-rw-rw-   0 root         (0) root         (0)    16613 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/tasks.py
--rw-rw-rw-   0 root         (0) root         (0)    39347 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/timed_services.py
--rw-rw-rw-   0 root         (0) root         (0)    30357 2024-03-21 16:29:21.000000 NEMO-5.4.0/NEMO/views/tool_control.py
--rw-rw-rw-   0 root         (0) root         (0)     7963 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/training.py
--rw-rw-rw-   0 root         (0) root         (0)     2164 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/tutorials.py
--rw-rw-rw-   0 root         (0) root         (0)    21395 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/views/usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1204 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/user_requests.py
--rw-rw-rw-   0 root         (0) root         (0)    25049 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/views/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.651196 NEMO-5.4.0/NEMO/widgets/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/widgets/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3925 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/widgets/configuration_editor.py
--rw-rw-rw-   0 root         (0) root         (0)    39555 2024-04-03 17:49:31.000000 NEMO-5.4.0/NEMO/widgets/dynamic_form.py
--rw-rw-rw-   0 root         (0) root         (0)     9709 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/widgets/item_tree.py
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-06 04:03:19.000000 NEMO-5.4.0/NEMO/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 17:49:49.652196 NEMO-5.4.0/NEMO.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    20518 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-04-03 17:49:49.000000 NEMO-5.4.0/NEMO.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1749 2024-04-03 17:49:49.653196 NEMO-5.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4477 2024-04-03 17:49:31.000000 NEMO-5.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-03 17:49:31.000000 NEMO-5.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      109 2024-04-03 17:49:49.654196 NEMO-5.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-03 17:49:31.000000 NEMO-5.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.887635 NEMO-5.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1865 2024-03-06 04:03:19.000000 NEMO-5.4.1/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-06 04:03:19.000000 NEMO-5.4.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.798633 NEMO-5.4.1/NEMO/
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7689 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    64058 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/admin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.799634 NEMO-5.4.1/NEMO/apps/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.800634 NEMO-5.4.1/NEMO/apps/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/area_access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.779633 NEMO-5.4.1/NEMO/apps/area_access/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.800634 NEMO-5.4.1/NEMO/apps/area_access/static/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/area_access/static/area_access/area_access.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.779633 NEMO-5.4.1/NEMO/apps/area_access/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.804633 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     1601 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/badge_not_found.html
+-rw-rw-rw-   0 root         (0) root         (0)     9831 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/choose_area.html
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/door_is_open.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/farewell_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/inactive.html
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/login_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/logout_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1755 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/logout_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)      240 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      339 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/not_logged_in.html
+-rw-rw-rw-   0 root         (0) root         (0)      211 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/physical_access_denied.html
+-rw-rw-rw-   0 root         (0) root         (0)      593 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/welcome_screen.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/area_access/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    15349 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/apps/area_access/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.805634 NEMO-5.4.1/NEMO/apps/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/contracts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4294 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/customization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.805634 NEMO-5.4.1/NEMO/apps/contracts/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/contracts/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.806634 NEMO-5.4.1/NEMO/apps/contracts/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/contracts/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/management/commands/send_email_contract_reminders.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.806634 NEMO-5.4.1/NEMO/apps/contracts/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     7784 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/migrations/0002_increase_document_path_length.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/contracts/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5550 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.779633 NEMO-5.4.1/NEMO/apps/contracts/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.807634 NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/contractors.html
+-rw-rw-rw-   0 root         (0) root         (0)     4746 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     3744 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/procurements.html
+-rw-rw-rw-   0 root         (0) root         (0)     5178 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/service_contracts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.807634 NEMO-5.4.1/NEMO/apps/contracts/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     3577 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/templates/customizations/customizations_contracts.html
+-rw-rw-rw-   0 root         (0) root         (0)      838 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/contracts/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.807634 NEMO-5.4.1/NEMO/apps/contracts/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/contracts/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11009 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/contracts/views/contracts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.808634 NEMO-5.4.1/NEMO/apps/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/kiosk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.780633 NEMO-5.4.1/NEMO/apps/kiosk/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.808634 NEMO-5.4.1/NEMO/apps/kiosk/static/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/kiosk/static/kiosk/kiosk.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.780633 NEMO-5.4.1/NEMO/apps/kiosk/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.810634 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/choices.html
+-rw-rw-rw-   0 root         (0) root         (0)     1223 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)    15451 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/success.html
+-rw-rw-rw-   0 root         (0) root         (0)    23584 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     1628 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html
+-rw-rw-rw-   0 root         (0) root         (0)     4111 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation_extra.html
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/apps/kiosk/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    17507 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/apps/kiosk/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.811634 NEMO-5.4.1/NEMO/apps/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10252 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/apps/sensors/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      968 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/customizations.py
+-rw-rw-rw-   0 root         (0) root         (0)     2767 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/apps/sensors/evaluators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.811634 NEMO-5.4.1/NEMO/apps/sensors/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/sensors/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.812634 NEMO-5.4.1/NEMO/apps/sensors/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/sensors/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/management/commands/manage_sensor_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.812634 NEMO-5.4.1/NEMO/apps/sensors/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     9355 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/apps/sensors/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14350 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/apps/sensors/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     8703 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/apps/sensors/sensors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.780633 NEMO-5.4.1/NEMO/apps/sensors/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.814634 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)   408236 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chart.js
+-rw-rw-rw-   0 root         (0) root         (0)   195090 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chart.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     1376 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js
+-rw-rw-rw-   0 root         (0) root         (0)     7659 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    66305 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/static/sensors/sensors.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.781633 NEMO-5.4.1/NEMO/apps/sensors/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.814634 NEMO-5.4.1/NEMO/apps/sensors/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     8089 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.814634 NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/
+-rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/sensor_alerts.html
+-rw-rw-rw-   0 root         (0) root         (0)    16375 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/sensor_data.html
+-rw-rw-rw-   0 root         (0) root         (0)     4202 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/sensors.html
+-rw-rw-rw-   0 root         (0) root         (0)      829 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     6227 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/apps/sensors/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4434 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/context_processors.py
+-rw-rw-rw-   0 root         (0) root         (0)     7067 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4757 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/evaluators.py
+-rw-rw-rw-   0 root         (0) root         (0)     4927 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4342 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    16617 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)    22250 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/interlocks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.815634 NEMO-5.4.1/NEMO/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.817634 NEMO-5.4.1/NEMO/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/area_auto_logout_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/cancel_unused_reservations.py
+-rw-rw-rw-   0 root         (0) root         (0)      415 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/create_closure_alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)      409 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/manage_recurring_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)      464 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/manage_tool_qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_out_of_time_reservation_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_reservation_ending_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_reservation_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_usage_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_user_access_expiration_reminders.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/management/commands/send_email_weekend_access_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     6338 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.825634 NEMO-5.4.1/NEMO/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)    64745 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0001_version_1_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    39249 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0002_version_1_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)     8947 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0012_version_2_0_0_squashed.py
+-rw-rw-rw-   0 root         (0) root         (0)    11366 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0020_version_3_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0021_version_3_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0022_version_3_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1220 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0023_badgereader.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0024_contactinformation_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0025_version_3_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     6944 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0026_version_3_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0027_version_3_8_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0028_version_3_9_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0030_version_3_9_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3190 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0031_version_3_10_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     3972 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0032_version_3_11_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0033_version_3_12_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0034_version_3_13_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0035_version_3_14_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     9890 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0036_version_3_15_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     4101 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0037_version_3_16_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0038_version_4_0_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     4010 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0039_version_4_1_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2896 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0040_version_4_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      516 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0041_version_4_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)    20584 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0042_version_4_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      570 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0043_version_4_3_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6333 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0044_version_4_4_0.py
+-rw-rw-rw-   0 root         (0) root         (0)    16787 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0045_version_4_5_0.py
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0045_version_4_5_5.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0046_version_4_6_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0047_version_4_6_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0048_version_4_6_3.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0049_version_4_7_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      765 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0050_consumable_add_self_checkout_and_notes.py
+-rw-rw-rw-   0 root         (0) root         (0)     7273 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0051_request_reviewers_in_tool_and_area.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0052_area_add_auto_logout_time.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0053_consumable_withdraw_add_usage_event_link.py
+-rw-rw-rw-   0 root         (0) root         (0)     1712 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0054_documents_update_max_length.py
+-rw-rw-rw-   0 root         (0) root         (0)     7122 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0055_reservationconfigurationoption.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0056_version_5_2_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0057_version_5_3_0.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0058_reservation_confirmation_override_prefs.py
+-rw-rw-rw-   0 root         (0) root         (0)      801 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0059_tool_pre_usage_questions.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0060_add_impersonate_permission.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0061_alter_interlock_unique_together.py
+-rw-rw-rw-   0 root         (0) root         (0)     1047 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0062_migrate_email_upcoming_reservation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6993 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations/0063_knowledge_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      641 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/migrations/0064_consumable_self_checkout_only_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/migrations/0065_door_adjacent_area.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/migrations/0066_tool_ask_to_leave_area_when_done_using.py
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/migrations/0067_project_allow_staff_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)     2040 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/migrations/0068_door_multiple_areas.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/migrations_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/mixins.py
+-rw-rw-rw-   0 root         (0) root         (0)     4632 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/model_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)   183416 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)    50755 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/policy.py
+-rw-rw-rw-   0 root         (0) root         (0)    10709 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/provisioning.py
+-rw-rw-rw-   0 root         (0) root         (0)     6697 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/rates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/rest_filter_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/rest_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)    17749 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.830634 NEMO-5.4.1/NEMO/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.830634 NEMO-5.4.1/NEMO/static/admin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.831634 NEMO-5.4.1/NEMO/static/admin/dynamic_form_preview/
+-rw-rw-rw-   0 root         (0) root         (0)     4209 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.css
+-rw-rw-rw-   0 root         (0) root         (0)     2586 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.831634 NEMO-5.4.1/NEMO/static/admin/physical_access_level/
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/admin/physical_access_level/access_level.js
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/admin/time_options_override.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.831634 NEMO-5.4.1/NEMO/static/admin/tool/
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/admin/tool/tool.js
+-rw-rw-rw-   0 root         (0) root         (0)     1615 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/static/badge_reader.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.782633 NEMO-5.4.1/NEMO/static/bootstrap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.833634 NEMO-5.4.1/NEMO/static/bootstrap/css/
+-rw-rw-rw-   0 root         (0) root         (0)    22608 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css
+-rw-rw-rw-   0 root         (0) root         (0)    43339 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map
+-rw-rw-rw-   0 root         (0) root         (0)    19963 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   141622 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.css
+-rw-rw-rw-   0 root         (0) root         (0)   380986 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.css.map
+-rw-rw-rw-   0 root         (0) root         (0)   117305 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.834634 NEMO-5.4.1/NEMO/static/bootstrap/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    20127 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot
+-rw-rw-rw-   0 root         (0) root         (0)   108738 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45404 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    23424 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff
+-rw-rw-rw-   0 root         (0) root         (0)    18028 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.835634 NEMO-5.4.1/NEMO/static/bootstrap/js/
+-rw-rw-rw-   0 root         (0) root         (0)    67546 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/js/bootstrap.js
+-rw-rw-rw-   0 root         (0) root         (0)    35951 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/bootstrap/js/bootstrap.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.836634 NEMO-5.4.1/NEMO/static/datetimepicker/
+-rw-rw-rw-   0 root         (0) root         (0)     9020 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)   105978 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.837634 NEMO-5.4.1/NEMO/static/fullcalendar/
+-rw-rw-rw-   0 root         (0) root         (0)    28531 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   358115 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)    13687 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.min.css
+-rw-rw-rw-   0 root         (0) root         (0)   166724 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.838634 NEMO-5.4.1/NEMO/static/icons/
+-rw-rw-rw-   0 root         (0) root         (0)    24065 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/icons/agreement.png
+-rw-rw-rw-   0 root         (0) root         (0)    16685 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/icons/caution.png
+-rw-rw-rw-   0 root         (0) root         (0)     4664 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/icons/preferences.png
+-rw-rw-rw-   0 root         (0) root         (0)   247387 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    84320 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/jquery.min.js
+-rw-rw-rw-   0 root         (0) root         (0)  1183392 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/jumbotron_watermark.bmp
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/mobile.js
+-rw-rw-rw-   0 root         (0) root         (0)   174603 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/moment.js
+-rw-rw-rw-   0 root         (0) root         (0)    58102 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/moment.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    86041 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/moment.min.js.map
+-rw-rw-rw-   0 root         (0) root         (0)    19266 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/nemo.css
+-rw-rw-rw-   0 root         (0) root         (0)    24034 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/static/nemo.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.838634 NEMO-5.4.1/NEMO/static/numpad/
+-rw-rw-rw-   0 root         (0) root         (0)    12285 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/numpad/custom_numpad.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)      255 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/numpad/numpad.jquery.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.840634 NEMO-5.4.1/NEMO/static/pickadate/
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/default.css
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/default.date.css
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/default.time.css
+-rw-rw-rw-   0 root         (0) root         (0)    48215 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/picker.date.js
+-rw-rw-rw-   0 root         (0) root         (0)    36941 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/picker.js
+-rw-rw-rw-   0 root         (0) root         (0)    31899 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/pickadate/picker.time.js
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/robots.txt
+-rw-rw-rw-   0 root         (0) root         (0)    48446 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/typeahead.jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    20748 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/typeahead.jquery.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.841634 NEMO-5.4.1/NEMO/static/virtualkeyboard/
+-rw-rw-rw-   0 root         (0) root         (0)   113008 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.js
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js
+-rw-rw-rw-   0 root         (0) root         (0)     7848 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/virtualkeyboard/keyboard-basic.css
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.843634 NEMO-5.4.1/NEMO/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.844634 NEMO-5.4.1/NEMO/templates/abuse/
+-rw-rw-rw-   0 root         (0) root         (0)     5236 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/abuse/abuse.html
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/abuse/user_drill_down.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.845634 NEMO-5.4.1/NEMO/templates/accounts_and_projects/
+-rw-rw-rw-   0 root         (0) root         (0)     9016 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/account_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     7399 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     3388 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/create_account.html
+-rw-rw-rw-   0 root         (0) root         (0)     7972 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/create_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1025 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/documents_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     4165 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/projects.html
+-rw-rw-rw-   0 root         (0) root         (0)    10628 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/transfer_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/accounts_and_projects/users_for_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      458 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/acknowledgement.html
+-rw-rw-rw-   0 root         (0) root         (0)     6537 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/alerts.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.847634 NEMO-5.4.1/NEMO/templates/area_access/
+-rw-rw-rw-   0 root         (0) root         (0)     4262 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/area_access.html
+-rw-rw-rw-   0 root         (0) root         (0)     2172 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/calendar_self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/change_project.html
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/login_areas.html
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/new_area_access_record.html
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/new_area_access_record_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1894 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/area_access/self_login.html
+-rw-rw-rw-   0 root         (0) root         (0)      992 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/authorization_failed.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.848634 NEMO-5.4.1/NEMO/templates/base/
+-rw-rw-rw-   0 root         (0) root         (0)      376 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base/footer.html
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base/impersonate_header.html
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base/navbar.html
+-rw-rw-rw-   0 root         (0) root         (0)    12140 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base/navbar_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base/popup.html
+-rw-rw-rw-   0 root         (0) root         (0)     7300 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.850634 NEMO-5.4.1/NEMO/templates/calendar/
+-rw-rw-rw-   0 root         (0) root         (0)    37109 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/configuration.html
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/configuration_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     3720 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/configuration_helper.html
+-rw-rw-rw-   0 root         (0) root         (0)     1417 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/policy_dialog.html
+-rw-rw-rw-   0 root         (0) root         (0)     1525 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/project_choice.html
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/proxy_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     2756 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/reservation_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     1782 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/reservation_questions.html
+-rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/reservation_warning.html
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/scheduled_outage_information.html
+-rw-rw-rw-   0 root         (0) root         (0)     2029 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/specific_user_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)     2612 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/calendar/usage_event_feed.html
+-rw-rw-rw-   0 root         (0) root         (0)    10209 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/configuration_agenda.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.851634 NEMO-5.4.1/NEMO/templates/consumables/
+-rw-rw-rw-   0 root         (0) root         (0)    11089 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/consumables/consumables.html
+-rw-rw-rw-   0 root         (0) root         (0)     1617 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/consumables/consumables_order.html
+-rw-rw-rw-   0 root         (0) root         (0)    13475 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/consumables/recurring_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     5868 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/consumables/recurring_charges.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.851634 NEMO-5.4.1/NEMO/templates/contact/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/contact/contact_staff.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.854634 NEMO-5.4.1/NEMO/templates/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)     1853 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations.html
+-rw-rw-rw-   0 root         (0) root         (0)    11038 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_application.html
+-rw-rw-rw-   0 root         (0) root         (0)    14374 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_calendar.html
+-rw-rw-rw-   0 root         (0) root         (0)    11917 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_emails.html
+-rw-rw-rw-   0 root         (0) root         (0)     2806 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_interlock.html
+-rw-rw-rw-   0 root         (0) root         (0)     2647 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_knowledge_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     7799 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_projects_and_accounts.html
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_rates.html
+-rw-rw-rw-   0 root         (0) root         (0)     4133 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_recurring_charges.html
+-rw-rw-rw-   0 root         (0) root         (0)     2907 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)    20124 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     5071 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_safety.html
+-rw-rw-rw-   0 root         (0) root         (0)    30060 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_templates.html
+-rw-rw-rw-   0 root         (0) root         (0)    19946 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_tool.html
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_training.html
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_upload.html
+-rw-rw-rw-   0 root         (0) root         (0)     6186 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/customizations/customizations_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      508 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/display_success_and_redirect.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.855634 NEMO-5.4.1/NEMO/templates/email/
+-rw-rw-rw-   0 root         (0) root         (0)    11342 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/email/compose_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     4906 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/email/email_broadcast.html
+-rw-rw-rw-   0 root         (0) root         (0)     1454 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/email/email_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.856634 NEMO-5.4.1/NEMO/templates/event_details/
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/event_details/area_access_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/event_details/outage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)    13988 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/event_details/reservation_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      623 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/event_details/usage_details.html
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/facility_rules.html
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/feedback.html
+-rw-rw-rw-   0 root         (0) root         (0)     1190 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1475 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/impersonate.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.856634 NEMO-5.4.1/NEMO/templates/jumbotron/
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/jumbotron/jumbotron.html
+-rw-rw-rw-   0 root         (0) root         (0)     5819 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/jumbotron/jumbotron_content.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.856634 NEMO-5.4.1/NEMO/templates/knowledge_base/
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     1115 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     3317 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base_items.html
+-rw-rw-rw-   0 root         (0) root         (0)    11635 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/landing.html
+-rw-rw-rw-   0 root         (0) root         (0)     4656 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.857634 NEMO-5.4.1/NEMO/templates/maintenance/
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/maintenance/closed_task_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     7551 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/maintenance/maintenance.html
+-rw-rw-rw-   0 root         (0) root         (0)    10855 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/maintenance/pending_task_details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.859634 NEMO-5.4.1/NEMO/templates/mobile/
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/cancellation_result.html
+-rw-rw-rw-   0 root         (0) root         (0)     2535 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/choose_item.html
+-rw-rw-rw-   0 root         (0) root         (0)      522 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1224 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/individual_outage.html
+-rw-rw-rw-   0 root         (0) root         (0)     4128 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/individual_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)     4814 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/new_reservation.html
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/no_active_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/reservation_extra.html
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/reservation_success.html
+-rw-rw-rw-   0 root         (0) root         (0)     1666 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/mobile/view_calendar.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.859634 NEMO-5.4.1/NEMO/templates/news/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/news/archived_news.html
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/news/new_news_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/news/news_update_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2537 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/news/recent_news.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/no_project.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.860634 NEMO-5.4.1/NEMO/templates/occupancy/
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/occupancy/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/occupancy/occupancy_content.html
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/occupancy/occupancy_count.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.860634 NEMO-5.4.1/NEMO/templates/pagination/
+-rw-rw-rw-   0 root         (0) root         (0)      839 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/pagination/pagination_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/pagination/pagination_column.html
+-rw-rw-rw-   0 root         (0) root         (0)      658 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/pagination/pagination_pages.html
+-rw-rw-rw-   0 root         (0) root         (0)      651 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/pagination/pagination_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)     3267 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/qualifications.html
+-rw-rw-rw-   0 root         (0) root         (0)     5480 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/templates/refresh_sidebar_icons.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.861635 NEMO-5.4.1/NEMO/templates/remote_work/
+-rw-rw-rw-   0 root         (0) root         (0)    13396 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/remote_work/remote_work.html
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/remote_work/remote_work_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.861635 NEMO-5.4.1/NEMO/templates/requests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.861635 NEMO-5.4.1/NEMO/templates/requests/access_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     9117 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/access_requests/access_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/access_requests/access_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     3784 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/access_requests/access_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.862635 NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     9867 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     7649 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.862635 NEMO-5.4.1/NEMO/templates/requests/buddy_requests/
+-rw-rw-rw-   0 root         (0) root         (0)     4779 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/buddy_requests/buddy_request.html
+-rw-rw-rw-   0 root         (0) root         (0)     5731 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/buddy_requests/buddy_requests.html
+-rw-rw-rw-   0 root         (0) root         (0)     4418 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/requests/user_requests.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.863634 NEMO-5.4.1/NEMO/templates/resources/
+-rw-rw-rw-   0 root         (0) root         (0)     4080 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/resources/modify_resource.html
+-rw-rw-rw-   0 root         (0) root         (0)     5358 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/resources/resource_details.html
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/resources/resources.html
+-rw-rw-rw-   0 root         (0) root         (0)     4780 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/resources/scheduled_outage.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.863634 NEMO-5.4.1/NEMO/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/rest_framework/api.html
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/rest_framework/custom_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.865635 NEMO-5.4.1/NEMO/templates/safety/
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety.html
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_base.html
+-rw-rw-rw-   0 root         (0) root         (0)     9496 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_data_sheets.html
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_issues.html
+-rw-rw-rw-   0 root         (0) root         (0)     2037 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_issues_create.html
+-rw-rw-rw-   0 root         (0) root         (0)     2400 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_issues_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     2282 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_issues_update.html
+-rw-rw-rw-   0 root         (0) root         (0)     2307 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/safety/safety_items.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.866634 NEMO-5.4.1/NEMO/templates/snippets/
+-rw-rw-rw-   0 root         (0) root         (0)      519 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/snippets/button.html
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/snippets/contact_person.html
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/snippets/document_list.html
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/snippets/embedded_document.html
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/snippets/tool_info.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.867635 NEMO-5.4.1/NEMO/templates/staff_charges/
+-rw-rw-rw-   0 root         (0) root         (0)      948 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/change_status.html
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/choose_project.html
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/end_area_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1284 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/new_staff_charge.html
+-rw-rw-rw-   0 root         (0) root         (0)     1049 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/reminder.html
+-rw-rw-rw-   0 root         (0) root         (0)     2145 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/staff_charges/staff_charges_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.867635 NEMO-5.4.1/NEMO/templates/status_dashboard/
+-rw-rw-rw-   0 root         (0) root         (0)     2333 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/status_dashboard/occupancy.html
+-rw-rw-rw-   0 root         (0) root         (0)    11703 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/status_dashboard/staff.html
+-rw-rw-rw-   0 root         (0) root         (0)     8559 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/status_dashboard/staff_absence.html
+-rw-rw-rw-   0 root         (0) root         (0)     7477 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/status_dashboard/status_dashboard.html
+-rw-rw-rw-   0 root         (0) root         (0)     4927 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/status_dashboard/tools.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.868635 NEMO-5.4.1/NEMO/templates/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)     3107 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tasks/resolve.html
+-rw-rw-rw-   0 root         (0) root         (0)     6800 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tasks/update.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.870635 NEMO-5.4.1/NEMO/templates/tool_control/
+-rw-rw-rw-   0 root         (0) root         (0)      820 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/config_history.html
+-rw-rw-rw-   0 root         (0) root         (0)     1009 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)      771 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/interlock_error.html
+-rw-rw-rw-   0 root         (0) root         (0)     1034 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/logout_user.html
+-rw-rw-rw-   0 root         (0) root         (0)     5162 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/past_tasks_and_comments.html
+-rw-rw-rw-   0 root         (0) root         (0)     3079 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/qualified_users.html
+-rw-rw-rw-   0 root         (0) root         (0)    16755 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/tool_control.html
+-rw-rw-rw-   0 root         (0) root         (0)    55529 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/tool_status.html
+-rw-rw-rw-   0 root         (0) root         (0)    10808 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/usage_data.html
+-rw-rw-rw-   0 root         (0) root         (0)      422 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/tool_control/use_tool_for_other.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.870635 NEMO-5.4.1/NEMO/templates/training/
+-rw-rw-rw-   0 root         (0) root         (0)      557 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/training/get_projects.html
+-rw-rw-rw-   0 root         (0) root         (0)     5757 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/training/training.html
+-rw-rw-rw-   0 root         (0) root         (0)     5695 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/training/training_entry.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.871635 NEMO-5.4.1/NEMO/templates/usage/
+-rw-rw-rw-   0 root         (0) root         (0)      977 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/usage/adjustment_request_button.html
+-rw-rw-rw-   0 root         (0) root         (0)     5458 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/usage/billing.html
+-rw-rw-rw-   0 root         (0) root         (0)    11290 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/usage/usage.html
+-rw-rw-rw-   0 root         (0) root         (0)    10462 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/usage/usage_base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.871635 NEMO-5.4.1/NEMO/templates/users/
+-rw-rw-rw-   0 root         (0) root         (0)    29353 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/users/create_or_modify_user.html
+-rw-rw-rw-   0 root         (0) root         (0)    21255 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/users/preferences.html
+-rw-rw-rw-   0 root         (0) root         (0)     5399 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/users/safe_deactivation.html
+-rw-rw-rw-   0 root         (0) root         (0)     5563 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/templates/users/users.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.872635 NEMO-5.4.1/NEMO/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9466 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/templatetags/custom_tags_and_filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.874635 NEMO-5.4.1/NEMO/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.874635 NEMO-5.4.1/NEMO/tests/test_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/test_api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/tests/test_api/test_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5747 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_api/test_crud.py
+-rw-rw-rw-   0 root         (0) root         (0)    29763 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/tests/test_area_access.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.876635 NEMO-5.4.1/NEMO/tests/test_calendar/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/test_calendar/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33680 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_area_reservation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)    22955 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_outage.py
+-rw-rw-rw-   0 root         (0) root         (0)    11729 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_freed_time.py
+-rw-rw-rw-   0 root         (0) root         (0)    18987 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_qualification_expiration.py
+-rw-rw-rw-   0 root         (0) root         (0)    30268 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_reservation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10126 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_closures.py
+-rw-rw-rw-   0 root         (0) root         (0)    24973 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/tests/test_consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)    15018 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     3680 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/tests/test_evaluators.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_formats.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.876635 NEMO-5.4.1/NEMO/tests/test_interlocks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/test_interlocks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3597 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_interlocks/test_modbus_interlock.py
+-rw-rw-rw-   0 root         (0) root         (0)    11445 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_interlocks/test_stanford_interlock.py
+-rw-rw-rw-   0 root         (0) root         (0)     7059 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_interlocks/test_web_relay_interlock.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.877635 NEMO-5.4.1/NEMO/tests/test_requests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/test_requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9460 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_requests/test_adjustment_requests.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.877635 NEMO-5.4.1/NEMO/tests/test_sensors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/tests/test_sensors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2229 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/tests/test_sensors/test_modbus_sensors.py
+-rw-rw-rw-   0 root         (0) root         (0)     5067 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/tests/test_staff_charges.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2024-03-20 03:03:10.000000 NEMO-5.4.1/NEMO/tests/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)    18834 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)     3390 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/tests/test_utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    32325 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    27428 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/utilities.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.885635 NEMO-5.4.1/NEMO/views/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5483 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/abuse.py
+-rw-rw-rw-   0 root         (0) root         (0)    12996 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/access_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    14108 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/accounts_and_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)    18838 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/adjustment_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/alerts.py
+-rw-rw-rw-   0 root         (0) root         (0)    22064 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/api.py
+-rw-rw-rw-   0 root         (0) root         (0)    13969 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/api_billing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2700 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/api_file_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    21857 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/area_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    13996 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     7251 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/buddy_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    55977 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2334 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/charge_validation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2705 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/configuration_agenda.py
+-rw-rw-rw-   0 root         (0) root         (0)      454 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    12946 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/views/consumables.py
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/contact_staff.py
+-rw-rw-rw-   0 root         (0) root         (0)    25225 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/customization.py
+-rw-rw-rw-   0 root         (0) root         (0)     3763 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)    14607 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/email.py
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/event_details.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/feedback.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-03-14 03:03:20.000000 NEMO-5.4.1/NEMO/views/get_projects.py
+-rw-rw-rw-   0 root         (0) root         (0)     4745 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/history.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/jumbotron.py
+-rw-rw-rw-   0 root         (0) root         (0)     3967 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/knowledge_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3631 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/landing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3007 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/maintenance.py
+-rw-rw-rw-   0 root         (0) root         (0)     9060 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/mobile.py
+-rw-rw-rw-   0 root         (0) root         (0)     3793 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/news.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/notifications.py
+-rw-rw-rw-   0 root         (0) root         (0)     1542 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     5650 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/qualifications.py
+-rw-rw-rw-   0 root         (0) root         (0)    11231 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/remote_work.py
+-rw-rw-rw-   0 root         (0) root         (0)     4095 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     9657 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/safety.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/sidebar.py
+-rw-rw-rw-   0 root         (0) root         (0)    23435 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/status_dashboard.py
+-rw-rw-rw-   0 root         (0) root         (0)    16613 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)    39347 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/timed_services.py
+-rw-rw-rw-   0 root         (0) root         (0)    30357 2024-03-21 16:29:21.000000 NEMO-5.4.1/NEMO/views/tool_control.py
+-rw-rw-rw-   0 root         (0) root         (0)     7963 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/training.py
+-rw-rw-rw-   0 root         (0) root         (0)     2164 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/tutorials.py
+-rw-rw-rw-   0 root         (0) root         (0)    21395 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/views/usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1204 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/user_requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    25049 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/views/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.886635 NEMO-5.4.1/NEMO/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-04 15:56:12.000000 NEMO-5.4.1/NEMO/widgets/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/widgets/configuration_editor.py
+-rw-rw-rw-   0 root         (0) root         (0)    39555 2024-04-03 17:49:31.000000 NEMO-5.4.1/NEMO/widgets/dynamic_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     9709 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/widgets/item_tree.py
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-06 04:03:19.000000 NEMO-5.4.1/NEMO/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 15:56:30.886635 NEMO-5.4.1/NEMO.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    20518 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-04 15:56:30.000000 NEMO-5.4.1/NEMO.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-04-04 15:56:30.887635 NEMO-5.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4478 2024-04-04 15:56:12.000000 NEMO-5.4.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-04-03 17:49:31.000000 NEMO-5.4.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-04 15:56:30.888635 NEMO-5.4.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-04 15:56:12.000000 NEMO-5.4.1/setup.py
```

### Comparing `NEMO-5.4.0/LICENSE.md` & `NEMO-5.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/__init__.py` & `NEMO-5.4.1/NEMO/__init__.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/actions.py` & `NEMO-5.4.1/NEMO/actions.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/admin.py` & `NEMO-5.4.1/NEMO/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/alerts.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/already_logged_in.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/already_logged_in.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/base.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/choose_area.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/choose_area.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/choose_project.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/logout_success.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/logout_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/logout_warning.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/logout_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/templates/area_access/resource_unavailable.html` & `NEMO-5.4.1/NEMO/apps/area_access/templates/area_access/resource_unavailable.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/urls.py` & `NEMO-5.4.1/NEMO/apps/area_access/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/area_access/views.py` & `NEMO-5.4.1/NEMO/apps/area_access/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/admin.py` & `NEMO-5.4.1/NEMO/apps/contracts/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/migrations/0001_initial.py` & `NEMO-5.4.1/NEMO/apps/contracts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/migrations/0002_increase_document_path_length.py` & `NEMO-5.4.1/NEMO/apps/contracts/migrations/0002_increase_document_path_length.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/models.py` & `NEMO-5.4.1/NEMO/apps/contracts/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/contractors.html` & `NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/contractors.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html` & `NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/contracts_and_procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/procurements.html` & `NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/procurements.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/templates/contracts/service_contracts.html` & `NEMO-5.4.1/NEMO/apps/contracts/templates/contracts/service_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/templates/customizations/customizations_contracts.html` & `NEMO-5.4.1/NEMO/apps/contracts/templates/customizations/customizations_contracts.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/urls.py` & `NEMO-5.4.1/NEMO/apps/contracts/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/contracts/views/contracts.py` & `NEMO-5.4.1/NEMO/apps/contracts/views/contracts.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/acknowledgement.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/category_choices.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/category_choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/choices.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/choices.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/error.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/kiosk.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/kiosk.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/success.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/success.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_information.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_project_selection_snippet.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/templates/kiosk/tool_reservation_extra.html` & `NEMO-5.4.1/NEMO/apps/kiosk/templates/kiosk/tool_reservation_extra.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/urls.py` & `NEMO-5.4.1/NEMO/apps/kiosk/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/kiosk/views.py` & `NEMO-5.4.1/NEMO/apps/kiosk/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/admin.py` & `NEMO-5.4.1/NEMO/apps/sensors/admin.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/customizations.py` & `NEMO-5.4.1/NEMO/apps/sensors/customizations.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/evaluators.py` & `NEMO-5.4.1/NEMO/apps/sensors/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/migrations/0001_initial.py` & `NEMO-5.4.1/NEMO/apps/sensors/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/models.py` & `NEMO-5.4.1/NEMO/apps/sensors/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/sensors.py` & `NEMO-5.4.1/NEMO/apps/sensors/sensors.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chart.js` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chart.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chart.min.js` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chart.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/chartjs-adapter-moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/daterangepicker.css` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/daterangepicker.js` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/daterangepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/static/sensors/sensors.css` & `NEMO-5.4.1/NEMO/apps/sensors/static/sensors/sensors.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/templates/customizations/customizations_sensors.html` & `NEMO-5.4.1/NEMO/apps/sensors/templates/customizations/customizations_sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/sensor_data.html` & `NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/sensor_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/templates/sensors/sensors.html` & `NEMO-5.4.1/NEMO/apps/sensors/templates/sensors/sensors.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/urls.py` & `NEMO-5.4.1/NEMO/apps/sensors/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/apps/sensors/views.py` & `NEMO-5.4.1/NEMO/apps/sensors/views.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/context_processors.py` & `NEMO-5.4.1/NEMO/context_processors.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/decorators.py` & `NEMO-5.4.1/NEMO/decorators.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/evaluators.py` & `NEMO-5.4.1/NEMO/evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/exceptions.py` & `NEMO-5.4.1/NEMO/exceptions.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/fields.py` & `NEMO-5.4.1/NEMO/fields.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/forms.py` & `NEMO-5.4.1/NEMO/forms.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/interlocks.py` & `NEMO-5.4.1/NEMO/interlocks.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/management/commands/send_email_usage_reminders.py` & `NEMO-5.4.1/NEMO/management/commands/send_email_usage_reminders.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/middleware.py` & `NEMO-5.4.1/NEMO/middleware.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0001_version_1_0_0.py` & `NEMO-5.4.1/NEMO/migrations/0001_version_1_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0002_version_1_0_0_squashed.py` & `NEMO-5.4.1/NEMO/migrations/0002_version_1_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0012_version_2_0_0_squashed.py` & `NEMO-5.4.1/NEMO/migrations/0012_version_2_0_0_squashed.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0020_version_3_0_0.py` & `NEMO-5.4.1/NEMO/migrations/0020_version_3_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0021_version_3_1_0.py` & `NEMO-5.4.1/NEMO/migrations/0021_version_3_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0022_version_3_3_0.py` & `NEMO-5.4.1/NEMO/migrations/0022_version_3_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0023_badgereader.py` & `NEMO-5.4.1/NEMO/migrations/0023_badgereader.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0024_contactinformation_user.py` & `NEMO-5.4.1/NEMO/migrations/0024_contactinformation_user.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0025_version_3_6_0.py` & `NEMO-5.4.1/NEMO/migrations/0025_version_3_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0026_version_3_7_0.py` & `NEMO-5.4.1/NEMO/migrations/0026_version_3_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0028_version_3_9_0.py` & `NEMO-5.4.1/NEMO/migrations/0028_version_3_9_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0030_version_3_9_2.py` & `NEMO-5.4.1/NEMO/migrations/0030_version_3_9_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0031_version_3_10_0.py` & `NEMO-5.4.1/NEMO/migrations/0031_version_3_10_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0032_version_3_11_0.py` & `NEMO-5.4.1/NEMO/migrations/0032_version_3_11_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0035_version_3_14_0.py` & `NEMO-5.4.1/NEMO/migrations/0035_version_3_14_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0036_version_3_15_0.py` & `NEMO-5.4.1/NEMO/migrations/0036_version_3_15_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0037_version_3_16_0.py` & `NEMO-5.4.1/NEMO/migrations/0037_version_3_16_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0038_version_4_0_0.py` & `NEMO-5.4.1/NEMO/migrations/0038_version_4_0_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0039_version_4_1_0.py` & `NEMO-5.4.1/NEMO/migrations/0039_version_4_1_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0040_version_4_2_0.py` & `NEMO-5.4.1/NEMO/migrations/0040_version_4_2_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0041_version_4_2_1.py` & `NEMO-5.4.1/NEMO/migrations/0041_version_4_2_1.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0042_version_4_3_0.py` & `NEMO-5.4.1/NEMO/migrations/0042_version_4_3_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0043_version_4_3_2.py` & `NEMO-5.4.1/NEMO/migrations/0043_version_4_3_2.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0044_version_4_4_0.py` & `NEMO-5.4.1/NEMO/migrations/0044_version_4_4_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0045_version_4_5_0.py` & `NEMO-5.4.1/NEMO/migrations/0045_version_4_5_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0045_version_4_5_5.py` & `NEMO-5.4.1/NEMO/migrations/0045_version_4_5_5.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0046_version_4_6_0.py` & `NEMO-5.4.1/NEMO/migrations/0046_version_4_6_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0048_version_4_6_3.py` & `NEMO-5.4.1/NEMO/migrations/0048_version_4_6_3.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0049_version_4_7_0.py` & `NEMO-5.4.1/NEMO/migrations/0049_version_4_7_0.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0050_consumable_add_self_checkout_and_notes.py` & `NEMO-5.4.1/NEMO/migrations/0050_consumable_add_self_checkout_and_notes.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0051_request_reviewers_in_tool_and_area.py` & `NEMO-5.4.1/NEMO/migrations/0051_request_reviewers_in_tool_and_area.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0052_area_add_auto_logout_time.py` & `NEMO-5.4.1/NEMO/migrations/0052_area_add_auto_logout_time.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0053_consumable_withdraw_add_usage_event_link.py` & `NEMO-5.4.1/NEMO/migrations/0053_consumable_withdraw_add_usage_event_link.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0054_documents_update_max_length.py` & `NEMO-5.4.1/NEMO/migrations/0054_documents_update_max_length.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0055_reservationconfigurationoption.py` & `NEMO-5.4.1/NEMO/migrations/0055_reservationconfigurationoption.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0058_reservation_confirmation_override_prefs.py` & `NEMO-5.4.1/NEMO/migrations/0058_reservation_confirmation_override_prefs.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0059_tool_pre_usage_questions.py` & `NEMO-5.4.1/NEMO/migrations/0059_tool_pre_usage_questions.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0060_add_impersonate_permission.py` & `NEMO-5.4.1/NEMO/migrations/0060_add_impersonate_permission.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0062_migrate_email_upcoming_reservation.py` & `NEMO-5.4.1/NEMO/migrations/0062_migrate_email_upcoming_reservation.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0063_knowledge_base.py` & `NEMO-5.4.1/NEMO/migrations/0063_knowledge_base.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0064_consumable_self_checkout_only_users.py` & `NEMO-5.4.1/NEMO/migrations/0064_consumable_self_checkout_only_users.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0065_door_adjacent_area.py` & `NEMO-5.4.1/NEMO/migrations/0065_door_adjacent_area.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0066_tool_ask_to_leave_area_when_done_using.py` & `NEMO-5.4.1/NEMO/migrations/0066_tool_ask_to_leave_area_when_done_using.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0067_project_allow_staff_charges.py` & `NEMO-5.4.1/NEMO/migrations/0067_project_allow_staff_charges.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations/0068_door_multiple_areas.py` & `NEMO-5.4.1/NEMO/migrations/0068_door_multiple_areas.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/migrations_utils.py` & `NEMO-5.4.1/NEMO/migrations_utils.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/mixins.py` & `NEMO-5.4.1/NEMO/mixins.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/model_tree.py` & `NEMO-5.4.1/NEMO/model_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/models.py` & `NEMO-5.4.1/NEMO/models.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/parsers.py` & `NEMO-5.4.1/NEMO/parsers.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/permissions.py` & `NEMO-5.4.1/NEMO/permissions.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/policy.py` & `NEMO-5.4.1/NEMO/policy.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/provisioning.py` & `NEMO-5.4.1/NEMO/provisioning.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/rates.py` & `NEMO-5.4.1/NEMO/rates.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/rest_filter_backend.py` & `NEMO-5.4.1/NEMO/rest_filter_backend.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/serializers.py` & `NEMO-5.4.1/NEMO/serializers.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.css` & `NEMO-5.4.1/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.js` & `NEMO-5.4.1/NEMO/static/admin/dynamic_form_preview/dynamic_form_preview.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/admin/physical_access_level/access_level.js` & `NEMO-5.4.1/NEMO/static/admin/physical_access_level/access_level.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/admin/time_options_override.js` & `NEMO-5.4.1/NEMO/static/admin/time_options_override.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/admin/tool/tool.js` & `NEMO-5.4.1/NEMO/static/admin/tool/tool.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/badge_reader.js` & `NEMO-5.4.1/NEMO/static/badge_reader.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.css` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.css.map` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap-theme.min.css` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.css` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.css.map` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/css/bootstrap.min.css` & `NEMO-5.4.1/NEMO/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot` & `NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg` & `NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf` & `NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff` & `NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2` & `NEMO-5.4.1/NEMO/static/bootstrap/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/js/bootstrap.js` & `NEMO-5.4.1/NEMO/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/bootstrap/js/bootstrap.min.js` & `NEMO-5.4.1/NEMO/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.css` & `NEMO-5.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/datetimepicker/bootstrap-datetimepicker.js` & `NEMO-5.4.1/NEMO/static/datetimepicker/bootstrap-datetimepicker.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/favicon.ico` & `NEMO-5.4.1/NEMO/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.css` & `NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.js` & `NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.min.css` & `NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/fullcalendar/fullcalendar.min.js` & `NEMO-5.4.1/NEMO/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/icons/agreement.png` & `NEMO-5.4.1/NEMO/static/icons/agreement.png`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/icons/caution.png` & `NEMO-5.4.1/NEMO/static/icons/caution.png`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/icons/preferences.png` & `NEMO-5.4.1/NEMO/static/icons/preferences.png`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/jquery.js` & `NEMO-5.4.1/NEMO/static/jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/jquery.min.js` & `NEMO-5.4.1/NEMO/static/jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/jumbotron_watermark.bmp` & `NEMO-5.4.1/NEMO/static/jumbotron_watermark.bmp`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/mobile.js` & `NEMO-5.4.1/NEMO/static/mobile.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/moment.js` & `NEMO-5.4.1/NEMO/static/moment.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/moment.min.js` & `NEMO-5.4.1/NEMO/static/moment.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/moment.min.js.map` & `NEMO-5.4.1/NEMO/static/moment.min.js.map`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/nemo.css` & `NEMO-5.4.1/NEMO/static/nemo.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/nemo.js` & `NEMO-5.4.1/NEMO/static/nemo.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/numpad/custom_numpad.jquery.js` & `NEMO-5.4.1/NEMO/static/numpad/custom_numpad.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/default.css` & `NEMO-5.4.1/NEMO/static/pickadate/default.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/default.date.css` & `NEMO-5.4.1/NEMO/static/pickadate/default.date.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/default.time.css` & `NEMO-5.4.1/NEMO/static/pickadate/default.time.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/picker.date.js` & `NEMO-5.4.1/NEMO/static/pickadate/picker.date.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/picker.js` & `NEMO-5.4.1/NEMO/static/pickadate/picker.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/pickadate/picker.time.js` & `NEMO-5.4.1/NEMO/static/pickadate/picker.time.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/typeahead.jquery.js` & `NEMO-5.4.1/NEMO/static/typeahead.jquery.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/typeahead.jquery.min.js` & `NEMO-5.4.1/NEMO/static/typeahead.jquery.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/virtualkeyboard/jquery.keyboard.js` & `NEMO-5.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/virtualkeyboard/jquery.keyboard.min.js` & `NEMO-5.4.1/NEMO/static/virtualkeyboard/jquery.keyboard.min.js`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/virtualkeyboard/keyboard-basic.css` & `NEMO-5.4.1/NEMO/static/virtualkeyboard/keyboard-basic.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/static/virtualkeyboard/keyboard-basic.min.css` & `NEMO-5.4.1/NEMO/static/virtualkeyboard/keyboard-basic.min.css`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/abuse/abuse.html` & `NEMO-5.4.1/NEMO/templates/abuse/abuse.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/abuse/user_drill_down.html` & `NEMO-5.4.1/NEMO/templates/abuse/user_drill_down.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/account_and_projects.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/account_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/accounts_and_projects.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/accounts_and_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/create_account.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/create_account.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/create_project.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/create_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/documents_for_project.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/documents_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/projects.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/transfer_charges.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/transfer_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/accounts_and_projects/users_for_project.html` & `NEMO-5.4.1/NEMO/templates/accounts_and_projects/users_for_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/alerts.html` & `NEMO-5.4.1/NEMO/templates/alerts.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/area_access.html` & `NEMO-5.4.1/NEMO/templates/area_access/area_access.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/calendar_self_login.html` & `NEMO-5.4.1/NEMO/templates/area_access/calendar_self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/change_project.html` & `NEMO-5.4.1/NEMO/templates/area_access/change_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/login_areas.html` & `NEMO-5.4.1/NEMO/templates/area_access/login_areas.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/new_area_access_record.html` & `NEMO-5.4.1/NEMO/templates/area_access/new_area_access_record.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/new_area_access_record_details.html` & `NEMO-5.4.1/NEMO/templates/area_access/new_area_access_record_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/area_access/self_login.html` & `NEMO-5.4.1/NEMO/templates/area_access/self_login.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/authorization_failed.html` & `NEMO-5.4.1/NEMO/templates/authorization_failed.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/base/navbar_base.html` & `NEMO-5.4.1/NEMO/templates/base/navbar_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/base.html` & `NEMO-5.4.1/NEMO/templates/base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/calendar.html` & `NEMO-5.4.1/NEMO/templates/calendar/calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/configuration.html` & `NEMO-5.4.1/NEMO/templates/calendar/configuration.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/configuration_event_feed.html` & `NEMO-5.4.1/NEMO/templates/calendar/configuration_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/configuration_helper.html` & `NEMO-5.4.1/NEMO/templates/calendar/configuration_helper.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/policy_dialog.html` & `NEMO-5.4.1/NEMO/templates/calendar/policy_dialog.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/project_choice.html` & `NEMO-5.4.1/NEMO/templates/calendar/project_choice.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/proxy_reservation.html` & `NEMO-5.4.1/NEMO/templates/calendar/proxy_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/reservation_event_feed.html` & `NEMO-5.4.1/NEMO/templates/calendar/reservation_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/reservation_questions.html` & `NEMO-5.4.1/NEMO/templates/calendar/reservation_questions.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/reservation_warning.html` & `NEMO-5.4.1/NEMO/templates/calendar/reservation_warning.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/scheduled_outage_information.html` & `NEMO-5.4.1/NEMO/templates/calendar/scheduled_outage_information.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/specific_user_feed.html` & `NEMO-5.4.1/NEMO/templates/calendar/specific_user_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/calendar/usage_event_feed.html` & `NEMO-5.4.1/NEMO/templates/calendar/usage_event_feed.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/configuration_agenda.html` & `NEMO-5.4.1/NEMO/templates/configuration_agenda.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/consumables/consumables.html` & `NEMO-5.4.1/NEMO/templates/consumables/consumables.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/consumables/consumables_order.html` & `NEMO-5.4.1/NEMO/templates/consumables/consumables_order.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/consumables/recurring_charge.html` & `NEMO-5.4.1/NEMO/templates/consumables/recurring_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/consumables/recurring_charges.html` & `NEMO-5.4.1/NEMO/templates/consumables/recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/contact/contact_staff.html` & `NEMO-5.4.1/NEMO/templates/contact/contact_staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_application.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_application.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_calendar.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_dashboard.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_emails.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_emails.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_interlock.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_interlock.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_knowledge_base.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_knowledge_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_projects_and_accounts.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_projects_and_accounts.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_rates.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_rates.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_recurring_charges.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_recurring_charges.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_remote_work.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_requests.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_safety.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_templates.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_templates.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_tool.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_tool.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_training.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_training.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_upload.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_upload.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/customizations/customizations_user.html` & `NEMO-5.4.1/NEMO/templates/customizations/customizations_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/email/compose_email.html` & `NEMO-5.4.1/NEMO/templates/email/compose_email.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/email/email_broadcast.html` & `NEMO-5.4.1/NEMO/templates/email/email_broadcast.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/email/email_form.html` & `NEMO-5.4.1/NEMO/templates/email/email_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/event_details/area_access_details.html` & `NEMO-5.4.1/NEMO/templates/event_details/area_access_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/event_details/outage_details.html` & `NEMO-5.4.1/NEMO/templates/event_details/outage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/event_details/reservation_details.html` & `NEMO-5.4.1/NEMO/templates/event_details/reservation_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/event_details/usage_details.html` & `NEMO-5.4.1/NEMO/templates/event_details/usage_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/feedback.html` & `NEMO-5.4.1/NEMO/templates/feedback.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/history.html` & `NEMO-5.4.1/NEMO/templates/history.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/impersonate.html` & `NEMO-5.4.1/NEMO/templates/impersonate.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/jumbotron/jumbotron.html` & `NEMO-5.4.1/NEMO/templates/jumbotron/jumbotron.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/jumbotron/jumbotron_content.html` & `NEMO-5.4.1/NEMO/templates/jumbotron/jumbotron_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base.html` & `NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base_base.html` & `NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/knowledge_base/knowledge_base_items.html` & `NEMO-5.4.1/NEMO/templates/knowledge_base/knowledge_base_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/landing.html` & `NEMO-5.4.1/NEMO/templates/landing.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/login.html` & `NEMO-5.4.1/NEMO/templates/login.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/maintenance/closed_task_details.html` & `NEMO-5.4.1/NEMO/templates/maintenance/closed_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/maintenance/maintenance.html` & `NEMO-5.4.1/NEMO/templates/maintenance/maintenance.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/maintenance/pending_task_details.html` & `NEMO-5.4.1/NEMO/templates/maintenance/pending_task_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/cancellation_result.html` & `NEMO-5.4.1/NEMO/templates/mobile/cancellation_result.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/choose_item.html` & `NEMO-5.4.1/NEMO/templates/mobile/choose_item.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/error.html` & `NEMO-5.4.1/NEMO/templates/mobile/error.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/individual_outage.html` & `NEMO-5.4.1/NEMO/templates/mobile/individual_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/individual_reservation.html` & `NEMO-5.4.1/NEMO/templates/mobile/individual_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/new_reservation.html` & `NEMO-5.4.1/NEMO/templates/mobile/new_reservation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/reservation_extra.html` & `NEMO-5.4.1/NEMO/templates/mobile/reservation_extra.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/reservation_success.html` & `NEMO-5.4.1/NEMO/templates/mobile/reservation_success.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/mobile/view_calendar.html` & `NEMO-5.4.1/NEMO/templates/mobile/view_calendar.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/news/archived_news.html` & `NEMO-5.4.1/NEMO/templates/news/archived_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/news/new_news_form.html` & `NEMO-5.4.1/NEMO/templates/news/new_news_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/news/news_update_form.html` & `NEMO-5.4.1/NEMO/templates/news/news_update_form.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/news/recent_news.html` & `NEMO-5.4.1/NEMO/templates/news/recent_news.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/occupancy/occupancy.html` & `NEMO-5.4.1/NEMO/templates/occupancy/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/occupancy/occupancy_content.html` & `NEMO-5.4.1/NEMO/templates/occupancy/occupancy_content.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/occupancy/occupancy_count.html` & `NEMO-5.4.1/NEMO/templates/occupancy/occupancy_count.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/pagination/pagination_base.html` & `NEMO-5.4.1/NEMO/templates/pagination/pagination_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/pagination/pagination_column.html` & `NEMO-5.4.1/NEMO/templates/pagination/pagination_column.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/pagination/pagination_pages.html` & `NEMO-5.4.1/NEMO/templates/pagination/pagination_pages.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/pagination/pagination_selector.html` & `NEMO-5.4.1/NEMO/templates/pagination/pagination_selector.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/qualifications.html` & `NEMO-5.4.1/NEMO/templates/qualifications.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/remote_work/remote_work.html` & `NEMO-5.4.1/NEMO/templates/remote_work/remote_work.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/remote_work/remote_work_base.html` & `NEMO-5.4.1/NEMO/templates/remote_work/remote_work_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/access_requests/access_request.html` & `NEMO-5.4.1/NEMO/templates/requests/access_requests/access_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/access_requests/access_requests.html` & `NEMO-5.4.1/NEMO/templates/requests/access_requests/access_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/access_requests/access_requests_table.html` & `NEMO-5.4.1/NEMO/templates/requests/access_requests/access_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_request.html` & `NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_requests.html` & `NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html` & `NEMO-5.4.1/NEMO/templates/requests/adjustment_requests/adjustment_requests_table.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/buddy_requests/buddy_request.html` & `NEMO-5.4.1/NEMO/templates/requests/buddy_requests/buddy_request.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/buddy_requests/buddy_requests.html` & `NEMO-5.4.1/NEMO/templates/requests/buddy_requests/buddy_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/requests/user_requests.html` & `NEMO-5.4.1/NEMO/templates/requests/user_requests.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/resources/modify_resource.html` & `NEMO-5.4.1/NEMO/templates/resources/modify_resource.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/resources/resource_details.html` & `NEMO-5.4.1/NEMO/templates/resources/resource_details.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/resources/resources.html` & `NEMO-5.4.1/NEMO/templates/resources/resources.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/resources/scheduled_outage.html` & `NEMO-5.4.1/NEMO/templates/resources/scheduled_outage.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/rest_framework/api.html` & `NEMO-5.4.1/NEMO/templates/rest_framework/api.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety.html` & `NEMO-5.4.1/NEMO/templates/safety/safety.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_base.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_data_sheets.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_data_sheets.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_issues.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_issues.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_issues_create.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_issues_create.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_issues_resolved.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_issues_resolved.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_issues_update.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_issues_update.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/safety/safety_items.html` & `NEMO-5.4.1/NEMO/templates/safety/safety_items.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/snippets/button.html` & `NEMO-5.4.1/NEMO/templates/snippets/button.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/snippets/contact_person.html` & `NEMO-5.4.1/NEMO/templates/snippets/contact_person.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/snippets/document_list.html` & `NEMO-5.4.1/NEMO/templates/snippets/document_list.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/snippets/embedded_document.html` & `NEMO-5.4.1/NEMO/templates/snippets/embedded_document.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/snippets/tool_info.html` & `NEMO-5.4.1/NEMO/templates/snippets/tool_info.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/change_status.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/change_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/choose_project.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/choose_project.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/end_area_charge.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/end_area_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/new_staff_charge.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/new_staff_charge.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/reminder.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/reminder.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/staff_charges/staff_charges_base.html` & `NEMO-5.4.1/NEMO/templates/staff_charges/staff_charges_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/status_dashboard/occupancy.html` & `NEMO-5.4.1/NEMO/templates/status_dashboard/occupancy.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/status_dashboard/staff.html` & `NEMO-5.4.1/NEMO/templates/status_dashboard/staff.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/status_dashboard/staff_absence.html` & `NEMO-5.4.1/NEMO/templates/status_dashboard/staff_absence.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/status_dashboard/status_dashboard.html` & `NEMO-5.4.1/NEMO/templates/status_dashboard/status_dashboard.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/status_dashboard/tools.html` & `NEMO-5.4.1/NEMO/templates/status_dashboard/tools.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tasks/resolve.html` & `NEMO-5.4.1/NEMO/templates/tasks/resolve.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tasks/update.html` & `NEMO-5.4.1/NEMO/templates/tasks/update.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/config_history.html` & `NEMO-5.4.1/NEMO/templates/tool_control/config_history.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/get_projects.html` & `NEMO-5.4.1/NEMO/templates/tool_control/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/interlock_error.html` & `NEMO-5.4.1/NEMO/templates/tool_control/interlock_error.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/logout_user.html` & `NEMO-5.4.1/NEMO/templates/tool_control/logout_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/past_tasks_and_comments.html` & `NEMO-5.4.1/NEMO/templates/tool_control/past_tasks_and_comments.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/qualified_users.html` & `NEMO-5.4.1/NEMO/templates/tool_control/qualified_users.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/tool_control.html` & `NEMO-5.4.1/NEMO/templates/tool_control/tool_control.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/tool_status.html` & `NEMO-5.4.1/NEMO/templates/tool_control/tool_status.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/tool_control/usage_data.html` & `NEMO-5.4.1/NEMO/templates/tool_control/usage_data.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/training/get_projects.html` & `NEMO-5.4.1/NEMO/templates/training/get_projects.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/training/training.html` & `NEMO-5.4.1/NEMO/templates/training/training.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/training/training_entry.html` & `NEMO-5.4.1/NEMO/templates/training/training_entry.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/usage/adjustment_request_button.html` & `NEMO-5.4.1/NEMO/templates/usage/adjustment_request_button.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/usage/billing.html` & `NEMO-5.4.1/NEMO/templates/usage/billing.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/usage/usage.html` & `NEMO-5.4.1/NEMO/templates/usage/usage.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/usage/usage_base.html` & `NEMO-5.4.1/NEMO/templates/usage/usage_base.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/users/create_or_modify_user.html` & `NEMO-5.4.1/NEMO/templates/users/create_or_modify_user.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/users/preferences.html` & `NEMO-5.4.1/NEMO/templates/users/preferences.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/users/safe_deactivation.html` & `NEMO-5.4.1/NEMO/templates/users/safe_deactivation.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templates/users/users.html` & `NEMO-5.4.1/NEMO/templates/users/users.html`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/templatetags/custom_tags_and_filters.py` & `NEMO-5.4.1/NEMO/templatetags/custom_tags_and_filters.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_api/test_billing.py` & `NEMO-5.4.1/NEMO/tests/test_api/test_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_api/test_crud.py` & `NEMO-5.4.1/NEMO/tests/test_api/test_crud.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_area_access.py` & `NEMO-5.4.1/NEMO/tests/test_area_access.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_area_reservation.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_area_reservation.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_calendar.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_calendar.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_outage.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_outage.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_freed_time.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_freed_time.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_qualification_expiration.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_qualification_expiration.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_calendar/test_tool_reservation.py` & `NEMO-5.4.1/NEMO/tests/test_calendar/test_tool_reservation.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_closures.py` & `NEMO-5.4.1/NEMO/tests/test_closures.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_consumables.py` & `NEMO-5.4.1/NEMO/tests/test_consumables.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_dynamic_form.py` & `NEMO-5.4.1/NEMO/tests/test_dynamic_form.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_evaluators.py` & `NEMO-5.4.1/NEMO/tests/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_formats.py` & `NEMO-5.4.1/NEMO/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_interlocks/test_modbus_interlock.py` & `NEMO-5.4.1/NEMO/tests/test_interlocks/test_modbus_interlock.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_interlocks/test_stanford_interlock.py` & `NEMO-5.4.1/NEMO/tests/test_interlocks/test_stanford_interlock.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_interlocks/test_web_relay_interlock.py` & `NEMO-5.4.1/NEMO/tests/test_interlocks/test_web_relay_interlock.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_misc.py` & `NEMO-5.4.1/NEMO/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_requests/test_adjustment_requests.py` & `NEMO-5.4.1/NEMO/tests/test_requests/test_adjustment_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_sensors/test_modbus_sensors.py` & `NEMO-5.4.1/NEMO/tests/test_sensors/test_modbus_sensors.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_settings.py` & `NEMO-5.4.1/NEMO/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_staff_charges.py` & `NEMO-5.4.1/NEMO/tests/test_staff_charges.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_tool.py` & `NEMO-5.4.1/NEMO/tests/test_tool.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_urls.py` & `NEMO-5.4.1/NEMO/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/tests/test_utilities.py` & `NEMO-5.4.1/NEMO/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/urls.py` & `NEMO-5.4.1/NEMO/urls.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/utilities.py` & `NEMO-5.4.1/NEMO/utilities.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/validators.py` & `NEMO-5.4.1/NEMO/validators.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/abuse.py` & `NEMO-5.4.1/NEMO/views/abuse.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/access_requests.py` & `NEMO-5.4.1/NEMO/views/access_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/accounts_and_projects.py` & `NEMO-5.4.1/NEMO/views/accounts_and_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/adjustment_requests.py` & `NEMO-5.4.1/NEMO/views/adjustment_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/alerts.py` & `NEMO-5.4.1/NEMO/views/alerts.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/api.py` & `NEMO-5.4.1/NEMO/views/api.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/api_billing.py` & `NEMO-5.4.1/NEMO/views/api_billing.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/api_file_import.py` & `NEMO-5.4.1/NEMO/views/api_file_import.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/area_access.py` & `NEMO-5.4.1/NEMO/views/area_access.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/authentication.py` & `NEMO-5.4.1/NEMO/views/authentication.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/buddy_requests.py` & `NEMO-5.4.1/NEMO/views/buddy_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/calendar.py` & `NEMO-5.4.1/NEMO/views/calendar.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/charge_validation.py` & `NEMO-5.4.1/NEMO/views/charge_validation.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/configuration_agenda.py` & `NEMO-5.4.1/NEMO/views/configuration_agenda.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/consumables.py` & `NEMO-5.4.1/NEMO/views/consumables.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/customization.py` & `NEMO-5.4.1/NEMO/views/customization.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/documents.py` & `NEMO-5.4.1/NEMO/views/documents.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/email.py` & `NEMO-5.4.1/NEMO/views/email.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/event_details.py` & `NEMO-5.4.1/NEMO/views/event_details.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/feedback.py` & `NEMO-5.4.1/NEMO/views/feedback.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/get_projects.py` & `NEMO-5.4.1/NEMO/views/get_projects.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/history.py` & `NEMO-5.4.1/NEMO/views/history.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/jumbotron.py` & `NEMO-5.4.1/NEMO/views/jumbotron.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/knowledge_base.py` & `NEMO-5.4.1/NEMO/views/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/landing.py` & `NEMO-5.4.1/NEMO/views/landing.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/maintenance.py` & `NEMO-5.4.1/NEMO/views/maintenance.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/mobile.py` & `NEMO-5.4.1/NEMO/views/mobile.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/news.py` & `NEMO-5.4.1/NEMO/views/news.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/notifications.py` & `NEMO-5.4.1/NEMO/views/notifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/pagination.py` & `NEMO-5.4.1/NEMO/views/pagination.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/qualifications.py` & `NEMO-5.4.1/NEMO/views/qualifications.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/remote_work.py` & `NEMO-5.4.1/NEMO/views/remote_work.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/resources.py` & `NEMO-5.4.1/NEMO/views/resources.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/safety.py` & `NEMO-5.4.1/NEMO/views/safety.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/sidebar.py` & `NEMO-5.4.1/NEMO/views/sidebar.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/status_dashboard.py` & `NEMO-5.4.1/NEMO/views/status_dashboard.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/tasks.py` & `NEMO-5.4.1/NEMO/views/tasks.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/timed_services.py` & `NEMO-5.4.1/NEMO/views/timed_services.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/tool_control.py` & `NEMO-5.4.1/NEMO/views/tool_control.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/training.py` & `NEMO-5.4.1/NEMO/views/training.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/tutorials.py` & `NEMO-5.4.1/NEMO/views/tutorials.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/usage.py` & `NEMO-5.4.1/NEMO/views/usage.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/user_requests.py` & `NEMO-5.4.1/NEMO/views/user_requests.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/views/users.py` & `NEMO-5.4.1/NEMO/views/users.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/widgets/configuration_editor.py` & `NEMO-5.4.1/NEMO/widgets/configuration_editor.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/widgets/dynamic_form.py` & `NEMO-5.4.1/NEMO/widgets/dynamic_form.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO/widgets/item_tree.py` & `NEMO-5.4.1/NEMO/widgets/item_tree.py`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/NEMO.egg-info/PKG-INFO` & `NEMO-5.4.1/NEMO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 5.4.0
+Version: 5.4.1
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-5.4.0/NEMO.egg-info/SOURCES.txt` & `NEMO-5.4.1/NEMO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NEMO-5.4.0/PKG-INFO` & `NEMO-5.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NEMO
-Version: 5.4.0
+Version: 5.4.1
 Summary: NEMO is a laboratory logistics web application. Use it to schedule reservations, control tool access, track maintenance issues, and more.
 Home-page: https://github.com/usnistgov/NEMO
 Author: Center for Nanoscale Science and Technology
 Author-email: CNSTapplications@nist.gov
 License: Public domain
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `NEMO-5.4.0/README.md` & `NEMO-5.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![Code style: black](https://img.shields.io/badge/python%20style-black-000000.svg)](https://github.com/psf/black)
 [![Code style: djlint](https://img.shields.io/badge/html%20style-djlint-black.svg)](https://www.djlint.com)
+
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/NEMO?label=python)](https://www.python.org/downloads/release/python-380/)
 [![Docker Image Version (latest semver)](https://img.shields.io/docker/v/nanofab/nemo?label=NEMO%20docker%20version)](https://hub.docker.com/r/nanofab/nemo)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/usnistgov/nemo?label=NEMO%20github%20version)](https://github.com/usnistgov/NEMO/releases)
 [![PyPI](https://img.shields.io/pypi/v/nemo?label=NEMO%20pypi%20version)](https://pypi.org/project/NEMO/)
 
 The NEMO web application is laboratory logistics software that strives to be intuitive and easy to use, making life easier in the lab. NEMO manages tool reservations, control access to tools, and streamline logistics and communication. The code is open source and free so that other labs can benefit.
```

### Comparing `NEMO-5.4.0/setup.py` & `NEMO-5.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_namespace_packages, setup
 
 setup(
     name="NEMO",
-    version="5.4.0",
+    version="5.4.1",
     python_requires=">=3.8, <4",
     packages=find_namespace_packages(exclude=["resources", "resources.*", "build", "build.*"]),
     include_package_data=True,
     url="https://github.com/usnistgov/NEMO",
     license="Public domain",
     author="Center for Nanoscale Science and Technology",
     author_email="CNSTapplications@nist.gov",
```

