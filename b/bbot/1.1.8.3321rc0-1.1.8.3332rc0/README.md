# Comparing `tmp/bbot-1.1.8.3321rc0.tar.gz` & `tmp/bbot-1.1.8.3332rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.1.8.3321rc0.tar", max compression
+gzip compressed data, was "bbot-1.1.8.3332rc0.tar", max compression
```

## Comparing `bbot-1.1.8.3321rc0.tar` & `bbot-1.1.8.3332rc0.tar`

### file list

```diff
@@ -1,346 +1,346 @@
--rw-r--r--   0        0        0    32473 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/LICENSE
--rw-r--r--   0        0        0    40272 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/README.md
--rw-r--r--   0        0        0      211 2024-05-15 21:42:22.242473 bbot-1.1.8.3321rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     7898 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      450 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    17601 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/cli.py
--rw-r--r--   0        0        0       59 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3588 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     9843 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     5182 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1341 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      617 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/errors.py
--rw-r--r--   0        0        0       91 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    46323 2024-05-15 21:42:08.598548 bbot-1.1.8.3321rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1656 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0     1232 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/flags.py
--rw-r--r--   0        0        0       86 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3583 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/async_helpers.py
--rw-r--r--   0        0        0     1537 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     4341 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/cloud.py
--rw-r--r--   0        0        0    10976 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    14117 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     9199 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    47786 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     5639 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/files.py
--rw-r--r--   0        0        0     6354 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0    12632 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1408 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    82906 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    22071 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0    10041 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0     1990 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/ratelimiter.py
--rw-r--r--   0        0        0     3463 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     5947 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     8781 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0    31838 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    19801 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0      191 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     8118 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     4158 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     2328 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/ajaxpro.py
--rw-r--r--   0        0        0     1824 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     1372 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/azure_realm.py
--rw-r--r--   0        0        0     4691 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     4150 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/baddns.py
--rw-r--r--   0        0        0     1245 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/baddns_zone.py
--rw-r--r--   0        0        0     3549 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    59062 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2352 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1299 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0      655 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_amazon.py
--rw-r--r--   0        0        0     1020 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      775 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1915 2024-05-15 21:42:08.602548 bbot-1.1.8.3321rc0/bbot/modules/bucket_file_enum.py
--rw-r--r--   0        0        0     1352 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2540 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bucket_google.py
--rw-r--r--   0        0        0     4911 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     6553 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1188 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     3371 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      798 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     1522 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/chaos.py
--rw-r--r--   0        0        0     1810 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/code_repository.py
--rw-r--r--   0        0        0      735 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/columbus.py
--rw-r--r--   0        0        0     3297 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/credshed.py
--rw-r--r--   0        0        0      376 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1230 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0     5316 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/dastardly.py
--rw-r--r--   0        0        0    14079 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    17260 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5239 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     3928 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dehashed.py
--rw-r--r--   0        0        0      930 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/digitorus.py
--rw-r--r--   0        0        0     5324 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     3186 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     8781 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/docker_pull.py
--rw-r--r--   0        0        0     3271 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dockerhub.py
--rw-r--r--   0        0        0     9245 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/dotnetnuke.py
--rw-r--r--   0        0        0      791 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11758 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     7540 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/filedownload.py
--rw-r--r--   0        0        0     2184 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1195 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7794 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     1329 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/git.py
--rw-r--r--   0        0        0     2073 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/git_clone.py
--rw-r--r--   0        0        0     3147 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_codesearch.py
--rw-r--r--   0        0        0     8735 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_org.py
--rw-r--r--   0        0        0     6070 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/github_workflows.py
--rw-r--r--   0        0        0     5655 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/gitlab.py
--rw-r--r--   0        0        0    11415 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      890 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7172 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     6758 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     5990 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     2098 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0    13124 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      304 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    18695 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     8286 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     4384 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/internetdb.py
--rw-r--r--   0        0        0     2123 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ip2location.py
--rw-r--r--   0        0        0     1539 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     1767 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0     1541 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    10816 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    21031 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0      857 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/myssl.py
--rw-r--r--   0        0        0     2281 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/newsletters.py
--rw-r--r--   0        0        0     5506 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/nmap.py
--rw-r--r--   0        0        0     4731 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0     5852 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/oauth.py
--rw-r--r--   0        0        0      774 2024-05-15 21:42:08.606548 bbot-1.1.8.3321rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0    14731 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     3215 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2604 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0      531 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/discord.py
--rw-r--r--   0        0        0      985 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/emails.py
--rw-r--r--   0        0        0     2182 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1907 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1375 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     2746 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      210 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     1117 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/slack.py
--rw-r--r--   0        0        0     1886 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/splunk.py
--rw-r--r--   0        0        0     1430 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/subdomains.py
--rw-r--r--   0        0        0      723 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/teams.py
--rw-r--r--   0        0        0     3627 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     2218 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1689 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1681 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     9552 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1619 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1420 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0     5479 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/postman.py
--rw-r--r--   0        0        0      832 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1602 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8456 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      828 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2025 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2898 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1201 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0      792 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1993 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sitedossier.py
--rw-r--r--   0        0        0     1478 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1408 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     2000 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     7822 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     1327 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/subdomaincenter.py
--rw-r--r--   0        0        0      553 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    17041 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0     5744 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/bucket.py
--rw-r--r--   0        0        0     1308 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/github.py
--rw-r--r--   0        0        0     2436 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/portscanner.py
--rw-r--r--   0        0        0     1182 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/shodan.py
--rw-r--r--   0        0        0     6100 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/subdomain_enum.py
--rw-r--r--   0        0        0     3789 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/templates/webhook.py
--rw-r--r--   0        0        0      678 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     4527 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/trufflehog.py
--rw-r--r--   0        0        0     4102 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2992 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2325 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1591 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     2010 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1272 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2871 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2336 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      793 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    29339 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    42299 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     2702 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0    11540 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scanner/target.py
--rwxr-xr-x   0        0        0     5889 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/scripts/docs.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.610548 bbot-1.1.8.3321rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    12010 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0     4870 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0       31 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/coverage.cfg
--rwxr-xr-x   0        0        0      652 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0     1091 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      323 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_output.ndjson
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1445 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test__module__tests.py
--rw-r--r--   0        0        0     5523 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_agent.py
--rw-r--r--   0        0        0     6544 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cli.py
--rw-r--r--   0        0        0     3808 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cloud_helpers.py
--rw-r--r--   0        0        0     5853 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_command.py
--rw-r--r--   0        0        0      495 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_config.py
--rw-r--r--   0        0        0      722 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_depsinstaller.py
--rw-r--r--   0        0        0     7572 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_dns.py
--rw-r--r--   0        0        0       79 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_docs.py
--rw-r--r--   0        0        0    23553 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_events.py
--rw-r--r--   0        0        0      702 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_files.py
--rw-r--r--   0        0        0    31826 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_helpers.py
--rw-r--r--   0        0        0    16305 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_deduplication.py
--rw-r--r--   0        0        0    79706 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
--rw-r--r--   0        0        0    16943 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_modules_basic.py
--rw-r--r--   0        0        0     2657 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_python_api.py
--rw-r--r--   0        0        0     7144 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_regexes.py
--rw-r--r--   0        0        0     2870 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scan.py
--rw-r--r--   0        0        0      706 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scope.py
--rw-r--r--   0        0        0     2175 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_target.py
--rw-r--r--   0        0        0    13141 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_web.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0        0 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/__init__.py
--rw-r--r--   0        0        0     5344 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/base.py
--rw-r--r--   0        0        0      664 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
--rw-r--r--   0        0        0      473 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
--rw-r--r--   0        0        0     2789 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
--rw-r--r--   0        0        0      546 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
--rw-r--r--   0        0        0    10606 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
--rw-r--r--   0        0        0     3098 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
--rw-r--r--   0        0        0     1207 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
--rw-r--r--   0        0        0     4805 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
--rw-r--r--   0        0        0     2795 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
--rw-r--r--   0        0        0     2397 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
--rw-r--r--   0        0        0     5599 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
--rw-r--r--   0        0        0     1045 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
--rw-r--r--   0        0        0     1101 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
--rw-r--r--   0        0        0     3984 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
--rw-r--r--   0        0        0      552 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
--rw-r--r--   0        0        0      907 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
--rw-r--r--   0        0        0     2282 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
--rw-r--r--   0        0        0      506 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
--rw-r--r--   0        0        0     1312 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
--rw-r--r--   0        0        0     5051 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
--rw-r--r--   0        0        0     3551 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
--rw-r--r--   0        0        0      982 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
--rw-r--r--   0        0        0     3956 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
--rw-r--r--   0        0        0      636 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
--rw-r--r--   0        0        0      956 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
--rw-r--r--   0        0        0     2047 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
--rw-r--r--   0        0        0      564 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
--rw-r--r--   0        0        0     3362 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
--rw-r--r--   0        0        0      762 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
--rw-r--r--   0        0        0      717 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
--rw-r--r--   0        0        0      273 2024-05-15 21:42:08.614548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
--rw-r--r--   0        0        0     2321 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
--rw-r--r--   0        0        0     3615 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
--rw-r--r--   0        0        0     1613 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
--rw-r--r--   0        0        0     1863 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
--rw-r--r--   0        0        0      952 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
--rw-r--r--   0        0        0    59749 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
--rw-r--r--   0        0        0    27988 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
--rw-r--r--   0        0        0     3907 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
--rw-r--r--   0        0        0     8232 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
--rw-r--r--   0        0        0      461 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
--rw-r--r--   0        0        0      944 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
--rw-r--r--   0        0        0    14708 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
--rw-r--r--   0        0        0     2955 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
--rw-r--r--   0        0        0     7669 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
--rw-r--r--   0        0        0     2389 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
--rw-r--r--   0        0        0      445 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
--rw-r--r--   0        0        0     1946 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
--rw-r--r--   0        0        0     2040 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
--rw-r--r--   0        0        0     1656 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git.py
--rw-r--r--   0        0        0    12266 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
--rw-r--r--   0        0        0     3718 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
--rw-r--r--   0        0        0    24606 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
--rw-r--r--   0        0        0    35521 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
--rw-r--r--   0        0        0    11579 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
--rw-r--r--   0        0        0     3433 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
--rw-r--r--   0        0        0      609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
--rw-r--r--   0        0        0     2702 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
--rw-r--r--   0        0        0     2155 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_http.py
--rw-r--r--   0        0        0     4939 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
--rw-r--r--   0        0        0      249 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_human.py
--rw-r--r--   0        0        0      665 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
--rw-r--r--   0        0        0     4086 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
--rw-r--r--   0        0        0     2879 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
--rw-r--r--   0        0        0     2231 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
--rw-r--r--   0        0        0     1123 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
--rw-r--r--   0        0        0      604 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
--rw-r--r--   0        0        0     2767 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
--rw-r--r--   0        0        0     1006 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_json.py
--rw-r--r--   0        0        0     1641 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
--rw-r--r--   0        0        0     1711 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
--rw-r--r--   0        0        0      428 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
--rw-r--r--   0        0        0     1532 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
--rw-r--r--   0        0        0     1030 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
--rw-r--r--   0        0        0     2305 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
--rw-r--r--   0        0        0     3618 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
--rw-r--r--   0        0        0     1116 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
--rw-r--r--   0        0        0     5609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
--rw-r--r--   0        0        0     9402 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
--rw-r--r--   0        0        0     1160 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
--rw-r--r--   0        0        0     2142 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
--rw-r--r--   0        0        0    10680 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
--rw-r--r--   0        0        0     2190 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
--rw-r--r--   0        0        0      961 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
--rw-r--r--   0        0        0     1609 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
--rw-r--r--   0        0        0    14768 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
--rw-r--r--   0        0        0      184 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_python.py
--rw-r--r--   0        0        0      750 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
--rw-r--r--   0        0        0      747 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
--rw-r--r--   0        0        0     1564 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
--rw-r--r--   0        0        0      537 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
--rw-r--r--   0        0        0      758 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
--rw-r--r--   0        0        0      713 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
--rw-r--r--   0        0        0     6220 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
--rw-r--r--   0        0        0     2321 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
--rw-r--r--   0        0        0      415 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
--rw-r--r--   0        0        0     2426 2024-05-15 21:42:08.618548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
--rw-r--r--   0        0        0     1700 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_social.py
--rw-r--r--   0        0        0     3121 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
--rw-r--r--   0        0        0     1866 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
--rw-r--r--   0        0        0      706 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
--rw-r--r--   0        0        0      610 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
--rw-r--r--   0        0        0     1116 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
--rw-r--r--   0        0        0      611 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
--rw-r--r--   0        0        0     1222 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
--rw-r--r--   0        0        0     7751 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
--rw-r--r--   0        0        0      489 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
--rw-r--r--   0        0        0    62527 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
--rw-r--r--   0        0        0     1144 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
--rw-r--r--   0        0        0     2902 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
--rw-r--r--   0        0        0     2874 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
--rw-r--r--   0        0        0    15239 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
--rw-r--r--   0        0        0     3401 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
--rw-r--r--   0        0        0     1304 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
--rw-r--r--   0        0        0      936 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
--rw-r--r--   0        0        0      548 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
--rw-r--r--   0        0        0     2026 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
--rw-r--r--   0        0        0     1009 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
--rw-r--r--   0        0        0     1979 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
--rw-r--r--   0        0        0     1103 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/testsslcert.pem
--rw-r--r--   0        0        0     1704 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/test/testsslkey.pem
--rw-r--r--   0        0        0      476 2024-05-15 21:42:08.622548 bbot-1.1.8.3321rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0      764 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/ms_on_prem_subdomains.txt
--rw-r--r--   0        0        0    32226 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0    17458 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_headers.txt
--rw-r--r--   0        0        0    54887 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_parameters.txt
--rw-r--r--   0        0        0     6068 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2024-05-15 21:42:08.626548 bbot-1.1.8.3321rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     2663 2024-05-15 21:42:22.238473 bbot-1.1.8.3321rc0/pyproject.toml
--rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.8.3321rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/LICENSE
+-rw-r--r--   0        0        0    40272 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/README.md
+-rw-r--r--   0        0        0      211 2024-05-16 15:16:53.605980 bbot-1.1.8.3332rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     7898 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      450 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    17601 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/cli.py
+-rw-r--r--   0        0        0       59 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3588 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     9843 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     5182 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1341 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      617 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0       91 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    46323 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1656 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0     1232 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/flags.py
+-rw-r--r--   0        0        0       86 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3583 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/async_helpers.py
+-rw-r--r--   0        0        0     1537 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     4341 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/cloud.py
+-rw-r--r--   0        0        0    11950 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    14117 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     9199 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    47786 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     5639 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/files.py
+-rw-r--r--   0        0        0     6354 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0    12632 2024-05-16 15:16:38.529855 bbot-1.1.8.3332rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1408 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    82906 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    22071 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0    10041 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0     1990 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/ratelimiter.py
+-rw-r--r--   0        0        0     3463 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     5947 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     8781 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0    31838 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    19801 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0      191 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     8118 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     4158 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     2328 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/ajaxpro.py
+-rw-r--r--   0        0        0     1824 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     1372 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/azure_realm.py
+-rw-r--r--   0        0        0     4691 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     4150 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/baddns.py
+-rw-r--r--   0        0        0     1245 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/baddns_zone.py
+-rw-r--r--   0        0        0     3549 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    59062 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2352 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1299 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0      655 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_amazon.py
+-rw-r--r--   0        0        0     1020 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      775 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1915 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_file_enum.py
+-rw-r--r--   0        0        0     1352 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2540 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bucket_google.py
+-rw-r--r--   0        0        0     4911 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     6553 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1188 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     3371 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      798 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     1522 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/chaos.py
+-rw-r--r--   0        0        0     1810 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/code_repository.py
+-rw-r--r--   0        0        0      735 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/columbus.py
+-rw-r--r--   0        0        0     3297 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/credshed.py
+-rw-r--r--   0        0        0      376 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1230 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0     5316 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/deadly/dastardly.py
+-rw-r--r--   0        0        0    14079 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    17260 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5239 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     3928 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/dehashed.py
+-rw-r--r--   0        0        0      930 2024-05-16 15:16:38.533855 bbot-1.1.8.3332rc0/bbot/modules/digitorus.py
+-rw-r--r--   0        0        0     5324 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     3186 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     8781 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/docker_pull.py
+-rw-r--r--   0        0        0     3271 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/dockerhub.py
+-rw-r--r--   0        0        0     9245 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/dotnetnuke.py
+-rw-r--r--   0        0        0      791 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11758 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     7540 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/filedownload.py
+-rw-r--r--   0        0        0     2184 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1195 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7794 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     1329 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/git.py
+-rw-r--r--   0        0        0     2073 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/git_clone.py
+-rw-r--r--   0        0        0     3147 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/github_codesearch.py
+-rw-r--r--   0        0        0     8735 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/github_org.py
+-rw-r--r--   0        0        0     6070 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/github_workflows.py
+-rw-r--r--   0        0        0     5655 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/gitlab.py
+-rw-r--r--   0        0        0    12165 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      890 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7172 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     6758 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     5990 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     2098 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0    13124 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      304 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    18695 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     8286 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     4384 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/internetdb.py
+-rw-r--r--   0        0        0     2123 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/ip2location.py
+-rw-r--r--   0        0        0     1539 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     1767 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0     1541 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    10816 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    21031 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0      857 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/myssl.py
+-rw-r--r--   0        0        0     2281 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/newsletters.py
+-rw-r--r--   0        0        0     5506 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/nmap.py
+-rw-r--r--   0        0        0     4731 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0     5852 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/oauth.py
+-rw-r--r--   0        0        0      774 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    14731 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     3215 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2604 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0      531 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/discord.py
+-rw-r--r--   0        0        0      985 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/emails.py
+-rw-r--r--   0        0        0     2182 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1907 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1375 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     2746 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      210 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     1117 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/slack.py
+-rw-r--r--   0        0        0     1886 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/splunk.py
+-rw-r--r--   0        0        0     1430 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/subdomains.py
+-rw-r--r--   0        0        0      723 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/teams.py
+-rw-r--r--   0        0        0     3627 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     2218 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1689 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1681 2024-05-16 15:16:38.537855 bbot-1.1.8.3332rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     9552 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1619 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1420 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0     5479 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/postman.py
+-rw-r--r--   0        0        0      832 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1602 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8456 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      828 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2025 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2898 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1201 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0      792 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1993 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/sitedossier.py
+-rw-r--r--   0        0        0     1478 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1408 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     2000 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     7822 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     1327 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/subdomaincenter.py
+-rw-r--r--   0        0        0      553 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    17041 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0     5744 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/bucket.py
+-rw-r--r--   0        0        0     1308 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/github.py
+-rw-r--r--   0        0        0     2436 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/portscanner.py
+-rw-r--r--   0        0        0     1182 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/shodan.py
+-rw-r--r--   0        0        0     6100 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/subdomain_enum.py
+-rw-r--r--   0        0        0     3789 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/templates/webhook.py
+-rw-r--r--   0        0        0      678 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     4527 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/trufflehog.py
+-rw-r--r--   0        0        0     4102 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2992 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2325 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1591 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     2010 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1272 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2871 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2336 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      793 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    29339 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    42299 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     2702 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0    11540 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scanner/target.py
+-rwxr-xr-x   0        0        0     5889 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/scripts/docs.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    12010 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0     4870 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0       31 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/coverage.cfg
+-rwxr-xr-x   0        0        0      652 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0     1091 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      323 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_output.ndjson
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1445 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test__module__tests.py
+-rw-r--r--   0        0        0     5523 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_agent.py
+-rw-r--r--   0        0        0     6544 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_cli.py
+-rw-r--r--   0        0        0     3808 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_cloud_helpers.py
+-rw-r--r--   0        0        0     6384 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_command.py
+-rw-r--r--   0        0        0      495 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_config.py
+-rw-r--r--   0        0        0      722 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_depsinstaller.py
+-rw-r--r--   0        0        0     7572 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_dns.py
+-rw-r--r--   0        0        0       79 2024-05-16 15:16:38.541855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_docs.py
+-rw-r--r--   0        0        0    23553 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_events.py
+-rw-r--r--   0        0        0      702 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_files.py
+-rw-r--r--   0        0        0    31826 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_helpers.py
+-rw-r--r--   0        0        0    16305 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_manager_deduplication.py
+-rw-r--r--   0        0        0    79706 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py
+-rw-r--r--   0        0        0    16943 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_modules_basic.py
+-rw-r--r--   0        0        0     2657 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_python_api.py
+-rw-r--r--   0        0        0     7144 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_regexes.py
+-rw-r--r--   0        0        0     2870 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_scan.py
+-rw-r--r--   0        0        0      706 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_scope.py
+-rw-r--r--   0        0        0     2175 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_target.py
+-rw-r--r--   0        0        0    13141 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_web.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/__init__.py
+-rw-r--r--   0        0        0     5344 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/base.py
+-rw-r--r--   0        0        0      664 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py
+-rw-r--r--   0        0        0      473 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_aggregate.py
+-rw-r--r--   0        0        0     2789 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py
+-rw-r--r--   0        0        0      546 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py
+-rw-r--r--   0        0        0    10606 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_asn.py
+-rw-r--r--   0        0        0     3098 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py
+-rw-r--r--   0        0        0     1207 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py
+-rw-r--r--   0        0        0     4805 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py
+-rw-r--r--   0        0        0     2795 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py
+-rw-r--r--   0        0        0     2397 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py
+-rw-r--r--   0        0        0     5599 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py
+-rw-r--r--   0        0        0     1045 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py
+-rw-r--r--   0        0        0     1101 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py
+-rw-r--r--   0        0        0     3984 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py
+-rw-r--r--   0        0        0      552 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py
+-rw-r--r--   0        0        0      907 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py
+-rw-r--r--   0        0        0     2282 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py
+-rw-r--r--   0        0        0      506 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_firebase.py
+-rw-r--r--   0        0        0     1312 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py
+-rw-r--r--   0        0        0     5051 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py
+-rw-r--r--   0        0        0     3551 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py
+-rw-r--r--   0        0        0      982 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_c99.py
+-rw-r--r--   0        0        0     3956 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_censys.py
+-rw-r--r--   0        0        0      636 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py
+-rw-r--r--   0        0        0      956 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py
+-rw-r--r--   0        0        0     2047 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py
+-rw-r--r--   0        0        0      564 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py
+-rw-r--r--   0        0        0     3362 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py
+-rw-r--r--   0        0        0      762 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py
+-rw-r--r--   0        0        0      717 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_crt.py
+-rw-r--r--   0        0        0      273 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_csv.py
+-rw-r--r--   0        0        0     2321 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py
+-rw-r--r--   0        0        0     3615 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py
+-rw-r--r--   0        0        0     1613 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py
+-rw-r--r--   0        0        0     1863 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_discord.py
+-rw-r--r--   0        0        0      952 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py
+-rw-r--r--   0        0        0    59749 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py
+-rw-r--r--   0        0        0    27988 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py
+-rw-r--r--   0        0        0     3907 2024-05-16 15:16:38.545855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py
+-rw-r--r--   0        0        0     8232 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py
+-rw-r--r--   0        0        0      461 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_emailformat.py
+-rw-r--r--   0        0        0      944 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_emails.py
+-rw-r--r--   0        0        0    14708 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py
+-rw-r--r--   0        0        0     2955 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py
+-rw-r--r--   0        0        0     7669 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py
+-rw-r--r--   0        0        0     2389 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py
+-rw-r--r--   0        0        0      445 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_fingerprintx.py
+-rw-r--r--   0        0        0     1946 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py
+-rw-r--r--   0        0        0     2040 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py
+-rw-r--r--   0        0        0     1656 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_git.py
+-rw-r--r--   0        0        0    12266 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py
+-rw-r--r--   0        0        0     3718 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py
+-rw-r--r--   0        0        0    24606 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py
+-rw-r--r--   0        0        0    35521 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py
+-rw-r--r--   0        0        0    11579 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py
+-rw-r--r--   0        0        0     3433 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py
+-rw-r--r--   0        0        0      609 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py
+-rw-r--r--   0        0        0     2702 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py
+-rw-r--r--   0        0        0     2155 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_http.py
+-rw-r--r--   0        0        0     4939 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py
+-rw-r--r--   0        0        0      249 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_human.py
+-rw-r--r--   0        0        0      665 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py
+-rw-r--r--   0        0        0     4086 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py
+-rw-r--r--   0        0        0     2879 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py
+-rw-r--r--   0        0        0     2231 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py
+-rw-r--r--   0        0        0     1123 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py
+-rw-r--r--   0        0        0      604 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py
+-rw-r--r--   0        0        0     2767 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py
+-rw-r--r--   0        0        0     1006 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_json.py
+-rw-r--r--   0        0        0     1641 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py
+-rw-r--r--   0        0        0     1711 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py
+-rw-r--r--   0        0        0      428 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_massdns.py
+-rw-r--r--   0        0        0     1532 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py
+-rw-r--r--   0        0        0     1030 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py
+-rw-r--r--   0        0        0     2305 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py
+-rw-r--r--   0        0        0     3618 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py
+-rw-r--r--   0        0        0     1116 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py
+-rw-r--r--   0        0        0     5609 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py
+-rw-r--r--   0        0        0     9402 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py
+-rw-r--r--   0        0        0     1160 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_otx.py
+-rw-r--r--   0        0        0     2142 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py
+-rw-r--r--   0        0        0    10680 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py
+-rw-r--r--   0        0        0     2190 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py
+-rw-r--r--   0        0        0      961 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py
+-rw-r--r--   0        0        0     1609 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py
+-rw-r--r--   0        0        0    14768 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_postman.py
+-rw-r--r--   0        0        0      184 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_python.py
+-rw-r--r--   0        0        0      750 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py
+-rw-r--r--   0        0        0      747 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py
+-rw-r--r--   0        0        0     1564 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_robots.py
+-rw-r--r--   0        0        0      537 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py
+-rw-r--r--   0        0        0      758 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py
+-rw-r--r--   0        0        0      713 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py
+-rw-r--r--   0        0        0     6220 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py
+-rw-r--r--   0        0        0     2321 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py
+-rw-r--r--   0        0        0      415 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_slack.py
+-rw-r--r--   0        0        0     2426 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py
+-rw-r--r--   0        0        0     1700 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_social.py
+-rw-r--r--   0        0        0     3121 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py
+-rw-r--r--   0        0        0     1866 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py
+-rw-r--r--   0        0        0      706 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py
+-rw-r--r--   0        0        0      610 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py
+-rw-r--r--   0        0        0     1116 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py
+-rw-r--r--   0        0        0      611 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py
+-rw-r--r--   0        0        0     1222 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_teams.py
+-rw-r--r--   0        0        0     7751 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py
+-rw-r--r--   0        0        0      489 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_threatminer.py
+-rw-r--r--   0        0        0    62527 2024-05-16 15:16:38.549855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py
+-rw-r--r--   0        0        0     1144 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py
+-rw-r--r--   0        0        0     2902 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py
+-rw-r--r--   0        0        0     2874 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py
+-rw-r--r--   0        0        0    15239 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py
+-rw-r--r--   0        0        0     3401 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py
+-rw-r--r--   0        0        0     1304 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py
+-rw-r--r--   0        0        0      936 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py
+-rw-r--r--   0        0        0      548 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py
+-rw-r--r--   0        0        0     2026 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py
+-rw-r--r--   0        0        0     1009 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py
+-rw-r--r--   0        0        0     1979 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py
+-rw-r--r--   0        0        0     1103 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/testsslcert.pem
+-rw-r--r--   0        0        0     1704 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/test/testsslkey.pem
+-rw-r--r--   0        0        0      476 2024-05-16 15:16:38.553855 bbot-1.1.8.3332rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0      764 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/ms_on_prem_subdomains.txt
+-rw-r--r--   0        0        0    32226 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0    17458 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/paramminer_headers.txt
+-rw-r--r--   0        0        0    54887 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/paramminer_parameters.txt
+-rw-r--r--   0        0        0     6068 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2024-05-16 15:16:38.557855 bbot-1.1.8.3332rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     2663 2024-05-16 15:16:53.601980 bbot-1.1.8.3332rc0/pyproject.toml
+-rw-r--r--   0        0        0    42361 1970-01-01 00:00:00.000000 bbot-1.1.8.3332rc0/PKG-INFO
```

### Comparing `bbot-1.1.8.3321rc0/LICENSE` & `bbot-1.1.8.3332rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/README.md` & `bbot-1.1.8.3332rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/agent/agent.py` & `bbot-1.1.8.3332rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/cli.py` & `bbot-1.1.8.3332rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/configurator/__init__.py` & `bbot-1.1.8.3332rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/configurator/args.py` & `bbot-1.1.8.3332rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/configurator/environ.py` & `bbot-1.1.8.3332rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/configurator/files.py` & `bbot-1.1.8.3332rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/errors.py` & `bbot-1.1.8.3332rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/event/base.py` & `bbot-1.1.8.3332rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/event/helpers.py` & `bbot-1.1.8.3332rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/flags.py` & `bbot-1.1.8.3332rc0/bbot/core/flags.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/async_helpers.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/async_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/cache.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/cloud.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/cloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/command.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import os
 import asyncio
 import logging
 import traceback
