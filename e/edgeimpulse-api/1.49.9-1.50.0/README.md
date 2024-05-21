# Comparing `tmp/edgeimpulse_api-1.49.9.tar.gz` & `tmp/edgeimpulse_api-1.50.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgeimpulse_api-1.49.9.tar", max compression
+gzip compressed data, was "edgeimpulse_api-1.50.0.tar", max compression
```

## Comparing `edgeimpulse_api-1.49.9.tar` & `edgeimpulse_api-1.50.0.tar`

### file list

```diff
@@ -1,925 +1,941 @@
--rw-r--r--   0        0        0      377 2024-04-17 10:43:42.926402 edgeimpulse_api-1.49.9/README.md
--rw-r--r--   0        0        0    88508 2024-04-17 10:44:15.302117 edgeimpulse_api-1.49.9/edgeimpulse_api/__init__.py
--rw-r--r--   0        0        0     2172 2024-04-17 10:43:42.926402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/__init__.py
--rw-r--r--   0        0        0   386649 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/admin_api.py
--rw-r--r--   0        0        0    11231 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/auth_api.py
--rw-r--r--   0        0        0     6235 2024-04-17 10:43:42.930402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/cdn_api.py
--rw-r--r--   0        0        0    59980 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/classify_api.py
--rw-r--r--   0        0        0    72480 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/deployment_api.py
--rw-r--r--   0        0        0    80789 2024-04-17 10:43:42.934402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/devices_api.py
--rw-r--r--   0        0        0   139045 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/dsp_api.py
--rw-r--r--   0        0        0    19442 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/email_verification_api.py
--rw-r--r--   0        0        0     6435 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/export_api.py
--rw-r--r--   0        0        0     5996 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/feature_flags_api.py
--rw-r--r--   0        0        0    11921 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/health_api.py
--rw-r--r--   0        0        0    49621 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/impulse_api.py
--rw-r--r--   0        0        0   238420 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/jobs_api.py
--rw-r--r--   0        0        0   154112 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/learn_api.py
--rw-r--r--   0        0        0     6483 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/login_api.py
--rw-r--r--   0        0        0    17897 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/metrics_api.py
--rw-r--r--   0        0        0    85275 2024-04-17 10:43:42.938402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/optimization_api.py
--rw-r--r--   0        0        0   197840 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_blocks_api.py
--rw-r--r--   0        0        0    92715 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_create_project_api.py
--rw-r--r--   0        0        0   331750 2024-04-17 10:43:42.942402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_api.py
--rw-r--r--   0        0        0    80882 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_campaigns_api.py
--rw-r--r--   0        0        0    58218 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_jobs_api.py
--rw-r--r--   0        0        0    53291 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_pipelines_api.py
--rw-r--r--   0        0        0    45490 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_portals_api.py
--rw-r--r--   0        0        0   505317 2024-04-17 10:43:42.946402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/organizations_api.py
--rw-r--r--   0        0        0    60377 2024-04-17 10:43:42.950402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/performance_calibration_api.py
--rw-r--r--   0        0        0   270960 2024-04-17 10:43:42.954402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/projects_api.py
--rw-r--r--   0        0        0   414581 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/raw_data_api.py
--rw-r--r--   0        0        0    35671 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/themes_api.py
--rw-r--r--   0        0        0    43486 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/third_party_auth_api.py
--rw-r--r--   0        0        0    45692 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/upload_portal_api.py
--rw-r--r--   0        0        0   247228 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/user_api.py
--rw-r--r--   0        0        0    42135 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api/whitelabels_api.py
--rw-r--r--   0        0        0    29331 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/api_client.py
--rw-r--r--   0        0        0    15659 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/configuration.py
--rw-r--r--   0        0        0     5113 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/exceptions.py
--rw-r--r--   0        0        0    85883 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/__init__.py
--rw-r--r--   0        0        0     2897 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
--rw-r--r--   0        0        0     1982 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_or_verify_email_request.py
--rw-r--r--   0        0        0     2052 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_api_key_request.py
--rw-r--r--   0        0        0     1963 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_collaborator_request.py
--rw-r--r--   0        0        0     2223 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_hmac_key_request.py
--rw-r--r--   0        0        0     2299 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_member_request.py
--rw-r--r--   0        0        0     2418 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request.py
--rw-r--r--   0        0        0     2122 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
--rw-r--r--   0        0        0     2806 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_bucket_request.py
--rw-r--r--   0        0        0     2794 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     2469 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2152 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     4230 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2359 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2042 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
--rw-r--r--   0        0        0     2269 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2816 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2054 2024-04-17 10:43:42.958402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_request.py
--rw-r--r--   0        0        0     2266 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response.py
--rw-r--r--   0        0        0     1949 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response_all_of.py
--rw-r--r--   0        0        0     4885 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     2339 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     6169 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_request.py
--rw-r--r--   0        0        0     2325 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2001 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2659 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request.py
--rw-r--r--   0        0        0     2370 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     1940 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
--rw-r--r--   0        0        0     1961 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
--rw-r--r--   0        0        0     2661 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_api_key_request.py
--rw-r--r--   0        0        0     2542 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request.py
--rw-r--r--   0        0        0     2246 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
--rw-r--r--   0        0        0     2344 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request.py
--rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
--rw-r--r--   0        0        0     2146 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_user_request.py
--rw-r--r--   0        0        0     2097 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_user_request.py
--rw-r--r--   0        0        0     5903 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization.py
--rw-r--r--   0        0        0     2396 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization_all_of.py
--rw-r--r--   0        0        0     3259 2024-04-17 10:43:42.962402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_project.py
--rw-r--r--   0        0        0     7529 2024-04-17 10:43:42.966402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user.py
--rw-r--r--   0        0        0     5318 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user_all_of.py
--rw-r--r--   0        0        0     2386 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_data_export_request.py
--rw-r--r--   0        0        0     2262 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_request.py
--rw-r--r--   0        0        0     2718 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_project_request.py
--rw-r--r--   0        0        0     1905 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_enable_feature_request.py
--rw-r--r--   0        0        0     2546 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response.py
--rw-r--r--   0        0        0     2222 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
--rw-r--r--   0        0        0     2735 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response.py
--rw-r--r--   0        0        0     2428 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
--rw-r--r--   0        0        0     2318 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
--rw-r--r--   0        0        0     2022 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
--rw-r--r--   0        0        0     2217 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response.py
--rw-r--r--   0        0        0     1910 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
--rw-r--r--   0        0        0     3148 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
--rw-r--r--   0        0        0     2647 2024-04-17 10:43:42.970402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2323 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
--rw-r--r--   0        0        0     3029 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     3046 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response.py
--rw-r--r--   0        0        0     2746 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
--rw-r--r--   0        0        0     3409 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
--rw-r--r--   0        0        0     2243 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
--rw-r--r--   0        0        0     1947 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
--rw-r--r--   0        0        0     2914 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response.py
--rw-r--r--   0        0        0     2614 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
--rw-r--r--   0        0        0     2096 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
--rw-r--r--   0        0        0     2208 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response.py
--rw-r--r--   0        0        0     1901 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
--rw-r--r--   0        0        0     2245 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_metrics_response.py
--rw-r--r--   0        0        0     2452 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response.py
--rw-r--r--   0        0        0     2128 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response_all_of.py
--rw-r--r--   0        0        0     2507 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response.py
--rw-r--r--   0        0        0     2183 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
--rw-r--r--   0        0        0     2807 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response.py
--rw-r--r--   0        0        0     2500 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of.py
--rw-r--r--   0        0        0     2878 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
--rw-r--r--   0        0        0     2445 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects.py
--rw-r--r--   0        0        0     2836 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects_response.py
--rw-r--r--   0        0        0     4245 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response.py
--rw-r--r--   0        0        0     3084 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response_all_of.py
--rw-r--r--   0        0        0     2158 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_toggle_data_migration_request.py
--rw-r--r--   0        0        0     2397 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_data_export_request.py
--rw-r--r--   0        0        0     3936 2024-04-17 10:43:42.974402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_request.py
--rw-r--r--   0        0        0     2015 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_permissions_request.py
--rw-r--r--   0        0        0     2830 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_request.py
--rw-r--r--   0        0        0     2532 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_trial_request.py
--rw-r--r--   0        0        0     2525 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/akida_edge_learning_config.py
--rw-r--r--   0        0        0      512 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_capacity.py
--rw-r--r--   0        0        0     2512 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata.py
--rw-r--r--   0        0        0     2212 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
--rw-r--r--   0        0        0     5499 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata.py
--rw-r--r--   0        0        0     5221 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
--rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
--rw-r--r--   0        0        0     4079 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response.py
--rw-r--r--   0        0        0     3812 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of.py
--rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of_axes.py
--rw-r--r--   0        0        0     3188 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_result.py
--rw-r--r--   0        0        0     3029 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response.py
--rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2375 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     3358 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/application_budget.py
--rw-r--r--   0        0        0      506 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_image_enum.py
--rw-r--r--   0        0        0     3635 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_spectrogram.py
--rw-r--r--   0        0        0     1895 2024-04-17 10:43:42.978402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/autotune_dsp_request.py
--rw-r--r--   0        0        0      505 2024-04-17 10:43:42.982402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_display_category.py
--rw-r--r--   0        0        0      560 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_type.py
--rw-r--r--   0        0        0     2044 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box.py
--rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box_with_score.py
--rw-r--r--   0        0        0     2197 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_on_device_model_request.py
--rw-r--r--   0        0        0     2433 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_organization_on_device_model_request.py
--rw-r--r--   0        0        0     2459 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
--rw-r--r--   0        0        0     2041 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/change_password_request.py
--rw-r--r--   0        0        0     3701 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response.py
--rw-r--r--   0        0        0     3394 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of.py
--rw-r--r--   0        0        0     3769 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
--rw-r--r--   0        0        0     2055 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
--rw-r--r--   0        0        0     3255 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page.py
--rw-r--r--   0        0        0     2948 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page_all_of.py
--rw-r--r--   0        0        0     4026 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response.py
--rw-r--r--   0        0        0     3759 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_all_of.py
--rw-r--r--   0        0        0     6252 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification.py
--rw-r--r--   0        0        0     2755 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification_details.py
--rw-r--r--   0        0        0     3816 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_v2200_response.py
--rw-r--r--   0        0        0     3004 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/convert_user_request.py
--rw-r--r--   0        0        0     3495 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_data.py
--rw-r--r--   0        0        0     3114 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue.py
--rw-r--r--   0        0        0     3241 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
--rw-r--r--   0        0        0     2484 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
--rw-r--r--   0        0        0     2183 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response.py
--rw-r--r--   0        0        0     1859 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response_all_of.py
--rw-r--r--   0        0        0     2255 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response.py
--rw-r--r--   0        0        0     1938 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response_all_of.py
--rw-r--r--   0        0        0     2404 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response.py
--rw-r--r--   0        0        0     2125 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response_all_of.py
--rw-r--r--   0        0        0     2387 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_device_request.py
--rw-r--r--   0        0        0     2850 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response.py
--rw-r--r--   0        0        0     2319 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
--rw-r--r--   0        0        0     6569 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request.py
--rw-r--r--   0        0        0     4092 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
--rw-r--r--   0        0        0     2491 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response.py
--rw-r--r--   0        0        0     2185 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
--rw-r--r--   0        0        0     2600 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_request.py
--rw-r--r--   0        0        0     2830 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response.py
--rw-r--r--   0        0        0     2551 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     1990 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_request.py
--rw-r--r--   0        0        0     2454 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response.py
--rw-r--r--   0        0        0     2148 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response_all_of.py
--rw-r--r--   0        0        0     2155 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_usage_report_body.py
--rw-r--r--   0        0        0     2185 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_pipeline_response.py
--rw-r--r--   0        0        0     2504 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_request.py
--rw-r--r--   0        0        0     2378 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response.py
--rw-r--r--   0        0        0     2072 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response_all_of.py
--rw-r--r--   0        0        0     2276 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_request.py
--rw-r--r--   0        0        0     2414 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response.py
--rw-r--r--   0        0        0     2135 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
--rw-r--r--   0        0        0     2413 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_request.py
--rw-r--r--   0        0        0     2450 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response.py
--rw-r--r--   0        0        0     2144 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     4197 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_request.py
--rw-r--r--   0        0        0     2393 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response.py
--rw-r--r--   0        0        0     2114 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response_all_of.py
--rw-r--r--   0        0        0     2919 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_request.py
--rw-r--r--   0        0        0     2672 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response.py
--rw-r--r--   0        0        0     2393 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response_all_of.py
--rw-r--r--   0        0        0     4384 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_request.py
--rw-r--r--   0        0        0     2438 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response.py
--rw-r--r--   0        0        0     2121 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2094 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/created_updated_by_user.py
--rw-r--r--   0        0        0     2051 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_request.py
--rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response.py
--rw-r--r--   0        0        0     1943 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response_all_of.py
--rw-r--r--   0        0        0     2368 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data.py
--rw-r--r--   0        0        0     3412 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data_scores_inner.py
--rw-r--r--   0        0        0     4054 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign.py
--rw-r--r--   0        0        0     2989 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_dashboard.py
--rw-r--r--   0        0        0     2786 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph.py
--rw-r--r--   0        0        0     3352 2024-04-17 10:43:42.986402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
--rw-r--r--   0        0        0     2047 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
--rw-r--r--   0        0        0     1934 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_link.py
--rw-r--r--   0        0        0     1957 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_query.py
--rw-r--r--   0        0        0     3292 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response.py
--rw-r--r--   0        0        0     3003 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
--rw-r--r--   0        0        0     2838 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_settings.py
--rw-r--r--   0        0        0     2149 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data.py
--rw-r--r--   0        0        0     2111 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data_ratio.py
--rw-r--r--   0        0        0     1898 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/delete_portal_file_request.py
--rw-r--r--   0        0        0     2230 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dependency_data.py
--rw-r--r--   0        0        0     2280 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
--rw-r--r--   0        0        0     2408 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
--rw-r--r--   0        0        0     2155 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
--rw-r--r--   0        0        0     2484 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
--rw-r--r--   0        0        0     2344 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
--rw-r--r--   0        0        0     2780 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
--rw-r--r--   0        0        0     2200 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
--rw-r--r--   0        0        0     4397 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request.py
--rw-r--r--   0        0        0     2833 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
--rw-r--r--   0        0        0     8503 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
--rw-r--r--   0        0        0     8065 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
--rw-r--r--   0        0        0     5950 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target.py
--rw-r--r--   0        0        0     1926 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_badge.py
--rw-r--r--   0        0        0      737 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_engine.py
--rw-r--r--   0        0        0     2702 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response.py
--rw-r--r--   0        0        0     2395 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     2248 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_created_response.py
--rw-r--r--   0        0        0     2032 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request.py
--rw-r--r--   0        0        0     2134 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request_update.py
--rw-r--r--   0        0        0     2113 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_response.py
--rw-r--r--   0        0        0     2864 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response.py
--rw-r--r--   0        0        0     2564 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response_all_of.py
--rw-r--r--   0        0        0     2030 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys.py
--rw-r--r--   0        0        0     2400 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys_response.py
--rw-r--r--   0        0        0     4816 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device.py
--rw-r--r--   0        0        0      516 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_debug_stream_type.py
--rw-r--r--   0        0        0     2811 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_inference_info.py
--rw-r--r--   0        0        0     2199 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response.py
--rw-r--r--   0        0        0     1920 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response_all_of.py
--rw-r--r--   0        0        0     2231 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_sensors_inner.py
--rw-r--r--   0        0        0     2094 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download.py
--rw-r--r--   0        0        0     1912 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_request.py
--rw-r--r--   0        0        0     2260 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response.py
--rw-r--r--   0        0        0     1954 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response_all_of.py
--rw-r--r--   0        0        0     2724 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results.py
--rw-r--r--   0        0        0     2417 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
--rw-r--r--   0        0        0     1968 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
--rw-r--r--   0        0        0     3660 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_block.py
--rw-r--r--   0        0        0     1834 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_request.py
--rw-r--r--   0        0        0     3092 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response.py
--rw-r--r--   0        0        0     2813 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response_all_of.py
--rw-r--r--   0        0        0     3016 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response.py
--rw-r--r--   0        0        0     2728 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
--rw-r--r--   0        0        0     2058 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
--rw-r--r--   0        0        0     2572 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
--rw-r--r--   0        0        0     2216 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response.py
--rw-r--r--   0        0        0     1920 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
--rw-r--r--   0        0        0     2294 2024-04-17 10:43:42.990402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group.py
--rw-r--r--   0        0        0     4216 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item.py
--rw-r--r--   0        0        0     2190 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
--rw-r--r--   0        0        0     2195 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_show_if.py
--rw-r--r--   0        0        0     4848 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info.py
--rw-r--r--   0        0        0     2376 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_features.py
--rw-r--r--   0        0        0     1885 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_performance.py
--rw-r--r--   0        0        0     5462 2024-04-17 10:43:42.994402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata.py
--rw-r--r--   0        0        0     2025 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
--rw-r--r--   0        0        0     2566 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config.py
--rw-r--r--   0        0        0     2531 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
--rw-r--r--   0        0        0     5820 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_response.py
--rw-r--r--   0        0        0     1963 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_named_axis.py
--rw-r--r--   0        0        0     3019 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response.py
--rw-r--r--   0        0        0     2729 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2278 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
--rw-r--r--   0        0        0     4639 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph.py
--rw-r--r--   0        0        0     1899 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
--rw-r--r--   0        0        0     2677 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_with_features.py
--rw-r--r--   0        0        0     2151 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features.py
--rw-r--r--   0        0        0     2030 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
--rw-r--r--   0        0        0     3697 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response.py
--rw-r--r--   0        0        0     3418 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of.py
--rw-r--r--   0        0        0     1969 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
--rw-r--r--   0        0        0     4579 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample.py
--rw-r--r--   0        0        0     4312 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
--rw-r--r--   0        0        0     3342 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response.py
--rw-r--r--   0        0        0     3042 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
--rw-r--r--   0        0        0     2748 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
--rw-r--r--   0        0        0     2213 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
--rw-r--r--   0        0        0     3353 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response.py
--rw-r--r--   0        0        0     3053 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
--rw-r--r--   0        0        0     2773 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
--rw-r--r--   0        0        0     2205 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
--rw-r--r--   0        0        0     1893 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/edit_sample_label_request.py
--rw-r--r--   0        0        0     4246 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_trial.py
--rw-r--r--   0        0        0     2960 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
--rw-r--r--   0        0        0     2885 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entitlement_limits.py
--rw-r--r--   0        0        0     2367 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response.py
--rw-r--r--   0        0        0     2077 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response_all_of.py
--rw-r--r--   0        0        0     2656 2024-04-17 10:43:42.998402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response.py
--rw-r--r--   0        0        0     2349 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response_all_of.py
--rw-r--r--   0        0        0     2099 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_result_value.py
--rw-r--r--   0        0        0     2366 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response.py
--rw-r--r--   0        0        0     2060 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response_all_of.py
--rw-r--r--   0        0        0     2511 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response.py
--rw-r--r--   0        0        0     2244 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response_all_of.py
--rw-r--r--   0        0        0     2116 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_keras_block_data_request.py
--rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_original_data_request.py
--rw-r--r--   0        0        0     2021 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_wav_data_request.py
--rw-r--r--   0        0        0      500 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/feature.py
--rw-r--r--   0        0        0     2206 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_request.py
--rw-r--r--   0        0        0     2804 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response.py
--rw-r--r--   0        0        0     2497 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of.py
--rw-r--r--   0        0        0     2090 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
--rw-r--r--   0        0        0     2665 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response.py
--rw-r--r--   0        0        0     2358 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of.py
--rw-r--r--   0        0        0     2322 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of_users.py
--rw-r--r--   0        0        0     2507 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/generate_features_request.py
--rw-r--r--   0        0        0     2083 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/generic_api_response.py
--rw-r--r--   0        0        0     2764 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response.py
--rw-r--r--   0        0        0     2457 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
--rw-r--r--   0        0        0     2156 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
--rw-r--r--   0        0        0     2698 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response.py
--rw-r--r--   0        0        0     2391 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     2713 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response.py
--rw-r--r--   0        0        0     2406 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
--rw-r--r--   0        0        0     3527 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response.py
--rw-r--r--   0        0        0     3260 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
--rw-r--r--   0        0        0     2588 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
--rw-r--r--   0        0        0     1954 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
--rw-r--r--   0        0        0     2345 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
--rw-r--r--   0        0        0     2078 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
--rw-r--r--   0        0        0     3400 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response.py
--rw-r--r--   0        0        0     3122 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0     3752 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response.py
--rw-r--r--   0        0        0     2402 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
--rw-r--r--   0        0        0     2349 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response.py
--rw-r--r--   0        0        0     2071 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response_all_of.py
--rw-r--r--   0        0        0     2434 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response.py
--rw-r--r--   0        0        0     2137 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response_all_of.py
--rw-r--r--   0        0        0     2752 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response.py
--rw-r--r--   0        0        0     2455 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of.py
--rw-r--r--   0        0        0     4251 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
--rw-r--r--   0        0        0     2859 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
--rw-r--r--   0        0        0     2456 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response.py
--rw-r--r--   0        0        0     2177 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
--rw-r--r--   0        0        0     2350 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response.py
--rw-r--r--   0        0        0     2045 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
--rw-r--r--   0        0        0     2788 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response.py
--rw-r--r--   0        0        0     2488 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of.py
--rw-r--r--   0        0        0     2118 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
--rw-r--r--   0        0        0     3930 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response.py
--rw-r--r--   0        0        0     3630 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
--rw-r--r--   0        0        0     2429 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request.py
--rw-r--r--   0        0        0     2007 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request_range.py
--rw-r--r--   0        0        0     2454 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response.py
--rw-r--r--   0        0        0     2157 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response_all_of.py
--rw-r--r--   0        0        0     2374 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response.py
--rw-r--r--   0        0        0     2077 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response_all_of.py
--rw-r--r--   0        0        0     3070 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_request.py
--rw-r--r--   0        0        0     2431 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response.py
--rw-r--r--   0        0        0     2152 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response_all_of.py
--rw-r--r--   0        0        0     2580 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response.py
--rw-r--r--   0        0        0     2256 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
--rw-r--r--   0        0        0     3358 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
--rw-r--r--   0        0        0     3578 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response.py
--rw-r--r--   0        0        0     3300 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
--rw-r--r--   0        0        0     2869 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
--rw-r--r--   0        0        0     2572 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response.py
--rw-r--r--   0        0        0     2265 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response_all_of.py
--rw-r--r--   0        0        0     2556 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response.py
--rw-r--r--   0        0        0     2232 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2701 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
--rw-r--r--   0        0        0     2377 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
--rw-r--r--   0        0        0     2890 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
--rw-r--r--   0        0        0     2583 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
--rw-r--r--   0        0        0     3158 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_response.py
--rw-r--r--   0        0        0     2939 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response.py
--rw-r--r--   0        0        0     2632 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
--rw-r--r--   0        0        0     2601 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response.py
--rw-r--r--   0        0        0     2277 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
--rw-r--r--   0        0        0     2982 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response.py
--rw-r--r--   0        0        0     2682 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
--rw-r--r--   0        0        0     2561 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response.py
--rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
--rw-r--r--   0        0        0     3411 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
--rw-r--r--   0        0        0     3111 2024-04-17 10:43:43.002402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
--rw-r--r--   0        0        0     3532 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
--rw-r--r--   0        0        0     2576 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response.py
--rw-r--r--   0        0        0     2252 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
--rw-r--r--   0        0        0     2690 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response.py
--rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
--rw-r--r--   0        0        0     2627 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response.py
--rw-r--r--   0        0        0     2310 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
--rw-r--r--   0        0        0     2603 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response.py
--rw-r--r--   0        0        0     2279 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     3670 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response.py
--rw-r--r--   0        0        0     3391 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2323 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_projects_data_count_response.py
--rw-r--r--   0        0        0     2906 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
--rw-r--r--   0        0        0     2589 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response.py
--rw-r--r--   0        0        0     2541 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
--rw-r--r--   0        0        0     2612 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_usage_report_response.py
--rw-r--r--   0        0        0     2905 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
--rw-r--r--   0        0        0     2598 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
--rw-r--r--   0        0        0     3012 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
--rw-r--r--   0        0        0     2712 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
--rw-r--r--   0        0        0     2722 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
--rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
--rw-r--r--   0        0        0     2922 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
--rw-r--r--   0        0        0     2615 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
--rw-r--r--   0        0        0     3151 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response.py
--rw-r--r--   0        0        0     2884 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
--rw-r--r--   0        0        0     3761 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response.py
--rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     4031 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
--rw-r--r--   0        0        0     2978 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
--rw-r--r--   0        0        0     3058 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
--rw-r--r--   0        0        0     2397 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response.py
--rw-r--r--   0        0        0     2073 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response_all_of.py
--rw-r--r--   0        0        0     2767 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_metadata_response.py
--rw-r--r--   0        0        0     3044 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_response.py
--rw-r--r--   0        0        0     2462 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response.py
--rw-r--r--   0        0        0     2184 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
--rw-r--r--   0        0        0     2694 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response.py
--rw-r--r--   0        0        0     2404 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response_all_of.py
--rw-r--r--   0        0        0     2414 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response.py
--rw-r--r--   0        0        0     2117 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response_all_of.py
--rw-r--r--   0        0        0     2592 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response.py
--rw-r--r--   0        0        0     2285 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response_all_of.py
--rw-r--r--   0        0        0     2495 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response.py
--rw-r--r--   0        0        0     2171 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
--rw-r--r--   0        0        0     3543 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response.py
--rw-r--r--   0        0        0     3276 2024-04-17 10:43:43.006402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
--rw-r--r--   0        0        0     8163 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response.py
--rw-r--r--   0        0        0     5497 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of.py
--rw-r--r--   0        0        0     2395 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
--rw-r--r--   0        0        0     2307 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response.py
--rw-r--r--   0        0        0     2021 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
--rw-r--r--   0        0        0     2514 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response.py
--rw-r--r--   0        0        0     2217 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response_all_of.py
--rw-r--r--   0        0        0     2776 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response.py
--rw-r--r--   0        0        0     2498 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
--rw-r--r--   0        0        0      580 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/image_input_scaling.py
--rw-r--r--   0        0        0     3738 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse.py
--rw-r--r--   0        0        0     6723 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_block_version.py
--rw-r--r--   0        0        0     6814 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block.py
--rw-r--r--   0        0        0     1967 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block_organization.py
--rw-r--r--   0        0        0     8958 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_input_block.py
--rw-r--r--   0        0        0     5612 2024-04-17 10:43:43.010402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_learn_block.py
--rw-r--r--   0        0        0     2627 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/input_block.py
--rw-r--r--   0        0        0     2323 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/invite_organization_member_request.py
--rw-r--r--   0        0        0     4172 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job.py
--rw-r--r--   0        0        0     2066 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_created_by_user.py
--rw-r--r--   0        0        0     5203 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details.py
--rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_all_of.py
--rw-r--r--   0        0        0     2613 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response.py
--rw-r--r--   0        0        0     2316 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response_all_of.py
--rw-r--r--   0        0        0     2257 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_failure_details.py
--rw-r--r--   0        0        0     2657 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response.py
--rw-r--r--   0        0        0     2350 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response_all_of.py
--rw-r--r--   0        0        0     3297 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response.py
--rw-r--r--   0        0        0     3007 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response_all_of.py
--rw-r--r--   0        0        0      546 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_parent_type_enum.py
--rw-r--r--   0        0        0     2944 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state.py
--rw-r--r--   0        0        0     1966 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state_execution_details.py
--rw-r--r--   0        0        0      598 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_status.py
--rw-r--r--   0        0        0     2965 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_step.py
--rw-r--r--   0        0        0     2713 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response.py
--rw-r--r--   0        0        0     2406 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of.py
--rw-r--r--   0        0        0     2089 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of_summary.py
--rw-r--r--   0        0        0     1961 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
--rw-r--r--   0        0        0     1993 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_custom_metric.py
--rw-r--r--   0        0        0     2510 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer.py
--rw-r--r--   0        0        0     2093 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_input.py
--rw-r--r--   0        0        0     2101 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_output.py
--rw-r--r--   0        0        0     5707 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata.py
--rw-r--r--   0        0        0     5440 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_all_of.py
--rw-r--r--   0        0        0     5421 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics.py
--rw-r--r--   0        0        0     4495 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
--rw-r--r--   0        0        0     2497 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
--rw-r--r--   0        0        0      562 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_type_enum.py
--rw-r--r--   0        0        0      524 2024-04-17 10:43:43.014402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_variant_enum.py
--rw-r--r--   0        0        0    11377 2024-04-17 10:43:43.018401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response.py
--rw-r--r--   0        0        0    11110 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response_all_of.py
--rw-r--r--   0        0        0     3392 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer.py
--rw-r--r--   0        0        0     2310 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer_type.py
--rw-r--r--   0        0        0     2529 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response.py
--rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response_all_of.py
--rw-r--r--   0        0        0     2633 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/latency_device.py
--rw-r--r--   0        0        0     3146 2024-04-17 10:43:43.022401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block.py
--rw-r--r--   0        0        0      933 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block_type.py
--rw-r--r--   0        0        0     2788 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response.py
--rw-r--r--   0        0        0     2488 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2619 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response.py
--rw-r--r--   0        0        0     2312 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response_all_of.py
--rw-r--r--   0        0        0     2726 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response.py
--rw-r--r--   0        0        0     2426 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of.py
--rw-r--r--   0        0        0     2918 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of_emails.py
--rw-r--r--   0        0        0     2767 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response.py
--rw-r--r--   0        0        0     2467 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
--rw-r--r--   0        0        0     2813 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response.py
--rw-r--r--   0        0        0     2513 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
--rw-r--r--   0        0        0     2381 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
--rw-r--r--   0        0        0     2745 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response.py
--rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response_all_of.py
--rw-r--r--   0        0        0     2200 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response.py
--rw-r--r--   0        0        0     1910 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response_all_of.py
--rw-r--r--   0        0        0     2921 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response.py
--rw-r--r--   0        0        0     2621 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
--rw-r--r--   0        0        0     2752 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response.py
--rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
--rw-r--r--   0        0        0     2902 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response.py
--rw-r--r--   0        0        0     2595 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
--rw-r--r--   0        0        0     2760 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
--rw-r--r--   0        0        0     3310 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response.py
--rw-r--r--   0        0        0     3031 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of.py
--rw-r--r--   0        0        0     3430 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
--rw-r--r--   0        0        0     2887 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
--rw-r--r--   0        0        0     2587 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
--rw-r--r--   0        0        0     2824 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
--rw-r--r--   0        0        0     2524 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
--rw-r--r--   0        0        0     3353 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response.py
--rw-r--r--   0        0        0     3074 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response_all_of.py
--rw-r--r--   0        0        0     2792 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response.py
--rw-r--r--   0        0        0     2485 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
--rw-r--r--   0        0        0     2857 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response.py
--rw-r--r--   0        0        0     2550 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of.py
--rw-r--r--   0        0        0     2858 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
--rw-r--r--   0        0        0     3449 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response.py
--rw-r--r--   0        0        0     3142 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
--rw-r--r--   0        0        0     2271 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
--rw-r--r--   0        0        0     2857 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response.py
--rw-r--r--   0        0        0     2550 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
--rw-r--r--   0        0        0     2819 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
--rw-r--r--   0        0        0     3103 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
--rw-r--r--   0        0        0     2803 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
--rw-r--r--   0        0        0     3055 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2755 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2988 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response.py
--rw-r--r--   0        0        0     2688 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
--rw-r--r--   0        0        0     2786 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response.py
--rw-r--r--   0        0        0     2486 2024-04-17 10:43:43.026401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response_all_of.py
--rw-r--r--   0        0        0     2512 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_request.py
--rw-r--r--   0        0        0     2872 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response.py
--rw-r--r--   0        0        0     2593 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects.py
--rw-r--r--   0        0        0     2681 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects_response.py
--rw-r--r--   0        0        0     3122 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
--rw-r--r--   0        0        0     2822 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
--rw-r--r--   0        0        0     2553 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects.py
--rw-r--r--   0        0        0     2944 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects_response.py
--rw-r--r--   0        0        0     2815 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response.py
--rw-r--r--   0        0        0     2508 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of.py
--rw-r--r--   0        0        0     2290 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2754 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response.py
--rw-r--r--   0        0        0     2454 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response_all_of.py
--rw-r--r--   0        0        0     2615 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response.py
--rw-r--r--   0        0        0     2308 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
--rw-r--r--   0        0        0     3933 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response.py
--rw-r--r--   0        0        0     3633 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of.py
--rw-r--r--   0        0        0     2353 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
--rw-r--r--   0        0        0     2053 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
--rw-r--r--   0        0        0     3960 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_versions.py
--rw-r--r--   0        0        0     2367 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_analytics_event_request.py
--rw-r--r--   0        0        0     2900 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response.py
--rw-r--r--   0        0        0     2600 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of.py
--rw-r--r--   0        0        0     2441 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
--rw-r--r--   0        0        0     2191 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_website_pageview_request.py
--rw-r--r--   0        0        0     2217 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response.py
--rw-r--r--   0        0        0     1911 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response_all_of.py
--rw-r--r--   0        0        0     2528 2024-04-17 10:43:43.030402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/memory_spec.py
--rw-r--r--   0        0        0     2746 2024-04-17 10:43:43.034402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response.py
--rw-r--r--   0        0        0     2449 2024-04-17 10:43:43.034402 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
--rw-r--r--   0        0        0     2128 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_for_model_variant.py
--rw-r--r--   0        0        0     2430 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/migration.py
--rw-r--r--   0        0        0      571 2024-04-17 10:43:43.038401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_engine_short_enum.py
--rw-r--r--   0        0        0     3010 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_prediction.py
--rw-r--r--   0        0        0     2895 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_result.py
--rw-r--r--   0        0        0     5046 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_variant_stats.py
--rw-r--r--   0        0        0     2128 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/move_raw_data_request.py
--rw-r--r--   0        0        0     2784 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_data.py
--rw-r--r--   0        0        0     3584 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score.py
--rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
--rw-r--r--   0        0        0     2687 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/note.py
--rw-r--r--   0        0        0     2221 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_request.py
--rw-r--r--   0        0        0     2994 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response.py
--rw-r--r--   0        0        0     2705 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
--rw-r--r--   0        0        0     2275 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
--rw-r--r--   0        0        0     2368 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response.py
--rw-r--r--   0        0        0     2051 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
--rw-r--r--   0        0        0     2887 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response.py
--rw-r--r--   0        0        0     2580 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
--rw-r--r--   0        0        0      775 2024-04-17 10:43:43.042401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_last_layer.py
--rw-r--r--   0        0        0     6491 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config.py
--rw-r--r--   0        0        0     6949 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response.py
--rw-r--r--   0        0        0     1920 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response_all_of.py
--rw-r--r--   0        0        0     2056 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_target_device.py
--rw-r--r--   0        0        0     2271 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response.py
--rw-r--r--   0        0        0     1964 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response.py
--rw-r--r--   0        0        0     2456 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response_all_of.py
--rw-r--r--   0        0        0     5546 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response.py
--rw-r--r--   0        0        0     5279 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of.py
--rw-r--r--   0        0        0     3284 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_status.py
--rw-r--r--   0        0        0     2273 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
--rw-r--r--   0        0        0     2749 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
--rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.046401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
--rw-r--r--   0        0        0     4717 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
--rw-r--r--   0        0        0     5801 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization.py
--rw-r--r--   0        0        0     2700 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_request.py
--rw-r--r--   0        0        0     2498 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response.py
--rw-r--r--   0        0        0     2209 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
--rw-r--r--   0        0        0     2835 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request.py
--rw-r--r--   0        0        0     2493 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
--rw-r--r--   0        0        0     2820 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_bucket.py
--rw-r--r--   0        0        0     2711 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_compute_time_usage.py
--rw-r--r--   0        0        0     9492 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project.py
--rw-r--r--   0        0        0      605 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
--rw-r--r--   0        0        0     2262 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_path_filter.py
--rw-r--r--   0        0        0     7464 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_request.py
--rw-r--r--   0        0        0     2543 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response.py
--rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response_all_of.py
--rw-r--r--   0        0        0     2704 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response.py
--rw-r--r--   0        0        0     2407 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
--rw-r--r--   0        0        0     2754 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_transformation_summary.py
--rw-r--r--   0        0        0    10387 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files.py
--rw-r--r--   0        0        0     2744 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
--rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
--rw-r--r--   0        0        0     2559 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request.py
--rw-r--r--   0        0        0     2327 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
--rw-r--r--   0        0        0     3041 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response.py
--rw-r--r--   0        0        0     2741 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
--rw-r--r--   0        0        0     2468 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
--rw-r--r--   0        0        0     3483 2024-04-17 10:43:43.050401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_export.py
--rw-r--r--   0        0        0     3476 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item.py
--rw-r--r--   0        0        0     2303 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item_files_inner.py
--rw-r--r--   0        0        0     4007 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset.py
--rw-r--r--   0        0        0     2800 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset_bucket.py
--rw-r--r--   0        0        0     6005 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_deploy_block.py
--rw-r--r--   0        0        0     4962 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dsp_block.py
--rw-r--r--   0        0        0     3037 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response.py
--rw-r--r--   0        0        0     2737 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
--rw-r--r--   0        0        0     7063 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
--rw-r--r--   0        0        0     6864 2024-04-17 10:43:43.054401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response.py
--rw-r--r--   0        0        0     6574 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of.py
--rw-r--r--   0        0        0     3915 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
--rw-r--r--   0        0        0     2267 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
--rw-r--r--   0        0        0     2338 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
--rw-r--r--   0        0        0     2458 2024-04-17 10:43:43.058401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
--rw-r--r--   0        0        0     2101 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_performance.py
--rw-r--r--   0        0        0      525 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_member_role.py
--rw-r--r--   0        0        0     2639 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response.py
--rw-r--r--   0        0        0     2315 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of.py
--rw-r--r--   0        0        0     4480 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
--rw-r--r--   0        0        0     6143 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline.py
--rw-r--r--   0        0        0     2595 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
--rw-r--r--   0        0        0     2275 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
--rw-r--r--   0        0        0     2314 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_item_count.py
--rw-r--r--   0        0        0     4129 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run.py
--rw-r--r--   0        0        0     5330 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run_step.py
--rw-r--r--   0        0        0     6532 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_step.py
--rw-r--r--   0        0        0     2351 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
--rw-r--r--   0        0        0     2344 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
--rw-r--r--   0        0        0     2037 2024-04-17 10:43:43.062401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_request.py
--rw-r--r--   0        0        0     7242 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_block.py
--rw-r--r--   0        0        0      611 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
--rw-r--r--   0        0        0     8670 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transformation_block.py
--rw-r--r--   0        0        0     3918 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_update_pipeline_body.py
--rw-r--r--   0        0        0     3351 2024-04-17 10:43:43.066401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_usage_report.py
--rw-r--r--   0        0        0     4882 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user.py
--rw-r--r--   0        0        0     2294 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user_all_of.py
--rw-r--r--   0        0        0     2104 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_detection.py
--rw-r--r--   0        0        0     3434 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_false_positive.py
--rw-r--r--   0        0        0     3770 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth.py
--rw-r--r--   0        0        0     2477 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
--rw-r--r--   0        0        0     4880 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set.py
--rw-r--r--   0        0        0     2255 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
--rw-r--r--   0        0        0     4092 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
--rw-r--r--   0        0        0     3007 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters.py
--rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters_standard.py
--rw-r--r--   0        0        0     2250 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_raw_detection.py
--rw-r--r--   0        0        0     2366 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
--rw-r--r--   0        0        0     2412 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
--rw-r--r--   0        0        0     2106 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
--rw-r--r--   0        0        0     1839 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/permission.py
--rw-r--r--   0        0        0     2491 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_file.py
--rw-r--r--   0        0        0     2537 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_info_response.py
--rw-r--r--   0        0        0     2666 2024-04-17 10:43:43.070401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/pretrained_model_tensor.py
--rw-r--r--   0        0        0     2403 2024-04-17 10:43:43.074401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_request.py
--rw-r--r--   0        0        0     3734 2024-04-17 10:43:43.074401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response.py
--rw-r--r--   0        0        0     3467 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
--rw-r--r--   0        0        0     2955 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info.py
--rw-r--r--   0        0        0     3117 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory.py
--rw-r--r--   0        0        0     1918 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_eon.py
--rw-r--r--   0        0        0     2065 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_tflite.py
--rw-r--r--   0        0        0     4335 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table.py
--rw-r--r--   0        0        0     2780 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu.py
--rw-r--r--   0        0        0     3042 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu_memory.py
--rw-r--r--   0        0        0     2250 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mpu.py
--rw-r--r--   0        0        0     2201 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_request.py
--rw-r--r--   0        0        0     3292 2024-04-17 10:43:43.078401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_response.py
--rw-r--r--   0        0        0     7873 2024-04-17 10:43:43.082401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project.py
--rw-r--r--   0        0        0     4545 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator.py
--rw-r--r--   0        0        0     1895 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator_all_of.py
--rw-r--r--   0        0        0     2416 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response.py
--rw-r--r--   0        0        0     2116 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
--rw-r--r--   0        0        0     2281 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response.py
--rw-r--r--   0        0        0     1964 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response_all_of.py
--rw-r--r--   0        0        0     2235 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_summary.py
--rw-r--r--   0        0        0     6854 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target.py
--rw-r--r--   0        0        0     2706 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target_all_of.py
--rw-r--r--   0        0        0     2780 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response.py
--rw-r--r--   0        0        0     2473 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
--rw-r--r--   0        0        0     1943 2024-04-17 10:43:43.086401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_dismiss_notification_request.py
--rw-r--r--   0        0        0     2680 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response.py
--rw-r--r--   0        0        0     2373 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response_all_of.py
--rw-r--r--   0        0        0    14783 2024-04-17 10:43:43.090401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response.py
--rw-r--r--   0        0        0    14516 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of.py
--rw-r--r--   0        0        0     4174 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
--rw-r--r--   0        0        0     2723 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
--rw-r--r--   0        0        0     2997 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
--rw-r--r--   0        0        0     3200 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
--rw-r--r--   0        0        0     2339 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_experiments.py
--rw-r--r--   0        0        0     2285 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_impulse.py
--rw-r--r--   0        0        0     2726 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_performance.py
--rw-r--r--   0        0        0     1977 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_readme.py
--rw-r--r--   0        0        0     2225 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
--rw-r--r--   0        0        0     2735 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_urls.py
--rw-r--r--   0        0        0     2478 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response.py
--rw-r--r--   0        0        0     2172 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response_all_of.py
--rw-r--r--   0        0        0     3554 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_private_data.py
--rw-r--r--   0        0        0     4127 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data.py
--rw-r--r--   0        0        0     1928 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data_readme.py
--rw-r--r--   0        0        0     2404 2024-04-17 10:43:43.094401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_sample_metadata.py
--rw-r--r--   0        0        0      576 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_tier_enum.py
--rw-r--r--   0        0        0     2804 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response.py
--rw-r--r--   0        0        0     2487 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
--rw-r--r--   0        0        0     2253 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
--rw-r--r--   0        0        0      606 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_type.py
--rw-r--r--   0        0        0     2316 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_version_request.py
--rw-r--r--   0        0        0      504 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_visibility.py
--rw-r--r--   0        0        0     4991 2024-04-17 10:43:43.098401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/public_organization_transformation_block.py
--rw-r--r--   0        0        0     2664 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_data.py
--rw-r--r--   0        0        0     3440 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_payload.py
--rw-r--r--   0        0        0     2537 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rebalance_dataset_response.py
--rw-r--r--   0        0        0     1984 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_collaborator_request.py
--rw-r--r--   0        0        0     1805 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_member_request.py
--rw-r--r--   0        0        0     1867 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_device_request.py
--rw-r--r--   0        0        0     2081 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_portal_file_request.py
--rw-r--r--   0        0        0     1867 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_sample_request.py
--rw-r--r--   0        0        0     2028 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_email_verification_request.py
--rw-r--r--   0        0        0     1873 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_reset_password_request.py
--rw-r--r--   0        0        0     2031 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/reset_password_request.py
--rw-r--r--   0        0        0     1896 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/resource_range.py
--rw-r--r--   0        0        0     1985 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_from_public_request.py
--rw-r--r--   0        0        0     2265 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_request.py
--rw-r--r--   0        0        0     2421 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_auto_labeler_request.py
--rw-r--r--   0        0        0     2669 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response.py
--rw-r--r--   0        0        0     2352 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
--rw-r--r--   0        0        0    11134 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample.py
--rw-r--r--   0        0        0     2443 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_bounding_boxes_request.py
--rw-r--r--   0        0        0     2000 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_metadata.py
--rw-r--r--   0        0        0     2517 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
--rw-r--r--   0        0        0     2071 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
--rw-r--r--   0        0        0     2341 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
--rw-r--r--   0        0        0     2024 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
--rw-r--r--   0        0        0     2756 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_pretrained_model_request.py
--rw-r--r--   0        0        0     3327 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response.py
--rw-r--r--   0        0        0     3003 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of.py
--rw-r--r--   0        0        0     2240 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_latency.py
--rw-r--r--   0        0        0     1914 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_ram.py
--rw-r--r--   0        0        0     2405 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request.py
--rw-r--r--   0        0        0     2055 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request_segments_inner.py
--rw-r--r--   0        0        0     3346 2024-04-17 10:43:43.102401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/send_user_feedback_request.py
--rw-r--r--   0        0        0     1981 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/sensor.py
--rw-r--r--   0        0        0     2142 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_anomaly_parameter_request.py
--rw-r--r--   0        0        0     9364 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_keras_parameter_request.py
--rw-r--r--   0        0        0     1893 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_datasets_request.py
--rw-r--r--   0        0        0     1905 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_role_request.py
--rw-r--r--   0        0        0     2219 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request.py
--rw-r--r--   0        0        0     2254 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request_all_of.py
--rw-r--r--   0        0        0     1923 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_organization_data_dataset_request.py
--rw-r--r--   0        0        0     1974 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_compute_time_request.py
--rw-r--r--   0        0        0     2011 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_dsp_file_size_request.py
--rw-r--r--   0        0        0     1919 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_metadata_request.py
--rw-r--r--   0        0        0     2531 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_structured_labels_request.py
--rw-r--r--   0        0        0     1915 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_syntiant_posterior_request.py
--rw-r--r--   0        0        0     2140 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_user_password_request.py
--rw-r--r--   0        0        0     2536 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response.py
--rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of.py
--rw-r--r--   0        0        0     2059 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of_token.py
--rw-r--r--   0        0        0     1971 2024-04-17 10:43:43.106401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/split_sample_in_frames_request.py
--rw-r--r--   0        0        0     2110 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/staff_info.py
--rw-r--r--   0        0        0     2292 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response.py
--rw-r--r--   0        0        0     1975 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
--rw-r--r--   0        0        0     2178 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
--rw-r--r--   0        0        0     5388 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_enterprise_trial_request.py
--rw-r--r--   0        0        0     2226 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response.py
--rw-r--r--   0        0        0     1909 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response_all_of.py
--rw-r--r--   0        0        0     2883 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_performance_calibration_request.py
--rw-r--r--   0        0        0     2838 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_request.py
--rw-r--r--   0        0        0     2189 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response.py
--rw-r--r--   0        0        0     1892 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response_all_of.py
--rw-r--r--   0        0        0     2795 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_training_request_anomaly.py
--rw-r--r--   0        0        0     1926 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/stop_device_debug_stream_request.py
--rw-r--r--   0        0        0     1967 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/store_segment_length_request.py
--rw-r--r--   0        0        0     3394 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_classify_result.py
--rw-r--r--   0        0        0     2270 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_label.py
--rw-r--r--   0        0        0     4399 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints.py
--rw-r--r--   0        0        0     2923 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints_device.py
--rw-r--r--   0        0        0     2347 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_memory.py
--rw-r--r--   0        0        0     3751 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_processor.py
--rw-r--r--   0        0        0     2433 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_request.py
--rw-r--r--   0        0        0     3074 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response.py
--rw-r--r--   0        0        0     2784 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
--rw-r--r--   0        0        0     3251 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme.py
--rw-r--r--   0        0        0     2239 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_colors.py
--rw-r--r--   0        0        0     2764 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_favicon.py
--rw-r--r--   0        0        0     2721 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_logos.py
--rw-r--r--   0        0        0     2245 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/third_party_auth.py
--rw-r--r--   0        0        0     1921 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/time_series_data_point.py
--rw-r--r--   0        0        0     2031 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_request.py
--rw-r--r--   0        0        0     2736 2024-04-17 10:43:43.110401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response.py
--rw-r--r--   0        0        0     2436 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response_all_of.py
--rw-r--r--   0        0        0     5380 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_learning_model.py
--rw-r--r--   0        0        0     2012 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_ownership_organization_request.py
--rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_block_additional_mount_point.py
--rw-r--r--   0        0        0      548 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_operates_on_enum.py
--rw-r--r--   0        0        0      588 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_status_enum.py
--rw-r--r--   0        0        0     2578 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_create_trial_impulse.py
--rw-r--r--   0        0        0     2462 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_run.py
--rw-r--r--   0        0        0     2570 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_space_impulse.py
--rw-r--r--   0        0        0     4991 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial.py
--rw-r--r--   0        0        0     2739 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_blocks_inner.py
--rw-r--r--   0        0        0     1935 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
--rw-r--r--   0        0        0     2211 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_impulse.py
--rw-r--r--   0        0        0     2028 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_job_request.py
--rw-r--r--   0        0        0     2281 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_add_collaborator_request.py
--rw-r--r--   0        0        0     2882 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_bucket_request.py
--rw-r--r--   0        0        0     2828 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_empty_project_request.py
--rw-r--r--   0        0        0     2428 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_project_request.py
--rw-r--r--   0        0        0     2913 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
--rw-r--r--   0        0        0     4154 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_request.py
--rw-r--r--   0        0        0     2158 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_item_request.py
--rw-r--r--   0        0        0     2977 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request.py
--rw-r--r--   0        0        0     2518 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
--rw-r--r--   0        0        0     2881 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dsp_block_request.py
--rw-r--r--   0        0        0     2724 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response.py
--rw-r--r--   0        0        0     2445 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response_all_of.py
--rw-r--r--   0        0        0     2766 2024-04-17 10:43:43.114401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_request.py
--rw-r--r--   0        0        0     5211 2024-04-17 10:43:43.118401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
--rw-r--r--   0        0        0     6072 2024-04-17 10:43:43.122401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transformation_block_request.py
--rw-r--r--   0        0        0    11806 2024-04-17 10:43:43.122401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_request.py
--rw-r--r--   0        0        0     1877 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_tags_request.py
--rw-r--r--   0        0        0     2259 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_colors_request.py
--rw-r--r--   0        0        0     2895 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_logos_request.py
--rw-r--r--   0        0        0     2205 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_third_party_auth_request.py
--rw-r--r--   0        0        0     1865 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_tuner_run_request.py
--rw-r--r--   0        0        0     2375 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_user_request.py
--rw-r--r--   0        0        0     1886 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_version_request.py
--rw-r--r--   0        0        0     2393 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
--rw-r--r--   0        0        0     2237 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
--rw-r--r--   0        0        0     2125 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
--rw-r--r--   0        0        0     2155 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
--rw-r--r--   0        0        0     2059 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_request.py
--rw-r--r--   0        0        0     2168 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response.py
--rw-r--r--   0        0        0     1882 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response_all_of.py
--rw-r--r--   0        0        0     2199 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_readme_image_response.py
--rw-r--r--   0        0        0     2185 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response.py
--rw-r--r--   0        0        0     1872 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response_all_of.py
--rw-r--r--   0        0        0     4330 2024-04-17 10:43:43.126401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user.py
--rw-r--r--   0        0        0     1991 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_by_third_party_activation_request.py
--rw-r--r--   0        0        0     1956 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
--rw-r--r--   0        0        0     1922 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_dismiss_notification_request.py
--rw-r--r--   0        0        0     2192 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_experiment.py
--rw-r--r--   0        0        0     2425 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
--rw-r--r--   0        0        0     2119 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
--rw-r--r--   0        0        0     4606 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_organization.py
--rw-r--r--   0        0        0     2144 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
--rw-r--r--   0        0        0     2480 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
--rw-r--r--   0        0        0     2191 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
--rw-r--r--   0        0        0      543 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_tier_enum.py
--rw-r--r--   0        0        0     1844 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_request.py
--rw-r--r--   0        0        0     2604 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response.py
--rw-r--r--   0        0        0     2307 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
--rw-r--r--   0        0        0     3049 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
--rw-r--r--   0        0        0     2633 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response.py
--rw-r--r--   0        0        0     2354 2024-04-17 10:43:43.130401 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response_all_of.py
--rw-r--r--   0        0        0     2708 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_request.py
--rw-r--r--   0        0        0     3432 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response.py
--rw-r--r--   0        0        0     3155 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
--rw-r--r--   0        0        0     2187 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
--rw-r--r--   0        0        0     1961 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
--rw-r--r--   0        0        0     1937 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_reset_password_request.py
--rw-r--r--   0        0        0     8565 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel.py
--rw-r--r--   0        0        0     2534 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
--rw-r--r--   0        0        0     2085 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
--rw-r--r--   0        0        0     2120 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
--rw-r--r--   0        0        0     2885 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response.py
--rw-r--r--   0        0        0     2585 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of.py
--rw-r--r--   0        0        0     2848 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
--rw-r--r--   0        0        0    12674 2024-04-17 10:43:43.134400 edgeimpulse_api-1.49.9/edgeimpulse_api/rest.py
--rw-r--r--   0        0        0     1019 2024-04-17 10:44:15.302117 edgeimpulse_api-1.49.9/pyproject.toml
--rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.49.9/PKG-INFO
+-rw-r--r--   0        0        0      377 2024-05-21 19:37:59.035578 edgeimpulse_api-1.50.0/README.md
+-rw-r--r--   0        0        0    90082 2024-05-21 19:38:53.678664 edgeimpulse_api-1.50.0/edgeimpulse_api/__init__.py
+-rw-r--r--   0        0        0     2172 2024-05-21 19:37:59.035578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/__init__.py
+-rw-r--r--   0        0        0   385743 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/admin_api.py
+-rw-r--r--   0        0        0    11231 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/auth_api.py
+-rw-r--r--   0        0        0     6235 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/cdn_api.py
+-rw-r--r--   0        0        0    67927 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/classify_api.py
+-rw-r--r--   0        0        0    72480 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/deployment_api.py
+-rw-r--r--   0        0        0    80789 2024-05-21 19:37:59.039578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/devices_api.py
+-rw-r--r--   0        0        0   139045 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/dsp_api.py
+-rw-r--r--   0        0        0    19442 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/email_verification_api.py
+-rw-r--r--   0        0        0     6435 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/export_api.py
+-rw-r--r--   0        0        0     5996 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/feature_flags_api.py
+-rw-r--r--   0        0        0    11921 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/health_api.py
+-rw-r--r--   0        0        0    49621 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/impulse_api.py
+-rw-r--r--   0        0        0   239795 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/jobs_api.py
+-rw-r--r--   0        0        0   154112 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/learn_api.py
+-rw-r--r--   0        0        0     6483 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/login_api.py
+-rw-r--r--   0        0        0    17897 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/metrics_api.py
+-rw-r--r--   0        0        0    85275 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/optimization_api.py
+-rw-r--r--   0        0        0   197840 2024-05-21 19:37:59.043578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_blocks_api.py
+-rw-r--r--   0        0        0    92715 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_create_project_api.py
+-rw-r--r--   0        0        0   331750 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_data_api.py
+-rw-r--r--   0        0        0    80882 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_data_campaigns_api.py
+-rw-r--r--   0        0        0    58661 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_jobs_api.py
+-rw-r--r--   0        0        0    53291 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_pipelines_api.py
+-rw-r--r--   0        0        0    45490 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_portals_api.py
+-rw-r--r--   0        0        0   505317 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/organizations_api.py
+-rw-r--r--   0        0        0    60377 2024-05-21 19:37:59.047578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/performance_calibration_api.py
+-rw-r--r--   0        0        0   276748 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/projects_api.py
+-rw-r--r--   0        0        0   414581 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/raw_data_api.py
+-rw-r--r--   0        0        0    35671 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/themes_api.py
+-rw-r--r--   0        0        0    43486 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/third_party_auth_api.py
+-rw-r--r--   0        0        0    45692 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/upload_portal_api.py
+-rw-r--r--   0        0        0   270581 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/user_api.py
+-rw-r--r--   0        0        0    42135 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api/whitelabels_api.py
+-rw-r--r--   0        0        0    29331 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/api_client.py
+-rw-r--r--   0        0        0    15659 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/configuration.py
+-rw-r--r--   0        0        0     5113 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/exceptions.py
+-rw-r--r--   0        0        0    87457 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/__init__.py
+-rw-r--r--   0        0        0     2897 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py
+-rw-r--r--   0        0        0     1982 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py
+-rw-r--r--   0        0        0     2052 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_api_key_request.py
+-rw-r--r--   0        0        0     1963 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_collaborator_request.py
+-rw-r--r--   0        0        0     2223 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_hmac_key_request.py
+-rw-r--r--   0        0        0     2299 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_member_request.py
+-rw-r--r--   0        0        0     2418 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2122 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2806 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_bucket_request.py
+-rw-r--r--   0        0        0     2794 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     2469 2024-05-21 19:37:59.051578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2152 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     4230 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2359 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2042 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py
+-rw-r--r--   0        0        0     2269 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2816 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2248 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2054 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_request.py
+-rw-r--r--   0        0        0     2266 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_response.py
+-rw-r--r--   0        0        0     1949 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py
+-rw-r--r--   0        0        0     4940 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     2339 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     6169 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_request.py
+-rw-r--r--   0        0        0     2325 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2001 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2659 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_project_api_key_request.py
+-rw-r--r--   0        0        0     2370 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     1940 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py
+-rw-r--r--   0        0        0     1961 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py
+-rw-r--r--   0        0        0     2661 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_api_key_request.py
+-rw-r--r--   0        0        0     2542 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_user_request.py
+-rw-r--r--   0        0        0     2246 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py
+-rw-r--r--   0        0        0     2344 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_api_key_request.py
+-rw-r--r--   0        0        0     2044 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py
+-rw-r--r--   0        0        0     2146 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_user_request.py
+-rw-r--r--   0        0        0     2097 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_user_request.py
+-rw-r--r--   0        0        0     6067 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_organization.py
+-rw-r--r--   0        0        0     2396 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_organization_all_of.py
+-rw-r--r--   0        0        0     3259 2024-05-21 19:37:59.071578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_project.py
+-rw-r--r--   0        0        0     7529 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_user.py
+-rw-r--r--   0        0        0     5318 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_user_all_of.py
+-rw-r--r--   0        0        0     2386 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_organization_data_export_request.py
+-rw-r--r--   0        0        0     2262 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_organization_request.py
+-rw-r--r--   0        0        0     2718 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_project_request.py
+-rw-r--r--   0        0        0     1905 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_enable_feature_request.py
+-rw-r--r--   0        0        0     2546 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migration_response.py
+-rw-r--r--   0        0        0     2222 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py
+-rw-r--r--   0        0        0     2735 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migrations_response.py
+-rw-r--r--   0        0        0     2428 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py
+-rw-r--r--   0        0        0     2318 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py
+-rw-r--r--   0        0        0     2022 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py
+-rw-r--r--   0        0        0     2217 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_metrics_response.py
+-rw-r--r--   0        0        0     1910 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3148 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py
+-rw-r--r--   0        0        0     2647 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2323 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py
+-rw-r--r--   0        0        0     3029 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2729 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     3046 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response.py
+-rw-r--r--   0        0        0     2746 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py
+-rw-r--r--   0        0        0     3409 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py
+-rw-r--r--   0        0        0     2243 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py
+-rw-r--r--   0        0        0     1947 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py
+-rw-r--r--   0        0        0     2914 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response.py
+-rw-r--r--   0        0        0     2614 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py
+-rw-r--r--   0        0        0     2096 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py
+-rw-r--r--   0        0        0     2208 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_ids_response.py
+-rw-r--r--   0        0        0     1901 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py
+-rw-r--r--   0        0        0     2245 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_metrics_response.py
+-rw-r--r--   0        0        0     2452 2024-05-21 19:37:59.075578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_response.py
+-rw-r--r--   0        0        0     2128 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_response_all_of.py
+-rw-r--r--   0        0        0     2507 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_trial_response.py
+-rw-r--r--   0        0        0     2183 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py
+-rw-r--r--   0        0        0     2807 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response.py
+-rw-r--r--   0        0        0     2500 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response_all_of.py
+-rw-r--r--   0        0        0     2878 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py
+-rw-r--r--   0        0        0     2445 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_list_projects.py
+-rw-r--r--   0        0        0     2836 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_list_projects_response.py
+-rw-r--r--   0        0        0     4245 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_organization_info_response.py
+-rw-r--r--   0        0        0     3084 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py
+-rw-r--r--   0        0        0     2158 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py
+-rw-r--r--   0        0        0     2397 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_organization_data_export_request.py
+-rw-r--r--   0        0        0     3936 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_organization_request.py
+-rw-r--r--   0        0        0     2015 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_permissions_request.py
+-rw-r--r--   0        0        0     2830 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_request.py
+-rw-r--r--   0        0        0     2532 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_trial_request.py
+-rw-r--r--   0        0        0     2525 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/akida_edge_learning_config.py
+-rw-r--r--   0        0        0      512 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_capacity.py
+-rw-r--r--   0        0        0     2512 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_gmm_metadata.py
+-rw-r--r--   0        0        0     2212 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py
+-rw-r--r--   0        0        0     5499 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata.py
+-rw-r--r--   0        0        0     5221 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py
+-rw-r--r--   0        0        0     2151 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py
+-rw-r--r--   0        0        0     4079 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response.py
+-rw-r--r--   0        0        0     3812 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response_all_of.py
+-rw-r--r--   0        0        0     2044 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py
+-rw-r--r--   0        0        0     3188 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_result.py
+-rw-r--r--   0        0        0     3029 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response.py
+-rw-r--r--   0        0        0     2729 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2375 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     3358 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/application_budget.py
+-rw-r--r--   0        0        0      506 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/augmentation_policy_image_enum.py
+-rw-r--r--   0        0        0     3635 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py
+-rw-r--r--   0        0        0     1895 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/autotune_dsp_request.py
+-rw-r--r--   0        0        0      499 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/billing_cycle.py
+-rw-r--r--   0        0        0      505 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/block_display_category.py
+-rw-r--r--   0        0        0      604 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/block_type.py
+-rw-r--r--   0        0        0     2044 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/bounding_box.py
+-rw-r--r--   0        0        0     2151 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/bounding_box_with_score.py
+-rw-r--r--   0        0        0     2197 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/build_on_device_model_request.py
+-rw-r--r--   0        0        0     2433 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/build_organization_on_device_model_request.py
+-rw-r--r--   0        0        0     2459 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py
+-rw-r--r--   0        0        0     2041 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/change_password_request.py
+-rw-r--r--   0        0        0     4041 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response.py
+-rw-r--r--   0        0        0     3741 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of.py
+-rw-r--r--   0        0        0     3769 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py
+-rw-r--r--   0        0        0     2055 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py
+-rw-r--r--   0        0        0     3255 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_page.py
+-rw-r--r--   0        0        0     2948 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_page_all_of.py
+-rw-r--r--   0        0        0     4064 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_for_variants200_response.py
+-rw-r--r--   0        0        0     4026 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response.py
+-rw-r--r--   0        0        0     3759 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_all_of.py
+-rw-r--r--   0        0        0     6252 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_classification.py
+-rw-r--r--   0        0        0     2755 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_classification_details.py
+-rw-r--r--   0        0        0     3984 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_multiple_variants.py
+-rw-r--r--   0        0        0     3706 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_multiple_variants_all_of.py
+-rw-r--r--   0        0        0     2768 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_variant_results.py
+-rw-r--r--   0        0        0     3816 2024-05-21 19:37:59.079578 edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_v2200_response.py
+-rw-r--r--   0        0        0     3004 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/convert_user_request.py
+-rw-r--r--   0        0        0     3495 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_data.py
+-rw-r--r--   0        0        0     3114 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue.py
+-rw-r--r--   0        0        0     3241 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py
+-rw-r--r--   0        0        0     2484 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py
+-rw-r--r--   0        0        0     2183 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/count_samples_response.py
+-rw-r--r--   0        0        0     1859 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/count_samples_response_all_of.py
+-rw-r--r--   0        0        0     2255 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_block_version_response.py
+-rw-r--r--   0        0        0     1938 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_block_version_response_all_of.py
+-rw-r--r--   0        0        0     2404 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_developer_profile_response.py
+-rw-r--r--   0        0        0     2125 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py
+-rw-r--r--   0        0        0     2387 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_device_request.py
+-rw-r--r--   0        0        0     2850 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_response.py
+-rw-r--r--   0        0        0     2319 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py
+-rw-r--r--   0        0        0     6569 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_user_request.py
+-rw-r--r--   0        0        0     4092 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py
+-rw-r--r--   0        0        0     2491 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_evaluation_user_response.py
+-rw-r--r--   0        0        0     2185 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py
+-rw-r--r--   0        0        0     2600 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_request.py
+-rw-r--r--   0        0        0     2830 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_response.py
+-rw-r--r--   0        0        0     2551 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     1990 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_request.py
+-rw-r--r--   0        0        0     2454 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_response.py
+-rw-r--r--   0        0        0     2148 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_response_all_of.py
+-rw-r--r--   0        0        0     2155 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_usage_report_body.py
+-rw-r--r--   0        0        0     2185 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_pipeline_response.py
+-rw-r--r--   0        0        0     2504 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_request.py
+-rw-r--r--   0        0        0     2378 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_response.py
+-rw-r--r--   0        0        0     2072 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_response_all_of.py
+-rw-r--r--   0        0        0     2276 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_request.py
+-rw-r--r--   0        0        0     2414 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_response.py
+-rw-r--r--   0        0        0     2135 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py
+-rw-r--r--   0        0        0     2413 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_request.py
+-rw-r--r--   0        0        0     2450 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_response.py
+-rw-r--r--   0        0        0     2144 2024-05-21 19:37:59.083577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     4446 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_request.py
+-rw-r--r--   0        0        0     2393 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_response.py
+-rw-r--r--   0        0        0     2114 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_response_all_of.py
+-rw-r--r--   0        0        0     2919 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_request.py
+-rw-r--r--   0        0        0     2672 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_response.py
+-rw-r--r--   0        0        0     2393 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py
+-rw-r--r--   0        0        0     4384 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_request.py
+-rw-r--r--   0        0        0     2438 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_response.py
+-rw-r--r--   0        0        0     2121 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2094 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/created_updated_by_user.py
+-rw-r--r--   0        0        0     2051 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_request.py
+-rw-r--r--   0        0        0     2248 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_response.py
+-rw-r--r--   0        0        0     1943 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_response_all_of.py
+-rw-r--r--   0        0        0     2368 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cross_validation_data.py
+-rw-r--r--   0        0        0     3412 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/cross_validation_data_scores_inner.py
+-rw-r--r--   0        0        0     4054 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign.py
+-rw-r--r--   0        0        0     2989 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_dashboard.py
+-rw-r--r--   0        0        0     2786 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph.py
+-rw-r--r--   0        0        0     3352 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py
+-rw-r--r--   0        0        0     2047 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py
+-rw-r--r--   0        0        0     1934 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_link.py
+-rw-r--r--   0        0        0     1957 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_query.py
+-rw-r--r--   0        0        0     3292 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_predictions_response.py
+-rw-r--r--   0        0        0     3003 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py
+-rw-r--r--   0        0        0     2838 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_settings.py
+-rw-r--r--   0        0        0     2149 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dataset_ratio_data.py
+-rw-r--r--   0        0        0     2111 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py
+-rw-r--r--   0        0        0     1898 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/delete_portal_file_request.py
+-rw-r--r--   0        0        0     2379 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/delete_user_request.py
+-rw-r--r--   0        0        0     2230 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dependency_data.py
+-rw-r--r--   0        0        0     2280 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py
+-rw-r--r--   0        0        0     2408 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py
+-rw-r--r--   0        0        0     2155 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py
+-rw-r--r--   0        0        0     2484 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py
+-rw-r--r--   0        0        0     2344 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py
+-rw-r--r--   0        0        0     2780 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py
+-rw-r--r--   0        0        0     2200 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py
+-rw-r--r--   0        0        0     4397 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request.py
+-rw-r--r--   0        0        0     2833 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py
+-rw-r--r--   0        0        0     8503 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py
+-rw-r--r--   0        0        0     8065 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py
+-rw-r--r--   0        0        0     5950 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target.py
+-rw-r--r--   0        0        0     1926 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target_badge.py
+-rw-r--r--   0        0        0      755 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target_engine.py
+-rw-r--r--   0        0        0     2702 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_targets_response.py
+-rw-r--r--   0        0        0     2395 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     2248 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_created_response.py
+-rw-r--r--   0        0        0     2032 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_request.py
+-rw-r--r--   0        0        0     2134 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_request_update.py
+-rw-r--r--   0        0        0     2113 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_response.py
+-rw-r--r--   0        0        0     2864 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_boards_response.py
+-rw-r--r--   0        0        0     2564 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_boards_response_all_of.py
+-rw-r--r--   0        0        0     2030 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_keys.py
+-rw-r--r--   0        0        0     2400 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_keys_response.py
+-rw-r--r--   0        0        0     4816 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device.py
+-rw-r--r--   0        0        0      516 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_debug_stream_type.py
+-rw-r--r--   0        0        0     2811 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_inference_info.py
+-rw-r--r--   0        0        0     2199 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_name_response.py
+-rw-r--r--   0        0        0     1920 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_name_response_all_of.py
+-rw-r--r--   0        0        0     2231 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_sensors_inner.py
+-rw-r--r--   0        0        0     2094 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/download.py
+-rw-r--r--   0        0        0     1912 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_request.py
+-rw-r--r--   0        0        0     2260 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_response.py
+-rw-r--r--   0        0        0     1954 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_response_all_of.py
+-rw-r--r--   0        0        0     2724 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results.py
+-rw-r--r--   0        0        0     2417 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py
+-rw-r--r--   0        0        0     1968 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py
+-rw-r--r--   0        0        0     3660 2024-05-21 19:37:59.087577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_block.py
+-rw-r--r--   0        0        0     1834 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_request.py
+-rw-r--r--   0        0        0     3092 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_response.py
+-rw-r--r--   0        0        0     2813 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_response_all_of.py
+-rw-r--r--   0        0        0     3016 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response.py
+-rw-r--r--   0        0        0     2728 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py
+-rw-r--r--   0        0        0     2058 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py
+-rw-r--r--   0        0        0     2572 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py
+-rw-r--r--   0        0        0     2216 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_labels_response.py
+-rw-r--r--   0        0        0     1920 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py
+-rw-r--r--   0        0        0     2294 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group.py
+-rw-r--r--   0        0        0     4216 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item.py
+-rw-r--r--   0        0        0     2190 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py
+-rw-r--r--   0        0        0     2195 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item_show_if.py
+-rw-r--r--   0        0        0     4848 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info.py
+-rw-r--r--   0        0        0     2376 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info_features.py
+-rw-r--r--   0        0        0     1885 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info_performance.py
+-rw-r--r--   0        0        0     5462 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata.py
+-rw-r--r--   0        0        0     2025 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py
+-rw-r--r--   0        0        0     2566 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_output_config.py
+-rw-r--r--   0        0        0     2531 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py
+-rw-r--r--   0        0        0     5820 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_response.py
+-rw-r--r--   0        0        0     1963 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_named_axis.py
+-rw-r--r--   0        0        0     3019 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py
+-rw-r--r--   0        0        0     2729 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2278 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py
+-rw-r--r--   0        0        0     4639 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_graph.py
+-rw-r--r--   0        0        0     1899 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py
+-rw-r--r--   0        0        0     2677 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_with_features.py
+-rw-r--r--   0        0        0     2151 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_without_features.py
+-rw-r--r--   0        0        0     2030 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py
+-rw-r--r--   0        0        0     3697 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response.py
+-rw-r--r--   0        0        0     3418 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_all_of.py
+-rw-r--r--   0        0        0     1969 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py
+-rw-r--r--   0        0        0     4579 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_with_sample.py
+-rw-r--r--   0        0        0     4312 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py
+-rw-r--r--   0        0        0     3342 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response.py
+-rw-r--r--   0        0        0     3042 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py
+-rw-r--r--   0        0        0     2748 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2213 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     3353 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response.py
+-rw-r--r--   0        0        0     3053 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py
+-rw-r--r--   0        0        0     2773 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py
+-rw-r--r--   0        0        0     2205 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py
+-rw-r--r--   0        0        0     1893 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/edit_sample_label_request.py
+-rw-r--r--   0        0        0     4235 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/enterprise_trial.py
+-rw-r--r--   0        0        0     2960 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py
+-rw-r--r--   0        0        0     2885 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/entitlement_limits.py
+-rw-r--r--   0        0        0     2367 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/entity_created_response.py
+-rw-r--r--   0        0        0     2077 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/entity_created_response_all_of.py
+-rw-r--r--   0        0        0     2656 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_job_response.py
+-rw-r--r--   0        0        0     2349 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_job_response_all_of.py
+-rw-r--r--   0        0        0     2099 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_result_value.py
+-rw-r--r--   0        0        0     2366 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_block_response.py
+-rw-r--r--   0        0        0     2060 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_block_response_all_of.py
+-rw-r--r--   0        0        0     2511 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_get_url_response.py
+-rw-r--r--   0        0        0     2244 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_get_url_response_all_of.py
+-rw-r--r--   0        0        0     2116 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_keras_block_data_request.py
+-rw-r--r--   0        0        0     2373 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_original_data_request.py
+-rw-r--r--   0        0        0     2021 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_wav_data_request.py
+-rw-r--r--   0        0        0      586 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/feature.py
+-rw-r--r--   0        0        0     2206 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_request.py
+-rw-r--r--   0        0        0     2804 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response.py
+-rw-r--r--   0        0        0     2497 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py
+-rw-r--r--   0        0        0     2090 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py
+-rw-r--r--   0        0        0     2665 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response.py
+-rw-r--r--   0        0        0     2358 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response_all_of.py
+-rw-r--r--   0        0        0     2322 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response_all_of_users.py
+-rw-r--r--   0        0        0     2507 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/generate_features_request.py
+-rw-r--r--   0        0        0     2083 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/generic_api_response.py
+-rw-r--r--   0        0        0     2764 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response.py
+-rw-r--r--   0        0        0     2457 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py
+-rw-r--r--   0        0        0     2156 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py
+-rw-r--r--   0        0        0     2698 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_third_party_auth_response.py
+-rw-r--r--   0        0        0     2391 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     2713 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_whitelabels_response.py
+-rw-r--r--   0        0        0     2406 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py
+-rw-r--r--   0        0        0     3527 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response.py
+-rw-r--r--   0        0        0     3260 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of.py
+-rw-r--r--   0        0        0     2588 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py
+-rw-r--r--   0        0        0     1954 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py
+-rw-r--r--   0        0        0     2345 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py
+-rw-r--r--   0        0        0     2078 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py
+-rw-r--r--   0        0        0     3400 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_features_response.py
+-rw-r--r--   0        0        0     3122 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0     3752 2024-05-21 19:37:59.091577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_settings_response.py
+-rw-r--r--   0        0        0     2402 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py
+-rw-r--r--   0        0        0     2349 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_deployment_response.py
+-rw-r--r--   0        0        0     2071 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_deployment_response_all_of.py
+-rw-r--r--   0        0        0     2434 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_device_response.py
+-rw-r--r--   0        0        0     2137 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_device_response_all_of.py
+-rw-r--r--   0        0        0     2752 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response.py
+-rw-r--r--   0        0        0     2455 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py
+-rw-r--r--   0        0        0     4251 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py
+-rw-r--r--   0        0        0     2859 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2456 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_code_response.py
+-rw-r--r--   0        0        0     2177 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_code_response_all_of.py
+-rw-r--r--   0        0        0     2350 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_status_response.py
+-rw-r--r--   0        0        0     2045 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_status_response_all_of.py
+-rw-r--r--   0        0        0     2788 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response.py
+-rw-r--r--   0        0        0     2488 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response_all_of.py
+-rw-r--r--   0        0        0     2118 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py
+-rw-r--r--   0        0        0     3930 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_blocks_response.py
+-rw-r--r--   0        0        0     3630 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2429 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_records_request.py
+-rw-r--r--   0        0        0     2007 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_records_request_range.py
+-rw-r--r--   0        0        0     2454 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_response.py
+-rw-r--r--   0        0        0     2157 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_response_all_of.py
+-rw-r--r--   0        0        0     2374 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_job_response.py
+-rw-r--r--   0        0        0     2077 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_job_response_all_of.py
+-rw-r--r--   0        0        0     3070 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_request.py
+-rw-r--r--   0        0        0     2431 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_response.py
+-rw-r--r--   0        0        0     2152 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_response_all_of.py
+-rw-r--r--   0        0        0     2580 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response.py
+-rw-r--r--   0        0        0     2256 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response_all_of.py
+-rw-r--r--   0        0        0     3358 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py
+-rw-r--r--   0        0        0     3578 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response.py
+-rw-r--r--   0        0        0     3300 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py
+-rw-r--r--   0        0        0     2869 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py
+-rw-r--r--   0        0        0     2887 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_model_variants_response.py
+-rw-r--r--   0        0        0     2597 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_model_variants_response_all_of.py
+-rw-r--r--   0        0        0     2572 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_notes_response.py
+-rw-r--r--   0        0        0     2265 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_notes_response_all_of.py
+-rw-r--r--   0        0        0     2556 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_bucket_response.py
+-rw-r--r--   0        0        0     2232 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2701 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py
+-rw-r--r--   0        0        0     2377 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py
+-rw-r--r--   0        0        0     2890 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py
+-rw-r--r--   0        0        0     2583 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py
+-rw-r--r--   0        0        0     3158 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_response.py
+-rw-r--r--   0        0        0     2939 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py
+-rw-r--r--   0        0        0     2632 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py
+-rw-r--r--   0        0        0     2601 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_export_response.py
+-rw-r--r--   0        0        0     2277 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_export_response_all_of.py
+-rw-r--r--   0        0        0     2982 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_exports_response.py
+-rw-r--r--   0        0        0     2682 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py
+-rw-r--r--   0        0        0     2561 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_response.py
+-rw-r--r--   0        0        0     2237 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py
+-rw-r--r--   0        0        0     3411 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py
+-rw-r--r--   0        0        0     3111 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py
+-rw-r--r--   0        0        0     3532 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py
+-rw-r--r--   0        0        0     2576 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dataset_response.py
+-rw-r--r--   0        0        0     2252 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py
+-rw-r--r--   0        0        0     2690 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_deploy_block_response.py
+-rw-r--r--   0        0        0     2373 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py
+-rw-r--r--   0        0        0     2627 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dsp_block_response.py
+-rw-r--r--   0        0        0     2310 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py
+-rw-r--r--   0        0        0     2603 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2279 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     3670 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_portal_response.py
+-rw-r--r--   0        0        0     3391 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2323 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py
+-rw-r--r--   0        0        0     2906 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py
+-rw-r--r--   0        0        0     2589 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transformation_block_response.py
+-rw-r--r--   0        0        0     2541 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py
+-rw-r--r--   0        0        0     2612 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_usage_report_response.py
+-rw-r--r--   0        0        0     2905 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py
+-rw-r--r--   0        0        0     2598 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py
+-rw-r--r--   0        0        0     3012 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py
+-rw-r--r--   0        0        0     2712 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py
+-rw-r--r--   0        0        0     2722 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py
+-rw-r--r--   0        0        0     2425 2024-05-21 19:37:59.095577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2922 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py
+-rw-r--r--   0        0        0     2615 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py
+-rw-r--r--   0        0        0     3151 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_status_response.py
+-rw-r--r--   0        0        0     2884 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py
+-rw-r--r--   0        0        0     3761 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response.py
+-rw-r--r--   0        0        0     3483 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     4031 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py
+-rw-r--r--   0        0        0     2978 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py
+-rw-r--r--   0        0        0     3058 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py
+-rw-r--r--   0        0        0     2397 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_public_metrics_response.py
+-rw-r--r--   0        0        0     2073 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py
+-rw-r--r--   0        0        0     2767 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_sample_metadata_response.py
+-rw-r--r--   0        0        0     3044 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_sample_response.py
+-rw-r--r--   0        0        0     2462 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_syntiant_posterior_response.py
+-rw-r--r--   0        0        0     2184 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py
+-rw-r--r--   0        0        0     2694 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_target_constraints_response.py
+-rw-r--r--   0        0        0     2404 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_target_constraints_response_all_of.py
+-rw-r--r--   0        0        0     2414 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_theme_response.py
+-rw-r--r--   0        0        0     2117 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_theme_response_all_of.py
+-rw-r--r--   0        0        0     2592 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_themes_response.py
+-rw-r--r--   0        0        0     2285 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_themes_response_all_of.py
+-rw-r--r--   0        0        0     2495 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_third_party_auth_response.py
+-rw-r--r--   0        0        0     2171 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py
+-rw-r--r--   0        0        0     3543 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py
+-rw-r--r--   0        0        0     3276 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py
+-rw-r--r--   0        0        0    10235 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_response.py
+-rw-r--r--   0        0        0     7461 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_response_all_of.py
+-rw-r--r--   0        0        0     2395 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py
+-rw-r--r--   0        0        0     2307 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_domain_response.py
+-rw-r--r--   0        0        0     2021 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py
+-rw-r--r--   0        0        0     2514 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_response.py
+-rw-r--r--   0        0        0     2217 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py
+-rw-r--r--   0        0        0     2776 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/has_data_explorer_features_response.py
+-rw-r--r--   0        0        0     2498 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py
+-rw-r--r--   0        0        0      642 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/image_input_scaling.py
+-rw-r--r--   0        0        0     3738 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse.py
+-rw-r--r--   0        0        0     6723 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_block_version.py
+-rw-r--r--   0        0        0     6814 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_dsp_block.py
+-rw-r--r--   0        0        0     1967 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_dsp_block_organization.py
+-rw-r--r--   0        0        0     8958 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_input_block.py
+-rw-r--r--   0        0        0     5612 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_learn_block.py
+-rw-r--r--   0        0        0     2627 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/input_block.py
+-rw-r--r--   0        0        0     2323 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/invite_organization_member_request.py
+-rw-r--r--   0        0        0     4172 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job.py
+-rw-r--r--   0        0        0     2066 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_created_by_user.py
+-rw-r--r--   0        0        0     5203 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details.py
+-rw-r--r--   0        0        0     2736 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_all_of.py
+-rw-r--r--   0        0        0     2613 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_response.py
+-rw-r--r--   0        0        0     2316 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_response_all_of.py
+-rw-r--r--   0        0        0     2257 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_failure_details.py
+-rw-r--r--   0        0        0     2657 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_logs_response.py
+-rw-r--r--   0        0        0     2350 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_logs_response_all_of.py
+-rw-r--r--   0        0        0     3297 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_metrics_response.py
+-rw-r--r--   0        0        0     3007 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_metrics_response_all_of.py
+-rw-r--r--   0        0        0      546 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_parent_type_enum.py
+-rw-r--r--   0        0        0     2944 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_state.py
+-rw-r--r--   0        0        0     1966 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_state_execution_details.py
+-rw-r--r--   0        0        0      598 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_status.py
+-rw-r--r--   0        0        0     2965 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_step.py
+-rw-r--r--   0        0        0     2713 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response.py
+-rw-r--r--   0        0        0     2406 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response_all_of.py
+-rw-r--r--   0        0        0     2089 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py
+-rw-r--r--   0        0        0     1961 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py
+-rw-r--r--   0        0        0     1993 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_custom_metric.py
+-rw-r--r--   0        0        0     2510 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer.py
+-rw-r--r--   0        0        0     2093 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer_input.py
+-rw-r--r--   0        0        0     2101 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer_output.py
+-rw-r--r--   0        0        0     5707 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata.py
+-rw-r--r--   0        0        0     5440 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_all_of.py
+-rw-r--r--   0        0        0     5421 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics.py
+-rw-r--r--   0        0        0     4495 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py
+-rw-r--r--   0        0        0     2497 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py
+-rw-r--r--   0        0        0      562 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_type_enum.py
+-rw-r--r--   0        0        0      524 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_variant_enum.py
+-rw-r--r--   0        0        0    11377 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_response.py
+-rw-r--r--   0        0        0    11110 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_response_all_of.py
+-rw-r--r--   0        0        0     3392 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_visual_layer.py
+-rw-r--r--   0        0        0     2310 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_visual_layer_type.py
+-rw-r--r--   0        0        0     2529 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/last_modification_date_response.py
+-rw-r--r--   0        0        0     2239 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/last_modification_date_response_all_of.py
+-rw-r--r--   0        0        0     2633 2024-05-21 19:37:59.099577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/latency_device.py
+-rw-r--r--   0        0        0     3482 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/learn_block.py
+-rw-r--r--   0        0        0      933 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/learn_block_type.py
+-rw-r--r--   0        0        0     2788 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response.py
+-rw-r--r--   0        0        0     2488 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2619 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_devices_response.py
+-rw-r--r--   0        0        0     2312 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_devices_response_all_of.py
+-rw-r--r--   0        0        0     2726 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response.py
+-rw-r--r--   0        0        0     2426 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response_all_of.py
+-rw-r--r--   0        0        0     2918 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response_all_of_emails.py
+-rw-r--r--   0        0        0     2767 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_enterprise_trials_response.py
+-rw-r--r--   0        0        0     2467 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py
+-rw-r--r--   0        0        0     2813 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response.py
+-rw-r--r--   0        0        0     2513 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py
+-rw-r--r--   0        0        0     2381 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py
+-rw-r--r--   0        0        0     2745 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_jobs_response.py
+-rw-r--r--   0        0        0     2445 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_jobs_response_all_of.py
+-rw-r--r--   0        0        0     2200 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_models_response.py
+-rw-r--r--   0        0        0     1910 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_models_response_all_of.py
+-rw-r--r--   0        0        0     2921 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response.py
+-rw-r--r--   0        0        0     2621 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py
+-rw-r--r--   0        0        0     2752 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_response.py
+-rw-r--r--   0        0        0     2445 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py
+-rw-r--r--   0        0        0     2902 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response.py
+-rw-r--r--   0        0        0     2595 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py
+-rw-r--r--   0        0        0     2760 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py
+-rw-r--r--   0        0        0     3310 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response.py
+-rw-r--r--   0        0        0     3031 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response_all_of.py
+-rw-r--r--   0        0        0     3430 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py
+-rw-r--r--   0        0        0     2887 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py
+-rw-r--r--   0        0        0     2587 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2824 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py
+-rw-r--r--   0        0        0     2524 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3353 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_files_response.py
+-rw-r--r--   0        0        0     3074 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_files_response_all_of.py
+-rw-r--r--   0        0        0     2792 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_pipelines_response.py
+-rw-r--r--   0        0        0     2485 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py
+-rw-r--r--   0        0        0     2857 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response.py
+-rw-r--r--   0        0        0     2550 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py
+-rw-r--r--   0        0        0     2858 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py
+-rw-r--r--   0        0        0     3449 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response.py
+-rw-r--r--   0        0        0     3142 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py
+-rw-r--r--   0        0        0     2271 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py
+-rw-r--r--   0        0        0     2857 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response.py
+-rw-r--r--   0        0        0     2550 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py
+-rw-r--r--   0        0        0     2819 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py
+-rw-r--r--   0        0        0     3103 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py
+-rw-r--r--   0        0        0     2803 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py
+-rw-r--r--   0        0        0     3055 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2755 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2988 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_usage_reports_response.py
+-rw-r--r--   0        0        0     2688 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py
+-rw-r--r--   0        0        0     2786 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organizations_response.py
+-rw-r--r--   0        0        0     2486 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organizations_response_all_of.py
+-rw-r--r--   0        0        0     2512 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py
+-rw-r--r--   0        0        0     2872 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py
+-rw-r--r--   0        0        0     2593 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_projects.py
+-rw-r--r--   0        0        0     2681 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_projects_response.py
+-rw-r--r--   0        0        0     3122 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py
+-rw-r--r--   0        0        0     2822 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py
+-rw-r--r--   0        0        0     2553 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_projects.py
+-rw-r--r--   0        0        0     2944 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_projects_response.py
+-rw-r--r--   0        0        0     2815 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response.py
+-rw-r--r--   0        0        0     2508 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response_all_of.py
+-rw-r--r--   0        0        0     2290 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2754 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_samples_response.py
+-rw-r--r--   0        0        0     2454 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_samples_response_all_of.py
+-rw-r--r--   0        0        0     2615 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_tuner_runs_response.py
+-rw-r--r--   0        0        0     2308 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_tuner_runs_response_all_of.py
+-rw-r--r--   0        0        0     3933 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response.py
+-rw-r--r--   0        0        0     3633 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of.py
+-rw-r--r--   0        0        0     2353 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py
+-rw-r--r--   0        0        0     2053 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py
+-rw-r--r--   0        0        0     3960 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py
+-rw-r--r--   0        0        0     2367 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_analytics_event_request.py
+-rw-r--r--   0        0        0     2900 2024-05-21 19:37:59.103577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response.py
+-rw-r--r--   0        0        0     2600 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response_all_of.py
+-rw-r--r--   0        0        0     2441 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py
+-rw-r--r--   0        0        0     2191 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_website_pageview_request.py
+-rw-r--r--   0        0        0     2217 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/login_response.py
+-rw-r--r--   0        0        0     1911 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/login_response_all_of.py
+-rw-r--r--   0        0        0     2528 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/memory_spec.py
+-rw-r--r--   0        0        0     2746 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_all_variants_response.py
+-rw-r--r--   0        0        0     2449 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_all_variants_response_all_of.py
+-rw-r--r--   0        0        0     2128 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_for_model_variant.py
+-rw-r--r--   0        0        0     2430 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/migration.py
+-rw-r--r--   0        0        0      571 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_engine_short_enum.py
+-rw-r--r--   0        0        0     3010 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_prediction.py
+-rw-r--r--   0        0        0     2895 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_result.py
+-rw-r--r--   0        0        0     5046 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_variant_stats.py
+-rw-r--r--   0        0        0     2128 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/move_raw_data_request.py
+-rw-r--r--   0        0        0     2784 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_data.py
+-rw-r--r--   0        0        0     3584 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_score.py
+-rw-r--r--   0        0        0     2736 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py
+-rw-r--r--   0        0        0     2687 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/note.py
+-rw-r--r--   0        0        0     2221 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_request.py
+-rw-r--r--   0        0        0     2994 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response.py
+-rw-r--r--   0        0        0     2705 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py
+-rw-r--r--   0        0        0     2275 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py
+-rw-r--r--   0        0        0     2368 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py
+-rw-r--r--   0        0        0     2051 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py
+-rw-r--r--   0        0        0     2887 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_response.py
+-rw-r--r--   0        0        0     2580 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py
+-rw-r--r--   0        0        0      775 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_last_layer.py
+-rw-r--r--   0        0        0     6491 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config.py
+-rw-r--r--   0        0        0     6949 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_response.py
+-rw-r--r--   0        0        0     1920 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_response_all_of.py
+-rw-r--r--   0        0        0     2056 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_target_device.py
+-rw-r--r--   0        0        0     2271 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py
+-rw-r--r--   0        0        0     1964 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_space_response.py
+-rw-r--r--   0        0        0     2456 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_space_response_all_of.py
+-rw-r--r--   0        0        0     5546 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response.py
+-rw-r--r--   0        0        0     5279 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of.py
+-rw-r--r--   0        0        0     3284 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py
+-rw-r--r--   0        0        0     2273 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py
+-rw-r--r--   0        0        0     2749 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py
+-rw-r--r--   0        0        0     2425 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py
+-rw-r--r--   0        0        0     4717 2024-05-21 19:37:59.107577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py
+-rw-r--r--   0        0        0     5965 2024-05-21 19:37:59.111577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization.py
+-rw-r--r--   0        0        0     2700 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_request.py
+-rw-r--r--   0        0        0     2498 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_response.py
+-rw-r--r--   0        0        0     2209 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py
+-rw-r--r--   0        0        0     2835 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_dataset_request.py
+-rw-r--r--   0        0        0     2493 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2820 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_bucket.py
+-rw-r--r--   0        0        0     2711 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_compute_time_usage.py
+-rw-r--r--   0        0        0     9492 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project.py
+-rw-r--r--   0        0        0      605 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py
+-rw-r--r--   0        0        0     2262 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_path_filter.py
+-rw-r--r--   0        0        0     7464 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_request.py
+-rw-r--r--   0        0        0     2543 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_response.py
+-rw-r--r--   0        0        0     2237 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_response_all_of.py
+-rw-r--r--   0        0        0     2704 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_status_response.py
+-rw-r--r--   0        0        0     2407 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py
+-rw-r--r--   0        0        0     2754 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py
+-rw-r--r--   0        0        0    10387 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files.py
+-rw-r--r--   0        0        0     2744 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py
+-rw-r--r--   0        0        0     3483 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py
+-rw-r--r--   0        0        0     2559 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py
+-rw-r--r--   0        0        0     2327 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py
+-rw-r--r--   0        0        0     3041 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py
+-rw-r--r--   0        0        0     2741 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py
+-rw-r--r--   0        0        0     2468 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py
+-rw-r--r--   0        0        0     3483 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_export.py
+-rw-r--r--   0        0        0     3476 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_item.py
+-rw-r--r--   0        0        0     2303 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_item_files_inner.py
+-rw-r--r--   0        0        0     4007 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dataset.py
+-rw-r--r--   0        0        0     2800 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dataset_bucket.py
+-rw-r--r--   0        0        0     6005 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_deploy_block.py
+-rw-r--r--   0        0        0     4962 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dsp_block.py
+-rw-r--r--   0        0        0     3037 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response.py
+-rw-r--r--   0        0        0     2737 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py
+-rw-r--r--   0        0        0     7063 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py
+-rw-r--r--   0        0        0     6864 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response.py
+-rw-r--r--   0        0        0     6574 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of.py
+-rw-r--r--   0        0        0     3915 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py
+-rw-r--r--   0        0        0     2267 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py
+-rw-r--r--   0        0        0     2338 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py
+-rw-r--r--   0        0        0     2458 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py
+-rw-r--r--   0        0        0     2101 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_performance.py
+-rw-r--r--   0        0        0      525 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_member_role.py
+-rw-r--r--   0        0        0     2639 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response.py
+-rw-r--r--   0        0        0     2315 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response_all_of.py
+-rw-r--r--   0        0        0     4480 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0     6143 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline.py
+-rw-r--r--   0        0        0     2595 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py
+-rw-r--r--   0        0        0     2275 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py
+-rw-r--r--   0        0        0     2314 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_item_count.py
+-rw-r--r--   0        0        0     4129 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_run.py
+-rw-r--r--   0        0        0     5330 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_run_step.py
+-rw-r--r--   0        0        0     6532 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_step.py
+-rw-r--r--   0        0        0     2351 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py
+-rw-r--r--   0        0        0     2344 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py
+-rw-r--r--   0        0        0     2037 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_request.py
+-rw-r--r--   0        0        0     7562 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transfer_learning_block.py
+-rw-r--r--   0        0        0      611 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py
+-rw-r--r--   0        0        0     8670 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transformation_block.py
+-rw-r--r--   0        0        0     3918 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_update_pipeline_body.py
+-rw-r--r--   0        0        0     3351 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_usage_report.py
+-rw-r--r--   0        0        0     5030 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_user.py
+-rw-r--r--   0        0        0     2294 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_user_all_of.py
+-rw-r--r--   0        0        0     2104 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_detection.py
+-rw-r--r--   0        0        0     3434 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_false_positive.py
+-rw-r--r--   0        0        0     3770 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_ground_truth.py
+-rw-r--r--   0        0        0     2477 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py
+-rw-r--r--   0        0        0     4880 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set.py
+-rw-r--r--   0        0        0     2255 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py
+-rw-r--r--   0        0        0     4092 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py
+-rw-r--r--   0        0        0     3007 2024-05-21 19:37:59.115577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameters.py
+-rw-r--r--   0        0        0     2585 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py
+-rw-r--r--   0        0        0     2250 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_raw_detection.py
+-rw-r--r--   0        0        0     2366 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py
+-rw-r--r--   0        0        0     2412 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py
+-rw-r--r--   0        0        0     2106 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py
+-rw-r--r--   0        0        0     1839 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/permission.py
+-rw-r--r--   0        0        0     2491 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/portal_file.py
+-rw-r--r--   0        0        0     2537 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/portal_info_response.py
+-rw-r--r--   0        0        0     2666 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/pretrained_model_tensor.py
+-rw-r--r--   0        0        0     2403 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_request.py
+-rw-r--r--   0        0        0     3734 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_response.py
+-rw-r--r--   0        0        0     3467 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py
+-rw-r--r--   0        0        0     2955 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info.py
+-rw-r--r--   0        0        0     3117 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory.py
+-rw-r--r--   0        0        0     1918 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory_eon.py
+-rw-r--r--   0        0        0     2065 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py
+-rw-r--r--   0        0        0     4335 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table.py
+-rw-r--r--   0        0        0     2780 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mcu.py
+-rw-r--r--   0        0        0     3042 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py
+-rw-r--r--   0        0        0     2250 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mpu.py
+-rw-r--r--   0        0        0     2201 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_tf_lite_request.py
+-rw-r--r--   0        0        0     3292 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_tf_lite_response.py
+-rw-r--r--   0        0        0     7873 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project.py
+-rw-r--r--   0        0        0     4693 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_collaborator.py
+-rw-r--r--   0        0        0     1895 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_collaborator_all_of.py
+-rw-r--r--   0        0        0     2416 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_axes_summary_response.py
+-rw-r--r--   0        0        0     2116 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py
+-rw-r--r--   0        0        0     2281 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_interval_response.py
+-rw-r--r--   0        0        0     1964 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_interval_response_all_of.py
+-rw-r--r--   0        0        0     2235 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_summary.py
+-rw-r--r--   0        0        0     6854 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_target.py
+-rw-r--r--   0        0        0     2706 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_target_all_of.py
+-rw-r--r--   0        0        0     2780 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_targets_response.py
+-rw-r--r--   0        0        0     2473 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py
+-rw-r--r--   0        0        0     1943 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2680 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_downloads_response.py
+-rw-r--r--   0        0        0     2373 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_downloads_response_all_of.py
+-rw-r--r--   0        0        0    14783 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response.py
+-rw-r--r--   0        0        0    14516 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of.py
+-rw-r--r--   0        0        0     4174 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py
+-rw-r--r--   0        0        0     2723 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py
+-rw-r--r--   0        0        0     2997 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py
+-rw-r--r--   0        0        0     3200 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py
+-rw-r--r--   0        0        0     2339 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py
+-rw-r--r--   0        0        0     2285 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py
+-rw-r--r--   0        0        0     2726 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_performance.py
+-rw-r--r--   0        0        0     1977 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_readme.py
+-rw-r--r--   0        0        0     2225 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py
+-rw-r--r--   0        0        0     2735 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_urls.py
+-rw-r--r--   0        0        0     2478 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_summary_response.py
+-rw-r--r--   0        0        0     2172 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_summary_response_all_of.py
+-rw-r--r--   0        0        0     2715 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_model_variant.py
+-rw-r--r--   0        0        0     3554 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_private_data.py
+-rw-r--r--   0        0        0     4127 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_public_data.py
+-rw-r--r--   0        0        0     1928 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_public_data_readme.py
+-rw-r--r--   0        0        0     2404 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_sample_metadata.py
+-rw-r--r--   0        0        0      576 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_tier_enum.py
+-rw-r--r--   0        0        0     2804 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response.py
+-rw-r--r--   0        0        0     2487 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py
+-rw-r--r--   0        0        0     2253 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py
+-rw-r--r--   0        0        0      606 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_type.py
+-rw-r--r--   0        0        0     2316 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_version_request.py
+-rw-r--r--   0        0        0      504 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_visibility.py
+-rw-r--r--   0        0        0     4991 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/public_organization_transformation_block.py
+-rw-r--r--   0        0        0      588 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/public_project_tier_availability.py
+-rw-r--r--   0        0        0     2664 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/raw_sample_data.py
+-rw-r--r--   0        0        0     3440 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/raw_sample_payload.py
+-rw-r--r--   0        0        0     2537 2024-05-21 19:37:59.119577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/rebalance_dataset_response.py
+-rw-r--r--   0        0        0     1984 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/remove_collaborator_request.py
+-rw-r--r--   0        0        0     1805 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/remove_member_request.py
+-rw-r--r--   0        0        0     1867 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_device_request.py
+-rw-r--r--   0        0        0     2081 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_portal_file_request.py
+-rw-r--r--   0        0        0     1867 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_sample_request.py
+-rw-r--r--   0        0        0     2028 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/request_email_verification_request.py
+-rw-r--r--   0        0        0     1873 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/request_reset_password_request.py
+-rw-r--r--   0        0        0     2031 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/reset_password_request.py
+-rw-r--r--   0        0        0     1896 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/resource_range.py
+-rw-r--r--   0        0        0     1985 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/restore_project_from_public_request.py
+-rw-r--r--   0        0        0     2265 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/restore_project_request.py
+-rw-r--r--   0        0        0     2421 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_auto_labeler_request.py
+-rw-r--r--   0        0        0     2669 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_organization_pipeline_response.py
+-rw-r--r--   0        0        0     2352 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py
+-rw-r--r--   0        0        0    11134 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample.py
+-rw-r--r--   0        0        0     2443 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample_bounding_boxes_request.py
+-rw-r--r--   0        0        0     2000 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample_metadata.py
+-rw-r--r--   0        0        0     2517 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_request.py
+-rw-r--r--   0        0        0     2071 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py
+-rw-r--r--   0        0        0     2341 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_response.py
+-rw-r--r--   0        0        0     2024 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py
+-rw-r--r--   0        0        0     2756 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_pretrained_model_request.py
+-rw-r--r--   0        0        0     3327 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response.py
+-rw-r--r--   0        0        0     3003 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of.py
+-rw-r--r--   0        0        0     2240 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py
+-rw-r--r--   0        0        0     1914 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py
+-rw-r--r--   0        0        0     2405 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/segment_sample_request.py
+-rw-r--r--   0        0        0     2055 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py
+-rw-r--r--   0        0        0     3346 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/send_user_feedback_request.py
+-rw-r--r--   0        0        0     1981 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/sensor.py
+-rw-r--r--   0        0        0     2142 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_anomaly_parameter_request.py
+-rw-r--r--   0        0        0     9364 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_keras_parameter_request.py
+-rw-r--r--   0        0        0     1893 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_member_datasets_request.py
+-rw-r--r--   0        0        0     1905 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_member_role_request.py
+-rw-r--r--   0        0        0     2219 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_optimize_space_request.py
+-rw-r--r--   0        0        0     2254 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py
+-rw-r--r--   0        0        0     1923 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_organization_data_dataset_request.py
+-rw-r--r--   0        0        0     1974 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_project_compute_time_request.py
+-rw-r--r--   0        0        0     2011 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py
+-rw-r--r--   0        0        0     1919 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_sample_metadata_request.py
+-rw-r--r--   0        0        0     2531 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_sample_structured_labels_request.py
+-rw-r--r--   0        0        0     1915 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_syntiant_posterior_request.py
+-rw-r--r--   0        0        0     2140 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_user_password_request.py
+-rw-r--r--   0        0        0     2536 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response.py
+-rw-r--r--   0        0        0     2239 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response_all_of.py
+-rw-r--r--   0        0        0     2059 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response_all_of_token.py
+-rw-r--r--   0        0        0     1971 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/split_sample_in_frames_request.py
+-rw-r--r--   0        0        0     2110 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/staff_info.py
+-rw-r--r--   0        0        0     2098 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_classify_job_request.py
+-rw-r--r--   0        0        0     2292 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_debug_stream_response.py
+-rw-r--r--   0        0        0     1975 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py
+-rw-r--r--   0        0        0     2178 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py
+-rw-r--r--   0        0        0     5388 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_enterprise_trial_request.py
+-rw-r--r--   0        0        0     2226 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_job_response.py
+-rw-r--r--   0        0        0     1909 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_job_response_all_of.py
+-rw-r--r--   0        0        0     2883 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_performance_calibration_request.py
+-rw-r--r--   0        0        0     2838 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_request.py
+-rw-r--r--   0        0        0     2189 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_response.py
+-rw-r--r--   0        0        0     1892 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_response_all_of.py
+-rw-r--r--   0        0        0     2795 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_training_request_anomaly.py
+-rw-r--r--   0        0        0     1926 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/stop_device_debug_stream_request.py
+-rw-r--r--   0        0        0     1967 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/store_segment_length_request.py
+-rw-r--r--   0        0        0     3394 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/structured_classify_result.py
+-rw-r--r--   0        0        0     2270 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/structured_label.py
+-rw-r--r--   0        0        0     4399 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_constraints.py
+-rw-r--r--   0        0        0     2923 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_constraints_device.py
+-rw-r--r--   0        0        0     2347 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_memory.py
+-rw-r--r--   0        0        0     3751 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_processor.py
+-rw-r--r--   0        0        0     2433 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_request.py
+-rw-r--r--   0        0        0     3074 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_response.py
+-rw-r--r--   0        0        0     2784 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py
+-rw-r--r--   0        0        0     3251 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme.py
+-rw-r--r--   0        0        0     2239 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_colors.py
+-rw-r--r--   0        0        0     2764 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_favicon.py
+-rw-r--r--   0        0        0     2721 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_logos.py
+-rw-r--r--   0        0        0     2245 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/third_party_auth.py
+-rw-r--r--   0        0        0     1921 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/time_series_data_point.py
+-rw-r--r--   0        0        0     2031 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_request.py
+-rw-r--r--   0        0        0     2736 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_response.py
+-rw-r--r--   0        0        0     2436 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_response_all_of.py
+-rw-r--r--   0        0        0     5380 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/transfer_learning_model.py
+-rw-r--r--   0        0        0     2012 2024-05-21 19:37:59.123577 edgeimpulse_api-1.50.0/edgeimpulse_api/models/transfer_ownership_organization_request.py
+-rw-r--r--   0        0        0     2585 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py
+-rw-r--r--   0        0        0      548 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_job_operates_on_enum.py
+-rw-r--r--   0        0        0      588 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_job_status_enum.py
+-rw-r--r--   0        0        0     2578 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_create_trial_impulse.py
+-rw-r--r--   0        0        0     2462 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_run.py
+-rw-r--r--   0        0        0     2570 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_space_impulse.py
+-rw-r--r--   0        0        0     4991 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial.py
+-rw-r--r--   0        0        0     2739 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py
+-rw-r--r--   0        0        0     1935 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py
+-rw-r--r--   0        0        0     2211 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_impulse.py
+-rw-r--r--   0        0        0     2028 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_job_request.py
+-rw-r--r--   0        0        0     2281 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py
+-rw-r--r--   0        0        0     2882 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_bucket_request.py
+-rw-r--r--   0        0        0     2828 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py
+-rw-r--r--   0        0        0     2428 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_create_project_request.py
+-rw-r--r--   0        0        0     2913 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py
+-rw-r--r--   0        0        0     4154 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_campaign_request.py
+-rw-r--r--   0        0        0     2158 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_item_request.py
+-rw-r--r--   0        0        0     2977 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dataset_request.py
+-rw-r--r--   0        0        0     2518 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dataset_request_bucket.py
+-rw-r--r--   0        0        0     2881 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dsp_block_request.py
+-rw-r--r--   0        0        0     2724 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_portal_response.py
+-rw-r--r--   0        0        0     2445 2024-05-21 19:37:59.171576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py
+-rw-r--r--   0        0        0     2953 2024-05-21 19:37:59.175576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_request.py
+-rw-r--r--   0        0        0     5266 2024-05-21 19:37:59.175576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py
+-rw-r--r--   0        0        0     6072 2024-05-21 19:37:59.175576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_transformation_block_request.py
+-rw-r--r--   0        0        0    12462 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_project_request.py
+-rw-r--r--   0        0        0     1877 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_project_tags_request.py
+-rw-r--r--   0        0        0     2259 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_theme_colors_request.py
+-rw-r--r--   0        0        0     2895 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_theme_logos_request.py
+-rw-r--r--   0        0        0     2205 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_third_party_auth_request.py
+-rw-r--r--   0        0        0     1865 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_tuner_run_request.py
+-rw-r--r--   0        0        0     2641 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_user_request.py
+-rw-r--r--   0        0        0     1886 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_version_request.py
+-rw-r--r--   0        0        0     2393 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py
+-rw-r--r--   0        0        0     2237 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py
+-rw-r--r--   0        0        0     2125 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py
+-rw-r--r--   0        0        0     2155 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py
+-rw-r--r--   0        0        0     2059 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_request.py
+-rw-r--r--   0        0        0     2403 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upgrade_subscription_request.py
+-rw-r--r--   0        0        0     2168 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_asset_response.py
+-rw-r--r--   0        0        0     1882 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_asset_response_all_of.py
+-rw-r--r--   0        0        0     2199 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_readme_image_response.py
+-rw-r--r--   0        0        0     2185 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_user_photo_response.py
+-rw-r--r--   0        0        0     1872 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py
+-rw-r--r--   0        0        0     4478 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user.py
+-rw-r--r--   0        0        0     1991 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_by_third_party_activation_request.py
+-rw-r--r--   0        0        0     1956 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     1922 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_dismiss_notification_request.py
+-rw-r--r--   0        0        0     2192 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_experiment.py
+-rw-r--r--   0        0        0     2425 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_generate_new_mfa_key_response.py
+-rw-r--r--   0        0        0     2119 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     4725 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_organization.py
+-rw-r--r--   0        0        0      686 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_projects_sort_order.py
+-rw-r--r--   0        0        0     2144 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_request.py
+-rw-r--r--   0        0        0     2480 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_response.py
+-rw-r--r--   0        0        0     2191 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py
+-rw-r--r--   0        0        0     2695 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_subscription_metrics_response.py
+-rw-r--r--   0        0        0     2398 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_subscription_metrics_response_all_of.py
+-rw-r--r--   0        0        0     3225 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_subscription_metrics_response_all_of_metrics.py
+-rw-r--r--   0        0        0      573 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_tier_enum.py
+-rw-r--r--   0        0        0     1844 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_request.py
+-rw-r--r--   0        0        0     2604 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response.py
+-rw-r--r--   0        0        0     2307 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py
+-rw-r--r--   0        0        0     3049 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py
+-rw-r--r--   0        0        0     2633 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_email_response.py
+-rw-r--r--   0        0        0     2354 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_email_response_all_of.py
+-rw-r--r--   0        0        0     2708 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_request.py
+-rw-r--r--   0        0        0     3432 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response.py
+-rw-r--r--   0        0        0     3155 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py
+-rw-r--r--   0        0        0     2187 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py
+-rw-r--r--   0        0        0     1961 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_existing_bucket_request.py
+-rw-r--r--   0        0        0     1937 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_reset_password_request.py
+-rw-r--r--   0        0        0     8565 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel.py
+-rw-r--r--   0        0        0     2534 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py
+-rw-r--r--   0        0        0     2085 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py
+-rw-r--r--   0        0        0     2120 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py
+-rw-r--r--   0        0        0     2885 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response.py
+-rw-r--r--   0        0        0     2585 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response_all_of.py
+-rw-r--r--   0        0        0     2848 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py
+-rw-r--r--   0        0        0    12674 2024-05-21 19:37:59.179576 edgeimpulse_api-1.50.0/edgeimpulse_api/rest.py
+-rw-r--r--   0        0        0     1019 2024-05-21 19:38:53.674664 edgeimpulse_api-1.50.0/pyproject.toml
+-rw-r--r--   0        0        0     1391 1970-01-01 00:00:00.000000 edgeimpulse_api-1.50.0/PKG-INFO
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/__init__.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     The version of the OpenAPI document: 1.0.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.49.9" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+__version__ = "1.50.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 
 # import apis into sdk package
 from edgeimpulse_api.api.admin_api import AdminApi
 from edgeimpulse_api.api.auth_api import AuthApi
 from edgeimpulse_api.api.cdn_api import CDNApi
 from edgeimpulse_api.api.classify_api import ClassifyApi
 from edgeimpulse_api.api.dsp_api import DSPApi
