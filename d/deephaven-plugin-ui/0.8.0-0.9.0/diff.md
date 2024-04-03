# Comparing `tmp/deephaven-plugin-ui-0.8.0.tar.gz` & `tmp/deephaven-plugin-ui-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-ui-0.8.0.tar", last modified: Wed Feb 28 20:18:50 2024, max compression
+gzip compressed data, was "deephaven-plugin-ui-0.9.0.tar", last modified: Sat Mar  9 00:40:15 2024, max compression
```

## Comparing `deephaven-plugin-ui-0.8.0.tar` & `deephaven-plugin-ui-0.9.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.332523 deephaven-plugin-ui-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-28 20:18:50.332523 deephaven-plugin-ui-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-02-28 20:18:50.332523 deephaven-plugin-ui-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.316523 deephaven-plugin-ui-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.316523 deephaven-plugin-ui-0.8.0/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.320523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.320523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/RenderContext.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.320523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/fragment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/html.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/item.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/make_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/picker.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/row.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/section.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.324523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/accessibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/action_button.py
--rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/button.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/button_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/flex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.324523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/BaseElement.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/DashboardElement.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/Element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/FunctionElement.py
--rw-r--r--   0 runner    (1001) docker     (127)    17654 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/UITable.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.328523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_cell_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_column_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_effect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_execution_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_liveness_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_memo.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_render_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_row_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_row_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_table_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_table_listener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.328523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/DashboardType.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/ElementMessageStream.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/ElementType.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.328523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/NodeEncoder.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/RenderedNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/Renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.328523 deephaven-plugin-ui-0.8.0/src/deephaven/ui/types/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-28 20:17:19.000000 deephaven-plugin-ui-0.8.0/src/deephaven/ui/types/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 20:18:50.332523 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-28 20:18:50.000000 deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.525283 deephaven-plugin-ui-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-09 00:40:15.525283 deephaven-plugin-ui-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-03-09 00:40:15.525283 deephaven-plugin-ui-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.513283 deephaven-plugin-ui-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.509283 deephaven-plugin-ui-0.9.0/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.513283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.513283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/RenderContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.517283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/make_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/section.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.517283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/accessibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/action_button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10854 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/button.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/button_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/flex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.517283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/BaseElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/DashboardElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/Element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/FunctionElement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19135 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/UITable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.521283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_cell_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_column_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_execution_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_liveness_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_memo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_render_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_row_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_row_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_table_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_table_listener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.521283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/DashboardType.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/ElementMessageStream.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/ElementType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.521283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/NodeEncoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/RenderedNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/Renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.521283 deephaven-plugin-ui-0.9.0/src/deephaven/ui/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-09 00:38:45.000000 deephaven-plugin-ui-0.9.0/src/deephaven/ui/types/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 00:40:15.525283 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2708 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-09 00:40:15.000000 deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-ui-0.8.0/LICENSE` & `deephaven-plugin-ui-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/PKG-INFO` & `deephaven-plugin-ui-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-ui
-Version: 0.8.0
+Version: 0.9.0
 Summary: deephaven.ui plugin
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Deephaven Data Labs
 Author-email: support@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,graph
@@ -16,14 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deephaven-core>=0.31.0
 Requires-Dist: deephaven-plugin>=0.6.0
 Requires-Dist: json-rpc
+Requires-Dist: typing_extensions
 
 # deephaven.ui Plugin
 
 Plugin prototype for programmatic layouts and callbacks. Currently calling it `deephaven.ui` but that's not set in stone.
 
 ## Build
```

### Comparing `deephaven-plugin-ui-0.8.0/README.md` & `deephaven-plugin-ui-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/setup.cfg` & `deephaven-plugin-ui-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 package_dir = 
 	=src
 packages = find_namespace:
 install_requires = 
 	deephaven-core>=0.31.0
 	deephaven-plugin>=0.6.0
 	json-rpc
