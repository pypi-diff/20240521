# Comparing `tmp/django_appointment-3.5.1.tar.gz` & `tmp/django_appointment-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_appointment-3.5.1.tar", last modified: Sat May 18 19:24:27 2024, max compression
+gzip compressed data, was "django_appointment-3.5.2.tar", last modified: Tue May 21 12:26:01 2024, max compression
```

## Comparing `django_appointment-3.5.1.tar` & `django_appointment-3.5.2.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.029801 django_appointment-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-18 19:24:18.000000 django_appointment-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-18 19:24:18.000000 django_appointment-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-18 19:24:27.029801 django_appointment-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-05-18 19:24:18.000000 django_appointment-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.013801 django_appointment-3.5.1/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.013801 django_appointment-3.5.1/appointment/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/email_sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/email_sender/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/logger_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/messages_.py
--rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.005801 django_appointment-3.5.1/appointment/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.013801 django_appointment-3.5.1/appointment/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.013801 django_appointment-3.5.1/appointment/static/css/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/admin.css
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/btn.css
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/days_off.css
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/display_appointment.css
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/service.css
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/staff_member.css
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/user_profile.css
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/app_admin/working_hours.css
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/appointments-user-details.css
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/appointments.css
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/appt-common.css
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/thank_you.css
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/css/verification_code.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.013801 django_appointment-3.5.1/appointment/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/img/email_hd_bg.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.017801 django_appointment-3.5.1/appointment/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.017801 django_appointment-3.5.1/appointment/static/js/app_admin/
--rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/js/app_admin/staff_index.js
--rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/js/appointments.js
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/js/js-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.017801 django_appointment-3.5.1/appointment/static/js/modal/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/js/modal/error_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/static/js/modal/show_modal.js
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.005801 django_appointment-3.5.1/appointment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.017801 django_appointment-3.5.1/appointment/templates/administration/
--rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/display_appointment.html
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/email_change_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/manage_day_off.html
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/manage_service.html
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/manage_staff_member.html
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/manage_staff_personal_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/manage_working_hours.html
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/service_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/staff_index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/staff_list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/administration/user_profile.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/templates/appointment/
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/appointment_client_information.html
--rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/appointments.html
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/default_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/enter_verification_code.html
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/rescheduling_thank_you.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/set_password.html
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/appointment/thank_you.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/templates/base_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/base_templates/base.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/templates/email_sender/
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/email_sender/admin_new_appointment_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/email_sender/reminder_email.html
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/email_sender/reschedule_email.html
--rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/email_sender/thank_you_email.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/templates/error_pages/
--rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/error_pages/304_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/error_pages/403_forbidden.html
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/error_pages/403_forbidden_rescheduling.html
--rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/error_pages/404_not_found.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/templates/modal/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/modal/confirm_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/modal/error_modal.html
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/templates/modal/event_details_modal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.021801 django_appointment-3.5.1/appointment/tests/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/base/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.025801 django_appointment-3.5.1/appointment/tests/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/mixins/base_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.025801 django_appointment-3.5.1/appointment/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_appointment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_appointment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_appointment_reschedule_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_day_off.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_email_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_password_reset_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_payment_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_staff_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/models/test_working_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/test_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    56544 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.029801 django_appointment-3.5.1/appointment/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_staff_member_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/tests/utils/test_view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.029801 django_appointment-3.5.1/appointment/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/date_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    26916 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/db_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/email_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/json_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/utils/view_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/views.py
--rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-05-18 19:24:18.000000 django_appointment-3.5.1/appointment/views_admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 19:24:27.029801 django_appointment-3.5.1/django_appointment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-18 19:24:26.000000 django_appointment-3.5.1/django_appointment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-18 19:24:26.000000 django_appointment-3.5.1/django_appointment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 19:24:26.000000 django_appointment-3.5.1/django_appointment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-18 19:24:26.000000 django_appointment-3.5.1/django_appointment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 19:24:26.000000 django_appointment-3.5.1/django_appointment.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-18 19:24:18.000000 django_appointment-3.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-18 19:24:18.000000 django_appointment-3.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-18 19:24:27.033801 django_appointment-3.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-18 19:24:18.000000 django_appointment-3.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-21 12:25:49.000000 django_appointment-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-21 12:25:49.000000 django_appointment-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-21 12:26:01.048050 django_appointment-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13776 2024-05-21 12:25:49.000000 django_appointment-3.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.028050 django_appointment-3.5.2/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/email_sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/email_sender/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/logger_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/messages_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33603 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26946 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.024050 django_appointment-3.5.2/appointment/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/css/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/admin.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/btn.css
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/days_off.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/display_appointment.css
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/service.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/staff_member.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/user_profile.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/app_admin/working_hours.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appointments-user-details.css
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appointments.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/appt-common.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/thank_you.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/css/verification_code.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   119329 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/img/email_hd_bg.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/app_admin/
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/app_admin/staff_index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/appointments.js
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/js-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.032050 django_appointment-3.5.2/appointment/static/js/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/modal/error_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/static/js/modal/show_modal.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.024050 django_appointment-3.5.2/appointment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/administration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/display_appointment.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/email_change_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_day_off.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_service.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_staff_member.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_staff_personal_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9866 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/manage_working_hours.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/service_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    16047 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/staff_index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/staff_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15954 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/administration/user_profile.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/appointment/
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/appointment_client_information.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7809 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/appointments.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/default_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/enter_verification_code.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/rescheduling_thank_you.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/set_password.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/appointment/thank_you.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/base_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/base_templates/base.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.036050 django_appointment-3.5.2/appointment/templates/email_sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/admin_new_appointment_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/reminder_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/reschedule_email.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12601 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/email_sender/thank_you_email.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/templates/error_pages/
+-rw-r--r--   0 runner    (1001) docker     (127)    14602 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/304_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden_rescheduling.html
+-rw-r--r--   0 runner    (1001) docker     (127)    23059 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/error_pages/404_not_found.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/templates/modal/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/confirm_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/error_modal.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/templates/modal/event_details_modal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/base/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.040050 django_appointment-3.5.2/appointment/tests/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/mixins/base_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.044050 django_appointment-3.5.2/appointment/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11148 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_appointment_reschedule_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_day_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_email_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_password_reset_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_payment_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10589 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_staff_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/models/test_working_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41704 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56544 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.044050 django_appointment-3.5.2/appointment/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51195 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10575 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_staff_member_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/tests/utils/test_view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6985 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/appointment/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26916 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/db_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9997 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/email_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/json_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/utils/view_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27957 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24134 2024-05-21 12:25:49.000000 django_appointment-3.5.2/appointment/views_admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:26:01.048050 django_appointment-3.5.2/django_appointment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15374 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4847 2024-05-21 12:26:01.000000 django_appointment-3.5.2/django_appointment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-21 12:26:00.000000 django_appointment-3.5.2/django_appointment.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 12:25:49.000000 django_appointment-3.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 12:25:49.000000 django_appointment-3.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-21 12:26:01.048050 django_appointment-3.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-21 12:25:49.000000 django_appointment-3.5.2/setup.py
```

### Comparing `django_appointment-3.5.1/LICENSE` & `django_appointment-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/MANIFEST.in` & `django_appointment-3.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/PKG-INFO` & `django_appointment-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.5.1
+Version: 3.5.2
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
 Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