@@ -162,32 +162,37 @@
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of import AnomalyTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of_data import AnomalyTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.application_budget import ApplicationBudget
 from edgeimpulse_api.models.augmentation_policy_image_enum import AugmentationPolicyImageEnum
 from edgeimpulse_api.models.augmentation_policy_spectrogram import AugmentationPolicySpectrogram
 from edgeimpulse_api.models.autotune_dsp_request import AutotuneDspRequest
+from edgeimpulse_api.models.billing_cycle import BillingCycle
 from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
 from edgeimpulse_api.models.block_type import BlockType
 from edgeimpulse_api.models.bounding_box import BoundingBox
 from edgeimpulse_api.models.bounding_box_with_score import BoundingBoxWithScore
 from edgeimpulse_api.models.build_on_device_model_request import BuildOnDeviceModelRequest
 from edgeimpulse_api.models.build_organization_on_device_model_request import BuildOrganizationOnDeviceModelRequest
 from edgeimpulse_api.models.calculate_data_quality_metrics_request import CalculateDataQualityMetricsRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_all_of import ClassifyJobResponseAllOf
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy_total_summary import ClassifyJobResponseAllOfAccuracyTotalSummary
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
 from edgeimpulse_api.models.classify_job_response_page_all_of import ClassifyJobResponsePageAllOf
