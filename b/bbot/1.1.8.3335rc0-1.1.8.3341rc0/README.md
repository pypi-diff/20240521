# Comparing `tmp/bbot-1.1.8.3335rc0.tar.gz` & `tmp/bbot-1.1.8.3341rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.8.3335rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.8.3341rc0.tar", max compression
```

## Comparing `bbot-1.1.8.3335rc0.tar` & `bbot-1.1.8.3341rc0.tar`

### file list

```diff
@@ -1,346 +1,346 @@
--rw-r--r--   0        0        0    32473 2024-05-16 22:57:04.311059 bbot-1.1.8.3335rc0/LICENSE
--rw-r--r--   0        0        0    40272 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/README.md
--rw-r--r--   0        0        0      211 2024-05-16 22:57:18.543117 bbot-1.1.8.3335rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7898 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    17601 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/cli.py
--rw-r--r--   0        0        0       59 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3588 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9843 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5182 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1341 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      617 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/errors.py
--rw-r--r--   0        0        0       91 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    46323 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1656 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1232 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       86 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3583 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     1537 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     4341 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/cloud.py
--rw-r--r--   0        0        0    11950 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14117 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9199 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    47786 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     5639 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     6354 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0    12632 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    82906 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    22071 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0    10041 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1990 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     3463 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     5947 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     8781 2024-05-16 22:57:04.315059 bbot-1.1.8.3335rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    31838 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    19801 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0      191 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8118 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     4158 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     2328 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/ajaxpro.py
--rw-r--r--   0        0        0     1824 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1372 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     4691 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     4150 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/baddns.py
--rw-r--r--   0        0        0     1245 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/baddns_zone.py
--rw-r--r--   0        0        0     3549 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    59062 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2352 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1299 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0      655 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_amazon.py
--rw-r--r--   0        0        0     1020 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      775 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1915 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_file_enum.py
--rw-r--r--   0        0        0     1352 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2540 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bucket_google.py
--rw-r--r--   0        0        0     4911 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     6553 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1188 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3371 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      798 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     1522 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/chaos.py
--rw-r--r--   0        0        0     1810 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/code_repository.py
--rw-r--r--   0        0        0      735 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     3297 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/credshed.py
--rw-r--r--   0        0        0      376 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1230 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0     5316 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/deadly/dastardly.py
--rw-r--r--   0        0        0    14079 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    17260 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5239 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     3928 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/dehashed.py
--rw-r--r--   0        0        0      930 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     5324 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     3186 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     8781 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/docker_pull.py
--rw-r--r--   0        0        0     3271 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/dockerhub.py
--rw-r--r--   0        0        0     9245 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/dotnetnuke.py
--rw-r--r--   0        0        0      791 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11758 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     7540 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/filedownload.py
--rw-r--r--   0        0        0     2184 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1195 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7794 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1329 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2073 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/git_clone.py
--rw-r--r--   0        0        0     3147 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/github_codesearch.py
--rw-r--r--   0        0        0     8735 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/github_org.py
--rw-r--r--   0        0        0     6070 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/github_workflows.py
--rw-r--r--   0        0        0     5655 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/gitlab.py
--rw-r--r--   0        0        0    12223 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      890 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7172 2024-05-16 22:57:04.319059 bbot-1.1.8.3335rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     6758 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5990 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2098 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0    13124 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    18695 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     8286 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     4384 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/internetdb.py
--rw-r--r--   0        0        0     2123 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/ip2location.py
--rw-r--r--   0        0        0     1539 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     1767 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1541 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10816 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    21031 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      857 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     2281 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/newsletters.py
--rw-r--r--   0        0        0     5506 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4731 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5852 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      774 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    14731 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     3215 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2604 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0      531 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/discord.py
--rw-r--r--   0        0        0      985 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/emails.py
--rw-r--r--   0        0        0     2182 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1907 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1375 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     2746 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1117 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/slack.py
--rw-r--r--   0        0        0     1886 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/splunk.py
--rw-r--r--   0        0        0     1430 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0      723 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/teams.py
--rw-r--r--   0        0        0     3627 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2218 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1689 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9552 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1619 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1420 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0     5479 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/postman.py
--rw-r--r--   0        0        0      832 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8456 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      828 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2025 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2898 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1201 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0      792 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1993 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/sitedossier.py
--rw-r--r--   0        0        0     1478 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1408 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     2000 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7822 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     1327 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      553 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    17041 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0     5744 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/bucket.py
--rw-r--r--   0        0        0     1308 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/github.py
--rw-r--r--   0        0        0     2436 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/portscanner.py
--rw-r--r--   0        0        0     1182 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/shodan.py
--rw-r--r--   0        0        0     6100 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/subdomain_enum.py
--rw-r--r--   0        0        0     3789 2024-05-16 22:57:04.323059 bbot-1.1.8.3335rc0/bbot/modules/templates/webhook.py
--rw-r--r--   0        0        0      678 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4527 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/trufflehog.py
--rw-r--r--   0        0        0     4102 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2992 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2325 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1591 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     2010 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1272 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2871 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2336 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    29339 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    42299 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     2702 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0    11540 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     5889 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    12010 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     4870 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0       31 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/coverage.cfg
--rwxr-xr-x   0        0        0      652 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1091 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_output.ndjson
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5523 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6544 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0     3808 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     6384 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     7572 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    23553 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    31826 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0    16305 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_manager_deduplication.py
--rw-r--r--   0        0        0    79706 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
--rw-r--r--   0        0        0    16943 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     2657 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     7144 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2870 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2175 2024-05-16 22:57:04.327059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    13141 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     5344 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      664 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      473 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0     2789 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
--rw-r--r--   0        0        0      546 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     3098 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     4805 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     2795 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
--rw-r--r--   0        0        0     2397 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
--rw-r--r--   0        0        0     5599 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3984 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
--rw-r--r--   0        0        0      552 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      907 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0     2282 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
--rw-r--r--   0        0        0      506 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1312 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
--rw-r--r--   0        0        0     5051 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      956 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
--rw-r--r--   0        0        0     2047 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
--rw-r--r--   0        0        0      564 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0     3362 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
--rw-r--r--   0        0        0      762 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     2321 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
--rw-r--r--   0        0        0     3615 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
--rw-r--r--   0        0        0     1613 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0     1863 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
--rw-r--r--   0        0        0      952 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0    27988 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
--rw-r--r--   0        0        0     3907 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
--rw-r--r--   0        0        0     8232 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
--rw-r--r--   0        0        0      461 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0      944 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
--rw-r--r--   0        0        0    14708 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     2955 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0     2389 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
--rw-r--r--   0        0        0      445 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0    12266 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
--rw-r--r--   0        0        0     3718 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
--rw-r--r--   0        0        0    24606 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
--rw-r--r--   0        0        0    35521 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
--rw-r--r--   0        0        0    11579 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
--rw-r--r--   0        0        0     3433 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0     2155 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     4939 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2879 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     2231 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
--rw-r--r--   0        0        0     1123 2024-05-16 22:57:04.331059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
--rw-r--r--   0        0        0      604 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2767 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0     1006 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0     1641 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1711 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      428 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0     1030 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0     2305 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
--rw-r--r--   0        0        0     3618 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     5609 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9402 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0    14768 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
--rw-r--r--   0        0        0      184 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      537 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      713 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     6220 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
--rw-r--r--   0        0        0     2321 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0      415 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
--rw-r--r--   0        0        0     2426 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0     1700 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     3121 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0     1866 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
--rw-r--r--   0        0        0      706 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0      610 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     1222 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
--rw-r--r--   0        0        0     7751 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0    62527 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
--rw-r--r--   0        0        0     1144 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0     1304 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2026 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1979 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1103 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     1704 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2024-05-16 22:57:04.335059 bbot-1.1.8.3335rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0      764 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/ms_on_prem_subdomains.txt
--rw-r--r--   0        0        0    32226 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2024-05-16 22:57:04.343059 bbot-1.1.8.3335rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     2663 2024-05-16 22:57:18.543117 bbot-1.1.8.3335rc0/pyproject.toml
--rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.8.3335rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/LICENSE
+-rw-r--r--   0        0        0    40272 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/README.md
+-rw-r--r--   0        0        0      211 2024-05-21 17:36:45.116629 bbot-1.1.8.3341rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7898 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    17601 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/cli.py
+-rw-r--r--   0        0        0       59 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3588 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9843 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5182 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1341 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0       91 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    46323 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1656 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1232 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       86 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     1537 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     4341 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/cloud.py
+-rw-r--r--   0        0        0    11950 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9199 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    47786 2024-05-21 17:36:22.288488 bbot-1.1.8.3341rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     5639 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     6354 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0    12632 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    82906 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    22071 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0    10041 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1990 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     3463 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     5947 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     8781 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    31838 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    19801 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0      191 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8118 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     4158 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     2413 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/ajaxpro.py
+-rw-r--r--   0        0        0     1915 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1463 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     4782 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     4235 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/baddns.py
+-rw-r--r--   0        0        0     1330 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/baddns_zone.py
+-rw-r--r--   0        0        0     3634 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    59062 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2446 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1398 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0      746 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_amazon.py
+-rw-r--r--   0        0        0     1111 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      866 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1992 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_file_enum.py
+-rw-r--r--   0        0        0     1443 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2631 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bucket_google.py
+-rw-r--r--   0        0        0     5010 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     6607 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1287 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3470 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      889 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     1621 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/chaos.py
+-rw-r--r--   0        0        0     1901 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/code_repository.py
+-rw-r--r--   0        0        0      826 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     3366 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/credshed.py
+-rw-r--r--   0        0        0      428 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1321 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0     5407 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/deadly/dastardly.py
+-rw-r--r--   0        0        0    14132 2024-05-21 17:36:22.292488 bbot-1.1.8.3341rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    17351 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5293 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     4020 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/dehashed.py
+-rw-r--r--   0        0        0     1021 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     5384 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     3277 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     8872 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/docker_pull.py
+-rw-r--r--   0        0        0     3362 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/dockerhub.py
+-rw-r--r--   0        0        0     9330 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/dotnetnuke.py
+-rw-r--r--   0        0        0      882 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11843 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     7631 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/filedownload.py
+-rw-r--r--   0        0        0     2275 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1294 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7848 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1420 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2164 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/git_clone.py
+-rw-r--r--   0        0        0     3246 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/github_codesearch.py
+-rw-r--r--   0        0        0     8826 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/github_org.py
+-rw-r--r--   0        0        0     6161 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/github_workflows.py
+-rw-r--r--   0        0        0     5746 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/gitlab.py
+-rw-r--r--   0        0        0    12283 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      981 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7257 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     6849 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     6075 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2197 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0    13208 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      395 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    18780 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     8371 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     4475 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/internetdb.py
+-rw-r--r--   0        0        0     2222 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/ip2location.py
+-rw-r--r--   0        0        0     1630 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     1862 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1632 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10907 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    21122 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      948 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     2367 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/newsletters.py
+-rw-r--r--   0        0        0     5597 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4816 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5943 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      865 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    14816 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     3215 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2664 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0      622 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/discord.py
+-rw-r--r--   0        0        0     1076 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/emails.py
+-rw-r--r--   0        0        0     2273 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1967 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1466 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     2806 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      270 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1208 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/slack.py
+-rw-r--r--   0        0        0     1966 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/splunk.py
+-rw-r--r--   0        0        0     1521 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0      814 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/teams.py
+-rw-r--r--   0        0        0     3712 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2278 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1759 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1766 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9636 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1718 2024-05-21 17:36:22.296488 bbot-1.1.8.3341rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1511 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0     5570 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/postman.py
+-rw-r--r--   0        0        0      923 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1693 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8547 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      919 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2079 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2989 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1300 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0      891 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     2084 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1569 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1462 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     2091 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7898 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     1418 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      625 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    17126 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0     5744 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/bucket.py
+-rw-r--r--   0        0        0     1308 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/github.py
+-rw-r--r--   0        0        0     2436 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/portscanner.py
+-rw-r--r--   0        0        0     1182 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/shodan.py
+-rw-r--r--   0        0        0     6100 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/subdomain_enum.py
+-rw-r--r--   0        0        0     3789 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/templates/webhook.py
+-rw-r--r--   0        0        0      754 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4618 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/trufflehog.py
+-rw-r--r--   0        0        0     4187 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     3068 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2401 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1690 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     2095 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1342 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2940 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2435 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    29339 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    42299 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     2702 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0    11540 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     5889 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    12010 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     4870 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0       31 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/coverage.cfg
+-rwxr-xr-x   0        0        0      652 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1091 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_output.ndjson
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5523 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6544 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0     3808 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     6384 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     7572 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    23553 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2024-05-21 17:36:22.300488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    31826 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0    16305 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_manager_deduplication.py
+-rw-r--r--   0        0        0    79706 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
+-rw-r--r--   0        0        0    16943 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     2657 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7144 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2870 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2175 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    13141 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     5344 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      664 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      473 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0     2789 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
+-rw-r--r--   0        0        0      546 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     3098 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     4805 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     2795 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
+-rw-r--r--   0        0        0     2397 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
+-rw-r--r--   0        0        0     5599 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3984 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
+-rw-r--r--   0        0        0      552 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      907 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0     2282 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
+-rw-r--r--   0        0        0      506 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1312 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
+-rw-r--r--   0        0        0     5051 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      956 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
+-rw-r--r--   0        0        0     2047 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
+-rw-r--r--   0        0        0      564 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0     3362 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
+-rw-r--r--   0        0        0      762 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     2321 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
+-rw-r--r--   0        0        0     3615 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
+-rw-r--r--   0        0        0     1613 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0     1863 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
+-rw-r--r--   0        0        0      952 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0    27988 2024-05-21 17:36:22.304488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
+-rw-r--r--   0        0        0     3907 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
+-rw-r--r--   0        0        0     8232 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
+-rw-r--r--   0        0        0      461 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0      944 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
+-rw-r--r--   0        0        0    14708 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     2955 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0     2389 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
+-rw-r--r--   0        0        0      445 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0    12266 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
+-rw-r--r--   0        0        0     3718 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
+-rw-r--r--   0        0        0    24606 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
+-rw-r--r--   0        0        0    35521 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
+-rw-r--r--   0        0        0    11579 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
+-rw-r--r--   0        0        0     3433 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0     2155 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     4939 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2879 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     2231 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
+-rw-r--r--   0        0        0     1123 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
+-rw-r--r--   0        0        0      604 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2767 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0     1006 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0     1641 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1711 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      428 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0     1030 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0     2305 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
+-rw-r--r--   0        0        0     3618 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     5609 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9402 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0    14768 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
+-rw-r--r--   0        0        0      184 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      537 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      713 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0      415 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
+-rw-r--r--   0        0        0     2426 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0     1700 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     3121 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0     1866 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
+-rw-r--r--   0        0        0      706 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0      610 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     1222 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
+-rw-r--r--   0        0        0     7751 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0    62527 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
+-rw-r--r--   0        0        0     1144 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2024-05-21 17:36:22.308488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0     1304 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2026 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1979 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1103 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     1704 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2024-05-21 17:36:22.312488 bbot-1.1.8.3341rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0      764 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/ms_on_prem_subdomains.txt
+-rw-r--r--   0        0        0    32226 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2024-05-21 17:36:22.316488 bbot-1.1.8.3341rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     2663 2024-05-21 17:36:45.116629 bbot-1.1.8.3341rc0/pyproject.toml
+-rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.8.3341rc0/PKG-INFO
```

### Comparing `bbot-1.1.8.3335rc0/LICENSE` & `bbot-1.1.8.3341rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/README.md` & `bbot-1.1.8.3341rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/agent/agent.py` & `bbot-1.1.8.3341rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/cli.py` & `bbot-1.1.8.3341rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.8.3341rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/configurator/args.py` & `bbot-1.1.8.3341rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/configurator/environ.py` & `bbot-1.1.8.3341rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/configurator/files.py` & `bbot-1.1.8.3341rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/errors.py` & `bbot-1.1.8.3341rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/event/base.py` & `bbot-1.1.8.3341rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/event/helpers.py` & `bbot-1.1.8.3341rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/flags.py` & `bbot-1.1.8.3341rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/cache.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/cloud.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/command.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/diff.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/dns.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/files.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/helper.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/logger.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/misc.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/modules.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/url.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/validators.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/web.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.8.3341rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/core/logger/logger.py` & `bbot-1.1.8.3341rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/defaults.yml` & `bbot-1.1.8.3341rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ajaxpro.py` & `bbot-1.1.8.3341rc0/bbot/modules/ajaxpro.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
     Reference: https://mogwailabs.de/en/blog/2022/01/vulnerability-spotlight-rce-in-ajax.net-professional/
     """
 
     ajaxpro_regex = re.compile(r'<script.+src="([\/a-zA-Z0-9\._]+,[a-zA-Z0-9\._]+\.ashx)"')
     watched_events = ["HTTP_RESPONSE", "URL"]
     produced_events = ["VULNERABILITY", "FINDING"]
     flags = ["active", "safe", "web-thorough"]
-    meta = {"description": "Check for potentially vulnerable Ajaxpro instances"}
+    meta = {
+        "description": "Check for potentially vulnerable Ajaxpro instances",
+        "created_date": "2024-01-18",
+        "author": "@liquidsec",
+    }
 
     async def handle_event(self, event):
         if event.type == "URL":
             if "dir" not in event.tags:
                 return False
             for stem in ["ajax", "ajaxpro"]:
                 probe_url = f"{event.data}{stem}/whatever.ashx"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/anubisdb.py` & `bbot-1.1.8.3341rc0/bbot/modules/anubisdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class anubisdb(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query jldc.me's database for subdomains"}
+    meta = {
+        "description": "Query jldc.me's database for subdomains",
+        "created_date": "2022-10-04",
+        "author": "@TheTechromancer",
+    }
     options = {"limit": 1000}
     options_desc = {
         "limit": "Limit the number of subdomains returned per query (increasing this may slow the scan due to garbage results from this API)"
     }
 
     base_url = "https://jldc.me/anubis/subdomains"
     dns_abort_depth = 5
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/azure_realm.py` & `bbot-1.1.8.3341rc0/bbot/modules/azure_realm.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from .base import BaseModule
 
 
 class azure_realm(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["affiliates", "subdomain-enum", "cloud-enum", "web-basic", "web-thorough", "passive", "safe"]
-    meta = {"description": 'Retrieves the "AuthURL" from login.microsoftonline.com/getuserrealm'}
+    meta = {
+        "description": 'Retrieves the "AuthURL" from login.microsoftonline.com/getuserrealm',
+        "created_date": "2023-07-12",
+        "author": "@TheTechromancer",
+    }
 
     async def setup(self):
         self.processed = set()
         return True
 
     async def handle_event(self, event):
         _, domain = self.helpers.split_domain(event.data)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.8.3341rc0/bbot/modules/azure_tenant.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from bbot.modules.base import BaseModule
 
 
 class azure_tenant(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "cloud-enum", "passive", "safe"]
-    meta = {"description": "Query Azure for tenant sister domains"}
+    meta = {
+        "description": "Query Azure for tenant sister domains",
+        "created_date": "2024-07-04",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://autodiscover-s.outlook.com"
     in_scope_only = True
     per_domain_only = True
 
     async def setup(self):
         self.processed = set()
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/baddns.py` & `bbot-1.1.8.3341rc0/bbot/modules/baddns.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 include_logger(logging.getLogger("baddns"))
 
 
 class baddns(BaseModule):
     watched_events = ["DNS_NAME", "DNS_NAME_UNRESOLVED"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "safe", "web-basic", "baddns", "cloud-enum", "subdomain-hijack"]
-    meta = {"description": "Check hosts for domain/subdomain takeovers"}
+    meta = {
+        "description": "Check hosts for domain/subdomain takeovers",
+        "created_date": "2024-01-18",
+        "author": "@liquidsec",
+    }
     options = {"custom_nameservers": [], "only_high_confidence": False}
     options_desc = {
         "custom_nameservers": "Force BadDNS to use a list of custom nameservers",
         "only_high_confidence": "Do not emit low-confidence or generic detections",
     }
     max_event_handlers = 8
     deps_pip = ["baddns~=1.1.0"]
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/baddns_zone.py` & `bbot-1.1.8.3341rc0/bbot/modules/baddns_zone.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 include_logger(logging.getLogger("baddns_zone"))
 
 
 class baddns_zone(baddns_module):
     watched_events = ["DNS_NAME"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "safe", "subdomain-enum", "baddns", "cloud-enum"]
-    meta = {"description": "Check hosts for DNS zone transfers and NSEC walks"}
+    meta = {
+        "description": "Check hosts for DNS zone transfers and NSEC walks",
+        "created_date": "2024-01-29",
+        "author": "@liquidsec",
+    }
     options = {"custom_nameservers": [], "only_high_confidence": False}
     options_desc = {
         "custom_nameservers": "Force BadDNS to use a list of custom nameservers",
         "only_high_confidence": "Do not emit low-confidence or generic detections",
     }
     max_event_handlers = 8
     deps_pip = ["baddns~=1.1.0"]
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/badsecrets.py` & `bbot-1.1.8.3341rc0/bbot/modules/badsecrets.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from badsecrets.base import carve_all_modules
 
 
 class badsecrets(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING", "VULNERABILITY", "TECHNOLOGY"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Library for detecting known or weak secrets across many web frameworks"}
+    meta = {
+        "description": "Library for detecting known or weak secrets across many web frameworks",
+        "created_date": "2022-11-19",
+        "author": "@liquidsec",
+    }
     deps_pip = ["badsecrets~=0.4.490"]
 
     @property
     def _max_event_handlers(self):
         return max(1, multiprocessing.cpu_count() - 1)
 
     async def handle_event(self, event):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/base.py` & `bbot-1.1.8.3341rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bevigil.py` & `bbot-1.1.8.3341rc0/bbot/modules/bevigil.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,20 @@
     """
     Retrieve OSINT data from mobile applications using BeVigil
     """
 
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME", "URL_UNVERIFIED"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Retrieve OSINT data from mobile applications using BeVigil", "auth_required": True}
+    meta = {
+        "description": "Retrieve OSINT data from mobile applications using BeVigil",
+        "created_date": "2022-10-26",
+        "author": "@alt-glitch",
+        "auth_required": True,
+    }
     options = {"api_key": "", "urls": False}
     options_desc = {"api_key": "BeVigil OSINT API Key", "urls": "Emit URLs in addition to DNS_NAMEs"}
 
     base_url = "https://osint.bevigil.com/api"
 
     async def setup(self):
         self.api_key = self.config.get("api_key", "")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/binaryedge.py` & `bbot-1.1.8.3341rc0/bbot/modules/binaryedge.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class binaryedge(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the BinaryEdge API", "auth_required": True}
+    meta = {
+        "description": "Query the BinaryEdge API",
+        "created_date": "2024-08-18",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": "", "max_records": 1000}
     options_desc = {
         "api_key": "BinaryEdge API key",
         "max_records": "Limit results to help prevent exceeding API quota",
     }
 
     base_url = "https://api.binaryedge.io/v2"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.8.3341rc0/bbot/modules/bucket_azure.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.bucket import bucket_template
 
 
 class bucket_azure(bucket_template):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
-    meta = {"description": "Check for Azure storage blobs related to target"}
+    meta = {
+        "description": "Check for Azure storage blobs related to target",
+        "created_date": "2022-11-04",
+        "author": "@TheTechromancer",
+    }
     options = {"permutations": False}
     options_desc = {
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "azure"
     delimiters = ("", "-")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.8.3341rc0/bbot/modules/bucket_digitalocean.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.bucket import bucket_template
 
 
 class bucket_digitalocean(bucket_template):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "slow", "cloud-enum", "web-thorough"]
-    meta = {"description": "Check for DigitalOcean spaces related to target"}
+    meta = {
+        "description": "Check for DigitalOcean spaces related to target",
+        "created_date": "2022-11-08",
+        "author": "@TheTechromancer",
+    }
     options = {"permutations": False}
     options_desc = {
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "digitalocean"
     delimiters = ("", "-")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bucket_file_enum.py` & `bbot-1.1.8.3341rc0/bbot/modules/bucket_file_enum.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     """
     Enumerate files in a public bucket
     """
 
     watched_events = ["STORAGE_BUCKET"]
     produced_events = ["URL_UNVERIFIED"]
     meta = {
-        "description": "Works in conjunction with the filedownload module to download files from open storage buckets. Currently supported cloud providers: AWS"
+        "description": "Works in conjunction with the filedownload module to download files from open storage buckets. Currently supported cloud providers: AWS",
+        "created_date": "2023-11-14",
+        "author": "@TheTechromancer",
     }
     flags = ["passive", "safe", "cloud-enum"]
     options = {
         "file_limit": 50,
     }
     options_desc = {"file_limit": "Limit the number of files downloaded per bucket"}
     scope_distance_modifier = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.8.3341rc0/bbot/modules/bucket_firebase.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.bucket import bucket_template
 
 
 class bucket_firebase(bucket_template):
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
-    meta = {"description": "Check for open Firebase databases related to target"}
+    meta = {
+        "description": "Check for open Firebase databases related to target",
+        "created_date": "2023-03-20",
+        "author": "@TheTechromancer",
+    }
     options = {"permutations": False}
     options_desc = {
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "google"
     delimiters = ("", "-")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bucket_google.py` & `bbot-1.1.8.3341rc0/bbot/modules/bucket_google.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,19 @@
     """
     Adapted from https://github.com/RhinoSecurityLabs/GCPBucketBrute/blob/master/gcpbucketbrute.py
     """
 
     watched_events = ["DNS_NAME", "STORAGE_BUCKET"]
     produced_events = ["STORAGE_BUCKET", "FINDING"]
     flags = ["active", "safe", "cloud-enum", "web-basic", "web-thorough"]
-    meta = {"description": "Check for Google object storage related to target"}
+    meta = {
+        "description": "Check for Google object storage related to target",
+        "created_date": "2022-11-04",
+        "author": "@TheTechromancer",
+    }
     options = {"permutations": False}
     options_desc = {
         "permutations": "Whether to try permutations",
     }
 
     cloud_helper_name = "google"
     delimiters = ("", "-", ".", "_")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/builtwith.py` & `bbot-1.1.8.3341rc0/bbot/modules/builtwith.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class builtwith(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query Builtwith.com for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query Builtwith.com for subdomains",
+        "created_date": "2022-08-23",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": "", "redirects": True}
     options_desc = {"api_key": "Builtwith API key", "redirects": "Also look up inbound and outbound redirects"}
     base_url = "https://api.builtwith.com"
 
     async def ping(self):
         # builtwith does not have a ping feature, so we skip it to save API credits
         return
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/bypass403.py` & `bbot-1.1.8.3341rc0/bbot/modules/bypass403.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     signatures.append(("GET", "{scheme}://{netloc}/{path}", {hp_key: header_payloads[hp_key]}, False))
 
 
 class bypass403(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Check 403 pages for common bypasses"}
+    meta = {"description": "Check 403 pages for common bypasses", "created_date": "2022-07-05", "author": "@liquidsec"}
     in_scope_only = True
 
     async def do_checks(self, compare_helper, event, collapse_threshold):
         results = set()
         error_count = 0
 
         for sig in signatures:
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/c99.py` & `bbot-1.1.8.3341rc0/bbot/modules/c99.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class c99(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the C99 API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query the C99 API for subdomains",
+        "created_date": "2022-07-08",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "c99.nl API key"}
 
     base_url = "https://api.c99.nl"
 
     async def ping(self):
         url = f"{self.base_url}/randomnumber?key={self.api_key}&between=1,100&json"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/censys.py` & `bbot-1.1.8.3341rc0/bbot/modules/censys.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,20 @@
     """
     thanks to https://github.com/owasp-amass/amass/blob/master/resources/scripts/cert/censys.ads
     """
 
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the Censys API", "auth_required": True}
+    meta = {
+        "description": "Query the Censys API",
+        "created_date": "2022-08-04",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_id": "", "api_secret": "", "max_pages": 5}
     options_desc = {
         "api_id": "Censys.io API ID",
         "api_secret": "Censys.io API Secret",
         "max_pages": "Maximum number of pages to fetch (100 results per page)",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/certspotter.py` & `bbot-1.1.8.3341rc0/bbot/modules/certspotter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class certspotter(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query Certspotter's API for subdomains"}
+    meta = {
+        "description": "Query Certspotter's API for subdomains",
+        "created_date": "2022-07-28",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://api.certspotter.com/v1"
 
     def request_url(self, query):
         url = f"{self.base_url}/issuances?domain={self.helpers.quote(query)}&include_subdomains=true&expand=dns_names"
         return self.request_with_fail_count(url, timeout=self.http_timeout + 30)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/chaos.py` & `bbot-1.1.8.3341rc0/bbot/modules/chaos.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class chaos(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query ProjectDiscovery's Chaos API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query ProjectDiscovery's Chaos API for subdomains",
+        "created_date": "2022-08-14",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "Chaos API key"}
 
     base_url = "https://dns.projectdiscovery.io/dns"
 
     async def ping(self):
         url = f"{self.base_url}/example.com"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/code_repository.py` & `bbot-1.1.8.3341rc0/bbot/modules/code_repository.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import re
 from bbot.modules.base import BaseModule
 
 
 class code_repository(BaseModule):
     watched_events = ["URL_UNVERIFIED"]
     produced_events = ["CODE_REPOSITORY"]
-    meta = {"description": "Look for code repository links in webpages"}
+    meta = {
+        "description": "Look for code repository links in webpages",
+        "created_date": "2024-05-15",
+        "author": "@domwhewell-sage",
+    }
     flags = ["passive", "safe", "repo-enum"]
 
     # platform name : (regex, case_sensitive)
     code_repositories = {
         "git": [
             (r"github.com/[a-zA-Z0-9_-]+/[a-zA-Z0-9_-]+", False),
             (r"gitlab.(?:com|org)/[a-zA-Z0-9_-]+/[a-zA-Z0-9_-]+", False),
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/columbus.py` & `bbot-1.1.8.3341rc0/bbot/modules/digitorus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,31 @@
+import re
+
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
-class columbus(subdomain_enum):
+class digitorus(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query the Columbus Project API for subdomains"}
+    meta = {
+        "description": "Query certificatedetails.com for subdomains",
+        "created_date": "2023-07-25",
+        "author": "@TheTechromancer",
+    }
 
-    base_url = "https://columbus.elmasy.com/api/lookup"
+    base_url = "https://certificatedetails.com"
 
     async def request_url(self, query):
-        url = f"{self.base_url}/{self.helpers.quote(query)}?days=365"
-        return await self.request_with_fail_count(url)
+        url = f"{self.base_url}/{self.helpers.quote(query)}"
+        return await self.helpers.request(url)
 
     def parse_results(self, r, query):
         results = set()
-        json = r.json()
-        if json and isinstance(json, list):
-            return set([f"{s.lower()}.{query}" for s in json])
+        content = getattr(r, "text", "")
+        extract_regex = re.compile(r"[\w.-]+\." + query, re.I)
+        if content:
+            for match in extract_regex.finditer(content):
+                subdomain = match.group().lower()
+                if subdomain and subdomain.endswith(f".{query}"):
+                    results.add(subdomain)
         return results
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/credshed.py` & `bbot-1.1.8.3341rc0/bbot/modules/credshed.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class credshed(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["PASSWORD", "HASHED_PASSWORD", "USERNAME", "EMAIL_ADDRESS"]
     flags = ["passive", "safe"]
     meta = {
         "description": "Send queries to your own credshed server to check for known credentials of your targets",
+        "created_date": "2023-10-12",
+        "author": "@SpamFaux",
         "auth_required": True,
     }
     options = {"username": "", "password": "", "credshed_url": ""}
     options_desc = {
         "username": "Credshed username",
         "password": "Credshed password",
         "credshed_url": "URL of credshed server",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/crt.py` & `bbot-1.1.8.3341rc0/bbot/modules/crt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class crt(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query crt.sh (certificate transparency) for subdomains"}
+    meta = {
+        "description": "Query crt.sh (certificate transparency) for subdomains",
+        "created_date": "2022-05-13",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://crt.sh"
     reject_wildcards = False
 
     async def setup(self):
         self.cert_ids = set()
         return await super().setup()
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/deadly/dastardly.py` & `bbot-1.1.8.3341rc0/bbot/modules/deadly/dastardly.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.modules.base import BaseModule
 
 
 class dastardly(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["active", "aggressive", "slow", "web-thorough"]
-    meta = {"description": "Lightweight web application security scanner"}
+    meta = {
+        "description": "Lightweight web application security scanner",
+        "created_date": "2023-12-11",
+        "author": "@domwhewell-sage",
+    }
 
     deps_pip = ["lxml~=4.9.2"]
     deps_ansible = [
         {
             "name": "Check if Docker is already installed",
             "command": "docker --version",
             "register": "docker_installed",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.8.3341rc0/bbot/modules/deadly/ffuf.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import base64
 
 
 class ffuf(BaseModule):
     watched_events = ["URL"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["aggressive", "active"]
-    meta = {"description": "A fast web fuzzer written in Go"}
+    meta = {"description": "A fast web fuzzer written in Go", "created_date": "2022-04-10", "author": "@pmueller"}
 
     options = {
         "wordlist": "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Discovery/Web-Content/raft-small-directories.txt",
         "lines": 5000,
         "max_depth": 0,
         "version": "2.0.0",
         "extensions": "",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.8.3341rc0/bbot/modules/deadly/nuclei.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from bbot.modules.base import BaseModule
 
 
 class nuclei(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING", "VULNERABILITY", "TECHNOLOGY"]
     flags = ["active", "aggressive"]
-    meta = {"description": "Fast and customisable vulnerability scanner"}
+    meta = {
+        "description": "Fast and customisable vulnerability scanner",
+        "created_date": "2022-03-12",
+        "author": "@TheTechromancer",
+    }
 
     options = {
         "version": "3.2.0",
         "tags": "",
         "templates": "",
         "severity": "",
         "ratelimit": 150,
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.8.3341rc0/bbot/modules/deadly/vhost.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bbot.modules.deadly.ffuf import ffuf
 
 
 class vhost(ffuf):
     watched_events = ["URL"]
     produced_events = ["VHOST", "DNS_NAME"]
     flags = ["active", "aggressive", "slow"]
-    meta = {"description": "Fuzz for virtual hosts"}
+    meta = {"description": "Fuzz for virtual hosts", "created_date": "2022-05-02", "author": "@liquidsec"}
 
     special_vhost_list = ["127.0.0.1", "localhost", "host.docker.internal"]
     options = {
         "wordlist": "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Discovery/DNS/subdomains-top1million-5000.txt",
         "force_basehost": "",
         "lines": 5000,
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/dehashed.py` & `bbot-1.1.8.3341rc0/bbot/modules/dehashed.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from bbot.modules.base import BaseModule
 
 
 class dehashed(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["PASSWORD", "HASHED_PASSWORD", "USERNAME"]
     flags = ["passive", "safe", "email-enum"]
-    meta = {"description": "Execute queries against dehashed.com for exposed credentials", "auth_required": True}
+    meta = {
+        "description": "Execute queries against dehashed.com for exposed credentials",
+        "created_date": "2023-10-12",
+        "author": "@SpamFaux",
+        "auth_required": True,
+    }
     options = {"username": "", "api_key": ""}
     options_desc = {"username": "Email Address associated with your API key", "api_key": "DeHashed API Key"}
     target_only = True
 
     base_url = "https://api.dehashed.com/search"
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/digitorus.py` & `bbot-1.1.8.3341rc0/bbot/modules/subdomaincenter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,41 @@
-import re
-
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
-class digitorus(subdomain_enum):
+class subdomaincenter(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query certificatedetails.com for subdomains"}
-
-    base_url = "https://certificatedetails.com"
+    meta = {
+        "description": "Query subdomain.center's API for subdomains",
+        "created_date": "2023-07-26",
+        "author": "@TheTechromancer",
+    }
+
+    base_url = "https://api.subdomain.center"
+    retries = 2
+
+    async def sleep(self, time_to_wait):
+        self.info(f"Sleeping for {time_to_wait} seconds to avoid rate limit")
+        await self.helpers.sleep(time_to_wait)
 
     async def request_url(self, query):
-        url = f"{self.base_url}/{self.helpers.quote(query)}"
-        return await self.helpers.request(url)
+        url = f"{self.base_url}/?domain={self.helpers.quote(query)}"
+        response = None
+        status_code = 0
+        for i, _ in enumerate(range(self.retries + 1)):
+            if i > 0:
+                self.verbose(f"Retry #{i} for {query} after response code {status_code}")
+            response = await self.helpers.request(url, timeout=self.http_timeout + 30)
+            status_code = getattr(response, "status_code", 0)
+            if status_code == 429:
+                await self.sleep(20)
+            else:
+                break
+        return response
 
     def parse_results(self, r, query):
         results = set()
-        content = getattr(r, "text", "")
-        extract_regex = re.compile(r"[\w.-]+\." + query, re.I)
-        if content:
-            for match in extract_regex.finditer(content):
-                subdomain = match.group().lower()
-                if subdomain and subdomain.endswith(f".{query}"):
-                    results.add(subdomain)
+        json = r.json()
+        if json and isinstance(json, list):
+            results = set(json)
         return results
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.8.3341rc0/bbot/modules/dnscommonsrv.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 ]
 
 
 class dnscommonsrv(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Check for common SRV records"}
+    meta = {"description": "Check for common SRV records", "created_date": "2022-05-15", "author": "@TheTechromancer"}
     options = {"top": 50, "max_event_handlers": 10}
     options_desc = {
         "top": "How many of the top SRV records to check",
         "max_event_handlers": "How many instances of the module to run concurrently",
     }
     _max_event_handlers = 10
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.8.3341rc0/bbot/modules/dnsdumpster.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class dnsdumpster(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query dnsdumpster for subdomains"}
+    meta = {
+        "description": "Query dnsdumpster for subdomains",
+        "created_date": "2022-03-12",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://dnsdumpster.com"
 
     async def query(self, domain):
         ret = []
         # first, get the CSRF tokens
         res1 = await self.request_with_fail_count(self.base_url)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/docker_pull.py` & `bbot-1.1.8.3341rc0/bbot/modules/docker_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from bbot.modules.base import BaseModule
 
 
 class docker_pull(BaseModule):
     watched_events = ["CODE_REPOSITORY"]
     produced_events = ["FILESYSTEM"]
     flags = ["passive", "safe", "slow"]
-    meta = {"description": "Download images from a docker repository"}
+    meta = {
+        "description": "Download images from a docker repository",
+        "created_date": "2024-03-24",
+        "author": "@domwhewell-sage",
+    }
     options = {"all_tags": False, "output_folder": ""}
     options_desc = {
         "all_tags": "Download all tags from each registry (Default False)",
         "output_folder": "Folder to download docker repositories to",
     }
 
     scope_distance_modifier = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/dockerhub.py` & `bbot-1.1.8.3341rc0/bbot/modules/dockerhub.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.base import BaseModule
 
 
 class dockerhub(BaseModule):
     watched_events = ["SOCIAL", "ORG_STUB"]
     produced_events = ["SOCIAL", "CODE_REPOSITORY", "URL_UNVERIFIED"]
     flags = ["passive", "safe"]
-    meta = {"description": "Search for docker repositories of discovered orgs/usernames"}
+    meta = {
+        "description": "Search for docker repositories of discovered orgs/usernames",
+        "created_date": "2024-03-12",
+        "author": "@domwhewell-sage",
+    }
 
     site_url = "https://hub.docker.com"
     api_url = f"{site_url}/v2"
 
     scope_distance_modifier = 2
 
     async def filter_event(self, event):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/dotnetnuke.py` & `bbot-1.1.8.3341rc0/bbot/modules/dotnetnuke.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,19 @@
     exploit_probe = {
         "DNNPersonalization": r'<profile><item key="name1: key1" type="System.Data.Services.Internal.ExpandedWrapper`2[[DotNetNuke.Common.Utilities.FileSystemUtils],[System.Windows.Data.ObjectDataProvider, PresentationFramework, Version=4.0.0.0, Culture=neutral, PublicKeyToken=31bf3856ad364e35]], System.Data.Services, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089"><ExpandedWrapperOfFileSystemUtilsObjectDataProvider xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"><ExpandedElement/><ProjectedProperty0><MethodName>WriteFile</MethodName><MethodParameters><anyType xsi:type="xsd:string">C:\Windows\win.ini</anyType></MethodParameters><ObjectInstance xsi:type="FileSystemUtils"></ObjectInstance></ProjectedProperty0></ExpandedWrapperOfFileSystemUtilsObjectDataProvider></item></profile>'
     }
 
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["VULNERABILITY", "TECHNOLOGY"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Scan for critical DotNetNuke (DNN) vulnerabilities"}
+    meta = {
+        "description": "Scan for critical DotNetNuke (DNN) vulnerabilities",
+        "created_date": "2023-11-21",
+        "author": "@liquidsec",
+    }
 
     async def setup(self):
         self.event_dict = {}
         self.interactsh_subdomain_tags = {}
         self.interactsh_instance = None
 
         if self.scan.config.get("interactsh_disable", False) == False:
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/emailformat.py` & `bbot-1.1.8.3341rc0/bbot/modules/emailformat.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.base import BaseModule
 
 
 class emailformat(BaseModule):
     watched_events = ["DNS_NAME"]
     produced_events = ["EMAIL_ADDRESS"]
     flags = ["passive", "email-enum", "safe"]
-    meta = {"description": "Query email-format.com for email addresses"}
+    meta = {
+        "description": "Query email-format.com for email addresses",
+        "created_date": "2022-07-11",
+        "author": "@TheTechromancer",
+    }
     in_scope_only = False
     per_domain_only = True
 
     base_url = "https://www.email-format.com"
 
     async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.8.3341rc0/bbot/modules/ffuf_shortnames.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,19 @@
     return list(found_prefixes)
 
 
 class ffuf_shortnames(ffuf):
     watched_events = ["URL_HINT"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["aggressive", "active", "iis-shortnames", "web-thorough"]
-    meta = {"description": "Use ffuf in combination IIS shortnames"}
+    meta = {
+        "description": "Use ffuf in combination IIS shortnames",
+        "created_date": "2022-07-05",
+        "author": "@liquidsec",
+    }
 
     options = {
         "wordlist": "",  # default is defined within setup function
         "wordlist_extensions": "",  # default is defined within setup function
         "lines": 1000000,
         "max_depth": 1,
         "version": "2.0.0",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/filedownload.py` & `bbot-1.1.8.3341rc0/bbot/modules/filedownload.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,19 @@
     Capable of identifying interesting files even if the extension is not in the URL.
     E.g. if a PDF is being served at https://evilcorp.com/mypdf, it will still be downloaded and given the proper extension.
     """
 
     watched_events = ["URL_UNVERIFIED", "HTTP_RESPONSE"]
     produced_events = []
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Download common filetypes such as PDF, DOCX, PPTX, etc."}
+    meta = {
+        "description": "Download common filetypes such as PDF, DOCX, PPTX, etc.",
+        "created_date": "2023-10-11",
+        "author": "@TheTechromancer",
+    }
     options = {
         "extensions": [
             "bak",  #  Backup File
             "bash",  #  Bash Script or Configuration
             "bashrc",  #  Bash Script or Configuration
             "conf",  #  Configuration File
             "cfg",  #  Configuration File
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.8.3341rc0/bbot/modules/fingerprintx.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from bbot.modules.base import BaseModule
 
 
 class fingerprintx(BaseModule):
     watched_events = ["OPEN_TCP_PORT"]
     produced_events = ["PROTOCOL"]
     flags = ["active", "safe", "service-enum", "slow"]
-    meta = {"description": "Fingerprint exposed services like RDP, SSH, MySQL, etc."}
+    meta = {
+        "description": "Fingerprint exposed services like RDP, SSH, MySQL, etc.",
+        "created_date": "2023-01-30",
+        "author": "@TheTechromancer",
+    }
     options = {"version": "1.1.4"}
     options_desc = {"version": "fingerprintx version"}
     _batch_size = 10
     _max_event_handlers = 2
     _priority = 2
 
     deps_ansible = [
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/fullhunt.py` & `bbot-1.1.8.3341rc0/bbot/modules/fullhunt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class fullhunt(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the fullhunt.io API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query the fullhunt.io API for subdomains",
+        "created_date": "2022-08-24",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "FullHunt API Key"}
 
     base_url = "https://fullhunt.io/api/v1"
 
     async def setup(self):
         self.api_key = self.config.get("api_key", "")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.8.3341rc0/bbot/modules/generic_ssrf.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             self.process(event, r, subdomain_tag)
 
 
 class generic_ssrf(BaseModule):
     watched_events = ["URL"]
     produced_events = ["VULNERABILITY"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Check for generic SSRFs"}
+    meta = {"description": "Check for generic SSRFs", "created_date": "2022-07-30", "author": "@liquidsec"}
     in_scope_only = True
 
     deps_apt = ["curl"]
 
     async def setup(self):
         self.submodules = {}
         self.interactsh_subdomain_tags = {}
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/git.py` & `bbot-1.1.8.3341rc0/bbot/modules/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from bbot.modules.base import BaseModule
 
 
 class git(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Check for exposed .git repositories"}
+    meta = {
+        "description": "Check for exposed .git repositories",
+        "created_date": "2023-05-30",
+        "author": "@TheTechromancer",
+    }
 
     in_scope_only = True
 
     fp_regex = re.compile(r"<html|<body", re.I)
 
     async def handle_event(self, event):
         base_url = event.data.rstrip("/")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/git_clone.py` & `bbot-1.1.8.3341rc0/bbot/modules/git_clone.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.modules.templates.github import github
 
 
 class git_clone(github):
     watched_events = ["CODE_REPOSITORY"]
     produced_events = ["FILESYSTEM"]
     flags = ["passive", "safe", "slow"]
-    meta = {"description": "Clone code github repositories"}
+    meta = {
+        "description": "Clone code github repositories",
+        "created_date": "2024-03-08",
+        "author": "@domwhewell-sage",
+    }
     options = {"api_key": "", "output_folder": ""}
     options_desc = {"api_key": "Github token", "output_folder": "Folder to clone repositories to"}
 
     deps_apt = ["git"]
 
     scope_distance_modifier = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/github_codesearch.py` & `bbot-1.1.8.3341rc0/bbot/modules/github_codesearch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.github import github
 
 
 class github_codesearch(github):
     watched_events = ["DNS_NAME"]
     produced_events = ["CODE_REPOSITORY", "URL_UNVERIFIED"]
     flags = ["passive", "subdomain-enum", "safe"]
-    meta = {"description": "Query Github's API for code containing the target domain name", "auth_required": True}
+    meta = {
+        "description": "Query Github's API for code containing the target domain name",
+        "created_date": "2023-12-14",
+        "author": "@domwhewell-sage",
+        "auth_required": True,
+    }
     options = {"api_key": "", "limit": 100}
     options_desc = {"api_key": "Github token", "limit": "Limit code search to this many results"}
 
     github_raw_url = "https://raw.githubusercontent.com/"
 
     async def setup(self):
         self.limit = self.config.get("limit", 100)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/github_org.py` & `bbot-1.1.8.3341rc0/bbot/modules/github_org.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.github import github
 
 
 class github_org(github):
     watched_events = ["ORG_STUB", "SOCIAL"]
     produced_events = ["CODE_REPOSITORY"]
     flags = ["passive", "subdomain-enum", "safe"]
-    meta = {"description": "Query Github's API for organization and member repositories"}
+    meta = {
+        "description": "Query Github's API for organization and member repositories",
+        "created_date": "2023-12-14",
+        "author": "@domwhewell-sage",
+    }
     options = {"api_key": "", "include_members": True, "include_member_repos": False}
     options_desc = {
         "api_key": "Github token",
         "include_members": "Enumerate organization members",
         "include_member_repos": "Also enumerate organization members' repositories",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/github_workflows.py` & `bbot-1.1.8.3341rc0/bbot/modules/github_workflows.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from bbot.modules.templates.github import github
 
 
 class github_workflows(github):
     watched_events = ["CODE_REPOSITORY"]
     produced_events = ["FILESYSTEM"]
     flags = ["passive", "safe"]
-    meta = {"description": "Download a github repositories workflow logs"}
+    meta = {
+        "description": "Download a github repositories workflow logs",
+        "created_date": "2024-04-29",
+        "author": "@domwhewell-sage",
+    }
     options = {"api_key": "", "num_logs": 1}
     options_desc = {
         "api_key": "Github token",
         "num_logs": "For each workflow fetch the last N successful runs logs (max 100)",
     }
 
     scope_distance_modifier = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/gitlab.py` & `bbot-1.1.8.3341rc0/bbot/modules/gitlab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.base import BaseModule
 
 
 class gitlab(BaseModule):
     watched_events = ["HTTP_RESPONSE", "TECHNOLOGY", "SOCIAL"]
     produced_events = ["TECHNOLOGY", "SOCIAL", "CODE_REPOSITORY", "FINDING"]
     flags = ["active", "safe"]
-    meta = {"description": "Detect GitLab instances and query them for repositories"}
+    meta = {
+        "description": "Detect GitLab instances and query them for repositories",
+        "created_date": "2024-03-11",
+        "author": "@TheTechromancer",
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "Gitlab access token"}
 
     scope_distance_modifier = 2
 
     async def setup(self):
         self.headers = {}
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/gowitness.py` & `bbot-1.1.8.3341rc0/bbot/modules/gowitness.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bbot.modules.base import BaseModule
 
 
 class gowitness(BaseModule):
     watched_events = ["URL", "SOCIAL"]
     produced_events = ["WEBSCREENSHOT", "URL", "URL_UNVERIFIED", "TECHNOLOGY"]
     flags = ["active", "safe", "web-screenshots"]
-    meta = {"description": "Take screenshots of webpages"}
+    meta = {"description": "Take screenshots of webpages", "created_date": "2022-07-08", "author": "@TheTechromancer"}
     options = {
         "version": "2.4.2",
         "threads": 0,
         "timeout": 10,
         "resolution_x": 1440,
         "resolution_y": 900,
         "output_path": "",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/hackertarget.py` & `bbot-1.1.8.3341rc0/bbot/modules/otx.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
-class hackertarget(subdomain_enum):
+class otx(subdomain_enum):
+    flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the hackertarget.com API for subdomains"}
+    meta = {
+        "description": "Query otx.alienvault.com for subdomains",
+        "created_date": "2022-08-24",
+        "author": "@TheTechromancer",
+    }
 
-    base_url = "https://api.hackertarget.com"
+    base_url = "https://otx.alienvault.com"
 
-    async def request_url(self, query):
-        url = f"{self.base_url}/hostsearch/?q={self.helpers.quote(query)}"
-        response = await self.request_with_fail_count(url)
-        return response
+    def request_url(self, query):
+        url = f"{self.base_url}/api/v1/indicators/domain/{self.helpers.quote(query)}/passive_dns"
+        return self.request_with_fail_count(url)
 
     def parse_results(self, r, query):
-        for line in r.text.splitlines():
-            host = line.split(",")[0]
-            try:
-                self.helpers.validators.validate_host(host)
-                yield host
-            except ValueError:
-                self.debug(f"Error validating API result: {line}")
-                continue
+        j = r.json()
+        if isinstance(j, dict):
+            for entry in j.get("passive_dns", []):
+                subdomain = entry.get("hostname", "")
+                if subdomain:
+                    yield subdomain
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/host_header.py` & `bbot-1.1.8.3341rc0/bbot/modules/host_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.core.errors import InteractshError
 
 
 class host_header(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Try common HTTP Host header spoofing techniques"}
+    meta = {
+        "description": "Try common HTTP Host header spoofing techniques",
+        "created_date": "2022-07-27",
+        "author": "@liquidsec",
+    }
 
     in_scope_only = True
     per_hostport_only = True
 
     deps_apt = ["curl"]
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/httpx.py` & `bbot-1.1.8.3341rc0/bbot/modules/httpx.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,19 @@
 from bbot.core.helpers.web import is_login_page
 
 
 class httpx(BaseModule):
     watched_events = ["OPEN_TCP_PORT", "URL_UNVERIFIED", "URL"]
     produced_events = ["URL", "HTTP_RESPONSE"]
     flags = ["active", "safe", "web-basic", "web-thorough", "social-enum", "subdomain-enum", "cloud-enum"]
-    meta = {"description": "Visit webpages. Many other modules rely on httpx"}
+    meta = {
+        "description": "Visit webpages. Many other modules rely on httpx",
+        "created_date": "2022-07-08",
+        "author": "@TheTechromancer",
+    }
 
     options = {
         "threads": 50,
         "in_scope_only": True,
         "version": "1.2.5",
         "max_response_size": 5242880,
         "store_responses": False,
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/hunt.py` & `bbot-1.1.8.3341rc0/bbot/modules/hunt.py`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,19 @@
 }
 
 
 class hunt(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "safe", "web-thorough"]
-    meta = {"description": "Watch for commonly-exploitable HTTP parameters"}
+    meta = {
+        "description": "Watch for commonly-exploitable HTTP parameters",
+        "created_date": "2022-07-20",
+        "author": "@liquidsec",
+    }
     # accept all events regardless of scope distance
     scope_distance_modifier = None
 
     async def handle_event(self, event):
         body = event.data.get("body", "")
         for p in extract_params_html(body):
             for k in hunt_param_dict.keys():
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/hunterio.py` & `bbot-1.1.8.3341rc0/bbot/modules/hunterio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class hunterio(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["EMAIL_ADDRESS", "DNS_NAME", "URL_UNVERIFIED"]
     flags = ["passive", "email-enum", "subdomain-enum", "safe"]
-    meta = {"description": "Query hunter.io for emails", "auth_required": True}
+    meta = {
+        "description": "Query hunter.io for emails",
+        "created_date": "2022-04-25",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "Hunter.IO API key"}
 
     base_url = "https://api.hunter.io/v2"
     limit = 100
 
     async def ping(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.8.3341rc0/bbot/modules/iis_shortnames.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
     pass
 
 
 class iis_shortnames(BaseModule):
     watched_events = ["URL"]
     produced_events = ["URL_HINT"]
     flags = ["active", "safe", "web-basic", "web-thorough", "iis-shortnames"]
-    meta = {"description": "Check for IIS shortname vulnerability"}
+    meta = {
+        "description": "Check for IIS shortname vulnerability",
+        "created_date": "2022-04-15",
+        "author": "@pmueller",
+    }
     options = {"detect_only": True, "max_node_count": 50}
     options_desc = {
         "detect_only": "Only detect the vulnerability and do not run the shortname scanner",
         "max_node_count": "Limit how many nodes to attempt to resolve on any given recursion branch",
     }
     in_scope_only = True
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/internal/base.py` & `bbot-1.1.8.3341rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.8.3341rc0/bbot/modules/internal/excavate.py`

 * *Files 0% similar despite different names*

```diff
@@ -334,15 +334,19 @@
         )
 
 
 class excavate(BaseInternalModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["passive"]
-    meta = {"description": "Passively extract juicy tidbits from scan data"}
+    meta = {
+        "description": "Passively extract juicy tidbits from scan data",
+        "created_date": "2022-06-27",
+        "author": "@liquidsec",
+    }
 
     scope_distance_modifier = None
 
     async def setup(self):
         self.csp = CSPExtractor(self)
         self.hostname = HostnameExtractor(self)
         self.url = URLExtractor(self)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.8.3341rc0/bbot/modules/internal/speculate.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,19 @@
         "STORAGE_BUCKET",
         "SOCIAL",
         "AZURE_TENANT",
         "USERNAME",
     ]
     produced_events = ["DNS_NAME", "OPEN_TCP_PORT", "IP_ADDRESS", "FINDING", "ORG_STUB"]
     flags = ["passive"]
-    meta = {"description": "Derive certain event types from others by common sense"}
+    meta = {
+        "description": "Derive certain event types from others by common sense",
+        "created_date": "2022-05-03",
+        "author": "@liquidsec",
+    }
 
     options = {"max_hosts": 65536, "ports": "80,443"}
     options_desc = {
         "max_hosts": "Max number of IP_RANGE hosts to convert into IP_ADDRESS events",
         "ports": "The set of ports to speculate on",
     }
     scope_distance_modifier = 1
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/internetdb.py` & `bbot-1.1.8.3341rc0/bbot/modules/internetdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,19 @@
         ]
     }
     """
 
     watched_events = ["IP_ADDRESS", "DNS_NAME"]
     produced_events = ["TECHNOLOGY", "VULNERABILITY", "FINDING", "OPEN_TCP_PORT", "DNS_NAME"]
     flags = ["passive", "safe", "portscan", "subdomain-enum"]
-    meta = {"description": "Query Shodan's InternetDB for open ports, hostnames, technologies, and vulnerabilities"}
+    meta = {
+        "description": "Query Shodan's InternetDB for open ports, hostnames, technologies, and vulnerabilities",
+        "created_date": "2023-12-22",
+        "author": "@TheTechromancer",
+    }
 
     _qsize = 500
 
     base_url = "https://internetdb.shodan.io"
 
     async def setup(self):
         self.processed = set()
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ip2location.py` & `bbot-1.1.8.3341rc0/bbot/modules/ip2location.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,20 @@
     """
     IP2Location.io Geolocation API.
     """
 
     watched_events = ["IP_ADDRESS"]
     produced_events = ["GEOLOCATION"]
     flags = ["passive", "safe"]
-    meta = {"description": "Query IP2location.io's API for geolocation information. ", "auth_required": True}
+    meta = {
+        "description": "Query IP2location.io's API for geolocation information. ",
+        "created_date": "2023-09-12",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": "", "lang": ""}
     options_desc = {
         "api_key": "IP2location.io API Key",
         "lang": "Translation information(ISO639-1). The translation is only applicable for continent, country, region and city name.",
     }
     scope_distance_modifier = 1
     _priority = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.8.3341rc0/bbot/modules/ipneighbor.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from bbot.modules.base import BaseModule
 
 
 class ipneighbor(BaseModule):
     watched_events = ["IP_ADDRESS"]
     produced_events = ["IP_ADDRESS"]
     flags = ["passive", "subdomain-enum", "aggressive"]
-    meta = {"description": "Look beside IPs in their surrounding subnet"}
+    meta = {
+        "description": "Look beside IPs in their surrounding subnet",
+        "created_date": "2022-06-08",
+        "author": "@TheTechromancer",
+    }
     options = {"num_bits": 4}
     options_desc = {"num_bits": "Netmask size (in CIDR notation) to check. Default is 4 bits (16 hosts)"}
     scope_distance_modifier = 1
 
     async def setup(self):
         self.processed = set()
         self.num_bits = max(1, int(self.config.get("num_bits", 4)))
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ipstack.py` & `bbot-1.1.8.3341rc0/bbot/modules/ipstack.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,20 @@
     Ipstack GeoIP
     Leverages the ipstack.com API to geolocate a host by IP address.
     """
 
     watched_events = ["IP_ADDRESS"]
     produced_events = ["GEOLOCATION"]
     flags = ["passive", "safe"]
-    meta = {"description": "Query IPStack's GeoIP API", "auth_required": True}
+    meta = {
+        "description": "Query IPStack's GeoIP API",
+        "created_date": "2022-11-26",
+        "author": "@tycoonslive",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "IPStack GeoIP API Key"}
     scope_distance_modifier = 1
     _priority = 2
     suppress_dupes = False
 
     base_url = "http://api.ipstack.com"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/leakix.py` & `bbot-1.1.8.3341rc0/bbot/modules/leakix.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 class leakix(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
     options = {"api_key": ""}
     # NOTE: API key is not required (but having one will get you more results)
     options_desc = {"api_key": "LeakIX API Key"}
-    meta = {"description": "Query leakix.net for subdomains"}
+    meta = {
+        "description": "Query leakix.net for subdomains",
+        "created_date": "2022-07-11",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://leakix.net"
 
     async def setup(self):
         ret = await super(subdomain_enum_apikey, self).setup()
         self.headers = {"Accept": "application/json"}
         self.api_key = self.config.get("api_key", "")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/masscan.py` & `bbot-1.1.8.3341rc0/bbot/modules/masscan.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from bbot.modules.templates.portscanner import portscanner
 
 
 class masscan(portscanner):
     flags = ["active", "portscan", "aggressive"]
     watched_events = ["IP_ADDRESS", "IP_RANGE"]
     produced_events = ["OPEN_TCP_PORT"]
-    meta = {"description": "Port scan with masscan. By default, scans top 100 ports."}
+    meta = {
+        "description": "Port scan with masscan. By default, scans top 100 ports.",
+        "created_date": "2023-01-27",
+        "author": "@TheTechromancer",
+    }
     options = {
         "top_ports": 100,
         "ports": "",
         # ping scan at 600 packets/s ~= entire private IP space in 8 hours
         "rate": 600,
         "wait": 5,
         "ping_first": False,
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/massdns.py` & `bbot-1.1.8.3341rc0/bbot/modules/massdns.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,19 @@
     This is especially use for bug bounties because it enables you to recognize distant/rare subdomains at a glance.
     Subdomains with higher mutation levels are more likely to be distant/rare or never-before-seen.
     """
 
     flags = ["subdomain-enum", "passive", "aggressive"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Brute-force subdomains with massdns (highly effective)"}
+    meta = {
+        "description": "Brute-force subdomains with massdns (highly effective)",
+        "created_date": "2023-03-29",
+        "author": "@TheTechromancer",
+    }
     options = {
         "wordlist": "https://raw.githubusercontent.com/danielmiessler/SecLists/master/Discovery/DNS/subdomains-top1million-5000.txt",
         "max_resolvers": 1000,
         "max_mutations": 500,
         "max_depth": 5,
     }
     options_desc = {
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/myssl.py` & `bbot-1.1.8.3341rc0/bbot/modules/myssl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class myssl(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query myssl.com's API for subdomains"}
+    meta = {
+        "description": "Query myssl.com's API for subdomains",
+        "created_date": "2023-07-10",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://myssl.com/api/v1/discover_sub_domain"
 
     async def request_url(self, query):
         url = f"{self.base_url}?domain={self.helpers.quote(query)}"
         return await self.request_with_fail_count(url)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/newsletters.py` & `bbot-1.1.8.3341rc0/bbot/modules/newsletters.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 # https://geekout.mattnavarra.com/
 
 
 class newsletters(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "safe"]
-    meta = {"description": "Searches for Newsletter Submission Entry Fields on Websites"}
+    meta = {
+        "description": "Searches for Newsletter Submission Entry Fields on Websites",
+        "created_date": "2024-02-02",
+        "author": "@stryker2k2",
+    }
 
     # Parse through Website to find a Text Entry Box of 'type = email'
     # and ensure that there is placeholder text within it.
     def find_type(self, soup):
         email_type = soup.find(type="email")
         if email_type:
             regex = re.compile(r"placeholder")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/nmap.py` & `bbot-1.1.8.3341rc0/bbot/modules/nmap.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.modules.templates.portscanner import portscanner
 
 
 class nmap(portscanner):
     watched_events = ["IP_ADDRESS", "DNS_NAME", "IP_RANGE"]
     produced_events = ["OPEN_TCP_PORT"]
     flags = ["active", "portscan", "aggressive", "web-thorough"]
-    meta = {"description": "Port scan with nmap. By default, scans top 100 ports."}
+    meta = {
+        "description": "Port scan with nmap. By default, scans top 100 ports.",
+        "created_date": "2022-03-12",
+        "author": "@TheTechromancer",
+    }
     options = {
         "top_ports": 100,
         "ports": "",
         "timing": "T4",
         "skip_host_discovery": True,
     }
     options_desc = {
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/ntlm.py` & `bbot-1.1.8.3341rc0/bbot/modules/ntlm.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,19 @@
         Cancel pending requests and break out of loop when valid endpoint is found
         (waiting on https://github.com/encode/httpcore/discussions/783/ to be fixed first)
     """
 
     watched_events = ["URL", "HTTP_RESPONSE"]
     produced_events = ["FINDING", "DNS_NAME"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Watch for HTTP endpoints that support NTLM authentication"}
+    meta = {
+        "description": "Watch for HTTP endpoints that support NTLM authentication",
+        "created_date": "2022-07-25",
+        "author": "@liquidsec",
+    }
     options = {"try_all": False}
     options_desc = {"try_all": "Try every NTLM endpoint"}
 
     in_scope_only = True
 
     async def setup(self):
         self.processed = set()
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/oauth.py` & `bbot-1.1.8.3341rc0/bbot/modules/oauth.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from .base import BaseModule
 
 
 class OAUTH(BaseModule):
     watched_events = ["DNS_NAME", "URL_UNVERIFIED"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "cloud-enum", "web-basic", "web-thorough", "active", "safe"]
-    meta = {"description": "Enumerate OAUTH and OpenID Connect services"}
+    meta = {
+        "description": "Enumerate OAUTH and OpenID Connect services",
+        "created_date": "2023-07-12",
+        "author": "@TheTechromancer",
+    }
     options = {"try_all": False}
     options_desc = {"try_all": "Check for OAUTH/IODC on every subdomain and URL."}
 
     in_scope_only = False
     scope_distance_modifier = 1
     _max_event_handlers = 2
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/otx.py` & `bbot-1.1.8.3341rc0/bbot/modules/columbus.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
-class otx(subdomain_enum):
+class columbus(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query otx.alienvault.com for subdomains"}
+    meta = {
+        "description": "Query the Columbus Project API for subdomains",
+        "created_date": "2023-06-01",
+        "author": "@TheTechromancer",
+    }
 
-    base_url = "https://otx.alienvault.com"
+    base_url = "https://columbus.elmasy.com/api/lookup"
 
-    def request_url(self, query):
-        url = f"{self.base_url}/api/v1/indicators/domain/{self.helpers.quote(query)}/passive_dns"
-        return self.request_with_fail_count(url)
+    async def request_url(self, query):
+        url = f"{self.base_url}/{self.helpers.quote(query)}?days=365"
+        return await self.request_with_fail_count(url)
 
     def parse_results(self, r, query):
-        j = r.json()
-        if isinstance(j, dict):
-            for entry in j.get("passive_dns", []):
-                subdomain = entry.get("hostname", "")
-                if subdomain:
-                    yield subdomain
+        results = set()
+        json = r.json()
+        if json and isinstance(json, list):
+            return set([f"{s.lower()}.{query}" for s in json])
+        return results
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/asset_inventory.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         "VULNERABILITY",
         "TECHNOLOGY",
         "IP_ADDRESS",
         "WAF",
         "HTTP_RESPONSE",
     ]
     produced_events = ["IP_ADDRESS", "OPEN_TCP_PORT"]
-    meta = {"description": "Merge hosts, open ports, technologies, findings, etc. into a single asset inventory CSV"}
+    meta = {
+        "description": "Merge hosts, open ports, technologies, findings, etc. into a single asset inventory CSV",
+        "created_date": "2022-09-30",
+        "author": "@liquidsec",
+    }
     options = {"output_file": "", "use_previous": False, "recheck": False, "summary_netmask": 16}
     options_desc = {
         "output_file": "Set a custom output file",
         "use_previous": "Emit previous asset inventory as new events (use in conjunction with -n <old_scan_name>)",
         "recheck": "When use_previous=True, don't retain past details like open ports or findings. Instead, allow them to be rediscovered by the new scan",
         "summary_netmask": "Subnet mask to use when summarizing IP addresses at end of scan",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/base.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/csv.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/csv.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from contextlib import suppress
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class CSV(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Output to CSV"}
+    meta = {"description": "Output to CSV", "created_date": "2022-04-07", "author": "@TheTechromancer"}
     options = {"output_file": ""}
     options_desc = {"output_file": "Output to CSV file"}
 
     header_row = ["Event type", "Event data", "IP Address", "Source Module", "Scope Distance", "Event Tags"]
     filename = "output.csv"
     accept_dupes = False
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/discord.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/discord.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 from bbot.modules.templates.webhook import WebhookOutputModule
 
 
 class Discord(WebhookOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Message a Discord channel when certain events are encountered"}
+    meta = {
+        "description": "Message a Discord channel when certain events are encountered",
+        "created_date": "2023-08-14",
+        "author": "@TheTechromancer",
+    }
     options = {"webhook_url": "", "event_types": ["VULNERABILITY", "FINDING"], "min_severity": "LOW"}
     options_desc = {
         "webhook_url": "Discord webhook URL",
         "event_types": "Types of events to send",
         "min_severity": "Only allow VULNERABILITY events of this severity or higher",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/emails.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/emails.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.base import BaseModule
 from bbot.modules.output.human import Human
 
 
 class Emails(Human):
     watched_events = ["EMAIL_ADDRESS"]
     flags = ["email-enum"]
-    meta = {"description": "Output any email addresses found belonging to the target domain"}
+    meta = {
+        "description": "Output any email addresses found belonging to the target domain",
+        "created_date": "2023-12-23",
+        "author": "@domwhewell-sage",
+    }
     options = {"output_file": ""}
     options_desc = {"output_file": "Output to file"}
     in_scope_only = True
 
     output_filename = "emails.txt"
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/http.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.core.errors import RequestError
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class HTTP(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Send every event to a custom URL via a web request"}
+    meta = {
+        "description": "Send every event to a custom URL via a web request",
+        "created_date": "2022-04-13",
+        "author": "@TheTechromancer",
+    }
     options = {
         "url": "",
         "method": "POST",
         "bearer": "",
         "username": "",
         "password": "",
         "timeout": 10,
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/human.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/human.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from bbot.core.helpers.logger import log_to_stderr
 from bbot.modules.output.base import BaseOutputModule
 
 
 class Human(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Output to text"}
+    meta = {"description": "Output to text", "created_date": "2022-04-07", "author": "@TheTechromancer"}
     options = {"output_file": "", "console": True}
     options_desc = {"output_file": "Output to file", "console": "Output to console"}
     vuln_severity_map = {"LOW": "HUGEWARNING", "MEDIUM": "HUGEWARNING", "HIGH": "CRITICAL", "CRITICAL": "CRITICAL"}
     accept_dupes = False
 
     output_filename = "output.txt"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/json.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from contextlib import suppress
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class JSON(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Output to Newline-Delimited JSON (NDJSON)"}
+    meta = {
+        "description": "Output to Newline-Delimited JSON (NDJSON)",
+        "created_date": "2022-04-07",
+        "author": "@TheTechromancer",
+    }
     options = {"output_file": "", "console": False, "siem_friendly": False}
     options_desc = {
         "output_file": "Output to file",
         "console": "Output to console",
         "siem_friendly": "Output JSON in a SIEM-friendly format for ingestion into Elastic, Splunk, etc.",
     }
     _preserve_graph = True
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/neo4j.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     > docker remove <CONTAINER_ID>
 
     # start a stopped container
     > docker start <CONTAINER_ID>
     """
 
     watched_events = ["*"]
-    meta = {"description": "Output to Neo4j"}
+    meta = {"description": "Output to Neo4j", "created_date": "2022-04-07", "author": "@TheTechromancer"}
     options = {"uri": "bolt://localhost:7687", "username": "neo4j", "password": "bbotislife"}
     options_desc = {
         "uri": "Neo4j server + port",
         "username": "Neo4j username",
         "password": "Neo4j password",
     }
     deps_pip = ["neo4j"]
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/slack.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/slack.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import yaml
 
 from bbot.modules.templates.webhook import WebhookOutputModule
 
 
 class Slack(WebhookOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Message a Slack channel when certain events are encountered"}
+    meta = {
+        "description": "Message a Slack channel when certain events are encountered",
+        "created_date": "2023-08-14",
+        "author": "@TheTechromancer",
+    }
     options = {"webhook_url": "", "event_types": ["VULNERABILITY", "FINDING"], "min_severity": "LOW"}
     options_desc = {
         "webhook_url": "Discord webhook URL",
         "event_types": "Types of events to send",
         "min_severity": "Only allow VULNERABILITY events of this severity or higher",
     }
     good_status_code = 200
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/splunk.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/splunk.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.core.errors import RequestError
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class Splunk(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Send every event to a splunk instance through HTTP Event Collector"}
+    meta = {
+        "description": "Send every event to a splunk instance through HTTP Event Collector",
+        "created_date": "2024-02-17",
+        "author": "@w0Tx",
+    }
     options = {
         "url": "",
         "hectoken": "",
         "index": "",
         "source": "",
         "timeout": 10,
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/subdomains.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.base import BaseModule
 from bbot.modules.output.human import Human
 
 
 class Subdomains(Human):
     watched_events = ["DNS_NAME", "DNS_NAME_UNRESOLVED"]
     flags = ["subdomain-enum"]
-    meta = {"description": "Output only resolved, in-scope subdomains"}
+    meta = {
+        "description": "Output only resolved, in-scope subdomains",
+        "created_date": "2023-07-31",
+        "author": "@TheTechromancer",
+    }
     options = {"output_file": "", "include_unresolved": False}
     options_desc = {"output_file": "Output to file", "include_unresolved": "Include unresolved subdomains in output"}
     accept_dupes = False
     in_scope_only = True
 
     output_filename = "subdomains.txt"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/teams.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/teams.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from bbot.modules.templates.webhook import WebhookOutputModule
 
 
 class Teams(WebhookOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Message a Teams channel when certain events are encountered"}
+    meta = {
+        "description": "Message a Teams channel when certain events are encountered",
+        "created_date": "2023-08-14",
+        "author": "@TheTechromancer",
+    }
     options = {"webhook_url": "", "event_types": ["VULNERABILITY", "FINDING"], "min_severity": "LOW"}
     options_desc = {
         "webhook_url": "Discord webhook URL",
         "event_types": "Types of events to send",
         "min_severity": "Only allow VULNERABILITY events of this severity or higher",
     }
     _max_event_handlers = 5
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/web_report.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/web_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.output.base import BaseOutputModule
 import markdown
 import html
 
 
 class web_report(BaseOutputModule):
     watched_events = ["URL", "TECHNOLOGY", "FINDING", "VULNERABILITY", "VHOST"]
-    meta = {"description": "Create a markdown report with web assets"}
+    meta = {
+        "description": "Create a markdown report with web assets",
+        "created_date": "2023-02-08",
+        "author": "@liquidsec",
+    }
     options = {
         "output_file": "",
         "css_theme_file": "https://cdnjs.cloudflare.com/ajax/libs/github-markdown-css/5.1.0/github-markdown.min.css",
     }
     options_desc = {"output_file": "Output to file", "css_theme_file": "CSS theme URL for HTML output"}
     deps_pip = ["markdown~=3.4.3"]
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/output/websocket.py` & `bbot-1.1.8.3341rc0/bbot/modules/output/websocket.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import websockets
 
 from bbot.modules.output.base import BaseOutputModule
 
 
 class Websocket(BaseOutputModule):
     watched_events = ["*"]
-    meta = {"description": "Output to websockets"}
+    meta = {"description": "Output to websockets", "created_date": "2022-04-15", "author": "@TheTechromancer"}
     options = {"url": "", "token": "", "preserve_graph": True}
     options_desc = {
         "url": "Web URL",
         "token": "Authorization Bearer token",
         "preserve_graph": "Preserve full chains of events in the graph (prevents orphans)",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.8.3341rc0/bbot/modules/paramminer_cookies.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
     """
 
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-paramminer"]
     meta = {
         "description": "Smart brute-force to check for common HTTP cookie parameters",
+        "created_date": "2022-06-27",
+        "author": "@liquidsec",
     }
     options = {
         "wordlist": "",  # default is defined within setup function
         "http_extract": True,
         "skip_boring_words": True,
     }
     options_desc = {
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.8.3341rc0/bbot/modules/paramminer_getparams.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,19 @@
     """
     Inspired by https://github.com/PortSwigger/param-miner
     """
 
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-paramminer"]
-    meta = {"description": "Use smart brute-force to check for common HTTP GET parameters"}
+    meta = {
+        "description": "Use smart brute-force to check for common HTTP GET parameters",
+        "created_date": "2022-06-28",
+        "author": "@liquidsec",
+    }
     scanned_hosts = []
     options = {
         "wordlist": "",  # default is defined within setup function
         "http_extract": True,
         "skip_boring_words": True,
     }
     options_desc = {
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.8.3341rc0/bbot/modules/paramminer_headers.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,19 @@
     """
     Inspired by https://github.com/PortSwigger/param-miner
     """
 
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-paramminer"]
-    meta = {"description": "Use smart brute-force to check for common HTTP header parameters"}
+    meta = {
+        "description": "Use smart brute-force to check for common HTTP header parameters",
+        "created_date": "2022-04-15",
+        "author": "@pmueller",
+    }
     options = {
         "wordlist": "",  # default is defined within setup function
         "http_extract": True,
         "skip_boring_words": True,
     }
     options_desc = {
         "wordlist": "Define the wordlist to be used to derive headers",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/passivetotal.py` & `bbot-1.1.8.3341rc0/bbot/modules/passivetotal.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class passivetotal(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the PassiveTotal API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query the PassiveTotal API for subdomains",
+        "created_date": "2022-08-08",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"username": "", "api_key": ""}
     options_desc = {"username": "RiskIQ Username", "api_key": "RiskIQ API Key"}
 
     base_url = "https://api.passivetotal.org/v2"
 
     async def setup(self):
         self.username = self.config.get("username", "")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/pgp.py` & `bbot-1.1.8.3341rc0/bbot/modules/pgp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class pgp(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["EMAIL_ADDRESS"]
     flags = ["passive", "email-enum", "safe"]
-    meta = {"description": "Query common PGP servers for email addresses"}
+    meta = {
+        "description": "Query common PGP servers for email addresses",
+        "created_date": "2022-08-10",
+        "author": "@TheTechromancer",
+    }
     options = {
         "search_urls": [
             "https://keyserver.ubuntu.com/pks/lookup?fingerprint=on&op=vindex&search=<query>",
             "http://the.earth.li:11371/pks/lookup?fingerprint=on&op=vindex&search=<query>",
         ]
     }
     options_desc = {"search_urls": "PGP key servers to search"}
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/postman.py` & `bbot-1.1.8.3341rc0/bbot/modules/postman.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class postman(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["passive", "subdomain-enum", "safe"]
-    meta = {"description": "Query Postman's API for related workspaces, collections, requests"}
+    meta = {
+        "description": "Query Postman's API for related workspaces, collections, requests",
+        "created_date": "2023-12-23",
+        "author": "@domwhewell-sage",
+    }
 
     base_url = "https://www.postman.com/_api"
 
     headers = {
         "Content-Type": "application/json",
         "X-App-Version": "10.18.8-230926-0808",
         "X-Entity-Team-Id": "0",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/rapiddns.py` & `bbot-1.1.8.3341rc0/bbot/modules/rapiddns.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class rapiddns(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query rapiddns.io for subdomains"}
+    meta = {
+        "description": "Query rapiddns.io for subdomains",
+        "created_date": "2022-08-24",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://rapiddns.io"
 
     async def request_url(self, query):
         url = f"{self.base_url}/subdomain/{self.helpers.quote(query)}?full=1#result"
         response = await self.request_with_fail_count(url)
         return response
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.8.3341rc0/bbot/modules/report/affiliates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.report.base import BaseReportModule
 
 
 class affiliates(BaseReportModule):
     watched_events = ["*"]
     produced_events = []
     flags = ["passive", "safe", "affiliates"]
-    meta = {"description": "Summarize affiliate domains at the end of a scan"}
+    meta = {
+        "description": "Summarize affiliate domains at the end of a scan",
+        "created_date": "2022-07-25",
+        "author": "@TheTechromancer",
+    }
     scope_distance_modifier = None
     accept_dupes = True
 
     async def setup(self):
         self.affiliates = {}
         return True
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/report/asn.py` & `bbot-1.1.8.3341rc0/bbot/modules/report/asn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.report.base import BaseReportModule
 
 
 class asn(BaseReportModule):
     watched_events = ["IP_ADDRESS"]
     produced_events = ["ASN"]
     flags = ["passive", "subdomain-enum", "safe"]
-    meta = {"description": "Query ripe and bgpview.io for ASNs"}
+    meta = {
+        "description": "Query ripe and bgpview.io for ASNs",
+        "created_date": "2022-07-25",
+        "author": "@TheTechromancer",
+    }
     scope_distance_modifier = 1
     # we accept dupes to avoid missing data
     # because sometimes IP addresses are re-emitted with lower scope distances
     accept_dupes = True
 
     async def setup(self):
         self.asn_counts = {}
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/robots.py` & `bbot-1.1.8.3341rc0/bbot/modules/robots.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from bbot.modules.base import BaseModule
 
 
 class robots(BaseModule):
     watched_events = ["URL"]
     produced_events = ["URL_UNVERIFIED"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Look for and parse robots.txt"}
+    meta = {"description": "Look for and parse robots.txt", "created_date": "2023-02-01", "author": "@liquidsec"}
 
     options = {"include_sitemap": False, "include_allow": True, "include_disallow": True}
     options_desc = {
         "include_sitemap": "Include 'sitemap' entries",
         "include_allow": "Include 'Allow' Entries",
         "include_disallow": "Include 'Disallow' Entries",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/secretsdb.py` & `bbot-1.1.8.3341rc0/bbot/modules/secretsdb.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from .base import BaseModule
 
 
 class secretsdb(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["FINDING"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
-    meta = {"description": "Detect common secrets with secrets-patterns-db"}
+    meta = {
+        "description": "Detect common secrets with secrets-patterns-db",
+        "created_date": "2023-03-17",
+        "author": "@TheTechromancer",
+    }
     options = {
         "min_confidence": 99,
         "signatures": "https://raw.githubusercontent.com/blacklanternsecurity/secrets-patterns-db/master/db/rules-stable.yml",
     }
     options_desc = {
         "min_confidence": "Only use signatures with this confidence score or higher",
         "signatures": "File path or URL to YAML signatures",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/securitytrails.py` & `bbot-1.1.8.3341rc0/bbot/modules/securitytrails.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class securitytrails(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query the SecurityTrails API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query the SecurityTrails API for subdomains",
+        "created_date": "2022-07-03",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "SecurityTrails API key"}
 
     base_url = "https://api.securitytrails.com/v1"
 
     async def setup(self):
         self.limit = 100
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.8.3341rc0/bbot/modules/shodan_dns.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.shodan import shodan
 
 
 class shodan_dns(shodan):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query Shodan for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query Shodan for subdomains",
+        "created_date": "2022-07-03",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "Shodan API key"}
 
     base_url = "https://api.shodan.io"
 
     async def request_url(self, query):
         url = f"{self.base_url}/dns/domain/{self.helpers.quote(query)}?key={self.api_key}"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/sitedossier.py` & `bbot-1.1.8.3341rc0/bbot/modules/sitedossier.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum
 
 
 class sitedossier(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
-    meta = {"description": "Query sitedossier.com for subdomains"}
+    meta = {
+        "description": "Query sitedossier.com for subdomains",
+        "created_date": "2023-08-04",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "http://www.sitedossier.com/parentdomain"
     max_pages = 10
 
     async def handle_event(self, event):
         query = self.make_query(event)
         async for hostname in self.query(query):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/skymem.py` & `bbot-1.1.8.3341rc0/bbot/modules/skymem.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 from .emailformat import emailformat
 
 
 class skymem(emailformat):
     watched_events = ["DNS_NAME"]
     produced_events = ["EMAIL_ADDRESS"]
     flags = ["passive", "email-enum", "safe"]
-    meta = {"description": "Query skymem.info for email addresses"}
+    meta = {
+        "description": "Query skymem.info for email addresses",
+        "created_date": "2022-07-11",
+        "author": "@TheTechromancer",
+    }
 
     base_url = "https://www.skymem.info"
 
     async def handle_event(self, event):
         _, query = self.helpers.split_domain(event.data)
         # get first page
         url = f"{self.base_url}/srch?q={self.helpers.quote(query)}"
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/smuggler.py` & `bbot-1.1.8.3341rc0/bbot/modules/smuggler.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 
 
 class smuggler(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "slow", "web-thorough"]
-    meta = {"description": "Check for HTTP smuggling"}
+    meta = {"description": "Check for HTTP smuggling", "created_date": "2022-07-06", "author": "@liquidsec"}
 
     in_scope_only = True
     per_hostport_only = True
 
     deps_ansible = [
         {
             "name": "Get smuggler repo",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/social.py` & `bbot-1.1.8.3341rc0/bbot/modules/social.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import re
 from bbot.modules.base import BaseModule
 
 
 class social(BaseModule):
     watched_events = ["URL_UNVERIFIED"]
     produced_events = ["SOCIAL"]
-    meta = {"description": "Look for social media links in webpages"}
+    meta = {
+        "description": "Look for social media links in webpages",
+        "created_date": "2023-03-28",
+        "author": "@TheTechromancer",
+    }
     flags = ["passive", "safe", "social-enum"]
 
     # platform name : (regex, case_sensitive)
     social_media_platforms = {
         "linkedin": (r"linkedin.com/(?:in|company)/([a-zA-Z0-9-]+)", False),
         "facebook": (r"facebook.com/([a-zA-Z0-9.]+)", False),
         "twitter": (r"twitter.com/([a-zA-Z0-9_]{1,15})", False),
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/sslcert.py` & `bbot-1.1.8.3341rc0/bbot/modules/sslcert.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 class sslcert(BaseModule):
     watched_events = ["OPEN_TCP_PORT"]
     produced_events = ["DNS_NAME", "EMAIL_ADDRESS"]
     flags = ["affiliates", "subdomain-enum", "email-enum", "active", "safe", "web-basic", "web-thorough"]
     meta = {
         "description": "Visit open ports and retrieve SSL certificates",
+        "created_date": "2022-03-30",
+        "author": "@TheTechromancer",
     }
     options = {"timeout": 5.0, "skip_non_ssl": True}
     options_desc = {"timeout": "Socket connect timeout in seconds", "skip_non_ssl": "Don't try common non-SSL ports"}
     deps_apt = ["openssl"]
     deps_pip = ["pyOpenSSL~=24.0.0"]
     _max_event_handlers = 25
     scope_distance_modifier = 1
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/sublist3r.py` & `bbot-1.1.8.3341rc0/bbot/modules/sublist3r.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,13 +4,15 @@
 class sublist3r(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     # tag "subdomain-enum" removed 2023-02-24 because API is offline
     flags = ["passive", "safe"]
     meta = {
         "description": "Query sublist3r's API for subdomains",
+        "created_date": "2022-03-29",
+        "author": "@Want-EyeTea",
     }
 
     base_url = "https://api.sublist3r.com/search.php"
 
     def request_url(self, query):
         return self.request_with_fail_count(f"{self.base_url}?domain={query}", timeout=self.http_timeout + 10)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/telerik.py` & `bbot-1.1.8.3341rc0/bbot/modules/telerik.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,19 @@
 from bbot.modules.base import BaseModule
 
 
 class telerik(BaseModule):
     watched_events = ["URL", "HTTP_RESPONSE"]
     produced_events = ["VULNERABILITY", "FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Scan for critical Telerik vulnerabilities"}
+    meta = {
+        "description": "Scan for critical Telerik vulnerabilities",
+        "created_date": "2022-04-10",
+        "author": "@liquidsec",
+    }
 
     telerikVersions = [
         "2007.1423",
         "2007.1521",
         "2007.1626",
         "2007.2918",
         "2007.21010",
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/bucket.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/bucket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/github.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/portscanner.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/portscanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/shodan.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/shodan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/subdomain_enum.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/subdomain_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/templates/webhook.py` & `bbot-1.1.8.3341rc0/bbot/modules/templates/webhook.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/threatminer.py` & `bbot-1.1.8.3341rc0/bbot/modules/threatminer.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class threatminer(subdomain_enum):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
     meta = {
         "description": "Query threatminer's API for subdomains",
+        "created_date": "2022-07-28",
+        "author": "@TheTechromancer",
     }
 
     base_url = "https://api.threatminer.org/v2"
 
     async def request_url(self, query):
         url = f"{self.base_url}/domain.php?q={self.helpers.quote(query)}&rt=5"
         r = await self.request_with_fail_count(url, timeout=self.http_timeout + 30)
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/trufflehog.py` & `bbot-1.1.8.3341rc0/bbot/modules/trufflehog.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.modules.base import BaseModule
 
 
 class trufflehog(BaseModule):
     watched_events = ["FILESYSTEM"]
     produced_events = ["FINDING", "VULNERABILITY"]
     flags = ["passive", "safe"]
-    meta = {"description": "TruffleHog is a tool for finding credentials"}
+    meta = {
+        "description": "TruffleHog is a tool for finding credentials",
+        "created_date": "2024-03-12",
+        "author": "@domwhewell-sage",
+    }
 
     options = {
         "version": "3.75.1",
         "only_verified": True,
         "concurrency": 8,
     }
     options_desc = {
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.8.3341rc0/bbot/modules/url_manipulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 from bbot.core.errors import HttpCompareError
 
 
 class url_manipulation(BaseModule):
     watched_events = ["URL"]
     produced_events = ["FINDING"]
     flags = ["active", "aggressive", "web-thorough"]
-    meta = {"description": "Attempt to identify URL parsing/routing based vulnerabilities"}
+    meta = {
+        "description": "Attempt to identify URL parsing/routing based vulnerabilities",
+        "created_date": "2022-09-27",
+        "author": "@liquidsec",
+    }
     in_scope_only = True
 
     options = {"allow_redirects": True}
     options_desc = {
         "allow_redirects": "Allowing redirects will sometimes create false positives. Disallowing will sometimes create false negatives. Allowed by default."
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/urlscan.py` & `bbot-1.1.8.3341rc0/bbot/modules/urlscan.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 class urlscan(subdomain_enum):
     flags = ["subdomain-enum", "passive", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME", "URL_UNVERIFIED"]
     meta = {
         "description": "Query urlscan.io for subdomains",
+        "created_date": "2022-06-09",
+        "author": "@TheTechromancer",
     }
     options = {"urls": False}
     options_desc = {"urls": "Emit URLs in addition to DNS_NAMEs"}
 
     base_url = "https://urlscan.io/api/v1"
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/viewdns.py` & `bbot-1.1.8.3341rc0/bbot/modules/viewdns.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     """
 
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "passive", "safe"]
     meta = {
         "description": "Query viewdns.info's reverse whois for related domains",
+        "created_date": "2022-07-04",
+        "author": "@TheTechromancer",
     }
     base_url = "https://viewdns.info"
     in_scope_only = True
     per_domain_only = True
     _qsize = 1
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/virustotal.py` & `bbot-1.1.8.3341rc0/bbot/modules/virustotal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class virustotal(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query VirusTotal's API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query VirusTotal's API for subdomains",
+        "created_date": "2022-08-25",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": ""}
     options_desc = {"api_key": "VirusTotal API Key"}
 
     base_url = "https://www.virustotal.com/api/v3"
 
     async def setup(self):
         self.api_key = self.config.get("api_key", "")
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/wafw00f.py` & `bbot-1.1.8.3341rc0/bbot/modules/wafw00f.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,19 @@
     """
     https://github.com/EnableSecurity/wafw00f
     """
 
     watched_events = ["URL"]
     produced_events = ["WAF"]
     flags = ["active", "aggressive"]
-    meta = {"description": "Web Application Firewall Fingerprinting Tool"}
+    meta = {
+        "description": "Web Application Firewall Fingerprinting Tool",
+        "created_date": "2023-02-15",
+        "author": "@liquidsec",
+    }
 
     deps_pip = ["wafw00f~=2.2.0"]
 
     options = {"generic_detect": True}
     options_desc = {"generic_detect": "When no specific WAF detections are made, try to perform a generic detect"}
 
     in_scope_only = True
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.8.3341rc0/bbot/modules/wappalyzer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 class wappalyzer(BaseModule):
     watched_events = ["HTTP_RESPONSE"]
     produced_events = ["TECHNOLOGY"]
     flags = ["active", "safe", "web-basic", "web-thorough"]
     meta = {
         "description": "Extract technologies from web responses",
+        "created_date": "2022-04-15",
+        "author": "@liquidsec",
     }
     deps_pip = ["python-Wappalyzer~=0.3.1", "aiohttp~=3.9.0b0"]
     # accept all events regardless of scope distance
     scope_distance_modifier = None
     _max_event_handlers = 5
 
     async def setup(self):
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/wayback.py` & `bbot-1.1.8.3341rc0/bbot/modules/wayback.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 class wayback(subdomain_enum):
     flags = ["passive", "subdomain-enum", "safe"]
     watched_events = ["DNS_NAME"]
     produced_events = ["URL_UNVERIFIED", "DNS_NAME"]
     meta = {
         "description": "Query archive.org's API for subdomains",
+        "created_date": "2022-04-01",
+        "author": "@pmueller",
     }
     options = {"urls": False, "garbage_threshold": 10}
     options_desc = {
         "urls": "emit URLs in addition to DNS_NAMEs",
         "garbage_threshold": "Dedupe similar urls if they are in a group of this size or higher (lower values == less garbage data)",
     }
     in_scope_only = True
```

### Comparing `bbot-1.1.8.3335rc0/bbot/modules/zoomeye.py` & `bbot-1.1.8.3341rc0/bbot/modules/zoomeye.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from bbot.modules.templates.subdomain_enum import subdomain_enum_apikey
 
 
 class zoomeye(subdomain_enum_apikey):
     watched_events = ["DNS_NAME"]
     produced_events = ["DNS_NAME"]
     flags = ["affiliates", "subdomain-enum", "passive", "safe"]
-    meta = {"description": "Query ZoomEye's API for subdomains", "auth_required": True}
+    meta = {
+        "description": "Query ZoomEye's API for subdomains",
+        "created_date": "2022-08-03",
+        "author": "@TheTechromancer",
+        "auth_required": True,
+    }
     options = {"api_key": "", "max_pages": 20, "include_related": False}
     options_desc = {
         "api_key": "ZoomEye API key",
         "max_pages": "How many pages of results to fetch",
         "include_related": "Include domains which may be related to the target",
     }
```

### Comparing `bbot-1.1.8.3335rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.8.3341rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/scanner/manager.py` & `bbot-1.1.8.3341rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/scanner/scanner.py` & `bbot-1.1.8.3341rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/scanner/stats.py` & `bbot-1.1.8.3341rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/scanner/target.py` & `bbot-1.1.8.3341rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/scripts/docs.py` & `bbot-1.1.8.3341rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.8.3341rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/conftest.py` & `bbot-1.1.8.3341rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/run_tests.sh` & `bbot-1.1.8.3341rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test.conf` & `bbot-1.1.8.3341rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_manager_deduplication.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_manager_deduplication.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_discord.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_emails.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_json.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_postman.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_teams.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.8.3341rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/testsslcert.pem` & `bbot-1.1.8.3341rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/test/testsslkey.pem` & `bbot-1.1.8.3341rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/ms_on_prem_subdomains.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/ms_on_prem_subdomains.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.8.3341rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.8.3341rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3335rc0/pyproject.toml` & `bbot-1.1.8.3341rc0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.8.3335rc"
+version = "v1.1.8.3341rc"
 description = "OSINT automation for hackers."
 authors = [
     "TheTechromancer",
     "Paul Mueller",
 ]
 license = "GPL-3.0"
 readme = "README.md"
```

### Comparing `bbot-1.1.8.3335rc0/PKG-INFO` & `bbot-1.1.8.3341rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.8.3335rc0
+Version: 1.1.8.3341rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Keywords: python,cli,automation,osint,neo4j,scanner,python-library,hacking,recursion,pentesting,recon,command-line-tool,bugbounty,subdomains,security-tools,subdomain-scanner,osint-framework,attack-surface,subdomain-enumeration,osint-tool
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