```

### Comparing `django_appointment-3.5.1/README.md` & `django_appointment-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/__init__.py` & `django_appointment-3.5.2/appointment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,9 +2,9 @@
 __author_email__ = "django-appt@adamspierredavid.com"
 __author_website__ = "https://adamspierredavid.com/"
 __description__ = "Managing appointment scheduling with customizable slots, staff features, and conflict handling."
 __package_name__ = "django-appointment"
 __url__ = "https://github.com/adamspd/django-appointment"
 __package_website__ = "https://django-appt.adamspierredavid.com/"
 __package_doc_url__ = "https://django-appt-doc.adamspierredavid.com/overview.html"
-__version__ = "3.5.1"
+__version__ = "3.5.2"
 __test_version__ = False
```

### Comparing `django_appointment-3.5.1/appointment/admin.py` & `django_appointment-3.5.2/appointment/admin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/decorators.py` & `django_appointment-3.5.2/appointment/decorators.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/email_sender/email_sender.py` & `django_appointment-3.5.2/appointment/email_sender/email_sender.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/forms.py` & `django_appointment-3.5.2/appointment/forms.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/messages_.py` & `django_appointment-3.5.2/appointment/messages_.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/models.py` & `django_appointment-3.5.2/appointment/models.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/services.py` & `django_appointment-3.5.2/appointment/services.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/settings.py` & `django_appointment-3.5.2/appointment/settings.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/admin.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/admin.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/btn.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/btn.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/days_off.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/days_off.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/display_appointment.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/display_appointment.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/service.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/service.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/staff_member.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/staff_member.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/user_profile.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/user_profile.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/app_admin/working_hours.css` & `django_appointment-3.5.2/appointment/static/css/app_admin/working_hours.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/appointments-user-details.css` & `django_appointment-3.5.2/appointment/static/css/appointments-user-details.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/appt-common.css` & `django_appointment-3.5.2/appointment/static/css/appt-common.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/thank_you.css` & `django_appointment-3.5.2/appointment/static/css/thank_you.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/css/verification_code.css` & `django_appointment-3.5.2/appointment/static/css/verification_code.css`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/img/email_hd_bg.jpg` & `django_appointment-3.5.2/appointment/static/img/email_hd_bg.jpg`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/js/app_admin/staff_index.js` & `django_appointment-3.5.2/appointment/static/js/app_admin/staff_index.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/js/appointments.js` & `django_appointment-3.5.2/appointment/static/js/appointments.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/js/modal/error_modal.js` & `django_appointment-3.5.2/appointment/static/js/modal/error_modal.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/static/js/modal/show_modal.js` & `django_appointment-3.5.2/appointment/static/js/modal/show_modal.js`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tasks.py` & `django_appointment-3.5.2/appointment/tasks.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/display_appointment.html` & `django_appointment-3.5.2/appointment/templates/administration/display_appointment.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/email_change_verification_code.html` & `django_appointment-3.5.2/appointment/templates/administration/email_change_verification_code.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/manage_day_off.html` & `django_appointment-3.5.2/appointment/templates/administration/manage_day_off.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/manage_service.html` & `django_appointment-3.5.2/appointment/templates/administration/manage_service.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/manage_staff_member.html` & `django_appointment-3.5.2/appointment/templates/administration/manage_staff_member.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/manage_staff_personal_info.html` & `django_appointment-3.5.2/appointment/templates/administration/manage_staff_personal_info.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/manage_working_hours.html` & `django_appointment-3.5.2/appointment/templates/administration/manage_working_hours.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/service_list.html` & `django_appointment-3.5.2/appointment/templates/administration/service_list.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/staff_index.html` & `django_appointment-3.5.2/appointment/templates/administration/staff_index.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/staff_list.html` & `django_appointment-3.5.2/appointment/templates/administration/staff_list.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/administration/user_profile.html` & `django_appointment-3.5.2/appointment/templates/administration/user_profile.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/appointment_client_information.html` & `django_appointment-3.5.2/appointment/templates/appointment/appointment_client_information.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/appointments.html` & `django_appointment-3.5.2/appointment/templates/appointment/appointments.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/default_thank_you.html` & `django_appointment-3.5.2/appointment/templates/appointment/default_thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/enter_verification_code.html` & `django_appointment-3.5.2/appointment/templates/appointment/enter_verification_code.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/rescheduling_thank_you.html` & `django_appointment-3.5.2/appointment/templates/appointment/rescheduling_thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/set_password.html` & `django_appointment-3.5.2/appointment/templates/appointment/set_password.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/appointment/thank_you.html` & `django_appointment-3.5.2/appointment/templates/appointment/thank_you.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/base_templates/base.html` & `django_appointment-3.5.2/appointment/templates/base_templates/base.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/email_sender/admin_new_appointment_email.html` & `django_appointment-3.5.2/appointment/templates/email_sender/admin_new_appointment_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/email_sender/reminder_email.html` & `django_appointment-3.5.2/appointment/templates/email_sender/reminder_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/email_sender/reschedule_email.html` & `django_appointment-3.5.2/appointment/templates/email_sender/reschedule_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/email_sender/thank_you_email.html` & `django_appointment-3.5.2/appointment/templates/email_sender/thank_you_email.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/error_pages/304_already_submitted.html` & `django_appointment-3.5.2/appointment/templates/error_pages/304_already_submitted.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/error_pages/403_forbidden.html` & `django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/error_pages/403_forbidden_rescheduling.html` & `django_appointment-3.5.2/appointment/templates/error_pages/403_forbidden_rescheduling.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/error_pages/404_not_found.html` & `django_appointment-3.5.2/appointment/templates/error_pages/404_not_found.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/modal/confirm_modal.html` & `django_appointment-3.5.2/appointment/templates/modal/confirm_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/modal/error_modal.html` & `django_appointment-3.5.2/appointment/templates/modal/error_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/templates/modal/event_details_modal.html` & `django_appointment-3.5.2/appointment/templates/modal/event_details_modal.html`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/base/base_test.py` & `django_appointment-3.5.2/appointment/tests/base/base_test.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/mixins/base_mixin.py` & `django_appointment-3.5.2/appointment/tests/mixins/base_mixin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_appointment.py` & `django_appointment-3.5.2/appointment/tests/models/test_appointment.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_appointment_request.py` & `django_appointment-3.5.2/appointment/tests/models/test_appointment_request.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_appointment_reschedule_history.py` & `django_appointment-3.5.2/appointment/tests/models/test_appointment_reschedule_history.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_config.py` & `django_appointment-3.5.2/appointment/tests/models/test_config.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_day_off.py` & `django_appointment-3.5.2/appointment/tests/models/test_day_off.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_email_verification.py` & `django_appointment-3.5.2/appointment/tests/models/test_email_verification.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_password_reset_token.py` & `django_appointment-3.5.2/appointment/tests/models/test_password_reset_token.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_payment_info.py` & `django_appointment-3.5.2/appointment/tests/models/test_payment_info.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_service.py` & `django_appointment-3.5.2/appointment/tests/models/test_service.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_staff_member.py` & `django_appointment-3.5.2/appointment/tests/models/test_staff_member.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/models/test_working_hours.py` & `django_appointment-3.5.2/appointment/tests/models/test_working_hours.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/test_services.py` & `django_appointment-3.5.2/appointment/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/test_settings.py` & `django_appointment-3.5.2/appointment/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/test_tasks.py` & `django_appointment-3.5.2/appointment/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/test_views.py` & `django_appointment-3.5.2/appointment/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_date_time.py` & `django_appointment-3.5.2/appointment/tests/utils/test_date_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_db_helpers.py` & `django_appointment-3.5.2/appointment/tests/utils/test_db_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_email_ops.py` & `django_appointment-3.5.2/appointment/tests/utils/test_email_ops.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_json_context.py` & `django_appointment-3.5.2/appointment/tests/utils/test_json_context.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_permissions.py` & `django_appointment-3.5.2/appointment/tests/utils/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_session.py` & `django_appointment-3.5.2/appointment/tests/utils/test_session.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_staff_member_time.py` & `django_appointment-3.5.2/appointment/tests/utils/test_staff_member_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_validators.py` & `django_appointment-3.5.2/appointment/tests/utils/test_validators.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/tests/utils/test_view_helpers.py` & `django_appointment-3.5.2/appointment/tests/utils/test_view_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/urls.py` & `django_appointment-3.5.2/appointment/urls.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/date_time.py` & `django_appointment-3.5.2/appointment/utils/date_time.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/db_helpers.py` & `django_appointment-3.5.2/appointment/utils/db_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/email_ops.py` & `django_appointment-3.5.2/appointment/utils/email_ops.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/error_codes.py` & `django_appointment-3.5.2/appointment/utils/error_codes.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/json_context.py` & `django_appointment-3.5.2/appointment/utils/json_context.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/permissions.py` & `django_appointment-3.5.2/appointment/utils/permissions.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/session.py` & `django_appointment-3.5.2/appointment/utils/session.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/utils/view_helpers.py` & `django_appointment-3.5.2/appointment/utils/view_helpers.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/views.py` & `django_appointment-3.5.2/appointment/views.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/appointment/views_admin.py` & `django_appointment-3.5.2/appointment/views_admin.py`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/django_appointment.egg-info/PKG-INFO` & `django_appointment-3.5.2/django_appointment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-appointment
-Version: 3.5.1
+Version: 3.5.2
 Summary: Managing appointment scheduling with customizable slots, staff features, and conflict handling.
 Home-page: https://github.com/adamspd/django-appointment
 Author: Adams Pierre David
 Author-email: django-appt@adamspierredavid.com
 License: Apache License 2.0
 Project-URL: Author's Website, https://adamspierredavid.com/
 Project-URL: Package's demo Website, https://django-appt.adamspierredavid.com/
```

### Comparing `django_appointment-3.5.1/django_appointment.egg-info/SOURCES.txt` & `django_appointment-3.5.2/django_appointment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/setup.cfg` & `django_appointment-3.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `django_appointment-3.5.1/setup.py` & `django_appointment-3.5.2/setup.py`

 * *Files identical despite different names*