+from edgeimpulse_api.models.classify_sample_for_variants200_response import ClassifySampleForVariants200Response
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.classify_sample_response_all_of import ClassifySampleResponseAllOf
 from edgeimpulse_api.models.classify_sample_response_classification import ClassifySampleResponseClassification
 from edgeimpulse_api.models.classify_sample_response_classification_details import ClassifySampleResponseClassificationDetails
+from edgeimpulse_api.models.classify_sample_response_multiple_variants import ClassifySampleResponseMultipleVariants
+from edgeimpulse_api.models.classify_sample_response_multiple_variants_all_of import ClassifySampleResponseMultipleVariantsAllOf
+from edgeimpulse_api.models.classify_sample_response_variant_results import ClassifySampleResponseVariantResults
 from edgeimpulse_api.models.classify_sample_v2200_response import ClassifySampleV2200Response
 from edgeimpulse_api.models.convert_user_request import ConvertUserRequest
 from edgeimpulse_api.models.cosine_similarity_data import CosineSimilarityData
 from edgeimpulse_api.models.cosine_similarity_issue import CosineSimilarityIssue
 from edgeimpulse_api.models.cosine_similarity_issue_issues_inner import CosineSimilarityIssueIssuesInner
 from edgeimpulse_api.models.cosine_similarity_issue_issues_inner_windows_inner import CosineSimilarityIssueIssuesInnerWindowsInner
 from edgeimpulse_api.models.count_samples_response import CountSamplesResponse