+	typing_extensions
 include_package_data = True
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 deephaven.plugin =
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/__init__.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from deephaven.plugin import Registration, Callback
 from .components import *
 from .elements import *
 from .hooks import *
 from .object_types import *
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 
 class UIRegistration(Registration):
     @classmethod
     def register_into(cls, callback: Callback) -> None:
         callback.register(DashboardType)
         callback.register(ElementType)
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/RenderContext.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/RenderContext.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/_internal/utils.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/__init__.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,17 @@
 from .panel import panel
 from .spectrum import *
 from .table import table
 from .dashboard import dashboard
 from .row import row
 from .column import column
 from .stack import stack
+from .picker import picker
+from .section import section
+from .item import item
 
 from . import html
 
 
 __all__ = [
     "action_button",
     "button",
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/column.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/column.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/html.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/html.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/make_component.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/make_component.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/picker.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/picker.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import Callable, Any
 
 from deephaven.table import Table, PartitionedTable
 from .section import SectionElement, PickerItem
 from ..elements import BaseElement
 from .._internal.utils import create_props
-from ..types import ColumnName, Key, TooltipOptions
+from ..types import ColumnName, Key
 
 PickerElement = BaseElement
 
 
 def picker(
     *children: PickerItem | SectionElement | Table | PartitionedTable,
     key_column: ColumnName | None = None,
@@ -18,15 +18,14 @@
     description_column: ColumnName | None = None,
     icon_column: ColumnName | None = None,
     title_column: ColumnName | None = None,
     default_selected_key: Key | None = None,
     selected_key: Key | None = None,
     on_selection_change: Callable[[Key], None] | None = None,
     on_change: Callable[[Key], None] | None = None,
-    tooltip: bool | TooltipOptions | None = None,
     **props: Any,
 ) -> PickerElement:
     """
     A picker that can be used to select from a list. Children should be one of four types:
     If children are of type PickerItem, they are the dropdown options.
     If children are of type SectionElement, they are the dropdown sections.
     If children are of type Table, the values in the table are the dropdown options.
@@ -56,18 +55,14 @@
             The initial selected key in the collection (uncontrolled).
         selected_key:
             The currently selected key in the collection (controlled).
         on_selection_change:
             Handler that is called when the selection changes.
         on_change:
             Alias of `on_selection_change`. Handler that is called when the selection changes.
-        tooltip:
-            Whether to show a tooltip on hover.
-            If `True`, the tooltip will show.
-            If `TooltipOptions`, the tooltip will be created with the specified options.
         **props:
             Any other Picker prop, except items.
 
     Returns:
         The rendered Picker.
     """
     children, props = create_props(locals())
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/row.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/row.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/section.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/section.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/action_button.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/action_button.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/basic.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/basic.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,22 +57,14 @@
     Named icon_wrapper so as not to conflict with the Deephaven icon component.
     TODO: This doesn't seem to work correctly. It throws an error saying `Cannot read properties of undefined (reading 'className')`.
     https://react-spectrum.adobe.com/react-spectrum/Icon.html
     """
     return spectrum_element("Icon", *children, **props)
 
 
-def item(*children, **props):
-    """
-    Python implementation for the Adobe React Spectrum Item component.
-    Used with Tabs: https://react-spectrum.adobe.com/react-spectrum/Tabs.html
-    """
-    return spectrum_element("Item", *children, **props)
-
-
 def illustrated_message(*children, **props):
     """
     Python implementation for the Adobe React Spectrum IllustratedMessage component.
     https://react-spectrum.adobe.com/react-spectrum/IllustratedMessage.html
     """
     return spectrum_element("IllustratedMessage", *children, **props)
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/button.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/button.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/button_group.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/button_group.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/events.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/events.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/flex.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/flex.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/spectrum/layout.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/spectrum/layout.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/components/stack.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/components/stack.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/BaseElement.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/BaseElement.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/Element.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/Element.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/FunctionElement.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/FunctionElement.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/elements/UITable.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/elements/UITable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from __future__ import annotations
 
-import collections
 import logging
+import sys
 from typing import Callable, Literal, Sequence, Any, cast
+from warnings import warn
+
+if sys.version_info < (3, 11):
+    from typing_extensions import TypedDict, NotRequired
+else:
+    from typing import TypedDict, NotRequired
+
 from deephaven.table import Table
 from deephaven import SortDirection
 from .Element import Element
 from ..types import (
     ColumnName,
     AggregationOperation,
     SearchMode,
     QuickFilterExpression,
     Color,
     ContextMenuAction,
     CellIndex,
+    CellPressCallback,
+    ColumnPressCallback,
     RowData,
     ContextMenuMode,
     DataBarAxis,
     DataBarValuePlacement,
     DataBarDirection,
     SelectionMode,
     TableSortDirection,
@@ -44,41 +53,91 @@
     elif direction == SortDirection.DESCENDING:
         return "DESC"
     elif direction in {"ASC", "DESC"}:
         return cast(StringSortDirection, direction)
     raise ValueError(f"Invalid table sort direction: {direction}")
 
 
-class UITable(Element):
+class UITableProps(TypedDict):
+    can_search: NotRequired[bool]
     """
-    Wrap a Table with some extra props for giving hints to displaying a table
+    Whether the search bar is accessible or not. Use the system default if no value set.
+    """
+
+    on_row_press: NotRequired[RowPressCallback]
+    """
+    Callback function to run when a row is clicked.
+    The first parameter is the row index, and the second is the row data provided in a dictionary where the
+    column names are the keys.
+    """
+
+    on_row_double_press: NotRequired[RowPressCallback]
+    """
+    The callback function to run when a row is double clicked.
+    The first parameter is the row index, and the second is the row data provided in a dictionary where the
+    column names are the keys.
     """
 
-    _table: Table
+    on_cell_press: NotRequired[CellPressCallback]
     """
-    The table that is wrapped with some extra props
+    The callback function to run when a cell is clicked.
+    The first parameter is the cell index, and the second is the row data provided in a dictionary where the
+    column names are the keys.
     """
 
-    _props: dict[str, Any]
+    on_cell_double_press: NotRequired[CellPressCallback]
     """
-    The extra props that are added by each method
+    The callback function to run when a cell is double clicked.
+    The first parameter is the cell index, and the second is the row data provided in a dictionary where the
+    column names are the keys.
     """
 
-    def __init__(self, table: Table, props: dict[str, Any] = {}):
+    on_column_press: NotRequired[ColumnPressCallback]
+    """
+    The callback function to run when a column is clicked.
+    The first parameter is the column name.
+    """
+
+    on_column_double_press: NotRequired[ColumnPressCallback]
+    """
+    The callback function to run when a column is double clicked.
+    The first parameter is the column name.
+    """
+
+    table: Table
+    """
+    The table to wrap
+    """
+
+
+class UITable(Element):
+    """
+    Wrap a Table with some extra props for giving hints to displaying a table
+    """
+
+    _props: UITableProps
+    """
+    The props that are passed to the frontend
+    """
+
+    def __init__(
+        self,
+        table: Table,
+        **props: Any,
+    ):
         """
         Create a UITable from the passed in table. UITable provides an [immutable fluent interface](https://en.wikipedia.org/wiki/Fluent_interface#Immutability) for adding UI hints to a table.
 
         Args:
             table: The table to wrap
+            props: UITableProps props to pass to the frontend.
         """
-        self._table = table
 
-        # Store the extra props that are added by each method
-        # This is a shallow copy of the props so that we don't mutate the passed in props dict
-        self._props = {**props}
+        # Store all the props that were passed in
+        self._props = UITableProps(**props, table=table)
 
     @property
     def name(self):
         return "deephaven.ui.elements.UITable"
 
     def _with_prop(self, key: str, value: Any) -> "UITable":
         """
@@ -88,15 +147,15 @@
             key: The key to add to the props
             value: The value to add with the associated key
 
         Returns:
             A new UITable with the passed in prop added to the existing props
         """
         logger.debug("_with_prop(%s, %s)", key, value)
-        return UITable(self._table, {**self._props, key: value})
+        return UITable(**{**self._props, key: value})
 
     def _with_appendable_prop(self, key: str, value: Any) -> "UITable":
         """
         Create a new UITable with the passed in prop added to the existing prop
         list (if it exists) or a new list with the passed in value
 
         Args:
@@ -110,38 +169,37 @@
         existing = self._props.get(key, [])
 
         if not isinstance(existing, list):
             raise ValueError(f"Expected {key} to be a list")
 
         value = value if isinstance(value, list) else [value]
 
-        return UITable(self._table, {**self._props, key: existing + value})
+        return UITable(**{**self._props, key: existing + value})
 
-    def _with_dict_prop(self, prop_name: str, value: dict) -> "UITable":
+    def _with_dict_prop(self, key: str, value: dict[str, Any]) -> "UITable":
         """
         Create a new UITable with the passed in prop in a dictionary.
         This will override any existing prop with the same key within
         the dict stored at prop_name.
 
 
         Args:
             prop_name: The key to add to the props
             value: The value to add with the associated key
 
         Returns:
             A new UITable with the passed in prop added to the existing props
         """
-        logger.debug("_with_dict_prop(%s, %s)", prop_name, value)
-        existing = self._props.get(prop_name, {})
-        new = {**existing, **value}
-        return UITable(self._table, {**self._props, prop_name: new})
+        logger.debug("_with_dict_prop(%s, %s)", key, value)
+        existing = self._props.get(key, {})
+        return UITable(**{**self._props, key: {**existing, **value}})  # type: ignore
 
     def render(self, context: RenderContext) -> dict[str, Any]:
         logger.debug("Returning props %s", self._props)
-        return dict_to_camel_case({**self._props, "table": self._table})
+        return dict_to_camel_case({**self._props})
 
     def aggregations(
         self,
         operations: dict[ColumnName, list[AggregationOperation]],
         operation_order: list[AggregationOperation] | None = None,
         default_operation: AggregationOperation | None = None,
         group_by: list[ColumnName] | None = None,
@@ -274,17 +332,21 @@
         Returns:
             A new UITable
         """
         raise NotImplementedError()
 
     def context_menu(
         self,
-        items: ContextMenuAction
-        | list[ContextMenuAction]
-        | Callable[[CellIndex, RowData], ContextMenuAction | list[ContextMenuAction]],
+        items: (
+            ContextMenuAction
+            | list[ContextMenuAction]
+            | Callable[
+                [CellIndex, RowData], ContextMenuAction | list[ContextMenuAction]
+            ]
+        ),
         mode: ContextMenuMode = "CELL",
     ) -> "UITable":
         """
         Add custom items to the context menu.
         You can provide a list of actions that always appear,
         or a callback that can process the selection and send back menu items asynchronously.
         You can also specify whether you want the menu items provided for a cell context menu,
@@ -391,40 +453,32 @@
             columns: The columns to hide from the table. May be a single column name.
 
         Returns:
             A new UITable
         """
         raise NotImplementedError()
 
-    def on_row_press(self, callback: RowPressCallback) -> "UITable":
-        """
-        Add a callback for when a press on a row is released (e.g. a row is clicked).
-
-        Args:
-            callback: The callback function to run when a row is clicked.
-                The first parameter is the row index, and the second is the row data provided in a dictionary where the
-                column names are the keys.
-
-        Returns:
-            A new UITable
-        """
-        raise NotImplementedError()
-
     def on_row_double_press(self, callback: RowPressCallback) -> "UITable":
         """
         Add a callback for when a row is double clicked.
+        *Deprecated: Use the on_row_double_press keyword arg instead.
 
         Args:
             callback: The callback function to run when a row is double clicked.
               The first parameter is the row index, and the second is the row data provided in a dictionary where the
               column names are the keys.
 
         Returns:
             A new UITable
         """
+        warn(
+            "on_row_double_press function is deprecated. Use the on_row_double_press keyword arg instead.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self._with_prop("on_row_double_press", callback)
 
     def quick_filter(
         self, filter: dict[ColumnName, QuickFilterExpression]
     ) -> "UITable":
         """
         Add a quick filter for the UI to apply to the table.
@@ -477,15 +531,15 @@
             )
 
             # map deephaven sort direction to frontend sort direction
             direction_list = [
                 remap_sort_direction(direction) for direction in direction_list_unmapped
             ]
 
-        by_list = by if isinstance(by, Sequence) else [by]
+        by_list = [by] if isinstance(by, str) else by
 
         if direction and len(direction_list) != len(by_list):
             raise ValueError("by and direction must be the same length")
 
         if direction:
             sorts = [
                 {"column": column, "direction": direction, "is_abs": False}
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/__init__.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_callback.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_callback.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_cell_data.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_cell_data.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_column_data.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_column_data.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_effect.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_effect.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_execution_context.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_execution_context.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_liveness_scope.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_liveness_scope.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 from __future__ import annotations
 
 from .._internal import get_context
+from .use_memo import use_memo
 from .use_ref import use_ref, Ref
 from typing import Callable
 from deephaven.liveness_scope import LivenessScope
 
 
-def use_liveness_scope(func: Callable) -> Callable:
+def use_liveness_scope(func: Callable, dependencies: set) -> Callable:
     """
     Wraps a Callable in a liveness scope, and ensures that when invoked, if that callable
     causes the component to render, the scope will be retained by that render pass. It is
     not appropriate to wrap functions that will be called within the render - this is intended
     for calls made from outside a currently rendering component.
 
     Args:
         func: The function to wrap
+        dependencies: Dependencies of the provided function, so the hook knows when to re-wrap it
 
     Returns:
         The wrapped Callable
     """
     scope_ref: Ref[LivenessScope | None] = use_ref(None)
 
-    # If the value is set, the wrapped callable was invoked since we were last called - the current render
-    # cycle now will manage it, and release it when appropriate.
-    if scope_ref.current:
-        get_context().manage(scope_ref.current)
-        scope_ref.current = None
-
-    def wrapped(*args, **kwargs):
-        # If one does not exist, create a liveness scope, to hold actions from running the provided callable.
-        # Instead of releasing it right away, we leave it open until the render queue picks up any changes in
-        # that callable, see above.
-        if scope_ref.current is None:
-            scope_ref.current = LivenessScope()
-        with scope_ref.current.open():
-            func(*args, **kwargs)
+    def make_wrapper():
 
-    return wrapped
+        # If the value is set, the wrapped callable was invoked since we were last called - the current render
+        # cycle now will manage it, and release it when appropriate.
+        if scope_ref.current:
+            get_context().manage(scope_ref.current)
+            scope_ref.current = None
+
+        def wrapped(*args, **kwargs):
+            # If one does not exist, create a liveness scope, to hold actions from running the provided callable.
+            # Instead of releasing it right away, we leave it open until the render queue picks up any changes in
+            # that callable, see above.
+            if scope_ref.current is None:
+                scope_ref.current = LivenessScope()
+            with scope_ref.current.open():
+                func(*args, **kwargs)
+
+        return wrapped
+
+    return use_memo(make_wrapper, dependencies)
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_memo.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_memo.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_ref.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_ref.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_row_data.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_row_data.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_row_list.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_row_list.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_state.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_state.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_table_data.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_table_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,10 +138,12 @@
     if has_exclusive_lock(ctx.update_graph):
         executor_name = "serial"
     else:
         executor_name = "concurrent"
 
     table_updated = lambda: _set_new_data(table, sentinel, set_data, set_is_sentinel)
 
-    ui.use_table_listener(table, partial(_on_update, ctx, table_updated, executor_name))
+    ui.use_table_listener(
+        table, partial(_on_update, ctx, table_updated, executor_name), set()
+    )
 
     return transform(data, is_sentinel)
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/hooks/use_table_listener.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/hooks/use_table_listener.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from functools import partial
-from typing import Callable
+from typing import Any, Callable, Sequence
 
 from deephaven.table import Table
 from deephaven.table_listener import listen, TableUpdate, TableListener
 from deephaven.execution_context import get_exec_ctx, ExecutionContext
 
 from .use_effect import use_effect
 from ..types import LockType
@@ -63,25 +63,27 @@
         return with_ctx(listener)
     raise ValueError("Listener must be a function or a TableListener")
 
 
 def use_table_listener(
     table: Table,
     listener: Callable[[TableUpdate, bool], None] | TableListener,
+    dependencies: set[Any] | Sequence[Any],
     description: str | None = None,
     do_replay: bool = False,
     replay_lock: LockType = "shared",
 ) -> None:
     """
     Listen to a table and call a listener when the table updates.
 
     Args:
         table: The table to listen to.
         listener: Either a function or a TableListener with an on_update function.
           The function must take a TableUpdate and is_replay bool.
+        dependencies: Dependencies of the listener function, so the hook knows when to recreate the listener
         description: An optional description for the UpdatePerformanceTracker to append to the listener’s
           entry description, default is None.
         do_replay: Whether to replay the initial snapshot of the table, default is False.
         replay_lock: The lock type used during replay, default is ‘shared’, can also be ‘exclusive’.
     """
 
     if not table.is_refreshing and not do_replay:
@@ -101,8 +103,11 @@
             description=description,  # type: ignore # missing Optional type
             do_replay=do_replay,
             replay_lock=replay_lock,
         )
 
         return lambda: handle.stop()
 
-    use_effect(start_listener, {table, listener, description, do_replay, replay_lock})
+    use_effect(
+        start_listener,
+        {table, listener, description, do_replay, replay_lock} | set(dependencies),
+    )
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/ElementMessageStream.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/ElementMessageStream.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/object_types/ElementType.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/object_types/ElementType.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/NodeEncoder.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/NodeEncoder.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/RenderedNode.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/RenderedNode.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/renderer/Renderer.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/renderer/Renderer.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven/ui/types/types.py` & `deephaven-plugin-ui-0.9.0/src/deephaven/ui/types/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,74 @@
-from typing import Any, Dict, Literal, Union, List, Tuple, Optional, Callable, TypedDict
+from typing import Any, Dict, Literal, Union, List, Tuple, Callable, TypedDict
 from deephaven import SortDirection
 
-RowIndex = Optional[int]
+
+class CellData(TypedDict):
+    """
+    Data for one cell. Returned with click handlers.
+    """
+
+    type: str
+    """
+    Type of the cell data
+    """
+
+    text: str
+    """
+    Text of the cell data
+    """
+
+    value: Any
+    """
+    Raw value of the cell data
+    """
+
+
+class RowDataValue(CellData):
+    """
+    Data for value of one column in a row. Returned with row press handlers.
+    """
+
+    isExpandable: bool
+    """
+    Whether this row is expandable.
+    """
+
+    isGrouped: bool
+    """
+    Whether this row is grouped.
+    """
+
+
+ColumnIndex = int
+"""
+Index of a column in a table.
+"""
+
+RowIndex = int
+"""
+Index of a row in a table.
+"""
+
+CellIndex = Tuple[ColumnIndex, RowIndex]
+"""
+Index of a cell in a table.
+"""
+
+GridIndex = Tuple[Union[ColumnIndex, None], Union[RowIndex, None]]
+"""
+Index of a spot on the grid. A value of None indicates a header row or column.
+"""
+
+
+ColumnName = str
 RowDataMap = Dict[str, Any]
 RowPressCallback = Callable[[RowIndex, RowDataMap], None]
+CellPressCallback = Callable[[CellIndex, CellData], None]
+ColumnPressCallback = Callable[[ColumnName], None]
 AggregationOperation = Literal[
     "COUNT",
     "COUNT_DISTINCT",
     "DISTINCT",
     "MIN",
     "MAX",
     "SUM",
@@ -16,59 +77,31 @@
     "AVG",
     "STD",
     "FIRST",
     "LAST",
     "UNIQUE",
     "SKIP",
 ]
-ColumnIndex = Union[int, None]
-CellIndex = Tuple[RowIndex, ColumnIndex]
 DeephavenColor = Literal["salmon", "lemonchiffon"]
 HexColor = str
 Color = Union[DeephavenColor, HexColor]
-# A ColumnIndex of None indicates a header row
-ColumnName = str
 ContextMenuAction = Dict[str, Any]
 ContextMenuModeOption = Literal["CELL", "ROW_HEADER", "COLUMN_HEADER"]
 ContextMenuMode = Union[ContextMenuModeOption, List[ContextMenuModeOption], None]
 DataBarAxis = Literal["PROPORTIONAL", "MIDDLE", "DIRECTIONAL"]
 DataBarDirection = Literal["LTR", "RTL"]
 DataBarValuePlacement = Literal["BESIDE", "OVERLAP", "HIDE"]
 # TODO: Fill in the list of Deephaven Colors we allow
 LockType = Literal["shared", "exclusive"]
 QuickFilterExpression = str
 RowData = Dict[ColumnName, Any]
-# A RowIndex of None indicates a header column
-RowIndex = Optional[int]
 ColumnData = List[Any]
 TableData = Dict[ColumnName, ColumnData]
 SearchMode = Literal["SHOW", "HIDE", "DEFAULT"]
 SelectionMode = Literal["CELL", "ROW", "COLUMN"]
 Sentinel = Any
 TransformedData = Any
 StringSortDirection = Literal["ASC", "DESC"]
 TableSortDirection = Union[StringSortDirection, SortDirection]
 # Stringable is a type that is naturally convertible to a string
 Stringable = Union[str, int, float, bool]
 Key = Stringable
-
-PlacementOptions = Literal[
-    "auto",
-    "auto-start",
-    "auto-end",
-    "top",
-    "top-start",
-    "top-end",
-    "bottom",
-    "bottom-start",
-    "bottom-end",
-    "right",
-    "right-start",
-    "right-end",
-    "left",
-    "left-start",
-    "left-end",
-]
-
-
-class TooltipOptions(TypedDict):
-    placement: Optional[PlacementOptions]
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/PKG-INFO` & `deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-ui
-Version: 0.8.0
+Version: 0.9.0
 Summary: deephaven.ui plugin
 Home-page: https://github.com/deephaven/deephaven-plugins
 Author: Deephaven Data Labs
 Author-email: support@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugins
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugins/issues
 Keywords: deephaven,plugin,graph
@@ -16,14 +16,15 @@
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Development Status :: 3 - Alpha
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: deephaven-core>=0.31.0
 Requires-Dist: deephaven-plugin>=0.6.0
 Requires-Dist: json-rpc
+Requires-Dist: typing_extensions
 
 # deephaven.ui Plugin
 
 Plugin prototype for programmatic layouts and callbacks. Currently calling it `deephaven.ui` but that's not set in stone.
 
 ## Build
```

### Comparing `deephaven-plugin-ui-0.8.0/src/deephaven_plugin_ui.egg-info/SOURCES.txt` & `deephaven-plugin-ui-0.9.0/src/deephaven_plugin_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