+from signal import SIGINT
 from subprocess import CompletedProcess, CalledProcessError
 
 from .misc import smart_decode, smart_encode
 
 log = logging.getLogger("bbot.core.helpers.command")
 
 
-async def run(self, *command, check=False, text=True, **kwargs):
+async def run(self, *command, check=False, text=True, idle_timeout=None, **kwargs):
     """Runs a command asynchronously and gets its output as a string.
 
     This method is a simple helper for executing a command and capturing its output.
     If an error occurs during execution, it can optionally raise an error or just log the stderr.
 
     Args:
         *command (str): The command to run as separate arguments.
         check (bool, optional): If set to True, raises an error if the subprocess exits with a non-zero status.
                                 Defaults to False.
         text (bool, optional): If set to True, decodes the subprocess output to string. Defaults to True.
+        idle_timeout (int, optional): Sets a limit on the number of seconds the process can run before throwing a TimeoutError
         **kwargs (dict): Additional keyword arguments for the subprocess.
 
     Returns:
         CompletedProcess: A completed process object with attributes for the command, return code, stdout, and stderr.
 
     Raises:
         CalledProcessError: If the subprocess exits with a non-zero status and `check=True`.
@@ -41,15 +43,23 @@
         proc_tracker.add(proc)
         try:
             if _input is not None:
                 if isinstance(_input, (list, tuple)):
                     _input = b"\n".join(smart_encode(i) for i in _input) + b"\n"
                 else:
                     _input = smart_encode(_input)
-            stdout, stderr = await proc.communicate(_input)
+
+            try:
+                if idle_timeout is not None:
+                    stdout, stderr = await asyncio.wait_for(proc.communicate(_input), timeout=idle_timeout)
+                else:
+                    stdout, stderr = await proc.communicate(_input)
+            except asyncio.exceptions.TimeoutError:
+                proc.send_signal(SIGINT)
+                raise
 
             # surface stderr
             if text:
                 if stderr is not None:
                     stderr = smart_decode(stderr)
                 if stdout is not None:
                     stdout = smart_decode(stdout)
@@ -61,25 +71,26 @@
                     log.warning(f"Stderr for run({command_str}):\n\t{stderr}")
 
             return CompletedProcess(command, proc.returncode, stdout, stderr)
         finally:
             proc_tracker.remove(proc)
 
 
-async def run_live(self, *command, check=False, text=True, **kwargs):
+async def run_live(self, *command, check=False, text=True, idle_timeout=None, **kwargs):
     """Runs a command asynchronously and iterates through its output line by line in realtime.
 
     This method is useful for executing a command and capturing its output on-the-fly, as it is generated.
     If an error occurs during execution, it can optionally raise an error or just log the stderr.
 
     Args:
         *command (str): The command to run as separate arguments.
         check (bool, optional): If set to True, raises an error if the subprocess exits with a non-zero status.
                                 Defaults to False.
         text (bool, optional): If set to True, decodes the subprocess output to string. Defaults to True.