@@ -261,14 +266,15 @@
 from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
 from edgeimpulse_api.models.data_explorer_predictions_response import DataExplorerPredictionsResponse
 from edgeimpulse_api.models.data_explorer_predictions_response_all_of import DataExplorerPredictionsResponseAllOf
 from edgeimpulse_api.models.data_explorer_settings import DataExplorerSettings
 from edgeimpulse_api.models.dataset_ratio_data import DatasetRatioData
 from edgeimpulse_api.models.dataset_ratio_data_ratio import DatasetRatioDataRatio
 from edgeimpulse_api.models.delete_portal_file_request import DeletePortalFileRequest
+from edgeimpulse_api.models.delete_user_request import DeleteUserRequest
 from edgeimpulse_api.models.dependency_data import DependencyData
 from edgeimpulse_api.models.deploy_pretrained_model_input_audio import DeployPretrainedModelInputAudio
 from edgeimpulse_api.models.deploy_pretrained_model_input_image import DeployPretrainedModelInputImage
 from edgeimpulse_api.models.deploy_pretrained_model_input_other import DeployPretrainedModelInputOther
 from edgeimpulse_api.models.deploy_pretrained_model_input_time_series import DeployPretrainedModelInputTimeSeries
 from edgeimpulse_api.models.deploy_pretrained_model_model_classification import DeployPretrainedModelModelClassification
 from edgeimpulse_api.models.deploy_pretrained_model_model_object_detection import DeployPretrainedModelModelObjectDetection
@@ -401,14 +407,16 @@
 from edgeimpulse_api.models.get_job_response_all_of import GetJobResponseAllOf
 from edgeimpulse_api.models.get_label_noise_data_response import GetLabelNoiseDataResponse
 from edgeimpulse_api.models.get_label_noise_data_response_all_of import GetLabelNoiseDataResponseAllOf
 from edgeimpulse_api.models.get_label_noise_data_response_all_of_data import GetLabelNoiseDataResponseAllOfData
 from edgeimpulse_api.models.get_last_deployment_build_response import GetLastDeploymentBuildResponse
 from edgeimpulse_api.models.get_last_deployment_build_response_all_of import GetLastDeploymentBuildResponseAllOf
 from edgeimpulse_api.models.get_last_deployment_build_response_all_of_last_build import GetLastDeploymentBuildResponseAllOfLastBuild
+from edgeimpulse_api.models.get_model_variants_response import GetModelVariantsResponse
+from edgeimpulse_api.models.get_model_variants_response_all_of import GetModelVariantsResponseAllOf
 from edgeimpulse_api.models.get_notes_response import GetNotesResponse
 from edgeimpulse_api.models.get_notes_response_all_of import GetNotesResponseAllOf
 from edgeimpulse_api.models.get_organization_bucket_response import GetOrganizationBucketResponse
 from edgeimpulse_api.models.get_organization_bucket_response_all_of import GetOrganizationBucketResponseAllOf
 from edgeimpulse_api.models.get_organization_data_campaign_dashboard_response import GetOrganizationDataCampaignDashboardResponse
 from edgeimpulse_api.models.get_organization_data_campaign_dashboard_response_all_of import GetOrganizationDataCampaignDashboardResponseAllOf
 from edgeimpulse_api.models.get_organization_data_campaign_dashboards_response import GetOrganizationDataCampaignDashboardsResponse
@@ -768,26 +776,28 @@
 from edgeimpulse_api.models.project_info_response_all_of_impulse import ProjectInfoResponseAllOfImpulse
 from edgeimpulse_api.models.project_info_response_all_of_performance import ProjectInfoResponseAllOfPerformance
 from edgeimpulse_api.models.project_info_response_all_of_readme import ProjectInfoResponseAllOfReadme
 from edgeimpulse_api.models.project_info_response_all_of_show_getting_started_wizard import ProjectInfoResponseAllOfShowGettingStartedWizard
 from edgeimpulse_api.models.project_info_response_all_of_urls import ProjectInfoResponseAllOfUrls
 from edgeimpulse_api.models.project_info_summary_response import ProjectInfoSummaryResponse
 from edgeimpulse_api.models.project_info_summary_response_all_of import ProjectInfoSummaryResponseAllOf
+from edgeimpulse_api.models.project_model_variant import ProjectModelVariant
 from edgeimpulse_api.models.project_private_data import ProjectPrivateData
 from edgeimpulse_api.models.project_public_data import ProjectPublicData
 from edgeimpulse_api.models.project_public_data_readme import ProjectPublicDataReadme
 from edgeimpulse_api.models.project_sample_metadata import ProjectSampleMetadata
 from edgeimpulse_api.models.project_tier_enum import ProjectTierEnum
 from edgeimpulse_api.models.project_training_data_summary_response import ProjectTrainingDataSummaryResponse
 from edgeimpulse_api.models.project_training_data_summary_response_all_of import ProjectTrainingDataSummaryResponseAllOf
 from edgeimpulse_api.models.project_training_data_summary_response_all_of_data_summary import ProjectTrainingDataSummaryResponseAllOfDataSummary
 from edgeimpulse_api.models.project_type import ProjectType
 from edgeimpulse_api.models.project_version_request import ProjectVersionRequest
 from edgeimpulse_api.models.project_visibility import ProjectVisibility
 from edgeimpulse_api.models.public_organization_transformation_block import PublicOrganizationTransformationBlock
+from edgeimpulse_api.models.public_project_tier_availability import PublicProjectTierAvailability
 from edgeimpulse_api.models.raw_sample_data import RawSampleData
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
 from edgeimpulse_api.models.rename_portal_file_request import RenamePortalFileRequest
@@ -831,14 +841,15 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_classify_job_request import StartClassifyJobRequest
 from edgeimpulse_api.models.start_device_debug_stream_response import StartDeviceDebugStreamResponse
 from edgeimpulse_api.models.start_device_debug_stream_response_all_of import StartDeviceDebugStreamResponseAllOf
 from edgeimpulse_api.models.start_device_snapshot_debug_stream_request import StartDeviceSnapshotDebugStreamRequest
 from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
@@ -903,30 +914,35 @@
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
 from edgeimpulse_api.models.update_version_request import UpdateVersionRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
 from edgeimpulse_api.models.update_whitelabel_learning_blocks_request import UpdateWhitelabelLearningBlocksRequest
 from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
+from edgeimpulse_api.models.upgrade_subscription_request import UpgradeSubscriptionRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_asset_response_all_of import UploadAssetResponseAllOf
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.upload_user_photo_response_all_of import UploadUserPhotoResponseAllOf
 from edgeimpulse_api.models.user import User
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.user_delete_totp_mfa_key_request import UserDeleteTotpMfaKeyRequest
 from edgeimpulse_api.models.user_dismiss_notification_request import UserDismissNotificationRequest
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_generate_new_mfa_key_response import UserGenerateNewMfaKeyResponse
 from edgeimpulse_api.models.user_generate_new_mfa_key_response_all_of import UserGenerateNewMfaKeyResponseAllOf
 from edgeimpulse_api.models.user_organization import UserOrganization
+from edgeimpulse_api.models.user_projects_sort_order import UserProjectsSortOrder
 from edgeimpulse_api.models.user_set_totp_mfa_key_request import UserSetTotpMfaKeyRequest
 from edgeimpulse_api.models.user_set_totp_mfa_key_response import UserSetTotpMfaKeyResponse
 from edgeimpulse_api.models.user_set_totp_mfa_key_response_all_of import UserSetTotpMfaKeyResponseAllOf
+from edgeimpulse_api.models.user_subscription_metrics_response import UserSubscriptionMetricsResponse
+from edgeimpulse_api.models.user_subscription_metrics_response_all_of import UserSubscriptionMetricsResponseAllOf
+from edgeimpulse_api.models.user_subscription_metrics_response_all_of_metrics import UserSubscriptionMetricsResponseAllOfMetrics
 from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 from edgeimpulse_api.models.verify_dsp_block_url_request import VerifyDspBlockUrlRequest
 from edgeimpulse_api.models.verify_dsp_block_url_response import VerifyDspBlockUrlResponse
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of import VerifyDspBlockUrlResponseAllOf
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
 from edgeimpulse_api.models.verify_email_response import VerifyEmailResponse
 from edgeimpulse_api.models.verify_email_response_all_of import VerifyEmailResponseAllOf
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/__init__.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/admin_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/admin_api.py`

 * *Files identical despite different names*

```diff
@@ -2483,23 +2483,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def admin_delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], full_deletion : Annotated[Optional[StrictBool], Field(description="Set to true for full deletion")] = None, **kwargs) -> StartJobResponse:  # noqa: E501
+    def admin_delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> StartJobResponse:  # noqa: E501
         """Delete a user
 
-        Admin-only API to delete a user. If `fullDeletion` is set, it deletes the user's identifiable information and files. Otherwise, it soft deletes the user by setting it's `delete_date` value.
+        Admin-only API to delete a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param full_deletion: Set to true for full deletion
-        :type full_deletion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -2508,26 +2506,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: StartJobResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._admin_delete_user_with_http_info(user_id, full_deletion, **kwargs)  # noqa: E501
+        return self._admin_delete_user_with_http_info(user_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _admin_delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], full_deletion : Annotated[Optional[StrictBool], Field(description="Set to true for full deletion")] = None, **kwargs):  # noqa: E501
+    def _admin_delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
         """Delete a user 
 
-        Admin-only API to delete a user. If `fullDeletion` is set, it deletes the user's identifiable information and files. Otherwise, it soft deletes the user by setting it's `delete_date` value.
+        Admin-only API to delete a user.
 
         :param user_id: User ID (required)
         :type user_id: int
