# Comparing `tmp/fathom_global_client_sdk-0.8.0-py3-none-any.whl.zip` & `tmp/fathom_global_client_sdk-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,338 +1,28 @@
-Zip file size: 909888 bytes, number of entries: 336
--rw-r--r--  2.0 unx      263 b- defN 23-Nov-17 10:06 fathom/__init__.py
--r-xr-xr-x  2.0 unx     1243 b- defN 23-Nov-17 10:08 fathom/api/v2/common_pb2.py
--r-xr-xr-x  2.0 unx    21359 b- defN 23-Nov-17 10:08 fathom/api/v2/fathom_pb2.py
--r-xr-xr-x  2.0 unx     7417 b- defN 23-Nov-17 10:08 fathom/api/v2/fathom_pb2.pyi
--r-xr-xr-x  2.0 unx     7973 b- defN 23-Nov-17 10:08 fathom/api/v2/fathom_pb2_grpc.py
--r-xr-xr-x  2.0 unx     9409 b- defN 23-Nov-17 10:08 fathom/api/v2/portfolio_pb2.py
--r-xr-xr-x  2.0 unx     3132 b- defN 23-Nov-17 10:08 fathom/api/v2/portfolio_pb2.pyi
--r-xr-xr-x  2.0 unx     6539 b- defN 23-Nov-17 10:08 fathom/api/v2/portfolio_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-17 10:06 fathom/sdk/__init__.py
--rw-r--r--  2.0 unx     4540 b- defN 23-Nov-17 10:06 fathom/sdk/client.py
--rw-r--r--  2.0 unx      713 b- defN 23-Nov-17 10:06 fathom/sdk/common.py
--rw-r--r--  2.0 unx     7279 b- defN 23-Nov-17 10:06 fathom/sdk/v1.py
--rw-r--r--  2.0 unx    10172 b- defN 23-Nov-17 10:06 fathom/sdk/v2.py
--r-xr-xr-x  2.0 unx     1297 b- defN 23-Nov-17 10:08 proto/data/data_pb2.py
--r-xr-xr-x  2.0 unx      556 b- defN 23-Nov-17 10:08 proto/data/data_pb2.pyi
--r-xr-xr-x  2.0 unx    19028 b- defN 23-Nov-17 10:08 proto/fathom/fathom_pb2.py
--r-xr-xr-x  2.0 unx     7069 b- defN 23-Nov-17 10:08 proto/fathom/fathom_pb2.pyi
--r-xr-xr-x  2.0 unx     6013 b- defN 23-Nov-17 10:08 proto/fathom/fathom_pb2_grpc.py
--r-xr-xr-x  2.0 unx     2967 b- defN 23-Nov-17 10:08 proto/geo/geo_pb2.py
--r-xr-xr-x  2.0 unx     1481 b- defN 23-Nov-17 10:08 proto/geo/geo_pb2.pyi
--r-xr-xr-x  2.0 unx     2712 b- defN 23-Nov-17 10:08 protoc_gen_openapiv2/options/annotations_pb2.py
--r-xr-xr-x  2.0 unx    19672 b- defN 23-Nov-17 10:08 protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/__init__.py
--rw-r--r--  2.0 unx      357 b- defN 23-Nov-03 12:54 site-packages/astunparse/__init__.py
--rw-r--r--  2.0 unx     1222 b- defN 23-Nov-03 12:54 site-packages/astunparse/__main__.py
--rw-r--r--  2.0 unx     1408 b- defN 23-Nov-03 12:54 site-packages/astunparse/printer.py
--rw-r--r--  2.0 unx    27426 b- defN 23-Nov-03 12:54 site-packages/astunparse/unparser.py
--rw-r--r--  2.0 unx       94 b- defN 23-Nov-03 12:54 site-packages/certifi/__init__.py
--rw-r--r--  2.0 unx      243 b- defN 23-Nov-03 12:54 site-packages/certifi/__main__.py
--rw-r--r--  2.0 unx     4219 b- defN 23-Nov-03 12:54 site-packages/certifi/core.py
--rw-r--r--  2.0 unx     1549 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/__init__.py
--rw-r--r--  2.0 unx    18624 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/api.py
--rw-r--r--  2.0 unx    20069 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/assets/__init__.py
--rw-r--r--  2.0 unx    12554 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/cd.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/cli/__init__.py
--rw-r--r--  2.0 unx     9744 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/cli/normalizer.py
--rw-r--r--  2.0 unx    19101 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/constant.py
--rw-r--r--  2.0 unx     2071 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/legacy.py
--rw-r--r--  2.0 unx    18258 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/md.py
--rw-r--r--  2.0 unx    11492 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/models.py
--rw-r--r--  2.0 unx    11544 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/utils.py
--rw-r--r--  2.0 unx       79 b- defN 23-Nov-03 12:54 site-packages/charset_normalizer/version.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/google/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/api/__init__.py
--rw-r--r--  2.0 unx     2133 b- defN 23-Nov-03 12:53 site-packages/google/api/annotations_pb2.py
--rw-r--r--  2.0 unx     5569 b- defN 23-Nov-03 12:53 site-packages/google/api/auth_pb2.py
--rw-r--r--  2.0 unx     3477 b- defN 23-Nov-03 12:53 site-packages/google/api/backend_pb2.py
--rw-r--r--  2.0 unx     3034 b- defN 23-Nov-03 12:53 site-packages/google/api/billing_pb2.py
--rw-r--r--  2.0 unx     2623 b- defN 23-Nov-03 12:53 site-packages/google/api/client_pb2.py
--rw-r--r--  2.0 unx     3374 b- defN 23-Nov-03 12:53 site-packages/google/api/config_change_pb2.py
--rw-r--r--  2.0 unx     3138 b- defN 23-Nov-03 12:53 site-packages/google/api/consumer_pb2.py
--rw-r--r--  2.0 unx     2844 b- defN 23-Nov-03 12:53 site-packages/google/api/context_pb2.py
--rw-r--r--  2.0 unx     2122 b- defN 23-Nov-03 12:53 site-packages/google/api/control_pb2.py
--rw-r--r--  2.0 unx     7845 b- defN 23-Nov-03 12:53 site-packages/google/api/distribution_pb2.py
--rw-r--r--  2.0 unx     3698 b- defN 23-Nov-03 12:53 site-packages/google/api/documentation_pb2.py
--rw-r--r--  2.0 unx     2380 b- defN 23-Nov-03 12:53 site-packages/google/api/endpoint_pb2.py
--rw-r--r--  2.0 unx     3449 b- defN 23-Nov-03 12:53 site-packages/google/api/error_reason_pb2.py
--rw-r--r--  2.0 unx     2824 b- defN 23-Nov-03 12:53 site-packages/google/api/field_behavior_pb2.py
--rw-r--r--  2.0 unx     3701 b- defN 23-Nov-03 12:53 site-packages/google/api/http_pb2.py
--rw-r--r--  2.0 unx     2344 b- defN 23-Nov-03 12:53 site-packages/google/api/httpbody_pb2.py
--rw-r--r--  2.0 unx     2581 b- defN 23-Nov-03 12:53 site-packages/google/api/label_pb2.py
--rw-r--r--  2.0 unx     2277 b- defN 23-Nov-03 12:53 site-packages/google/api/launch_stage_pb2.py
--rw-r--r--  2.0 unx     2402 b- defN 23-Nov-03 12:53 site-packages/google/api/log_pb2.py
--rw-r--r--  2.0 unx     3014 b- defN 23-Nov-03 12:53 site-packages/google/api/logging_pb2.py
--rw-r--r--  2.0 unx     6432 b- defN 23-Nov-03 12:53 site-packages/google/api/metric_pb2.py
--rw-r--r--  2.0 unx     6324 b- defN 23-Nov-03 12:53 site-packages/google/api/monitored_resource_pb2.py
--rw-r--r--  2.0 unx     3129 b- defN 23-Nov-03 12:53 site-packages/google/api/monitoring_pb2.py
--rw-r--r--  2.0 unx     5303 b- defN 23-Nov-03 12:53 site-packages/google/api/quota_pb2.py
--rw-r--r--  2.0 unx     4870 b- defN 23-Nov-03 12:53 site-packages/google/api/resource_pb2.py
--rw-r--r--  2.0 unx     3189 b- defN 23-Nov-03 12:53 site-packages/google/api/routing_pb2.py
--rw-r--r--  2.0 unx     6280 b- defN 23-Nov-03 12:53 site-packages/google/api/service_pb2.py
--rw-r--r--  2.0 unx     2292 b- defN 23-Nov-03 12:53 site-packages/google/api/source_info_pb2.py
--rw-r--r--  2.0 unx     3583 b- defN 23-Nov-03 12:53 site-packages/google/api/system_parameter_pb2.py
--rw-r--r--  2.0 unx     2791 b- defN 23-Nov-03 12:53 site-packages/google/api/usage_pb2.py
--rw-r--r--  2.0 unx     4956 b- defN 23-Nov-03 12:53 site-packages/google/api/visibility_pb2.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/google/cloud/__init__.py
--rw-r--r--  2.0 unx     4032 b- defN 23-Nov-03 12:53 site-packages/google/cloud/extended_operations_pb2.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/google/cloud/location/__init__.py
--rw-r--r--  2.0 unx     6899 b- defN 23-Nov-03 12:53 site-packages/google/cloud/location/locations_pb2.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/google/gapic/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/gapic/metadata/__init__.py
--rw-r--r--  2.0 unx     8346 b- defN 23-Nov-03 12:53 site-packages/google/gapic/metadata/gapic_metadata_pb2.py
--rw-r--r--  2.0 unx      149 b- defN 23-Nov-03 12:53 site-packages/google/logging/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/logging/type/__init__.py
--rw-r--r--  2.0 unx     3176 b- defN 23-Nov-03 12:53 site-packages/google/logging/type/http_request_pb2.py
--rw-r--r--  2.0 unx     2622 b- defN 23-Nov-03 12:53 site-packages/google/logging/type/log_severity_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/__init__.py
--rw-r--r--  2.0 unx      797 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_grpc.py
--rw-r--r--  2.0 unx      914 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_grpc_pb2.py
--rw-r--r--  2.0 unx     2253 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_pb2.py
--rw-r--r--  2.0 unx    14464 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_pb2_grpc.py
--rw-r--r--  2.0 unx      222 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_proto.py
--rw-r--r--  2.0 unx    10431 b- defN 23-Nov-03 12:53 site-packages/google/longrunning/operations_proto_pb2.py
--rw-r--r--  2.0 unx     1705 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/__init__.py
--rw-r--r--  2.0 unx     1355 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/any_pb2.py
--rw-r--r--  2.0 unx     2539 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/api_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/compiler/__init__.py
--rw-r--r--  2.0 unx     2740 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/compiler/plugin_pb2.py
--rw-r--r--  2.0 unx    46474 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/descriptor.py
--rw-r--r--  2.0 unx     6819 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/descriptor_database.py
--rw-r--r--  2.0 unx   109072 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/descriptor_pb2.py
--rw-r--r--  2.0 unx    47281 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/descriptor_pool.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/duration_pb2.py
--rw-r--r--  2.0 unx     1319 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/empty_pb2.py
--rw-r--r--  2.0 unx     1401 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/field_mask_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/__init__.py
--rw-r--r--  2.0 unx     4562 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/api_implementation.py
--rw-r--r--  2.0 unx     5188 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/builder.py
--rw-r--r--  2.0 unx    23328 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/containers.py
--rw-r--r--  2.0 unx    37567 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/decoder.py
--rw-r--r--  2.0 unx    28656 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/encoder.py
--rw-r--r--  2.0 unx     4821 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/enum_type_wrapper.py
--rw-r--r--  2.0 unx     8443 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/extension_dict.py
--rw-r--r--  2.0 unx     3367 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/message_listener.py
--rw-r--r--  2.0 unx    58146 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/python_message.py
--rw-r--r--  2.0 unx    16912 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/type_checkers.py
--rw-r--r--  2.0 unx    30014 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/well_known_types.py
--rw-r--r--  2.0 unx     8444 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/internal/wire_format.py
--rw-r--r--  2.0 unx    35664 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/json_format.py
--rw-r--r--  2.0 unx    14523 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/message.py
--rw-r--r--  2.0 unx     7482 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/message_factory.py
--rw-r--r--  2.0 unx     5506 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/proto_builder.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/pyext/__init__.py
--rw-r--r--  2.0 unx     2851 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/pyext/cpp_message.py
--rw-r--r--  2.0 unx     3779 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/reflection.py
--rw-r--r--  2.0 unx     9146 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/service.py
--rw-r--r--  2.0 unx    11417 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/service_reflection.py
--rw-r--r--  2.0 unx     1416 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/source_context_pb2.py
--rw-r--r--  2.0 unx     2477 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/struct_pb2.py
--rw-r--r--  2.0 unx     6944 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/symbol_database.py
--rw-r--r--  2.0 unx     4728 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/text_encoding.py
--rw-r--r--  2.0 unx    60006 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/text_format.py
--rw-r--r--  2.0 unx     1439 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/timestamp_pb2.py
--rw-r--r--  2.0 unx     4425 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/type_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/util/__init__.py
--rw-r--r--  2.0 unx     6124 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/util/json_format_pb2.py
--rw-r--r--  2.0 unx    14095 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/util/json_format_proto3_pb2.py
--rw-r--r--  2.0 unx     2410 b- defN 23-Nov-03 12:53 site-packages/google/protobuf/wrappers_pb2.py
--rw-r--r--  2.0 unx      774 b- defN 23-Nov-03 12:53 site-packages/google/rpc/__init__.py
--rw-r--r--  2.0 unx     2707 b- defN 23-Nov-03 12:53 site-packages/google/rpc/code_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/rpc/context/__init__.py
--rw-r--r--  2.0 unx    14660 b- defN 23-Nov-03 12:53 site-packages/google/rpc/context/attribute_context_pb2.py
--rw-r--r--  2.0 unx    11094 b- defN 23-Nov-03 12:53 site-packages/google/rpc/error_details_pb2.py
--rw-r--r--  2.0 unx     2302 b- defN 23-Nov-03 12:53 site-packages/google/rpc/status_pb2.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/google/type/__init__.py
--rw-r--r--  2.0 unx     2343 b- defN 23-Nov-03 12:53 site-packages/google/type/calendar_period_pb2.py
--rw-r--r--  2.0 unx     2343 b- defN 23-Nov-03 12:53 site-packages/google/type/color_pb2.py
--rw-r--r--  2.0 unx     2138 b- defN 23-Nov-03 12:53 site-packages/google/type/date_pb2.py
--rw-r--r--  2.0 unx     3165 b- defN 23-Nov-03 12:53 site-packages/google/type/datetime_pb2.py
--rw-r--r--  2.0 unx     2278 b- defN 23-Nov-03 12:53 site-packages/google/type/dayofweek_pb2.py
--rw-r--r--  2.0 unx     2132 b- defN 23-Nov-03 12:53 site-packages/google/type/decimal_pb2.py
--rw-r--r--  2.0 unx     2153 b- defN 23-Nov-03 12:53 site-packages/google/type/expr_pb2.py
--rw-r--r--  2.0 unx     2166 b- defN 23-Nov-03 12:53 site-packages/google/type/fraction_pb2.py
--rw-r--r--  2.0 unx     2364 b- defN 23-Nov-03 12:53 site-packages/google/type/interval_pb2.py
--rw-r--r--  2.0 unx     2144 b- defN 23-Nov-03 12:53 site-packages/google/type/latlng_pb2.py
--rw-r--r--  2.0 unx     2270 b- defN 23-Nov-03 12:53 site-packages/google/type/localized_text_pb2.py
--rw-r--r--  2.0 unx     2151 b- defN 23-Nov-03 12:53 site-packages/google/type/money_pb2.py
--rw-r--r--  2.0 unx     2398 b- defN 23-Nov-03 12:53 site-packages/google/type/month_pb2.py
--rw-r--r--  2.0 unx     3046 b- defN 23-Nov-03 12:53 site-packages/google/type/phone_number_pb2.py
--rw-r--r--  2.0 unx     2654 b- defN 23-Nov-03 12:53 site-packages/google/type/postal_address_pb2.py
--rw-r--r--  2.0 unx     2261 b- defN 23-Nov-03 12:53 site-packages/google/type/quaternion_pb2.py
--rw-r--r--  2.0 unx     2266 b- defN 23-Nov-03 12:53 site-packages/google/type/timeofday_pb2.py
--rw-r--r--  2.0 unx    82896 b- defN 23-Nov-03 12:53 site-packages/grpc/__init__.py
--rw-r--r--  2.0 unx     2135 b- defN 23-Nov-03 12:53 site-packages/grpc/_auth.py
--rw-r--r--  2.0 unx    63514 b- defN 23-Nov-03 12:53 site-packages/grpc/_channel.py
--rw-r--r--  2.0 unx     6254 b- defN 23-Nov-03 12:53 site-packages/grpc/_common.py
--rw-r--r--  2.0 unx     1695 b- defN 23-Nov-03 12:53 site-packages/grpc/_compression.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/_cython/__init__.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/_cython/_cygrpc/__init__.py
--rw-r--r--  2.0 unx       26 b- defN 23-Nov-03 12:53 site-packages/grpc/_grpcio_metadata.py
--rw-r--r--  2.0 unx    20367 b- defN 23-Nov-03 12:53 site-packages/grpc/_interceptor.py
--rw-r--r--  2.0 unx     3916 b- defN 23-Nov-03 12:53 site-packages/grpc/_plugin_wrapping.py
--rw-r--r--  2.0 unx     5564 b- defN 23-Nov-03 12:53 site-packages/grpc/_runtime_protos.py
--rw-r--r--  2.0 unx    37668 b- defN 23-Nov-03 12:53 site-packages/grpc/_server.py
--rw-r--r--  2.0 unx    23408 b- defN 23-Nov-03 12:53 site-packages/grpc/_simple_stubs.py
--rw-r--r--  2.0 unx     5180 b- defN 23-Nov-03 12:53 site-packages/grpc/_utilities.py
--rw-r--r--  2.0 unx     3160 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/__init__.py
--rw-r--r--  2.0 unx     7313 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_base_call.py
--rw-r--r--  2.0 unx    13229 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_base_channel.py
--rw-r--r--  2.0 unx    12188 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_base_server.py
--rw-r--r--  2.0 unx    24469 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_call.py
--rw-r--r--  2.0 unx    20174 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_channel.py
--rw-r--r--  2.0 unx    40008 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_interceptor.py
--rw-r--r--  2.0 unx     4570 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_metadata.py
--rw-r--r--  2.0 unx     8699 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_server.py
--rw-r--r--  2.0 unx     1363 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_typing.py
--rw-r--r--  2.0 unx      821 b- defN 23-Nov-03 12:53 site-packages/grpc/aio/_utils.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/__init__.py
--rw-r--r--  2.0 unx    27512 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/_client_adaptations.py
--rw-r--r--  2.0 unx     1606 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/_metadata.py
--rw-r--r--  2.0 unx    13817 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/_server_adaptations.py
--rw-r--r--  2.0 unx    11822 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/implementations.py
--rw-r--r--  2.0 unx     5955 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/interfaces.py
--rw-r--r--  2.0 unx     4933 b- defN 23-Nov-03 12:53 site-packages/grpc/beta/utilities.py
--rw-r--r--  2.0 unx     4058 b- defN 23-Nov-03 12:53 site-packages/grpc/experimental/__init__.py
--rw-r--r--  2.0 unx      660 b- defN 23-Nov-03 12:53 site-packages/grpc/experimental/aio/__init__.py
--rw-r--r--  2.0 unx      973 b- defN 23-Nov-03 12:53 site-packages/grpc/experimental/gevent.py
--rw-r--r--  2.0 unx     1533 b- defN 23-Nov-03 12:53 site-packages/grpc/experimental/session_cache.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/__init__.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/common/__init__.py
--rw-r--r--  2.0 unx      988 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/common/cardinality.py
--rw-r--r--  2.0 unx      824 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/common/style.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/__init__.py
--rw-r--r--  2.0 unx      872 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/abandonment.py
--rw-r--r--  2.0 unx     3151 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/callable_util.py
--rw-r--r--  2.0 unx     8091 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/future.py
--rw-r--r--  2.0 unx     2276 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/logging_pool.py
--rw-r--r--  2.0 unx     1389 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/stream.py
--rw-r--r--  2.0 unx     4772 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/foundation/stream_util.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/__init__.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/base/__init__.py
--rw-r--r--  2.0 unx    12046 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/base/base.py
--rw-r--r--  2.0 unx     2455 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/base/utilities.py
--rw-r--r--  2.0 unx      577 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/face/__init__.py
--rw-r--r--  2.0 unx    39620 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/face/face.py
--rw-r--r--  2.0 unx     6711 b- defN 23-Nov-03 12:53 site-packages/grpc/framework/interfaces/face/utilities.py
--rw-r--r--  2.0 unx      849 b- defN 23-Nov-03 12:54 site-packages/idna/__init__.py
--rw-r--r--  2.0 unx     3374 b- defN 23-Nov-03 12:54 site-packages/idna/codec.py
--rw-r--r--  2.0 unx      321 b- defN 23-Nov-03 12:54 site-packages/idna/compat.py
--rw-r--r--  2.0 unx    12950 b- defN 23-Nov-03 12:54 site-packages/idna/core.py
--rw-r--r--  2.0 unx    44375 b- defN 23-Nov-03 12:54 site-packages/idna/idnadata.py
--rw-r--r--  2.0 unx     1881 b- defN 23-Nov-03 12:54 site-packages/idna/intranges.py
--rw-r--r--  2.0 unx       21 b- defN 23-Nov-03 12:54 site-packages/idna/package_data.py
--rw-r--r--  2.0 unx   206539 b- defN 23-Nov-03 12:54 site-packages/idna/uts46data.py
--rw-r--r--  2.0 unx     1927 b- defN 23-Nov-03 12:54 site-packages/jinja2/__init__.py
--rw-r--r--  2.0 unx     1958 b- defN 23-Nov-03 12:54 site-packages/jinja2/_identifier.py
--rw-r--r--  2.0 unx     2472 b- defN 23-Nov-03 12:54 site-packages/jinja2/async_utils.py
--rw-r--r--  2.0 unx    14061 b- defN 23-Nov-03 12:54 site-packages/jinja2/bccache.py
--rw-r--r--  2.0 unx    72172 b- defN 23-Nov-03 12:54 site-packages/jinja2/compiler.py
--rw-r--r--  2.0 unx     1433 b- defN 23-Nov-03 12:54 site-packages/jinja2/constants.py
--rw-r--r--  2.0 unx     6299 b- defN 23-Nov-03 12:54 site-packages/jinja2/debug.py
--rw-r--r--  2.0 unx     1267 b- defN 23-Nov-03 12:54 site-packages/jinja2/defaults.py
--rw-r--r--  2.0 unx    61349 b- defN 23-Nov-03 12:54 site-packages/jinja2/environment.py
--rw-r--r--  2.0 unx     5071 b- defN 23-Nov-03 12:54 site-packages/jinja2/exceptions.py
--rw-r--r--  2.0 unx    31502 b- defN 23-Nov-03 12:54 site-packages/jinja2/ext.py
--rw-r--r--  2.0 unx    53509 b- defN 23-Nov-03 12:54 site-packages/jinja2/filters.py
--rw-r--r--  2.0 unx    10704 b- defN 23-Nov-03 12:54 site-packages/jinja2/idtracking.py
--rw-r--r--  2.0 unx    29726 b- defN 23-Nov-03 12:54 site-packages/jinja2/lexer.py
--rw-r--r--  2.0 unx    23207 b- defN 23-Nov-03 12:54 site-packages/jinja2/loaders.py
--rw-r--r--  2.0 unx     4396 b- defN 23-Nov-03 12:54 site-packages/jinja2/meta.py
--rw-r--r--  2.0 unx     4226 b- defN 23-Nov-03 12:54 site-packages/jinja2/nativetypes.py
--rw-r--r--  2.0 unx    34550 b- defN 23-Nov-03 12:54 site-packages/jinja2/nodes.py
--rw-r--r--  2.0 unx     1650 b- defN 23-Nov-03 12:54 site-packages/jinja2/optimizer.py
--rw-r--r--  2.0 unx    39595 b- defN 23-Nov-03 12:54 site-packages/jinja2/parser.py
--rw-r--r--  2.0 unx    33476 b- defN 23-Nov-03 12:54 site-packages/jinja2/runtime.py
--rw-r--r--  2.0 unx    14584 b- defN 23-Nov-03 12:54 site-packages/jinja2/sandbox.py
--rw-r--r--  2.0 unx     5905 b- defN 23-Nov-03 12:54 site-packages/jinja2/tests.py
--rw-r--r--  2.0 unx    23965 b- defN 23-Nov-03 12:54 site-packages/jinja2/utils.py
--rw-r--r--  2.0 unx     3568 b- defN 23-Nov-03 12:54 site-packages/jinja2/visitor.py
--rw-r--r--  2.0 unx     9306 b- defN 23-Nov-03 12:54 site-packages/markupsafe/__init__.py
--rw-r--r--  2.0 unx     1713 b- defN 23-Nov-03 12:54 site-packages/markupsafe/_native.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:53 site-packages/protoc_gen_validate/__init__.py
--rw-r--r--  2.0 unx    50287 b- defN 23-Nov-03 12:53 site-packages/protoc_gen_validate/validator.py
--rw-r--r--  2.0 unx     4963 b- defN 23-Nov-03 12:53 site-packages/requests/__init__.py
--rw-r--r--  2.0 unx      435 b- defN 23-Nov-03 12:53 site-packages/requests/__version__.py
--rw-r--r--  2.0 unx     1495 b- defN 23-Nov-03 12:53 site-packages/requests/_internal_utils.py
--rw-r--r--  2.0 unx    19553 b- defN 23-Nov-03 12:53 site-packages/requests/adapters.py
--rw-r--r--  2.0 unx     6449 b- defN 23-Nov-03 12:53 site-packages/requests/api.py
--rw-r--r--  2.0 unx    10187 b- defN 23-Nov-03 12:53 site-packages/requests/auth.py
--rw-r--r--  2.0 unx      429 b- defN 23-Nov-03 12:53 site-packages/requests/certs.py
--rw-r--r--  2.0 unx     1451 b- defN 23-Nov-03 12:53 site-packages/requests/compat.py
--rw-r--r--  2.0 unx    18560 b- defN 23-Nov-03 12:53 site-packages/requests/cookies.py
--rw-r--r--  2.0 unx     3811 b- defN 23-Nov-03 12:53 site-packages/requests/exceptions.py
--rw-r--r--  2.0 unx     3875 b- defN 23-Nov-03 12:53 site-packages/requests/help.py
--rw-r--r--  2.0 unx      733 b- defN 23-Nov-03 12:53 site-packages/requests/hooks.py
--rw-r--r--  2.0 unx    35223 b- defN 23-Nov-03 12:53 site-packages/requests/models.py
--rw-r--r--  2.0 unx      957 b- defN 23-Nov-03 12:53 site-packages/requests/packages.py
--rw-r--r--  2.0 unx    30373 b- defN 23-Nov-03 12:53 site-packages/requests/sessions.py
--rw-r--r--  2.0 unx     4235 b- defN 23-Nov-03 12:53 site-packages/requests/status_codes.py
--rw-r--r--  2.0 unx     2912 b- defN 23-Nov-03 12:53 site-packages/requests/structures.py
--rw-r--r--  2.0 unx    33448 b- defN 23-Nov-03 12:53 site-packages/requests/utils.py
--rw-r--r--  2.0 unx    34549 b- defN 23-Nov-03 12:54 site-packages/six.py
--rw-r--r--  2.0 unx     5028 b- defN 23-Nov-03 12:54 site-packages/urllib3/__init__.py
--rw-r--r--  2.0 unx     5651 b- defN 23-Nov-03 12:54 site-packages/urllib3/_base_connection.py
--rw-r--r--  2.0 unx    15561 b- defN 23-Nov-03 12:54 site-packages/urllib3/_collections.py
--rw-r--r--  2.0 unx     7756 b- defN 23-Nov-03 12:54 site-packages/urllib3/_request_methods.py
--rw-r--r--  2.0 unx       98 b- defN 23-Nov-03 12:54 site-packages/urllib3/_version.py
--rw-r--r--  2.0 unx    33511 b- defN 23-Nov-03 12:54 site-packages/urllib3/connection.py
--rw-r--r--  2.0 unx    42961 b- defN 23-Nov-03 12:54 site-packages/urllib3/connectionpool.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/_securetransport/__init__.py
--rw-r--r--  2.0 unx    14452 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/_securetransport/bindings.py
--rw-r--r--  2.0 unx    16220 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/_securetransport/low_level.py
--rw-r--r--  2.0 unx    19437 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/pyopenssl.py
--rw-r--r--  2.0 unx    34121 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/securetransport.py
--rw-r--r--  2.0 unx     7715 b- defN 23-Nov-03 12:54 site-packages/urllib3/contrib/socks.py
--rw-r--r--  2.0 unx     9289 b- defN 23-Nov-03 12:54 site-packages/urllib3/exceptions.py
--rw-r--r--  2.0 unx    11026 b- defN 23-Nov-03 12:54 site-packages/urllib3/fields.py
--rw-r--r--  2.0 unx     2395 b- defN 23-Nov-03 12:54 site-packages/urllib3/filepost.py
--rw-r--r--  2.0 unx    22160 b- defN 23-Nov-03 12:54 site-packages/urllib3/poolmanager.py
--rw-r--r--  2.0 unx    39802 b- defN 23-Nov-03 12:54 site-packages/urllib3/response.py
--rw-r--r--  2.0 unx     1051 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/__init__.py
--rw-r--r--  2.0 unx     4462 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/connection.py
--rw-r--r--  2.0 unx     1148 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/proxy.py
--rw-r--r--  2.0 unx     8111 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/request.py
--rw-r--r--  2.0 unx     3374 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/response.py
--rw-r--r--  2.0 unx    18375 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/retry.py
--rw-r--r--  2.0 unx    18540 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/ssl_.py
--rw-r--r--  2.0 unx     5812 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/ssl_match_hostname.py
--rw-r--r--  2.0 unx     9045 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/ssltransport.py
--rw-r--r--  2.0 unx    10529 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/timeout.py
--rw-r--r--  2.0 unx    15213 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/url.py
--rw-r--r--  2.0 unx     1146 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/util.py
--rw-r--r--  2.0 unx     4423 b- defN 23-Nov-03 12:54 site-packages/urllib3/util/wait.py
--rw-r--r--  2.0 unx     8340 b- defN 23-Nov-03 12:54 site-packages/validate_email.py
--rw-r--r--  2.0 unx       59 b- defN 23-Nov-03 12:54 site-packages/wheel/__init__.py
--rw-r--r--  2.0 unx      455 b- defN 23-Nov-03 12:54 site-packages/wheel/__main__.py
--rw-r--r--  2.0 unx      746 b- defN 23-Nov-03 12:54 site-packages/wheel/_setuptools_logging.py
--rw-r--r--  2.0 unx    19868 b- defN 23-Nov-03 12:54 site-packages/wheel/bdist_wheel.py
--rw-r--r--  2.0 unx     3932 b- defN 23-Nov-03 12:54 site-packages/wheel/cli/__init__.py
--rwxr-xr-x  2.0 unx     9427 b- defN 23-Nov-03 12:54 site-packages/wheel/cli/convert.py
--rw-r--r--  2.0 unx     4338 b- defN 23-Nov-03 12:54 site-packages/wheel/cli/pack.py
--rw-r--r--  2.0 unx     5124 b- defN 23-Nov-03 12:54 site-packages/wheel/cli/tags.py
--rw-r--r--  2.0 unx     1021 b- defN 23-Nov-03 12:54 site-packages/wheel/cli/unpack.py
--rw-r--r--  2.0 unx    16143 b- defN 23-Nov-03 12:54 site-packages/wheel/macosx_libfile.py
--rw-r--r--  2.0 unx     5889 b- defN 23-Nov-03 12:54 site-packages/wheel/metadata.py
--rw-r--r--  2.0 unx      621 b- defN 23-Nov-03 12:54 site-packages/wheel/util.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/__init__.py
--rw-r--r--  2.0 unx     3266 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_elffile.py
--rw-r--r--  2.0 unx     8813 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_manylinux.py
--rw-r--r--  2.0 unx     2524 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_musllinux.py
--rw-r--r--  2.0 unx     9399 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_parser.py
--rw-r--r--  2.0 unx     1431 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_structures.py
--rw-r--r--  2.0 unx     5148 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/_tokenizer.py
--rw-r--r--  2.0 unx     8161 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/markers.py
--rw-r--r--  2.0 unx     3264 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/requirements.py
--rw-r--r--  2.0 unx    39047 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/specifiers.py
--rw-r--r--  2.0 unx    18065 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/tags.py
--rw-r--r--  2.0 unx     4355 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/utils.py
--rw-r--r--  2.0 unx    16295 b- defN 23-Nov-03 12:54 site-packages/wheel/vendored/packaging/version.py
--rw-r--r--  2.0 unx     7674 b- defN 23-Nov-03 12:54 site-packages/wheel/wheelfile.py
--r-xr-xr-x  2.0 unx    15874 b- defN 23-Nov-17 10:08 validate/validate_pb2.py
-?rw-------  2.0 unx       91 b- defN 23-Nov-17 10:08 fathom_global_client_sdk-0.8.0.dist-info/WHEEL
-?rw-------  2.0 unx     1611 b- defN 23-Nov-17 10:08 fathom_global_client_sdk-0.8.0.dist-info/METADATA
-?rw-------  2.0 unx    32481 b- defN 23-Nov-17 10:08 fathom_global_client_sdk-0.8.0.dist-info/RECORD
-336 files, 3407314 bytes uncompressed, 857538 bytes compressed:  74.8%
+Zip file size: 40462 bytes, number of entries: 26
+?rwxrwxrwx  2.0 unx      263 b- defN 80-Jan-01 00:00 fathom/__init__.py
+?rwxrwxrwx  2.0 unx     1300 b- defN 80-Jan-01 00:00 fathom/api/v2/common_pb2.py
+?rwxrwxrwx  2.0 unx    24785 b- defN 80-Jan-01 00:00 fathom/api/v2/fathom_pb2.py
+?rwxrwxrwx  2.0 unx     8447 b- defN 80-Jan-01 00:00 fathom/api/v2/fathom_pb2.pyi
+?rwxrwxrwx  2.0 unx     9767 b- defN 80-Jan-01 00:00 fathom/api/v2/fathom_pb2_grpc.py
+?rwxrwxrwx  2.0 unx     9682 b- defN 80-Jan-01 00:00 fathom/api/v2/portfolio_pb2.py
+?rwxrwxrwx  2.0 unx     3133 b- defN 80-Jan-01 00:00 fathom/api/v2/portfolio_pb2.pyi
+?rwxrwxrwx  2.0 unx     6539 b- defN 80-Jan-01 00:00 fathom/api/v2/portfolio_pb2_grpc.py
+?rwxrwxrwx  2.0 unx        0 b- defN 80-Jan-01 00:00 fathom/sdk/__init__.py
+?rwxrwxrwx  2.0 unx     5911 b- defN 80-Jan-01 00:00 fathom/sdk/client.py
+?rwxrwxrwx  2.0 unx      713 b- defN 80-Jan-01 00:00 fathom/sdk/common.py
+?rwxrwxrwx  2.0 unx     7499 b- defN 80-Jan-01 00:00 fathom/sdk/v1.py
+?rwxrwxrwx  2.0 unx    10528 b- defN 80-Jan-01 00:00 fathom/sdk/v2.py
+?rwxrwxrwx  2.0 unx     1354 b- defN 80-Jan-01 00:00 proto/data/data_pb2.py
+?rwxrwxrwx  2.0 unx      556 b- defN 80-Jan-01 00:00 proto/data/data_pb2.pyi
+?rwxrwxrwx  2.0 unx    19609 b- defN 80-Jan-01 00:00 proto/fathom/fathom_pb2.py
+?rwxrwxrwx  2.0 unx     7074 b- defN 80-Jan-01 00:00 proto/fathom/fathom_pb2.pyi
+?rwxrwxrwx  2.0 unx     6013 b- defN 80-Jan-01 00:00 proto/fathom/fathom_pb2_grpc.py
+?rwxrwxrwx  2.0 unx     3144 b- defN 80-Jan-01 00:00 proto/geo/geo_pb2.py
+?rwxrwxrwx  2.0 unx     1484 b- defN 80-Jan-01 00:00 proto/geo/geo_pb2.pyi
+?rwxrwxrwx  2.0 unx     2310 b- defN 80-Jan-01 00:00 protoc_gen_openapiv2/options/annotations_pb2.py
+?rwxrwxrwx  2.0 unx    20065 b- defN 80-Jan-01 00:00 protoc_gen_openapiv2/options/openapiv2_pb2.py
+?rwxrwxrwx  2.0 unx    15599 b- defN 80-Jan-01 00:00 validate/validate_pb2.py
+?rwxrwxrwx  2.0 unx       91 b- defN 80-Jan-01 00:00 fathom_global_client_sdk-0.9.0.dist-info/WHEEL
+?rwxrwxrwx  2.0 unx     1914 b- defN 80-Jan-01 00:00 fathom_global_client_sdk-0.9.0.dist-info/METADATA
+?rwxrwxrwx  2.0 unx     2175 b- defN 80-Jan-01 00:00 fathom_global_client_sdk-0.9.0.dist-info/RECORD
+26 files, 169955 bytes uncompressed, 36964 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -60,950 +60,20 @@
 
 Filename: protoc_gen_openapiv2/options/annotations_pb2.py
 Comment: 
 
 Filename: protoc_gen_openapiv2/options/openapiv2_pb2.py
 Comment: 
 