+        idle_timeout (int, optional): Sets a limit on the number of seconds the process can remain idle (no lines sent to stdout) before throwing a TimeoutError
         **kwargs (dict): Additional keyword arguments for the subprocess.
 
     Yields:
         str or bytes: The output lines of the command, either as a decoded string (if `text=True`)
                       or as bytes (if `text=False`).
 
     Raises:
@@ -98,15 +109,21 @@
         try:
             input_task = None
             if _input is not None:
                 input_task = asyncio.create_task(_write_stdin(proc, _input))
 
             while 1:
                 try:
-                    line = await proc.stdout.readline()
+                    if idle_timeout is not None:
+                        line = await asyncio.wait_for(proc.stdout.readline(), timeout=idle_timeout)
+                    else:
+                        line = await proc.stdout.readline()
+                except asyncio.exceptions.TimeoutError:
+                    proc.send_signal(SIGINT)
+                    raise
                 except ValueError as e:
                     command_str = " ".join([str(c) for c in command])
                     log.warning(f"Error executing command {command_str}: {e}")
                     log.trace(traceback.format_exc())
                     continue
                 if not line:
                     break
```

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/diff.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/dns.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/files.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/helper.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/interactsh.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/logger.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/misc.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/modules.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/names_generator.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/ntlm.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/ratelimiter.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/ratelimiter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/regexes.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/url.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/validators.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/web.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.1.8.3332rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/core/logger/logger.py` & `bbot-1.1.8.3332rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/defaults.yml` & `bbot-1.1.8.3332rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ajaxpro.py` & `bbot-1.1.8.3332rc0/bbot/modules/ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/anubisdb.py` & `bbot-1.1.8.3332rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/azure_realm.py` & `bbot-1.1.8.3332rc0/bbot/modules/azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/azure_tenant.py` & `bbot-1.1.8.3332rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/baddns.py` & `bbot-1.1.8.3332rc0/bbot/modules/baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/baddns_zone.py` & `bbot-1.1.8.3332rc0/bbot/modules/baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/badsecrets.py` & `bbot-1.1.8.3332rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/base.py` & `bbot-1.1.8.3332rc0/bbot/modules/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bevigil.py` & `bbot-1.1.8.3332rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/binaryedge.py` & `bbot-1.1.8.3332rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_amazon.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_azure.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_file_enum.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_firebase.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bucket_google.py` & `bbot-1.1.8.3332rc0/bbot/modules/bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/builtwith.py` & `bbot-1.1.8.3332rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/bypass403.py` & `bbot-1.1.8.3332rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/c99.py` & `bbot-1.1.8.3332rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/censys.py` & `bbot-1.1.8.3332rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/certspotter.py` & `bbot-1.1.8.3332rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/chaos.py` & `bbot-1.1.8.3332rc0/bbot/modules/chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/code_repository.py` & `bbot-1.1.8.3332rc0/bbot/modules/code_repository.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/columbus.py` & `bbot-1.1.8.3332rc0/bbot/modules/columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/credshed.py` & `bbot-1.1.8.3332rc0/bbot/modules/credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/crt.py` & `bbot-1.1.8.3332rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/deadly/dastardly.py` & `bbot-1.1.8.3332rc0/bbot/modules/deadly/dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.1.8.3332rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.1.8.3332rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/deadly/vhost.py` & `bbot-1.1.8.3332rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/dehashed.py` & `bbot-1.1.8.3332rc0/bbot/modules/dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/digitorus.py` & `bbot-1.1.8.3332rc0/bbot/modules/digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.1.8.3332rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/dnsdumpster.py` & `bbot-1.1.8.3332rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/docker_pull.py` & `bbot-1.1.8.3332rc0/bbot/modules/docker_pull.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/dockerhub.py` & `bbot-1.1.8.3332rc0/bbot/modules/dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/dotnetnuke.py` & `bbot-1.1.8.3332rc0/bbot/modules/dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/emailformat.py` & `bbot-1.1.8.3332rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.1.8.3332rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/filedownload.py` & `bbot-1.1.8.3332rc0/bbot/modules/filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/fingerprintx.py` & `bbot-1.1.8.3332rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/fullhunt.py` & `bbot-1.1.8.3332rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/generic_ssrf.py` & `bbot-1.1.8.3332rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/git.py` & `bbot-1.1.8.3332rc0/bbot/modules/git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/git_clone.py` & `bbot-1.1.8.3332rc0/bbot/modules/git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/github_codesearch.py` & `bbot-1.1.8.3332rc0/bbot/modules/github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/github_org.py` & `bbot-1.1.8.3332rc0/bbot/modules/github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/github_workflows.py` & `bbot-1.1.8.3332rc0/bbot/modules/github_workflows.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/gitlab.py` & `bbot-1.1.8.3332rc0/bbot/modules/gitlab.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/gowitness.py` & `bbot-1.1.8.3332rc0/bbot/modules/gowitness.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import asyncio
 import sqlite3
+import multiprocessing
 from pathlib import Path
 from contextlib import suppress
 from shutil import copyfile, copymode
 
 from bbot.modules.base import BaseModule
 
 
@@ -15,23 +17,25 @@
         "version": "2.4.2",
         "threads": 4,
         "timeout": 10,
         "resolution_x": 1440,
         "resolution_y": 900,
         "output_path": "",
         "social": True,
+        "idle_timeout": 1800,
     }
     options_desc = {
-        "version": "gowitness version",
-        "threads": "threads used to run",
-        "timeout": "preflight check timeout",
-        "resolution_x": "screenshot resolution x",
-        "resolution_y": "screenshot resolution y",
-        "output_path": "where to save screenshots",
+        "version": "Gowitness version",
+        "threads": "How many gowitness threads to spawn - default is number of CPUs x 2",
+        "timeout": "Preflight check timeout",
+        "resolution_x": "Screenshot resolution x",
+        "resolution_y": "Screenshot resolution y",
+        "output_path": "Where to save screenshots",
         "social": "Whether to screenshot social media webpages",
+        "idle_timeout": "Skip the current gowitness batch if it stalls for longer than this many seconds",
     }
     deps_ansible = [
         {
             "name": "Install Chromium (Non-Debian)",
             "package": {"name": "chromium", "state": "present"},
             "become": True,
             "when": "ansible_facts['os_family'] != 'Debian'",
@@ -78,16 +82,19 @@
         },
     ]
     _batch_size = 100
     # gowitness accepts SOCIAL events up to distance 2, otherwise it is in-scope-only
     scope_distance_modifier = 2
 
     async def setup(self):
+        num_cpus = multiprocessing.cpu_count()
+        default_thread_count = min(20, num_cpus * 2)
         self.timeout = self.config.get("timeout", 10)
-        self.threads = self.config.get("threads", 4)
+        self.idle_timeout = self.config.get("idle_timeout", 1800)
+        self.threads = self.config.get("threads", default_thread_count)
         self.proxy = self.scan.config.get("http_proxy", "")
         self.resolution_x = self.config.get("resolution_x")
         self.resolution_y = self.config.get("resolution_y")
         self.visit_social = self.config.get("social", True)
         output_path = self.config.get("output_path")
         if output_path:
             self.base_path = Path(output_path) / "gowitness"
@@ -151,16 +158,21 @@
         for e in events:
             key = e.data
             if e.type == "SOCIAL":
                 key = e.data["url"]
             event_dict[key] = e
         stdin = "\n".join(list(event_dict))
 
-        async for line in self.run_process_live(self.command, input=stdin):
-            self.debug(line)
+        try:
+            async for line in self.run_process_live(self.command, input=stdin, idle_timeout=self.idle_timeout):
+                self.debug(line)
+        except asyncio.exceptions.TimeoutError:
+            urls_str = ",".join(event_dict)
+            self.warning(f"Gowitness timed out while visiting the following URLs: {urls_str}", trace=False)
+            return
 
         # emit web screenshots
         for filename, screenshot in self.new_screenshots.items():
             url = screenshot["url"]
             final_url = screenshot["final_url"]
             filename = screenshot["filename"]
             webscreenshot_data = {"filename": filename, "url": final_url}
@@ -208,14 +220,16 @@
         # resolution
         command += ["--resolution-x", str(self.resolution_x)]
         command += ["--resolution-y", str(self.resolution_y)]
         # input
         command += ["file", "-f", "-"]
         # threads
         command += ["--threads", str(self.threads)]
+        # timeout
+        command += ["--timeout", str(self.timeout)]
         return command
 
     @property
     def new_screenshots(self):
         screenshots = {}
         if self.db_path.is_file():
             with sqlite3.connect(str(self.db_path)) as con:
```

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/hackertarget.py` & `bbot-1.1.8.3332rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/host_header.py` & `bbot-1.1.8.3332rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/httpx.py` & `bbot-1.1.8.3332rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/hunt.py` & `bbot-1.1.8.3332rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/hunterio.py` & `bbot-1.1.8.3332rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/iis_shortnames.py` & `bbot-1.1.8.3332rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/internal/base.py` & `bbot-1.1.8.3332rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/internal/excavate.py` & `bbot-1.1.8.3332rc0/bbot/modules/internal/excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/internal/speculate.py` & `bbot-1.1.8.3332rc0/bbot/modules/internal/speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/internetdb.py` & `bbot-1.1.8.3332rc0/bbot/modules/internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ip2location.py` & `bbot-1.1.8.3332rc0/bbot/modules/ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ipneighbor.py` & `bbot-1.1.8.3332rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ipstack.py` & `bbot-1.1.8.3332rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/leakix.py` & `bbot-1.1.8.3332rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/masscan.py` & `bbot-1.1.8.3332rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/massdns.py` & `bbot-1.1.8.3332rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/myssl.py` & `bbot-1.1.8.3332rc0/bbot/modules/myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/newsletters.py` & `bbot-1.1.8.3332rc0/bbot/modules/newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/nmap.py` & `bbot-1.1.8.3332rc0/bbot/modules/nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/ntlm.py` & `bbot-1.1.8.3332rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/oauth.py` & `bbot-1.1.8.3332rc0/bbot/modules/oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/otx.py` & `bbot-1.1.8.3332rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/base.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/csv.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/csv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/discord.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/emails.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/http.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/human.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/human.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/json.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/neo4j.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/slack.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/slack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/splunk.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/subdomains.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/teams.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/web_report.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/output/websocket.py` & `bbot-1.1.8.3332rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.1.8.3332rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.1.8.3332rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/paramminer_headers.py` & `bbot-1.1.8.3332rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/passivetotal.py` & `bbot-1.1.8.3332rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/pgp.py` & `bbot-1.1.8.3332rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/postman.py` & `bbot-1.1.8.3332rc0/bbot/modules/postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/rapiddns.py` & `bbot-1.1.8.3332rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/report/affiliates.py` & `bbot-1.1.8.3332rc0/bbot/modules/report/affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/report/asn.py` & `bbot-1.1.8.3332rc0/bbot/modules/report/asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/riddler.py` & `bbot-1.1.8.3332rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/robots.py` & `bbot-1.1.8.3332rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/secretsdb.py` & `bbot-1.1.8.3332rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/securitytrails.py` & `bbot-1.1.8.3332rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/shodan_dns.py` & `bbot-1.1.8.3332rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/sitedossier.py` & `bbot-1.1.8.3332rc0/bbot/modules/sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/skymem.py` & `bbot-1.1.8.3332rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/smuggler.py` & `bbot-1.1.8.3332rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/social.py` & `bbot-1.1.8.3332rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/sslcert.py` & `bbot-1.1.8.3332rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/subdomaincenter.py` & `bbot-1.1.8.3332rc0/bbot/modules/subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/sublist3r.py` & `bbot-1.1.8.3332rc0/bbot/modules/sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/telerik.py` & `bbot-1.1.8.3332rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/bucket.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/bucket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/github.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/portscanner.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/portscanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/shodan.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/shodan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/subdomain_enum.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/subdomain_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/templates/webhook.py` & `bbot-1.1.8.3332rc0/bbot/modules/templates/webhook.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/threatminer.py` & `bbot-1.1.8.3332rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/trufflehog.py` & `bbot-1.1.8.3332rc0/bbot/modules/trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/url_manipulation.py` & `bbot-1.1.8.3332rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/urlscan.py` & `bbot-1.1.8.3332rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/viewdns.py` & `bbot-1.1.8.3332rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/virustotal.py` & `bbot-1.1.8.3332rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/wafw00f.py` & `bbot-1.1.8.3332rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/wappalyzer.py` & `bbot-1.1.8.3332rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/wayback.py` & `bbot-1.1.8.3332rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/modules/zoomeye.py` & `bbot-1.1.8.3332rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scanner/dispatcher.py` & `bbot-1.1.8.3332rc0/bbot/scanner/dispatcher.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scanner/manager.py` & `bbot-1.1.8.3332rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scanner/scanner.py` & `bbot-1.1.8.3332rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scanner/stats.py` & `bbot-1.1.8.3332rc0/bbot/scanner/stats.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scanner/target.py` & `bbot-1.1.8.3332rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/scripts/docs.py` & `bbot-1.1.8.3332rc0/bbot/scripts/docs.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/bbot_fixtures.py` & `bbot-1.1.8.3332rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/conftest.py` & `bbot-1.1.8.3332rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/run_tests.sh` & `bbot-1.1.8.3332rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test.conf` & `bbot-1.1.8.3332rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test__module__tests.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test__module__tests.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_agent.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cli.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_cloud_helpers.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_command.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+import time
 from ..bbot_fixtures import *
 from subprocess import CalledProcessError
 
 
 @pytest.mark.asyncio
 async def test_command(bbot_scanner, bbot_config):
     scan1 = bbot_scanner(config=bbot_config)
 