-        :param full_deletion: Set to true for full deletion
-        :type full_deletion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2547,16 +2543,15 @@
                  returns the request thread.
         :rtype: tuple(StartJobResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'user_id',
-            'full_deletion'
+            'user_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -2581,16 +2576,14 @@
         # process the path parameters
         _path_params = {}
         if _params['user_id']:
             _path_params['userId'] = _params['user_id']
 
         # process the query parameters
         _query_params = []
-        if _params.get('full_deletion') is not None:  # noqa: E501
-            _query_params.append(('fullDeletion', _params['full_deletion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/auth_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/cdn_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/cdn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/classify_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/classify_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,20 +13,21 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import Field, StrictBool, StrictInt
+from pydantic import Field, StrictBool, StrictInt, StrictStr
 
 from typing import Optional
 
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
+from edgeimpulse_api.models.classify_sample_for_variants200_response import ClassifySampleForVariants200Response
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.classify_sample_v2200_response import ClassifySampleV2200Response
 from edgeimpulse_api.models.get_sample_response import GetSampleResponse
 from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.metrics_all_variants_response import MetricsAllVariantsResponse
 
 from edgeimpulse_api.api_client import ApiClient
@@ -478,14 +479,168 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def classify_sample_for_variants(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], sample_id : Annotated[StrictInt, Field(..., description="Sample ID")], variants : Annotated[StrictStr, Field(..., description="List of keras model variants, given as a JSON string")], include_debug_info : Annotated[Optional[StrictBool], Field(description="Whether to return the debug information from FOMO classification.")] = None, **kwargs) -> ClassifySampleForVariants200Response:  # noqa: E501
+        """Classify sample for the given set of variants
+
+        Classify a complete file against the current impulse, for all given variants. Depending on the size of your file and whether the sample is resampled, you may get a job ID in the response. 
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param sample_id: Sample ID (required)
+        :type sample_id: int
+        :param variants: List of keras model variants, given as a JSON string (required)
+        :type variants: str
+        :param include_debug_info: Whether to return the debug information from FOMO classification.
+        :type include_debug_info: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ClassifySampleForVariants200Response
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._classify_sample_for_variants_with_http_info(project_id, sample_id, variants, include_debug_info, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _classify_sample_for_variants_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], sample_id : Annotated[StrictInt, Field(..., description="Sample ID")], variants : Annotated[StrictStr, Field(..., description="List of keras model variants, given as a JSON string")], include_debug_info : Annotated[Optional[StrictBool], Field(description="Whether to return the debug information from FOMO classification.")] = None, **kwargs):  # noqa: E501
+        """Classify sample for the given set of variants 
+
+        Classify a complete file against the current impulse, for all given variants. Depending on the size of your file and whether the sample is resampled, you may get a job ID in the response. 
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param sample_id: Sample ID (required)
+        :type sample_id: int
+        :param variants: List of keras model variants, given as a JSON string (required)
+        :type variants: str
+        :param include_debug_info: Whether to return the debug information from FOMO classification.
+        :type include_debug_info: bool
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(ClassifySampleForVariants200Response, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'project_id',
+            'sample_id',
+            'variants',
+            'include_debug_info'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method classify_sample_for_variants" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['project_id']:
+            _path_params['projectId'] = _params['project_id']
+        if _params['sample_id']:
+            _path_params['sampleId'] = _params['sample_id']
+
+        # process the query parameters
+        _query_params = []
+        if _params.get('include_debug_info') is not None:  # noqa: E501
+            _query_params.append(('includeDebugInfo', _params['include_debug_info']))
+        if _params.get('variants') is not None:  # noqa: E501
+            _query_params.append(('variants', _params['variants']))
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ClassifySampleForVariants200Response",
+        }
+
+        return self.api_client.call_api(
+            '/api/{projectId}/classify/v2/{sampleId}/variants', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/deployment_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/deployment_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/devices_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/devices_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/dsp_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/dsp_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/email_verification_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/email_verification_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/export_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/feature_flags_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/feature_flags_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/health_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/health_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/impulse_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/impulse_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/jobs_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/jobs_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 from edgeimpulse_api.models.log_stdout_response import LogStdoutResponse
 from edgeimpulse_api.models.profile_tf_lite_request import ProfileTfLiteRequest
 from edgeimpulse_api.models.profile_tf_lite_response import ProfileTfLiteResponse
 from edgeimpulse_api.models.project_version_request import ProjectVersionRequest
 from edgeimpulse_api.models.restore_project_from_public_request import RestoreProjectFromPublicRequest
 from edgeimpulse_api.models.restore_project_request import RestoreProjectRequest
 from edgeimpulse_api.models.set_keras_parameter_request import SetKerasParameterRequest
+from edgeimpulse_api.models.start_classify_job_request import StartClassifyJobRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
 from edgeimpulse_api.models.start_training_request_anomaly import StartTrainingRequestAnomaly
 from edgeimpulse_api.models.update_job_request import UpdateJobRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
@@ -2389,15 +2390,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_all_jobs(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, **kwargs) -> ListJobsResponse:  # noqa: E501
+    def list_all_jobs(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, key : Annotated[Optional[StrictStr], Field(description="Job key to filter on")] = None, **kwargs) -> ListJobsResponse:  # noqa: E501
         """List all jobs
 
         Get all jobs for this project
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param start_date: Start date
@@ -2406,14 +2407,16 @@
         :type end_date: datetime
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
         :type offset: int
         :param root_only: Whether to exclude jobs with a parent ID (so jobs started as part of another job)
         :type root_only: bool
+        :param key: Job key to filter on
+        :type key: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -2422,18 +2425,18 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ListJobsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._list_all_jobs_with_http_info(project_id, start_date, end_date, limit, offset, root_only, **kwargs)  # noqa: E501
+        return self._list_all_jobs_with_http_info(project_id, start_date, end_date, limit, offset, root_only, key, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _list_all_jobs_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, **kwargs):  # noqa: E501
+    def _list_all_jobs_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, key : Annotated[Optional[StrictStr], Field(description="Job key to filter on")] = None, **kwargs):  # noqa: E501
         """List all jobs 
 
         Get all jobs for this project
 
         :param project_id: Project ID (required)
         :type project_id: int
         :param start_date: Start date
@@ -2442,14 +2445,16 @@
         :type end_date: datetime
         :param limit: Maximum number of results
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
         :type offset: int
         :param root_only: Whether to exclude jobs with a parent ID (so jobs started as part of another job)
         :type root_only: bool
+        :param key: Job key to filter on
+        :type key: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -2474,15 +2479,16 @@
 
         _all_params = [
             'project_id',
             'start_date',
             'end_date',
             'limit',
             'offset',
-            'root_only'
+            'root_only',
+            'key'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -2517,14 +2523,16 @@
             _query_params.append(('endDate', _params['end_date']))
         if _params.get('limit') is not None:  # noqa: E501
             _query_params.append(('limit', _params['limit']))
         if _params.get('offset') is not None:  # noqa: E501
             _query_params.append(('offset', _params['offset']))
         if _params.get('root_only') is not None:  # noqa: E501
             _query_params.append(('rootOnly', _params['root_only']))
+        if _params.get('key') is not None:  # noqa: E501
+            _query_params.append(('key', _params['key']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -2998,21 +3006,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def start_classify_job(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs) -> StartJobResponse:  # noqa: E501
+    def start_classify_job(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_classify_job_request : Optional[StartClassifyJobRequest] = None, **kwargs) -> StartJobResponse:  # noqa: E501
         """Classify
 
         Classifies all items in the testing dataset against the current impulse. Updates are streamed over the websocket API.
 
         :param project_id: Project ID (required)
         :type project_id: int
+        :param start_classify_job_request:
+        :type start_classify_job_request: StartClassifyJobRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -3021,24 +3031,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: StartJobResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._start_classify_job_with_http_info(project_id, **kwargs)  # noqa: E501
+        return self._start_classify_job_with_http_info(project_id, start_classify_job_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _start_classify_job_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs):  # noqa: E501
+    def _start_classify_job_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], start_classify_job_request : Optional[StartClassifyJobRequest] = None, **kwargs):  # noqa: E501
         """Classify 
 
         Classifies all items in the testing dataset against the current impulse. Updates are streamed over the websocket API.
 
         :param project_id: Project ID (required)
         :type project_id: int
+        :param start_classify_job_request:
+        :type start_classify_job_request: StartClassifyJobRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -3058,15 +3070,16 @@
                  returns the request thread.
         :rtype: tuple(StartJobResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'project_id'
+            'project_id',
+            'start_classify_job_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -3101,19 +3114,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['start_classify_job_request']:
+            _body_params = _params['start_classify_job_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "StartJobResponse",
         }
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/learn_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/learn_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/login_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/login_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/metrics_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/optimization_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/optimization_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_blocks_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_blocks_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_create_project_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_create_project_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_data_campaigns_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_data_campaigns_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_jobs_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_jobs_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -907,15 +907,15 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_all_organization_jobs(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, exclude_pipeline_transform_jobs : Annotated[Optional[StrictBool], Field(description="Whether to exclude pipeline / transformation jobs")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, **kwargs) -> ListJobsResponse:  # noqa: E501
+    def list_all_organization_jobs(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, exclude_pipeline_transform_jobs : Annotated[Optional[StrictBool], Field(description="Whether to exclude pipeline / transformation jobs")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, key : Annotated[Optional[StrictStr], Field(description="Job key to filter on")] = None, **kwargs) -> ListJobsResponse:  # noqa: E501
         """List all jobs
 
         Get all jobs for this organization
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param start_date: Start date
@@ -926,14 +926,16 @@
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
         :type offset: int
         :param exclude_pipeline_transform_jobs: Whether to exclude pipeline / transformation jobs
         :type exclude_pipeline_transform_jobs: bool
         :param root_only: Whether to exclude jobs with a parent ID (so jobs started as part of another job)
         :type root_only: bool
+        :param key: Job key to filter on
+        :type key: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -942,18 +944,18 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ListJobsResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._list_all_organization_jobs_with_http_info(organization_id, start_date, end_date, limit, offset, exclude_pipeline_transform_jobs, root_only, **kwargs)  # noqa: E501
+        return self._list_all_organization_jobs_with_http_info(organization_id, start_date, end_date, limit, offset, exclude_pipeline_transform_jobs, root_only, key, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _list_all_organization_jobs_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, exclude_pipeline_transform_jobs : Annotated[Optional[StrictBool], Field(description="Whether to exclude pipeline / transformation jobs")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, **kwargs):  # noqa: E501
+    def _list_all_organization_jobs_with_http_info(self, organization_id : Annotated[StrictInt, Field(..., description="Organization ID")], start_date : Annotated[Optional[datetime], Field(description="Start date")] = None, end_date : Annotated[Optional[datetime], Field(description="End date")] = None, limit : Annotated[Optional[StrictInt], Field(description="Maximum number of results")] = None, offset : Annotated[Optional[StrictInt], Field(description="Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.")] = None, exclude_pipeline_transform_jobs : Annotated[Optional[StrictBool], Field(description="Whether to exclude pipeline / transformation jobs")] = None, root_only : Annotated[Optional[StrictBool], Field(description="Whether to exclude jobs with a parent ID (so jobs started as part of another job)")] = None, key : Annotated[Optional[StrictStr], Field(description="Job key to filter on")] = None, **kwargs):  # noqa: E501
         """List all jobs 
 
         Get all jobs for this organization
 
         :param organization_id: Organization ID (required)
         :type organization_id: int
         :param start_date: Start date
@@ -964,14 +966,16 @@
         :type limit: int
         :param offset: Offset in results, can be used in conjunction with LimitResultsParameter to implement paging.
         :type offset: int
         :param exclude_pipeline_transform_jobs: Whether to exclude pipeline / transformation jobs
         :type exclude_pipeline_transform_jobs: bool
         :param root_only: Whether to exclude jobs with a parent ID (so jobs started as part of another job)
         :type root_only: bool
+        :param key: Job key to filter on
+        :type key: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -997,15 +1001,16 @@
         _all_params = [
             'organization_id',
             'start_date',
             'end_date',
             'limit',
             'offset',
             'exclude_pipeline_transform_jobs',
-            'root_only'
+            'root_only',
+            'key'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1042,14 +1047,16 @@
             _query_params.append(('limit', _params['limit']))
         if _params.get('offset') is not None:  # noqa: E501
             _query_params.append(('offset', _params['offset']))
         if _params.get('exclude_pipeline_transform_jobs') is not None:  # noqa: E501
             _query_params.append(('excludePipelineTransformJobs', _params['exclude_pipeline_transform_jobs']))
         if _params.get('root_only') is not None:  # noqa: E501
             _query_params.append(('rootOnly', _params['root_only']))
+        if _params.get('key') is not None:  # noqa: E501
+            _query_params.append(('key', _params['key']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_pipelines_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_pipelines_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organization_portals_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organization_portals_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/organizations_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/performance_calibration_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/performance_calibration_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/projects_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/projects_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from edgeimpulse_api.models.add_project_api_key_request import AddProjectApiKeyRequest
 from edgeimpulse_api.models.create_project_request import CreateProjectRequest
 from edgeimpulse_api.models.create_project_response import CreateProjectResponse
 from edgeimpulse_api.models.development_boards_response import DevelopmentBoardsResponse
 from edgeimpulse_api.models.development_keys_response import DevelopmentKeysResponse
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_csv_wizard_uploaded_file_info import GetCsvWizardUploadedFileInfo
+from edgeimpulse_api.models.get_model_variants_response import GetModelVariantsResponse
 from edgeimpulse_api.models.get_notes_response import GetNotesResponse
 from edgeimpulse_api.models.get_target_constraints_response import GetTargetConstraintsResponse
 from edgeimpulse_api.models.last_modification_date_response import LastModificationDateResponse
 from edgeimpulse_api.models.list_api_keys_response import ListApiKeysResponse
 from edgeimpulse_api.models.list_email_response import ListEmailResponse
 from edgeimpulse_api.models.list_hmac_keys_response import ListHmacKeysResponse
 from edgeimpulse_api.models.list_projects_response import ListProjectsResponse
@@ -1312,14 +1313,147 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def get_model_variants(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs) -> GetModelVariantsResponse:  # noqa: E501
+        """Get a list of all model variants available for this project
+
+        Get a list of model variants applicable to all trained learn blocks in this project.
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GetModelVariantsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._get_model_variants_with_http_info(project_id, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _get_model_variants_with_http_info(self, project_id : Annotated[StrictInt, Field(..., description="Project ID")], **kwargs):  # noqa: E501
+        """Get a list of all model variants available for this project 
+
+        Get a list of model variants applicable to all trained learn blocks in this project.
+
+        :param project_id: Project ID (required)
+        :type project_id: int
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GetModelVariantsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'project_id'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_model_variants" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['project_id']:
+            _path_params['projectId'] = _params['project_id']
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GetModelVariantsResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/{projectId}/model-variants', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/raw_data_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/raw_data_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/themes_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/themes_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/third_party_auth_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/third_party_auth_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/upload_portal_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/upload_portal_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/user_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from edgeimpulse_api.models.convert_user_request import ConvertUserRequest
 from edgeimpulse_api.models.create_developer_profile_response import CreateDeveloperProfileResponse
 from edgeimpulse_api.models.create_enterprise_trial_response import CreateEnterpriseTrialResponse
 from edgeimpulse_api.models.create_enterprise_trial_user_request import CreateEnterpriseTrialUserRequest
 from edgeimpulse_api.models.create_evaluation_user_response import CreateEvaluationUserResponse
 from edgeimpulse_api.models.create_user_request import CreateUserRequest
 from edgeimpulse_api.models.create_user_response import CreateUserResponse
+from edgeimpulse_api.models.delete_user_request import DeleteUserRequest
 from edgeimpulse_api.models.enterprise_upgrade_or_trial_extension_request import EnterpriseUpgradeOrTrialExtensionRequest
 from edgeimpulse_api.models.generic_api_response import GenericApiResponse
 from edgeimpulse_api.models.get_jwt_response import GetJWTResponse
 from edgeimpulse_api.models.get_user_need_to_set_password_response import GetUserNeedToSetPasswordResponse
 from edgeimpulse_api.models.get_user_response import GetUserResponse
 from edgeimpulse_api.models.list_email_response import ListEmailResponse
 from edgeimpulse_api.models.list_enterprise_trials_response import ListEnterpriseTrialsResponse
@@ -40,21 +41,23 @@
 from edgeimpulse_api.models.list_organizations_response import ListOrganizationsResponse
 from edgeimpulse_api.models.request_reset_password_request import RequestResetPasswordRequest
 from edgeimpulse_api.models.reset_password_request import ResetPasswordRequest
 from edgeimpulse_api.models.send_user_feedback_request import SendUserFeedbackRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
+from edgeimpulse_api.models.upgrade_subscription_request import UpgradeSubscriptionRequest
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.user_delete_totp_mfa_key_request import UserDeleteTotpMfaKeyRequest
 from edgeimpulse_api.models.user_dismiss_notification_request import UserDismissNotificationRequest
 from edgeimpulse_api.models.user_generate_new_mfa_key_response import UserGenerateNewMfaKeyResponse
 from edgeimpulse_api.models.user_set_totp_mfa_key_request import UserSetTotpMfaKeyRequest
 from edgeimpulse_api.models.user_set_totp_mfa_key_response import UserSetTotpMfaKeyResponse
+from edgeimpulse_api.models.user_subscription_metrics_response import UserSubscriptionMetricsResponse
 from edgeimpulse_api.models.verify_reset_password_request import VerifyResetPasswordRequest
 
 from edgeimpulse_api.api_client import ApiClient
 from edgeimpulse_api.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -1575,19 +1578,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_current_user(self, **kwargs) -> GenericApiResponse:  # noqa: E501
+    def delete_current_user(self, delete_user_request : DeleteUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Delete current user
 
         Delete a user. This function is only available through a JWT token, and can only remove the current user.
 
+        :param delete_user_request: (required)
+        :type delete_user_request: DeleteUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -1596,22 +1601,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._delete_current_user_with_http_info(**kwargs)  # noqa: E501
+        return self._delete_current_user_with_http_info(delete_user_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _delete_current_user_with_http_info(self, **kwargs):  # noqa: E501
+    def _delete_current_user_with_http_info(self, delete_user_request : DeleteUserRequest, **kwargs):  # noqa: E501
         """Delete current user 
 
         Delete a user. This function is only available through a JWT token, and can only remove the current user.
 
+        :param delete_user_request: (required)
+        :type delete_user_request: DeleteUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1631,14 +1638,15 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'delete_user_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1671,19 +1679,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['delete_user_request']:
+            _body_params = _params['delete_user_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
@@ -1827,21 +1844,23 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs) -> GenericApiResponse:  # noqa: E501
+    def delete_user(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], delete_user_request : DeleteUserRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Delete user
 
         Delete a user. This function is only available through a JWT token, and can only remove the current user.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param delete_user_request: (required)
+        :type delete_user_request: DeleteUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -1850,24 +1869,26 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: GenericApiResponse
         """
         kwargs['_return_http_data_only'] = True
-        return self._delete_user_with_http_info(user_id, **kwargs)  # noqa: E501
+        return self._delete_user_with_http_info(user_id, delete_user_request, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def _delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], **kwargs):  # noqa: E501
+    def _delete_user_with_http_info(self, user_id : Annotated[StrictInt, Field(..., description="User ID")], delete_user_request : DeleteUserRequest, **kwargs):  # noqa: E501
         """Delete user 
 
         Delete a user. This function is only available through a JWT token, and can only remove the current user.
 
         :param user_id: User ID (required)
         :type user_id: int
+        :param delete_user_request: (required)
+        :type delete_user_request: DeleteUserRequest
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1887,15 +1908,16 @@
                  returns the request thread.
         :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'user_id'
+            'user_id',
+            'delete_user_request'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1930,19 +1952,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['delete_user_request']:
+            _body_params = _params['delete_user_request']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
 
         _response_types_map = {
             '200': "GenericApiResponse",
         }
 
@@ -5096,14 +5127,140 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def user_cancel_subscription(self, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Cancel subscription
+
+        Cancel the current subscription.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._user_cancel_subscription_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _user_cancel_subscription_with_http_info(self, **kwargs):  # noqa: E501
+        """Cancel subscription 
+
+        Cancel the current subscription.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method user_cancel_subscription" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/user/subscription/cancel', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def user_delete_totp_mfa_key(self, user_delete_totp_mfa_key_request : UserDeleteTotpMfaKeyRequest, **kwargs) -> GenericApiResponse:  # noqa: E501
         """Remove TOTP MFA key
 
         Disable MFA on this account using an TOTP token.
 
         :param user_delete_totp_mfa_key_request: (required)
         :type user_delete_totp_mfa_key_request: UserDeleteTotpMfaKeyRequest
@@ -5502,14 +5659,140 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def user_get_subscription_metrics(self, **kwargs) -> UserSubscriptionMetricsResponse:  # noqa: E501
+        """Get user billable compute metrics
+
+        Get billable compute metrics for a user. This function is only available to users with an active subscription.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: UserSubscriptionMetricsResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._user_get_subscription_metrics_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _user_get_subscription_metrics_with_http_info(self, **kwargs):  # noqa: E501
+        """Get user billable compute metrics 
+
+        Get billable compute metrics for a user. This function is only available to users with an active subscription.
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(UserSubscriptionMetricsResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method user_get_subscription_metrics" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "UserSubscriptionMetricsResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/user/subscription/metrics', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def user_set_totp_mfa_key(self, user_set_totp_mfa_key_request : UserSetTotpMfaKeyRequest, **kwargs) -> UserSetTotpMfaKeyResponse:  # noqa: E501
         """Set TOTP MFA key
 
         Enable MFA on this account using an TOTP token. First create a new key via `userGenerateNewTotpMfaKey`.
 
         :param user_set_totp_mfa_key_request: (required)
         :type user_set_totp_mfa_key_request: UserSetTotpMfaKeyRequest
@@ -5633,14 +5916,274 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def user_undo_cancel_subscription(self, **kwargs) -> GenericApiResponse:  # noqa: E501
+        """Undo subscription cancellation
+
+        Stop a pending cancellation. If you schedule a subscription to be canceled, and the subscription hasn't yet reached the end of the billing period, you can stop the cancellation. After a subscription has been canceled, you can't reactivate it. 
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: GenericApiResponse
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._user_undo_cancel_subscription_with_http_info(**kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _user_undo_cancel_subscription_with_http_info(self, **kwargs):  # noqa: E501
+        """Undo subscription cancellation 
+
+        Stop a pending cancellation. If you schedule a subscription to be canceled, and the subscription hasn't yet reached the end of the billing period, you can stop the cancellation. After a subscription has been canceled, you can't reactivate it. 
+
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(GenericApiResponse, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method user_undo_cancel_subscription" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {
+            '200': "GenericApiResponse",
+        }
+
+        return self.api_client.call_api(
+            '/api/user/subscription/undo-cancel', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
+    def user_upgrade_subscription(self, upgrade_subscription_request : UpgradeSubscriptionRequest, **kwargs) -> None:  # noqa: E501
+        """Upgrade subscription
+
+        Upgrade the current subscription.
+
+        :param upgrade_subscription_request: (required)
+        :type upgrade_subscription_request: UpgradeSubscriptionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self._user_upgrade_subscription_with_http_info(upgrade_subscription_request, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def _user_upgrade_subscription_with_http_info(self, upgrade_subscription_request : UpgradeSubscriptionRequest, **kwargs):  # noqa: E501
+        """Upgrade subscription 
+
+        Upgrade the current subscription.
+
+        :param upgrade_subscription_request: (required)
+        :type upgrade_subscription_request: UpgradeSubscriptionRequest
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'upgrade_subscription_request'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method user_upgrade_subscription" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['upgrade_subscription_request']:
+            _body_params = _params['upgrade_subscription_request']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['ApiKeyAuthentication', 'JWTAuthentication', 'JWTHttpHeaderAuthentication']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/user/subscription/upgrade', 'POST',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api/whitelabels_api.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api/whitelabels_api.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/api_client.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/api_client.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/configuration.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/configuration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/exceptions.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/__init__.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,32 +115,37 @@
 from edgeimpulse_api.models.anomaly_trained_features_response import AnomalyTrainedFeaturesResponse
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of import AnomalyTrainedFeaturesResponseAllOf
 from edgeimpulse_api.models.anomaly_trained_features_response_all_of_data import AnomalyTrainedFeaturesResponseAllOfData
 from edgeimpulse_api.models.application_budget import ApplicationBudget
 from edgeimpulse_api.models.augmentation_policy_image_enum import AugmentationPolicyImageEnum
 from edgeimpulse_api.models.augmentation_policy_spectrogram import AugmentationPolicySpectrogram
 from edgeimpulse_api.models.autotune_dsp_request import AutotuneDspRequest
+from edgeimpulse_api.models.billing_cycle import BillingCycle
 from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
 from edgeimpulse_api.models.block_type import BlockType
 from edgeimpulse_api.models.bounding_box import BoundingBox
 from edgeimpulse_api.models.bounding_box_with_score import BoundingBoxWithScore
 from edgeimpulse_api.models.build_on_device_model_request import BuildOnDeviceModelRequest
 from edgeimpulse_api.models.build_organization_on_device_model_request import BuildOrganizationOnDeviceModelRequest
 from edgeimpulse_api.models.calculate_data_quality_metrics_request import CalculateDataQualityMetricsRequest
 from edgeimpulse_api.models.change_password_request import ChangePasswordRequest
 from edgeimpulse_api.models.classify_job_response import ClassifyJobResponse
 from edgeimpulse_api.models.classify_job_response_all_of import ClassifyJobResponseAllOf
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy_total_summary import ClassifyJobResponseAllOfAccuracyTotalSummary
 from edgeimpulse_api.models.classify_job_response_page import ClassifyJobResponsePage
 from edgeimpulse_api.models.classify_job_response_page_all_of import ClassifyJobResponsePageAllOf
+from edgeimpulse_api.models.classify_sample_for_variants200_response import ClassifySampleForVariants200Response
 from edgeimpulse_api.models.classify_sample_response import ClassifySampleResponse
 from edgeimpulse_api.models.classify_sample_response_all_of import ClassifySampleResponseAllOf
 from edgeimpulse_api.models.classify_sample_response_classification import ClassifySampleResponseClassification
 from edgeimpulse_api.models.classify_sample_response_classification_details import ClassifySampleResponseClassificationDetails
+from edgeimpulse_api.models.classify_sample_response_multiple_variants import ClassifySampleResponseMultipleVariants
+from edgeimpulse_api.models.classify_sample_response_multiple_variants_all_of import ClassifySampleResponseMultipleVariantsAllOf
+from edgeimpulse_api.models.classify_sample_response_variant_results import ClassifySampleResponseVariantResults
 from edgeimpulse_api.models.classify_sample_v2200_response import ClassifySampleV2200Response
 from edgeimpulse_api.models.convert_user_request import ConvertUserRequest
 from edgeimpulse_api.models.cosine_similarity_data import CosineSimilarityData
 from edgeimpulse_api.models.cosine_similarity_issue import CosineSimilarityIssue
 from edgeimpulse_api.models.cosine_similarity_issue_issues_inner import CosineSimilarityIssueIssuesInner
 from edgeimpulse_api.models.cosine_similarity_issue_issues_inner_windows_inner import CosineSimilarityIssueIssuesInnerWindowsInner
 from edgeimpulse_api.models.count_samples_response import CountSamplesResponse
@@ -214,14 +219,15 @@
 from edgeimpulse_api.models.data_campaign_query import DataCampaignQuery
 from edgeimpulse_api.models.data_explorer_predictions_response import DataExplorerPredictionsResponse
 from edgeimpulse_api.models.data_explorer_predictions_response_all_of import DataExplorerPredictionsResponseAllOf
 from edgeimpulse_api.models.data_explorer_settings import DataExplorerSettings
 from edgeimpulse_api.models.dataset_ratio_data import DatasetRatioData
 from edgeimpulse_api.models.dataset_ratio_data_ratio import DatasetRatioDataRatio
 from edgeimpulse_api.models.delete_portal_file_request import DeletePortalFileRequest
+from edgeimpulse_api.models.delete_user_request import DeleteUserRequest
 from edgeimpulse_api.models.dependency_data import DependencyData
 from edgeimpulse_api.models.deploy_pretrained_model_input_audio import DeployPretrainedModelInputAudio
 from edgeimpulse_api.models.deploy_pretrained_model_input_image import DeployPretrainedModelInputImage
 from edgeimpulse_api.models.deploy_pretrained_model_input_other import DeployPretrainedModelInputOther
 from edgeimpulse_api.models.deploy_pretrained_model_input_time_series import DeployPretrainedModelInputTimeSeries
 from edgeimpulse_api.models.deploy_pretrained_model_model_classification import DeployPretrainedModelModelClassification
 from edgeimpulse_api.models.deploy_pretrained_model_model_object_detection import DeployPretrainedModelModelObjectDetection
@@ -354,14 +360,16 @@
 from edgeimpulse_api.models.get_job_response_all_of import GetJobResponseAllOf
 from edgeimpulse_api.models.get_label_noise_data_response import GetLabelNoiseDataResponse
 from edgeimpulse_api.models.get_label_noise_data_response_all_of import GetLabelNoiseDataResponseAllOf
 from edgeimpulse_api.models.get_label_noise_data_response_all_of_data import GetLabelNoiseDataResponseAllOfData
 from edgeimpulse_api.models.get_last_deployment_build_response import GetLastDeploymentBuildResponse
 from edgeimpulse_api.models.get_last_deployment_build_response_all_of import GetLastDeploymentBuildResponseAllOf
 from edgeimpulse_api.models.get_last_deployment_build_response_all_of_last_build import GetLastDeploymentBuildResponseAllOfLastBuild
+from edgeimpulse_api.models.get_model_variants_response import GetModelVariantsResponse
+from edgeimpulse_api.models.get_model_variants_response_all_of import GetModelVariantsResponseAllOf
 from edgeimpulse_api.models.get_notes_response import GetNotesResponse
 from edgeimpulse_api.models.get_notes_response_all_of import GetNotesResponseAllOf
 from edgeimpulse_api.models.get_organization_bucket_response import GetOrganizationBucketResponse
 from edgeimpulse_api.models.get_organization_bucket_response_all_of import GetOrganizationBucketResponseAllOf
 from edgeimpulse_api.models.get_organization_data_campaign_dashboard_response import GetOrganizationDataCampaignDashboardResponse
 from edgeimpulse_api.models.get_organization_data_campaign_dashboard_response_all_of import GetOrganizationDataCampaignDashboardResponseAllOf
 from edgeimpulse_api.models.get_organization_data_campaign_dashboards_response import GetOrganizationDataCampaignDashboardsResponse
@@ -721,26 +729,28 @@
 from edgeimpulse_api.models.project_info_response_all_of_impulse import ProjectInfoResponseAllOfImpulse
 from edgeimpulse_api.models.project_info_response_all_of_performance import ProjectInfoResponseAllOfPerformance
 from edgeimpulse_api.models.project_info_response_all_of_readme import ProjectInfoResponseAllOfReadme
 from edgeimpulse_api.models.project_info_response_all_of_show_getting_started_wizard import ProjectInfoResponseAllOfShowGettingStartedWizard
 from edgeimpulse_api.models.project_info_response_all_of_urls import ProjectInfoResponseAllOfUrls
 from edgeimpulse_api.models.project_info_summary_response import ProjectInfoSummaryResponse
 from edgeimpulse_api.models.project_info_summary_response_all_of import ProjectInfoSummaryResponseAllOf
+from edgeimpulse_api.models.project_model_variant import ProjectModelVariant
 from edgeimpulse_api.models.project_private_data import ProjectPrivateData
 from edgeimpulse_api.models.project_public_data import ProjectPublicData
 from edgeimpulse_api.models.project_public_data_readme import ProjectPublicDataReadme
 from edgeimpulse_api.models.project_sample_metadata import ProjectSampleMetadata
 from edgeimpulse_api.models.project_tier_enum import ProjectTierEnum
 from edgeimpulse_api.models.project_training_data_summary_response import ProjectTrainingDataSummaryResponse
 from edgeimpulse_api.models.project_training_data_summary_response_all_of import ProjectTrainingDataSummaryResponseAllOf
 from edgeimpulse_api.models.project_training_data_summary_response_all_of_data_summary import ProjectTrainingDataSummaryResponseAllOfDataSummary
 from edgeimpulse_api.models.project_type import ProjectType
 from edgeimpulse_api.models.project_version_request import ProjectVersionRequest
 from edgeimpulse_api.models.project_visibility import ProjectVisibility
 from edgeimpulse_api.models.public_organization_transformation_block import PublicOrganizationTransformationBlock
+from edgeimpulse_api.models.public_project_tier_availability import PublicProjectTierAvailability
 from edgeimpulse_api.models.raw_sample_data import RawSampleData
 from edgeimpulse_api.models.raw_sample_payload import RawSamplePayload
 from edgeimpulse_api.models.rebalance_dataset_response import RebalanceDatasetResponse
 from edgeimpulse_api.models.remove_collaborator_request import RemoveCollaboratorRequest
 from edgeimpulse_api.models.remove_member_request import RemoveMemberRequest
 from edgeimpulse_api.models.rename_device_request import RenameDeviceRequest
 from edgeimpulse_api.models.rename_portal_file_request import RenamePortalFileRequest
@@ -784,14 +794,15 @@
 from edgeimpulse_api.models.set_syntiant_posterior_request import SetSyntiantPosteriorRequest
 from edgeimpulse_api.models.set_user_password_request import SetUserPasswordRequest
 from edgeimpulse_api.models.socket_token_response import SocketTokenResponse
 from edgeimpulse_api.models.socket_token_response_all_of import SocketTokenResponseAllOf
 from edgeimpulse_api.models.socket_token_response_all_of_token import SocketTokenResponseAllOfToken
 from edgeimpulse_api.models.split_sample_in_frames_request import SplitSampleInFramesRequest
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.start_classify_job_request import StartClassifyJobRequest
 from edgeimpulse_api.models.start_device_debug_stream_response import StartDeviceDebugStreamResponse
 from edgeimpulse_api.models.start_device_debug_stream_response_all_of import StartDeviceDebugStreamResponseAllOf
 from edgeimpulse_api.models.start_device_snapshot_debug_stream_request import StartDeviceSnapshotDebugStreamRequest
 from edgeimpulse_api.models.start_enterprise_trial_request import StartEnterpriseTrialRequest
 from edgeimpulse_api.models.start_job_response import StartJobResponse
 from edgeimpulse_api.models.start_job_response_all_of import StartJobResponseAllOf
 from edgeimpulse_api.models.start_performance_calibration_request import StartPerformanceCalibrationRequest
@@ -856,30 +867,35 @@
 from edgeimpulse_api.models.update_user_request import UpdateUserRequest
 from edgeimpulse_api.models.update_version_request import UpdateVersionRequest
 from edgeimpulse_api.models.update_whitelabel_default_deployment_target_request import UpdateWhitelabelDefaultDeploymentTargetRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_options_order_request import UpdateWhitelabelDeploymentOptionsOrderRequest
 from edgeimpulse_api.models.update_whitelabel_deployment_targets_request import UpdateWhitelabelDeploymentTargetsRequest
 from edgeimpulse_api.models.update_whitelabel_learning_blocks_request import UpdateWhitelabelLearningBlocksRequest
 from edgeimpulse_api.models.update_whitelabel_request import UpdateWhitelabelRequest
+from edgeimpulse_api.models.upgrade_subscription_request import UpgradeSubscriptionRequest
 from edgeimpulse_api.models.upload_asset_response import UploadAssetResponse
 from edgeimpulse_api.models.upload_asset_response_all_of import UploadAssetResponseAllOf
 from edgeimpulse_api.models.upload_readme_image_response import UploadReadmeImageResponse
 from edgeimpulse_api.models.upload_user_photo_response import UploadUserPhotoResponse
 from edgeimpulse_api.models.upload_user_photo_response_all_of import UploadUserPhotoResponseAllOf
 from edgeimpulse_api.models.user import User
 from edgeimpulse_api.models.user_by_third_party_activation_request import UserByThirdPartyActivationRequest
 from edgeimpulse_api.models.user_delete_totp_mfa_key_request import UserDeleteTotpMfaKeyRequest
 from edgeimpulse_api.models.user_dismiss_notification_request import UserDismissNotificationRequest
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_generate_new_mfa_key_response import UserGenerateNewMfaKeyResponse
 from edgeimpulse_api.models.user_generate_new_mfa_key_response_all_of import UserGenerateNewMfaKeyResponseAllOf
 from edgeimpulse_api.models.user_organization import UserOrganization
+from edgeimpulse_api.models.user_projects_sort_order import UserProjectsSortOrder
 from edgeimpulse_api.models.user_set_totp_mfa_key_request import UserSetTotpMfaKeyRequest
 from edgeimpulse_api.models.user_set_totp_mfa_key_response import UserSetTotpMfaKeyResponse
 from edgeimpulse_api.models.user_set_totp_mfa_key_response_all_of import UserSetTotpMfaKeyResponseAllOf
+from edgeimpulse_api.models.user_subscription_metrics_response import UserSubscriptionMetricsResponse
+from edgeimpulse_api.models.user_subscription_metrics_response_all_of import UserSubscriptionMetricsResponseAllOf
+from edgeimpulse_api.models.user_subscription_metrics_response_all_of_metrics import UserSubscriptionMetricsResponseAllOfMetrics
 from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 from edgeimpulse_api.models.verify_dsp_block_url_request import VerifyDspBlockUrlRequest
 from edgeimpulse_api.models.verify_dsp_block_url_response import VerifyDspBlockUrlResponse
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of import VerifyDspBlockUrlResponseAllOf
 from edgeimpulse_api.models.verify_dsp_block_url_response_all_of_block import VerifyDspBlockUrlResponseAllOfBlock
 from edgeimpulse_api.models.verify_email_response import VerifyEmailResponse
 from edgeimpulse_api.models.verify_email_response_all_of import VerifyEmailResponseAllOf
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/activate_user_by_third_party_activation_code_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/activate_user_or_verify_email_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/activate_user_or_verify_email_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_api_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_collaborator_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_hmac_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_hmac_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_member_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_api_key_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_bucket_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_data_campaign_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_deploy_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_dsp_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_secret_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_secret_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transfer_learning_block_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 from edgeimpulse_api.models.organization_transfer_learning_operates_on import OrganizationTransferLearningOperatesOn
+from edgeimpulse_api.models.public_project_tier_availability import PublicProjectTierAvailability
 
 class AddOrganizationTransferLearningBlockRequest(BaseModel):
     name: StrictStr = ...
     docker_container: StrictStr = Field(..., alias="dockerContainer")
     description: StrictStr = ...
     operates_on: OrganizationTransferLearningOperatesOn = Field(..., alias="operatesOn")
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: StrictInt = Field(..., alias="implementationVersion")
     is_public: Optional[StrictBool] = Field(None, alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: Optional[List[StrictStr]] = Field(None, alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
-    is_public_enterprise_only: Optional[StrictBool] = Field(None, alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
+    public_project_tier_availability: Optional[PublicProjectTierAvailability] = Field(None, alias="publicProjectTierAvailability")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: Optional[List[Dict[str, Any]]] = Field(None, description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
     ind_requires_gpu: Optional[StrictBool] = Field(None, alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
-    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "isPublicEnterpriseOnly", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu"]
+    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "publicProjectTierAvailability", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -78,15 +79,15 @@
             "docker_container": obj.get("dockerContainer"),
             "description": obj.get("description"),
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
-            "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
+            "public_project_tier_availability": obj.get("publicProjectTierAvailability"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
             "image_input_scaling": obj.get("imageInputScaling"),
             "ind_requires_gpu": obj.get("indRequiresGpu")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_disallowed_email_domain_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_or_update_sso_domain_id_ps_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_api_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_organization_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_api_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_api_key_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_project_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_project_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_add_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_add_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_organization.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 from edgeimpulse_api.models.project import Project
 
 class AdminApiOrganization(BaseModel):
     id: StrictInt = ...
     name: StrictStr = Field(..., description="EdgeImpulse Inc.")
     logo: Optional[StrictStr] = None
     header_img: Optional[StrictStr] = Field(None, alias="headerImg")
+    show_header_img_mask: StrictBool = Field(..., alias="showHeaderImgMask")
     users: List[OrganizationUser] = ...
     is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
     whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this organization belongs to, if any.")
     projects: List[Project] = Field(..., description="Array with organizational projects")
     trial_id: Optional[StrictInt] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
     trial_expired_date: Optional[datetime] = Field(..., alias="trialExpiredDate", description="Date when the trial expired, if any. A expired trial has a grace period of 30 days before it's associated organization is deleted.")
     trial_upgraded_date: Optional[datetime] = Field(..., alias="trialUpgradedDate", description="Date when the trial was upgraded to a full enterprise account, if any.")
     created: datetime = Field(..., description="Date when the organization was created.")
     contract_start_date: Optional[datetime] = Field(None, alias="contractStartDate", description="Date when the current contract started, if any.")
     deleted_date: Optional[datetime] = Field(None, alias="deletedDate", description="The date in which the organization was deleted. If the organization is not deleted, this field is not set.")
-    __properties = ["id", "name", "logo", "headerImg", "users", "isDeveloperProfile", "whitelabelId", "projects", "trialId", "trialExpiredDate", "trialUpgradedDate", "created", "contractStartDate", "deletedDate"]
+    __properties = ["id", "name", "logo", "headerImg", "showHeaderImgMask", "users", "isDeveloperProfile", "whitelabelId", "projects", "trialId", "trialExpiredDate", "trialUpgradedDate", "created", "contractStartDate", "deletedDate"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -108,14 +109,15 @@
             return AdminApiOrganization.construct(**obj)
 
         _obj = AdminApiOrganization.construct(**{
             "id": obj.get("id"),
             "name": obj.get("name"),
             "logo": obj.get("logo"),
             "header_img": obj.get("headerImg"),
+            "show_header_img_mask": obj.get("showHeaderImgMask"),
             "users": [OrganizationUser.from_dict(_item) for _item in obj.get("users")] if obj.get("users") is not None else None,
             "is_developer_profile": obj.get("isDeveloperProfile"),
             "whitelabel_id": obj.get("whitelabelId"),
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "trial_id": obj.get("trialId"),
             "trial_expired_date": obj.get("trialExpiredDate"),
             "trial_upgraded_date": obj.get("trialUpgradedDate"),
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_organization_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_organization_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_project.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,23 +41,23 @@
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = ...
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
     stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
     has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    tier: UserTierEnum = ...
     organizations: List[UserOrganization] = Field(..., description="Organizations that the user is a member of. Only filled when requesting information about yourself.")
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
-    tier: UserTierEnum = ...
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
     trials: List[EnterpriseTrial] = Field(..., description="Current or past enterprise trials.")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "suspended", "trials"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier", "organizations", "projects", "experiments", "evaluation", "ambassador", "suspended", "trials"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -134,18 +134,18 @@
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
             "stripe_customer_id": obj.get("stripeCustomerId"),
             "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier"),
             "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
-            "tier": obj.get("tier"),
             "suspended": obj.get("suspended"),
             "trials": [EnterpriseTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_api_user_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_api_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_data_export_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_create_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_enable_feature_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_enable_feature_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migration_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migration_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migrations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_data_migrations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_disallowed_email_domains_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_metrics_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_compute_time_usage_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_report_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_organizations_response_all_of_organizations.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_domain_id_ps_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_sso_settings_response_all_of_sso_whitelist.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_ids_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_ids_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_metrics_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_user_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_get_users_response_all_of_users.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_get_users_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_list_projects_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_organization_info_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_toggle_data_migration_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_toggle_data_migration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_data_export_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_organization_data_export_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_permissions_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_permissions_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/admin_update_user_trial_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/admin_update_user_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/akida_edge_learning_config.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/akida_edge_learning_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_capacity.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_capacity.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_gmm_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_gmm_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_model_metadata_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_response_all_of_axes.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_response_all_of_axes.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_result.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/anomaly_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/application_budget.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/application_budget.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/augmentation_policy_spectrogram.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/augmentation_policy_spectrogram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/autotune_dsp_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/autotune_dsp_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/block_type.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_variant_enum.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,17 +15,16 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class BlockType(str, Enum):
+class KerasModelVariantEnum(str, Enum):
     """
     allowed enum values
     """
 
-    OFFICIAL = 'official'
-    PERSONAL = 'personal'
-    ENTERPRISE = 'enterprise'
-    COMMUNITY = 'community'
+    INT8 = 'int8'
+    FLOAT32 = 'float32'
+    AKIDA = 'akida'
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/bounding_box.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/bounding_box_with_score.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/bounding_box_with_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_on_device_model_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/build_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/build_organization_on_device_model_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/build_organization_on_device_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/calculate_data_quality_metrics_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/calculate_data_quality_metrics_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/change_password_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/change_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,24 +16,26 @@
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
+from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.model_prediction import ModelPrediction
 from edgeimpulse_api.models.model_result import ModelResult
 
 class ClassifyJobResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
     result: List[ModelResult] = ...
     predictions: List[ModelPrediction] = ...
     accuracy: ClassifyJobResponseAllOfAccuracy = ...
-    __properties = ["success", "error", "result", "predictions", "accuracy"]
+    available_variants: List[KerasModelVariantEnum] = Field(..., alias="availableVariants", description="List of all model variants for which classification results exist")
+    __properties = ["success", "error", "result", "predictions", "accuracy", "availableVariants"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -83,11 +85,12 @@
             return ClassifyJobResponse.construct(**obj)
 
         _obj = ClassifyJobResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "result": [ModelResult.from_dict(_item) for _item in obj.get("result")] if obj.get("result") is not None else None,
             "predictions": [ModelPrediction.from_dict(_item) for _item in obj.get("predictions")] if obj.get("predictions") is not None else None,
-            "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None
+            "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None,
+            "available_variants": obj.get("availableVariants")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,26 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 from edgeimpulse_api.models.classify_job_response_all_of_accuracy import ClassifyJobResponseAllOfAccuracy
+from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.model_prediction import ModelPrediction
 from edgeimpulse_api.models.model_result import ModelResult
 
 class ClassifyJobResponseAllOf(BaseModel):
     result: List[ModelResult] = ...
     predictions: List[ModelPrediction] = ...
     accuracy: ClassifyJobResponseAllOfAccuracy = ...
-    __properties = ["result", "predictions", "accuracy"]
+    available_variants: List[KerasModelVariantEnum] = Field(..., alias="availableVariants", description="List of all model variants for which classification results exist")
+    __properties = ["result", "predictions", "accuracy", "availableVariants"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -79,11 +81,12 @@
 
         if type(obj) is not dict:
             return ClassifyJobResponseAllOf.construct(**obj)
 
         _obj = ClassifyJobResponseAllOf.construct(**{
             "result": [ModelResult.from_dict(_item) for _item in obj.get("result")] if obj.get("result") is not None else None,
             "predictions": [ModelPrediction.from_dict(_item) for _item in obj.get("predictions")] if obj.get("predictions") is not None else None,
-            "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None
+            "accuracy": ClassifyJobResponseAllOfAccuracy.from_dict(obj.get("accuracy")) if obj.get("accuracy") is not None else None,
+            "available_variants": obj.get("availableVariants")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_all_of_accuracy_total_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_page.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_job_response_page_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_job_response_page_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_response_classification_details.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_response_classification_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/classify_sample_v2200_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/classify_sample_v2200_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/convert_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/convert_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue_issues_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cosine_similarity_issue_issues_inner_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/count_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/count_samples_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/count_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_block_version_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_block_version_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_block_version_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_developer_profile_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_developer_profile_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_developer_profile_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_device_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_user_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_enterprise_trial_user_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_evaluation_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_evaluation_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_evaluation_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_organization_usage_report_body.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_organization_usage_report_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_pipeline_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_project_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_signed_upload_link_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     privacy_policy: StrictBool = Field(..., alias="privacyPolicy", description="Whether the user accepted the privacy policy")
     activation_token: Optional[StrictStr] = Field(None, alias="activationToken", description="Activation token for users created via SSO")
     identity_provider: Optional[StrictStr] = Field(None, alias="identityProvider", description="Unique identifier of the identity provider asserting the identity of this user")
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="Job title of the user. Optional field")
     session_id: Optional[StrictStr] = Field(None, alias="sessionId", description="Session ID. Optional field")
     company_name: Optional[StrictStr] = Field(None, alias="companyName", description="ACME Inc.")
     utm_params: Optional[List[Dict[str, Any]]] = Field(None, alias="utmParams", description="List of UTM parameters.")
-    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName", "utmParams"]
+    no_activation_email: Optional[StrictBool] = Field(None, alias="noActivationEmail", description="If set, no welcome email will be sent for account activation")
+    __properties = ["name", "username", "email", "password", "projectName", "privacyPolicy", "activationToken", "identityProvider", "jobTitle", "sessionId", "companyName", "utmParams", "noActivationEmail"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -77,11 +78,12 @@
             "project_name": obj.get("projectName"),
             "privacy_policy": obj.get("privacyPolicy"),
             "activation_token": obj.get("activationToken"),
             "identity_provider": obj.get("identityProvider"),
             "job_title": obj.get("jobTitle"),
             "session_id": obj.get("sessionId"),
             "company_name": obj.get("companyName"),
-            "utm_params": obj.get("utmParams")
+            "utm_params": obj.get("utmParams"),
+            "no_activation_email": obj.get("noActivationEmail")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_user_third_party_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_user_third_party_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/create_whitelabel_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/create_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/created_updated_by_user.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/created_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/crop_sample_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/crop_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cross_validation_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/cross_validation_data_scores_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/cross_validation_data_scores_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_dashboard.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_dashboard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_graph_x_data_inner_values_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_link.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_link.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_campaign_query.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_campaign_query.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_predictions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_predictions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/data_explorer_settings.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/data_explorer_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dataset_ratio_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dataset_ratio_data_ratio.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dataset_ratio_data_ratio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/delete_portal_file_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/delete_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dependency_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dependency_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_audio.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_image.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_image.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_other.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_other.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_input_time_series.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_classification.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_object_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_model_regression.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deploy_pretrained_model_request_model_info_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_badge.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target_badge.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_target_engine.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_target_engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -30,8 +30,9 @@
     TENSORRT = 'tensorrt'
     TENSAIFLOW = 'tensaiflow'
     DRP_AI = 'drp-ai'
     TIDL = 'tidl'
     AKIDA = 'akida'
     SYNTIANT = 'syntiant'
     MEMRYX = 'memryx'
+    NEOX = 'neox'
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/deployment_targets_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_created_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_request_update.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_request_update.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_board_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_board_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_boards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_boards_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_boards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/development_keys_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/development_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_debug_stream_type.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_debug_stream_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_inference_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_inference_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_name_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_name_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_name_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/device_sensors_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/device_sensors_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/download.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/download_portal_file_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/download_portal_file_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_autotuner_results_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_config_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_importance_response_all_of_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_labels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_feature_labels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_select_options_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item_select_options_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_group_item_show_if.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_group_item_show_if.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_features.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_info_performance.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_info_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_included_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_output_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_output_config_shape.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_output_config_shape.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_metadata_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_named_axis.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_named_axis.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_performance_all_variants_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_graph.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_graph_axis_labels.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_graph_axis_labels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_with_features.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_with_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_without_features.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_request_without_features_read_only.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_all_of_performance.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_with_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_run_response_with_sample_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_sample_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/dsp_trained_features_response_all_of_sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/edit_sample_label_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/edit_sample_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_trial.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/enterprise_trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from datetime import datetime
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
 class EnterpriseTrial(BaseModel):
     id: StrictInt = Field(..., description="Unique identifier of the trial.")
     user_id: Optional[StrictInt] = Field(None, alias="userId", description="ID of the user who created the trial.")
-    organization_id: Optional[StrictInt] = Field(None, alias="organizationId", description="ID of the organization created for the trial.")
+    organization_id: StrictInt = Field(..., alias="organizationId", description="ID of the organization created for the trial.")
     created: datetime = Field(..., description="Date when the trial was created. Trials start immediately on creation.")
     expiration_date: datetime = Field(..., alias="expirationDate", description="Expiration date of the trial. The trial will be set as expired after this date. There will be a grace period of 30 days after a trial expires before fully deleting the trial organization. This field is ignored if the trial is requested by a non-admin user, defaulting to 14 days trial.")
     notes: Optional[StrictStr] = Field(None, description="Notes about the trial. Free form text. This field is ignored if the trial is requested by a non-admin user.")
     expired_date: Optional[datetime] = Field(..., alias="expiredDate", description="Date when the trial actually expired. This is set when the trial is expired by the system.")
     deleted_date: Optional[datetime] = Field(..., alias="deletedDate", description="Date when the trial was deleted. This is set when the trial is fully  deleted by the system.")
     upgraded_date: Optional[datetime] = Field(..., alias="upgradedDate", description="Date when the trial was upgraded to a full enterprise account.")
     __properties = ["id", "userId", "organizationId", "created", "expirationDate", "notes", "expiredDate", "deletedDate", "upgradedDate"]
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/enterprise_upgrade_or_trial_extension_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entitlement_limits.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/entitlement_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/entity_created_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/entity_created_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/entity_created_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_job_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/evaluate_result_value.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/evaluate_result_value.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_get_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_get_url_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_get_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_keras_block_data_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_keras_block_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_original_data_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_original_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/export_wav_data_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/export_wav_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_segment_sample_response_all_of_segments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/find_user_response_all_of_users.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/find_user_response_all_of_users.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/generate_features_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/generate_features_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/generic_api_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/generic_api_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_imported_from_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_whitelabels_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_all_whitelabels_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of_clusters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_auto_labeler_response_all_of_items.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_csv_wizard_uploaded_file_info_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_data_explorer_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_deployment_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_deployment_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_deployment_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_device_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_device_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_device_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of_cluster_infos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_diversity_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_code_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_code_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_code_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_email_verification_status_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_email_verification_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_feature_flags_response_all_of_flags.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_records_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_records_request_range.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_records_request_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_impulse_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_impulse_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_job_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_jwt_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_jwt_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_label_noise_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_last_deployment_build_response_all_of_last_build.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_notes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_notes_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_notes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboard_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_dashboards_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaign_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaign_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_campaigns_response_all_of_campaigns.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_export_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_export_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_export_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_exports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_exports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_data_item_transform_jobs_response_all_of_transformation_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dataset_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dataset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_deploy_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_deploy_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dsp_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_dsp_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_projects_data_count_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_projects_data_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transfer_learning_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transfer_learning_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transformation_block_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_transformation_block_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_organization_usage_report_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_organization_usage_report_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_ground_truth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameter_sets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_raw_result_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_performance_calibration_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_pretrained_model_response_all_of_model_profile_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_public_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_public_metrics_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_public_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_metadata_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_sample_metadata_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_sample_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_sample_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_syntiant_posterior_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_syntiant_posterior_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_target_constraints_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_target_constraints_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_target_constraints_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_theme_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_theme_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_theme_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_themes_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_themes_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_themes_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_third_party_auth_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_third_party_auth_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_third_party_auth_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_need_to_set_password_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_need_to_set_password_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_response.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
+from edgeimpulse_api.models.enterprise_trial import EnterpriseTrial
 from edgeimpulse_api.models.get_user_response_all_of_whitelabels import GetUserResponseAllOfWhitelabels
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.project import Project
 from edgeimpulse_api.models.staff_info import StaffInfo
 from edgeimpulse_api.models.user_experiment import UserExperiment
 from edgeimpulse_api.models.user_organization import UserOrganization
+from edgeimpulse_api.models.user_projects_sort_order import UserProjectsSortOrder
 from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 
 class GetUserResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
     id: StrictInt = ...
     username: StrictStr = ...
@@ -43,24 +45,30 @@
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = ...
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
     stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
     has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    tier: UserTierEnum = ...
     organizations: List[UserOrganization] = Field(..., description="Organizations that the user is a member of. Only filled when requesting information about yourself.")
     projects: List[Project] = ...
     experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
     evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
     ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
-    tier: UserTierEnum = ...
     whitelabels: Optional[List[GetUserResponseAllOfWhitelabels]] = Field(None, description="List of white labels the user is a member of")
     suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    notifications: List[StrictStr] = Field(..., description="List of notifications to show to the user")
-    __properties = ["success", "error", "id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "whitelabels", "suspended", "notifications"]
+    notifications: List[StrictStr] = Field(..., description="List of notifications to show to the user.")
+    subscription_downgrade_date: Optional[datetime] = Field(None, alias="subscriptionDowngradeDate", description="The date at which the user's subscription will be downgraded due to cancellation.")
+    subscription_termination_date: Optional[datetime] = Field(None, alias="subscriptionTerminationDate", description="The date at which the user's subscription will be automatically terminated due to failed payments.")
+    password_configured: StrictBool = Field(..., alias="passwordConfigured", description="Whether the user has configured a password")
+    projects_sort_order: UserProjectsSortOrder = Field(..., alias="projectsSortOrder")
+    active_enterprise_trial: Optional[EnterpriseTrial] = Field(None, alias="activeEnterpriseTrial")
+    has_enterprise_features_access: StrictBool = Field(..., alias="hasEnterpriseFeaturesAccess", description="Whether the current user has access to enterprise features. This is true if the user is an enterprise user, or has an active enterprise trial.")
+    __properties = ["success", "error", "id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier", "organizations", "projects", "experiments", "evaluation", "ambassador", "whitelabels", "suspended", "notifications", "subscriptionDowngradeDate", "subscriptionTerminationDate", "passwordConfigured", "projectsSortOrder", "activeEnterpriseTrial", "hasEnterpriseFeaturesAccess"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -108,14 +116,17 @@
         # override the default output from pydantic by calling `to_dict()` of each item in whitelabels (list)
         _items = []
         if self.whitelabels:
             for _item in self.whitelabels:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['whitelabels'] = _items
+        # override the default output from pydantic by calling `to_dict()` of active_enterprise_trial
+        if self.active_enterprise_trial:
+            _dict['activeEnterpriseTrial'] = self.active_enterprise_trial.to_dict()
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> GetUserResponse:
         """Create an instance of GetUserResponse from a dict"""
         if obj is None:
             return None
@@ -139,19 +150,25 @@
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
             "stripe_customer_id": obj.get("stripeCustomerId"),
             "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier"),
             "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
             "evaluation": obj.get("evaluation"),
             "ambassador": obj.get("ambassador"),
-            "tier": obj.get("tier"),
             "whitelabels": [GetUserResponseAllOfWhitelabels.from_dict(_item) for _item in obj.get("whitelabels")] if obj.get("whitelabels") is not None else None,
             "suspended": obj.get("suspended"),
-            "notifications": obj.get("notifications")
+            "notifications": obj.get("notifications"),
+            "subscription_downgrade_date": obj.get("subscriptionDowngradeDate"),
+            "subscription_termination_date": obj.get("subscriptionTerminationDate"),
+            "password_configured": obj.get("passwordConfigured"),
+            "projects_sort_order": obj.get("projectsSortOrder"),
+            "active_enterprise_trial": EnterpriseTrial.from_dict(obj.get("activeEnterpriseTrial")) if obj.get("activeEnterpriseTrial") is not None else None,
+            "has_enterprise_features_access": obj.get("hasEnterpriseFeaturesAccess")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,107 +12,103 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-
+from datetime import datetime
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
-from edgeimpulse_api.models.get_user_response_all_of_whitelabels import GetUserResponseAllOfWhitelabels
-from edgeimpulse_api.models.project import Project
-from edgeimpulse_api.models.user_experiment import UserExperiment
-from edgeimpulse_api.models.user_organization import UserOrganization
-from edgeimpulse_api.models.user_tier_enum import UserTierEnum
-
-class GetUserResponseAllOf(BaseModel):
-    email: StrictStr = ...
-    activated: StrictBool = ...
-    organizations: List[UserOrganization] = Field(..., description="Organizations that the user is a member of. Only filled when requesting information about yourself.")
-    projects: List[Project] = ...
-    experiments: List[UserExperiment] = Field(..., description="Experiments the user has access to. Enabling experiments can only be done through a JWT token.")
-    evaluation: Optional[StrictBool] = Field(None, description="Whether this is an ephemeral evaluation account.")
-    ambassador: Optional[StrictBool] = Field(None, description="Whether this user is an ambassador.")
-    tier: UserTierEnum = ...
-    whitelabels: Optional[List[GetUserResponseAllOfWhitelabels]] = Field(None, description="List of white labels the user is a member of")
-    suspended: StrictBool = Field(..., description="Whether the user is suspended.")
-    notifications: List[StrictStr] = Field(..., description="List of notifications to show to the user")
-    __properties = ["email", "activated", "organizations", "projects", "experiments", "evaluation", "ambassador", "tier", "whitelabels", "suspended", "notifications"]
+from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
+from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
+from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
+from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
+from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
+from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
+
+class KerasModelMetadata(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    created: datetime = Field(..., description="Date when the model was trained")
+    layers: List[KerasModelLayer] = Field(..., description="Layers of the neural network")
+    class_names: List[StrictStr] = Field(..., alias="classNames", description="Labels for the output layer")
+    labels: List[StrictStr] = Field(..., description="Original labels in the dataset when features were generated, e.g. used to render the feature explorer.")
+    available_model_types: List[KerasModelTypeEnum] = Field(..., alias="availableModelTypes", description="The types of model that are available")
+    recommended_model_type: KerasModelTypeEnum = Field(..., alias="recommendedModelType")
+    model_validation_metrics: List[KerasModelMetadataMetrics] = Field(..., alias="modelValidationMetrics", description="Metrics for each of the available model types")
+    has_trained_model: StrictBool = Field(..., alias="hasTrainedModel")
+    mode: StrictStr = ...
+    object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
+    image_input_scaling: ImageInputScaling = Field(..., alias="imageInputScaling")
+    __properties = ["success", "error", "created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+
+    @validator('mode')
+    def mode_validate_enum(cls, v):
+        if v not in ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm'):
+            raise ValueError("must validate the enum values ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm')")
+        return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> GetUserResponseAllOf:
-        """Create an instance of GetUserResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasModelMetadata:
+        """Create an instance of KerasModelMetadata from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in organizations (list)
-        _items = []
-        if self.organizations:
-            for _item in self.organizations:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['organizations'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in projects (list)
-        _items = []
-        if self.projects:
-            for _item in self.projects:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['projects'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in experiments (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in layers (list)
         _items = []
-        if self.experiments:
-            for _item in self.experiments:
+        if self.layers:
+            for _item in self.layers:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['experiments'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in whitelabels (list)
+            _dict['layers'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in model_validation_metrics (list)
         _items = []
-        if self.whitelabels:
-            for _item in self.whitelabels:
+        if self.model_validation_metrics:
+            for _item in self.model_validation_metrics:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['whitelabels'] = _items
+            _dict['modelValidationMetrics'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> GetUserResponseAllOf:
-        """Create an instance of GetUserResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> KerasModelMetadata:
+        """Create an instance of KerasModelMetadata from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return GetUserResponseAllOf.construct(**obj)
+            return KerasModelMetadata.construct(**obj)
 
-        _obj = GetUserResponseAllOf.construct(**{
-            "email": obj.get("email"),
-            "activated": obj.get("activated"),
-            "organizations": [UserOrganization.from_dict(_item) for _item in obj.get("organizations")] if obj.get("organizations") is not None else None,
-            "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
-            "experiments": [UserExperiment.from_dict(_item) for _item in obj.get("experiments")] if obj.get("experiments") is not None else None,
-            "evaluation": obj.get("evaluation"),
-            "ambassador": obj.get("ambassador"),
-            "tier": obj.get("tier"),
-            "whitelabels": [GetUserResponseAllOfWhitelabels.from_dict(_item) for _item in obj.get("whitelabels")] if obj.get("whitelabels") is not None else None,
-            "suspended": obj.get("suspended"),
-            "notifications": obj.get("notifications")
+        _obj = KerasModelMetadata.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "created": obj.get("created"),
+            "layers": [KerasModelLayer.from_dict(_item) for _item in obj.get("layers")] if obj.get("layers") is not None else None,
+            "class_names": obj.get("classNames"),
+            "labels": obj.get("labels"),
+            "available_model_types": obj.get("availableModelTypes"),
+            "recommended_model_type": obj.get("recommendedModelType"),
+            "model_validation_metrics": [KerasModelMetadataMetrics.from_dict(_item) for _item in obj.get("modelValidationMetrics")] if obj.get("modelValidationMetrics") is not None else None,
+            "has_trained_model": obj.get("hasTrainedModel"),
+            "mode": obj.get("mode"),
+            "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
+            "image_input_scaling": obj.get("imageInputScaling")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_user_response_all_of_whitelabels.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_domain_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_domain_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/get_whitelabel_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/get_whitelabel_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/has_data_explorer_features_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/has_data_explorer_features_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/image_input_scaling.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_tier_enum.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class ImageInputScaling(str, Enum):
+class UserTierEnum(str, Enum):
     """
     allowed enum values
     """
 
-    var_0__1 = '0..1'
-    var_1__1 = '-1..1'
-    var_128__127 = '-128..127'
-    var_0__255 = '0..255'
-    TORCH = 'torch'
+    FREE = 'free'
+    COMMUNITY_PLUS = 'community-plus'
+    PROFESSIONAL = 'professional'
+    ENTERPRISE = 'enterprise'
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_block_version.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_block_version.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_dsp_block_organization.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_dsp_block_organization.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_input_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/impulse_learn_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/impulse_learn_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/input_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/input_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/invite_organization_member_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/invite_organization_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_created_by_user.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_created_by_user.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_details_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_details_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_failure_details.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_failure_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_logs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_logs_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_logs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_metrics_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_parent_type_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_parent_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_state.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_state_execution_details.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_state_execution_details.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_status.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_step.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/job_summary_response_all_of_summary.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/job_summary_response_all_of_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keep_device_debug_stream_alive_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_custom_metric.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_custom_metric.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_input.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer_input.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_layer_output.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_layer_output.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_all_of.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,29 +21,27 @@
 from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
 from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
 from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 
-class KerasModelMetadata(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+class KerasModelMetadataAllOf(BaseModel):
     created: datetime = Field(..., description="Date when the model was trained")
     layers: List[KerasModelLayer] = Field(..., description="Layers of the neural network")
     class_names: List[StrictStr] = Field(..., alias="classNames", description="Labels for the output layer")
     labels: List[StrictStr] = Field(..., description="Original labels in the dataset when features were generated, e.g. used to render the feature explorer.")
     available_model_types: List[KerasModelTypeEnum] = Field(..., alias="availableModelTypes", description="The types of model that are available")
     recommended_model_type: KerasModelTypeEnum = Field(..., alias="recommendedModelType")
     model_validation_metrics: List[KerasModelMetadataMetrics] = Field(..., alias="modelValidationMetrics", description="Metrics for each of the available model types")
     has_trained_model: StrictBool = Field(..., alias="hasTrainedModel")
     mode: StrictStr = ...
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     image_input_scaling: ImageInputScaling = Field(..., alias="imageInputScaling")
-    __properties = ["success", "error", "created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
+    __properties = ["created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
 
     @validator('mode')
     def mode_validate_enum(cls, v):
         if v not in ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm'):
             raise ValueError("must validate the enum values ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm')")
         return v
 
@@ -56,16 +54,16 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadata:
-        """Create an instance of KerasModelMetadata from a JSON string"""
+    def from_json(cls, json_str: str) -> KerasModelMetadataAllOf:
+        """Create an instance of KerasModelMetadataAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
@@ -83,25 +81,23 @@
             for _item in self.model_validation_metrics:
                 if _item:
                     _items.append(_item.to_dict())
             _dict['modelValidationMetrics'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadata:
-        """Create an instance of KerasModelMetadata from a dict"""
+    def from_dict(cls, obj: dict) -> KerasModelMetadataAllOf:
+        """Create an instance of KerasModelMetadataAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadata.construct(**obj)
+            return KerasModelMetadataAllOf.construct(**obj)
 
-        _obj = KerasModelMetadata.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = KerasModelMetadataAllOf.construct(**{
             "created": obj.get("created"),
             "layers": [KerasModelLayer.from_dict(_item) for _item in obj.get("layers")] if obj.get("layers") is not None else None,
             "class_names": obj.get("classNames"),
             "labels": obj.get("labels"),
             "available_model_types": obj.get("availableModelTypes"),
             "recommended_model_type": obj.get("recommendedModelType"),
             "model_validation_metrics": [KerasModelMetadataMetrics.from_dict(_item) for _item in obj.get("modelValidationMetrics")] if obj.get("modelValidationMetrics") is not None else None,
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,41 +12,39 @@
 
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
-from datetime import datetime
+
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr, validator
-from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
-from edgeimpulse_api.models.keras_model_layer import KerasModelLayer
-from edgeimpulse_api.models.keras_model_metadata_metrics import KerasModelMetadataMetrics
-from edgeimpulse_api.models.keras_model_type_enum import KerasModelTypeEnum
-from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
-
-class KerasModelMetadataAllOf(BaseModel):
-    created: datetime = Field(..., description="Date when the model was trained")
-    layers: List[KerasModelLayer] = Field(..., description="Layers of the neural network")
-    class_names: List[StrictStr] = Field(..., alias="classNames", description="Labels for the output layer")
-    labels: List[StrictStr] = Field(..., description="Original labels in the dataset when features were generated, e.g. used to render the feature explorer.")
-    available_model_types: List[KerasModelTypeEnum] = Field(..., alias="availableModelTypes", description="The types of model that are available")
-    recommended_model_type: KerasModelTypeEnum = Field(..., alias="recommendedModelType")
-    model_validation_metrics: List[KerasModelMetadataMetrics] = Field(..., alias="modelValidationMetrics", description="Metrics for each of the available model types")
-    has_trained_model: StrictBool = Field(..., alias="hasTrainedModel")
-    mode: StrictStr = ...
-    object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
-    image_input_scaling: ImageInputScaling = Field(..., alias="imageInputScaling")
-    __properties = ["created", "layers", "classNames", "labels", "availableModelTypes", "recommendedModelType", "modelValidationMetrics", "hasTrainedModel", "mode", "objectDetectionLastLayer", "imageInputScaling"]
-
-    @validator('mode')
-    def mode_validate_enum(cls, v):
-        if v not in ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm'):
-            raise ValueError("must validate the enum values ('classification', 'regression', 'object-detection', 'visual-anomaly', 'anomaly-gmm')")
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
+from edgeimpulse_api.models.optimize_config import OptimizeConfig
+from edgeimpulse_api.models.optimize_state_response_all_of_status import OptimizeStateResponseAllOfStatus
+from edgeimpulse_api.models.optimize_state_response_all_of_workers import OptimizeStateResponseAllOfWorkers
+from edgeimpulse_api.models.tuner_trial import TunerTrial
+
+class OptimizeStateResponseAllOf(BaseModel):
+    config: OptimizeConfig = ...
+    status: OptimizeStateResponseAllOfStatus = ...
+    tuner_job_id: Optional[StrictInt] = Field(None, alias="tunerJobId", description="Actual tuner process, job message events will be tagged with this ID")
+    tuner_coordinator_job_id: Optional[StrictInt] = Field(None, alias="tunerCoordinatorJobId", description="The coordinator pod, attach the job runner to this process for finished events")
+    tuner_job_is_running: StrictBool = Field(..., alias="tunerJobIsRunning", description="Whether the job is active (if false => finished)")
+    trials: List[TunerTrial] = ...
+    project_data_type: StrictStr = Field(..., alias="projectDataType")
+    job_error: Optional[StrictStr] = Field(None, alias="jobError")
+    workers: List[OptimizeStateResponseAllOfWorkers] = ...
+    next_run_index: StrictInt = Field(..., alias="nextRunIndex")
+    __properties = ["config", "status", "tunerJobId", "tunerCoordinatorJobId", "tunerJobIsRunning", "trials", "projectDataType", "jobError", "workers", "nextRunIndex"]
+
+    @validator('project_data_type')
+    def project_data_type_validate_enum(cls, v):
+        if v not in ('audio', 'image', 'motion', 'other'):
+            raise ValueError("must validate the enum values ('audio', 'image', 'motion', 'other')")
         return v
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -54,57 +52,62 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> KerasModelMetadataAllOf:
-        """Create an instance of KerasModelMetadataAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> OptimizeStateResponseAllOf:
+        """Create an instance of OptimizeStateResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in layers (list)
+        # override the default output from pydantic by calling `to_dict()` of config
+        if self.config:
+            _dict['config'] = self.config.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of status
+        if self.status:
+            _dict['status'] = self.status.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in trials (list)
         _items = []
-        if self.layers:
-            for _item in self.layers:
+        if self.trials:
+            for _item in self.trials:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['layers'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in model_validation_metrics (list)
+            _dict['trials'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
         _items = []
-        if self.model_validation_metrics:
-            for _item in self.model_validation_metrics:
+        if self.workers:
+            for _item in self.workers:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['modelValidationMetrics'] = _items
+            _dict['workers'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> KerasModelMetadataAllOf:
-        """Create an instance of KerasModelMetadataAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> OptimizeStateResponseAllOf:
+        """Create an instance of OptimizeStateResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return KerasModelMetadataAllOf.construct(**obj)
+            return OptimizeStateResponseAllOf.construct(**obj)
 
-        _obj = KerasModelMetadataAllOf.construct(**{
-            "created": obj.get("created"),
-            "layers": [KerasModelLayer.from_dict(_item) for _item in obj.get("layers")] if obj.get("layers") is not None else None,
-            "class_names": obj.get("classNames"),
-            "labels": obj.get("labels"),
-            "available_model_types": obj.get("availableModelTypes"),
-            "recommended_model_type": obj.get("recommendedModelType"),
-            "model_validation_metrics": [KerasModelMetadataMetrics.from_dict(_item) for _item in obj.get("modelValidationMetrics")] if obj.get("modelValidationMetrics") is not None else None,
-            "has_trained_model": obj.get("hasTrainedModel"),
-            "mode": obj.get("mode"),
-            "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
-            "image_input_scaling": obj.get("imageInputScaling")
+        _obj = OptimizeStateResponseAllOf.construct(**{
+            "config": OptimizeConfig.from_dict(obj.get("config")) if obj.get("config") is not None else None,
+            "status": OptimizeStateResponseAllOfStatus.from_dict(obj.get("status")) if obj.get("status") is not None else None,
+            "tuner_job_id": obj.get("tunerJobId"),
+            "tuner_coordinator_job_id": obj.get("tunerCoordinatorJobId"),
+            "tuner_job_is_running": obj.get("tunerJobIsRunning"),
+            "trials": [TunerTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None,
+            "project_data_type": obj.get("projectDataType"),
+            "job_error": obj.get("jobError"),
+            "workers": [OptimizeStateResponseAllOfWorkers.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
+            "next_run_index": obj.get("nextRunIndex")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_metadata_metrics_on_device_performance_inner_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_type_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_model_type_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_model_variant_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/block_type.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,16 +15,18 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class KerasModelVariantEnum(str, Enum):
+class BlockType(str, Enum):
     """
     allowed enum values
     """
 
-    INT8 = 'int8'
-    FLOAT32 = 'float32'
-    AKIDA = 'akida'
+    OFFICIAL = 'official'
+    PERSONAL = 'personal'
+    ENTERPRISE = 'enterprise'
+    PRO_OR_ENTERPRISE = 'pro-or-enterprise'
+    COMMUNITY = 'community'
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_visual_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/keras_visual_layer_type.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/keras_visual_layer_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/last_modification_date_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/last_modification_date_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/last_modification_date_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/latency_device.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/latency_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/portal_info_response.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,72 +14,62 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
-from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
-from edgeimpulse_api.models.block_type import BlockType
-
-class LearnBlock(BaseModel):
-    type: StrictStr = ...
-    title: StrictStr = ...
-    author: StrictStr = ...
-    description: StrictStr = ...
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class PortalInfoResponse(BaseModel):
     name: StrictStr = ...
-    recommended: Optional[StrictBool] = None
-    organization_model_id: Optional[StrictInt] = Field(None, alias="organizationModelId")
-    is_public_enterprise_only: Optional[StrictBool] = Field(None, alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
-    block_type: BlockType = Field(..., alias="blockType")
-    display_category: Optional[BlockDisplayCategory] = Field(None, alias="displayCategory")
-    __properties = ["type", "title", "author", "description", "name", "recommended", "organizationModelId", "isPublicEnterpriseOnly", "blockType", "displayCategory"]
+    description: StrictStr = ...
+    organization_id: StrictInt = Field(..., alias="organizationId")
+    organization_name: StrictStr = Field(..., alias="organizationName")
+    organization_logo: Optional[StrictStr] = Field(None, alias="organizationLogo")
+    bucket_name: StrictStr = Field(..., alias="bucketName")
+    __properties = ["name", "description", "organizationId", "organizationName", "organizationLogo", "bucketName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> LearnBlock:
-        """Create an instance of LearnBlock from a JSON string"""
+    def from_json(cls, json_str: str) -> PortalInfoResponse:
+        """Create an instance of PortalInfoResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> LearnBlock:
-        """Create an instance of LearnBlock from a dict"""
+    def from_dict(cls, obj: dict) -> PortalInfoResponse:
+        """Create an instance of PortalInfoResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return LearnBlock.construct(**obj)
+            return PortalInfoResponse.construct(**obj)
 
-        _obj = LearnBlock.construct(**{
-            "type": obj.get("type"),
-            "title": obj.get("title"),
-            "author": obj.get("author"),
-            "description": obj.get("description"),
+        _obj = PortalInfoResponse.construct(**{
             "name": obj.get("name"),
-            "recommended": obj.get("recommended"),
-            "organization_model_id": obj.get("organizationModelId"),
-            "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
-            "block_type": obj.get("blockType"),
-            "display_category": obj.get("displayCategory")
+            "description": obj.get("description"),
+            "organization_id": obj.get("organizationId"),
+            "organization_name": obj.get("organizationName"),
+            "organization_logo": obj.get("organizationLogo"),
+            "bucket_name": obj.get("bucketName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/learn_block_type.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/learn_block_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_devices_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_devices_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_devices_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_email_response_all_of_emails.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_email_response_all_of_emails.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_enterprise_trials_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_enterprise_trials_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_hmac_keys_response_all_of_hmac_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_jobs_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_jobs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_models_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_api_keys_response_all_of_api_keys.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_buckets_user_response_all_of_buckets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_data_response_all_of_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_data_response_all_of_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_deploy_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_deploy_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_dsp_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_dsp_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_files_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_files_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_files_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_pipelines_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_portals_response_all_of_portals.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_projects_data_response_all_of_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_secrets_response_all_of_secrets.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transfer_learning_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_usage_reports_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organization_usage_reports_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organizations_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_organizations_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_organizations_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_portal_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_projects_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_organization_transformation_blocks_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_organization_transformation_blocks_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_projects.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_projects_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_public_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_samples_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_samples_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_samples_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_tuner_runs_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_tuner_runs_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_tuner_runs_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_bucket.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_custom_learn_blocks.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/list_versions_response_all_of_versions.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/list_versions_response_all_of_versions.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_analytics_event_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_analytics_event_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_stdout_response_all_of_stdout.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/log_website_pageview_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/log_website_pageview_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/login_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/login_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/login_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/memory_spec.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/memory_spec.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_all_variants_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_all_variants_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_all_variants_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/metrics_for_model_variant.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/metrics_for_model_variant.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/migration.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/migration.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_engine_short_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_engine_short_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_prediction.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_prediction.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_result.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/model_variant_stats.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/model_variant_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/move_raw_data_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/move_raw_data_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_score.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/neighbors_score_neighbor_windows_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/note.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/note.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_auto_label_response_all_of_results.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_count_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_count_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_label_queue_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/object_detection_last_layer.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/object_detection_last_layer.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_config_target_device.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_config_target_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_dsp_parameters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_dsp_parameters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_space_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_space_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_space_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,101 +13,97 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
-from edgeimpulse_api.models.optimize_config import OptimizeConfig
-from edgeimpulse_api.models.optimize_state_response_all_of_status import OptimizeStateResponseAllOfStatus
-from edgeimpulse_api.models.optimize_state_response_all_of_workers import OptimizeStateResponseAllOfWorkers
-from edgeimpulse_api.models.tuner_trial import TunerTrial
-
-class OptimizeStateResponseAllOf(BaseModel):
-    config: OptimizeConfig = ...
-    status: OptimizeStateResponseAllOfStatus = ...
-    tuner_job_id: Optional[StrictInt] = Field(None, alias="tunerJobId", description="Actual tuner process, job message events will be tagged with this ID")
-    tuner_coordinator_job_id: Optional[StrictInt] = Field(None, alias="tunerCoordinatorJobId", description="The coordinator pod, attach the job runner to this process for finished events")
-    tuner_job_is_running: StrictBool = Field(..., alias="tunerJobIsRunning", description="Whether the job is active (if false => finished)")
-    trials: List[TunerTrial] = ...
-    project_data_type: StrictStr = Field(..., alias="projectDataType")
-    job_error: Optional[StrictStr] = Field(None, alias="jobError")
-    workers: List[OptimizeStateResponseAllOfWorkers] = ...
-    next_run_index: StrictInt = Field(..., alias="nextRunIndex")
-    __properties = ["config", "status", "tunerJobId", "tunerCoordinatorJobId", "tunerJobIsRunning", "trials", "projectDataType", "jobError", "workers", "nextRunIndex"]
-
-    @validator('project_data_type')
-    def project_data_type_validate_enum(cls, v):
-        if v not in ('audio', 'image', 'motion', 'other'):
-            raise ValueError("must validate the enum values ('audio', 'image', 'motion', 'other')")
-        return v
+from typing import List
+from pydantic import BaseModel, Field
+from edgeimpulse_api.models.transfer_learning_model import TransferLearningModel
+
+class OptimizeTransferLearningModelsResponseAllOfModels(BaseModel):
+    image: List[TransferLearningModel] = ...
+    object_detection: List[TransferLearningModel] = Field(..., alias="objectDetection")
+    kws: List[TransferLearningModel] = ...
+    regression: List[TransferLearningModel] = ...
+    classification: List[TransferLearningModel] = ...
+    __properties = ["image", "objectDetection", "kws", "regression", "classification"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OptimizeStateResponseAllOf:
-        """Create an instance of OptimizeStateResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> OptimizeTransferLearningModelsResponseAllOfModels:
+        """Create an instance of OptimizeTransferLearningModelsResponseAllOfModels from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of config
-        if self.config:
-            _dict['config'] = self.config.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of status
-        if self.status:
-            _dict['status'] = self.status.to_dict()
-        # override the default output from pydantic by calling `to_dict()` of each item in trials (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in image (list)
         _items = []
-        if self.trials:
-            for _item in self.trials:
+        if self.image:
+            for _item in self.image:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['trials'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in workers (list)
+            _dict['image'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in object_detection (list)
         _items = []
-        if self.workers:
-            for _item in self.workers:
+        if self.object_detection:
+            for _item in self.object_detection:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['workers'] = _items
+            _dict['objectDetection'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in kws (list)
+        _items = []
+        if self.kws:
+            for _item in self.kws:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['kws'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in regression (list)
+        _items = []
+        if self.regression:
+            for _item in self.regression:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['regression'] = _items
+        # override the default output from pydantic by calling `to_dict()` of each item in classification (list)
+        _items = []
+        if self.classification:
+            for _item in self.classification:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict['classification'] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OptimizeStateResponseAllOf:
-        """Create an instance of OptimizeStateResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> OptimizeTransferLearningModelsResponseAllOfModels:
+        """Create an instance of OptimizeTransferLearningModelsResponseAllOfModels from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OptimizeStateResponseAllOf.construct(**obj)
+            return OptimizeTransferLearningModelsResponseAllOfModels.construct(**obj)
 
-        _obj = OptimizeStateResponseAllOf.construct(**{
-            "config": OptimizeConfig.from_dict(obj.get("config")) if obj.get("config") is not None else None,
-            "status": OptimizeStateResponseAllOfStatus.from_dict(obj.get("status")) if obj.get("status") is not None else None,
-            "tuner_job_id": obj.get("tunerJobId"),
-            "tuner_coordinator_job_id": obj.get("tunerCoordinatorJobId"),
-            "tuner_job_is_running": obj.get("tunerJobIsRunning"),
-            "trials": [TunerTrial.from_dict(_item) for _item in obj.get("trials")] if obj.get("trials") is not None else None,
-            "project_data_type": obj.get("projectDataType"),
-            "job_error": obj.get("jobError"),
-            "workers": [OptimizeStateResponseAllOfWorkers.from_dict(_item) for _item in obj.get("workers")] if obj.get("workers") is not None else None,
-            "next_run_index": obj.get("nextRunIndex")
+        _obj = OptimizeTransferLearningModelsResponseAllOfModels.construct(**{
+            "image": [TransferLearningModel.from_dict(_item) for _item in obj.get("image")] if obj.get("image") is not None else None,
+            "object_detection": [TransferLearningModel.from_dict(_item) for _item in obj.get("objectDetection")] if obj.get("objectDetection") is not None else None,
+            "kws": [TransferLearningModel.from_dict(_item) for _item in obj.get("kws")] if obj.get("kws") is not None else None,
+            "regression": [TransferLearningModel.from_dict(_item) for _item in obj.get("regression")] if obj.get("regression") is not None else None,
+            "classification": [TransferLearningModel.from_dict(_item) for _item in obj.get("classification")] if obj.get("classification") is not None else None
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_status.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of_status.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_state_response_all_of_workers.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_state_response_all_of_workers.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/optimize_transfer_learning_models_response_all_of_models.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,96 +14,88 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field
-from edgeimpulse_api.models.transfer_learning_model import TransferLearningModel
-
-class OptimizeTransferLearningModelsResponseAllOfModels(BaseModel):
-    image: List[TransferLearningModel] = ...
-    object_detection: List[TransferLearningModel] = Field(..., alias="objectDetection")
-    kws: List[TransferLearningModel] = ...
-    regression: List[TransferLearningModel] = ...
-    classification: List[TransferLearningModel] = ...
-    __properties = ["image", "objectDetection", "kws", "regression", "classification"]
+from pydantic import BaseModel, Field, StrictBool, StrictStr
+from edgeimpulse_api.models.performance_calibration_detection import PerformanceCalibrationDetection
+from edgeimpulse_api.models.performance_calibration_parameter_set_aggregate_stats import PerformanceCalibrationParameterSetAggregateStats
+from edgeimpulse_api.models.performance_calibration_parameter_set_stats_inner import PerformanceCalibrationParameterSetStatsInner
+from edgeimpulse_api.models.performance_calibration_parameters import PerformanceCalibrationParameters
+
+class PerformanceCalibrationParameterSet(BaseModel):
+    detections: List[PerformanceCalibrationDetection] = Field(..., description="All of the detections using this parameter set")
+    is_best: StrictBool = Field(..., alias="isBest", description="Whether this is considered the best parameter set")
+    labels: List[StrictStr] = Field(..., description="All of the possible labels in the detections array")
+    aggregate_stats: PerformanceCalibrationParameterSetAggregateStats = Field(..., alias="aggregateStats")
+    stats: List[PerformanceCalibrationParameterSetStatsInner] = ...
+    params: PerformanceCalibrationParameters = ...
+    window_size_ms: float = Field(..., alias="windowSizeMs", description="The size of the input block window in milliseconds.")
+    __properties = ["detections", "isBest", "labels", "aggregateStats", "stats", "params", "windowSizeMs"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> OptimizeTransferLearningModelsResponseAllOfModels:
-        """Create an instance of OptimizeTransferLearningModelsResponseAllOfModels from a JSON string"""
+    def from_json(cls, json_str: str) -> PerformanceCalibrationParameterSet:
+        """Create an instance of PerformanceCalibrationParameterSet from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of each item in image (list)
-        _items = []
-        if self.image:
-            for _item in self.image:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['image'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in object_detection (list)
-        _items = []
-        if self.object_detection:
-            for _item in self.object_detection:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['objectDetection'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in kws (list)
-        _items = []
-        if self.kws:
-            for _item in self.kws:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict['kws'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in regression (list)
+        # override the default output from pydantic by calling `to_dict()` of each item in detections (list)
         _items = []
-        if self.regression:
-            for _item in self.regression:
+        if self.detections:
+            for _item in self.detections:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['regression'] = _items
-        # override the default output from pydantic by calling `to_dict()` of each item in classification (list)
+            _dict['detections'] = _items
+        # override the default output from pydantic by calling `to_dict()` of aggregate_stats
+        if self.aggregate_stats:
+            _dict['aggregateStats'] = self.aggregate_stats.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of each item in stats (list)
         _items = []
-        if self.classification:
-            for _item in self.classification:
+        if self.stats:
+            for _item in self.stats:
                 if _item:
                     _items.append(_item.to_dict())
-            _dict['classification'] = _items
+            _dict['stats'] = _items
+        # override the default output from pydantic by calling `to_dict()` of params
+        if self.params:
+            _dict['params'] = self.params.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> OptimizeTransferLearningModelsResponseAllOfModels:
-        """Create an instance of OptimizeTransferLearningModelsResponseAllOfModels from a dict"""
+    def from_dict(cls, obj: dict) -> PerformanceCalibrationParameterSet:
+        """Create an instance of PerformanceCalibrationParameterSet from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return OptimizeTransferLearningModelsResponseAllOfModels.construct(**obj)
+            return PerformanceCalibrationParameterSet.construct(**obj)
 
-        _obj = OptimizeTransferLearningModelsResponseAllOfModels.construct(**{
-            "image": [TransferLearningModel.from_dict(_item) for _item in obj.get("image")] if obj.get("image") is not None else None,
-            "object_detection": [TransferLearningModel.from_dict(_item) for _item in obj.get("objectDetection")] if obj.get("objectDetection") is not None else None,
-            "kws": [TransferLearningModel.from_dict(_item) for _item in obj.get("kws")] if obj.get("kws") is not None else None,
-            "regression": [TransferLearningModel.from_dict(_item) for _item in obj.get("regression")] if obj.get("regression") is not None else None,
-            "classification": [TransferLearningModel.from_dict(_item) for _item in obj.get("classification")] if obj.get("classification") is not None else None
+        _obj = PerformanceCalibrationParameterSet.construct(**{
+            "detections": [PerformanceCalibrationDetection.from_dict(_item) for _item in obj.get("detections")] if obj.get("detections") is not None else None,
+            "is_best": obj.get("isBest"),
+            "labels": obj.get("labels"),
+            "aggregate_stats": PerformanceCalibrationParameterSetAggregateStats.from_dict(obj.get("aggregateStats")) if obj.get("aggregateStats") is not None else None,
+            "stats": [PerformanceCalibrationParameterSetStatsInner.from_dict(_item) for _item in obj.get("stats")] if obj.get("stats") is not None else None,
+            "params": PerformanceCalibrationParameters.from_dict(obj.get("params")) if obj.get("params") is not None else None,
+            "window_size_ms": obj.get("windowSizeMs")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,25 +23,26 @@
 from edgeimpulse_api.models.project import Project
 
 class Organization(BaseModel):
     id: StrictInt = ...
     name: StrictStr = Field(..., description="EdgeImpulse Inc.")
     logo: Optional[StrictStr] = None
     header_img: Optional[StrictStr] = Field(None, alias="headerImg")
+    show_header_img_mask: StrictBool = Field(..., alias="showHeaderImgMask")
     users: List[OrganizationUser] = ...
     is_developer_profile: StrictBool = Field(..., alias="isDeveloperProfile")
     whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this organization belongs to, if any.")
     projects: Optional[List[Project]] = None
     trial_id: Optional[StrictInt] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
     trial_expired_date: Optional[datetime] = Field(..., alias="trialExpiredDate", description="Date when the trial expired, if any. A expired trial has a grace period of 30 days before it's associated organization is deleted.")
     trial_upgraded_date: Optional[datetime] = Field(..., alias="trialUpgradedDate", description="Date when the trial was upgraded to a full enterprise account, if any.")
     created: datetime = Field(..., description="Date when the organization was created.")
     contract_start_date: Optional[datetime] = Field(None, alias="contractStartDate", description="Date when the current contract started, if any.")
     deleted_date: Optional[datetime] = Field(None, alias="deletedDate", description="The date in which the organization was deleted. If the organization is not deleted, this field is not set.")
-    __properties = ["id", "name", "logo", "headerImg", "users", "isDeveloperProfile", "whitelabelId", "projects", "trialId", "trialExpiredDate", "trialUpgradedDate", "created", "contractStartDate", "deletedDate"]
+    __properties = ["id", "name", "logo", "headerImg", "showHeaderImgMask", "users", "isDeveloperProfile", "whitelabelId", "projects", "trialId", "trialExpiredDate", "trialUpgradedDate", "created", "contractStartDate", "deletedDate"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -108,14 +109,15 @@
             return Organization.construct(**obj)
 
         _obj = Organization.construct(**{
             "id": obj.get("id"),
             "name": obj.get("name"),
             "logo": obj.get("logo"),
             "header_img": obj.get("headerImg"),
+            "show_header_img_mask": obj.get("showHeaderImgMask"),
             "users": [OrganizationUser.from_dict(_item) for _item in obj.get("users")] if obj.get("users") is not None else None,
             "is_developer_profile": obj.get("isDeveloperProfile"),
             "whitelabel_id": obj.get("whitelabelId"),
             "projects": [Project.from_dict(_item) for _item in obj.get("projects")] if obj.get("projects") is not None else None,
             "trial_id": obj.get("trialId"),
             "trial_expired_date": obj.get("trialExpiredDate"),
             "trial_upgraded_date": obj.get("trialUpgradedDate"),
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_data_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_add_dataset_request_bucket.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_add_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_bucket.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_compute_time_usage.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_compute_time_usage.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_output_dataset_path_rule.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_path_filter.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_path_filter.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_status_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_status_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_status_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_transformation_summary.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_transformation_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_create_project_with_files_all_of_files.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_request_queries_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_campaign_diff_response_all_of_queries.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_export.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_export.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_item.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_data_item_files_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_data_item_files_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dataset_bucket.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dataset_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_deploy_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_deploy_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_dsp_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_dsp_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_get_create_projects_response_all_of_jobs.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_image_input_scaling_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_cli_lists_object_detection_last_layer_options.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_default_compute_limits.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_info_response_all_of_performance.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_member_role.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_member_role.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_metrics_response_all_of_metrics.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_feeding_into_dataset.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_feeding_into_project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_item_count.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_item_count.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_run_step.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_run_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_pipeline_step.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_pipeline_step.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_disable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_enable_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_projects_data_batch_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_projects_data_batch_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transfer_learning_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
 from edgeimpulse_api.models.created_updated_by_user import CreatedUpdatedByUser
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 from edgeimpulse_api.models.organization_transfer_learning_operates_on import OrganizationTransferLearningOperatesOn
+from edgeimpulse_api.models.public_project_tier_availability import PublicProjectTierAvailability
 
 class OrganizationTransferLearningBlock(BaseModel):
     id: StrictInt = ...
     name: StrictStr = ...
     docker_container: StrictStr = Field(..., alias="dockerContainer")
     docker_container_managed_by_edge_impulse: StrictBool = Field(..., alias="dockerContainerManagedByEdgeImpulse")
     created: datetime = ...
@@ -38,23 +39,24 @@
     user_id: Optional[StrictInt] = Field(None, alias="userId")
     user_name: Optional[StrictStr] = Field(None, alias="userName")
     operates_on: OrganizationTransferLearningOperatesOn = Field(..., alias="operatesOn")
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: StrictInt = Field(..., alias="implementationVersion")
     is_public: StrictBool = Field(..., alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: List[StrictStr] = Field(..., alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
-    is_public_enterprise_only: StrictBool = Field(..., alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
-    enterprise_only: Optional[StrictBool] = Field(None, alias="enterpriseOnly", description="Whether this block is available to Edge Impulse only to enterprise users")
+    public_project_tier_availability: Optional[PublicProjectTierAvailability] = Field(None, alias="publicProjectTierAvailability")
+    is_public_enterprise_only: StrictBool = Field(..., alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to only enterprise users")
+    enterprise_only: Optional[StrictBool] = Field(None, alias="enterpriseOnly", description="Whether this block is available to only enterprise users")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: List[Dict[str, Any]] = Field(..., description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
     ind_requires_gpu: StrictBool = Field(..., alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
     source_code_available: StrictBool = Field(..., alias="sourceCodeAvailable")
     display_category: Optional[BlockDisplayCategory] = Field(None, alias="displayCategory")
-    __properties = ["id", "name", "dockerContainer", "dockerContainerManagedByEdgeImpulse", "created", "createdByUser", "lastUpdated", "lastUpdatedByUser", "description", "userId", "userName", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "isPublicEnterpriseOnly", "enterpriseOnly", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu", "sourceCodeAvailable", "displayCategory"]
+    __properties = ["id", "name", "dockerContainer", "dockerContainerManagedByEdgeImpulse", "created", "createdByUser", "lastUpdated", "lastUpdatedByUser", "description", "userId", "userName", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "publicProjectTierAvailability", "isPublicEnterpriseOnly", "enterpriseOnly", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu", "sourceCodeAvailable", "displayCategory"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -105,14 +107,15 @@
             "user_id": obj.get("userId"),
             "user_name": obj.get("userName"),
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
+            "public_project_tier_availability": obj.get("publicProjectTierAvailability"),
             "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
             "enterprise_only": obj.get("enterpriseOnly"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
             "image_input_scaling": obj.get("imageInputScaling"),
             "ind_requires_gpu": obj.get("indRequiresGpu"),
             "source_code_available": obj.get("sourceCodeAvailable"),
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transfer_learning_operates_on.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transfer_learning_operates_on.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_transformation_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_update_pipeline_body.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_update_pipeline_body.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_usage_report.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_usage_report.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.organization_member_role import OrganizationMemberRole
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 
 class OrganizationUser(BaseModel):
     id: StrictInt = ...
     username: StrictStr = ...
     name: StrictStr = ...
     email: StrictStr = ...
     photo: Optional[StrictStr] = None
@@ -37,19 +38,20 @@
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
     stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
     has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    tier: Optional[UserTierEnum] = None
     added: datetime = ...
     role: OrganizationMemberRole = ...
     project_count: StrictInt = Field(..., alias="projectCount")
     datasets: List[StrictStr] = ...
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "added", "role", "projectCount", "datasets"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier", "added", "role", "projectCount", "datasets"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -98,14 +100,15 @@
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
             "stripe_customer_id": obj.get("stripeCustomerId"),
             "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier"),
             "added": obj.get("added"),
             "role": obj.get("role"),
             "project_count": obj.get("projectCount"),
             "datasets": obj.get("datasets")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/organization_user_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/organization_user_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_detection.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_false_positive.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_false_positive.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_ground_truth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_ground_truth_samples_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set_aggregate_stats.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameter_set_stats_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameters.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_parameters_standard.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_parameters_standard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_raw_detection.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_raw_detection.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_save_parameter_set_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/performance_calibration_upload_labeled_audio_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/permission.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/permission.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_file.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/portal_file.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/portal_info_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,63 +13,65 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from typing import List, Optional
+from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 
-class PortalInfoResponse(BaseModel):
-    name: StrictStr = ...
-    description: StrictStr = ...
-    organization_id: StrictInt = Field(..., alias="organizationId")
-    organization_name: StrictStr = Field(..., alias="organizationName")
-    organization_logo: Optional[StrictStr] = Field(None, alias="organizationLogo")
-    bucket_name: StrictStr = Field(..., alias="bucketName")
-    __properties = ["name", "description", "organizationId", "organizationName", "organizationLogo", "bucketName"]
+class UpdateOrganizationRequest(BaseModel):
+    logo: Optional[StrictStr] = Field(None, description="New logo URL, or set to `null` to remove the logo.")
+    header_img: Optional[StrictStr] = Field(None, alias="headerImg", description="New leader image URL, or set to `null` to remove the leader.")
+    show_header_img_mask: Optional[StrictBool] = Field(None, alias="showHeaderImgMask")
+    name: Optional[StrictStr] = Field(None, description="New organization name.")
+    experiments: Optional[List[StrictStr]] = None
+    readme: Optional[StrictStr] = Field(None, description="Readme for the organization (in Markdown)")
+    job_limit_m: Optional[StrictInt] = Field(None, alias="jobLimitM", description="New job limit in seconds.")
+    __properties = ["logo", "headerImg", "showHeaderImgMask", "name", "experiments", "readme", "jobLimitM"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> PortalInfoResponse:
-        """Create an instance of PortalInfoResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateOrganizationRequest:
+        """Create an instance of UpdateOrganizationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> PortalInfoResponse:
-        """Create an instance of PortalInfoResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateOrganizationRequest:
+        """Create an instance of UpdateOrganizationRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return PortalInfoResponse.construct(**obj)
+            return UpdateOrganizationRequest.construct(**obj)
 
-        _obj = PortalInfoResponse.construct(**{
+        _obj = UpdateOrganizationRequest.construct(**{
+            "logo": obj.get("logo"),
+            "header_img": obj.get("headerImg"),
+            "show_header_img_mask": obj.get("showHeaderImgMask"),
             "name": obj.get("name"),
-            "description": obj.get("description"),
-            "organization_id": obj.get("organizationId"),
-            "organization_name": obj.get("organizationName"),
-            "organization_logo": obj.get("organizationLogo"),
-            "bucket_name": obj.get("bucketName")
+            "experiments": obj.get("experiments"),
+            "readme": obj.get("readme"),
+            "job_limit_m": obj.get("jobLimitM")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/pretrained_model_tensor.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/pretrained_model_tensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/preview_default_files_in_folder_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_eon.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory_eon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_info_memory_tflite.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_info_memory_tflite.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mcu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mcu_memory.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mcu_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_model_table_mpu.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_model_table_mpu.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_tf_lite_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/profile_tf_lite_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/profile_tf_lite_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_collaborator.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 
 class ProjectCollaborator(BaseModel):
     id: StrictInt = ...
     username: StrictStr = ...
     name: StrictStr = ...
     email: StrictStr = ...
     photo: Optional[StrictStr] = None
@@ -36,16 +37,17 @@
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
     stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
     has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
+    tier: Optional[UserTierEnum] = None
     is_owner: StrictBool = Field(..., alias="isOwner")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "isOwner"]
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier", "isOwner"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -94,11 +96,12 @@
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
             "stripe_customer_id": obj.get("stripeCustomerId"),
             "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier"),
             "is_owner": obj.get("isOwner")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_collaborator_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_collaborator_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_axes_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_axes_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_interval_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_interval_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_interval_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_data_summary.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_target.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_target_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_target_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_targets_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_deployment_targets_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_deployment_targets_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_dismiss_notification_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_downloads_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_downloads_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_downloads_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_acquisition_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_compute_time.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_compute_time.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_data_summary_per_category.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_deploy_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_experiments.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_experiments.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_impulse.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_performance.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_performance.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_readme.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_show_getting_started_wizard.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_response_all_of_urls.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_response_all_of_urls.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_info_summary_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_info_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_private_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_private_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_public_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_public_data_readme.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_public_data_readme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_sample_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_tier_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_tier_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_training_data_summary_response_all_of_data_summary.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_type.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_type.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/project_version_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/project_version_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/public_organization_transformation_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/public_organization_transformation_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_data.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/raw_sample_data.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/raw_sample_payload.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/raw_sample_payload.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rebalance_dataset_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/rebalance_dataset_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_collaborator_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/remove_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/remove_member_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/remove_member_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_device_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_device_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_portal_file_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_portal_file_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/rename_sample_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/rename_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_email_verification_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/request_email_verification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/request_reset_password_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/request_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/reset_password_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/resource_range.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/resource_range.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_from_public_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/restore_project_from_public_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/restore_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/restore_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_auto_labeler_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_auto_labeler_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_organization_pipeline_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/run_organization_pipeline_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_bounding_boxes_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample_bounding_boxes_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sample_metadata.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/sample_metadata.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_request_clusters_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_auto_labeler_clusters_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/save_pretrained_model_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/save_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_latency.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of_latency.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/score_trial_response_all_of_ram.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/score_trial_response_all_of_ram.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/segment_sample_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/segment_sample_request_segments_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/segment_sample_request_segments_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/send_user_feedback_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/send_user_feedback_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/sensor.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/sensor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_anomaly_parameter_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_anomaly_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_keras_parameter_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_keras_parameter_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_datasets_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_member_datasets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_member_role_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_member_role_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_optimize_space_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_optimize_space_request_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_optimize_space_request_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_organization_data_dataset_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_organization_data_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_compute_time_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_project_compute_time_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_project_dsp_file_size_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_project_dsp_file_size_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_metadata_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_sample_metadata_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_sample_structured_labels_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_sample_structured_labels_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_syntiant_posterior_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_syntiant_posterior_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/set_user_password_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/set_user_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/socket_token_response_all_of_token.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/socket_token_response_all_of_token.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/split_sample_in_frames_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/split_sample_in_frames_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/staff_info.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/staff_info.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_debug_stream_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_debug_stream_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_device_snapshot_debug_stream_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_enterprise_trial_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_enterprise_trial_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_job_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_job_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_job_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_performance_calibration_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_performance_calibration_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_sampling_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_sampling_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/start_training_request_anomaly.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/start_training_request_anomaly.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/stop_device_debug_stream_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/stop_device_debug_stream_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/store_segment_length_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/store_segment_length_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_classify_result.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/structured_classify_result.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/structured_label.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/structured_label.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_constraints.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_constraints_device.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_constraints_device.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_memory.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_memory.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/target_processor.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/target_processor.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/test_pretrained_model_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/test_pretrained_model_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_colors.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_colors.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_favicon.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_favicon.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/theme_logos.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/theme_logos.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/third_party_auth.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/third_party_auth.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/time_series_data_point.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/time_series_data_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/track_objects_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/track_objects_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_learning_model.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transfer_ownership_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/transfer_ownership_organization_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_block_additional_mount_point.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_block_additional_mount_point.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_operates_on_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_job_operates_on_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/transformation_job_status_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/transformation_job_status_enum.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_create_trial_impulse.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_create_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_run.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_run.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_space_impulse.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_space_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_blocks_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_blocks_inner.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_dsp_job_id.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_dsp_job_id.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/tuner_trial_impulse.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/tuner_trial_impulse.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_job_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_job_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_add_collaborator_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_add_collaborator_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_bucket_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_empty_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_create_empty_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_create_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_create_project_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_campaign_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_campaign_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_campaign_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_data_item_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_data_item_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dataset_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dataset_request_bucket.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dataset_request_bucket.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_dsp_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_dsp_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_portal_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_portal_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_portal_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_user_request.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,62 +14,61 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List, Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictStr
+from edgeimpulse_api.models.user_projects_sort_order import UserProjectsSortOrder
 
-class UpdateOrganizationRequest(BaseModel):
-    logo: Optional[StrictStr] = Field(None, description="New logo URL, or set to `null` to remove the logo.")
-    header_img: Optional[StrictStr] = Field(None, alias="headerImg", description="New leader image URL, or set to `null` to remove the leader.")
-    name: Optional[StrictStr] = Field(None, description="New organization name.")
-    experiments: Optional[List[StrictStr]] = None
-    readme: Optional[StrictStr] = Field(None, description="Readme for the organization (in Markdown)")
-    job_limit_m: Optional[StrictInt] = Field(None, alias="jobLimitM", description="New job limit in seconds.")
-    __properties = ["logo", "headerImg", "name", "experiments", "readme", "jobLimitM"]
+class UpdateUserRequest(BaseModel):
+    name: Optional[StrictStr] = Field(None, description="New full name")
+    job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="New job title")
+    company_name: Optional[StrictStr] = Field(None, alias="companyName", description="New company name")
+    experiments: Optional[List[StrictStr]] = Field(None, description="List of user experiments")
+    projects_sort_order: Optional[UserProjectsSortOrder] = Field(None, alias="projectsSortOrder")
+    __properties = ["name", "jobTitle", "companyName", "experiments", "projectsSortOrder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateOrganizationRequest:
-        """Create an instance of UpdateOrganizationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateUserRequest:
+        """Create an instance of UpdateUserRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateOrganizationRequest:
-        """Create an instance of UpdateOrganizationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateUserRequest:
+        """Create an instance of UpdateUserRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateOrganizationRequest.construct(**obj)
+            return UpdateUserRequest.construct(**obj)
 
-        _obj = UpdateOrganizationRequest.construct(**{
-            "logo": obj.get("logo"),
-            "header_img": obj.get("headerImg"),
+        _obj = UpdateUserRequest.construct(**{
             "name": obj.get("name"),
+            "job_title": obj.get("jobTitle"),
+            "company_name": obj.get("companyName"),
             "experiments": obj.get("experiments"),
-            "readme": obj.get("readme"),
-            "job_limit_m": obj.get("jobLimitM")
+            "projects_sort_order": obj.get("projectsSortOrder")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_transfer_learning_block_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,31 +19,32 @@
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.block_display_category import BlockDisplayCategory
 from edgeimpulse_api.models.image_input_scaling import ImageInputScaling
 from edgeimpulse_api.models.object_detection_last_layer import ObjectDetectionLastLayer
 from edgeimpulse_api.models.organization_transfer_learning_operates_on import OrganizationTransferLearningOperatesOn
+from edgeimpulse_api.models.public_project_tier_availability import PublicProjectTierAvailability
 
 class UpdateOrganizationTransferLearningBlockRequest(BaseModel):
     name: Optional[StrictStr] = None
     docker_container: Optional[StrictStr] = Field(None, alias="dockerContainer")
     description: Optional[StrictStr] = None
     operates_on: Optional[OrganizationTransferLearningOperatesOn] = Field(None, alias="operatesOn")
     object_detection_last_layer: Optional[ObjectDetectionLastLayer] = Field(None, alias="objectDetectionLastLayer")
     implementation_version: Optional[StrictInt] = Field(None, alias="implementationVersion")
     is_public: Optional[StrictBool] = Field(None, alias="isPublic", description="Whether this block is publicly available to Edge Impulse users (if false, then only for members of the owning organization)")
     is_public_for_devices: Optional[List[StrictStr]] = Field(None, alias="isPublicForDevices", description="If `isPublic` is true, the list of devices (from latencyDevices) for which this model can be shown.")
-    is_public_enterprise_only: Optional[StrictBool] = Field(None, alias="isPublicEnterpriseOnly", description="Whether this block is publicly available to Edge Impulse only to enterprise users")
+    public_project_tier_availability: Optional[PublicProjectTierAvailability] = Field(None, alias="publicProjectTierAvailability")
     repository_url: Optional[StrictStr] = Field(None, alias="repositoryUrl", description="URL to the source code of this custom learn block.")
     parameters: Optional[List[Dict[str, Any]]] = Field(None, description="List of parameters, spec'ed according to https://docs.edgeimpulse.com/docs/tips-and-tricks/adding-parameters-to-custom-blocks")
     image_input_scaling: Optional[ImageInputScaling] = Field(None, alias="imageInputScaling")
     ind_requires_gpu: Optional[StrictBool] = Field(None, alias="indRequiresGpu", description="If set, requires this block to be scheduled on GPU.")
     display_category: Optional[BlockDisplayCategory] = Field(None, alias="displayCategory")
-    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "isPublicEnterpriseOnly", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu", "displayCategory"]
+    __properties = ["name", "dockerContainer", "description", "operatesOn", "objectDetectionLastLayer", "implementationVersion", "isPublic", "isPublicForDevices", "publicProjectTierAvailability", "repositoryUrl", "parameters", "imageInputScaling", "indRequiresGpu", "displayCategory"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -80,15 +81,15 @@
             "docker_container": obj.get("dockerContainer"),
             "description": obj.get("description"),
             "operates_on": obj.get("operatesOn"),
             "object_detection_last_layer": obj.get("objectDetectionLastLayer"),
             "implementation_version": obj.get("implementationVersion"),
             "is_public": obj.get("isPublic"),
             "is_public_for_devices": obj.get("isPublicForDevices"),
-            "is_public_enterprise_only": obj.get("isPublicEnterpriseOnly"),
+            "public_project_tier_availability": obj.get("publicProjectTierAvailability"),
             "repository_url": obj.get("repositoryUrl"),
             "parameters": obj.get("parameters"),
             "image_input_scaling": obj.get("imageInputScaling"),
             "ind_requires_gpu": obj.get("indRequiresGpu"),
             "display_category": obj.get("displayCategory")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_organization_transformation_block_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_organization_transformation_block_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_project_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Any, Dict, List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr, validator
+from edgeimpulse_api.models.keras_model_variant_enum import KerasModelVariantEnum
 from edgeimpulse_api.models.project_visibility import ProjectVisibility
 
 class UpdateProjectRequest(BaseModel):
     logo: Optional[StrictStr] = Field(None, description="New logo URL, or set to `null` to remove the logo.")
     name: Optional[StrictStr] = Field(None, description="New project name.")
     description: Optional[StrictStr] = None
     project_visibility: Optional[ProjectVisibility] = Field(None, alias="projectVisibility")
@@ -54,15 +55,17 @@
     ind_pause_processing_samples: Optional[StrictBool] = Field(None, alias="indPauseProcessingSamples", description="Used in tests, to ensure samples that need to be processed async are not picked up until the flag is set to FALSE again.")
     show_sensor_data_in_acquisition_graph: Optional[StrictBool] = Field(None, alias="showSensorDataInAcquisitionGraph", description="Whether to show the actual sensor data in acquisition charts (only applies when you have structured labels)")
     last_deployment_target: Optional[StrictStr] = Field(None, alias="lastDeploymentTarget", description="Which deployment target was last selected (used to populate this deployment target again the next time you visit the deployment page). Should match the _format_ property of the response from listDeploymentTargetsForProject.")
     data_acquisition_page_size: Optional[StrictInt] = Field(None, alias="dataAcquisitionPageSize", description="Default page size on data acquisition")
     data_acquisition_view_type: Optional[StrictStr] = Field(None, alias="dataAcquisitionViewType", description="Default view type on data acquisition")
     data_acquisition_grid_column_count: Optional[StrictInt] = Field(None, alias="dataAcquisitionGridColumnCount", description="Number of grid columns in non-detailed view on data acquisition")
     data_acquisition_grid_column_count_detailed: Optional[StrictInt] = Field(None, alias="dataAcquisitionGridColumnCountDetailed", description="Number of grid columns in detailed view on data acquisition")
-    __properties = ["logo", "name", "description", "projectVisibility", "publicProjectListed", "lastDeployEonCompiler", "lastDeployModelEngine", "latencyDevice", "experiments", "showCreateFirstImpulse", "labelingMethod", "selectedProjectTypeInWizard", "gettingStartedStep", "useGpu", "computeTimeLimitM", "dspFileSizeMb", "enterprisePerformance", "trainJobRamMb", "metadata", "readme", "lastAcquisitionLabel", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "csvImportConfig", "inPretrainedModelFlow", "dspPageSize", "indPauseProcessingSamples", "showSensorDataInAcquisitionGraph", "lastDeploymentTarget", "dataAcquisitionPageSize", "dataAcquisitionViewType", "dataAcquisitionGridColumnCount", "dataAcquisitionGridColumnCountDetailed"]
+    default_profiling_variant: Optional[KerasModelVariantEnum] = Field(None, alias="defaultProfilingVariant")
+    enabled_model_profiling_variants: Optional[List[KerasModelVariantEnum]] = Field(None, alias="enabledModelProfilingVariants", description="Set of model variants enabled by default on the model testing and live classification pages.")
+    __properties = ["logo", "name", "description", "projectVisibility", "publicProjectListed", "lastDeployEonCompiler", "lastDeployModelEngine", "latencyDevice", "experiments", "showCreateFirstImpulse", "labelingMethod", "selectedProjectTypeInWizard", "gettingStartedStep", "useGpu", "computeTimeLimitM", "dspFileSizeMb", "enterprisePerformance", "trainJobRamMb", "metadata", "readme", "lastAcquisitionLabel", "trainJobNotificationUids", "dspJobNotificationUids", "modelTestingJobNotificationUids", "autoSegmenterJobNotificationUids", "exportJobNotificationUids", "csvImportConfig", "inPretrainedModelFlow", "dspPageSize", "indPauseProcessingSamples", "showSensorDataInAcquisitionGraph", "lastDeploymentTarget", "dataAcquisitionPageSize", "dataAcquisitionViewType", "dataAcquisitionGridColumnCount", "dataAcquisitionGridColumnCountDetailed", "defaultProfilingVariant", "enabledModelProfilingVariants"]
 
     @validator('labeling_method')
     def labeling_method_validate_enum(cls, v):
         if v is None:
             return v
 
         if v not in ('single_label', 'object_detection'):
@@ -153,11 +156,13 @@
             "dsp_page_size": obj.get("dspPageSize"),
             "ind_pause_processing_samples": obj.get("indPauseProcessingSamples"),
             "show_sensor_data_in_acquisition_graph": obj.get("showSensorDataInAcquisitionGraph"),
             "last_deployment_target": obj.get("lastDeploymentTarget"),
             "data_acquisition_page_size": obj.get("dataAcquisitionPageSize"),
             "data_acquisition_view_type": obj.get("dataAcquisitionViewType"),
             "data_acquisition_grid_column_count": obj.get("dataAcquisitionGridColumnCount"),
-            "data_acquisition_grid_column_count_detailed": obj.get("dataAcquisitionGridColumnCountDetailed")
+            "data_acquisition_grid_column_count_detailed": obj.get("dataAcquisitionGridColumnCountDetailed"),
+            "default_profiling_variant": obj.get("defaultProfilingVariant"),
+            "enabled_model_profiling_variants": obj.get("enabledModelProfilingVariants")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_project_tags_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_project_tags_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_colors_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_theme_colors_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_theme_logos_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_theme_logos_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_third_party_auth_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_third_party_auth_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_tuner_run_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_tuner_run_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_user_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_version_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,59 +13,53 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import List, Optional
-from pydantic import BaseModel, Field, StrictStr
+from typing import Optional
+from pydantic import BaseModel, StrictStr
 
-class UpdateUserRequest(BaseModel):
-    name: Optional[StrictStr] = Field(None, description="New full name")
-    job_title: Optional[StrictStr] = Field(None, alias="jobTitle", description="New job title")
-    company_name: Optional[StrictStr] = Field(None, alias="companyName", description="New company name")
-    experiments: Optional[List[StrictStr]] = Field(None, description="List of user experiments")
-    __properties = ["name", "jobTitle", "companyName", "experiments"]
+class UpdateVersionRequest(BaseModel):
+    description: Optional[StrictStr] = None
+    __properties = ["description"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateUserRequest:
-        """Create an instance of UpdateUserRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UpdateVersionRequest:
+        """Create an instance of UpdateVersionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateUserRequest:
-        """Create an instance of UpdateUserRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UpdateVersionRequest:
+        """Create an instance of UpdateVersionRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateUserRequest.construct(**obj)
+            return UpdateVersionRequest.construct(**obj)
 
-        _obj = UpdateUserRequest.construct(**{
-            "name": obj.get("name"),
-            "job_title": obj.get("jobTitle"),
-            "company_name": obj.get("companyName"),
-            "experiments": obj.get("experiments")
+        _obj = UpdateVersionRequest.construct(**{
+            "description": obj.get("description")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_version_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_asset_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,52 +14,56 @@
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UpdateVersionRequest(BaseModel):
-    description: Optional[StrictStr] = None
-    __properties = ["description"]
+class UploadAssetResponse(BaseModel):
+    success: StrictBool = Field(..., description="Whether the operation succeeded")
+    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+    url: Optional[StrictStr] = None
+    __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UpdateVersionRequest:
-        """Create an instance of UpdateVersionRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UpdateVersionRequest:
-        """Create an instance of UpdateVersionRequest from a dict"""
+    def from_dict(cls, obj: dict) -> UploadAssetResponse:
+        """Create an instance of UploadAssetResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UpdateVersionRequest.construct(**obj)
+            return UploadAssetResponse.construct(**obj)
 
-        _obj = UpdateVersionRequest.construct(**{
-            "description": obj.get("description")
+        _obj = UploadAssetResponse.construct(**{
+            "success": obj.get("success"),
+            "error": obj.get("error"),
+            "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_default_deployment_target_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_deployment_options_order_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_deployment_targets_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_learning_blocks_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/update_whitelabel_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/update_whitelabel_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_user_photo_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UploadAssetResponse(BaseModel):
+class UploadUserPhotoResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: Optional[StrictStr] = None
+    url: StrictStr = ...
     __properties = ["success", "error", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
@@ -35,35 +35,35 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadAssetResponse:
-        """Create an instance of UploadAssetResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
+        """Create an instance of UploadUserPhotoResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadAssetResponse.construct(**obj)
+            return UploadUserPhotoResponse.construct(**obj)
 
-        _obj = UploadAssetResponse.construct(**{
+        _obj = UploadUserPhotoResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_asset_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_asset_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_readme_image_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_readme_image_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_generate_new_mfa_key_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,54 +16,56 @@
 import re  # noqa: F401
 import json
 
 
 from typing import Optional
 from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UploadUserPhotoResponse(BaseModel):
+class UserGenerateNewMfaKeyResponse(BaseModel):
     success: StrictBool = Field(..., description="Whether the operation succeeded")
     error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
-    url: StrictStr = ...
-    __properties = ["success", "error", "url"]
+    key: StrictStr = Field(..., description="Secret key (use SHA-1).")
+    url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
+    __properties = ["success", "error", "key", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponse:
+        """Create an instance of UserGenerateNewMfaKeyResponse from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UploadUserPhotoResponse:
-        """Create an instance of UploadUserPhotoResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponse:
+        """Create an instance of UserGenerateNewMfaKeyResponse from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UploadUserPhotoResponse.construct(**obj)
+            return UserGenerateNewMfaKeyResponse.construct(**obj)
 
-        _obj = UploadUserPhotoResponse.construct(**{
+        _obj = UserGenerateNewMfaKeyResponse.construct(**{
             "success": obj.get("success"),
             "error": obj.get("error"),
+            "key": obj.get("key"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/upload_user_photo_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upload_user_photo_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import json
 
 from datetime import datetime
 from typing import List, Optional
 from pydantic import BaseModel, Field, StrictBool, StrictInt, StrictStr
 from edgeimpulse_api.models.permission import Permission
 from edgeimpulse_api.models.staff_info import StaffInfo
+from edgeimpulse_api.models.user_tier_enum import UserTierEnum
 
 class User(BaseModel):
     id: StrictInt = ...
     username: StrictStr = ...
     name: StrictStr = ...
     email: StrictStr = ...
     photo: Optional[StrictStr] = None
@@ -36,15 +37,16 @@
     job_title: Optional[StrictStr] = Field(None, alias="jobTitle")
     permissions: Optional[List[Permission]] = Field(None, description="List of permissions the user has")
     company_name: Optional[StrictStr] = Field(None, alias="companyName")
     activated: StrictBool = Field(..., description="Whether the user has activated their account or not.")
     mfa_configured: StrictBool = Field(..., alias="mfaConfigured", description="Whether the user has configured multi-factor authentication")
     stripe_customer_id: Optional[StrictStr] = Field(None, alias="stripeCustomerId", description="Stripe customer ID, if any.")
     has_pending_payments: Optional[StrictBool] = Field(None, alias="hasPendingPayments", description="Whether the user has pending payments.")
-    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments"]
+    tier: Optional[UserTierEnum] = None
+    __properties = ["id", "username", "name", "email", "photo", "created", "lastSeen", "staffInfo", "pending", "lastTosAcceptanceDate", "jobTitle", "permissions", "companyName", "activated", "mfaConfigured", "stripeCustomerId", "hasPendingPayments", "tier"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -92,11 +94,12 @@
             "last_tos_acceptance_date": obj.get("lastTosAcceptanceDate"),
             "job_title": obj.get("jobTitle"),
             "permissions": obj.get("permissions"),
             "company_name": obj.get("companyName"),
             "activated": obj.get("activated"),
             "mfa_configured": obj.get("mfaConfigured"),
             "stripe_customer_id": obj.get("stripeCustomerId"),
-            "has_pending_payments": obj.get("hasPendingPayments")
+            "has_pending_payments": obj.get("hasPendingPayments"),
+            "tier": obj.get("tier")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_by_third_party_activation_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_by_third_party_activation_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_delete_totp_mfa_key_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_dismiss_notification_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_dismiss_notification_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_experiment.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_experiment.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,59 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictBool, StrictStr
 
-class UserGenerateNewMfaKeyResponse(BaseModel):
-    success: StrictBool = Field(..., description="Whether the operation succeeded")
-    error: Optional[StrictStr] = Field(None, description="Optional error description (set if 'success' was false)")
+from pydantic import BaseModel, Field, StrictStr
+
+class UserGenerateNewMfaKeyResponseAllOf(BaseModel):
     key: StrictStr = Field(..., description="Secret key (use SHA-1).")
     url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
-    __properties = ["success", "error", "key", "url"]
+    __properties = ["key", "url"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponse:
-        """Create an instance of UserGenerateNewMfaKeyResponse from a JSON string"""
+    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponseAllOf:
+        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponse:
-        """Create an instance of UserGenerateNewMfaKeyResponse from a dict"""
+    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponseAllOf:
+        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserGenerateNewMfaKeyResponse.construct(**obj)
+            return UserGenerateNewMfaKeyResponseAllOf.construct(**obj)
 
-        _obj = UserGenerateNewMfaKeyResponse.construct(**{
-            "success": obj.get("success"),
-            "error": obj.get("error"),
+        _obj = UserGenerateNewMfaKeyResponseAllOf.construct(**{
             "key": obj.get("key"),
             "url": obj.get("url")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_generate_new_mfa_key_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,52 +16,52 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
 
-class UserGenerateNewMfaKeyResponseAllOf(BaseModel):
-    key: StrictStr = Field(..., description="Secret key (use SHA-1).")
-    url: StrictStr = Field(..., description="URL that will be converted into a QR code that can be scanned.")
-    __properties = ["key", "url"]
+class UserSetTotpMfaKeyRequest(BaseModel):
+    key: StrictStr = Field(..., description="Secret key obtained through `userGenerateNewMfaKey`.")
+    totp_token: StrictStr = Field(..., alias="totpToken", description="TOTP token that is valid for the key (to ensure the device is configured correctly)")
+    __properties = ["key", "totpToken"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserGenerateNewMfaKeyResponseAllOf:
-        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> UserSetTotpMfaKeyRequest:
+        """Create an instance of UserSetTotpMfaKeyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserGenerateNewMfaKeyResponseAllOf:
-        """Create an instance of UserGenerateNewMfaKeyResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> UserSetTotpMfaKeyRequest:
+        """Create an instance of UserSetTotpMfaKeyRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserGenerateNewMfaKeyResponseAllOf.construct(**obj)
+            return UserSetTotpMfaKeyRequest.construct(**obj)
 
-        _obj = UserGenerateNewMfaKeyResponseAllOf.construct(**{
+        _obj = UserSetTotpMfaKeyRequest.construct(**{
             "key": obj.get("key"),
-            "url": obj.get("url")
+            "totp_token": obj.get("totpToken")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_organization.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_organization.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     whitelabel_id: Optional[StrictInt] = Field(..., alias="whitelabelId", description="Unique identifier of the white label this project belongs to, if any.")
     is_admin: StrictBool = Field(..., alias="isAdmin", description="Whether the user is admin of this organization or not.")
     created: datetime = Field(..., description="When the organization was created.")
     trial_id: Optional[float] = Field(..., alias="trialId", description="Unique identifier of the trial this organization belongs to, if any.")
     trial_expired_date: Optional[datetime] = Field(..., alias="trialExpiredDate", description="Date when the trial expired, if any. A expired trial has a grace period of 30 days before it's associated organization is deleted.")
     trial_upgraded_date: Optional[datetime] = Field(..., alias="trialUpgradedDate", description="Date when the trial was upgraded to a full enterprise account, if any.")
     entitlement_limits: EntitlementLimits = Field(..., alias="entitlementLimits")
-    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId", "trialExpiredDate", "trialUpgradedDate", "entitlementLimits"]
+    user_count: StrictInt = Field(..., alias="userCount")
+    __properties = ["id", "name", "logo", "isDeveloperProfile", "whitelabelId", "isAdmin", "created", "trialId", "trialExpiredDate", "trialUpgradedDate", "entitlementLimits", "userCount"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -95,11 +96,12 @@
             "is_developer_profile": obj.get("isDeveloperProfile"),
             "whitelabel_id": obj.get("whitelabelId"),
             "is_admin": obj.get("isAdmin"),
             "created": obj.get("created"),
             "trial_id": obj.get("trialId"),
             "trial_expired_date": obj.get("trialExpiredDate"),
             "trial_upgraded_date": obj.get("trialUpgradedDate"),
-            "entitlement_limits": EntitlementLimits.from_dict(obj.get("entitlementLimits")) if obj.get("entitlementLimits") is not None else None
+            "entitlement_limits": EntitlementLimits.from_dict(obj.get("entitlementLimits")) if obj.get("entitlementLimits") is not None else None,
+            "user_count": obj.get("userCount")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_email_response_all_of.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,55 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictStr
 
-class UserSetTotpMfaKeyRequest(BaseModel):
-    key: StrictStr = Field(..., description="Secret key obtained through `userGenerateNewMfaKey`.")
-    totp_token: StrictStr = Field(..., alias="totpToken", description="TOTP token that is valid for the key (to ensure the device is configured correctly)")
-    __properties = ["key", "totpToken"]
+class VerifyEmailResponseAllOf(BaseModel):
+    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
+    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
+    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
+    __properties = ["email", "userId", "redirectUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserSetTotpMfaKeyRequest:
-        """Create an instance of UserSetTotpMfaKeyRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> UserSetTotpMfaKeyRequest:
-        """Create an instance of UserSetTotpMfaKeyRequest from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyEmailResponseAllOf:
+        """Create an instance of VerifyEmailResponseAllOf from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return UserSetTotpMfaKeyRequest.construct(**obj)
+            return VerifyEmailResponseAllOf.construct(**obj)
 
-        _obj = UserSetTotpMfaKeyRequest.construct(**{
-            "key": obj.get("key"),
-            "totp_token": obj.get("totpToken")
+        _obj = VerifyEmailResponseAllOf.construct(**{
+            "email": obj.get("email"),
+            "user_id": obj.get("userId"),
+            "redirect_url": obj.get("redirectUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/user_set_totp_mfa_key_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/user_tier_enum.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/feature.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UserTierEnum(str, Enum):
+class Feature(str, Enum):
     """
     allowed enum values
     """
 
-    FREE = 'free'
-    COMMUNITY_PLUS = 'community-plus'
-    PROFESSIONAL = 'professional'
+    SIGNUP_THANK_YOU_PAGE = 'signup-thank-you-page'
+    PROFESSIONAL_TIER = 'professional-tier'
+    STRIPE_LIVE_MODE = 'stripe-live-mode'
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_dsp_block_url_response_all_of_block.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_email_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_email_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictStr
 
-class VerifyEmailResponseAllOf(BaseModel):
-    email: Optional[StrictStr] = Field(None, description="Email address that was verified.")
-    user_id: Optional[float] = Field(None, alias="userId", description="ID of the user associated with the verified email address, if any.")
-    redirect_url: Optional[StrictStr] = Field(None, alias="redirectUrl", description="URL to redirect the user to after email verification.")
-    __properties = ["email", "userId", "redirectUrl"]
+from pydantic import BaseModel, Field, StrictInt, StrictStr
+
+class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
+    name: StrictStr = ...
+    size: StrictInt = ...
+    folder_name: StrictStr = Field(..., alias="folderName")
+    __properties = ["name", "size", "folderName"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyEmailResponseAllOf:
-        """Create an instance of VerifyEmailResponseAllOf from a JSON string"""
+    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyEmailResponseAllOf:
-        """Create an instance of VerifyEmailResponseAllOf from a dict"""
+    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
+        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyEmailResponseAllOf.construct(**obj)
+            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
 
-        _obj = VerifyEmailResponseAllOf.construct(**{
-            "email": obj.get("email"),
-            "user_id": obj.get("userId"),
-            "redirect_url": obj.get("redirectUrl")
+        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
+            "name": obj.get("name"),
+            "size": obj.get("size"),
+            "folder_name": obj.get("folderName")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_bucket_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_bucket_response_all_of_files.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,57 +13,57 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-
+from typing import Optional
 from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class VerifyOrganizationBucketResponseAllOfFiles(BaseModel):
-    name: StrictStr = ...
-    size: StrictInt = ...
-    folder_name: StrictStr = Field(..., alias="folderName")
-    __properties = ["name", "size", "folderName"]
+class WhitelabelAdminCreateOrganizationRequest(BaseModel):
+    organization_name: StrictStr = Field(..., alias="organizationName", description="The name of the organization.")
+    admin_id: Optional[StrictInt] = Field(None, alias="adminId", description="Unique identifier of the administrator of the new organization.")
+    admin_email: Optional[StrictStr] = Field(None, alias="adminEmail", description="Email of the administrator of the new organization.")
+    __properties = ["organizationName", "adminId", "adminEmail"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> VerifyOrganizationBucketResponseAllOfFiles:
-        """Create an instance of VerifyOrganizationBucketResponseAllOfFiles from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelAdminCreateOrganizationRequest:
+        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return VerifyOrganizationBucketResponseAllOfFiles.construct(**obj)
+            return WhitelabelAdminCreateOrganizationRequest.construct(**obj)
 
-        _obj = VerifyOrganizationBucketResponseAllOfFiles.construct(**{
-            "name": obj.get("name"),
-            "size": obj.get("size"),
-            "folder_name": obj.get("folderName")
+        _obj = WhitelabelAdminCreateOrganizationRequest.construct(**{
+            "organization_name": obj.get("organizationName"),
+            "admin_id": obj.get("adminId"),
+            "admin_email": obj.get("adminEmail")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_organization_existing_bucket_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_organization_existing_bucket_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/verify_reset_password_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/verify_reset_password_request.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_admin_create_organization_request.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,57 +13,55 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class WhitelabelAdminCreateOrganizationRequest(BaseModel):
-    organization_name: StrictStr = Field(..., alias="organizationName", description="The name of the organization.")
-    admin_id: Optional[StrictInt] = Field(None, alias="adminId", description="Unique identifier of the administrator of the new organization.")
-    admin_email: Optional[StrictStr] = Field(None, alias="adminEmail", description="Email of the administrator of the new organization.")
-    __properties = ["organizationName", "adminId", "adminEmail"]
+from pydantic import BaseModel, Field, StrictStr
+
+class WhitelabelAllLearningBlocksInner(BaseModel):
+    title: StrictStr = Field(..., description="The name of the learning block")
+    type: StrictStr = Field(..., description="The learning block type")
+    __properties = ["title", "type"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WhitelabelAdminCreateOrganizationRequest:
-        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelAllLearningBlocksInner:
+        """Create an instance of WhitelabelAllLearningBlocksInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WhitelabelAdminCreateOrganizationRequest:
-        """Create an instance of WhitelabelAdminCreateOrganizationRequest from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelAllLearningBlocksInner:
+        """Create an instance of WhitelabelAllLearningBlocksInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return WhitelabelAdminCreateOrganizationRequest.construct(**obj)
+            return WhitelabelAllLearningBlocksInner.construct(**obj)
 
-        _obj = WhitelabelAdminCreateOrganizationRequest.construct(**{
-            "organization_name": obj.get("organizationName"),
-            "admin_id": obj.get("adminId"),
-            "admin_email": obj.get("adminEmail")
+        _obj = WhitelabelAllLearningBlocksInner.construct(**{
+            "title": obj.get("title"),
+            "type": obj.get("type")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_all_learning_blocks_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,52 +16,52 @@
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
 
-class WhitelabelAllLearningBlocksInner(BaseModel):
-    title: StrictStr = Field(..., description="The name of the learning block")
-    type: StrictStr = Field(..., description="The learning block type")
-    __properties = ["title", "type"]
+class WhitelabelCustomDeploymentBlocksInner(BaseModel):
+    name: StrictStr = Field(..., description="The name of the custom deployment block")
+    id: float = Field(..., description="The custom deployment block ID")
+    __properties = ["name", "id"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WhitelabelAllLearningBlocksInner:
-        """Create an instance of WhitelabelAllLearningBlocksInner from a JSON string"""
+    def from_json(cls, json_str: str) -> WhitelabelCustomDeploymentBlocksInner:
+        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WhitelabelAllLearningBlocksInner:
-        """Create an instance of WhitelabelAllLearningBlocksInner from a dict"""
+    def from_dict(cls, obj: dict) -> WhitelabelCustomDeploymentBlocksInner:
+        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return WhitelabelAllLearningBlocksInner.construct(**obj)
+            return WhitelabelCustomDeploymentBlocksInner.construct(**obj)
 
-        _obj = WhitelabelAllLearningBlocksInner.construct(**{
-            "title": obj.get("title"),
-            "type": obj.get("type")
+        _obj = WhitelabelCustomDeploymentBlocksInner.construct(**{
+            "name": obj.get("name"),
+            "id": obj.get("id")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/whitelabel_custom_deployment_blocks_inner.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/upgrade_subscription_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,53 +15,56 @@
 import pprint
 import re  # noqa: F401
 import json
 
 
 
 from pydantic import BaseModel, Field, StrictStr
+from edgeimpulse_api.models.billing_cycle import BillingCycle
 
-class WhitelabelCustomDeploymentBlocksInner(BaseModel):
-    name: StrictStr = Field(..., description="The name of the custom deployment block")
-    id: float = Field(..., description="The custom deployment block ID")
-    __properties = ["name", "id"]
+class UpgradeSubscriptionRequest(BaseModel):
+    billing_cycle: BillingCycle = Field(..., alias="billingCycle")
+    success_url: StrictStr = Field(..., alias="successUrl", description="URL to redirect the user to after a successful checkout process.")
+    cancel_url: StrictStr = Field(..., alias="cancelUrl", description="URL to redirect the user to after the checkout process is canceled.")
+    __properties = ["billingCycle", "successUrl", "cancelUrl"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = False
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> WhitelabelCustomDeploymentBlocksInner:
-        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a JSON string"""
+    def from_json(cls, json_str: str) -> UpgradeSubscriptionRequest:
+        """Create an instance of UpgradeSubscriptionRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                           },
                           exclude_none=True)
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> WhitelabelCustomDeploymentBlocksInner:
-        """Create an instance of WhitelabelCustomDeploymentBlocksInner from a dict"""
+    def from_dict(cls, obj: dict) -> UpgradeSubscriptionRequest:
+        """Create an instance of UpgradeSubscriptionRequest from a dict"""
         if obj is None:
             return None
 
         if type(obj) is not dict:
-            return WhitelabelCustomDeploymentBlocksInner.construct(**obj)
+            return UpgradeSubscriptionRequest.construct(**obj)
 
-        _obj = WhitelabelCustomDeploymentBlocksInner.construct(**{
-            "name": obj.get("name"),
-            "id": obj.get("id")
+        _obj = UpgradeSubscriptionRequest.construct(**{
+            "billing_cycle": obj.get("billingCycle"),
+            "success_url": obj.get("successUrl"),
+            "cancel_url": obj.get("cancelUrl")
         })
         return _obj
```

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response_all_of.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/models/window_settings_response_all_of_window_settings.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/edgeimpulse_api/rest.py` & `edgeimpulse_api-1.50.0/edgeimpulse_api/rest.py`

 * *Files identical despite different names*

### Comparing `edgeimpulse_api-1.49.9/pyproject.toml` & `edgeimpulse_api-1.50.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgeimpulse-api"
-version = "1.49.9" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
+version = "1.50.0" #DO_NOT_CHANGE_REPLACED_BY_BUILD_SCRIPT
 description = "Python bindings for the Edge Impulse API."
 authors = ["EdgeImpulse Inc. <hello@edgeimpulse.com>"]
 license = "Apache-2.0"
 homepage = "https://edgeimpulse.com"
 documentation = "https://docs.edgeimpulse.com/reference/edge-impulse-api/edge-impulse-api"
 classifiers = [
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
```

### Comparing `edgeimpulse_api-1.49.9/PKG-INFO` & `edgeimpulse_api-1.50.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgeimpulse-api
-Version: 1.49.9
+Version: 1.50.0
 Summary: Python bindings for the Edge Impulse API.
 Home-page: https://edgeimpulse.com
 License: Apache-2.0
 Author: EdgeImpulse Inc.
 Author-email: hello@edgeimpulse.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

