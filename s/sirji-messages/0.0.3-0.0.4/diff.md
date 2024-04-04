# Comparing `tmp/sirji-messages-0.0.3.tar.gz` & `tmp/sirji-messages-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-messages-0.0.3.tar", last modified: Wed Apr  3 15:11:57 2024, max compression
+gzip compressed data, was "sirji-messages-0.0.4.tar", last modified: Thu Apr  4 13:11:07 2024, max compression
```

## Comparing `sirji-messages-0.0.3.tar` & `sirji-messages-0.0.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.580144 sirji-messages-0.0.3/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3854 2024-04-03 15:11:57.578682 sirji-messages-0.0.3/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3561 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:11:57.580371 sirji-messages-0.0.3/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      695 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.542204 sirji-messages-0.0.3/sirji_messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      565 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/action_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/agent_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/custom_exceptions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.544950 sirji-messages-0.0.3/sirji_messages/messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.558123 sirji-messages-0.0.3/sirji_messages/messages/actions/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/acknowledge.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/answer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/create_file.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/execute_command.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/feedback.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/generate_steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/infer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/inform.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/install_package.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/problem_statement.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/question.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/response.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/solution_complete.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/step_completed.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/step_started.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      784 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_search_term.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_url.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/training_output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2668 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3351 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2335 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/permissions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.558972 sirji-messages-0.0.3/sirji_messages/system_prompts/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.564154 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2469 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      822 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/executor.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1568 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/planner.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/researcher.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/user.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/factory.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.577353 sirji-messages-0.0.3/sirji_messages.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3854 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2240 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.565100 sirji-messages-0.0.3/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.567975 sirji-messages-0.0.3/tests/integration/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_message_factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_system_prompts.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_system_prompts_base.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.574284 sirji-messages-0.0.3/tests/unit/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_actions_base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_custom_exceptions.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_enums.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.858721 sirji-messages-0.0.4/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-04 13:11:07.858117 sirji-messages-0.0.4/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3611 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:11:07.858853 sirji-messages-0.0.4/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      714 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.825589 sirji-messages-0.0.4/sirji_messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      565 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/action_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/agent_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/custom_exceptions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.828518 sirji-messages-0.0.4/sirji_messages/messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.843010 sirji-messages-0.0.4/sirji_messages/messages/actions/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/acknowledge.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/answer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/create_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/execute_command.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/feedback.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/generate_steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/infer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/inform.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/install_package.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/problem_statement.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/question.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/response.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/solution_complete.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/step_completed.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/step_started.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      783 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_search_term.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_url.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/training_output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2668 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3807 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2335 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.844040 sirji-messages-0.0.4/sirji_messages/system_prompts/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.848342 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2469 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      822 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/executor.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1676 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/planner.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/researcher.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/user.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/factory.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.857559 sirji-messages-0.0.4/sirji_messages.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2240 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.849262 sirji-messages-0.0.4/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.852034 sirji-messages-0.0.4/tests/integration/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_message_factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_system_prompts.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_system_prompts_base.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.856639 sirji-messages-0.0.4/tests/unit/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_actions_base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_custom_exceptions.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_enums.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_permissions.py
```

### Comparing `sirji-messages-0.0.3/LICENSE` & `sirji-messages-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/PKG-INFO` & `sirji-messages-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sirji-messages
 
-`sirji-messages` is a comprehensive Python package for creating, parsing, validating, and managing message interactions based on permissions in multi-agent systems or applications.
+`sirji-messages` is a PyPI package that implements the Sirji message protocol with following highlights:
+
+- Message Factory
+- Permissions Matrix (for defining message actions allowed between two agents)
+- System prompt generation
 
 ## Installation
 
 ```bash
 pip install sirji-messages
 ```
```

### Comparing `sirji-messages-0.0.3/README.md` & `sirji-messages-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 # sirji-messages
 
