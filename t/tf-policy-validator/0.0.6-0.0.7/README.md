# Comparing `tmp/tf_policy_validator-0.0.6.tar.gz` & `tmp/tf_policy_validator-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf_policy_validator-0.0.6.tar", max compression
+gzip compressed data, was "tf_policy_validator-0.0.7.tar", max compression
```

## Comparing `tf_policy_validator-0.0.6.tar` & `tf_policy_validator-0.0.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      927 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/LICENSE
--rw-r--r--   0        0        0    12410 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/README.md
--rw-r--r--   0        0        0        0 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/__init__.py
--rw-r--r--   0        0        0      207 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/application_error.py
--rw-r--r--   0        0        0     3257 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/argument_actions.py
--rw-r--r--   0        0        0      971 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/client.py
--rw-r--r--   0        0        0     5023 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/config/default.yaml
--rw-r--r--   0        0        0     1764 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/config.py
--rw-r--r--   0        0        0     7165 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_1.md
--rw-r--r--   0        0        0     3960 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_2.md
--rw-r--r--   0        0        0     2544 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/doc/example_report_3.md
--rw-r--r--   0        0        0    11266 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/iam_check.py
--rw-r--r--   0        0        0     1106 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/__init__.py
--rw-r--r--   0        0        0      258 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/account_config.py
--rw-r--r--   0        0        0     2850 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/findings.py
--rw-r--r--   0        0        0      350 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamCheck.py
--rw-r--r--   0        0        0    10434 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamPolicy.py
--rw-r--r--   0        0        0    10094 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/iamcheck_AccessAnalyzer.py
--rw-r--r--   0        0        0     5198 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/reporter.py
--rw-r--r--   0        0        0    20014 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/lib/tfPlan.py
--rw-r--r--   0        0        0     1666 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/parameters.py
--rw-r--r--   0        0        0       38 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/pytest.ini
--rw-r--r--   0        0        0        0 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/__init__.py
--rw-r--r--   0        0        0     1458 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/aws_iam_policy.tf
--rw-r--r--   0        0        0       61 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/findings.json
--rw-r--r--   0        0        0     1458 2024-04-01 18:17:55.606823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/test.tf
--rw-r--r--   0        0        0     8277 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/iam_policy/test_plan.json
--rw-r--r--   0        0        0     4437 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_findings.json
--rw-r--r--   0        0        0      205 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_reference_policy.json
--rw-r--r--   0        0        0     3038 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/test.tf
--rw-r--r--   0        0        0    15609 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/identity_policies/test_plan.json
--rw-r--r--   0        0        0      781 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_findings.json
--rw-r--r--   0        0        0      299 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_reference_policy.json
--rw-r--r--   0        0        0      816 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_findings.json
--rw-r--r--   0        0        0      197 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_reference_policy.json
--rw-r--r--   0        0        0     1240 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test.tf
--rw-r--r--   0        0        0     8765 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test_plan.json
--rw-r--r--   0        0        0      111 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/provider.tf
--rw-r--r--   0        0        0      798 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_findings.json
--rw-r--r--   0        0        0      237 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_reference_policy.json
--rw-r--r--   0        0        0      783 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_findings.json
--rw-r--r--   0        0        0      178 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_reference_policy.json
--rw-r--r--   0        0        0      724 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test.tf
--rw-r--r--   0        0        0     2520 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test_plan.json
--rw-r--r--   0        0        0     2299 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_accessAnalyzer.py
--rw-r--r--   0        0        0      244 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_policy.json
--rw-r--r--   0        0        0     8277 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_policy_accessanalyzer.json
--rw-r--r--   0        0        0     1061 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/test/test_tf_plan.py
--rw-r--r--   0        0        0      810 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/iam_check/tools/regex_patterns.py
--rw-r--r--   0        0        0     1121 2024-04-01 18:17:55.610823 tf_policy_validator-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    13358 1970-01-01 00:00:00.000000 tf_policy_validator-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      927 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/LICENSE
+-rw-r--r--   0        0        0    12420 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/iam_check/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/iam_check/application_error.py
+-rw-r--r--   0        0        0     3257 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/iam_check/argument_actions.py
+-rw-r--r--   0        0        0      971 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/iam_check/client.py
+-rw-r--r--   0        0        0     5023 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/config/default.yaml
+-rw-r--r--   0        0        0     1764 2024-05-21 21:19:37.810938 tf_policy_validator-0.0.7/iam_check/config.py
+-rw-r--r--   0        0        0     7165 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/doc/example_report_1.md
+-rw-r--r--   0        0        0     3960 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/doc/example_report_2.md
+-rw-r--r--   0        0        0     2544 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/doc/example_report_3.md
+-rw-r--r--   0        0        0    11266 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/iam_check.py
+-rw-r--r--   0        0        0     1106 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/__init__.py
+-rw-r--r--   0        0        0      258 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/account_config.py
+-rw-r--r--   0        0        0     2850 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/findings.py
+-rw-r--r--   0        0        0      350 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/iamCheck.py
+-rw-r--r--   0        0        0    10434 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/iamPolicy.py
+-rw-r--r--   0        0        0    10094 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/iamcheck_AccessAnalyzer.py
+-rw-r--r--   0        0        0     5198 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/reporter.py
+-rw-r--r--   0        0        0    20014 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/lib/tfPlan.py
+-rw-r--r--   0        0        0     1666 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/parameters.py
+-rw-r--r--   0        0        0       38 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/pytest.ini
+-rw-r--r--   0        0        0        0 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/__init__.py
+-rw-r--r--   0        0        0     1458 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/aws_iam_policy.tf
+-rw-r--r--   0        0        0       61 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/iam_policy/findings.json
+-rw-r--r--   0        0        0     1458 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/iam_policy/test.tf
+-rw-r--r--   0        0        0     8277 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/iam_policy/test_plan.json
+-rw-r--r--   0        0        0     4437 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/identity_policies/identity_findings.json
+-rw-r--r--   0        0        0      205 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/identity_policies/identity_reference_policy.json
+-rw-r--r--   0        0        0     3038 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/identity_policies/test.tf
+-rw-r--r--   0        0        0    15609 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/identity_policies/test_plan.json
+-rw-r--r--   0        0        0      781 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/identity_findings.json
+-rw-r--r--   0        0        0      299 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/identity_reference_policy.json
+-rw-r--r--   0        0        0      816 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/resource_findings.json
+-rw-r--r--   0        0        0      197 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/resource_reference_policy.json
+-rw-r--r--   0        0        0     1240 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/test.tf
+-rw-r--r--   0        0        0     8765 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/multiple_policies/test_plan.json
+-rw-r--r--   0        0        0      111 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/provider.tf
+-rw-r--r--   0        0        0      798 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/identity_findings.json
+-rw-r--r--   0        0        0      237 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/identity_reference_policy.json
+-rw-r--r--   0        0        0      783 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/resource_findings.json
+-rw-r--r--   0        0        0      178 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/resource_reference_policy.json
+-rw-r--r--   0        0        0      724 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/test.tf
+-rw-r--r--   0        0        0     2520 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/test_plan.json
+-rw-r--r--   0        0        0     2299 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/test_accessAnalyzer.py
+-rw-r--r--   0        0        0      244 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/test_policy.json
+-rw-r--r--   0        0        0     8277 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/test_policy_accessanalyzer.json
+-rw-r--r--   0        0        0     1061 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/test/test_tf_plan.py
+-rw-r--r--   0        0        0      810 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/iam_check/tools/regex_patterns.py
+-rw-r--r--   0        0        0     1122 2024-05-21 21:19:37.814937 tf_policy_validator-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0    13369 1970-01-01 00:00:00.000000 tf_policy_validator-0.0.7/PKG-INFO
```

### Comparing `tf_policy_validator-0.0.6/LICENSE` & `tf_policy_validator-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/README.md` & `tf_policy_validator-0.0.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,16 +71,16 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time.
-| --treat-finding-type-as-blocking | | ERROR,SECURITY_WARNING,WARNING,SUGGESTION,NONE | Specify which finding types should be treated as blocking. Other finding types are treated as nonblocking.  If the tool detects any blocking finding types, it will exit with a non-zero exit code.  If all findings are nonblocking or there are no findings, the tool exits with an exit code of 0.  Defaults to "ERROR" and "SECURITY_WARNING". Specify as a comma separated list of finding types that should be blocking. Pass "NONE" to ignore all findings. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time.
+| --treat-finding-type-as-blocking | | ERROR, SECURITY_WARNING, WARNING, SUGGESTION, NONE | Specify which finding types should be treated as blocking. Other finding types are treated as nonblocking.  If the tool detects any blocking finding types, it will exit with a non-zero exit code.  If all findings are nonblocking or there are no findings, the tool exits with an exit code of 0.  Defaults to "ERROR" and "SECURITY_WARNING". Specify as a comma separated list of finding types that should be blocking. Pass "NONE" to ignore all findings. |
 | --allow-external-principals | | ACCOUNT,ARN | A comma separated list of external principals that should be ignored.  Specify as a comma separated list of a 12 digit AWS account ID, a federated web identity user, a federated SAML user, or an ARN. Specify "*" to allow anonymous access. (e.g. 123456789123,arn:aws:iam::111111111111:role/MyOtherRole,graph.facebook.com) |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 **check-no-new-access**
 ```
 tf-policy-validator check-no-new-access --config iam_check/config/default.yaml --template-path iam_check/test/test_policy_accessanalyzer.json --region us-west-2 --reference-policy-type identity --reference-policy iam_check/test/test_policy.json
 ```
 Parses IAM identity-based and resource-based policies from Terraform templates. Then runs the policies through IAM Access Analyzer for a custom check against a reference policy. Returns the findings from the custom check in JSON format. Exits with a non-zero error code if any findings categorized as blocking, based on new access, are found in your template. Exits with an error code of zero if all findings are non-blocking or there are no findings. You can find examples for reference policies and learn how to set up and run a custom policy check for new access in the [IAM Access Analyzer custom policy checks samples](https://github.com/aws-samples/iam-access-analyzer-custom-policy-check-samples) repository on GitHub.
@@ -88,15 +88,15 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
 | --reference-policy | Yes | FILE_PATH.json | A JSON formatted file that specifies the path to the reference policy that is used for a permissions comparison.   |
 | --reference-policy-type | Yes | IDENTITY or RESOURCE | The policy type associated with the IAM policy under analysis and the reference policy.  |
 | --treat-findings-as-non-blocking | | | When not specified, the tool detects any findings, it will exit with a non-zero exit code. When specified, the tool exits with an exit code of 0. |
 | --exclude-resource-types | | aws_resource_type, aws_resource_type | List of comma-separated resource types. Resource types should be the same as terraform template resource names such as aws_iam_group_policy, aws_iam_role |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 
 **check-access-not-granted**
@@ -108,15 +108,15 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
 | --actions | Yes | ACTION,ACTION,ACTION | List of comma-separated actions. |
 | --treat-findings-as-non-blocking | | | When not specified, the tool detects any findings, it will exit with a non-zero exit code. When specified, the tool exits with an exit code of 0. |
 | --exclude-resource-types | | aws_resource_type, aws_resource_type | List of comma-separated resource types. Resource types should be the same as terraform template resource names such as aws_iam_group_policy, aws_iam_role |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 
 ### Example to check Terraform template
 ```
```

### Comparing `tf_policy_validator-0.0.6/iam_check/argument_actions.py` & `tf_policy_validator-0.0.7/iam_check/argument_actions.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/client.py` & `tf_policy_validator-0.0.7/iam_check/client.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/config/default.yaml` & `tf_policy_validator-0.0.7/iam_check/config/default.yaml`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/config.py` & `tf_policy_validator-0.0.7/iam_check/config.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/doc/example_report_1.md` & `tf_policy_validator-0.0.7/iam_check/doc/example_report_1.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/doc/example_report_2.md` & `tf_policy_validator-0.0.7/iam_check/doc/example_report_2.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/doc/example_report_3.md` & `tf_policy_validator-0.0.7/iam_check/doc/example_report_3.md`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/iam_check.py` & `tf_policy_validator-0.0.7/iam_check/iam_check.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/__init__.py` & `tf_policy_validator-0.0.7/iam_check/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/findings.py` & `tf_policy_validator-0.0.7/iam_check/lib/findings.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/iamPolicy.py` & `tf_policy_validator-0.0.7/iam_check/lib/iamPolicy.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/iamcheck_AccessAnalyzer.py` & `tf_policy_validator-0.0.7/iam_check/lib/iamcheck_AccessAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/reporter.py` & `tf_policy_validator-0.0.7/iam_check/lib/reporter.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/lib/tfPlan.py` & `tf_policy_validator-0.0.7/iam_check/lib/tfPlan.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/parameters.py` & `tf_policy_validator-0.0.7/iam_check/parameters.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/aws_iam_policy.tf` & `tf_policy_validator-0.0.7/iam_check/test/aws_iam_policy.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/iam_policy/test.tf` & `tf_policy_validator-0.0.7/iam_check/test/iam_policy/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/iam_policy/test_plan.json` & `tf_policy_validator-0.0.7/iam_check/test/iam_policy/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/identity_policies/identity_findings.json` & `tf_policy_validator-0.0.7/iam_check/test/identity_policies/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/identity_policies/test.tf` & `tf_policy_validator-0.0.7/iam_check/test/identity_policies/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/identity_policies/test_plan.json` & `tf_policy_validator-0.0.7/iam_check/test/identity_policies/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/identity_findings.json` & `tf_policy_validator-0.0.7/iam_check/test/multiple_policies/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/resource_findings.json` & `tf_policy_validator-0.0.7/iam_check/test/multiple_policies/resource_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test.tf` & `tf_policy_validator-0.0.7/iam_check/test/multiple_policies/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/multiple_policies/test_plan.json` & `tf_policy_validator-0.0.7/iam_check/test/multiple_policies/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/identity_findings.json` & `tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/identity_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/resource_findings.json` & `tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/resource_findings.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test.tf` & `tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/test.tf`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/role_inline_assume_policy/test_plan.json` & `tf_policy_validator-0.0.7/iam_check/test/role_inline_assume_policy/test_plan.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/test_accessAnalyzer.py` & `tf_policy_validator-0.0.7/iam_check/test/test_accessAnalyzer.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/test_policy_accessanalyzer.json` & `tf_policy_validator-0.0.7/iam_check/test/test_policy_accessanalyzer.json`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/test/test_tf_plan.py` & `tf_policy_validator-0.0.7/iam_check/test/test_tf_plan.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/iam_check/tools/regex_patterns.py` & `tf_policy_validator-0.0.7/iam_check/tools/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `tf_policy_validator-0.0.6/pyproject.toml` & `tf_policy_validator-0.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tf-policy-validator"
-version = "0.0.6"
+version = "0.0.7"
 description = "A command line tool that validates AWS IAM Policies in a Terraform template against AWS IAM best practices"
 authors = ["Policy Validator Maintainers <terraform-policy-validator@amazon.com>"]
 readme = "README.md"
 packages = [{include = "iam_check"}]
 license = "MIT-0"
 keywords = ["amazon", "aws", "aws-samples", "eks", "kubernetes", "upgrade", "iam_check"]
 classifiers = [
@@ -22,15 +22,15 @@
 ]
 
 [tool.poetry.scripts]
 tf-policy-validator = "iam_check.iam_check:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-boto3 = "^1.26.77"
+boto3 = "^1.34.110"
 pyyaml = "^6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
 [build-system]
```

### Comparing `tf_policy_validator-0.0.6/PKG-INFO` & `tf_policy_validator-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-policy-validator
-Version: 0.0.6
+Version: 0.0.7
 Summary: A command line tool that validates AWS IAM Policies in a Terraform template against AWS IAM best practices
 License: MIT-0
 Keywords: amazon,aws,aws-samples,eks,kubernetes,upgrade,iam_check
 Author: Policy Validator Maintainers
 Author-email: terraform-policy-validator@amazon.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: boto3 (>=1.26.77,<2.0.0)
+Requires-Dist: boto3 (>=1.34.110,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Description-Content-Type: text/markdown
 
 ## IAM Policy Validator for Terraform
 A command line tool that takes a Terraform template, parses IAM identity-based and resource-based policies, then runs them through [IAM Access Analyzer policy validation checks](https://docs.aws.amazon.com/IAM/latest/UserGuide/access-analyzer-reference-policy-checks.html) and (optionally) through IAM Access Analyzer custom policy checks. Note that a charge is associated with each custom policy check. For more details about pricing, see [IAM Access Analyzer pricing](https://aws.amazon.com/iam/access-analyzer/pricing/).
 
 ## Table of Contents<!-- omit in toc -->
@@ -93,16 +93,16 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time.
-| --treat-finding-type-as-blocking | | ERROR,SECURITY_WARNING,WARNING,SUGGESTION,NONE | Specify which finding types should be treated as blocking. Other finding types are treated as nonblocking.  If the tool detects any blocking finding types, it will exit with a non-zero exit code.  If all findings are nonblocking or there are no findings, the tool exits with an exit code of 0.  Defaults to "ERROR" and "SECURITY_WARNING". Specify as a comma separated list of finding types that should be blocking. Pass "NONE" to ignore all findings. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time.
+| --treat-finding-type-as-blocking | | ERROR, SECURITY_WARNING, WARNING, SUGGESTION, NONE | Specify which finding types should be treated as blocking. Other finding types are treated as nonblocking.  If the tool detects any blocking finding types, it will exit with a non-zero exit code.  If all findings are nonblocking or there are no findings, the tool exits with an exit code of 0.  Defaults to "ERROR" and "SECURITY_WARNING". Specify as a comma separated list of finding types that should be blocking. Pass "NONE" to ignore all findings. |
 | --allow-external-principals | | ACCOUNT,ARN | A comma separated list of external principals that should be ignored.  Specify as a comma separated list of a 12 digit AWS account ID, a federated web identity user, a federated SAML user, or an ARN. Specify "*" to allow anonymous access. (e.g. 123456789123,arn:aws:iam::111111111111:role/MyOtherRole,graph.facebook.com) |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 **check-no-new-access**
 ```
 tf-policy-validator check-no-new-access --config iam_check/config/default.yaml --template-path iam_check/test/test_policy_accessanalyzer.json --region us-west-2 --reference-policy-type identity --reference-policy iam_check/test/test_policy.json
 ```
 Parses IAM identity-based and resource-based policies from Terraform templates. Then runs the policies through IAM Access Analyzer for a custom check against a reference policy. Returns the findings from the custom check in JSON format. Exits with a non-zero error code if any findings categorized as blocking, based on new access, are found in your template. Exits with an error code of zero if all findings are non-blocking or there are no findings. You can find examples for reference policies and learn how to set up and run a custom policy check for new access in the [IAM Access Analyzer custom policy checks samples](https://github.com/aws-samples/iam-access-analyzer-custom-policy-check-samples) repository on GitHub.
@@ -110,15 +110,15 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
 | --reference-policy | Yes | FILE_PATH.json | A JSON formatted file that specifies the path to the reference policy that is used for a permissions comparison.   |
 | --reference-policy-type | Yes | IDENTITY or RESOURCE | The policy type associated with the IAM policy under analysis and the reference policy.  |
 | --treat-findings-as-non-blocking | | | When not specified, the tool detects any findings, it will exit with a non-zero exit code. When specified, the tool exits with an exit code of 0. |
 | --exclude-resource-types | | aws_resource_type, aws_resource_type | List of comma-separated resource types. Resource types should be the same as terraform template resource names such as aws_iam_group_policy, aws_iam_role |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 
 **check-access-not-granted**
@@ -130,15 +130,15 @@
 | Arguments | Required |  Options | Description |
 | --------- | -------- | ---------| ----------- |
 | --help  | | | show this help message and exit |
 | --template-path | | FILE_NAME | The path to the Terraform plan file (JSON). |
 | --region | Yes | REGION | The destination region the resources will be deployed to. |
 | --profile | | PROFILE | The named profile to use for AWS API calls. |
 | --enable-logging | | | Enables log output to stdout |
-| --ignore-finding | | FINDING_CODE,RESOURCE_NAME,RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
+| --ignore-finding | | FINDING_CODE, RESOURCE_NAME, RESOURCE_NAME.FINDING_CODE | Allow validation failures to be ignored. Specify as a comma separated list of findings to be ignored. Can be individual finding codes (e.g. "PASS_ROLE_WITH_STAR_IN_RESOURCE"), a specific resource name (e.g. "MyResource"), or a combination of both separated by a period.(e.g. "MyResource.PASS_ROLE_WITH_STAR_IN_RESOURCE").  Names of finding codes may change in IAM Access Analyzer over time. |
 | --actions | Yes | ACTION,ACTION,ACTION | List of comma-separated actions. |
 | --treat-findings-as-non-blocking | | | When not specified, the tool detects any findings, it will exit with a non-zero exit code. When specified, the tool exits with an exit code of 0. |
 | --exclude-resource-types | | aws_resource_type, aws_resource_type | List of comma-separated resource types. Resource types should be the same as terraform template resource names such as aws_iam_group_policy, aws_iam_role |
 | --config |Yes | FILE_NAME1, FILE_NAME2, ... | A list of config files for running this script |
 
 ### Example to check Terraform template
 ```
```