-Filename: site-packages/__init__.py
-Comment: 
-
-Filename: site-packages/astunparse/__init__.py
-Comment: 
-
-Filename: site-packages/astunparse/__main__.py
-Comment: 
-
-Filename: site-packages/astunparse/printer.py
-Comment: 
-
-Filename: site-packages/astunparse/unparser.py
-Comment: 
-
-Filename: site-packages/certifi/__init__.py
-Comment: 
-
-Filename: site-packages/certifi/__main__.py
-Comment: 
-
-Filename: site-packages/certifi/core.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/__init__.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/api.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/assets/__init__.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/cd.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/cli/__init__.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/cli/normalizer.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/constant.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/legacy.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/md.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/models.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/utils.py
-Comment: 
-
-Filename: site-packages/charset_normalizer/version.py
-Comment: 
-
-Filename: site-packages/google/__init__.py
-Comment: 
-
-Filename: site-packages/google/api/__init__.py
-Comment: 
-
-Filename: site-packages/google/api/annotations_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/auth_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/backend_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/billing_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/client_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/config_change_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/consumer_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/context_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/control_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/distribution_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/documentation_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/endpoint_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/error_reason_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/field_behavior_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/http_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/httpbody_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/label_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/launch_stage_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/log_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/logging_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/metric_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/monitored_resource_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/monitoring_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/quota_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/resource_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/routing_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/service_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/source_info_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/system_parameter_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/usage_pb2.py
-Comment: 
-
-Filename: site-packages/google/api/visibility_pb2.py
-Comment: 
-
-Filename: site-packages/google/cloud/__init__.py
-Comment: 
-
-Filename: site-packages/google/cloud/extended_operations_pb2.py
-Comment: 
-
-Filename: site-packages/google/cloud/location/__init__.py
-Comment: 
-
-Filename: site-packages/google/cloud/location/locations_pb2.py
-Comment: 
-
-Filename: site-packages/google/gapic/__init__.py
-Comment: 
-
-Filename: site-packages/google/gapic/metadata/__init__.py
-Comment: 
-
-Filename: site-packages/google/gapic/metadata/gapic_metadata_pb2.py
-Comment: 
-
-Filename: site-packages/google/logging/__init__.py
-Comment: 
-
-Filename: site-packages/google/logging/type/__init__.py
-Comment: 
-
-Filename: site-packages/google/logging/type/http_request_pb2.py
-Comment: 
-
-Filename: site-packages/google/logging/type/log_severity_pb2.py
-Comment: 
-
-Filename: site-packages/google/longrunning/__init__.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_grpc.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_grpc_pb2.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_pb2.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_pb2_grpc.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_proto.py
-Comment: 
-
-Filename: site-packages/google/longrunning/operations_proto_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/__init__.py
-Comment: 
-
-Filename: site-packages/google/protobuf/any_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/api_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/compiler/__init__.py
-Comment: 
-
-Filename: site-packages/google/protobuf/compiler/plugin_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/descriptor.py
-Comment: 
-
-Filename: site-packages/google/protobuf/descriptor_database.py
-Comment: 
-
-Filename: site-packages/google/protobuf/descriptor_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/descriptor_pool.py
-Comment: 
-
-Filename: site-packages/google/protobuf/duration_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/empty_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/field_mask_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/__init__.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/api_implementation.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/builder.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/containers.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/decoder.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/encoder.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/enum_type_wrapper.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/extension_dict.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/message_listener.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/python_message.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/type_checkers.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/well_known_types.py
-Comment: 
-
-Filename: site-packages/google/protobuf/internal/wire_format.py
-Comment: 
-
-Filename: site-packages/google/protobuf/json_format.py
-Comment: 
-
-Filename: site-packages/google/protobuf/message.py
-Comment: 
-
-Filename: site-packages/google/protobuf/message_factory.py
-Comment: 
-
-Filename: site-packages/google/protobuf/proto_builder.py
-Comment: 
-
-Filename: site-packages/google/protobuf/pyext/__init__.py
-Comment: 
-
-Filename: site-packages/google/protobuf/pyext/cpp_message.py
-Comment: 
-
-Filename: site-packages/google/protobuf/reflection.py
-Comment: 
-
-Filename: site-packages/google/protobuf/service.py
-Comment: 
-
-Filename: site-packages/google/protobuf/service_reflection.py
-Comment: 
-
-Filename: site-packages/google/protobuf/source_context_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/struct_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/symbol_database.py
-Comment: 
-
-Filename: site-packages/google/protobuf/text_encoding.py
-Comment: 
-
-Filename: site-packages/google/protobuf/text_format.py
-Comment: 
-
-Filename: site-packages/google/protobuf/timestamp_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/type_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/util/__init__.py
-Comment: 
-
-Filename: site-packages/google/protobuf/util/json_format_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/util/json_format_proto3_pb2.py
-Comment: 
-
-Filename: site-packages/google/protobuf/wrappers_pb2.py
-Comment: 
-
-Filename: site-packages/google/rpc/__init__.py
-Comment: 
-
-Filename: site-packages/google/rpc/code_pb2.py
-Comment: 
-
-Filename: site-packages/google/rpc/context/__init__.py
-Comment: 
-
-Filename: site-packages/google/rpc/context/attribute_context_pb2.py
-Comment: 
-
-Filename: site-packages/google/rpc/error_details_pb2.py
-Comment: 
-
-Filename: site-packages/google/rpc/status_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/__init__.py
-Comment: 
-
-Filename: site-packages/google/type/calendar_period_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/color_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/date_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/datetime_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/dayofweek_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/decimal_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/expr_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/fraction_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/interval_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/latlng_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/localized_text_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/money_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/month_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/phone_number_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/postal_address_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/quaternion_pb2.py
-Comment: 
-
-Filename: site-packages/google/type/timeofday_pb2.py
-Comment: 
-
-Filename: site-packages/grpc/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/_auth.py
-Comment: 
-
-Filename: site-packages/grpc/_channel.py
-Comment: 
-
-Filename: site-packages/grpc/_common.py
-Comment: 
-
-Filename: site-packages/grpc/_compression.py
-Comment: 
-
-Filename: site-packages/grpc/_cython/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/_cython/_cygrpc/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/_grpcio_metadata.py
-Comment: 
-
-Filename: site-packages/grpc/_interceptor.py
-Comment: 
-
-Filename: site-packages/grpc/_plugin_wrapping.py
-Comment: 
-
-Filename: site-packages/grpc/_runtime_protos.py
-Comment: 
-
-Filename: site-packages/grpc/_server.py
-Comment: 
-
-Filename: site-packages/grpc/_simple_stubs.py
-Comment: 
-
-Filename: site-packages/grpc/_utilities.py
-Comment: 
-
-Filename: site-packages/grpc/aio/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_base_call.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_base_channel.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_base_server.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_call.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_channel.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_interceptor.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_metadata.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_server.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_typing.py
-Comment: 
-
-Filename: site-packages/grpc/aio/_utils.py
-Comment: 
-
-Filename: site-packages/grpc/beta/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/beta/_client_adaptations.py
-Comment: 
-
-Filename: site-packages/grpc/beta/_metadata.py
-Comment: 
-
-Filename: site-packages/grpc/beta/_server_adaptations.py
-Comment: 
-
-Filename: site-packages/grpc/beta/implementations.py
-Comment: 
-
-Filename: site-packages/grpc/beta/interfaces.py
-Comment: 
-
-Filename: site-packages/grpc/beta/utilities.py
-Comment: 
-
-Filename: site-packages/grpc/experimental/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/experimental/aio/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/experimental/gevent.py
-Comment: 
-
-Filename: site-packages/grpc/experimental/session_cache.py
-Comment: 
-
-Filename: site-packages/grpc/framework/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/common/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/common/cardinality.py
-Comment: 
-
-Filename: site-packages/grpc/framework/common/style.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/abandonment.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/callable_util.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/future.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/logging_pool.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/stream.py
-Comment: 
-
-Filename: site-packages/grpc/framework/foundation/stream_util.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/base/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/base/base.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/base/utilities.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/face/__init__.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/face/face.py
-Comment: 
-
-Filename: site-packages/grpc/framework/interfaces/face/utilities.py
-Comment: 
-
-Filename: site-packages/idna/__init__.py
-Comment: 
-
-Filename: site-packages/idna/codec.py
-Comment: 
-
-Filename: site-packages/idna/compat.py
-Comment: 
-
-Filename: site-packages/idna/core.py
-Comment: 
-
-Filename: site-packages/idna/idnadata.py
-Comment: 
-
-Filename: site-packages/idna/intranges.py
-Comment: 
-
-Filename: site-packages/idna/package_data.py
-Comment: 
-
-Filename: site-packages/idna/uts46data.py
-Comment: 
-
-Filename: site-packages/jinja2/__init__.py
-Comment: 
-
-Filename: site-packages/jinja2/_identifier.py
-Comment: 
-
-Filename: site-packages/jinja2/async_utils.py
-Comment: 
-
-Filename: site-packages/jinja2/bccache.py
-Comment: 
-
-Filename: site-packages/jinja2/compiler.py
-Comment: 
-
-Filename: site-packages/jinja2/constants.py
-Comment: 
-
-Filename: site-packages/jinja2/debug.py
-Comment: 
-
-Filename: site-packages/jinja2/defaults.py
-Comment: 
-
-Filename: site-packages/jinja2/environment.py
-Comment: 
-
-Filename: site-packages/jinja2/exceptions.py
-Comment: 
-
-Filename: site-packages/jinja2/ext.py
-Comment: 
-
-Filename: site-packages/jinja2/filters.py
-Comment: 
-
-Filename: site-packages/jinja2/idtracking.py
-Comment: 
-
-Filename: site-packages/jinja2/lexer.py
-Comment: 
-
-Filename: site-packages/jinja2/loaders.py
-Comment: 
-
-Filename: site-packages/jinja2/meta.py
-Comment: 
-
-Filename: site-packages/jinja2/nativetypes.py
-Comment: 
-
-Filename: site-packages/jinja2/nodes.py
-Comment: 
-
-Filename: site-packages/jinja2/optimizer.py
-Comment: 
-
-Filename: site-packages/jinja2/parser.py
-Comment: 
-
-Filename: site-packages/jinja2/runtime.py
-Comment: 
-
-Filename: site-packages/jinja2/sandbox.py
-Comment: 
-
-Filename: site-packages/jinja2/tests.py
-Comment: 
-
-Filename: site-packages/jinja2/utils.py
-Comment: 
-
-Filename: site-packages/jinja2/visitor.py
-Comment: 
-
-Filename: site-packages/markupsafe/__init__.py
-Comment: 
-
-Filename: site-packages/markupsafe/_native.py
-Comment: 
-
-Filename: site-packages/protoc_gen_validate/__init__.py
-Comment: 
-
-Filename: site-packages/protoc_gen_validate/validator.py
-Comment: 
-
-Filename: site-packages/requests/__init__.py
-Comment: 
-
-Filename: site-packages/requests/__version__.py
-Comment: 
-
-Filename: site-packages/requests/_internal_utils.py
-Comment: 
-
-Filename: site-packages/requests/adapters.py
-Comment: 
-
-Filename: site-packages/requests/api.py
-Comment: 
-
-Filename: site-packages/requests/auth.py
-Comment: 
-
-Filename: site-packages/requests/certs.py
-Comment: 
-
-Filename: site-packages/requests/compat.py
-Comment: 
-
-Filename: site-packages/requests/cookies.py
-Comment: 
-
-Filename: site-packages/requests/exceptions.py
-Comment: 
-
-Filename: site-packages/requests/help.py
-Comment: 
-
-Filename: site-packages/requests/hooks.py
-Comment: 
-
-Filename: site-packages/requests/models.py
-Comment: 
-
-Filename: site-packages/requests/packages.py
-Comment: 
-
-Filename: site-packages/requests/sessions.py
-Comment: 
-
-Filename: site-packages/requests/status_codes.py
-Comment: 
-
-Filename: site-packages/requests/structures.py
-Comment: 
-
-Filename: site-packages/requests/utils.py
-Comment: 
-
-Filename: site-packages/six.py
-Comment: 
-
-Filename: site-packages/urllib3/__init__.py
-Comment: 
-
-Filename: site-packages/urllib3/_base_connection.py
-Comment: 
-
-Filename: site-packages/urllib3/_collections.py
-Comment: 
-
-Filename: site-packages/urllib3/_request_methods.py
-Comment: 
-
-Filename: site-packages/urllib3/_version.py
-Comment: 
-
-Filename: site-packages/urllib3/connection.py
-Comment: 
-
-Filename: site-packages/urllib3/connectionpool.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/__init__.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/_securetransport/__init__.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/_securetransport/bindings.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/_securetransport/low_level.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/pyopenssl.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/securetransport.py
-Comment: 
-
-Filename: site-packages/urllib3/contrib/socks.py
-Comment: 
-
-Filename: site-packages/urllib3/exceptions.py
-Comment: 
-
-Filename: site-packages/urllib3/fields.py
-Comment: 
-
-Filename: site-packages/urllib3/filepost.py
-Comment: 
-
-Filename: site-packages/urllib3/poolmanager.py
-Comment: 
-
-Filename: site-packages/urllib3/response.py
-Comment: 
-
-Filename: site-packages/urllib3/util/__init__.py
-Comment: 
-
-Filename: site-packages/urllib3/util/connection.py
-Comment: 
-
-Filename: site-packages/urllib3/util/proxy.py
-Comment: 
-
-Filename: site-packages/urllib3/util/request.py
-Comment: 
-
-Filename: site-packages/urllib3/util/response.py
-Comment: 
-
-Filename: site-packages/urllib3/util/retry.py
-Comment: 
-
-Filename: site-packages/urllib3/util/ssl_.py
-Comment: 
-
-Filename: site-packages/urllib3/util/ssl_match_hostname.py
-Comment: 
-
-Filename: site-packages/urllib3/util/ssltransport.py
-Comment: 
-
-Filename: site-packages/urllib3/util/timeout.py
-Comment: 
-
-Filename: site-packages/urllib3/util/url.py
-Comment: 
-
-Filename: site-packages/urllib3/util/util.py
-Comment: 
-
-Filename: site-packages/urllib3/util/wait.py
-Comment: 
-
-Filename: site-packages/validate_email.py
-Comment: 
-
-Filename: site-packages/wheel/__init__.py
-Comment: 
-
-Filename: site-packages/wheel/__main__.py
-Comment: 
-
-Filename: site-packages/wheel/_setuptools_logging.py
-Comment: 
-
-Filename: site-packages/wheel/bdist_wheel.py
-Comment: 
-
-Filename: site-packages/wheel/cli/__init__.py
-Comment: 
-
-Filename: site-packages/wheel/cli/convert.py
-Comment: 
-
-Filename: site-packages/wheel/cli/pack.py
-Comment: 
-
-Filename: site-packages/wheel/cli/tags.py
-Comment: 
-
-Filename: site-packages/wheel/cli/unpack.py
-Comment: 
-
-Filename: site-packages/wheel/macosx_libfile.py
-Comment: 
-
-Filename: site-packages/wheel/metadata.py
-Comment: 
-
-Filename: site-packages/wheel/util.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/__init__.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/__init__.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_elffile.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_manylinux.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_musllinux.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_parser.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_structures.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/_tokenizer.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/markers.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/requirements.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/specifiers.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/tags.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/utils.py
-Comment: 
-
-Filename: site-packages/wheel/vendored/packaging/version.py
-Comment: 
-
-Filename: site-packages/wheel/wheelfile.py
-Comment: 
-
 Filename: validate/validate_pb2.py
 Comment: 
 