-`sirji-messages` is a comprehensive Python package for creating, parsing, validating, and managing message interactions based on permissions in multi-agent systems or applications.
+`sirji-messages` is a PyPI package that implements the Sirji message protocol with following highlights:
+
+- Message Factory
+- Permissions Matrix (for defining message actions allowed between two agents)
+- System prompt generation
 
 ## Installation
 
 ```bash
 pip install sirji-messages
 ```
 
@@ -114,8 +118,8 @@
 # Measure coverage, excluding test files
 coverage run --omit="tests/*" -m pytest
 coverage report
 ```
 
 ## License
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-messages-0.0.3/setup.py` & `sirji-messages-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-messages',
-    version='0.0.3',
+    version='0.0.4',
     author='Sirji',
     description='Sirji messaging protocol implementation to create, validate and parse messages.',
+    license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-messages-0.0.3/sirji_messages/__init__.py` & `sirji-messages-0.0.4/sirji_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/action_enum.py` & `sirji-messages-0.0.4/sirji_messages/action_enum.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/acknowledge.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/acknowledge.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/answer.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/answer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/base.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/create_file.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/create_file.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/execute_command.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/execute_command.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/feedback.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/feedback.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/generate_steps.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/generate_steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/infer.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/infer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/inform.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/inform.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/install_package.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/install_package.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/output.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/problem_statement.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/problem_statement.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/question.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/question.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/response.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/response.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/solution_complete.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/solution_complete.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/step_completed.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/step_completed.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/step_started.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/step_started.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/steps.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_url.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import textwrap
 
 from sirji_messages import AgentEnum, ActionEnum
 from .base import BaseMessages
 
 
-class StepsMessage(BaseMessages):
+class TrainUsingUrlMessage(BaseMessages):
 
     def __init__(self):
-        self.action = ActionEnum.STEPS.name
-        self.from_agent = AgentEnum.PLANNER.name
-        self.to_agent = AgentEnum.CODER.name
+        self.action = ActionEnum.TRAIN_USING_URL.name
+        self.from_agent = AgentEnum.CODER.name
+        self.to_agent = AgentEnum.RESEARCHER.name
 
         super().__init__()
 
     def template_payload_part(self):
         return textwrap.dedent("""
-          DETAILS:
-          {details}
+          URL: {url}
           """)
 
     def sample(self):
         return self.generate({
-            "details": "List of steps to solve the problem. Each step is described as 'Step #: ....'."
+            "url": "The URL that needs to be crawled, parsed, and trained to answer questions."
         })
 
     def description(self):
-        return "List of steps required to solve the problem:"
+        return "Train using a URL:"
 
     @staticmethod
     def custom_properties():
-        return ['DETAILS']
+        return ['URL']
```

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_search_term.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_search_term.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/actions/training_output.py` & `sirji-messages-0.0.4/sirji_messages/messages/actions/training_output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/messages/factory.py` & `sirji-messages-0.0.4/sirji_messages/messages/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/parser.py` & `sirji-messages-0.0.4/sirji_messages/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     payload_dict = _parse_payload(payload, custom_properties)
 
     parsed_message = {"FROM": message_info["FROM"], "TO": message_info["TO"],
                       "ACTION": message_info["ACTION"], **payload_dict}
 
     if parsed_message.get("ACTION") == ActionEnum.STEPS.name:
         parsed_message = {
-            **parsed_message, "parsed_steps": _parse_steps(parsed_message)}
+            **parsed_message, "PARSED_STEPS": _parse_steps(parsed_message)}
 
     return parsed_message
 
 
 def _validate_message(message):
     message = message.strip()
     if not (message.startswith("```") and message.endswith("```")):
@@ -71,21 +71,32 @@
             payload_dict[last_key] += "\n" + line
     return payload_dict
 
 
 def _parse_steps(parsed_message):
     details = parsed_message.get("DETAILS", "")
     parsed_steps = []
