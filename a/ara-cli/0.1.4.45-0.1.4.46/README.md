# Comparing `tmp/ara_cli-0.1.4.45.tar.gz` & `tmp/ara_cli-0.1.4.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ara_cli-0.1.4.45.tar", last modified: Fri May 17 21:12:57 2024, max compression
+gzip compressed data, was "ara_cli-0.1.4.46.tar", last modified: Tue May 21 07:36:03 2024, max compression
```

## Comparing `ara_cli-0.1.4.45.tar` & `ara_cli-0.1.4.46.tar`

### file list

```diff
@@ -1,142 +1,147 @@
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/MANIFEST.in
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3974 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/README.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.173994 ara_cli-0.1.4.45/ara_cli/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    11262 2024-05-17 20:51:15.000000 ara_cli-0.1.4.45/ara_cli/__main__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/ara_config.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact_deleter.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3643 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/chat.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/classifier_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/file_classifier.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/filename_validator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5995 2024-05-17 20:37:01.000000 ara_cli-0.1.4.45/ara_cli/prompt_extractor.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15579 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/prompt_handler.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/prompt_rag.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/run_file_lister.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/template_manager.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.173994 ara_cli-0.1.4.45/ara_cli/templates/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/agile.artefacts
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.169994 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.173994 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.177994 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/prompts/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.177994 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_capability.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_epic.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_feature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_task.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_userstory.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_vision.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.169994 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.177994 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1060 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      797 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1413 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      836 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      807 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_empty_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1425 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      832 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      932 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      684 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/extend_scenario_outline_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/fix_steps_for_scenario_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/formulate_new_feature_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      264 2024-05-17 19:43:31.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/implement_fibonacci_example_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_error_fixing_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      448 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_feature_reverse_formulation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      288 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_js_implementation_from_task_description_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_js_steps_implementation_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      325 2024-05-17 20:11:15.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_empty_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      471 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_gherkin_expert_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.concept.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.customer.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.persona.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.step.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.technology.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.businessgoal
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.businessgoal_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.capability
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.capability_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.epic
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.epic_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.example
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.example_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.feature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.feature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.issue
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.keyfeature
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.keyfeature_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.steps_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      442 2024-05-17 19:23:10.000000 ara_cli-0.1.4.45/ara_cli/templates/template.task
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.task_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.userstory
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.userstory_exploration.md
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.vision
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/templates/template.vision_exploration.md
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/ara_cli/tests/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/__init__.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/test_artefact_link_updater.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/test_artefact_renamer.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/test_directory_navigator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/test_file_creator.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/tests/test_template_manager.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/ara_cli/vectorDB.py
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-17 20:52:41.000000 ara_cli-0.1.4.45/ara_cli/version.py
-drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-17 21:12:57.173994 ara_cli-0.1.4.45/ara_cli.egg-info/
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/PKG-INFO
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7091 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/entry_points.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/requires.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-17 21:12:57.000000 ara_cli-0.1.4.45/ara_cli.egg-info/top_level.txt
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-17 21:12:57.181994 ara_cli-0.1.4.45/setup.cfg
--rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-17 19:15:41.000000 ara_cli-0.1.4.45/setup.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       37 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/MANIFEST.in
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3962 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/README.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       33 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    11473 2024-05-21 07:35:01.000000 ara_cli-0.1.4.46/ara_cli/__main__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2182 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/ara_config.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1916 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4786 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1583 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_deleter.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3710 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      652 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3913 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3643 2024-05-18 20:11:16.000000 ara_cli-0.1.4.46/ara_cli/chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1446 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      108 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/classifier_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2690 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1369 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/file_classifier.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1695 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      118 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/filename_validator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1759 2024-05-18 21:13:35.000000 ara_cli-0.1.4.46/ara_cli/prompt_chat.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5966 2024-05-21 07:26:18.000000 ara_cli-0.1.4.46/ara_cli/prompt_extractor.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)    15579 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/prompt_handler.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5674 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/prompt_rag.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2428 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/run_file_lister.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     6919 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/template_manager.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli/templates/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     8185 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/agile.artefacts
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.226291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1483 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       49 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/prompts/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_businessgoal.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_capability.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_epic.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_feature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_keyfeature.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_task.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_userstory.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_vision.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.234291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.238291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      829 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1060 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      797 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1413 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      836 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      807 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/empty_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1425 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1611 2024-05-19 20:39:37.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      832 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1028 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      932 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_commands.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      684 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.238291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      254 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/classify_task_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       48 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/empty_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      206 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/error_fixing_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      126 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_fix_steps_for_scenario_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      155 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_formulation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       92 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_reverse_formulation_from_code_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      201 2024-05-18 21:20:54.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      391 2024-05-19 21:21:55.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_update_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      140 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_scenario_outline_extension_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      163 2024-05-19 21:13:03.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/feature_update_formulation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      264 2024-05-19 21:13:39.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/fibonacci_example_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      207 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/js_implementation_from_task_description_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      247 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/js_steps_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      215 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/python_cli_implementation_with_test_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      450 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/python_code_understanding_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      351 2024-05-19 21:22:51.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/task_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-19 21:18:05.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/prompts/task_stepwise_implementation_intention_and_context.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      866 2024-05-19 21:29:15.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rename.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       71 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/empty_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1024 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      971 2024-05-18 19:10:04.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      814 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2200 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/product_owner_rules.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      600 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      893 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2117 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1460 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2273 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2329 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4183 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1052 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      952 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2274 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      559 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      217 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      523 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.capability
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      208 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.capability_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      680 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.epic
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.epic_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      416 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.example
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.example_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     1053 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.feature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      199 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.feature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      745 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.issue
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      803 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      211 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.steps_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      442 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.task
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      190 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.task_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.userstory
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      193 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.userstory_exploration.md
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      640 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.vision
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      226 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/templates/template.vision_exploration.md
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/ara_cli/tests/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        0 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/__init__.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2457 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_artefact_link_updater.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5275 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_artefact_renamer.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      236 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_directory_navigator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     3727 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_file_creator.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     4036 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/tests/test_template_manager.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     2330 2024-05-19 21:36:29.000000 ara_cli-0.1.4.46/ara_cli/update_config_prompt.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     5402 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/ara_cli/vectorDB.py
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      146 2024-05-21 07:20:12.000000 ara_cli-0.1.4.46/ara_cli/version.py
+drwxr-xr-x   0 pyuser    (1000) pyuser    (1000)        0 2024-05-21 07:36:03.230291 ara_cli-0.1.4.46/ara_cli.egg-info/
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       54 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)     7111 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        1 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       78 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      145 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/requires.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)        8 2024-05-21 07:36:03.000000 ara_cli-0.1.4.46/ara_cli.egg-info/top_level.txt
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)       38 2024-05-21 07:36:03.242291 ara_cli-0.1.4.46/setup.cfg
+-rw-r--r--   0 pyuser    (1000) pyuser    (1000)      782 2024-05-18 17:21:46.000000 ara_cli-0.1.4.46/setup.py
```

### Comparing `ara_cli-0.1.4.45/README.md` & `ara_cli-0.1.4.46/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 - [ara usage](#ara-usage)
-- [Build \& Publish Base Docker Image for ARA CLI API](#build--publish-base-docker-image-for-ara-cli-api)
+- [Build \& Publish Base Docker Image for ARA CLI](#build--publish-base-docker-image-for-ara-cli)
 - [ara-cli publish](#ara-cli-publish)
   - [best practices commit and merge and recreate workspace](#best-practices-commit-and-merge-and-recreate-workspace)
   - [test and run during development](#test-and-run-during-development)
   - [set version and build and install locally for testing outside of container](#set-version-and-build-and-install-locally-for-testing-outside-of-container)
   - [upload to test pypi with test pypi API key](#upload-to-test-pypi-with-test-pypi-api-key)
   - [upload to live pypi with talsen team production API key (from main branch)](#upload-to-live-pypi-with-talsen-team-production-api-key-from-main-branch)
 
 # ara usage 
 See [user readme](docs/README.md)
 
-# Build & Publish Base Docker Image for ARA CLI API
+# Build & Publish Base Docker Image for ARA CLI
 
 ```bash
 bash ./docker/base/build.sh
 ```
 
 # ara-cli publish
 ## best practices commit and merge and recreate workspace
```

### Comparing `ara_cli-0.1.4.45/ara_cli/__main__.py` & `ara_cli-0.1.4.46/ara_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ara_cli.template_manager import SpecificationBreakdownAspects, TemplatePathManager
 from ara_cli.artefact_deleter import ArtefactDeleter
 from ara_cli.artefact_lister import ArtefactLister
 from ara_cli.vectorDB import create_DB, add_paths, reset_config, reset_DB, search_DB, update_DB
 from ara_cli.prompt_handler import read_prompt, send_prompt, append_headings, write_prompt_result, default_prompt_creation, initialize_prompt_templates, load_selected_prompt_templates, create_and_send_custom_prompt
 from ara_cli.prompt_extractor import extract_and_save_prompt_results
 from ara_cli.prompt_rag import search_and_add_relevant_files_to_prompt_givens
+from ara_cli.prompt_chat import initialize_prompt_chat_mode
 
 from ara_cli.chat import Chat
 
 def check_validity(condition, error_message):
     if not condition:
         print(error_message)
         sys.exit(1)
@@ -75,14 +76,16 @@
         search_and_add_relevant_files_to_prompt_givens(classifier, param)  # Invoking new method for 'init-rag' command
     elif (init == 'load'):
         load_selected_prompt_templates(classifier, param)
     elif (init == 'send'):
         create_and_send_custom_prompt(classifier, param)
     elif (init == 'extract'):
         extract_and_save_prompt_results(classifier, param)
+    elif (init == 'chat'):
+        initialize_prompt_chat_mode(classifier, param)  # Updated to call new method
     else:
         default_prompt_creation(classifier, param)
         prompt = read_prompt(classifier, param)
         
         if(prompt):
             append_headings(classifier, param, "prompt")
             write_prompt_result(classifier, param, prompt)
@@ -153,17 +156,16 @@
     list_parser = subparsers.add_parser("list", help="List files with optional tags")
     list_parser.add_argument("tags", nargs="*", help="Tags for listing files")
 
 def prompt_parser(subparsers):
     prompt_parser = subparsers.add_parser("prompt", help="Base command for prompt interaction mode")
     prompt_parser.add_argument("parameter", help="Name of artefact data directory for prompt creation and interaction")
     prompt_parser.add_argument("classifier", help="Classifier of the artefact")
-    prompt_parser.add_argument("steps", choices=['init', 'load', 'send', 'extract'],
-                               help="steps to be performed: 'init', 'load', 'send', or 'extract' the prompt config files in the prompt directory")
-
+    prompt_parser.add_argument("steps", choices=['init', 'load', 'send', 'extract', 'chat', 'init-rag'],
+                               help="steps to be performed: 'init', 'load', 'send', 'extract', 'chat', or 'init-rag' the prompt config files in the prompt directory")
 
 def vector_init_parser(vector_subparsers):
     init_parser = vector_subparsers.add_parser("init", help="Initialize vectorDB")
 
 def vector_update_parser(vector_subparsers):
     update_parser = vector_subparsers.add_parser("update", help="Update vectorDB")
     update_parser.add_argument("path", nargs='*', help="Path(s) to add to config file", default=None)
```

### Comparing `ara_cli-0.1.4.45/ara_cli/ara_config.py` & `ara_cli-0.1.4.46/ara_cli/ara_config.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact.py` & `ara_cli-0.1.4.46/ara_cli/artefact.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact_creator.py` & `ara_cli-0.1.4.46/ara_cli/artefact_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact_deleter.py` & `ara_cli-0.1.4.46/ara_cli/artefact_deleter.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact_link_updater.py` & `ara_cli-0.1.4.46/ara_cli/artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact_lister.py` & `ara_cli-0.1.4.46/ara_cli/artefact_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/artefact_renamer.py` & `ara_cli-0.1.4.46/ara_cli/artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/chat.py` & `ara_cli-0.1.4.46/ara_cli/chat.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/classifier.py` & `ara_cli-0.1.4.46/ara_cli/classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/directory_navigator.py` & `ara_cli-0.1.4.46/ara_cli/directory_navigator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/file_classifier.py` & `ara_cli-0.1.4.46/ara_cli/file_classifier.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/file_lister.py` & `ara_cli-0.1.4.46/ara_cli/file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/prompt_extractor.py` & `ara_cli-0.1.4.46/ara_cli/prompt_extractor.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,16 +59,20 @@
     print(f"Debug: End of extraction. Found {block_extraction_counter} blocks.")
 
 def modify_and_save_file(response, file_path):
     print(f"Debug: Modifying and saving file {file_path}")
     try:
         response_data = json_repair.loads(response)
         filename_from_response = response_data['filename']
-        print(f"Debug: Response parsed, filename from response: {filename_from_response}")
-
+        print(f"""Found in JSON merge response {response[:200]} ...
+        the file {filename_from_response}
+        loaded as this content string: 
+        {response_data['content'][:100]} ...
+        """)
+        
         if filename_from_response != file_path:
             user_decision = prompt_user_decision("Filename does not match, overwrite? (y/n): ")
             if user_decision.lower() not in ['y', 'yes']:
                 print("Debug: User chose not to overwrite")
                 print("Skipping block.")
                 return
 
@@ -106,25 +110,24 @@
     ```
     {content}
     ```
     * and given this existing file {filename}
     ```
     {content_of_existing_file}
     ```
-    * then merge the new content into {filename}
-    * merge the provided information only; do not add any new details
-    * as prompt response format of the merged file use strictly the following json format. Escape special characters properly so that your response is always a valid json format:
+    * Merge the new content into {filename}.
+    * Include only the provided information; do not add any new details.
+    * Use the following JSON format for the prompt response of the merged file:
     {{
-        "filename": "path\\filename.filextension",
-        "content":  "full content of the modified file"
-    }}
-    * do not respond any more than the specified valid json response format 
+        "filename": "path/filename.filextension",
+        "content":  "full content of the modified file in valid json format"
+    }} 
     """
 
-    print(f"Debug: modification prompt created: {prompt_text}")
+    # print(f"Debug: modification prompt created: {prompt_text}")
 
     return prompt_text
 
 def handle_existing_file(filename, block_content):
     if not os.path.isfile(filename):
         print(f"File {filename} does not exist, attempting to create")
         create_file_if_not_exist(filename, block_content)
```

### Comparing `ara_cli-0.1.4.45/ara_cli/prompt_handler.py` & `ara_cli-0.1.4.46/ara_cli/prompt_handler.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/prompt_rag.py` & `ara_cli-0.1.4.46/ara_cli/prompt_rag.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/run_file_lister.py` & `ara_cli-0.1.4.46/ara_cli/run_file_lister.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/template_manager.py` & `ara_cli-0.1.4.46/ara_cli/template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/agile.artefacts` & `ara_cli-0.1.4.46/ara_cli/templates/agile.artefacts`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_businessgoal.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_capability.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_epic.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_feature.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_keyfeature.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_task.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_userstory.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/commands/template_vision.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/commands/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_businessgoal.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_businessgoal.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_capability.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_capability.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_epic.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_epic.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_feature.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_feature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_keyfeature.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_keyfeature.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_task.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_task.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_userstory.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_userstory.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-creation/rules/template_vision.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-creation/rules/template_vision.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_empty_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/empty_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/error_fixing_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/refactoring_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/product_owner_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md` & `ara_cli-0.1.4.46/ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.concept.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.concept_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.customer.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.customer_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.persona.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.persona_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.step.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.step.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.technology.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md` & `ara_cli-0.1.4.46/ara_cli/templates/specification_breakdown_files/template.technology_exploration.md`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.businessgoal` & `ara_cli-0.1.4.46/ara_cli/templates/template.businessgoal`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.capability` & `ara_cli-0.1.4.46/ara_cli/templates/template.capability`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.epic` & `ara_cli-0.1.4.46/ara_cli/templates/template.epic`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.feature` & `ara_cli-0.1.4.46/ara_cli/templates/template.feature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.issue` & `ara_cli-0.1.4.46/ara_cli/templates/template.issue`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.keyfeature` & `ara_cli-0.1.4.46/ara_cli/templates/template.keyfeature`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.userstory` & `ara_cli-0.1.4.46/ara_cli/templates/template.userstory`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/templates/template.vision` & `ara_cli-0.1.4.46/ara_cli/templates/template.vision`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/tests/test_artefact_link_updater.py` & `ara_cli-0.1.4.46/ara_cli/tests/test_artefact_link_updater.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/tests/test_artefact_renamer.py` & `ara_cli-0.1.4.46/ara_cli/tests/test_artefact_renamer.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/tests/test_file_creator.py` & `ara_cli-0.1.4.46/ara_cli/tests/test_file_creator.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/tests/test_template_manager.py` & `ara_cli-0.1.4.46/ara_cli/tests/test_template_manager.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli/vectorDB.py` & `ara_cli-0.1.4.46/ara_cli/vectorDB.py`

 * *Files identical despite different names*

### Comparing `ara_cli-0.1.4.45/ara_cli.egg-info/SOURCES.txt` & `ara_cli-0.1.4.46/ara_cli.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,21 @@
 ara_cli/chat.py
 ara_cli/classifier.py
 ara_cli/classifier_validator.py
 ara_cli/directory_navigator.py
 ara_cli/file_classifier.py
 ara_cli/file_lister.py
 ara_cli/filename_validator.py
+ara_cli/prompt_chat.py
 ara_cli/prompt_extractor.py
 ara_cli/prompt_handler.py
 ara_cli/prompt_rag.py
 ara_cli/run_file_lister.py
 ara_cli/template_manager.py
+ara_cli/update_config_prompt.py
 ara_cli/vectorDB.py
 ara_cli/version.py
 ara_cli.egg-info/PKG-INFO
 ara_cli.egg-info/SOURCES.txt
 ara_cli.egg-info/dependency_links.txt
 ara_cli.egg-info/entry_points.txt
 ara_cli.egg-info/requires.txt
@@ -71,47 +73,50 @@
 ara_cli/templates/prompt-creation/rules/template_capability.md
 ara_cli/templates/prompt-creation/rules/template_epic.md
 ara_cli/templates/prompt-creation/rules/template_feature.md
 ara_cli/templates/prompt-creation/rules/template_keyfeature.md
 ara_cli/templates/prompt-creation/rules/template_task.md
 ara_cli/templates/prompt-creation/rules/template_userstory.md
 ara_cli/templates/prompt-creation/rules/template_vision.md
-ara_cli/templates/prompt-modules/commands/template_artefact_classification_commands.md
-ara_cli/templates/prompt-modules/commands/template_artefact_extension_commands.md
-ara_cli/templates/prompt-modules/commands/template_artefact_formulation_commands.md
-ara_cli/templates/prompt-modules/commands/template_code_generation_complex_commands.md
-ara_cli/templates/prompt-modules/commands/template_code_generation_simple_commands.md
-ara_cli/templates/prompt-modules/commands/template_empty_commands.md
-ara_cli/templates/prompt-modules/commands/template_error_fixing_commands.md
-ara_cli/templates/prompt-modules/commands/template_js_code_generation_simple_commands.md
-ara_cli/templates/prompt-modules/commands/template_refactoring_analysis_commands.md
-ara_cli/templates/prompt-modules/commands/template_refactoring_commands.md
-ara_cli/templates/prompt-modules/commands/template_reverse_engineer_feature_file_commands.md
-ara_cli/templates/prompt-modules/prompts/extend_scenario_outline_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/fix_steps_for_scenario_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/formulate_new_feature_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/implement_fibonacci_example_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_classify_task_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_empty_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_error_fixing_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_extend_feature_and_implementation_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_feature_reverse_formulation_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_feature_scenario_adaption_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_feature_scenario_implementation_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_js_implementation_from_task_description_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_js_steps_implementation_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_python_cli_implementation_with_test_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_python_code_understanding_intention_and_context.md
-ara_cli/templates/prompt-modules/prompts/template_python_implementation_from_task_description_intention_and_context.md
-ara_cli/templates/prompt-modules/rules/template_empty_rules.md
-ara_cli/templates/prompt-modules/rules/template_error_analysis_expert_rules.md
-ara_cli/templates/prompt-modules/rules/template_gherkin_expert_rules.md
-ara_cli/templates/prompt-modules/rules/template_js_expert_developer_rules.md
-ara_cli/templates/prompt-modules/rules/template_product_owner_rules.md
-ara_cli/templates/prompt-modules/rules/template_python_expert_developer_rules.md
+ara_cli/templates/prompt-modules/rename.py
+ara_cli/templates/prompt-modules/commands/artefact_classification_commands.md
+ara_cli/templates/prompt-modules/commands/artefact_extension_commands.md
+ara_cli/templates/prompt-modules/commands/artefact_formulation_commands.md
+ara_cli/templates/prompt-modules/commands/code_generation_complex_commands.md
+ara_cli/templates/prompt-modules/commands/code_generation_simple_commands.md
+ara_cli/templates/prompt-modules/commands/empty_commands.md
+ara_cli/templates/prompt-modules/commands/error_fixing_commands.md
+ara_cli/templates/prompt-modules/commands/feature_file_update_commands.md
+ara_cli/templates/prompt-modules/commands/js_code_generation_simple_commands.md
+ara_cli/templates/prompt-modules/commands/refactoring_analysis_commands.md
+ara_cli/templates/prompt-modules/commands/refactoring_commands.md
+ara_cli/templates/prompt-modules/commands/reverse_engineer_feature_file_commands.md
+ara_cli/templates/prompt-modules/prompts/classify_task_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/empty_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/error_fixing_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_fix_steps_for_scenario_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_formulation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_reverse_formulation_from_code_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_scenario_implementation_update_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_scenario_outline_extension_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/feature_update_formulation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/fibonacci_example_implementation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/js_implementation_from_task_description_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/js_steps_implementation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/python_cli_implementation_with_test_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/python_code_understanding_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/task_implementation_intention_and_context.md
+ara_cli/templates/prompt-modules/prompts/task_stepwise_implementation_intention_and_context.md
+ara_cli/templates/prompt-modules/rules/empty_rules.md
+ara_cli/templates/prompt-modules/rules/error_analysis_expert_rules.md
+ara_cli/templates/prompt-modules/rules/gherkin_expert_rules.md
+ara_cli/templates/prompt-modules/rules/js_expert_developer_rules.md
+ara_cli/templates/prompt-modules/rules/product_owner_rules.md
+ara_cli/templates/prompt-modules/rules/python_expert_developer_rules.md
 ara_cli/templates/specification_breakdown_files/template.concept.md
 ara_cli/templates/specification_breakdown_files/template.concept_exploration.md
 ara_cli/templates/specification_breakdown_files/template.customer.md
 ara_cli/templates/specification_breakdown_files/template.customer_exploration.md
 ara_cli/templates/specification_breakdown_files/template.persona.md
 ara_cli/templates/specification_breakdown_files/template.persona_exploration.md
 ara_cli/templates/specification_breakdown_files/template.step.md
```

### Comparing `ara_cli-0.1.4.45/setup.py` & `ara_cli-0.1.4.46/setup.py`

 * *Files identical despite different names*

