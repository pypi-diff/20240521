# Comparing `tmp/smol_k8s_lab-5.0.4.tar.gz` & `tmp/smol_k8s_lab-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smol_k8s_lab-5.0.4.tar", max compression
+gzip compressed data, was "smol_k8s_lab-5.1.0.tar", max compression
```

## Comparing `smol_k8s_lab-5.0.4.tar` & `smol_k8s_lab-5.1.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0    34260 2024-05-19 12:10:40.954392 smol_k8s_lab-5.0.4/LICENSE
--rw-r--r--   0        0        0    29410 2024-05-19 12:10:40.954392 smol_k8s_lab-5.0.4/README.md
--rw-r--r--   0        0        0     3300 2024-05-19 12:10:41.230394 smol_k8s_lab-5.0.4/pyproject.toml
--rwxr-xr-x   0        0        0    16188 2024-05-19 12:10:41.230394 smol_k8s_lab-5.0.4/smol_k8s_lab/__init__.py
--rw-r--r--   0        0        0  5853144 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/audio/audio-en.tar.gz
--rwxr-xr-x   0        0        0    12759 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/bw_cli.py
--rw-r--r--   0        0        0     1679 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden.css
--rw-r--r--   0        0        0     2093 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
--rw-r--r--   0        0        0     4524 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
--rw-r--r--   0        0        0     2395 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
--rw-r--r--   0        0        0     6916 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
--rw-r--r--   0        0        0    17031 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/audio/en.yml
--rw-r--r--   0        0        0     2364 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/audio/nl.yml
--rw-r--r--   0        0        0    78459 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/default_config.yaml
--rw-r--r--   0        0        0     5666 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/keycloak_config.json
--rw-r--r--   0        0        0      237 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/kind/kind-config-cilium.yaml
--rw-r--r--   0        0        0      385 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/kind/kind_cluster_config.yaml
--rw-r--r--   0        0        0      831 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
--rwxr-xr-x   0        0        0     3008 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/constants.py
--rwxr-xr-x   0        0        0    12945 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/env_config.py
--rw-r--r--   0        0        0     9821 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/__init__.py
--rw-r--r--   0        0        0     7789 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/argocd.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
--rw-r--r--   0        0        0     6581 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
--rw-r--r--   0        0        0     9763 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
--rw-r--r--   0        0        0    19076 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
--rw-r--r--   0        0        0    20511 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
--rw-r--r--   0        0        0     3372 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
--rw-r--r--   0        0        0     1285 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
--rw-r--r--   0        0        0     9134 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/initial_special.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/cilium.py
--rw-r--r--   0        0        0     2318 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/metallb.py
--rw-r--r--   0        0        0    10977 2024-05-19 12:10:41.238394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/netmaker.py
--rw-r--r--   0        0        0     2383 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/__init__.py
--rw-r--r--   0        0        0     8381 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/minio.py
--rw-r--r--   0        0        0     3617 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
--rw-r--r--   0        0        0     4286 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
--rw-r--r--   0        0        0     3759 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
--rw-r--r--   0        0        0     4805 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/vault.py
--rw-r--r--   0        0        0    11623 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/home_assistant.py
--rw-r--r--   0        0        0    21465 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/mastodon.py
--rwxr-xr-x   0        0        0     1706 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
--rw-r--r--   0        0        0    18842 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/matrix.py
--rw-r--r--   0        0        0    20726 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/nextcloud.py
--rwxr-xr-x   0        0        0     6182 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
--rw-r--r--   0        0        0     8034 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/__init__.py
--rw-r--r--   0        0        0     3755 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/k3d.py
--rw-r--r--   0        0        0     8481 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/k3s.py
--rw-r--r--   0        0        0     4821 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/kind.py
--rw-r--r--   0        0        0        1 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/__init__.py
--rw-r--r--   0        0        0     8642 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/argocd_util.py
--rw-r--r--   0        0        0     8689 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/backup.py
--rwxr-xr-x   0        0        0     8607 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/helm.py
--rw-r--r--   0        0        0    14252 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/k8s_lib.py
--rw-r--r--   0        0        0    22222 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/restores.py
--rw-r--r--   0        0        0     1358 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/__init__.py
--rw-r--r--   0        0        0    14333 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
--rw-r--r--   0        0        0     9712 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
--rw-r--r--   0        0        0    18578 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
--rw-r--r--   0        0        0    14373 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/input_widgets.py
--rwxr-xr-x   0        0        0     4002 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/invalid_apps.py
--rw-r--r--   0        0        0     6970 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/modify_globals.py
--rw-r--r--   0        0        0     3697 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/new_app_modal.py
--rwxr-xr-x   0        0        0    17593 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/apps_screen.py
--rw-r--r--   0        0        0    12891 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base.py
--rw-r--r--   0        0        0    33063 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/audio_widget.py
--rw-r--r--   0        0        0     7189 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/cluster_modal.py
--rw-r--r--   0        0        0     3384 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
--rwxr-xr-x   0        0        0     8926 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/confirm_screen.py
--rw-r--r--   0        0        0     1546 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/add_nodes_widget.tcss
--rw-r--r--   0        0        0     7174 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/apps_config.tcss
--rw-r--r--   0        0        0     1184 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/apps_init_config.tcss
--rw-r--r--   0        0        0     6681 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/base.tcss
--rw-r--r--   0        0        0      988 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/base_modal.tcss
--rw-r--r--   0        0        0     1371 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/cluster_modal.tcss
--rw-r--r--   0        0        0     1278 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/confirm.tcss
--rw-r--r--   0        0        0     1564 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/distro_config.tcss
--rw-r--r--   0        0        0      927 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/help.tcss
--rw-r--r--   0        0        0      984 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/invalid_apps.tcss
--rw-r--r--   0        0        0     2198 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/k3s.tcss
--rw-r--r--   0        0        0     1901 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/kind.tcss
--rw-r--r--   0        0        0     1259 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/modify_globals_modal.tcss
--rw-r--r--   0        0        0      770 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/new_app_modal.tcss
--rw-r--r--   0        0        0      112 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/new_option_modal.tcss
--rw-r--r--   0        0        0     1168 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/node_inputs_widget.tcss
--rw-r--r--   0        0        0     1101 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/node_modal.tcss
--rw-r--r--   0        0        0     3433 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
--rw-r--r--   0        0        0     2554 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/tui_config.tcss
--rwxr-xr-x   0        0        0    10391 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_screen.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/__init__.py
--rw-r--r--   0        0        0    17214 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/add_nodes.py
--rw-r--r--   0        0        0    14337 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/k3s_config.py
--rw-r--r--   0        0        0     6754 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/kind_config.py
--rw-r--r--   0        0        0     6060 2024-05-19 12:10:41.242394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
--rw-r--r--   0        0        0     4359 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
--rw-r--r--   0        0        0     4669 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
--rw-r--r--   0        0        0     4193 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/help_screen.py
--rwxr-xr-x   0        0        0     4020 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/make_screenshots.py
--rwxr-xr-x   0        0        0    11139 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/smol_k8s_config_screen.py
--rwxr-xr-x   0        0        0     8811 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/tui_config_screen.py
--rw-r--r--   0        0        0     9901 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/util.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/validators/__init__.py
--rw-r--r--   0        0        0      579 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/tui/validators/already_exists.py
--rw-r--r--   0        0        0        0 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/__init__.py
--rw-r--r--   0        0        0    16300 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/minio_lib.py
--rw-r--r--   0        0        0     1184 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/passwords.py
--rwxr-xr-x   0        0        0     2423 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/rich_cli/console_logging.py
--rwxr-xr-x   0        0        0     4720 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/rich_cli/help_text.py
--rw-r--r--   0        0        0     2610 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/run/final_cmd.py
--rwxr-xr-x   0        0        0     7483 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/run/subproc.py
--rw-r--r--   0        0        0     2837 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/value_from.py
--rw-r--r--   0        0        0      315 2024-05-19 12:10:41.246394 smol_k8s_lab-5.0.4/smol_k8s_lab/utils/yaml_with_comments.py
--rw-r--r--   0        0        0    31096 1970-01-01 00:00:00.000000 smol_k8s_lab-5.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-21 12:03:43.355464 smol_k8s_lab-5.1.0/LICENSE
+-rw-r--r--   0        0        0    29423 2024-05-21 12:03:43.355464 smol_k8s_lab-5.1.0/README.md
+-rw-r--r--   0        0        0     3300 2024-05-21 12:03:43.651462 smol_k8s_lab-5.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0    16188 2024-05-21 12:03:43.651462 smol_k8s_lab-5.1.0/smol_k8s_lab/__init__.py
+-rw-r--r--   0        0        0  5853144 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/audio/audio-en.tar.gz
+-rwxr-xr-x   0        0        0    12759 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/bw_cli.py
+-rw-r--r--   0        0        0     1679 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden.css
+-rw-r--r--   0        0        0     2093 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py
+-rw-r--r--   0        0        0     4524 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py
+-rw-r--r--   0        0        0     2395 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss
+-rw-r--r--   0        0        0     6916 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py
+-rw-r--r--   0        0        0    17031 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/en.yml
+-rw-r--r--   0        0        0     2364 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/nl.yml
+-rw-r--r--   0        0        0    78462 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/default_config.yaml
+-rw-r--r--   0        0        0     5666 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/keycloak_config.json
+-rw-r--r--   0        0        0      237 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/kind/kind-config-cilium.yaml
+-rw-r--r--   0        0        0      385 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/kind/kind_cluster_config.yaml
+-rw-r--r--   0        0        0      831 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml
+-rwxr-xr-x   0        0        0     3008 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/constants.py
+-rwxr-xr-x   0        0        0    12945 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/env_config.py
+-rw-r--r--   0        0        0     9821 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/__init__.py
+-rw-r--r--   0        0        0     7789 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/argocd.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/__init__.py
+-rw-r--r--   0        0        0     6581 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py
+-rw-r--r--   0        0        0     9763 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py
+-rw-r--r--   0        0        0    19076 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py
+-rw-r--r--   0        0        0    20511 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py
+-rw-r--r--   0        0        0     3372 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py
+-rw-r--r--   0        0        0     1285 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py
+-rw-r--r--   0        0        0     9134 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/initial_special.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/cilium.py
+-rw-r--r--   0        0        0     2318 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/metallb.py
+-rw-r--r--   0        0        0    10977 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/netmaker.py
+-rw-r--r--   0        0        0     2383 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/__init__.py
+-rw-r--r--   0        0        0     8381 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/minio.py
+-rw-r--r--   0        0        0     3617 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py
+-rw-r--r--   0        0        0     4286 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/__init__.py
+-rw-r--r--   0        0        0     2675 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py
+-rw-r--r--   0        0        0     3759 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py
+-rw-r--r--   0        0        0     4805 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py
+-rw-r--r--   0        0        0    11623 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/home_assistant.py
+-rw-r--r--   0        0        0    21465 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon.py
+-rwxr-xr-x   0        0        0     1706 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py
+-rw-r--r--   0        0        0    18842 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/matrix.py
+-rw-r--r--   0        0        0    20726 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud.py
+-rwxr-xr-x   0        0        0     6182 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py
+-rw-r--r--   0        0        0     8034 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/__init__.py
+-rw-r--r--   0        0        0     3755 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3d.py
+-rw-r--r--   0        0        0     8481 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3s.py
+-rw-r--r--   0        0        0     4821 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/kind.py
+-rw-r--r--   0        0        0        1 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/__init__.py
+-rw-r--r--   0        0        0     8642 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/argocd_util.py
+-rw-r--r--   0        0        0     8689 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/backup.py
+-rwxr-xr-x   0        0        0     8607 2024-05-21 12:03:43.663462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/helm.py
+-rw-r--r--   0        0        0    14252 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/k8s_lib.py
+-rw-r--r--   0        0        0    22222 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/restores.py
+-rw-r--r--   0        0        0     1358 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/__init__.py
+-rw-r--r--   0        0        0    14333 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py
+-rw-r--r--   0        0        0     9712 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py
+-rw-r--r--   0        0        0    18578 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py
+-rw-r--r--   0        0        0    14373 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/input_widgets.py
+-rwxr-xr-x   0        0        0     4002 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py
+-rw-r--r--   0        0        0     6970 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/modify_globals.py
+-rw-r--r--   0        0        0     3697 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py
+-rwxr-xr-x   0        0        0    17593 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/apps_screen.py
+-rw-r--r--   0        0        0    12891 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base.py
+-rw-r--r--   0        0        0    33063 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/audio_widget.py
+-rw-r--r--   0        0        0     7189 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py
+-rw-r--r--   0        0        0     3384 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py
+-rwxr-xr-x   0        0        0     8926 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/confirm_screen.py
+-rw-r--r--   0        0        0     1546 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss
+-rw-r--r--   0        0        0     7174 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_config.tcss
+-rw-r--r--   0        0        0     1184 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_init_config.tcss
+-rw-r--r--   0        0        0     6681 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base.tcss
+-rw-r--r--   0        0        0      988 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base_modal.tcss
+-rw-r--r--   0        0        0     1371 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/cluster_modal.tcss
+-rw-r--r--   0        0        0     1278 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/confirm.tcss
+-rw-r--r--   0        0        0     1564 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/distro_config.tcss
+-rw-r--r--   0        0        0      927 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/help.tcss
+-rw-r--r--   0        0        0      984 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/invalid_apps.tcss
+-rw-r--r--   0        0        0     2198 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/k3s.tcss
+-rw-r--r--   0        0        0     1901 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/kind.tcss
+-rw-r--r--   0        0        0     1259 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss
+-rw-r--r--   0        0        0      770 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_app_modal.tcss
+-rw-r--r--   0        0        0      112 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_option_modal.tcss
+-rw-r--r--   0        0        0     1168 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss
+-rw-r--r--   0        0        0     1101 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_modal.tcss
+-rw-r--r--   0        0        0     3433 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss
+-rw-r--r--   0        0        0     2554 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/tui_config.tcss
+-rwxr-xr-x   0        0        0    10391 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_screen.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/__init__.py
+-rw-r--r--   0        0        0    17214 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py
+-rw-r--r--   0        0        0    14337 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py
+-rw-r--r--   0        0        0     6754 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kind_config.py
+-rw-r--r--   0        0        0     6060 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py
+-rw-r--r--   0        0        0     4359 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py
+-rw-r--r--   0        0        0     4669 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py
+-rw-r--r--   0        0        0     4193 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/help_screen.py
+-rwxr-xr-x   0        0        0     4020 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/make_screenshots.py
+-rwxr-xr-x   0        0        0    11139 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/smol_k8s_config_screen.py
+-rwxr-xr-x   0        0        0     8811 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/tui_config_screen.py
+-rw-r--r--   0        0        0     9901 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/util.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/__init__.py
+-rw-r--r--   0        0        0      579 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/already_exists.py
+-rw-r--r--   0        0        0        0 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/__init__.py
+-rw-r--r--   0        0        0    16300 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/minio_lib.py
+-rw-r--r--   0        0        0     1184 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/passwords.py
+-rwxr-xr-x   0        0        0     2423 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/console_logging.py
+-rwxr-xr-x   0        0        0     4720 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/help_text.py
+-rw-r--r--   0        0        0     2610 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/final_cmd.py
+-rwxr-xr-x   0        0        0     7483 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/subproc.py
+-rw-r--r--   0        0        0     2837 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/value_from.py
+-rw-r--r--   0        0        0      315 2024-05-21 12:03:43.667462 smol_k8s_lab-5.1.0/smol_k8s_lab/utils/yaml_with_comments.py
+-rw-r--r--   0        0        0    31109 1970-01-01 00:00:00.000000 smol_k8s_lab-5.1.0/PKG-INFO
```

### Comparing `smol_k8s_lab-5.0.4/LICENSE` & `smol_k8s_lab-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/README.md` & `smol_k8s_lab-5.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 ### Features
 - Deploys [Argo CD](https://github.com/argoproj/argo-cd) by default, so you can manage your entire lab using files in [open source git repos](https://github.com/small-hack/argocd-apps)
   - Argo CD ships with a dashboard with a custom theme 💙
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
-  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups
+  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups and restores
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
 -----------------------------
 
 * [Installation](#installation)
     * [pipx](#pipx)
     * [brew (still unstable)](#brew-still-unstable)
```

#### html2text {}

```diff
@@ -18,35 +18,35 @@
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
 hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - featured initialized apps
 such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
 nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
 matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/
-k8s_apps/home_assistant/) include backups - Lots o' [docs](https://small-
-hack.github.io/smol-k8s-lab) ----------------------------- * [Installation]
-(#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-still-unstable)
-* [Usage](#usage) * [Initialization](#initialization) * [Under the hood]
-(#under-the-hood) * [Supported k8s distributions](#supported-k8s-distributions)
-* [Default Installed Applications](#default-installed-applications) * [Status]
-(#status) # Installation B sure to check out our full [installation guide]
-(https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it
-is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon). ## pipx
-`smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
-pipx)). If you've already got both and [other pre-reqs](https://small-
-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
-to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
-before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
-the future preferred installation method for macOS/Debian/Ubuntu, as this will
-also install any non-python prerequisites you need, so you don't need to worry
-about them. This method is new, so please [let us know if anything isn't
-working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
-tap the special homebrew repo for our formula and install it brew install
-small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
-and cli options with: ```bash smol-k8s-lab --help ```
+k8s_apps/home_assistant/) include backups and restores - Lots o' [docs](https:/
+/small-hack.github.io/smol-k8s-lab) ----------------------------- *
+[Installation](#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-
+still-unstable) * [Usage](#usage) * [Initialization](#initialization) * [Under
+the hood](#under-the-hood) * [Supported k8s distributions](#supported-k8s-
+distributions) * [Default Installed Applications](#default-installed-
+applications) * [Status](#status) # Installation B sure to check out our full
+[installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
+but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
+coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
+github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
+/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
+able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
+menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
+[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
+as this will also install any non-python prerequisites you need, so you don't
+need to worry about them. This method is new, so please [let us know if
+anything isn't working for you](https://github.com/small-hack/homebrew-tap/
+issues). ```bash # tap the special homebrew repo for our formula and install it
+brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
+the version and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
```

### Comparing `smol_k8s_lab-5.0.4/pyproject.toml` & `smol_k8s_lab-5.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name          = "smol_k8s_lab"
-version       = "5.0.4"
+version       = "5.1.0"
 description   = "CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD"
 authors       = ["Jesse Hitch <jessebot@linux.com>",
                  "Max Roby <emax@cloudydev.net>"]
 readme        = "README.md"
 packages      = [{include = "smol_k8s_lab"}]
 license       = "AGPL-3.0-or-later"
 homepage      = "https://small-hack.github.io/smol-k8s-lab"
@@ -35,19 +35,19 @@
 cryptography       = "^42.0"
 kubernetes         = "^29"
 minio              = "^7.2"
 pyfiglet           = "^1.0"
 pyjwt              = "^2.8"
 python             = ">=3.11,<3.13"
 pyyaml             = "^6.0"
-requests           = "^2.28"
+requests           = "^2.32"
 rich               = "^13.0"
 ruamel-yaml        = "^0.18"
 ruamel-yaml-string = "^0.1"
-textual            = "^0.61"
+textual            = "^0.62"
 xdg-base-dirs      = "^6.0"
 pygame             = "^2.5.2"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/__init__.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/audio/audio-en.tar.gz` & `smol_k8s_lab-5.1.0/smol_k8s_lab/audio/audio-en.tar.gz`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/bw_cli.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/bw_cli.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden.css` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden.css`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_app.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_credentials_modal_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/bitwarden/tui/bitwarden_existing_item_app.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/config/audio/en.yml` & `smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/en.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/config/audio/nl.yml` & `smol_k8s_lab-5.1.0/smol_k8s_lab/config/audio/nl.yml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/config/default_config.yaml` & `smol_k8s_lab-5.1.0/smol_k8s_lab/config/default_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -8,30 +8,30 @@
     enabled: true
     # show bottom footer help bar
     show_footer: true
     # accessibility options for users that benefit from TTS and Bell sounds
     accessibility:
       bell:
         # ring the built in terminal bell on focus to new elements on the screen
-        on_focus: true
+        on_focus: false
         # ring the built in terminal bell when something is wrong
-        on_error: true
+        on_error: false
       text_to_speech:
         # currently only english (en) and nederlands (nl) are available, but if you know
         # other languages, please help us translate (open an issue or discussion
         # on github 💙)
         language: "en"
         # use a specific cli program for text to speech - needs to be a full path
         # if it isn't in your default path. default is "" which means we'll use
         # pre-recorded audio files
         speech_program: ""
         # read aloud the screen title
         screen_titles: true
         # read aloud the screen description
-        screen_descriptions: true
+        screen_descriptions: false
         # read aloud the element id, value, and tooltip each time you switch focus
         on_focus: false
         # press f5 to read the element id and selected row of DataTables
         on_key_press: true
 
   run_command:
     # command to run after smol-k8s-lab is completed
```

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/config/keycloak_config.json` & `smol_k8s_lab-5.1.0/smol_k8s_lab/config/keycloak_config.json`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/config/smol-k8s-lab.appdata.xml` & `smol_k8s_lab-5.1.0/smol_k8s_lab/config/smol-k8s-lab.appdata.xml`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/constants.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/constants.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/env_config.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/env_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/__init__.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/argocd.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/argocd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/keycloak.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/vouch.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/vouch.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/identity_provider/zitadel_api.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/ingress/cert_manager.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/cert_manager.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/ingress/ingress_nginx_controller.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/initial_special.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/initial_special.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/cilium.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/cilium.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/metallb.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/metallb.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/networking/netmaker.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/networking/netmaker.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/__init__.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/minio.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/minio.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/postgres_operators.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/postgres_operators.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/operators/seaweedfs.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/operators/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/external_secrets_operator.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/infisical.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/infisical.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/secrets_management/vault.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/secrets_management/vault.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/home_assistant.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/home_assistant.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/mastodon.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/mastodon_rake.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/mastodon_rake.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/matrix.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/matrix.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/nextcloud.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_apps/social/nextcloud_occ_commands.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/__init__.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/k3d.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3d.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/k3s.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/k3s.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_distros/kind.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_distros/kind.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/argocd_util.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/argocd_util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/backup.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/backup.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/helm.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/helm.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/k8s_lib.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/k8s_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/k8s_tools/restores.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/k8s_tools/restores.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/__init__.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/app_inputs_confg.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/argocd_widgets.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/argocd_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/backup_and_restore.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/input_widgets.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/input_widgets.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/invalid_apps.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/invalid_apps.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/modify_globals.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/modify_globals.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/app_widgets/new_app_modal.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/app_widgets/new_app_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/apps_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/apps_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/audio_widget.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/audio_widget.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/cluster_modal.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/cluster_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/base_widgets/new_cluster_input.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/base_widgets/new_cluster_input.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/confirm_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/confirm_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/add_nodes_widget.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/add_nodes_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/apps_config.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/apps_init_config.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/apps_init_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/base.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/base_modal.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/base_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/cluster_modal.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/cluster_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/confirm.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/confirm.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/distro_config.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/distro_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/help.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/help.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/invalid_apps.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/invalid_apps.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/k3s.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/k3s.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/kind.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/kind.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/modify_globals_modal.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/modify_globals_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/new_app_modal.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/new_app_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/node_inputs_widget.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_inputs_widget.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/node_modal.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/node_modal.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/smol_k8s_cfg.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/css/tui_config.tcss` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/css/tui_config.tcss`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/add_nodes.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/add_nodes.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/k3s_config.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/k3s_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/kind_config.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kind_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/kubelet_config.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/kubelet_config.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/modify_node_modal.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/distro_widgets/node_adjustment.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/distro_widgets/node_adjustment.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/help_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/help_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/make_screenshots.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/make_screenshots.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/smol_k8s_config_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/smol_k8s_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/tui_config_screen.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/tui_config_screen.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/util.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/util.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/tui/validators/already_exists.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/tui/validators/already_exists.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/minio_lib.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/minio_lib.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/passwords.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/passwords.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/rich_cli/console_logging.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/console_logging.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/rich_cli/help_text.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/rich_cli/help_text.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/run/final_cmd.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/final_cmd.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/run/subproc.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/run/subproc.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/smol_k8s_lab/utils/value_from.py` & `smol_k8s_lab-5.1.0/smol_k8s_lab/utils/value_from.py`

 * *Files identical despite different names*

### Comparing `smol_k8s_lab-5.0.4/PKG-INFO` & `smol_k8s_lab-5.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smol_k8s_lab
-Version: 5.0.4
+Version: 5.1.0
 Summary: CLI and TUI to quickly install slimmer Kubernetes distros and then manage apps declaratively using Argo CD
 Home-page: https://small-hack.github.io/smol-k8s-lab
 License: AGPL-3.0-or-later
 Keywords: kubernetes,homelab,kind,k3s,k8s
 Author: Jesse Hitch
 Author-email: jessebot@linux.com
 Requires-Python: >=3.11,<3.13
@@ -22,19 +22,19 @@
 Requires-Dist: cryptography (>=42.0,<43.0)
 Requires-Dist: kubernetes (>=29,<30)
 Requires-Dist: minio (>=7.2,<8.0)
 Requires-Dist: pyfiglet (>=1.0,<2.0)
 Requires-Dist: pygame (>=2.5.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8,<3.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: requests (>=2.32,<3.0)
 Requires-Dist: rich (>=13.0,<14.0)
 Requires-Dist: ruamel-yaml (>=0.18,<0.19)
 Requires-Dist: ruamel-yaml-string (>=0.1,<0.2)
-Requires-Dist: textual (>=0.61,<0.62)
+Requires-Dist: textual (>=0.62,<0.63)
 Requires-Dist: xdg-base-dirs (>=6.0,<7.0)
 Project-URL: Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues
 Project-URL: Documentation, https://small-hack.github.io/smol-k8s-lab
 Project-URL: Repository, http://github.com/small-hack/smol-k8s-lab
 Description-Content-Type: text/markdown
 
 <h2 align="center">
@@ -63,15 +63,15 @@
 ### Features
 - Deploys [Argo CD](https://github.com/argoproj/argo-cd) by default, so you can manage your entire lab using files in [open source git repos](https://github.com/small-hack/argocd-apps)
   - Argo CD ships with a dashboard with a custom theme 💙
 - Supports multiple [k8s distros](#supported-k8s-distributions)
 - Specializes in using Bitwarden (though not required) to store sensitive values both locally and on your cluster
 - Manages all your authentication needs centrally using Zitadel and Vouch 💪
 - Supports initialization on a [range of common self-hosted apps](https://small-hack.github.io/smol-k8s-lab/k8s_apps/argocd/) 📱
-  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups
+  - featured initialized apps such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/k8s_apps/home_assistant/) include backups and restores
 - Lots o' [docs](https://small-hack.github.io/smol-k8s-lab)
 
 -----------------------------
 
 * [Installation](#installation)
     * [pipx](#pipx)
     * [brew (still unstable)](#brew-still-unstable)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.0.4 Summary: CLI and TUI to
+Metadata-Version: 2.1 Name: smol_k8s_lab Version: 5.1.0 Summary: CLI and TUI to
 quickly install slimmer Kubernetes distros and then manage apps declaratively
 using Argo CD Home-page: https://small-hack.github.io/smol-k8s-lab License:
 AGPL-3.0-or-later Keywords: kubernetes,homelab,kind,k3s,k8s Author: Jesse Hitch
 Author-email: jessebot@linux.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: End Users/
 Desktop Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 or later (AGPLv3+) Classifier: Operating System :: MacOS :: MacOS X
@@ -10,17 +10,17 @@
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: System ::
 Installation/Setup Requires-Dist: bcrypt (>=4.1,<5.0) Requires-Dist: click
 (>=8.1,<9.0) Requires-Dist: cryptography (>=42.0,<43.0) Requires-Dist:
 kubernetes (>=29,<30) Requires-Dist: minio (>=7.2,<8.0) Requires-Dist: pyfiglet
 (>=1.0,<2.0) Requires-Dist: pygame (>=2.5.2,<3.0.0) Requires-Dist: pyjwt
 (>=2.8,<3.0) Requires-Dist: pyyaml (>=6.0,<7.0) Requires-Dist: requests
-(>=2.28,<3.0) Requires-Dist: rich (>=13.0,<14.0) Requires-Dist: ruamel-yaml
+(>=2.32,<3.0) Requires-Dist: rich (>=13.0,<14.0) Requires-Dist: ruamel-yaml
 (>=0.18,<0.19) Requires-Dist: ruamel-yaml-string (>=0.1,<0.2) Requires-Dist:
-textual (>=0.61,<0.62) Requires-Dist: xdg-base-dirs (>=6.0,<7.0) Project-URL:
+textual (>=0.62,<0.63) Requires-Dist: xdg-base-dirs (>=6.0,<7.0) Project-URL:
 Bug Tracker, http://github.com/small-hack/smol-k8s-lab/issues Project-URL:
 Documentation, https://small-hack.github.io/smol-k8s-lab Project-URL:
 Repository, http://github.com/small-hack/smol-k8s-lab Description-Content-Type:
 text/markdown
   ********** [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ccaattppppuucccciinn//ccaattppppuucccciinn//mmaaiinn//aasssseettss//
 mmiisscc//ttrraannssppaarreenntt..ppnngg]]?ð??§?¸ ssmmooll--kk88ss--llaabb_[[_hh_tt_tt_pp_ss_::_//_//_ii_mm_gg_.._ss_hh_ii_ee_ll_dd_ss_.._ii_oo_//_gg_ii_tt_hh_uu_bb_//_vv_//_rr_ee_ll_ee_aa_ss_ee_//
                              _ss_mm_aa_ll_ll_--_hh_aa_cc_kk_//_ss_mm_oo_ll_--_kk_88_ss_--
@@ -41,35 +41,35 @@
 required) to store sensitive values both locally and on your cluster - Manages
 all your authentication needs centrally using Zitadel and Vouch ðª - Supports
 initialization on a [range of common self-hosted apps](https://small-
 hack.github.io/smol-k8s-lab/k8s_apps/argocd/) ð± - featured initialized apps
 such as [Nextcloud](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
 nextcloud/), [Matrix](https://small-hack.github.io/smol-k8s-lab/k8s_apps/
 matrix/), and [Home Assistant](https://small-hack.github.io/smol-k8s-lab/
-k8s_apps/home_assistant/) include backups - Lots o' [docs](https://small-
-hack.github.io/smol-k8s-lab) ----------------------------- * [Installation]
-(#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-still-unstable)
-* [Usage](#usage) * [Initialization](#initialization) * [Under the hood]
-(#under-the-hood) * [Supported k8s distributions](#supported-k8s-distributions)
-* [Default Installed Applications](#default-installed-applications) * [Status]
-(#status) # Installation B sure to check out our full [installation guide]
-(https://small-hack.github.io/smol-k8s-lab/installation/), but the gist of it
-is `smol-k8s-lab` can be installed via `pipx` (or `brew` coming soon). ## pipx
-`smol-k8s-lab` requires Python 3.11+ (and [pipx](https://github.com/pypa/
-pipx)). If you've already got both and [other pre-reqs](https://small-
-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be able
-to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help menu
-before proceeding smol-k8s-lab --help ``` ## brew (still unstable) [`brew`] is
-the future preferred installation method for macOS/Debian/Ubuntu, as this will
-also install any non-python prerequisites you need, so you don't need to worry
-about them. This method is new, so please [let us know if anything isn't
-working for you](https://github.com/small-hack/homebrew-tap/issues). ```bash #
-tap the special homebrew repo for our formula and install it brew install
-small-hack/tap/smol-k8s-lab ``` Then you should be able to check the version
-and cli options with: ```bash smol-k8s-lab --help ```
+k8s_apps/home_assistant/) include backups and restores - Lots o' [docs](https:/
+/small-hack.github.io/smol-k8s-lab) ----------------------------- *
+[Installation](#installation) * [pipx](#pipx) * [brew (still unstable)](#brew-
+still-unstable) * [Usage](#usage) * [Initialization](#initialization) * [Under
+the hood](#under-the-hood) * [Supported k8s distributions](#supported-k8s-
+distributions) * [Default Installed Applications](#default-installed-
+applications) * [Status](#status) # Installation B sure to check out our full
+[installation guide](https://small-hack.github.io/smol-k8s-lab/installation/),
+but the gist of it is `smol-k8s-lab` can be installed via `pipx` (or `brew`
+coming soon). ## pipx `smol-k8s-lab` requires Python 3.11+ (and [pipx](https://
+github.com/pypa/pipx)). If you've already got both and [other pre-reqs](https:/
+/small-hack.github.io/smol-k8s-lab/installation/#prerequisites), you should be
+able to: ```bash # install the CLI pipx install smol-k8s-lab # Check the help
+menu before proceeding smol-k8s-lab --help ``` ## brew (still unstable)
+[`brew`] is the future preferred installation method for macOS/Debian/Ubuntu,
+as this will also install any non-python prerequisites you need, so you don't
+need to worry about them. This method is new, so please [let us know if
+anything isn't working for you](https://github.com/small-hack/homebrew-tap/
+issues). ```bash # tap the special homebrew repo for our formula and install it
+brew install small-hack/tap/smol-k8s-lab ``` Then you should be able to check
+the version and cli options with: ```bash smol-k8s-lab --help ```
  _[_O_u_t_p_u_t_ _o_f_ _s_m_o_l_-_k_8_s_-_l_a_b_ _-_-_h_e_l_p_ _a_f_t_e_r_ _c_l_o_n_i_n_g_ _t_h_e_ _d_i_r_e_c_t_o_r_y_ _a_n_d_ _i_n_s_t_a_l_l_i_n_g_ _t_h_e
                                 _p_r_e_r_e_q_u_i_s_i_t_e_s_._]
 Checkout our [TUI docs](https://small-hack.github.io/smol-k8s-lab/tui/
 create_modify_screens/) for more info on how to get started playing with `smol-
 k8s-lab` :-) ## Usage ### Initialization After you've followed the installation
 instructions, if you're *new* to `smol-k8s-lab`, initialize a new config file:
 ```bash # we'll walk you through any configuration needed before # saving the
```