-    current_step_number = None
-    current_step_description = ""
-    for line in details.split("\n"):
-        if line.startswith("Step"):
-            if current_step_number is not None:
-                parsed_steps.append(
-                    {"step": current_step_number, "description": current_step_description.strip()})
-            current_step_number, current_step_description = line.split(":", 1)
-        else:
-            current_step_description += f"\n{line.strip()}"
-    if current_step_number is not None:
-        parsed_steps.append({"step": current_step_number,
-                            "description": current_step_description.strip()})
-    return parsed_steps
+    
+    if any(line.strip().startswith("Step") for line in details.split("\n")): 
+        current_step_number = None
+        current_step_description = ""
+        for line in details.split("\n"):
+            line = line.strip() 
+            if line.startswith("Step"):
+                if current_step_number is not None:
+                    parsed_steps.append(
+                        {"step": current_step_number.strip(), "description": current_step_description.strip()})
+                current_step_number, current_step_description = [part.strip() for part in line.split(":", 1)]
+            else:
+                current_step_description += f"\n{line}"
+        if current_step_number is not None:
+            parsed_steps.append({"step": current_step_number.strip(),
+                                "description": current_step_description.strip()})
+    else:
+        step_number = 1
+        for line in details.split("\n"):
+            line = line.strip()
+            if line:  
+                parsed_steps.append({"step": f"Step {step_number}", "description": line})
+                step_number += 1
+
+    return parsed_steps
```

### Comparing `sirji-messages-0.0.3/sirji_messages/permissions.py` & `sirji-messages-0.0.4/sirji_messages/permissions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/base.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/coder.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/coder.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/executor.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/executor.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/planner.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/planner.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
           You are a {self.name()} ({self.short_name()}), helping generate a list of non-technical steps required to solve the given problem statement (PS).
           """)
 
     def responsibilities(self):
         return textwrap.dedent(f"""
           - Pay close attention to PS while generating non-technical steps to solve the problem programmatically.
           - Use Python, if the programming language cannot be inferred from PS.
+          - Ensure that each step in the list of steps should start with 'Step #: ....'                    
           - Don't explain the steps further using sub-steps.
           - Generate concise steps enough to solve the problem statement.
           - Ensure that all the steps should be about either create file or install package or execute command or execute code to debug or git clone or read files.
           - Always add a step to execute the code and evaluate the response output. If the response has errors, solve them before moving ahead.                   
           - Focus on particular data points given in the PS and not solve the problem in a over-generalized manner.
           """)
```

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/researcher.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/user.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/user.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages/system_prompts/factory.py` & `sirji-messages-0.0.4/sirji_messages/system_prompts/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/sirji_messages.egg-info/PKG-INFO` & `sirji-messages-0.0.4/sirji_messages.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
+License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sirji-messages
 
-`sirji-messages` is a comprehensive Python package for creating, parsing, validating, and managing message interactions based on permissions in multi-agent systems or applications.
+`sirji-messages` is a PyPI package that implements the Sirji message protocol with following highlights:
+
+- Message Factory
+- Permissions Matrix (for defining message actions allowed between two agents)
+- System prompt generation
 
 ## Installation
 
 ```bash
 pip install sirji-messages
 ```
```

### Comparing `sirji-messages-0.0.3/sirji_messages.egg-info/SOURCES.txt` & `sirji-messages-0.0.4/sirji_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/integration/test_message_factory.py` & `sirji-messages-0.0.4/tests/integration/test_message_factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/integration/test_system_prompts.py` & `sirji-messages-0.0.4/tests/integration/test_system_prompts.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/integration/test_system_prompts_base.py` & `sirji-messages-0.0.4/tests/integration/test_system_prompts_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/unit/test_actions_base.py` & `sirji-messages-0.0.4/tests/unit/test_actions_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/unit/test_custom_exceptions.py` & `sirji-messages-0.0.4/tests/unit/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/unit/test_enums.py` & `sirji-messages-0.0.4/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/unit/test_parser.py` & `sirji-messages-0.0.4/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.3/tests/unit/test_permissions.py` & `sirji-messages-0.0.4/tests/unit/test_permissions.py`

 * *Files identical despite different names*