+    # test timeouts
+    command = ["sleep", "3"]
+    start = time.time()
+    with pytest.raises(asyncio.exceptions.TimeoutError):
+        await scan1.helpers.run(command, idle_timeout=1)
+    end = time.time()
+    elapsed = end - start
+    assert 0 < elapsed < 2
+
+    start = time.time()
+    with pytest.raises(asyncio.exceptions.TimeoutError):
+        async for line in scan1.helpers.run_live(command, idle_timeout=1):
+            print(line)
+    end = time.time()
+    elapsed = end - start
+    assert 0 < elapsed < 2
+
     # run
     assert "plumbus\n" == (await scan1.helpers.run(["echo", "plumbus"])).stdout
     assert b"plumbus\n" == (await scan1.helpers.run(["echo", "plumbus"], text=False)).stdout
     result = (await scan1.helpers.run(["cat"], input="some\nrandom\nstdin")).stdout
     assert result.splitlines() == ["some", "random", "stdin"]
     result = (await scan1.helpers.run(["cat"], input=b"some\nrandom\nstdin", text=False)).stdout
     assert result.splitlines() == [b"some", b"random", b"stdin"]
```

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_depsinstaller.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_dns.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_events.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_files.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_helpers.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_deduplication.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_manager_deduplication.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_manager_scope_accuracy.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_modules_basic.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_python_api.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_regexes.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scan.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_scope.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_target.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_1/test_web.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_1/test_web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/base.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_affiliates.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ajaxpro.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asn.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_asn.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_asset_inventory.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_azure_realm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_baddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_baddns_zone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_amazon.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_file_enum.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bucket_google.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_c99.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_censys.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_chaos.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_code_repository.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_columbus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_credshed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_crt.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dastardly.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dehashed.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_digitorus.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_discord.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_discord.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_docker_pull.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dockerhub.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_dotnetnuke.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_emails.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_emails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_excavate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_filedownload.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_git.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_git_clone.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_codesearch.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_org.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_github_workflows.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_gitlab.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_gowitness.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_http.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_internetdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ip2location.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_json.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_json.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_myssl.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_newsletters.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_nmap.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_oauth.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_otx.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_postman.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_postman.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_robots.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sitedossier.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_social.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_speculate.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_splunk.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_subdomaincenter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_subdomains.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_sublist3r.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_teams.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_teams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_trufflehog.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_web_report.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py` & `bbot-1.1.8.3332rc0/bbot/test/test_step_2/module_tests/test_module_zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/testsslcert.pem` & `bbot-1.1.8.3332rc0/bbot/test/testsslcert.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/test/testsslkey.pem` & `bbot-1.1.8.3332rc0/bbot/test/testsslkey.pem`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/ms_on_prem_subdomains.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/ms_on_prem_subdomains.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/nameservers.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_headers.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/paramminer_headers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/paramminer_parameters.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/paramminer_parameters.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.1.8.3332rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.1.8.3332rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.1.8.3321rc0/pyproject.toml` & `bbot-1.1.8.3332rc0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.1.8.3321rc"
+version = "v1.1.8.3332rc"
 description = "OSINT automation for hackers."
 authors = [
     "TheTechromancer",
     "Paul Mueller",
 ]
 license = "GPL-3.0"
 readme = "README.md"
```

### Comparing `bbot-1.1.8.3321rc0/PKG-INFO` & `bbot-1.1.8.3332rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.1.8.3321rc0
+Version: 1.1.8.3332rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Keywords: python,cli,automation,osint,neo4j,scanner,python-library,hacking,recursion,pentesting,recon,command-line-tool,bugbounty,subdomains,security-tools,subdomain-scanner,osint-framework,attack-surface,subdomain-enumeration,osint-tool
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