-Filename: fathom_global_client_sdk-0.8.0.dist-info/WHEEL
+Filename: fathom_global_client_sdk-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: fathom_global_client_sdk-0.8.0.dist-info/METADATA
+Filename: fathom_global_client_sdk-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: fathom_global_client_sdk-0.8.0.dist-info/RECORD
+Filename: fathom_global_client_sdk-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fathom/api/v2/common_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: fathom/api/v2/common.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,13 +16,12 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66\x61thom/api/v2/common.proto\x12\rfathom.api.v2\")\n\x08Metadata\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectIdBEZ3github.com/fathom-global/api/fathom/api/v2;fathomv2\xaa\x02\rFathom.Api.V2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fathom.api.v2.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
   _globals['_METADATA']._serialized_start=45
   _globals['_METADATA']._serialized_end=86
 # @@protoc_insertion_point(module_scope)
```

## fathom/api/v2/fathom_pb2.py

```diff
@@ -1,111 +1,124 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: fathom/api/v2/fathom.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from fathom.api.v2 import common_pb2 as fathom_dot_api_dot_v2_dot_common__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66\x61thom/api/v2/fathom.proto\x12\rfathom.api.v2\x1a\x1a\x66\x61thom/api/v2/common.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\"\xfa\x04\n\x15GetPolygonDataRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x30\n\x07polygon\x18\x03 \x01(\x0b\x32\x16.fathom.api.v2.PolygonR\x07polygon:\xc0\x03\x92\x41\xbc\x03\n,*\x14Polygon data request\xd2\x01\tlayer_ids\xd2\x01\x07polygon2\x8b\x03{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}B\x0b\n\t_metadata\"\xe1\x03\n\x16GetPolygonDataResponse\x12L\n\x07results\x18\x01 \x03(\x0b\x32\x32.fathom.api.v2.GetPolygonDataResponse.ResultsEntryR\x07results\x1aX\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32\x1c.fathom.api.v2.PolygonResultR\x05value:\x02\x38\x01:\x9e\x02\x92\x41\x9a\x02\n!*\x15Polygon data response\xd2\x01\x07results2\xf4\x01{\"results\": {\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"geo_tiff\": \"SUkqAAgAAAASAA...\"}, \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"code\": \"CODE_OUT_OF_BOUNDS\"}}}\"\xfc\x04\n\x16GetPolygonStatsRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x30\n\x07polygon\x18\x03 \x01(\x0b\x32\x16.fathom.api.v2.PolygonR\x07polygon:\xc1\x03\x92\x41\xbd\x03\n-*\x15Polygon stats request\xd2\x01\tlayer_ids\xd2\x01\x07polygon2\x8b\x03{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}B\x0b\n\t_metadata\"\xfe\x02\n\x17GetPolygonStatsResponse\x12M\n\x07results\x18\x01 \x03(\x0b\x32\x33.fathom.api.v2.GetPolygonStatsResponse.ResultsEntryR\x07results\x1aW\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.fathom.api.v2.PolygonStatsR\x05value:\x02\x38\x01:\xba\x01\x92\x41\xb6\x01\n\"*\x16Polygon stats response\xd2\x01\x07results2\x8f\x01{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"mean\": 5, \"max\": 10, \"min\": 1, \"std_dev\": 2}}}\"\xea\x04\n\x14GetPointsDataRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x36\n\x06points\x18\x03 \x03(\x0b\x32\x14.fathom.api.v2.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x06points:\xab\x03\x92\x41\xa7\x03\n)*\x12Point data request\xd2\x01\tlayer_ids\xd2\x01\x06points2\xf9\x02{\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}], \"layer_ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}B\x0b\n\t_metadata\"\xf3\x03\n\x15GetPointsDataResponse\x12K\n\x07results\x18\x01 \x03(\x0b\x32\x31.fathom.api.v2.GetPointsDataResponse.ResultsEntryR\x07results\x1aV\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.fathom.api.v2.PointResultR\x05value:\x02\x38\x01:\xb4\x02\x92\x41\xb0\x02\n\x1f*\x13Point data response\xd2\x01\x07results2\x8c\x02{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": -32768}, {\"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}]}}}\"\\\n\x18\x43reateAccessTokenRequest\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\"_\n\x19\x43reateAccessTokenResponse\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\x1f\n\x0b\x65xpire_secs\x18\x02 \x01(\x04R\nexpireSecs\"\xea\x01\n\rPolygonResult\x12\x1b\n\x08geo_tiff\x18\x01 \x01(\x0cH\x00R\x07geoTiff\x12\x36\n\x04\x63ode\x18\x02 \x01(\x0e\x32 .fathom.api.v2.PolygonResultCodeH\x00R\x04\x63ode:z\x92\x41w\nu*\x0ePolygon result2cEither a geo_tiff containing GeoTIFF data, or a code indicating why a GeoTIFF could not be returnedB\x08\n\x06result\"h\n\x10PointResultValue\x12\x35\n\x0bquery_point\x18\x01 \x01(\x0b\x32\x14.fathom.api.v2.PointR\nqueryPoint\x12\x15\n\x03val\x18\x02 \x01(\x05H\x00R\x03val\x88\x01\x01\x42\x06\n\x04_val\"F\n\x0bPointResult\x12\x37\n\x06values\x18\x01 \x03(\x0b\x32\x1f.fathom.api.v2.PointResultValueR\x06values\"s\n\x05Point\x12\x35\n\tlongitude\x18\x01 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80\x66@)\x00\x00\x00\x00\x00\x80\x66\xc0R\tlongitude\x12\x33\n\x08latitude\x18\x02 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80V@)\x00\x00\x00\x00\x00\x80V\xc0R\x08latitude\"A\n\x07Polygon\x12\x36\n\x06points\x18\x01 \x03(\x0b\x32\x14.fathom.api.v2.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x04R\x06points\"_\n\x0cPolygonStats\x12\x12\n\x04mean\x18\x01 \x01(\x05R\x04mean\x12\x10\n\x03min\x18\x02 \x01(\x05R\x03min\x12\x10\n\x03max\x18\x03 \x01(\x05R\x03max\x12\x17\n\x07std_dev\x18\x04 \x01(\x05R\x06stdDev*_\n\x11PolygonResultCode\x12#\n\x1fPOLYGON_RESULT_CODE_UNSPECIFIED\x10\x00\x12%\n!POLYGON_RESULT_CODE_OUT_OF_BOUNDS\x10\x01*`\n\nResolution\x12\x1a\n\x16RESOLUTION_UNSPECIFIED\x10\x00\x12\x18\n\x14RESOLUTION_1_ARC_SEC\x10\x01\x12\x1c\n\x18RESOLUTION_THIRD_ARC_SEC\x10\x02\x32\xa3\x11\n\rFathomService\x12\x8e\x04\n\x0eGetPolygonData\x12$.fathom.api.v2.GetPolygonDataRequest\x1a%.fathom.api.v2.GetPolygonDataResponse\"\xae\x03\x92\x41\x8f\x03J?\n\x03\x32\x30\x30\x12\x38\n\x0bGot results\x12)\n\'\x1a%.fathom.api.v2.GetPolygonDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x15\"\x10/v2/polygon:data:\x01*\x12\x89\x04\n\rGetPointsData\x12#.fathom.api.v2.GetPointsDataRequest\x1a$.fathom.api.v2.GetPointsDataResponse\"\xac\x03\x92\x41\x8e\x03J>\n\x03\x32\x30\x30\x12\x37\n\x0bGot results\x12(\n&\x1a$.fathom.api.v2.GetPointsDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x14\"\x0f/v2/points:data:\x01*\x12\x99\x04\n\x0fGetPolygonStats\x12%.fathom.api.v2.GetPolygonStatsRequest\x1a&.fathom.api.v2.GetPolygonStatsResponse\"\xb6\x03\x92\x41\x96\x03J@\n\x03\x32\x30\x30\x12\x39\n\x0bGot results\x12*\n(\x1a&.fathom.api.v2.GetPolygonStatsResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Jo\n\x03\x34\x30\x30\x12h\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"A\n\x10\x61pplication/json\x12-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x16\"\x11/v2/polygon:stats:\x01*\x12\xd8\x04\n\x11\x43reateAccessToken\x12\'.fathom.api.v2.CreateAccessTokenRequest\x1a(.fathom.api.v2.CreateAccessTokenResponse\"\xef\x03\x92\x41\xd2\x03JO\n\x03\x32\x30\x31\x12H\n\x18\x43reated new access token\x12,\n*\x1a(.fathom.api.v2.CreateAccessTokenResponseJ\x8b\x01\n\x03\x34\x30\x31\x12\x83\x01\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"X\n\x10\x61pplication/json\x12\x44{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\x03\x34\x30\x30\x12t\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"M\n\x10\x61pplication/json\x12\x39{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\x07\x64\x65\x66\x61ult\x12g\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"@\n\x10\x61pplication/json\x12,{\"code\":13,\"message\":\"Error fetching token\"}b\x00\x82\xd3\xe4\x93\x02\x13\"\x0e/v2/auth/token:\x01*BEZ3github.com/fathom-global/api/fathom/api/v2;fathomv2\xaa\x02\rFathom.Api.V2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x66\x61thom/api/v2/fathom.proto\x12\rfathom.api.v2\x1a\x1a\x66\x61thom/api/v2/common.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\"\xdc\x04\n\x1bGetGeoJSONPointsDataRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x64\n\x0epoints_geojson\x18\x03 \x03(\x0b\x32=.fathom.api.v2.GetGeoJSONPointsDataRequest.PointsGeojsonEntryR\rpointsGeojson\x1aX\n\x12PointsGeojsonEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01:\x8e\x02\x92\x41\x8a\x02\n?* GeoJSON based point data request\xd2\x01\tlayer_ids\xd2\x01\x0epoints_geojson2\xc6\x01{\"points_geojson\": {\"type\": \"Feature\", \"geometry\": {\"type\": \"Point\", \"coordinates\": [125.6, 10.1]}}, \"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}B\x0b\n\t_metadata\"\xfa\x04\n\x15GetPolygonDataRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x30\n\x07polygon\x18\x03 \x01(\x0b\x32\x16.fathom.api.v2.PolygonR\x07polygon:\xc0\x03\x92\x41\xbc\x03\n,*\x14Polygon data request\xd2\x01\tlayer_ids\xd2\x01\x07polygon2\x8b\x03{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}B\x0b\n\t_metadata\"\xe1\x03\n\x16GetPolygonDataResponse\x12L\n\x07results\x18\x01 \x03(\x0b\x32\x32.fathom.api.v2.GetPolygonDataResponse.ResultsEntryR\x07results\x1aX\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x32\n\x05value\x18\x02 \x01(\x0b\x32\x1c.fathom.api.v2.PolygonResultR\x05value:\x02\x38\x01:\x9e\x02\x92\x41\x9a\x02\n!*\x15Polygon data response\xd2\x01\x07results2\xf4\x01{\"results\": {\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"geo_tiff\": \"SUkqAAgAAAASAA...\"}, \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"code\": \"CODE_OUT_OF_BOUNDS\"}}}\"\xfc\x04\n\x16GetPolygonStatsRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x30\n\x07polygon\x18\x03 \x01(\x0b\x32\x16.fathom.api.v2.PolygonR\x07polygon:\xc1\x03\x92\x41\xbd\x03\n-*\x15Polygon stats request\xd2\x01\tlayer_ids\xd2\x01\x07polygon2\x8b\x03{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}B\x0b\n\t_metadata\"\xfe\x02\n\x17GetPolygonStatsResponse\x12M\n\x07results\x18\x01 \x03(\x0b\x32\x33.fathom.api.v2.GetPolygonStatsResponse.ResultsEntryR\x07results\x1aW\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.fathom.api.v2.PolygonStatsR\x05value:\x02\x38\x01:\xba\x01\x92\x41\xb6\x01\n\"*\x16Polygon stats response\xd2\x01\x07results2\x8f\x01{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"mean\": 5, \"max\": 10, \"min\": 1, \"std_dev\": 2}}}\"\xea\x04\n\x14GetPointsDataRequest\x12%\n\tlayer_ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x08layerIds\x12\x38\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataH\x00R\x08metadata\x88\x01\x01\x12\x36\n\x06points\x18\x03 \x03(\x0b\x32\x14.fathom.api.v2.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x06points:\xab\x03\x92\x41\xa7\x03\n)*\x12Point data request\xd2\x01\tlayer_ids\xd2\x01\x06points2\xf9\x02{\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}], \"layer_ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}B\x0b\n\t_metadata\"\xf3\x03\n\x15GetPointsDataResponse\x12K\n\x07results\x18\x01 \x03(\x0b\x32\x31.fathom.api.v2.GetPointsDataResponse.ResultsEntryR\x07results\x1aV\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x05value\x18\x02 \x01(\x0b\x32\x1a.fathom.api.v2.PointResultR\x05value:\x02\x38\x01:\xb4\x02\x92\x41\xb0\x02\n\x1f*\x13Point data response\xd2\x01\x07results2\x8c\x02{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": -32768}, {\"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}]}}}\"\\\n\x18\x43reateAccessTokenRequest\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret\"_\n\x19\x43reateAccessTokenResponse\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\x1f\n\x0b\x65xpire_secs\x18\x02 \x01(\x04R\nexpireSecs\"\xea\x01\n\rPolygonResult\x12\x1b\n\x08geo_tiff\x18\x01 \x01(\x0cH\x00R\x07geoTiff\x12\x36\n\x04\x63ode\x18\x02 \x01(\x0e\x32 .fathom.api.v2.PolygonResultCodeH\x00R\x04\x63ode:z\x92\x41w\nu*\x0ePolygon result2cEither a geo_tiff containing GeoTIFF data, or a code indicating why a GeoTIFF could not be returnedB\x08\n\x06result\"h\n\x10PointResultValue\x12\x35\n\x0bquery_point\x18\x01 \x01(\x0b\x32\x14.fathom.api.v2.PointR\nqueryPoint\x12\x15\n\x03val\x18\x02 \x01(\x05H\x00R\x03val\x88\x01\x01\x42\x06\n\x04_val\"F\n\x0bPointResult\x12\x37\n\x06values\x18\x01 \x03(\x0b\x32\x1f.fathom.api.v2.PointResultValueR\x06values\"s\n\x05Point\x12\x35\n\tlongitude\x18\x01 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80\x66@)\x00\x00\x00\x00\x00\x80\x66\xc0R\tlongitude\x12\x33\n\x08latitude\x18\x02 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80V@)\x00\x00\x00\x00\x00\x80V\xc0R\x08latitude\"A\n\x07Polygon\x12\x36\n\x06points\x18\x01 \x03(\x0b\x32\x14.fathom.api.v2.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x04R\x06points\"\x98\x01\n\x0cPolygonStats\x12\x17\n\x04mean\x18\x01 \x01(\x05H\x00R\x04mean\x88\x01\x01\x12\x15\n\x03min\x18\x02 \x01(\x05H\x01R\x03min\x88\x01\x01\x12\x15\n\x03max\x18\x03 \x01(\x05H\x02R\x03max\x88\x01\x01\x12\x1c\n\x07std_dev\x18\x04 \x01(\x05H\x03R\x06stdDev\x88\x01\x01\x42\x07\n\x05_meanB\x06\n\x04_minB\x06\n\x04_maxB\n\n\x08_std_dev*_\n\x11PolygonResultCode\x12#\n\x1fPOLYGON_RESULT_CODE_UNSPECIFIED\x10\x00\x12%\n!POLYGON_RESULT_CODE_OUT_OF_BOUNDS\x10\x01*`\n\nResolution\x12\x1a\n\x16RESOLUTION_UNSPECIFIED\x10\x00\x12\x18\n\x14RESOLUTION_1_ARC_SEC\x10\x01\x12\x1c\n\x18RESOLUTION_THIRD_ARC_SEC\x10\x02\x32\xf5\x12\n\rFathomService\x12\x8e\x04\n\x0eGetPolygonData\x12$.fathom.api.v2.GetPolygonDataRequest\x1a%.fathom.api.v2.GetPolygonDataResponse\"\xae\x03\x92\x41\x8f\x03J?\n\x03\x32\x30\x30\x12\x38\n\x0bGot results\x12)\n\'\x1a%.fathom.api.v2.GetPolygonDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x15\"\x10/v2/polygon:data:\x01*\x12\x89\x04\n\rGetPointsData\x12#.fathom.api.v2.GetPointsDataRequest\x1a$.fathom.api.v2.GetPointsDataResponse\"\xac\x03\x92\x41\x8e\x03J>\n\x03\x32\x30\x30\x12\x37\n\x0bGot results\x12(\n&\x1a$.fathom.api.v2.GetPointsDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x14\"\x0f/v2/points:data:\x01*\x12\xcf\x01\n\x14GetGeoJSONPointsData\x12*.fathom.api.v2.GetGeoJSONPointsDataRequest\x1a$.fathom.api.v2.GetPointsDataResponse\"e\x92\x41@J>\n\x03\x32\x30\x30\x12\x37\n\x0bGot results\x12(\n&\x1a$.fathom.api.v2.GetPointsDataResponse\x82\xd3\xe4\x93\x02\x1c\"\x17/v2/geojson/points:data:\x01*\x12\x99\x04\n\x0fGetPolygonStats\x12%.fathom.api.v2.GetPolygonStatsRequest\x1a&.fathom.api.v2.GetPolygonStatsResponse\"\xb6\x03\x92\x41\x96\x03J@\n\x03\x32\x30\x30\x12\x39\n\x0bGot results\x12*\n(\x1a&.fathom.api.v2.GetPolygonStatsResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Jo\n\x03\x34\x30\x30\x12h\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"A\n\x10\x61pplication/json\x12-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x16\"\x11/v2/polygon:stats:\x01*\x12\xd8\x04\n\x11\x43reateAccessToken\x12\'.fathom.api.v2.CreateAccessTokenRequest\x1a(.fathom.api.v2.CreateAccessTokenResponse\"\xef\x03\x92\x41\xd2\x03JO\n\x03\x32\x30\x31\x12H\n\x18\x43reated new access token\x12,\n*\x1a(.fathom.api.v2.CreateAccessTokenResponseJ\x8b\x01\n\x03\x34\x30\x31\x12\x83\x01\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"X\n\x10\x61pplication/json\x12\x44{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\x03\x34\x30\x30\x12t\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"M\n\x10\x61pplication/json\x12\x39{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\x07\x64\x65\x66\x61ult\x12g\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"@\n\x10\x61pplication/json\x12,{\"code\":13,\"message\":\"Error fetching token\"}b\x00\x82\xd3\xe4\x93\x02\x13\"\x0e/v2/auth/token:\x01*BEZ3github.com/fathom-global/api/fathom/api/v2;fathomv2\xaa\x02\rFathom.Api.V2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fathom.api.v2.fathom_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
-  _GETPOLYGONDATAREQUEST.fields_by_name['layer_ids']._options = None
-  _GETPOLYGONDATAREQUEST.fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _GETPOLYGONDATAREQUEST._options = None
-  _GETPOLYGONDATAREQUEST._serialized_options = b'\222A\274\003\n,*\024Polygon data request\322\001\tlayer_ids\322\001\007polygon2\213\003{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}'
-  _GETPOLYGONDATARESPONSE_RESULTSENTRY._options = None
-  _GETPOLYGONDATARESPONSE_RESULTSENTRY._serialized_options = b'8\001'
-  _GETPOLYGONDATARESPONSE._options = None
-  _GETPOLYGONDATARESPONSE._serialized_options = b'\222A\232\002\n!*\025Polygon data response\322\001\007results2\364\001{\"results\": {\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"geo_tiff\": \"SUkqAAgAAAASAA...\"}, \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"code\": \"CODE_OUT_OF_BOUNDS\"}}}'
-  _GETPOLYGONSTATSREQUEST.fields_by_name['layer_ids']._options = None
-  _GETPOLYGONSTATSREQUEST.fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _GETPOLYGONSTATSREQUEST._options = None
-  _GETPOLYGONSTATSREQUEST._serialized_options = b'\222A\275\003\n-*\025Polygon stats request\322\001\tlayer_ids\322\001\007polygon2\213\003{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}'
-  _GETPOLYGONSTATSRESPONSE_RESULTSENTRY._options = None
-  _GETPOLYGONSTATSRESPONSE_RESULTSENTRY._serialized_options = b'8\001'
-  _GETPOLYGONSTATSRESPONSE._options = None
-  _GETPOLYGONSTATSRESPONSE._serialized_options = b'\222A\266\001\n\"*\026Polygon stats response\322\001\007results2\217\001{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"mean\": 5, \"max\": 10, \"min\": 1, \"std_dev\": 2}}}'
-  _GETPOINTSDATAREQUEST.fields_by_name['layer_ids']._options = None
-  _GETPOINTSDATAREQUEST.fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _GETPOINTSDATAREQUEST.fields_by_name['points']._options = None
-  _GETPOINTSDATAREQUEST.fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _GETPOINTSDATAREQUEST._options = None
-  _GETPOINTSDATAREQUEST._serialized_options = b'\222A\247\003\n)*\022Point data request\322\001\tlayer_ids\322\001\006points2\371\002{\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}], \"layer_ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}'
-  _GETPOINTSDATARESPONSE_RESULTSENTRY._options = None
-  _GETPOINTSDATARESPONSE_RESULTSENTRY._serialized_options = b'8\001'
-  _GETPOINTSDATARESPONSE._options = None
-  _GETPOINTSDATARESPONSE._serialized_options = b'\222A\260\002\n\037*\023Point data response\322\001\007results2\214\002{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": -32768}, {\"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}]}}}'
-  _POLYGONRESULT._options = None
-  _POLYGONRESULT._serialized_options = b'\222Aw\nu*\016Polygon result2cEither a geo_tiff containing GeoTIFF data, or a code indicating why a GeoTIFF could not be returned'
-  _POINT.fields_by_name['longitude']._options = None
-  _POINT.fields_by_name['longitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200f@)\000\000\000\000\000\200f\300'
-  _POINT.fields_by_name['latitude']._options = None
-  _POINT.fields_by_name['latitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200V@)\000\000\000\000\000\200V\300'
-  _POLYGON.fields_by_name['points']._options = None
-  _POLYGON.fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\004'
-  _FATHOMSERVICE.methods_by_name['GetPolygonData']._options = None
-  _FATHOMSERVICE.methods_by_name['GetPolygonData']._serialized_options = b'\222A\217\003J?\n\003200\0228\n\013Got results\022)\n\'\032%.fathom.api.v2.GetPolygonDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\025\"\020/v2/polygon:data:\001*'
-  _FATHOMSERVICE.methods_by_name['GetPointsData']._options = None
-  _FATHOMSERVICE.methods_by_name['GetPointsData']._serialized_options = b'\222A\216\003J>\n\003200\0227\n\013Got results\022(\n&\032$.fathom.api.v2.GetPointsDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\024\"\017/v2/points:data:\001*'
-  _FATHOMSERVICE.methods_by_name['GetPolygonStats']._options = None
-  _FATHOMSERVICE.methods_by_name['GetPolygonStats']._serialized_options = b'\222A\226\003J@\n\003200\0229\n\013Got results\022*\n(\032&.fathom.api.v2.GetPolygonStatsResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Jo\n\003400\022h\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"A\n\020application/json\022-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\026\"\021/v2/polygon:stats:\001*'
-  _FATHOMSERVICE.methods_by_name['CreateAccessToken']._options = None
-  _FATHOMSERVICE.methods_by_name['CreateAccessToken']._serialized_options = b'\222A\322\003JO\n\003201\022H\n\030Created new access token\022,\n*\032(.fathom.api.v2.CreateAccessTokenResponseJ\213\001\n\003401\022\203\001\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"X\n\020application/json\022D{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\003400\022t\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"M\n\020application/json\0229{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\007default\022g\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"@\n\020application/json\022,{\"code\":13,\"message\":\"Error fetching token\"}b\000\202\323\344\223\002\023\"\016/v2/auth/token:\001*'
-  _globals['_POLYGONRESULTCODE']._serialized_start=4331
-  _globals['_POLYGONRESULTCODE']._serialized_end=4426
-  _globals['_RESOLUTION']._serialized_start=4428
-  _globals['_RESOLUTION']._serialized_end=4524
-  _globals['_GETPOLYGONDATAREQUEST']._serialized_start=177
-  _globals['_GETPOLYGONDATAREQUEST']._serialized_end=811
-  _globals['_GETPOLYGONDATARESPONSE']._serialized_start=814
-  _globals['_GETPOLYGONDATARESPONSE']._serialized_end=1295
-  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._serialized_start=918
-  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._serialized_end=1006
-  _globals['_GETPOLYGONSTATSREQUEST']._serialized_start=1298
-  _globals['_GETPOLYGONSTATSREQUEST']._serialized_end=1934
-  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_start=1937
-  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_end=2319
-  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._serialized_start=2043
-  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._serialized_end=2130
-  _globals['_GETPOINTSDATAREQUEST']._serialized_start=2322
-  _globals['_GETPOINTSDATAREQUEST']._serialized_end=2940
-  _globals['_GETPOINTSDATARESPONSE']._serialized_start=2943
-  _globals['_GETPOINTSDATARESPONSE']._serialized_end=3442
-  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._serialized_start=3045
-  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._serialized_end=3131
-  _globals['_CREATEACCESSTOKENREQUEST']._serialized_start=3444
-  _globals['_CREATEACCESSTOKENREQUEST']._serialized_end=3536
-  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_start=3538
-  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_end=3633
-  _globals['_POLYGONRESULT']._serialized_start=3636
-  _globals['_POLYGONRESULT']._serialized_end=3870
-  _globals['_POINTRESULTVALUE']._serialized_start=3872
-  _globals['_POINTRESULTVALUE']._serialized_end=3976
-  _globals['_POINTRESULT']._serialized_start=3978
-  _globals['_POINTRESULT']._serialized_end=4048
-  _globals['_POINT']._serialized_start=4050
-  _globals['_POINT']._serialized_end=4165
-  _globals['_POLYGON']._serialized_start=4167
-  _globals['_POLYGON']._serialized_end=4232
-  _globals['_POLYGONSTATS']._serialized_start=4234
-  _globals['_POLYGONSTATS']._serialized_end=4329
-  _globals['_FATHOMSERVICE']._serialized_start=4527
-  _globals['_FATHOMSERVICE']._serialized_end=6738
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
+  _globals['_GETGEOJSONPOINTSDATAREQUEST_POINTSGEOJSONENTRY']._options = None
+  _globals['_GETGEOJSONPOINTSDATAREQUEST_POINTSGEOJSONENTRY']._serialized_options = b'8\001'
+  _globals['_GETGEOJSONPOINTSDATAREQUEST'].fields_by_name['layer_ids']._options = None
+  _globals['_GETGEOJSONPOINTSDATAREQUEST'].fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_GETGEOJSONPOINTSDATAREQUEST']._options = None
+  _globals['_GETGEOJSONPOINTSDATAREQUEST']._serialized_options = b'\222A\212\002\n?* GeoJSON based point data request\322\001\tlayer_ids\322\001\016points_geojson2\306\001{\"points_geojson\": {\"type\": \"Feature\", \"geometry\": {\"type\": \"Point\", \"coordinates\": [125.6, 10.1]}}, \"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}'
+  _globals['_GETPOLYGONDATAREQUEST'].fields_by_name['layer_ids']._options = None
+  _globals['_GETPOLYGONDATAREQUEST'].fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_GETPOLYGONDATAREQUEST']._options = None
+  _globals['_GETPOLYGONDATAREQUEST']._serialized_options = b'\222A\274\003\n,*\024Polygon data request\322\001\tlayer_ids\322\001\007polygon2\213\003{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}'
+  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._options = None
+  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
+  _globals['_GETPOLYGONDATARESPONSE']._options = None
+  _globals['_GETPOLYGONDATARESPONSE']._serialized_options = b'\222A\232\002\n!*\025Polygon data response\322\001\007results2\364\001{\"results\": {\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"geo_tiff\": \"SUkqAAgAAAASAA...\"}, \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"code\": \"CODE_OUT_OF_BOUNDS\"}}}'
+  _globals['_GETPOLYGONSTATSREQUEST'].fields_by_name['layer_ids']._options = None
+  _globals['_GETPOLYGONSTATSREQUEST'].fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_GETPOLYGONSTATSREQUEST']._options = None
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_options = b'\222A\275\003\n-*\025Polygon stats request\322\001\tlayer_ids\322\001\007polygon2\213\003{\"layer_ids\": [\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\",\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"], \"polygon\": {\"points\": [{\"latitude\": 51.45, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": 0}, {\"latitude\": 51.55, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": -0.1}, {\"latitude\": 51.45, \"longitude\": 0}]}}'
+  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._options = None
+  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
+  _globals['_GETPOLYGONSTATSRESPONSE']._options = None
+  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_options = b'\222A\266\001\n\"*\026Polygon stats response\322\001\007results2\217\001{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"mean\": 5, \"max\": 10, \"min\": 1, \"std_dev\": 2}}}'
+  _globals['_GETPOINTSDATAREQUEST'].fields_by_name['layer_ids']._options = None
+  _globals['_GETPOINTSDATAREQUEST'].fields_by_name['layer_ids']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_GETPOINTSDATAREQUEST'].fields_by_name['points']._options = None
+  _globals['_GETPOINTSDATAREQUEST'].fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_GETPOINTSDATAREQUEST']._options = None
+  _globals['_GETPOINTSDATAREQUEST']._serialized_options = b'\222A\247\003\n)*\022Point data request\322\001\tlayer_ids\322\001\006points2\371\002{\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}], \"layer_ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}'
+  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._options = None
+  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
+  _globals['_GETPOINTSDATARESPONSE']._options = None
+  _globals['_GETPOINTSDATARESPONSE']._serialized_options = b'\222A\260\002\n\037*\023Point data response\322\001\007results2\214\002{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": -32768}, {\"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}]}}}'
+  _globals['_POLYGONRESULT']._options = None
+  _globals['_POLYGONRESULT']._serialized_options = b'\222Aw\nu*\016Polygon result2cEither a geo_tiff containing GeoTIFF data, or a code indicating why a GeoTIFF could not be returned'
+  _globals['_POINT'].fields_by_name['longitude']._options = None
+  _globals['_POINT'].fields_by_name['longitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200f@)\000\000\000\000\000\200f\300'
+  _globals['_POINT'].fields_by_name['latitude']._options = None
+  _globals['_POINT'].fields_by_name['latitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200V@)\000\000\000\000\000\200V\300'
+  _globals['_POLYGON'].fields_by_name['points']._options = None
+  _globals['_POLYGON'].fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\004'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonData']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonData']._serialized_options = b'\222A\217\003J?\n\003200\0228\n\013Got results\022)\n\'\032%.fathom.api.v2.GetPolygonDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\025\"\020/v2/polygon:data:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPointsData']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPointsData']._serialized_options = b'\222A\216\003J>\n\003200\0227\n\013Got results\022(\n&\032$.fathom.api.v2.GetPointsDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\024\"\017/v2/points:data:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetGeoJSONPointsData']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetGeoJSONPointsData']._serialized_options = b'\222A@J>\n\003200\0227\n\013Got results\022(\n&\032$.fathom.api.v2.GetPointsDataResponse\202\323\344\223\002\034\"\027/v2/geojson/points:data:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonStats']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonStats']._serialized_options = b'\222A\226\003J@\n\003200\0229\n\013Got results\022*\n(\032&.fathom.api.v2.GetPolygonStatsResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Jo\n\003400\022h\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"A\n\020application/json\022-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\026\"\021/v2/polygon:stats:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['CreateAccessToken']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['CreateAccessToken']._serialized_options = b'\222A\322\003JO\n\003201\022H\n\030Created new access token\022,\n*\032(.fathom.api.v2.CreateAccessTokenResponseJ\213\001\n\003401\022\203\001\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"X\n\020application/json\022D{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\003400\022t\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"M\n\020application/json\0229{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\007default\022g\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"@\n\020application/json\022,{\"code\":13,\"message\":\"Error fetching token\"}b\000\202\323\344\223\002\023\"\016/v2/auth/token:\001*'
+  _globals['_POLYGONRESULTCODE']._serialized_start=5026
+  _globals['_POLYGONRESULTCODE']._serialized_end=5121
+  _globals['_RESOLUTION']._serialized_start=5123
+  _globals['_RESOLUTION']._serialized_end=5219
+  _globals['_GETGEOJSONPOINTSDATAREQUEST']._serialized_start=207
+  _globals['_GETGEOJSONPOINTSDATAREQUEST']._serialized_end=811
+  _globals['_GETGEOJSONPOINTSDATAREQUEST_POINTSGEOJSONENTRY']._serialized_start=437
+  _globals['_GETGEOJSONPOINTSDATAREQUEST_POINTSGEOJSONENTRY']._serialized_end=525
+  _globals['_GETPOLYGONDATAREQUEST']._serialized_start=814
+  _globals['_GETPOLYGONDATAREQUEST']._serialized_end=1448
+  _globals['_GETPOLYGONDATARESPONSE']._serialized_start=1451
+  _globals['_GETPOLYGONDATARESPONSE']._serialized_end=1932
+  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._serialized_start=1555
+  _globals['_GETPOLYGONDATARESPONSE_RESULTSENTRY']._serialized_end=1643
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_start=1935
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_end=2571
+  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_start=2574
+  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_end=2956
+  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._serialized_start=2680
+  _globals['_GETPOLYGONSTATSRESPONSE_RESULTSENTRY']._serialized_end=2767
+  _globals['_GETPOINTSDATAREQUEST']._serialized_start=2959
+  _globals['_GETPOINTSDATAREQUEST']._serialized_end=3577
+  _globals['_GETPOINTSDATARESPONSE']._serialized_start=3580
+  _globals['_GETPOINTSDATARESPONSE']._serialized_end=4079
+  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._serialized_start=3682
+  _globals['_GETPOINTSDATARESPONSE_RESULTSENTRY']._serialized_end=3768
+  _globals['_CREATEACCESSTOKENREQUEST']._serialized_start=4081
+  _globals['_CREATEACCESSTOKENREQUEST']._serialized_end=4173
+  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_start=4175
+  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_end=4270
+  _globals['_POLYGONRESULT']._serialized_start=4273
+  _globals['_POLYGONRESULT']._serialized_end=4507
+  _globals['_POINTRESULTVALUE']._serialized_start=4509
+  _globals['_POINTRESULTVALUE']._serialized_end=4613
+  _globals['_POINTRESULT']._serialized_start=4615
+  _globals['_POINTRESULT']._serialized_end=4685
+  _globals['_POINT']._serialized_start=4687
+  _globals['_POINT']._serialized_end=4802
+  _globals['_POLYGON']._serialized_start=4804
+  _globals['_POLYGON']._serialized_end=4869
+  _globals['_POLYGONSTATS']._serialized_start=4872
+  _globals['_POLYGONSTATS']._serialized_end=5024
+  _globals['_FATHOMSERVICE']._serialized_start=5222
+  _globals['_FATHOMSERVICE']._serialized_end=7643
 # @@protoc_insertion_point(module_scope)
```

## fathom/api/v2/fathom_pb2.pyi

```diff
@@ -1,158 +1,176 @@
 from fathom.api.v2 import common_pb2 as _common_pb2
 from google.api import annotations_pb2 as _annotations_pb2
+from google.protobuf import struct_pb2 as _struct_pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as _annotations_pb2_1
 from validate import validate_pb2 as _validate_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PolygonResultCode(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     POLYGON_RESULT_CODE_UNSPECIFIED: _ClassVar[PolygonResultCode]
     POLYGON_RESULT_CODE_OUT_OF_BOUNDS: _ClassVar[PolygonResultCode]
 
 class Resolution(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     RESOLUTION_UNSPECIFIED: _ClassVar[Resolution]
     RESOLUTION_1_ARC_SEC: _ClassVar[Resolution]
     RESOLUTION_THIRD_ARC_SEC: _ClassVar[Resolution]
 POLYGON_RESULT_CODE_UNSPECIFIED: PolygonResultCode
 POLYGON_RESULT_CODE_OUT_OF_BOUNDS: PolygonResultCode
 RESOLUTION_UNSPECIFIED: Resolution
 RESOLUTION_1_ARC_SEC: Resolution
 RESOLUTION_THIRD_ARC_SEC: Resolution
 
+class GetGeoJSONPointsDataRequest(_message.Message):
+    __slots__ = ("layer_ids", "metadata", "points_geojson")
+    class PointsGeojsonEntry(_message.Message):
+        __slots__ = ("key", "value")
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: _struct_pb2.Value
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[_struct_pb2.Value, _Mapping]] = ...) -> None: ...
+    LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
+    METADATA_FIELD_NUMBER: _ClassVar[int]
+    POINTS_GEOJSON_FIELD_NUMBER: _ClassVar[int]
+    layer_ids: _containers.RepeatedScalarFieldContainer[str]
+    metadata: _common_pb2.Metadata
+    points_geojson: _containers.MessageMap[str, _struct_pb2.Value]
+    def __init__(self, layer_ids: _Optional[_Iterable[str]] = ..., metadata: _Optional[_Union[_common_pb2.Metadata, _Mapping]] = ..., points_geojson: _Optional[_Mapping[str, _struct_pb2.Value]] = ...) -> None: ...
+
 class GetPolygonDataRequest(_message.Message):
-    __slots__ = ["layer_ids", "metadata", "polygon"]
+    __slots__ = ("layer_ids", "metadata", "polygon")
     LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     POLYGON_FIELD_NUMBER: _ClassVar[int]
     layer_ids: _containers.RepeatedScalarFieldContainer[str]
     metadata: _common_pb2.Metadata
     polygon: Polygon
     def __init__(self, layer_ids: _Optional[_Iterable[str]] = ..., metadata: _Optional[_Union[_common_pb2.Metadata, _Mapping]] = ..., polygon: _Optional[_Union[Polygon, _Mapping]] = ...) -> None: ...
 
 class GetPolygonDataResponse(_message.Message):
-    __slots__ = ["results"]
+    __slots__ = ("results",)
     class ResultsEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: PolygonResult
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[PolygonResult, _Mapping]] = ...) -> None: ...
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.MessageMap[str, PolygonResult]
     def __init__(self, results: _Optional[_Mapping[str, PolygonResult]] = ...) -> None: ...
 
 class GetPolygonStatsRequest(_message.Message):
-    __slots__ = ["layer_ids", "metadata", "polygon"]
+    __slots__ = ("layer_ids", "metadata", "polygon")
     LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     POLYGON_FIELD_NUMBER: _ClassVar[int]
     layer_ids: _containers.RepeatedScalarFieldContainer[str]
     metadata: _common_pb2.Metadata
     polygon: Polygon
     def __init__(self, layer_ids: _Optional[_Iterable[str]] = ..., metadata: _Optional[_Union[_common_pb2.Metadata, _Mapping]] = ..., polygon: _Optional[_Union[Polygon, _Mapping]] = ...) -> None: ...
 
 class GetPolygonStatsResponse(_message.Message):
-    __slots__ = ["results"]
+    __slots__ = ("results",)
     class ResultsEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: PolygonStats
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[PolygonStats, _Mapping]] = ...) -> None: ...
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.MessageMap[str, PolygonStats]
     def __init__(self, results: _Optional[_Mapping[str, PolygonStats]] = ...) -> None: ...
 
 class GetPointsDataRequest(_message.Message):
-    __slots__ = ["layer_ids", "metadata", "points"]
+    __slots__ = ("layer_ids", "metadata", "points")
     LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     POINTS_FIELD_NUMBER: _ClassVar[int]
     layer_ids: _containers.RepeatedScalarFieldContainer[str]
     metadata: _common_pb2.Metadata
     points: _containers.RepeatedCompositeFieldContainer[Point]
     def __init__(self, layer_ids: _Optional[_Iterable[str]] = ..., metadata: _Optional[_Union[_common_pb2.Metadata, _Mapping]] = ..., points: _Optional[_Iterable[_Union[Point, _Mapping]]] = ...) -> None: ...
 
 class GetPointsDataResponse(_message.Message):
-    __slots__ = ["results"]
+    __slots__ = ("results",)
     class ResultsEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: PointResult
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[PointResult, _Mapping]] = ...) -> None: ...
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.MessageMap[str, PointResult]
     def __init__(self, results: _Optional[_Mapping[str, PointResult]] = ...) -> None: ...
 
 class CreateAccessTokenRequest(_message.Message):
-    __slots__ = ["client_id", "client_secret"]
+    __slots__ = ("client_id", "client_secret")
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
     client_id: str
     client_secret: str
     def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[str] = ...) -> None: ...
 
 class CreateAccessTokenResponse(_message.Message):
-    __slots__ = ["access_token", "expire_secs"]
+    __slots__ = ("access_token", "expire_secs")
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
     EXPIRE_SECS_FIELD_NUMBER: _ClassVar[int]
     access_token: str
     expire_secs: int
     def __init__(self, access_token: _Optional[str] = ..., expire_secs: _Optional[int] = ...) -> None: ...
 
 class PolygonResult(_message.Message):
-    __slots__ = ["geo_tiff", "code"]
+    __slots__ = ("geo_tiff", "code")
     GEO_TIFF_FIELD_NUMBER: _ClassVar[int]
     CODE_FIELD_NUMBER: _ClassVar[int]
     geo_tiff: bytes
     code: PolygonResultCode
     def __init__(self, geo_tiff: _Optional[bytes] = ..., code: _Optional[_Union[PolygonResultCode, str]] = ...) -> None: ...
 
 class PointResultValue(_message.Message):
-    __slots__ = ["query_point", "val"]
+    __slots__ = ("query_point", "val")
     QUERY_POINT_FIELD_NUMBER: _ClassVar[int]
     VAL_FIELD_NUMBER: _ClassVar[int]
     query_point: Point
     val: int
     def __init__(self, query_point: _Optional[_Union[Point, _Mapping]] = ..., val: _Optional[int] = ...) -> None: ...
 
 class PointResult(_message.Message):
-    __slots__ = ["values"]
+    __slots__ = ("values",)
     VALUES_FIELD_NUMBER: _ClassVar[int]
     values: _containers.RepeatedCompositeFieldContainer[PointResultValue]
     def __init__(self, values: _Optional[_Iterable[_Union[PointResultValue, _Mapping]]] = ...) -> None: ...
 
 class Point(_message.Message):
-    __slots__ = ["longitude", "latitude"]
+    __slots__ = ("longitude", "latitude")
     LONGITUDE_FIELD_NUMBER: _ClassVar[int]
     LATITUDE_FIELD_NUMBER: _ClassVar[int]
     longitude: float
     latitude: float
     def __init__(self, longitude: _Optional[float] = ..., latitude: _Optional[float] = ...) -> None: ...
 
 class Polygon(_message.Message):
-    __slots__ = ["points"]
+    __slots__ = ("points",)
     POINTS_FIELD_NUMBER: _ClassVar[int]
     points: _containers.RepeatedCompositeFieldContainer[Point]
     def __init__(self, points: _Optional[_Iterable[_Union[Point, _Mapping]]] = ...) -> None: ...
 
 class PolygonStats(_message.Message):
-    __slots__ = ["mean", "min", "max", "std_dev"]
+    __slots__ = ("mean", "min", "max", "std_dev")
     MEAN_FIELD_NUMBER: _ClassVar[int]
     MIN_FIELD_NUMBER: _ClassVar[int]
     MAX_FIELD_NUMBER: _ClassVar[int]
     STD_DEV_FIELD_NUMBER: _ClassVar[int]
     mean: int
     min: int
     max: int
```

## fathom/api/v2/fathom_pb2_grpc.py

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonDataResponse.FromString,
                 )
         self.GetPointsData = channel.unary_unary(
                 '/fathom.api.v2.FathomService/GetPointsData',
                 request_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataRequest.SerializeToString,
                 response_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.FromString,
                 )
+        self.GetGeoJSONPointsData = channel.unary_unary(
+                '/fathom.api.v2.FathomService/GetGeoJSONPointsData',
+                request_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetGeoJSONPointsDataRequest.SerializeToString,
+                response_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.FromString,
+                )
         self.GetPolygonStats = channel.unary_unary(
                 '/fathom.api.v2.FathomService/GetPolygonStats',
                 request_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonStatsRequest.SerializeToString,
                 response_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonStatsResponse.FromString,
                 )
         self.CreateAccessToken = channel.unary_unary(
                 '/fathom.api.v2.FathomService/CreateAccessToken',
@@ -47,14 +52,20 @@
 
     def GetPointsData(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetGeoJSONPointsData(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetPolygonStats(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateAccessToken(self, request, context):
@@ -72,14 +83,19 @@
                     response_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonDataResponse.SerializeToString,
             ),
             'GetPointsData': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPointsData,
                     request_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataRequest.FromString,
                     response_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.SerializeToString,
             ),
+            'GetGeoJSONPointsData': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetGeoJSONPointsData,
+                    request_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetGeoJSONPointsDataRequest.FromString,
+                    response_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.SerializeToString,
+            ),
             'GetPolygonStats': grpc.unary_unary_rpc_method_handler(
                     servicer.GetPolygonStats,
                     request_deserializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonStatsRequest.FromString,
                     response_serializer=fathom_dot_api_dot_v2_dot_fathom__pb2.GetPolygonStatsResponse.SerializeToString,
             ),
             'CreateAccessToken': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateAccessToken,
@@ -127,14 +143,31 @@
         return grpc.experimental.unary_unary(request, target, '/fathom.api.v2.FathomService/GetPointsData',
             fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataRequest.SerializeToString,
             fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def GetGeoJSONPointsData(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/fathom.api.v2.FathomService/GetGeoJSONPointsData',
+            fathom_dot_api_dot_v2_dot_fathom__pb2.GetGeoJSONPointsDataRequest.SerializeToString,
+            fathom_dot_api_dot_v2_dot_fathom__pb2.GetPointsDataResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetPolygonStats(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

## fathom/api/v2/portfolio_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: fathom/api/v2/portfolio.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -20,35 +21,34 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x66\x61thom/api/v2/portfolio.proto\x12\rfathom.api.v2\x1a\x1a\x66\x61thom/api/v2/common.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\"\xc4\x03\n\x1a\x43reatePortfolioTaskRequest\x12\'\n\tlayer_ids\x18\x01 \x03(\tB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10(R\x08layerIds\x12\x33\n\x08metadata\x18\x02 \x01(\x0b\x32\x17.fathom.api.v2.MetadataR\x08metadata:\xc7\x02\x92\x41\xc3\x02\n(*\x1aPortfolio creation request\xd2\x01\tlayer_ids2\x96\x02{\"layerIds\": [\"GLOBAL-1ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1ARCSEC-00_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1_3ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\"]}\"\x90\x01\n\x1b\x43reatePortfolioTaskResponse\x12\x17\n\x07task_id\x18\x01 \x01(\tR\x06taskId\x12\x1d\n\nupload_url\x18\x02 \x01(\tR\tuploadUrl:9\x92\x41\x36\n4*\x1bPortfolio creation response\xd2\x01\x07task_id\xd2\x01\nupload_url\"m\n\x1dGetPortfolioTaskStatusRequest\x12!\n\x07task_id\x18\x01 \x01(\tB\x08\xfa\x42\x05r\x03\xb0\x01\x01R\x06taskId:)\x92\x41&\n$*\x18Portfolio status request\xd2\x01\x07task_id\"\xc7\x01\n\x1eGetPortfolioTaskStatusResponse\x12:\n\x0btask_status\x18\x01 \x01(\x0e\x32\x19.fathom.api.v2.TaskStatusR\ntaskStatus\x12!\n\x0c\x64ownload_url\x18\x02 \x01(\tR\x0b\x64ownloadUrl\x12\x16\n\x06\x65rrors\x18\x03 \x03(\tR\x06\x65rrors:.\x92\x41+\n)*\x19Portfolio status response\xd2\x01\x0btask_status\"Q\n\x1dGetPortfolioQuotaInfoResponse\x12\x12\n\x04used\x18\x01 \x01(\x03R\x04used\x12\x1c\n\tremaining\x18\x02 \x01(\x03R\tremaining*\xc1\x01\n\nTaskStatus\x12\x1b\n\x17TASK_STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13TASK_STATUS_PENDING\x10\x01\x12\x18\n\x14TASK_STATUS_COMPLETE\x10\x02\x12\x15\n\x11TASK_STATUS_ERROR\x10\x03\x12\x1b\n\x17TASK_STATUS_IN_PROGRESS\x10\x04\x12\x17\n\x13TASK_STATUS_EXPIRED\x10\x05\x12\x16\n\x12TASK_STATUS_QUEUED\x10\x06\x32\xbe\n\n\x10PortfolioService\x12\xbc\x04\n\x13\x43reatePortfolioTask\x12).fathom.api.v2.CreatePortfolioTaskRequest\x1a*.fathom.api.v2.CreatePortfolioTaskResponse\"\xcd\x03\x92\x41\xb0\x03J\xc9\x01\n\x03\x32\x30\x30\x12\xc1\x01\n\x18\x43reated task succesfully\x12.\n,\x1a*.fathom.api.v2.CreatePortfolioTaskResponse\"u\n\x10\x61pplication/json\x12\x61{\"taskId\": \"59acb604-6c65-45e5-acc2-2561b17e1d6f\", \"uploadUrl\": \"https://example.com/upload.csv\"}Jo\n\x03\x34\x30\x30\x12h\n\x11Invalid task spec\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No layers passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x13\"\x0e/v2/portfolios:\x01*\x12\xf3\x04\n\x16GetPortfolioTaskStatus\x12,.fathom.api.v2.GetPortfolioTaskStatusRequest\x1a-.fathom.api.v2.GetPortfolioTaskStatusResponse\"\xfb\x03\x92\x41\xd7\x03J\xa8\x01\n\x03\x32\x30\x30\x12\xa0\x01\n\x08Got task\x12\x31\n/\x1a-.fathom.api.v2.GetPortfolioTaskStatusResponse\"a\n\x10\x61pplication/json\x12M{\"taskStatus\": \"COMPLETE\", \"downloadUrl\": \"https://example.com/download.csv\"}J\xb6\x01\n\x03\x34\x30\x30\x12\xae\x01\n\x15\x45rror processing task\x12\x31\n/\x1a-.fathom.api.v2.GetPortfolioTaskStatusResponse\"b\n\x10\x61pplication/json\x12N{\"taskStatus\": \"ERROR\", \"errors\": [\"there was an error processing the input\"]}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x1a\x12\x18/v2/portfolios/{task_id}\x12u\n\x15GetPortfolioQuotaInfo\x12\x16.google.protobuf.Empty\x1a,.fathom.api.v2.GetPortfolioQuotaInfoResponse\"\x16\x82\xd3\xe4\x93\x02\x10\x12\x0e/v2/portfoliosBEZ3github.com/fathom-global/api/fathom/api/v2;fathomv2\xaa\x02\rFathom.Api.V2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'fathom.api.v2.portfolio_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
-  _CREATEPORTFOLIOTASKREQUEST.fields_by_name['layer_ids']._options = None
-  _CREATEPORTFOLIOTASKREQUEST.fields_by_name['layer_ids']._serialized_options = b'\372B\007\222\001\004\010\001\020('
-  _CREATEPORTFOLIOTASKREQUEST._options = None
-  _CREATEPORTFOLIOTASKREQUEST._serialized_options = b'\222A\303\002\n(*\032Portfolio creation request\322\001\tlayer_ids2\226\002{\"layerIds\": [\"GLOBAL-1ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1ARCSEC-00_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1_3ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\"]}'
-  _CREATEPORTFOLIOTASKRESPONSE._options = None
-  _CREATEPORTFOLIOTASKRESPONSE._serialized_options = b'\222A6\n4*\033Portfolio creation response\322\001\007task_id\322\001\nupload_url'
-  _GETPORTFOLIOTASKSTATUSREQUEST.fields_by_name['task_id']._options = None
-  _GETPORTFOLIOTASKSTATUSREQUEST.fields_by_name['task_id']._serialized_options = b'\372B\005r\003\260\001\001'
-  _GETPORTFOLIOTASKSTATUSREQUEST._options = None
-  _GETPORTFOLIOTASKSTATUSREQUEST._serialized_options = b'\222A&\n$*\030Portfolio status request\322\001\007task_id'
-  _GETPORTFOLIOTASKSTATUSRESPONSE._options = None
-  _GETPORTFOLIOTASKSTATUSRESPONSE._serialized_options = b'\222A+\n)*\031Portfolio status response\322\001\013task_status'
-  _PORTFOLIOSERVICE.methods_by_name['CreatePortfolioTask']._options = None
-  _PORTFOLIOSERVICE.methods_by_name['CreatePortfolioTask']._serialized_options = b'\222A\260\003J\311\001\n\003200\022\301\001\n\030Created task succesfully\022.\n,\032*.fathom.api.v2.CreatePortfolioTaskResponse\"u\n\020application/json\022a{\"taskId\": \"59acb604-6c65-45e5-acc2-2561b17e1d6f\", \"uploadUrl\": \"https://example.com/upload.csv\"}Jo\n\003400\022h\n\021Invalid task spec\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No layers passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\023\"\016/v2/portfolios:\001*'
-  _PORTFOLIOSERVICE.methods_by_name['GetPortfolioTaskStatus']._options = None
-  _PORTFOLIOSERVICE.methods_by_name['GetPortfolioTaskStatus']._serialized_options = b'\222A\327\003J\250\001\n\003200\022\240\001\n\010Got task\0221\n/\032-.fathom.api.v2.GetPortfolioTaskStatusResponse\"a\n\020application/json\022M{\"taskStatus\": \"COMPLETE\", \"downloadUrl\": \"https://example.com/download.csv\"}J\266\001\n\003400\022\256\001\n\025Error processing task\0221\n/\032-.fathom.api.v2.GetPortfolioTaskStatusResponse\"b\n\020application/json\022N{\"taskStatus\": \"ERROR\", \"errors\": [\"there was an error processing the input\"]}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\032\022\030/v2/portfolios/{task_id}'
-  _PORTFOLIOSERVICE.methods_by_name['GetPortfolioQuotaInfo']._options = None
-  _PORTFOLIOSERVICE.methods_by_name['GetPortfolioQuotaInfo']._serialized_options = b'\202\323\344\223\002\020\022\016/v2/portfolios'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z3github.com/fathom-global/api/fathom/api/v2;fathomv2\252\002\rFathom.Api.V2'
+  _globals['_CREATEPORTFOLIOTASKREQUEST'].fields_by_name['layer_ids']._options = None
+  _globals['_CREATEPORTFOLIOTASKREQUEST'].fields_by_name['layer_ids']._serialized_options = b'\372B\007\222\001\004\010\001\020('
+  _globals['_CREATEPORTFOLIOTASKREQUEST']._options = None
+  _globals['_CREATEPORTFOLIOTASKREQUEST']._serialized_options = b'\222A\303\002\n(*\032Portfolio creation request\322\001\tlayer_ids2\226\002{\"layerIds\": [\"GLOBAL-1ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1ARCSEC-00_OFFSET-1in100-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\", \"GLOBAL-1_3ARCSEC-00_OFFSET-1in10-PLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v0.0.0_test\"]}'
+  _globals['_CREATEPORTFOLIOTASKRESPONSE']._options = None
+  _globals['_CREATEPORTFOLIOTASKRESPONSE']._serialized_options = b'\222A6\n4*\033Portfolio creation response\322\001\007task_id\322\001\nupload_url'
+  _globals['_GETPORTFOLIOTASKSTATUSREQUEST'].fields_by_name['task_id']._options = None
+  _globals['_GETPORTFOLIOTASKSTATUSREQUEST'].fields_by_name['task_id']._serialized_options = b'\372B\005r\003\260\001\001'
+  _globals['_GETPORTFOLIOTASKSTATUSREQUEST']._options = None
+  _globals['_GETPORTFOLIOTASKSTATUSREQUEST']._serialized_options = b'\222A&\n$*\030Portfolio status request\322\001\007task_id'
+  _globals['_GETPORTFOLIOTASKSTATUSRESPONSE']._options = None
+  _globals['_GETPORTFOLIOTASKSTATUSRESPONSE']._serialized_options = b'\222A+\n)*\031Portfolio status response\322\001\013task_status'
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['CreatePortfolioTask']._options = None
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['CreatePortfolioTask']._serialized_options = b'\222A\260\003J\311\001\n\003200\022\301\001\n\030Created task succesfully\022.\n,\032*.fathom.api.v2.CreatePortfolioTaskResponse\"u\n\020application/json\022a{\"taskId\": \"59acb604-6c65-45e5-acc2-2561b17e1d6f\", \"uploadUrl\": \"https://example.com/upload.csv\"}Jo\n\003400\022h\n\021Invalid task spec\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No layers passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\023\"\016/v2/portfolios:\001*'
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['GetPortfolioTaskStatus']._options = None
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['GetPortfolioTaskStatus']._serialized_options = b'\222A\327\003J\250\001\n\003200\022\240\001\n\010Got task\0221\n/\032-.fathom.api.v2.GetPortfolioTaskStatusResponse\"a\n\020application/json\022M{\"taskStatus\": \"COMPLETE\", \"downloadUrl\": \"https://example.com/download.csv\"}J\266\001\n\003400\022\256\001\n\025Error processing task\0221\n/\032-.fathom.api.v2.GetPortfolioTaskStatusResponse\"b\n\020application/json\022N{\"taskStatus\": \"ERROR\", \"errors\": [\"there was an error processing the input\"]}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\032\022\030/v2/portfolios/{task_id}'
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['GetPortfolioQuotaInfo']._options = None
+  _globals['_PORTFOLIOSERVICE'].methods_by_name['GetPortfolioQuotaInfo']._serialized_options = b'\202\323\344\223\002\020\022\016/v2/portfolios'
   _globals['_TASKSTATUS']._serialized_start=1207
   _globals['_TASKSTATUS']._serialized_end=1400
   _globals['_CREATEPORTFOLIOTASKREQUEST']._serialized_start=209
   _globals['_CREATEPORTFOLIOTASKREQUEST']._serialized_end=661
   _globals['_CREATEPORTFOLIOTASKRESPONSE']._serialized_start=664
   _globals['_CREATEPORTFOLIOTASKRESPONSE']._serialized_end=808
   _globals['_GETPORTFOLIOTASKSTATUSREQUEST']._serialized_start=810
```

## fathom/api/v2/portfolio_pb2.pyi

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class TaskStatus(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     TASK_STATUS_UNSPECIFIED: _ClassVar[TaskStatus]
     TASK_STATUS_PENDING: _ClassVar[TaskStatus]
     TASK_STATUS_COMPLETE: _ClassVar[TaskStatus]
     TASK_STATUS_ERROR: _ClassVar[TaskStatus]
     TASK_STATUS_IN_PROGRESS: _ClassVar[TaskStatus]
     TASK_STATUS_EXPIRED: _ClassVar[TaskStatus]
     TASK_STATUS_QUEUED: _ClassVar[TaskStatus]
@@ -25,45 +25,45 @@
 TASK_STATUS_COMPLETE: TaskStatus
 TASK_STATUS_ERROR: TaskStatus
 TASK_STATUS_IN_PROGRESS: TaskStatus
 TASK_STATUS_EXPIRED: TaskStatus
 TASK_STATUS_QUEUED: TaskStatus
 
 class CreatePortfolioTaskRequest(_message.Message):
-    __slots__ = ["layer_ids", "metadata"]
+    __slots__ = ("layer_ids", "metadata")
     LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     layer_ids: _containers.RepeatedScalarFieldContainer[str]
     metadata: _common_pb2.Metadata
     def __init__(self, layer_ids: _Optional[_Iterable[str]] = ..., metadata: _Optional[_Union[_common_pb2.Metadata, _Mapping]] = ...) -> None: ...
 
 class CreatePortfolioTaskResponse(_message.Message):
-    __slots__ = ["task_id", "upload_url"]
+    __slots__ = ("task_id", "upload_url")
     TASK_ID_FIELD_NUMBER: _ClassVar[int]
     UPLOAD_URL_FIELD_NUMBER: _ClassVar[int]
     task_id: str
     upload_url: str
     def __init__(self, task_id: _Optional[str] = ..., upload_url: _Optional[str] = ...) -> None: ...
 
 class GetPortfolioTaskStatusRequest(_message.Message):
-    __slots__ = ["task_id"]
+    __slots__ = ("task_id",)
     TASK_ID_FIELD_NUMBER: _ClassVar[int]
     task_id: str
     def __init__(self, task_id: _Optional[str] = ...) -> None: ...
 
 class GetPortfolioTaskStatusResponse(_message.Message):
-    __slots__ = ["task_status", "download_url", "errors"]
+    __slots__ = ("task_status", "download_url", "errors")
     TASK_STATUS_FIELD_NUMBER: _ClassVar[int]
     DOWNLOAD_URL_FIELD_NUMBER: _ClassVar[int]
     ERRORS_FIELD_NUMBER: _ClassVar[int]
     task_status: TaskStatus
     download_url: str
     errors: _containers.RepeatedScalarFieldContainer[str]
     def __init__(self, task_status: _Optional[_Union[TaskStatus, str]] = ..., download_url: _Optional[str] = ..., errors: _Optional[_Iterable[str]] = ...) -> None: ...
 
 class GetPortfolioQuotaInfoResponse(_message.Message):
-    __slots__ = ["used", "remaining"]
+    __slots__ = ("used", "remaining")
     USED_FIELD_NUMBER: _ClassVar[int]
     REMAINING_FIELD_NUMBER: _ClassVar[int]
     used: int
     remaining: int
     def __init__(self, used: _Optional[int] = ..., remaining: _Optional[int] = ...) -> None: ...
```

## fathom/sdk/client.py

```diff
@@ -1,45 +1,74 @@
 """The Fathom API client for querying flood and related data.
 """
+import json
 import logging
 from datetime import datetime, timedelta
-from typing import Any, MutableMapping
+from typing import Any, List, MutableMapping, Optional, Tuple
 
 import grpc
 
-from proto.fathom import fathom_pb2, fathom_pb2_grpc
+from fathom.api.v2 import fathom_pb2, fathom_pb2_grpc
 
 from .common import FathomException
 
 FATHOM_GRPC_CHANNEL_MSG_SIZE = 10 * 1024 * 1024  # default 10MB
 
 log = logging.getLogger(__name__)
 
 
-class BaseClient:
-    """A Client for interacting with the Fathom API."""
+def _default_channel_opts() -> List[Tuple[str, str]]:
+    """Default options for all connections"""
+    service_default_config = {
+        "methodConfig": [
+            {
+                # Empty name field means this applies to all RPCs
+                "name": [{}],
+                "retryPolicy": {
+                    "maxAttempts": 5,
+                    "initialBackoff": "0.1s",
+                    "maxBackoff": "5s",
+                    "backoffMultiplier": 2,
+                    "retryableStatusCodes": ["UNAVAILABLE"],
+                },
+            }
+        ]
+    }
+
+    service_default_config = json.dumps(service_default_config)
+
+    return [
+        ("grpc.service_config", service_default_config),
+    ]
 
+
+class BaseClient:
     def __init__(
         self,
         client_id: str,
         client_secret: str,
         api_address: str = "api.fathom.global",
         msg_channel_size: int = FATHOM_GRPC_CHANNEL_MSG_SIZE,
+        *,
+        grpc_interceptors: Optional[List[grpc.UnaryUnaryClientInterceptor]] = None,
     ) -> None:
-        """Constructs a new Client, connected to a remote server.
+        """Constructs a new Client, connected to a remote server. Should not be used directly - use the V1 or V2
+        specific clients instead.
 
         Args:
             api_address: Address of the Fathom API server.
             client_id: Client ID to identify a registered client on the
                     authorization server.
             client_secret: Client Secret used with client_id to get an
                     access token.
             msg_channel_size: gRPC message channel size, it is 10MB by
                 default but if you will be dealing with data size larger than
                 the default, you can configure the size.
+            grpc_interceptors: An optional list of grpc interceptors to add
+                to the grpc channel, for logging or other purposes.
         """
         log.info("fathom.Client: connecting to {}".format(api_address))
 
         if not client_id:
             raise FathomException("Client ID can not be empty")
         if not client_secret:
             raise FathomException("Client secret can not be empty")
@@ -51,14 +80,15 @@
         self._client_secret = client_secret
         self._auth_conn = None
         self._message_size = msg_channel_size
 
         # expired at creation.
         self._token_expiry = datetime.utcnow() + timedelta(seconds=-0.5)
         self._channel = None
+        self._client_interceptors = grpc_interceptors
 
         self._stub_cache: MutableMapping[Any, Any] = {}
 
         # Check auth and initialise the channel
         _, _ = self._get_channel()
 
     def __enter__(self):
@@ -69,34 +99,40 @@
 
     def close(self):
         if channel := getattr(self, "_channel", None):
             channel.close()
             log.info("fathom.Client: closed gRPC channel")
             del self._channel
 
-    def _get_channel(self) -> (grpc.Channel, bool):
+    def _get_channel(self) -> Tuple[grpc.Channel, bool]:
         """Checks that the api credentials are still valid using an
         expiration time, creates a new grpc channel or use the previously
         created grpc channel depending on the condition.
         """
+
         channel_opt = [
             ("grpc.max_send_message_length", self._message_size),
             ("grpc.max_receive_message_length", self._message_size),
+            *_default_channel_opts(),
         ]
 
         new = False
 
         if self._token_expiry <= datetime.utcnow() or self._channel is None:
             call_creds = grpc.access_token_call_credentials(self._api_access_token())
             creds = grpc.composite_channel_credentials(
                 grpc.ssl_channel_credentials(), call_creds
             )
             self._channel = grpc.secure_channel(
                 self._api_addr, creds, options=channel_opt
             )
+            if self._client_interceptors:
+                self._channel = grpc.intercept_channel(
+                    self._channel, *self._client_interceptors
+                )
             new = True
 
         return self._channel, new
 
     def _get_stub(self, stub_type):
         """Gets a new stub for the given type from a new or cached channel"""
         channel, new = self._get_channel()
@@ -110,16 +146,17 @@
 
     def _api_access_token(self) -> str:
         """Returns an access token to authenticate with the Fathom API."""
         try:
             request = fathom_pb2.CreateAccessTokenRequest(
                 client_id=self._client_id, client_secret=self._client_secret
             )
+            channel_opt = [*_default_channel_opts()]
             channel = grpc.secure_channel(
-                self._api_addr, grpc.ssl_channel_credentials()
+                self._api_addr, grpc.ssl_channel_credentials(), options=channel_opt
             )
             stub = fathom_pb2_grpc.FathomServiceStub(channel)
             response = stub.CreateAccessToken(request)
             channel.close()
             self._token_expiry = datetime.utcnow() + timedelta(
                 seconds=response.expire_secs
             )
```

## fathom/sdk/v1.py

```diff
@@ -14,14 +14,21 @@
     write_tiff_data_to_file,
 )
 
 log = logging.getLogger(__name__)
 
 
 class Client(BaseClient):
+    """A client that talks to the V1 Fathom API. See [BaseClient](./python.md#fathom.sdk.client.BaseClient) for
+    instantiation options.
+
+    Attributes:
+        geo: Client to talk to the geospatial data API
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.geo: "GeoClient" = GeoClient(self)
         self.get_points = self.geo.get_points
         self.get_polygon = self.geo.get_polygon
         self.get_with_shapefile = self.geo.get_with_shapefile
```

## fathom/sdk/v2.py

```diff
@@ -22,14 +22,22 @@
     write_tiff_data_to_file,
 )
 
 log = logging.getLogger(__name__)
 
 
 class Client(BaseClient):
+    """A client that talks to the V2 Fathom API. See [BaseClient](./python.md#fathom.sdk.client.BaseClient) for
+    instantiation options.
+
+    Attributes:
+        geo: Client to talk to the geospatial data API
+        portfolio: Client to talk to the large portfolio API
+    """
+
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.geo: "GeoClient" = GeoClient(self)
         self.portfolio: "PortfolioClient" = PortfolioClient(self)
 
 
@@ -76,14 +84,15 @@
     def create_task(
         self, layer_ids: List[str], project_id: Optional[str] = None
     ) -> portfolio_pb2.CreatePortfolioTaskResponse:
         """Create a new portfolio task
 
         Args:
             layer_ids: Layer IDs to use for task
+            project_id: Identifier to differentiate projects using the API.
         """
 
         metadata = _metadata_from_project_id(project_id)
         request = portfolio_pb2.CreatePortfolioTaskRequest(
             layer_ids=layer_ids, metadata=metadata
         )
 
@@ -191,15 +200,15 @@
         project_id: Optional[str] = None,
     ) -> fathom_pb2.GetPointsDataResponse:
         """Returns data pertaining to a list of lat-lng coordinates.
 
         Args:
             points: A list of coordinates.
             layer_ids: The identifiers of the types of data being requested.
-            project_id: Idenitifier to differentiate projects using the API.
+            project_id: Identifier to differentiate projects using the API.
         """
 
         request = fathom_pb2.GetPointsDataRequest(
             points=points,
             layer_ids=layer_ids,
             metadata=_metadata_from_project_id(project_id),
         )
```

## proto/data/data_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: proto/data/data.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -15,13 +16,12 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15proto/data/data.proto\x12\x04\x64\x61ta*`\n\nResolution\x12\x1a\n\x16RESOLUTION_UNSPECIFIED\x10\x00\x12\x18\n\x14RESOLUTION_1_ARC_SEC\x10\x01\x12\x1c\n\x18RESOLUTION_THIRD_ARC_SEC\x10\x02\x42\x37Z\'github.com/fathom-global/api/proto/data\xaa\x02\x0b\x46\x61thom.Datab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.data.data_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z\'github.com/fathom-global/api/proto/data\252\002\013Fathom.Data'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z\'github.com/fathom-global/api/proto/data\252\002\013Fathom.Data'
   _globals['_RESOLUTION']._serialized_start=31
   _globals['_RESOLUTION']._serialized_end=127
 # @@protoc_insertion_point(module_scope)
```

## proto/data/data_pb2.pyi

```diff
@@ -1,14 +1,14 @@
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from typing import ClassVar as _ClassVar
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Resolution(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     RESOLUTION_UNSPECIFIED: _ClassVar[Resolution]
     RESOLUTION_1_ARC_SEC: _ClassVar[Resolution]
     RESOLUTION_THIRD_ARC_SEC: _ClassVar[Resolution]
 RESOLUTION_UNSPECIFIED: Resolution
 RESOLUTION_1_ARC_SEC: Resolution
 RESOLUTION_THIRD_ARC_SEC: Resolution
```

## proto/fathom/fathom_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: proto/fathom/fathom.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -14,85 +15,84 @@
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from proto.data import data_pb2 as proto_dot_data_dot_data__pb2
 from proto.geo import geo_pb2 as proto_dot_geo_dot_geo__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 from validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19proto/fathom/fathom.proto\x12\x06\x66\x61thom\x1a\x1cgoogle/api/annotations.proto\x1a\x15proto/data/data.proto\x1a\x13proto/geo/geo.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\"^\n\x0cPolygonStats\x12\x12\n\x04mean\x18\x01 \x01(\x05R\x04mean\x12\x10\n\x03min\x18\x02 \x01(\x05R\x03min\x12\x10\n\x03max\x18\x03 \x01(\x05R\x03max\x12\x16\n\x06stddev\x18\x04 \x01(\x05R\x06stddev\"\xa5\x02\n\x16GetPolygonStatsRequest\x12&\n\x07polygon\x18\x01 \x01(\x0b\x32\x0c.geo.PolygonR\x07polygon\x12&\n\x06layers\x18\x02 \x01(\x0b\x32\x0e.fathom.LayersR\x06layers\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32,.fathom.GetPolygonStatsRequest.MetadataEntryR\x08metadata\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01:4\x92\x41\x31\n/*\x1aPolygon statistics request\xd2\x01\x06layers\xd2\x01\x07polygon\"\xab\x01\n\x17GetPolygonStatsResponse\x12@\n\x05stats\x18\x01 \x03(\x0b\x32*.fathom.GetPolygonStatsResponse.StatsEntryR\x05stats\x1aN\n\nStatsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x14.fathom.PolygonStatsR\x05value:\x02\x38\x01\"\xe3\x06\n\x0eGetDataRequest\x12(\n\x07polygon\x18\x02 \x01(\x0b\x32\x0c.geo.PolygonH\x00R\x07polygon\x12)\n\x06points\x18\x05 \x01(\x0b\x32\x0f.geo.MultiPointH\x00R\x06points\x12$\n\x08shp_file\x18\x04 \x01(\x0c\x42\x07\xfa\x42\x04z\x02\x10\x44H\x00R\x07shpFile\x12&\n\x06layers\x18\x03 \x01(\x0b\x32\x0e.fathom.LayersR\x06layers\x12@\n\x08metadata\x18\x06 \x03(\x0b\x32$.fathom.GetDataRequest.MetadataEntryR\x08metadata\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01:\x94\x04\x92\x41\x90\x04\nr*\x0fGetData request2VUsing this endpoint via REST only support \'points\', not \'polygon\' or \'shp_file\' inputs\xd2\x01\x06layers2\x99\x03{\"points\": {\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}]},\"layers\": {\"layer_ids\": {\"ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}}}B\x12\n\x0b\x63oordinates\x12\x03\xf8\x42\x01J\x04\x08\x01\x10\x02\"\x80\x01\n\x06Layers\x12\x39\n\tlayer_ids\x18\x01 \x01(\x0b\x32\x1a.fathom.Layers.IdentifiersH\x00R\x08layerIds\x1a)\n\x0bIdentifiers\x12\x1a\n\x03ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x03idsB\n\n\x03ids\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03\"\xa0\x0c\n\x0fGetDataResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.fathom.GetDataResponse.ResultsEntryR\x07results\x1aH\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x0c.fathom.DataR\x05value:\x02\x38\x01:\x82\x0b\x92\x41\xfe\n\n\x1c*\x10GetData response\xd2\x01\x07results2\xdd\n{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44870370370371}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"code\": \"NO_DATA\"}, {\"sw_corner\": {\"longitude\": -105.1162962962963, \"latitude\": 39.62851851851852}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_THIRD_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 205}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 90}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"}}}\"\xe6\x02\n\x04\x44\x61ta\x12\x30\n\nresolution\x18\x01 \x01(\x0e\x32\x10.data.ResolutionR\nresolution\x12*\n\x06values\x18\x04 \x03(\x0b\x32\x12.fathom.Data.ValueR\x06values\x12.\n\x08polygons\x18\x05 \x01(\x0b\x32\x10.fathom.PolygonsH\x00R\x08polygons\x12\"\n\x04\x63ode\x18\x06 \x01(\x0e\x32\x0c.fathom.CodeH\x00R\x04\x63ode\x1a\xa0\x01\n\x05Value\x12\'\n\tsw_corner\x18\x01 \x01(\x0b\x32\n.geo.PointR\x08swCorner\x12+\n\x0bquery_point\x18\x05 \x01(\x0b\x32\n.geo.PointR\nqueryPoint\x12\x12\n\x03val\x18\x02 \x01(\rH\x00R\x03val\x12\"\n\x04\x63ode\x18\x03 \x01(\x0e\x32\x0c.fathom.CodeH\x00R\x04\x63odeB\t\n\x07payloadB\t\n\x07payload\"\'\n\x08Polygons\x12\x1b\n\tgeo_tiffs\x18\x01 \x03(\x0cR\x08geoTiffs\"\x84\x02\n\x18\x43reateAccessTokenRequest\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret:\xa5\x01\x92\x41\xa1\x01\n;*\x1d\x41\x63\x63\x65ss token creation request\xd2\x01\tclient_id\xd2\x01\rclient_secret2b{\"client_id\": \"ieKoa2kuuMucaeleithu\", \"client_secret\": \"JiefahPeeli3NoVoochaibuc4ongie3eib2ai5ch\"}\"\xc8\x01\n\x19\x43reateAccessTokenResponse\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\x1f\n\x0b\x65xpire_secs\x18\x02 \x01(\x04R\nexpireSecs:g\x92\x41\x64\n *\x1e\x41\x63\x63\x65ss token creation response2@{\"access_token\": \"zahhuZa5aikae6OhW2su\", \"expire_secs\": \"86400\"}*9\n\x04\x43ode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07NO_DATA\x10\x01\x12\x13\n\x0fPERMANENT_WATER\x10\x02\x32\xc1\x0c\n\rFathomService\x12\xdf\x03\n\x07GetData\x12\x16.fathom.GetDataRequest\x1a\x17.fathom.GetDataResponse\"\xa2\x03\x92\x41\x81\x03J1\n\x03\x32\x30\x30\x12*\n\x0bGot results\x12\x1b\n\x19\x1a\x17.fathom.GetDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x17\"\x12/v1/layers:getData:\x01*\x12\x87\x04\n\x0fGetPolygonStats\x12\x1e.fathom.GetPolygonStatsRequest\x1a\x1f.fathom.GetPolygonStatsResponse\"\xb2\x03\x92\x41\x8f\x03J9\n\x03\x32\x30\x30\x12\x32\n\x0bGot results\x12#\n!\x1a\x1f.fathom.GetPolygonStatsResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Jo\n\x03\x34\x30\x30\x12h\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"A\n\x10\x61pplication/json\x12-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x19\"\x14/v1/polygon:getStats:\x01*\x12\xc3\x04\n\x11\x43reateAccessToken\x12 .fathom.CreateAccessTokenRequest\x1a!.fathom.CreateAccessTokenResponse\"\xe8\x03\x92\x41\xcb\x03JH\n\x03\x32\x30\x30\x12\x41\n\x18\x43reated new access token\x12%\n#\x1a!.fathom.CreateAccessTokenResponseJ\x8b\x01\n\x03\x34\x30\x31\x12\x83\x01\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"X\n\x10\x61pplication/json\x12\x44{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\x03\x34\x30\x30\x12t\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"M\n\x10\x61pplication/json\x12\x39{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\x07\x64\x65\x66\x61ult\x12g\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"@\n\x10\x61pplication/json\x12,{\"code\":13,\"message\":\"Error fetching token\"}b\x00\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/auth/token:\x01*B\xdf\x02Z)github.com/fathom-global/api/proto/fathom\xaa\x02\nFathom.Api\x92\x41\xa3\x02\x12\xc1\x01\n\nFathom API\x12\x8e\x01The Fathom API.\n\nNote that all error response will include a gRPC response code - see https://grpc.github.io/grpc/core/md_doc_statuscodes.html\"\x1f\n\x06\x46\x61thom\x12\x15https://fathom.global2\x01\x31\x1a\x11\x61pi.fathom.global*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ#\n!\n\nApiKeyAuth\x12\x13\x08\x02\x1a\rAuthorization \x02\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19proto/fathom/fathom.proto\x12\x06\x66\x61thom\x1a\x1cgoogle/api/annotations.proto\x1a\x15proto/data/data.proto\x1a\x13proto/geo/geo.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\"\x96\x01\n\x0cPolygonStats\x12\x17\n\x04mean\x18\x01 \x01(\x05H\x00R\x04mean\x88\x01\x01\x12\x15\n\x03min\x18\x02 \x01(\x05H\x01R\x03min\x88\x01\x01\x12\x15\n\x03max\x18\x03 \x01(\x05H\x02R\x03max\x88\x01\x01\x12\x1b\n\x06stddev\x18\x04 \x01(\x05H\x03R\x06stddev\x88\x01\x01\x42\x07\n\x05_meanB\x06\n\x04_minB\x06\n\x04_maxB\t\n\x07_stddev\"\xa5\x02\n\x16GetPolygonStatsRequest\x12&\n\x07polygon\x18\x01 \x01(\x0b\x32\x0c.geo.PolygonR\x07polygon\x12&\n\x06layers\x18\x02 \x01(\x0b\x32\x0e.fathom.LayersR\x06layers\x12H\n\x08metadata\x18\x03 \x03(\x0b\x32,.fathom.GetPolygonStatsRequest.MetadataEntryR\x08metadata\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01:4\x92\x41\x31\n/*\x1aPolygon statistics request\xd2\x01\x06layers\xd2\x01\x07polygon\"\xab\x01\n\x17GetPolygonStatsResponse\x12@\n\x05stats\x18\x01 \x03(\x0b\x32*.fathom.GetPolygonStatsResponse.StatsEntryR\x05stats\x1aN\n\nStatsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12*\n\x05value\x18\x02 \x01(\x0b\x32\x14.fathom.PolygonStatsR\x05value:\x02\x38\x01\"\xe3\x06\n\x0eGetDataRequest\x12(\n\x07polygon\x18\x02 \x01(\x0b\x32\x0c.geo.PolygonH\x00R\x07polygon\x12)\n\x06points\x18\x05 \x01(\x0b\x32\x0f.geo.MultiPointH\x00R\x06points\x12$\n\x08shp_file\x18\x04 \x01(\x0c\x42\x07\xfa\x42\x04z\x02\x10\x44H\x00R\x07shpFile\x12&\n\x06layers\x18\x03 \x01(\x0b\x32\x0e.fathom.LayersR\x06layers\x12@\n\x08metadata\x18\x06 \x03(\x0b\x32$.fathom.GetDataRequest.MetadataEntryR\x08metadata\x1a;\n\rMetadataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01:\x94\x04\x92\x41\x90\x04\nr*\x0fGetData request2VUsing this endpoint via REST only support \'points\', not \'polygon\' or \'shp_file\' inputs\xd2\x01\x06layers2\x99\x03{\"points\": {\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}]},\"layers\": {\"layer_ids\": {\"ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}}}B\x12\n\x0b\x63oordinates\x12\x03\xf8\x42\x01J\x04\x08\x01\x10\x02\"\x80\x01\n\x06Layers\x12\x39\n\tlayer_ids\x18\x01 \x01(\x0b\x32\x1a.fathom.Layers.IdentifiersH\x00R\x08layerIds\x1a)\n\x0bIdentifiers\x12\x1a\n\x03ids\x18\x01 \x03(\tB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x03idsB\n\n\x03ids\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03\"\xa0\x0c\n\x0fGetDataResponse\x12>\n\x07results\x18\x01 \x03(\x0b\x32$.fathom.GetDataResponse.ResultsEntryR\x07results\x1aH\n\x0cResultsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\"\n\x05value\x18\x02 \x01(\x0b\x32\x0c.fathom.DataR\x05value:\x02\x38\x01:\x82\x0b\x92\x41\xfe\n\n\x1c*\x10GetData response\xd2\x01\x07results2\xdd\n{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44870370370371}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"code\": \"NO_DATA\"}, {\"sw_corner\": {\"longitude\": -105.1162962962963, \"latitude\": 39.62851851851852}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_THIRD_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 205}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 90}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"}}}\"\xe6\x02\n\x04\x44\x61ta\x12\x30\n\nresolution\x18\x01 \x01(\x0e\x32\x10.data.ResolutionR\nresolution\x12*\n\x06values\x18\x04 \x03(\x0b\x32\x12.fathom.Data.ValueR\x06values\x12.\n\x08polygons\x18\x05 \x01(\x0b\x32\x10.fathom.PolygonsH\x00R\x08polygons\x12\"\n\x04\x63ode\x18\x06 \x01(\x0e\x32\x0c.fathom.CodeH\x00R\x04\x63ode\x1a\xa0\x01\n\x05Value\x12\'\n\tsw_corner\x18\x01 \x01(\x0b\x32\n.geo.PointR\x08swCorner\x12+\n\x0bquery_point\x18\x05 \x01(\x0b\x32\n.geo.PointR\nqueryPoint\x12\x12\n\x03val\x18\x02 \x01(\rH\x00R\x03val\x12\"\n\x04\x63ode\x18\x03 \x01(\x0e\x32\x0c.fathom.CodeH\x00R\x04\x63odeB\t\n\x07payloadB\t\n\x07payload\"\'\n\x08Polygons\x12\x1b\n\tgeo_tiffs\x18\x01 \x03(\x0cR\x08geoTiffs\"\x84\x02\n\x18\x43reateAccessTokenRequest\x12\x1b\n\tclient_id\x18\x01 \x01(\tR\x08\x63lientId\x12#\n\rclient_secret\x18\x02 \x01(\tR\x0c\x63lientSecret:\xa5\x01\x92\x41\xa1\x01\n;*\x1d\x41\x63\x63\x65ss token creation request\xd2\x01\tclient_id\xd2\x01\rclient_secret2b{\"client_id\": \"ieKoa2kuuMucaeleithu\", \"client_secret\": \"JiefahPeeli3NoVoochaibuc4ongie3eib2ai5ch\"}\"\xc8\x01\n\x19\x43reateAccessTokenResponse\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12\x1f\n\x0b\x65xpire_secs\x18\x02 \x01(\x04R\nexpireSecs:g\x92\x41\x64\n *\x1e\x41\x63\x63\x65ss token creation response2@{\"access_token\": \"zahhuZa5aikae6OhW2su\", \"expire_secs\": \"86400\"}*9\n\x04\x43ode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0b\n\x07NO_DATA\x10\x01\x12\x13\n\x0fPERMANENT_WATER\x10\x02\x32\xc1\x0c\n\rFathomService\x12\xdf\x03\n\x07GetData\x12\x16.fathom.GetDataRequest\x1a\x17.fathom.GetDataResponse\"\xa2\x03\x92\x41\x81\x03J1\n\x03\x32\x30\x30\x12*\n\x0bGot results\x12\x1b\n\x19\x1a\x17.fathom.GetDataResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Ji\n\x03\x34\x30\x30\x12\x62\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\";\n\x10\x61pplication/json\x12\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x17\"\x12/v1/layers:getData:\x01*\x12\x87\x04\n\x0fGetPolygonStats\x12\x1e.fathom.GetPolygonStatsRequest\x1a\x1f.fathom.GetPolygonStatsResponse\"\xb2\x03\x92\x41\x8f\x03J9\n\x03\x32\x30\x30\x12\x32\n\x0bGot results\x12#\n!\x1a\x1f.fathom.GetPolygonStatsResponseJn\n\x03\x34\x30\x31\x12g\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"<\n\x10\x61pplication/json\x12({\"code\":16,\"message\":\"No authorization\"}Jo\n\x03\x34\x30\x30\x12h\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"A\n\x10\x61pplication/json\x12-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\x07\x64\x65\x66\x61ult\x12\x66\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"?\n\x10\x61pplication/json\x12+{\"code\":13,\"message\":\"Error querying data\"}\x82\xd3\xe4\x93\x02\x19\"\x14/v1/polygon:getStats:\x01*\x12\xc3\x04\n\x11\x43reateAccessToken\x12 .fathom.CreateAccessTokenRequest\x1a!.fathom.CreateAccessTokenResponse\"\xe8\x03\x92\x41\xcb\x03JH\n\x03\x32\x30\x30\x12\x41\n\x18\x43reated new access token\x12%\n#\x1a!.fathom.CreateAccessTokenResponseJ\x8b\x01\n\x03\x34\x30\x31\x12\x83\x01\n\x0f\x42\x61\x64 credentials\x12\x16\n\x14\x1a\x12.google.rpc.Status\"X\n\x10\x61pplication/json\x12\x44{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\x03\x34\x30\x30\x12t\n\x0b\x42\x61\x64 request\x12\x16\n\x14\x1a\x12.google.rpc.Status\"M\n\x10\x61pplication/json\x12\x39{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\x07\x64\x65\x66\x61ult\x12g\n\x0bOther error\x12\x16\n\x14\x1a\x12.google.rpc.Status\"@\n\x10\x61pplication/json\x12,{\"code\":13,\"message\":\"Error fetching token\"}b\x00\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/auth/token:\x01*B\xdf\x02Z)github.com/fathom-global/api/proto/fathom\xaa\x02\nFathom.Api\x92\x41\xa3\x02\x12\xc1\x01\n\nFathom API\x12\x8e\x01The Fathom API.\n\nNote that all error response will include a gRPC response code - see https://grpc.github.io/grpc/core/md_doc_statuscodes.html\"\x1f\n\x06\x46\x61thom\x12\x15https://fathom.global2\x01\x31\x1a\x11\x61pi.fathom.global*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ#\n!\n\nApiKeyAuth\x12\x13\x08\x02\x1a\rAuthorization \x02\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.fathom.fathom_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z)github.com/fathom-global/api/proto/fathom\252\002\nFathom.Api\222A\243\002\022\301\001\n\nFathom API\022\216\001The Fathom API.\n\nNote that all error response will include a gRPC response code - see https://grpc.github.io/grpc/core/md_doc_statuscodes.html\"\037\n\006Fathom\022\025https://fathom.global2\0011\032\021api.fathom.global*\001\0022\020application/json:\020application/jsonZ#\n!\n\nApiKeyAuth\022\023\010\002\032\rAuthorization \002'
-  _GETPOLYGONSTATSREQUEST_METADATAENTRY._options = None
-  _GETPOLYGONSTATSREQUEST_METADATAENTRY._serialized_options = b'8\001'
-  _GETPOLYGONSTATSREQUEST._options = None
-  _GETPOLYGONSTATSREQUEST._serialized_options = b'\222A1\n/*\032Polygon statistics request\322\001\006layers\322\001\007polygon'
-  _GETPOLYGONSTATSRESPONSE_STATSENTRY._options = None
-  _GETPOLYGONSTATSRESPONSE_STATSENTRY._serialized_options = b'8\001'
-  _GETDATAREQUEST_METADATAENTRY._options = None
-  _GETDATAREQUEST_METADATAENTRY._serialized_options = b'8\001'
-  _GETDATAREQUEST.oneofs_by_name['coordinates']._options = None
-  _GETDATAREQUEST.oneofs_by_name['coordinates']._serialized_options = b'\370B\001'
-  _GETDATAREQUEST.fields_by_name['shp_file']._options = None
-  _GETDATAREQUEST.fields_by_name['shp_file']._serialized_options = b'\372B\004z\002\020D'
-  _GETDATAREQUEST._options = None
-  _GETDATAREQUEST._serialized_options = b'\222A\220\004\nr*\017GetData request2VUsing this endpoint via REST only support \'points\', not \'polygon\' or \'shp_file\' inputs\322\001\006layers2\231\003{\"points\": {\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}]},\"layers\": {\"layer_ids\": {\"ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}}}'
-  _LAYERS_IDENTIFIERS.fields_by_name['ids']._options = None
-  _LAYERS_IDENTIFIERS.fields_by_name['ids']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _LAYERS.oneofs_by_name['ids']._options = None
-  _LAYERS.oneofs_by_name['ids']._serialized_options = b'\370B\001'
-  _GETDATARESPONSE_RESULTSENTRY._options = None
-  _GETDATARESPONSE_RESULTSENTRY._serialized_options = b'8\001'
-  _GETDATARESPONSE._options = None
-  _GETDATARESPONSE._serialized_options = b'\222A\376\n\n\034*\020GetData response\322\001\007results2\335\n{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44870370370371}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"code\": \"NO_DATA\"}, {\"sw_corner\": {\"longitude\": -105.1162962962963, \"latitude\": 39.62851851851852}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_THIRD_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 205}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 90}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"}}}'
-  _CREATEACCESSTOKENREQUEST._options = None
-  _CREATEACCESSTOKENREQUEST._serialized_options = b'\222A\241\001\n;*\035Access token creation request\322\001\tclient_id\322\001\rclient_secret2b{\"client_id\": \"ieKoa2kuuMucaeleithu\", \"client_secret\": \"JiefahPeeli3NoVoochaibuc4ongie3eib2ai5ch\"}'
-  _CREATEACCESSTOKENRESPONSE._options = None
-  _CREATEACCESSTOKENRESPONSE._serialized_options = b'\222Ad\n *\036Access token creation response2@{\"access_token\": \"zahhuZa5aikae6OhW2su\", \"expire_secs\": \"86400\"}'
-  _FATHOMSERVICE.methods_by_name['GetData']._options = None
-  _FATHOMSERVICE.methods_by_name['GetData']._serialized_options = b'\222A\201\003J1\n\003200\022*\n\013Got results\022\033\n\031\032\027.fathom.GetDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\027\"\022/v1/layers:getData:\001*'
-  _FATHOMSERVICE.methods_by_name['GetPolygonStats']._options = None
-  _FATHOMSERVICE.methods_by_name['GetPolygonStats']._serialized_options = b'\222A\217\003J9\n\003200\0222\n\013Got results\022#\n!\032\037.fathom.GetPolygonStatsResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Jo\n\003400\022h\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"A\n\020application/json\022-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\031\"\024/v1/polygon:getStats:\001*'
-  _FATHOMSERVICE.methods_by_name['CreateAccessToken']._options = None
-  _FATHOMSERVICE.methods_by_name['CreateAccessToken']._serialized_options = b'\222A\313\003JH\n\003200\022A\n\030Created new access token\022%\n#\032!.fathom.CreateAccessTokenResponseJ\213\001\n\003401\022\203\001\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"X\n\020application/json\022D{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\003400\022t\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"M\n\020application/json\0229{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\007default\022g\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"@\n\020application/json\022,{\"code\":13,\"message\":\"Error fetching token\"}b\000\202\323\344\223\002\023\"\016/v1/auth/token:\001*'
-  _globals['_CODE']._serialized_start=4190
-  _globals['_CODE']._serialized_end=4247
-  _globals['_POLYGONSTATS']._serialized_start=184
-  _globals['_POLYGONSTATS']._serialized_end=278
-  _globals['_GETPOLYGONSTATSREQUEST']._serialized_start=281
-  _globals['_GETPOLYGONSTATSREQUEST']._serialized_end=574
-  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._serialized_start=461
-  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._serialized_end=520
-  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_start=577
-  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_end=748
-  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._serialized_start=670
-  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._serialized_end=748
-  _globals['_GETDATAREQUEST']._serialized_start=751
-  _globals['_GETDATAREQUEST']._serialized_end=1618
-  _globals['_GETDATAREQUEST_METADATAENTRY']._serialized_start=461
-  _globals['_GETDATAREQUEST_METADATAENTRY']._serialized_end=520
-  _globals['_LAYERS']._serialized_start=1621
-  _globals['_LAYERS']._serialized_end=1749
-  _globals['_LAYERS_IDENTIFIERS']._serialized_start=1690
-  _globals['_LAYERS_IDENTIFIERS']._serialized_end=1731
-  _globals['_GETDATARESPONSE']._serialized_start=1752
-  _globals['_GETDATARESPONSE']._serialized_end=3320
-  _globals['_GETDATARESPONSE_RESULTSENTRY']._serialized_start=1835
-  _globals['_GETDATARESPONSE_RESULTSENTRY']._serialized_end=1907
-  _globals['_DATA']._serialized_start=3323
-  _globals['_DATA']._serialized_end=3681
-  _globals['_DATA_VALUE']._serialized_start=3510
-  _globals['_DATA_VALUE']._serialized_end=3670
-  _globals['_POLYGONS']._serialized_start=3683
-  _globals['_POLYGONS']._serialized_end=3722
-  _globals['_CREATEACCESSTOKENREQUEST']._serialized_start=3725
-  _globals['_CREATEACCESSTOKENREQUEST']._serialized_end=3985
-  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_start=3988
-  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_end=4188
-  _globals['_FATHOMSERVICE']._serialized_start=4250
-  _globals['_FATHOMSERVICE']._serialized_end=5851
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z)github.com/fathom-global/api/proto/fathom\252\002\nFathom.Api\222A\243\002\022\301\001\n\nFathom API\022\216\001The Fathom API.\n\nNote that all error response will include a gRPC response code - see https://grpc.github.io/grpc/core/md_doc_statuscodes.html\"\037\n\006Fathom\022\025https://fathom.global2\0011\032\021api.fathom.global*\001\0022\020application/json:\020application/jsonZ#\n!\n\nApiKeyAuth\022\023\010\002\032\rAuthorization \002'
+  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._options = None
+  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._serialized_options = b'8\001'
+  _globals['_GETPOLYGONSTATSREQUEST']._options = None
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_options = b'\222A1\n/*\032Polygon statistics request\322\001\006layers\322\001\007polygon'
+  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._options = None
+  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._serialized_options = b'8\001'
+  _globals['_GETDATAREQUEST_METADATAENTRY']._options = None
+  _globals['_GETDATAREQUEST_METADATAENTRY']._serialized_options = b'8\001'
+  _globals['_GETDATAREQUEST'].oneofs_by_name['coordinates']._options = None
+  _globals['_GETDATAREQUEST'].oneofs_by_name['coordinates']._serialized_options = b'\370B\001'
+  _globals['_GETDATAREQUEST'].fields_by_name['shp_file']._options = None
+  _globals['_GETDATAREQUEST'].fields_by_name['shp_file']._serialized_options = b'\372B\004z\002\020D'
+  _globals['_GETDATAREQUEST']._options = None
+  _globals['_GETDATAREQUEST']._serialized_options = b'\222A\220\004\nr*\017GetData request2VUsing this endpoint via REST only support \'points\', not \'polygon\' or \'shp_file\' inputs\322\001\006layers2\231\003{\"points\": {\"points\": [{\"longitude\": -2.601340, \"latitude\": 51.448765}, {\"longitude\": -105.1162333, \"latitude\": 39.628574}]},\"layers\": {\"layer_ids\": {\"ids\": [\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\", \"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\"]}}}'
+  _globals['_LAYERS_IDENTIFIERS'].fields_by_name['ids']._options = None
+  _globals['_LAYERS_IDENTIFIERS'].fields_by_name['ids']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_LAYERS'].oneofs_by_name['ids']._options = None
+  _globals['_LAYERS'].oneofs_by_name['ids']._serialized_options = b'\370B\001'
+  _globals['_GETDATARESPONSE_RESULTSENTRY']._options = None
+  _globals['_GETDATARESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
+  _globals['_GETDATARESPONSE']._options = None
+  _globals['_GETDATARESPONSE']._serialized_options = b'\222A\376\n\n\034*\020GetData response\322\001\007results2\335\n{\"results\": {\"US-1_3ARCSEC-00_OFFSET-1in1000-FLUVIAL-DEFENDED-DEPTH-2020-PERCENTILE50-v2.0.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44870370370371}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"code\": \"NO_DATA\"}, {\"sw_corner\": {\"longitude\": -105.1162962962963, \"latitude\": 39.62851851851852}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_THIRD_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in1000-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 205}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"},\"GLOBAL-1ARCSEC-NW_OFFSET-1in100-FLUVIAL-UNDEFENDED-DEPTH-2020-PERCENTILE50-v3.0\": {\"values\": [{\"sw_corner\": {\"longitude\": -2.6013888888888888, \"latitude\": 51.44861111111111}, \"query_point\": {\"longitude\": -2.60134, \"latitude\": 51.448765}, \"val\": 90}, {\"sw_corner\": {\"longitude\": -105.11638888888889, \"latitude\": 39.62833333333333}, \"query_point\": {\"longitude\": -105.1162333, \"latitude\": 39.628574}, \"val\": 0}], \"resolution\": \"RESOLUTION_1_ARC_SEC\"}}}'
+  _globals['_CREATEACCESSTOKENREQUEST']._options = None
+  _globals['_CREATEACCESSTOKENREQUEST']._serialized_options = b'\222A\241\001\n;*\035Access token creation request\322\001\tclient_id\322\001\rclient_secret2b{\"client_id\": \"ieKoa2kuuMucaeleithu\", \"client_secret\": \"JiefahPeeli3NoVoochaibuc4ongie3eib2ai5ch\"}'
+  _globals['_CREATEACCESSTOKENRESPONSE']._options = None
+  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_options = b'\222Ad\n *\036Access token creation response2@{\"access_token\": \"zahhuZa5aikae6OhW2su\", \"expire_secs\": \"86400\"}'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetData']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetData']._serialized_options = b'\222A\201\003J1\n\003200\022*\n\013Got results\022\033\n\031\032\027.fathom.GetDataResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Ji\n\003400\022b\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\";\n\020application/json\022\'{\"code\":3,\"message\":\"No points passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\027\"\022/v1/layers:getData:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonStats']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['GetPolygonStats']._serialized_options = b'\222A\217\003J9\n\003200\0222\n\013Got results\022#\n!\032\037.fathom.GetPolygonStatsResponseJn\n\003401\022g\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"<\n\020application/json\022({\"code\":16,\"message\":\"No authorization\"}Jo\n\003400\022h\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"A\n\020application/json\022-{\"code\":3,\"message\":\"Invalid polygon passed\"}Jq\n\007default\022f\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"?\n\020application/json\022+{\"code\":13,\"message\":\"Error querying data\"}\202\323\344\223\002\031\"\024/v1/polygon:getStats:\001*'
+  _globals['_FATHOMSERVICE'].methods_by_name['CreateAccessToken']._options = None
+  _globals['_FATHOMSERVICE'].methods_by_name['CreateAccessToken']._serialized_options = b'\222A\313\003JH\n\003200\022A\n\030Created new access token\022%\n#\032!.fathom.CreateAccessTokenResponseJ\213\001\n\003401\022\203\001\n\017Bad credentials\022\026\n\024\032\022.google.rpc.Status\"X\n\020application/json\022D{\"code\":16,\"message\":\"Invalid client id and client secret provided\"}J{\n\003400\022t\n\013Bad request\022\026\n\024\032\022.google.rpc.Status\"M\n\020application/json\0229{\"code\":3,\"message\":\"Empty Client ID or Secret provided\"}Jr\n\007default\022g\n\013Other error\022\026\n\024\032\022.google.rpc.Status\"@\n\020application/json\022,{\"code\":13,\"message\":\"Error fetching token\"}b\000\202\323\344\223\002\023\"\016/v1/auth/token:\001*'
+  _globals['_CODE']._serialized_start=4247
+  _globals['_CODE']._serialized_end=4304
+  _globals['_POLYGONSTATS']._serialized_start=185
+  _globals['_POLYGONSTATS']._serialized_end=335
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_start=338
+  _globals['_GETPOLYGONSTATSREQUEST']._serialized_end=631
+  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._serialized_start=518
+  _globals['_GETPOLYGONSTATSREQUEST_METADATAENTRY']._serialized_end=577
+  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_start=634
+  _globals['_GETPOLYGONSTATSRESPONSE']._serialized_end=805
+  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._serialized_start=727
+  _globals['_GETPOLYGONSTATSRESPONSE_STATSENTRY']._serialized_end=805
+  _globals['_GETDATAREQUEST']._serialized_start=808
+  _globals['_GETDATAREQUEST']._serialized_end=1675
+  _globals['_GETDATAREQUEST_METADATAENTRY']._serialized_start=518
+  _globals['_GETDATAREQUEST_METADATAENTRY']._serialized_end=577
+  _globals['_LAYERS']._serialized_start=1678
+  _globals['_LAYERS']._serialized_end=1806
+  _globals['_LAYERS_IDENTIFIERS']._serialized_start=1747
+  _globals['_LAYERS_IDENTIFIERS']._serialized_end=1788
+  _globals['_GETDATARESPONSE']._serialized_start=1809
+  _globals['_GETDATARESPONSE']._serialized_end=3377
+  _globals['_GETDATARESPONSE_RESULTSENTRY']._serialized_start=1892
+  _globals['_GETDATARESPONSE_RESULTSENTRY']._serialized_end=1964
+  _globals['_DATA']._serialized_start=3380
+  _globals['_DATA']._serialized_end=3738
+  _globals['_DATA_VALUE']._serialized_start=3567
+  _globals['_DATA_VALUE']._serialized_end=3727
+  _globals['_POLYGONS']._serialized_start=3740
+  _globals['_POLYGONS']._serialized_end=3779
+  _globals['_CREATEACCESSTOKENREQUEST']._serialized_start=3782
+  _globals['_CREATEACCESSTOKENREQUEST']._serialized_end=4042
+  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_start=4045
+  _globals['_CREATEACCESSTOKENRESPONSE']._serialized_end=4245
+  _globals['_FATHOMSERVICE']._serialized_start=4307
+  _globals['_FATHOMSERVICE']._serialized_end=5908
 # @@protoc_insertion_point(module_scope)
```

## proto/fathom/fathom_pb2.pyi

```diff
@@ -8,68 +8,68 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Code(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-    __slots__ = []
+    __slots__ = ()
     UNSPECIFIED: _ClassVar[Code]
     NO_DATA: _ClassVar[Code]
     PERMANENT_WATER: _ClassVar[Code]
 UNSPECIFIED: Code
 NO_DATA: Code
 PERMANENT_WATER: Code
 
 class PolygonStats(_message.Message):
-    __slots__ = ["mean", "min", "max", "stddev"]
+    __slots__ = ("mean", "min", "max", "stddev")
     MEAN_FIELD_NUMBER: _ClassVar[int]
     MIN_FIELD_NUMBER: _ClassVar[int]
     MAX_FIELD_NUMBER: _ClassVar[int]
     STDDEV_FIELD_NUMBER: _ClassVar[int]
     mean: int
     min: int
     max: int
     stddev: int
     def __init__(self, mean: _Optional[int] = ..., min: _Optional[int] = ..., max: _Optional[int] = ..., stddev: _Optional[int] = ...) -> None: ...
 
 class GetPolygonStatsRequest(_message.Message):
-    __slots__ = ["polygon", "layers", "metadata"]
+    __slots__ = ("polygon", "layers", "metadata")
     class MetadataEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     POLYGON_FIELD_NUMBER: _ClassVar[int]
     LAYERS_FIELD_NUMBER: _ClassVar[int]
     METADATA_FIELD_NUMBER: _ClassVar[int]
     polygon: _geo_pb2.Polygon
     layers: Layers
     metadata: _containers.ScalarMap[str, str]
     def __init__(self, polygon: _Optional[_Union[_geo_pb2.Polygon, _Mapping]] = ..., layers: _Optional[_Union[Layers, _Mapping]] = ..., metadata: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class GetPolygonStatsResponse(_message.Message):
-    __slots__ = ["stats"]
+    __slots__ = ("stats",)
     class StatsEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: PolygonStats
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[PolygonStats, _Mapping]] = ...) -> None: ...
     STATS_FIELD_NUMBER: _ClassVar[int]
     stats: _containers.MessageMap[str, PolygonStats]
     def __init__(self, stats: _Optional[_Mapping[str, PolygonStats]] = ...) -> None: ...
 
 class GetDataRequest(_message.Message):
-    __slots__ = ["polygon", "points", "shp_file", "layers", "metadata"]
+    __slots__ = ("polygon", "points", "shp_file", "layers", "metadata")
     class MetadataEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: str
         def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
     POLYGON_FIELD_NUMBER: _ClassVar[int]
     POINTS_FIELD_NUMBER: _ClassVar[int]
@@ -80,41 +80,41 @@
     points: _geo_pb2.MultiPoint
     shp_file: bytes
     layers: Layers
     metadata: _containers.ScalarMap[str, str]
     def __init__(self, polygon: _Optional[_Union[_geo_pb2.Polygon, _Mapping]] = ..., points: _Optional[_Union[_geo_pb2.MultiPoint, _Mapping]] = ..., shp_file: _Optional[bytes] = ..., layers: _Optional[_Union[Layers, _Mapping]] = ..., metadata: _Optional[_Mapping[str, str]] = ...) -> None: ...
 
 class Layers(_message.Message):
-    __slots__ = ["layer_ids"]
+    __slots__ = ("layer_ids",)
     class Identifiers(_message.Message):
-        __slots__ = ["ids"]
+        __slots__ = ("ids",)
         IDS_FIELD_NUMBER: _ClassVar[int]
         ids: _containers.RepeatedScalarFieldContainer[str]
         def __init__(self, ids: _Optional[_Iterable[str]] = ...) -> None: ...
     LAYER_IDS_FIELD_NUMBER: _ClassVar[int]
     layer_ids: Layers.Identifiers
     def __init__(self, layer_ids: _Optional[_Union[Layers.Identifiers, _Mapping]] = ...) -> None: ...
 
 class GetDataResponse(_message.Message):
-    __slots__ = ["results"]
+    __slots__ = ("results",)
     class ResultsEntry(_message.Message):
-        __slots__ = ["key", "value"]
+        __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
         key: str
         value: Data
         def __init__(self, key: _Optional[str] = ..., value: _Optional[_Union[Data, _Mapping]] = ...) -> None: ...
     RESULTS_FIELD_NUMBER: _ClassVar[int]
     results: _containers.MessageMap[str, Data]
     def __init__(self, results: _Optional[_Mapping[str, Data]] = ...) -> None: ...
 
 class Data(_message.Message):
-    __slots__ = ["resolution", "values", "polygons", "code"]
+    __slots__ = ("resolution", "values", "polygons", "code")
     class Value(_message.Message):
-        __slots__ = ["sw_corner", "query_point", "val", "code"]
+        __slots__ = ("sw_corner", "query_point", "val", "code")
         SW_CORNER_FIELD_NUMBER: _ClassVar[int]
         QUERY_POINT_FIELD_NUMBER: _ClassVar[int]
         VAL_FIELD_NUMBER: _ClassVar[int]
         CODE_FIELD_NUMBER: _ClassVar[int]
         sw_corner: _geo_pb2.Point
         query_point: _geo_pb2.Point
         val: int
@@ -127,27 +127,27 @@
     resolution: _data_pb2.Resolution
     values: _containers.RepeatedCompositeFieldContainer[Data.Value]
     polygons: Polygons
     code: Code
     def __init__(self, resolution: _Optional[_Union[_data_pb2.Resolution, str]] = ..., values: _Optional[_Iterable[_Union[Data.Value, _Mapping]]] = ..., polygons: _Optional[_Union[Polygons, _Mapping]] = ..., code: _Optional[_Union[Code, str]] = ...) -> None: ...
 
 class Polygons(_message.Message):
-    __slots__ = ["geo_tiffs"]
+    __slots__ = ("geo_tiffs",)
     GEO_TIFFS_FIELD_NUMBER: _ClassVar[int]
     geo_tiffs: _containers.RepeatedScalarFieldContainer[bytes]
     def __init__(self, geo_tiffs: _Optional[_Iterable[bytes]] = ...) -> None: ...
 
 class CreateAccessTokenRequest(_message.Message):
-    __slots__ = ["client_id", "client_secret"]
+    __slots__ = ("client_id", "client_secret")
     CLIENT_ID_FIELD_NUMBER: _ClassVar[int]
     CLIENT_SECRET_FIELD_NUMBER: _ClassVar[int]
     client_id: str
     client_secret: str
     def __init__(self, client_id: _Optional[str] = ..., client_secret: _Optional[str] = ...) -> None: ...
 
 class CreateAccessTokenResponse(_message.Message):
-    __slots__ = ["access_token", "expire_secs"]
+    __slots__ = ("access_token", "expire_secs")
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
     EXPIRE_SECS_FIELD_NUMBER: _ClassVar[int]
     access_token: str
     expire_secs: int
     def __init__(self, access_token: _Optional[str] = ..., expire_secs: _Optional[int] = ...) -> None: ...
```

## proto/geo/geo_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: proto/geo/geo.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,27 +17,26 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13proto/geo/geo.proto\x12\x03geo\x1a\x17validate/validate.proto\"s\n\x05Point\x12\x35\n\tlongitude\x18\x01 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80\x66@)\x00\x00\x00\x00\x00\x80\x66\xc0R\tlongitude\x12\x33\n\x08latitude\x18\x02 \x01(\x01\x42\x17\xfa\x42\x14\x12\x12\x19\x00\x00\x00\x00\x00\x80V@)\x00\x00\x00\x00\x00\x80V\xc0R\x08latitude\":\n\nMultiPoint\x12,\n\x06points\x18\x01 \x03(\x0b\x32\n.geo.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x01R\x06points\":\n\nLineString\x12,\n\x06points\x18\x01 \x03(\x0b\x32\n.geo.PointB\x08\xfa\x42\x05\x92\x01\x02\x08\x02R\x06points\"<\n\x07Polygon\x12\x31\n\x05lines\x18\x01 \x03(\x0b\x32\x0f.geo.LineStringB\n\xfa\x42\x07\x92\x01\x04\x08\x01\x10\x01R\x05linesB5Z&github.com/fathom-global/api/proto/geo\xaa\x02\nFathom.Geob\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'proto.geo.geo_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z&github.com/fathom-global/api/proto/geo\252\002\nFathom.Geo'
-  _POINT.fields_by_name['longitude']._options = None
-  _POINT.fields_by_name['longitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200f@)\000\000\000\000\000\200f\300'
-  _POINT.fields_by_name['latitude']._options = None
-  _POINT.fields_by_name['latitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200V@)\000\000\000\000\000\200V\300'
-  _MULTIPOINT.fields_by_name['points']._options = None
-  _MULTIPOINT.fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\001'
-  _LINESTRING.fields_by_name['points']._options = None
-  _LINESTRING.fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\002'
-  _POLYGON.fields_by_name['lines']._options = None
-  _POLYGON.fields_by_name['lines']._serialized_options = b'\372B\007\222\001\004\010\001\020\001'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'Z&github.com/fathom-global/api/proto/geo\252\002\nFathom.Geo'
+  _globals['_POINT'].fields_by_name['longitude']._options = None
+  _globals['_POINT'].fields_by_name['longitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200f@)\000\000\000\000\000\200f\300'
+  _globals['_POINT'].fields_by_name['latitude']._options = None
+  _globals['_POINT'].fields_by_name['latitude']._serialized_options = b'\372B\024\022\022\031\000\000\000\000\000\200V@)\000\000\000\000\000\200V\300'
+  _globals['_MULTIPOINT'].fields_by_name['points']._options = None
+  _globals['_MULTIPOINT'].fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\001'
+  _globals['_LINESTRING'].fields_by_name['points']._options = None
+  _globals['_LINESTRING'].fields_by_name['points']._serialized_options = b'\372B\005\222\001\002\010\002'
+  _globals['_POLYGON'].fields_by_name['lines']._options = None
+  _globals['_POLYGON'].fields_by_name['lines']._serialized_options = b'\372B\007\222\001\004\010\001\020\001'
   _globals['_POINT']._serialized_start=53
   _globals['_POINT']._serialized_end=168
   _globals['_MULTIPOINT']._serialized_start=170
   _globals['_MULTIPOINT']._serialized_end=228
   _globals['_LINESTRING']._serialized_start=230
   _globals['_LINESTRING']._serialized_end=288
   _globals['_POLYGON']._serialized_start=290
```

## proto/geo/geo_pb2.pyi

```diff
@@ -3,31 +3,31 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Point(_message.Message):
-    __slots__ = ["longitude", "latitude"]
+    __slots__ = ("longitude", "latitude")
     LONGITUDE_FIELD_NUMBER: _ClassVar[int]
     LATITUDE_FIELD_NUMBER: _ClassVar[int]
     longitude: float
     latitude: float
     def __init__(self, longitude: _Optional[float] = ..., latitude: _Optional[float] = ...) -> None: ...
 
 class MultiPoint(_message.Message):
-    __slots__ = ["points"]
+    __slots__ = ("points",)
     POINTS_FIELD_NUMBER: _ClassVar[int]
     points: _containers.RepeatedCompositeFieldContainer[Point]
     def __init__(self, points: _Optional[_Iterable[_Union[Point, _Mapping]]] = ...) -> None: ...
 
 class LineString(_message.Message):
-    __slots__ = ["points"]
+    __slots__ = ("points",)
     POINTS_FIELD_NUMBER: _ClassVar[int]
     points: _containers.RepeatedCompositeFieldContainer[Point]
     def __init__(self, points: _Optional[_Iterable[_Union[Point, _Mapping]]] = ...) -> None: ...
 
 class Polygon(_message.Message):
-    __slots__ = ["lines"]
+    __slots__ = ("lines",)
     LINES_FIELD_NUMBER: _ClassVar[int]
     lines: _containers.RepeatedCompositeFieldContainer[LineString]
     def __init__(self, lines: _Optional[_Iterable[_Union[LineString, _Mapping]]] = ...) -> None: ...
```

## protoc_gen_openapiv2/options/annotations_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: protoc-gen-openapiv2/options/annotations.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -17,16 +18,10 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.protoc-gen-openapiv2/options/annotations.proto\x12)grpc.gateway.protoc_gen_openapiv2.options\x1a google/protobuf/descriptor.proto\x1a,protoc-gen-openapiv2/options/openapiv2.proto:~\n\x11openapiv2_swagger\x12\x1c.google.protobuf.FileOptions\x18\x92\x08 \x01(\x0b\x32\x32.grpc.gateway.protoc_gen_openapiv2.options.SwaggerR\x10openapiv2Swagger:\x86\x01\n\x13openapiv2_operation\x12\x1e.google.protobuf.MethodOptions\x18\x92\x08 \x01(\x0b\x32\x34.grpc.gateway.protoc_gen_openapiv2.options.OperationR\x12openapiv2Operation:~\n\x10openapiv2_schema\x12\x1f.google.protobuf.MessageOptions\x18\x92\x08 \x01(\x0b\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.SchemaR\x0fopenapiv2Schema:u\n\ropenapiv2_tag\x12\x1f.google.protobuf.ServiceOptions\x18\x92\x08 \x01(\x0b\x32..grpc.gateway.protoc_gen_openapiv2.options.TagR\x0copenapiv2Tag:~\n\x0fopenapiv2_field\x12\x1d.google.protobuf.FieldOptions\x18\x92\x08 \x01(\x0b\x32\x35.grpc.gateway.protoc_gen_openapiv2.options.JSONSchemaR\x0eopenapiv2FieldBHZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/optionsb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.annotations_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.FileOptions.RegisterExtension(openapiv2_swagger)
-  google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(openapiv2_operation)
-  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(openapiv2_schema)
-  google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(openapiv2_tag)
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(openapiv2_field)
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/options'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'ZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/options'
 # @@protoc_insertion_point(module_scope)
```

## protoc_gen_openapiv2/options/openapiv2_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: protoc-gen-openapiv2/options/openapiv2.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -16,45 +17,44 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,protoc-gen-openapiv2/options/openapiv2.proto\x12)grpc.gateway.protoc_gen_openapiv2.options\x1a\x1cgoogle/protobuf/struct.proto\"\xb3\x08\n\x07Swagger\x12\x18\n\x07swagger\x18\x01 \x01(\tR\x07swagger\x12\x43\n\x04info\x18\x02 \x01(\x0b\x32/.grpc.gateway.protoc_gen_openapiv2.options.InfoR\x04info\x12\x12\n\x04host\x18\x03 \x01(\tR\x04host\x12\x1b\n\tbase_path\x18\x04 \x01(\tR\x08\x62\x61sePath\x12K\n\x07schemes\x18\x05 \x03(\x0e\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.SchemeR\x07schemes\x12\x1a\n\x08\x63onsumes\x18\x06 \x03(\tR\x08\x63onsumes\x12\x1a\n\x08produces\x18\x07 \x03(\tR\x08produces\x12_\n\tresponses\x18\n \x03(\x0b\x32\x41.grpc.gateway.protoc_gen_openapiv2.options.Swagger.ResponsesEntryR\tresponses\x12q\n\x14security_definitions\x18\x0b \x01(\x0b\x32>.grpc.gateway.protoc_gen_openapiv2.options.SecurityDefinitionsR\x13securityDefinitions\x12Z\n\x08security\x18\x0c \x03(\x0b\x32>.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirementR\x08security\x12\x42\n\x04tags\x18\r \x03(\x0b\x32..grpc.gateway.protoc_gen_openapiv2.options.TagR\x04tags\x12\x65\n\rexternal_docs\x18\x0e \x01(\x0b\x32@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentationR\x0c\x65xternalDocs\x12\x62\n\nextensions\x18\x0f \x03(\x0b\x32\x42.grpc.gateway.protoc_gen_openapiv2.options.Swagger.ExtensionsEntryR\nextensions\x1aq\n\x0eResponsesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12I\n\x05value\x18\x02 \x01(\x0b\x32\x33.grpc.gateway.protoc_gen_openapiv2.options.ResponseR\x05value:\x02\x38\x01\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01J\x04\x08\x08\x10\tJ\x04\x08\t\x10\n\"\xd6\x07\n\tOperation\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags\x12\x18\n\x07summary\x18\x02 \x01(\tR\x07summary\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x65\n\rexternal_docs\x18\x04 \x01(\x0b\x32@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentationR\x0c\x65xternalDocs\x12!\n\x0coperation_id\x18\x05 \x01(\tR\x0boperationId\x12\x1a\n\x08\x63onsumes\x18\x06 \x03(\tR\x08\x63onsumes\x12\x1a\n\x08produces\x18\x07 \x03(\tR\x08produces\x12\x61\n\tresponses\x18\t \x03(\x0b\x32\x43.grpc.gateway.protoc_gen_openapiv2.options.Operation.ResponsesEntryR\tresponses\x12K\n\x07schemes\x18\n \x03(\x0e\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.SchemeR\x07schemes\x12\x1e\n\ndeprecated\x18\x0b \x01(\x08R\ndeprecated\x12Z\n\x08security\x18\x0c \x03(\x0b\x32>.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirementR\x08security\x12\x64\n\nextensions\x18\r \x03(\x0b\x32\x44.grpc.gateway.protoc_gen_openapiv2.options.Operation.ExtensionsEntryR\nextensions\x12U\n\nparameters\x18\x0e \x01(\x0b\x32\x35.grpc.gateway.protoc_gen_openapiv2.options.ParametersR\nparameters\x1aq\n\x0eResponsesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12I\n\x05value\x18\x02 \x01(\x0b\x32\x33.grpc.gateway.protoc_gen_openapiv2.options.ResponseR\x05value:\x02\x38\x01\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01J\x04\x08\x08\x10\t\"b\n\nParameters\x12T\n\x07headers\x18\x01 \x03(\x0b\x32:.grpc.gateway.protoc_gen_openapiv2.options.HeaderParameterR\x07headers\"\xa3\x02\n\x0fHeaderParameter\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12S\n\x04type\x18\x03 \x01(\x0e\x32?.grpc.gateway.protoc_gen_openapiv2.options.HeaderParameter.TypeR\x04type\x12\x16\n\x06\x66ormat\x18\x04 \x01(\tR\x06\x66ormat\x12\x1a\n\x08required\x18\x05 \x01(\x08R\x08required\"E\n\x04Type\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06STRING\x10\x01\x12\n\n\x06NUMBER\x10\x02\x12\x0b\n\x07INTEGER\x10\x03\x12\x0b\n\x07\x42OOLEAN\x10\x04J\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08\"\xd8\x01\n\x06Header\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x16\n\x06\x66ormat\x18\x03 \x01(\tR\x06\x66ormat\x12\x18\n\x07\x64\x65\x66\x61ult\x18\x06 \x01(\tR\x07\x64\x65\x66\x61ult\x12\x18\n\x07pattern\x18\r \x01(\tR\x07patternJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\n\x10\x0bJ\x04\x08\x0b\x10\x0cJ\x04\x08\x0c\x10\rJ\x04\x08\x0e\x10\x0fJ\x04\x08\x0f\x10\x10J\x04\x08\x10\x10\x11J\x04\x08\x11\x10\x12J\x04\x08\x12\x10\x13\"\x9a\x05\n\x08Response\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12I\n\x06schema\x18\x02 \x01(\x0b\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.SchemaR\x06schema\x12Z\n\x07headers\x18\x03 \x03(\x0b\x32@.grpc.gateway.protoc_gen_openapiv2.options.Response.HeadersEntryR\x07headers\x12]\n\x08\x65xamples\x18\x04 \x03(\x0b\x32\x41.grpc.gateway.protoc_gen_openapiv2.options.Response.ExamplesEntryR\x08\x65xamples\x12\x63\n\nextensions\x18\x05 \x03(\x0b\x32\x43.grpc.gateway.protoc_gen_openapiv2.options.Response.ExtensionsEntryR\nextensions\x1am\n\x0cHeadersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12G\n\x05value\x18\x02 \x01(\x0b\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.HeaderR\x05value:\x02\x38\x01\x1a;\n\rExamplesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\"\xd6\x03\n\x04Info\x12\x14\n\x05title\x18\x01 \x01(\tR\x05title\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12(\n\x10terms_of_service\x18\x03 \x01(\tR\x0etermsOfService\x12L\n\x07\x63ontact\x18\x04 \x01(\x0b\x32\x32.grpc.gateway.protoc_gen_openapiv2.options.ContactR\x07\x63ontact\x12L\n\x07license\x18\x05 \x01(\x0b\x32\x32.grpc.gateway.protoc_gen_openapiv2.options.LicenseR\x07license\x12\x18\n\x07version\x18\x06 \x01(\tR\x07version\x12_\n\nextensions\x18\x07 \x03(\x0b\x32?.grpc.gateway.protoc_gen_openapiv2.options.Info.ExtensionsEntryR\nextensions\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\"E\n\x07\x43ontact\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\x12\x14\n\x05\x65mail\x18\x03 \x01(\tR\x05\x65mail\"/\n\x07License\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\"K\n\x15\x45xternalDocumentation\x12 \n\x0b\x64\x65scription\x18\x01 \x01(\tR\x0b\x64\x65scription\x12\x10\n\x03url\x18\x02 \x01(\tR\x03url\"\xaa\x02\n\x06Schema\x12V\n\x0bjson_schema\x18\x01 \x01(\x0b\x32\x35.grpc.gateway.protoc_gen_openapiv2.options.JSONSchemaR\njsonSchema\x12$\n\rdiscriminator\x18\x02 \x01(\tR\rdiscriminator\x12\x1b\n\tread_only\x18\x03 \x01(\x08R\x08readOnly\x12\x65\n\rexternal_docs\x18\x05 \x01(\x0b\x32@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentationR\x0c\x65xternalDocs\x12\x18\n\x07\x65xample\x18\x06 \x01(\tR\x07\x65xampleJ\x04\x08\x04\x10\x05\"\xd7\n\n\nJSONSchema\x12\x10\n\x03ref\x18\x03 \x01(\tR\x03ref\x12\x14\n\x05title\x18\x05 \x01(\tR\x05title\x12 \n\x0b\x64\x65scription\x18\x06 \x01(\tR\x0b\x64\x65scription\x12\x18\n\x07\x64\x65\x66\x61ult\x18\x07 \x01(\tR\x07\x64\x65\x66\x61ult\x12\x1b\n\tread_only\x18\x08 \x01(\x08R\x08readOnly\x12\x18\n\x07\x65xample\x18\t \x01(\tR\x07\x65xample\x12\x1f\n\x0bmultiple_of\x18\n \x01(\x01R\nmultipleOf\x12\x18\n\x07maximum\x18\x0b \x01(\x01R\x07maximum\x12+\n\x11\x65xclusive_maximum\x18\x0c \x01(\x08R\x10\x65xclusiveMaximum\x12\x18\n\x07minimum\x18\r \x01(\x01R\x07minimum\x12+\n\x11\x65xclusive_minimum\x18\x0e \x01(\x08R\x10\x65xclusiveMinimum\x12\x1d\n\nmax_length\x18\x0f \x01(\x04R\tmaxLength\x12\x1d\n\nmin_length\x18\x10 \x01(\x04R\tminLength\x12\x18\n\x07pattern\x18\x11 \x01(\tR\x07pattern\x12\x1b\n\tmax_items\x18\x14 \x01(\x04R\x08maxItems\x12\x1b\n\tmin_items\x18\x15 \x01(\x04R\x08minItems\x12!\n\x0cunique_items\x18\x16 \x01(\x08R\x0buniqueItems\x12%\n\x0emax_properties\x18\x18 \x01(\x04R\rmaxProperties\x12%\n\x0emin_properties\x18\x19 \x01(\x04R\rminProperties\x12\x1a\n\x08required\x18\x1a \x03(\tR\x08required\x12\x14\n\x05\x61rray\x18\" \x03(\tR\x05\x61rray\x12_\n\x04type\x18# \x03(\x0e\x32K.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema.JSONSchemaSimpleTypesR\x04type\x12\x16\n\x06\x66ormat\x18$ \x01(\tR\x06\x66ormat\x12\x12\n\x04\x65num\x18. \x03(\tR\x04\x65num\x12z\n\x13\x66ield_configuration\x18\xe9\x07 \x01(\x0b\x32H.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema.FieldConfigurationR\x12\x66ieldConfiguration\x12\x65\n\nextensions\x18\x30 \x03(\x0b\x32\x45.grpc.gateway.protoc_gen_openapiv2.options.JSONSchema.ExtensionsEntryR\nextensions\x1a<\n\x12\x46ieldConfiguration\x12&\n\x0fpath_param_name\x18/ \x01(\tR\rpathParamName\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\"w\n\x15JSONSchemaSimpleTypes\x12\x0b\n\x07UNKNOWN\x10\x00\x12\t\n\x05\x41RRAY\x10\x01\x12\x0b\n\x07\x42OOLEAN\x10\x02\x12\x0b\n\x07INTEGER\x10\x03\x12\x08\n\x04NULL\x10\x04\x12\n\n\x06NUMBER\x10\x05\x12\n\n\x06OBJECT\x10\x06\x12\n\n\x06STRING\x10\x07J\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03J\x04\x08\x04\x10\x05J\x04\x08\x12\x10\x13J\x04\x08\x13\x10\x14J\x04\x08\x17\x10\x18J\x04\x08\x1b\x10\x1cJ\x04\x08\x1c\x10\x1dJ\x04\x08\x1d\x10\x1eJ\x04\x08\x1e\x10\"J\x04\x08%\x10*J\x04\x08*\x10+J\x04\x08+\x10.\"\xd9\x02\n\x03Tag\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x65\n\rexternal_docs\x18\x03 \x01(\x0b\x32@.grpc.gateway.protoc_gen_openapiv2.options.ExternalDocumentationR\x0c\x65xternalDocs\x12^\n\nextensions\x18\x04 \x03(\x0b\x32>.grpc.gateway.protoc_gen_openapiv2.options.Tag.ExtensionsEntryR\nextensions\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\"\xf7\x01\n\x13SecurityDefinitions\x12h\n\x08security\x18\x01 \x03(\x0b\x32L.grpc.gateway.protoc_gen_openapiv2.options.SecurityDefinitions.SecurityEntryR\x08security\x1av\n\rSecurityEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12O\n\x05value\x18\x02 \x01(\x0b\x32\x39.grpc.gateway.protoc_gen_openapiv2.options.SecuritySchemeR\x05value:\x02\x38\x01\"\xff\x06\n\x0eSecurityScheme\x12R\n\x04type\x18\x01 \x01(\x0e\x32>.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.TypeR\x04type\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12L\n\x02in\x18\x04 \x01(\x0e\x32<.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.InR\x02in\x12R\n\x04\x66low\x18\x05 \x01(\x0e\x32>.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.FlowR\x04\x66low\x12+\n\x11\x61uthorization_url\x18\x06 \x01(\tR\x10\x61uthorizationUrl\x12\x1b\n\ttoken_url\x18\x07 \x01(\tR\x08tokenUrl\x12I\n\x06scopes\x18\x08 \x01(\x0b\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.ScopesR\x06scopes\x12i\n\nextensions\x18\t \x03(\x0b\x32I.grpc.gateway.protoc_gen_openapiv2.options.SecurityScheme.ExtensionsEntryR\nextensions\x1aU\n\x0f\x45xtensionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\"K\n\x04Type\x12\x10\n\x0cTYPE_INVALID\x10\x00\x12\x0e\n\nTYPE_BASIC\x10\x01\x12\x10\n\x0cTYPE_API_KEY\x10\x02\x12\x0f\n\x0bTYPE_OAUTH2\x10\x03\"1\n\x02In\x12\x0e\n\nIN_INVALID\x10\x00\x12\x0c\n\x08IN_QUERY\x10\x01\x12\r\n\tIN_HEADER\x10\x02\"j\n\x04\x46low\x12\x10\n\x0c\x46LOW_INVALID\x10\x00\x12\x11\n\rFLOW_IMPLICIT\x10\x01\x12\x11\n\rFLOW_PASSWORD\x10\x02\x12\x14\n\x10\x46LOW_APPLICATION\x10\x03\x12\x14\n\x10\x46LOW_ACCESS_CODE\x10\x04\"\xf6\x02\n\x13SecurityRequirement\x12\x8a\x01\n\x14security_requirement\x18\x01 \x03(\x0b\x32W.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement.SecurityRequirementEntryR\x13securityRequirement\x1a\x30\n\x18SecurityRequirementValue\x12\x14\n\x05scope\x18\x01 \x03(\tR\x05scope\x1a\x9f\x01\n\x18SecurityRequirementEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12m\n\x05value\x18\x02 \x01(\x0b\x32W.grpc.gateway.protoc_gen_openapiv2.options.SecurityRequirement.SecurityRequirementValueR\x05value:\x02\x38\x01\"\x96\x01\n\x06Scopes\x12R\n\x05scope\x18\x01 \x03(\x0b\x32<.grpc.gateway.protoc_gen_openapiv2.options.Scopes.ScopeEntryR\x05scope\x1a\x38\n\nScopeEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01*;\n\x06Scheme\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04HTTP\x10\x01\x12\t\n\x05HTTPS\x10\x02\x12\x06\n\x02WS\x10\x03\x12\x07\n\x03WSS\x10\x04\x42HZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/optionsb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.openapiv2_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'ZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/options'
-  _SWAGGER_RESPONSESENTRY._options = None
-  _SWAGGER_RESPONSESENTRY._serialized_options = b'8\001'
-  _SWAGGER_EXTENSIONSENTRY._options = None
-  _SWAGGER_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _OPERATION_RESPONSESENTRY._options = None
-  _OPERATION_RESPONSESENTRY._serialized_options = b'8\001'
-  _OPERATION_EXTENSIONSENTRY._options = None
-  _OPERATION_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _RESPONSE_HEADERSENTRY._options = None
-  _RESPONSE_HEADERSENTRY._serialized_options = b'8\001'
-  _RESPONSE_EXAMPLESENTRY._options = None
-  _RESPONSE_EXAMPLESENTRY._serialized_options = b'8\001'
-  _RESPONSE_EXTENSIONSENTRY._options = None
-  _RESPONSE_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _INFO_EXTENSIONSENTRY._options = None
-  _INFO_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _JSONSCHEMA_EXTENSIONSENTRY._options = None
-  _JSONSCHEMA_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _TAG_EXTENSIONSENTRY._options = None
-  _TAG_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _SECURITYDEFINITIONS_SECURITYENTRY._options = None
-  _SECURITYDEFINITIONS_SECURITYENTRY._serialized_options = b'8\001'
-  _SECURITYSCHEME_EXTENSIONSENTRY._options = None
-  _SECURITYSCHEME_EXTENSIONSENTRY._serialized_options = b'8\001'
-  _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._options = None
-  _SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY._serialized_options = b'8\001'
-  _SCOPES_SCOPEENTRY._options = None
-  _SCOPES_SCOPEENTRY._serialized_options = b'8\001'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'ZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/options'
+  _globals['_SWAGGER_RESPONSESENTRY']._options = None
+  _globals['_SWAGGER_RESPONSESENTRY']._serialized_options = b'8\001'
+  _globals['_SWAGGER_EXTENSIONSENTRY']._options = None
+  _globals['_SWAGGER_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_OPERATION_RESPONSESENTRY']._options = None
+  _globals['_OPERATION_RESPONSESENTRY']._serialized_options = b'8\001'
+  _globals['_OPERATION_EXTENSIONSENTRY']._options = None
+  _globals['_OPERATION_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_RESPONSE_HEADERSENTRY']._options = None
+  _globals['_RESPONSE_HEADERSENTRY']._serialized_options = b'8\001'
+  _globals['_RESPONSE_EXAMPLESENTRY']._options = None
+  _globals['_RESPONSE_EXAMPLESENTRY']._serialized_options = b'8\001'
+  _globals['_RESPONSE_EXTENSIONSENTRY']._options = None
+  _globals['_RESPONSE_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_INFO_EXTENSIONSENTRY']._options = None
+  _globals['_INFO_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_JSONSCHEMA_EXTENSIONSENTRY']._options = None
+  _globals['_JSONSCHEMA_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_TAG_EXTENSIONSENTRY']._options = None
+  _globals['_TAG_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_SECURITYDEFINITIONS_SECURITYENTRY']._options = None
+  _globals['_SECURITYDEFINITIONS_SECURITYENTRY']._serialized_options = b'8\001'
+  _globals['_SECURITYSCHEME_EXTENSIONSENTRY']._options = None
+  _globals['_SECURITYSCHEME_EXTENSIONSENTRY']._serialized_options = b'8\001'
+  _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY']._options = None
+  _globals['_SECURITYREQUIREMENT_SECURITYREQUIREMENTENTRY']._serialized_options = b'8\001'
+  _globals['_SCOPES_SCOPEENTRY']._options = None
+  _globals['_SCOPES_SCOPEENTRY']._serialized_options = b'8\001'
   _globals['_SCHEME']._serialized_start=7833
   _globals['_SCHEME']._serialized_end=7892
   _globals['_SWAGGER']._serialized_start=122
   _globals['_SWAGGER']._serialized_end=1197
   _globals['_SWAGGER_RESPONSESENTRY']._serialized_start=985
   _globals['_SWAGGER_RESPONSESENTRY']._serialized_end=1098
   _globals['_SWAGGER_EXTENSIONSENTRY']._serialized_start=1100
```

## validate/validate_pb2.py

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: validate/validate.proto
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -18,21 +19,16 @@
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17validate/validate.proto\x12\x08validate\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xc8\x08\n\nFieldRules\x12\x30\n\x07message\x18\x11 \x01(\x0b\x32\x16.validate.MessageRulesR\x07message\x12,\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x14.validate.FloatRulesH\x00R\x05\x66loat\x12/\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x15.validate.DoubleRulesH\x00R\x06\x64ouble\x12,\n\x05int32\x18\x03 \x01(\x0b\x32\x14.validate.Int32RulesH\x00R\x05int32\x12,\n\x05int64\x18\x04 \x01(\x0b\x32\x14.validate.Int64RulesH\x00R\x05int64\x12/\n\x06uint32\x18\x05 \x01(\x0b\x32\x15.validate.UInt32RulesH\x00R\x06uint32\x12/\n\x06uint64\x18\x06 \x01(\x0b\x32\x15.validate.UInt64RulesH\x00R\x06uint64\x12/\n\x06sint32\x18\x07 \x01(\x0b\x32\x15.validate.SInt32RulesH\x00R\x06sint32\x12/\n\x06sint64\x18\x08 \x01(\x0b\x32\x15.validate.SInt64RulesH\x00R\x06sint64\x12\x32\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x16.validate.Fixed32RulesH\x00R\x07\x66ixed32\x12\x32\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x16.validate.Fixed64RulesH\x00R\x07\x66ixed64\x12\x35\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x17.validate.SFixed32RulesH\x00R\x08sfixed32\x12\x35\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x17.validate.SFixed64RulesH\x00R\x08sfixed64\x12)\n\x04\x62ool\x18\r \x01(\x0b\x32\x13.validate.BoolRulesH\x00R\x04\x62ool\x12/\n\x06string\x18\x0e \x01(\x0b\x32\x15.validate.StringRulesH\x00R\x06string\x12,\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x14.validate.BytesRulesH\x00R\x05\x62ytes\x12)\n\x04\x65num\x18\x10 \x01(\x0b\x32\x13.validate.EnumRulesH\x00R\x04\x65num\x12\x35\n\x08repeated\x18\x12 \x01(\x0b\x32\x17.validate.RepeatedRulesH\x00R\x08repeated\x12&\n\x03map\x18\x13 \x01(\x0b\x32\x12.validate.MapRulesH\x00R\x03map\x12&\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x12.validate.AnyRulesH\x00R\x03\x61ny\x12\x35\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x17.validate.DurationRulesH\x00R\x08\x64uration\x12\x38\n\ttimestamp\x18\x16 \x01(\x0b\x32\x18.validate.TimestampRulesH\x00R\ttimestampB\x06\n\x04type\"\xb0\x01\n\nFloatRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x02R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x02R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x02R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x02R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x02R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x02R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x02R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb1\x01\n\x0b\x44oubleRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x01R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x01R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x01R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x01R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x01R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x01R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x01R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb0\x01\n\nInt32Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x05R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x05R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x05R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x05R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x05R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x05R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x05R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb0\x01\n\nInt64Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x03R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x03R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x03R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x03R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x03R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x03R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x03R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb1\x01\n\x0bUInt32Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\rR\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\rR\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\rR\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\rR\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\rR\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\rR\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\rR\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb1\x01\n\x0bUInt64Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x04R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x04R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x04R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x04R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x04R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x04R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x04R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb1\x01\n\x0bSInt32Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x11R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x11R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x11R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x11R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x11R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x11R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x11R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb1\x01\n\x0bSInt64Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x12R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x12R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x12R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x12R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x12R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x12R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x12R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb2\x01\n\x0c\x46ixed32Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x07R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x07R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x07R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x07R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x07R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x07R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x07R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb2\x01\n\x0c\x46ixed64Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x06R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x06R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x06R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x06R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x06R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x06R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x06R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb3\x01\n\rSFixed32Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x0fR\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x0fR\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x0fR\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x0fR\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x0fR\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x0fR\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x0fR\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"\xb3\x01\n\rSFixed64Rules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x10R\x05\x63onst\x12\x0e\n\x02lt\x18\x02 \x01(\x10R\x02lt\x12\x10\n\x03lte\x18\x03 \x01(\x10R\x03lte\x12\x0e\n\x02gt\x18\x04 \x01(\x10R\x02gt\x12\x10\n\x03gte\x18\x05 \x01(\x10R\x03gte\x12\x0e\n\x02in\x18\x06 \x03(\x10R\x02in\x12\x15\n\x06not_in\x18\x07 \x03(\x10R\x05notIn\x12!\n\x0cignore_empty\x18\x08 \x01(\x08R\x0bignoreEmpty\"!\n\tBoolRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x08R\x05\x63onst\"\xd4\x05\n\x0bStringRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\tR\x05\x63onst\x12\x10\n\x03len\x18\x13 \x01(\x04R\x03len\x12\x17\n\x07min_len\x18\x02 \x01(\x04R\x06minLen\x12\x17\n\x07max_len\x18\x03 \x01(\x04R\x06maxLen\x12\x1b\n\tlen_bytes\x18\x14 \x01(\x04R\x08lenBytes\x12\x1b\n\tmin_bytes\x18\x04 \x01(\x04R\x08minBytes\x12\x1b\n\tmax_bytes\x18\x05 \x01(\x04R\x08maxBytes\x12\x18\n\x07pattern\x18\x06 \x01(\tR\x07pattern\x12\x16\n\x06prefix\x18\x07 \x01(\tR\x06prefix\x12\x16\n\x06suffix\x18\x08 \x01(\tR\x06suffix\x12\x1a\n\x08\x63ontains\x18\t \x01(\tR\x08\x63ontains\x12!\n\x0cnot_contains\x18\x17 \x01(\tR\x0bnotContains\x12\x0e\n\x02in\x18\n \x03(\tR\x02in\x12\x15\n\x06not_in\x18\x0b \x03(\tR\x05notIn\x12\x16\n\x05\x65mail\x18\x0c \x01(\x08H\x00R\x05\x65mail\x12\x1c\n\x08hostname\x18\r \x01(\x08H\x00R\x08hostname\x12\x10\n\x02ip\x18\x0e \x01(\x08H\x00R\x02ip\x12\x14\n\x04ipv4\x18\x0f \x01(\x08H\x00R\x04ipv4\x12\x14\n\x04ipv6\x18\x10 \x01(\x08H\x00R\x04ipv6\x12\x12\n\x03uri\x18\x11 \x01(\x08H\x00R\x03uri\x12\x19\n\x07uri_ref\x18\x12 \x01(\x08H\x00R\x06uriRef\x12\x1a\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08H\x00R\x07\x61\x64\x64ress\x12\x14\n\x04uuid\x18\x16 \x01(\x08H\x00R\x04uuid\x12@\n\x10well_known_regex\x18\x18 \x01(\x0e\x32\x14.validate.KnownRegexH\x00R\x0ewellKnownRegex\x12\x1c\n\x06strict\x18\x19 \x01(\x08:\x04trueR\x06strict\x12!\n\x0cignore_empty\x18\x1a \x01(\x08R\x0bignoreEmptyB\x0c\n\nwell_known\"\xe2\x02\n\nBytesRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x0cR\x05\x63onst\x12\x10\n\x03len\x18\r \x01(\x04R\x03len\x12\x17\n\x07min_len\x18\x02 \x01(\x04R\x06minLen\x12\x17\n\x07max_len\x18\x03 \x01(\x04R\x06maxLen\x12\x18\n\x07pattern\x18\x04 \x01(\tR\x07pattern\x12\x16\n\x06prefix\x18\x05 \x01(\x0cR\x06prefix\x12\x16\n\x06suffix\x18\x06 \x01(\x0cR\x06suffix\x12\x1a\n\x08\x63ontains\x18\x07 \x01(\x0cR\x08\x63ontains\x12\x0e\n\x02in\x18\x08 \x03(\x0cR\x02in\x12\x15\n\x06not_in\x18\t \x03(\x0cR\x05notIn\x12\x10\n\x02ip\x18\n \x01(\x08H\x00R\x02ip\x12\x14\n\x04ipv4\x18\x0b \x01(\x08H\x00R\x04ipv4\x12\x14\n\x04ipv6\x18\x0c \x01(\x08H\x00R\x04ipv6\x12!\n\x0cignore_empty\x18\x0e \x01(\x08R\x0bignoreEmptyB\x0c\n\nwell_known\"k\n\tEnumRules\x12\x14\n\x05\x63onst\x18\x01 \x01(\x05R\x05\x63onst\x12!\n\x0c\x64\x65\x66ined_only\x18\x02 \x01(\x08R\x0b\x64\x65\x66inedOnly\x12\x0e\n\x02in\x18\x03 \x03(\x05R\x02in\x12\x15\n\x06not_in\x18\x04 \x03(\x05R\x05notIn\">\n\x0cMessageRules\x12\x12\n\x04skip\x18\x01 \x01(\x08R\x04skip\x12\x1a\n\x08required\x18\x02 \x01(\x08R\x08required\"\xb0\x01\n\rRepeatedRules\x12\x1b\n\tmin_items\x18\x01 \x01(\x04R\x08minItems\x12\x1b\n\tmax_items\x18\x02 \x01(\x04R\x08maxItems\x12\x16\n\x06unique\x18\x03 \x01(\x08R\x06unique\x12*\n\x05items\x18\x04 \x01(\x0b\x32\x14.validate.FieldRulesR\x05items\x12!\n\x0cignore_empty\x18\x05 \x01(\x08R\x0bignoreEmpty\"\xdc\x01\n\x08MapRules\x12\x1b\n\tmin_pairs\x18\x01 \x01(\x04R\x08minPairs\x12\x1b\n\tmax_pairs\x18\x02 \x01(\x04R\x08maxPairs\x12\x1b\n\tno_sparse\x18\x03 \x01(\x08R\x08noSparse\x12(\n\x04keys\x18\x04 \x01(\x0b\x32\x14.validate.FieldRulesR\x04keys\x12,\n\x06values\x18\x05 \x01(\x0b\x32\x14.validate.FieldRulesR\x06values\x12!\n\x0cignore_empty\x18\x06 \x01(\x08R\x0bignoreEmpty\"M\n\x08\x41nyRules\x12\x1a\n\x08required\x18\x01 \x01(\x08R\x08required\x12\x0e\n\x02in\x18\x02 \x03(\tR\x02in\x12\x15\n\x06not_in\x18\x03 \x03(\tR\x05notIn\"\xe9\x02\n\rDurationRules\x12\x1a\n\x08required\x18\x01 \x01(\x08R\x08required\x12/\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05\x63onst\x12)\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationR\x02lt\x12+\n\x03lte\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03lte\x12)\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x02gt\x12+\n\x03gte\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03gte\x12)\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.DurationR\x02in\x12\x30\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.DurationR\x05notIn\"\xf3\x02\n\x0eTimestampRules\x12\x1a\n\x08required\x18\x01 \x01(\x08R\x08required\x12\x30\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05\x63onst\x12*\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x02lt\x12,\n\x03lte\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03lte\x12*\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x02gt\x12,\n\x03gte\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03gte\x12\x15\n\x06lt_now\x18\x07 \x01(\x08R\x05ltNow\x12\x15\n\x06gt_now\x18\x08 \x01(\x08R\x05gtNow\x12\x31\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationR\x06within*F\n\nKnownRegex\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x14\n\x10HTTP_HEADER_NAME\x10\x01\x12\x15\n\x11HTTP_HEADER_VALUE\x10\x02:<\n\x08\x64isabled\x12\x1f.google.protobuf.MessageOptions\x18\xaf\x08 \x01(\x08R\x08\x64isabled::\n\x07ignored\x12\x1f.google.protobuf.MessageOptions\x18\xb0\x08 \x01(\x08R\x07ignored::\n\x08required\x12\x1d.google.protobuf.OneofOptions\x18\xaf\x08 \x01(\x08R\x08required:J\n\x05rules\x12\x1d.google.protobuf.FieldOptions\x18\xaf\x08 \x01(\x0b\x32\x14.validate.FieldRulesR\x05rulesBP\n\x1aio.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'validate.validate_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(disabled)
-  google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(ignored)
-  google_dot_protobuf_dot_descriptor__pb2.OneofOptions.RegisterExtension(required)
-  google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(rules)
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\032io.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate'
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\032io.envoyproxy.pgv.validateZ2github.com/envoyproxy/protoc-gen-validate/validate'
   _globals['_KNOWNREGEX']._serialized_start=5909
   _globals['_KNOWNREGEX']._serialized_end=5979
   _globals['_FIELDRULES']._serialized_start=137
   _globals['_FIELDRULES']._serialized_end=1233
   _globals['_FLOATRULES']._serialized_start=1236
   _globals['_FLOATRULES']._serialized_end=1412
   _globals['_DOUBLERULES']._serialized_start=1415
```

## Comparing `fathom_global_client_sdk-0.8.0.dist-info/METADATA` & `fathom_global_client_sdk-0.9.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 Name: fathom_global_client_sdk
 Author: Fathom
 Home-page: https://fathom.global
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: protoc-gen-validate==0.10.1
-Requires-Dist: googleapis-common-protos==1.56.2
-Requires-Dist: grpcio==1.50.0
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Requires-Dist: googleapis-common-protos==1.62.0
+Requires-Dist: grpcio==1.60.0
+Requires-Dist: protoc-gen-validate==1.0.2
 Requires-Dist: requests>=2,<3
-Version: 0.8.0
+Version: 0.9.0
 
 # Fathom Python SDK client
 
 The Python SDK client for communicating with the Fathom API
 
 Example usage:
```

