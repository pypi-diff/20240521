# Comparing `tmp/puncia-0.15.tar.gz` & `tmp/puncia-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puncia-0.15.tar", last modified: Tue Mar 19 02:05:48 2024, max compression
+gzip compressed data, was "puncia-0.16.tar", last modified: Tue May 21 19:52:48 2024, max compression
```

## Comparing `puncia-0.15.tar` & `puncia-0.16.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-03-19 02:05:48.559876 puncia-0.15/
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     5861 2024-03-19 02:05:48.559876 puncia-0.15/PKG-INFO
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     5245 2024-03-19 02:05:33.000000 puncia-0.15/README.md
-drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-03-19 02:05:48.555876 puncia-0.15/puncia/
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        0 2023-09-03 18:22:30.000000 puncia-0.15/puncia/__init__.py
--rwxrwxr-x   0 glatisant  (1000) glatisant  (1000)     4422 2024-03-19 02:05:33.000000 puncia-0.15/puncia/__main__.py
-drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-03-19 02:05:48.559876 puncia-0.15/puncia.egg-info/
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     5861 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/PKG-INFO
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)      238 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/SOURCES.txt
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        1 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/dependency_links.txt
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)       49 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/entry_points.txt
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        9 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/requires.txt
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        7 2024-03-19 02:05:48.000000 puncia-0.15/puncia.egg-info/top_level.txt
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)       38 2024-03-19 02:05:48.559876 puncia-0.15/setup.cfg
--rw-rw-r--   0 glatisant  (1000) glatisant  (1000)      885 2024-03-19 02:05:33.000000 puncia-0.15/setup.py
+drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-05-21 19:52:48.958050 puncia-0.16/
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     1105 2024-03-25 13:34:16.000000 puncia-0.16/LICENSE
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     7753 2024-05-21 19:52:48.954050 puncia-0.16/PKG-INFO
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     7119 2024-05-21 19:26:51.000000 puncia-0.16/README.md
+drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-05-21 19:52:48.954050 puncia-0.16/puncia/
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        0 2023-09-03 18:22:30.000000 puncia-0.16/puncia/__init__.py
+-rwxrwxr-x   0 glatisant  (1000) glatisant  (1000)     5972 2024-05-21 19:50:16.000000 puncia-0.16/puncia/__main__.py
+drwxrwxr-x   0 glatisant  (1000) glatisant  (1000)        0 2024-05-21 19:52:48.954050 puncia-0.16/puncia.egg-info/
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)     7753 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/PKG-INFO
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)      246 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/SOURCES.txt
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        1 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/dependency_links.txt
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)       49 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/entry_points.txt
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        9 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/requires.txt
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)        7 2024-05-21 19:52:48.000000 puncia-0.16/puncia.egg-info/top_level.txt
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)       38 2024-05-21 19:52:48.958050 puncia-0.16/setup.cfg
+-rw-rw-r--   0 glatisant  (1000) glatisant  (1000)      904 2024-05-21 17:43:08.000000 puncia-0.16/setup.py
```

### Comparing `puncia-0.15/PKG-INFO` & `puncia-0.16/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: puncia
-Version: 0.15
-Summary: The Panthera(P.)uncia of Cybersecurity - Official CLI utility for Subdomain Center & Exploit Observer
-Home-page: https://github.com/ARPSyndicate/puncia
-Author: A.R.P. Syndicate
-Author-email: ayush@arpsyndicate.io
-License: UNKNOWN
-Project-URL: A.R.P. Syndicate, https://www.arpsyndicate.io
-Project-URL: Subdomain Center, https://subdomain.center
-Project-URL: Exploit Observer, https://exploit.observer
-Keywords: subdomains subdomain exploits exploit arpsyndicate panthera uncia puncia snow leopard
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-
 #  The Panthera(P.)uncia of Cybersecurity 
 ### Official CLI utility for Subdomain Center & Exploit Observer
 
 [![Downloads](https://pepy.tech/badge/puncia)](https://pepy.tech/project/puncia)
 <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
 <img alt="GitHub stars" src="https://img.shields.io/github/stars/ARPSyndicate/puncia"> 
 <br>
@@ -41,46 +26,57 @@
 {
     "subdomain": [
         "domainA.com",
         "domainB.com"
     ],
     "exploit": [
         "eoidentifierA",
-        "eoidentifierA"
+        "eoidentifierB"
     ]
 }
 ```
 
 ## Supported EOIdentifiers
-1. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
-2. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
-3. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
-4. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
-5. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
-6. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2) 
+1. A.R.P. Syndicate Vulnerability & Exploit Data Aggregation System (VEDAS) - [`puncia exploit VEDAS:OBLIVIONHAWK`](https://api.exploit.observer/?keyword=VEDAS:OBLIVIONHAWK) 
+2. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
+3. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
+4. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
+5. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
+6. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
 7. CSA Global Security Database (GSD) - [`puncia exploit GSD-2021-3450`](https://api.exploit.observer/?keyword=GSD-2021-3450)
-8. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
-9. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
-10. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
-11. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
-12. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
-13. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
-14. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
-15. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
-16. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
-17. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
-18. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
-19. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
-20. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
-21. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
+8. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2)
+9. GitHub Commits (GHCOMMIT) - [`puncia exploit GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00`](https://api.exploit.observer/?keyword=GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00) 
+10. Veracode SourceClear Vulnerability Database (SRCCLR-SID) - [`puncia exploit SRCCLR-SID-3173`](https://api.exploit.observer/?keyword=SRCCLR-SID-3173)
+11. Snyk Vulnerability Database (SNYK) - [`puncia exploit SNYK-JAVA-ORGCLOJURE-5740378`](https://api.exploit.observer/?keyword=SNYK-JAVA-ORGCLOJURE-5740378)
+12. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
+13. 0Day Today (0DAY-ID) - [`puncia exploit 0DAY-ID-24705`](https://api.exploit.observer/?keyword=0DAY-ID-24705)
+14. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
+15. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
+16. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
+17. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
+18. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
+19. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
+20. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
+21. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
+22. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
+23. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
+24. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
+25. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
+26. Zero Science Lab (ZSL) - [`puncia exploit ZSL-2022-5743`](https://api.exploit.observer/?keyword=ZSL-2022-5743)
+27. VARIoT Exploits (VAR-E) - [`puncia exploit VAR-E-201704-0525`](https://api.exploit.observer/?keyword=VAR-E-201704-0525)
+28. VARIoT Vulnerabilities (VAR) - [`puncia exploit VAR-202404-0085`](https://api.exploit.observer/?keyword=VAR-202404-0085)
+29. Russian VIDs with no associated CVEs (^RU_NON_CVE) - [`puncia exploit ^RU_NON_CVE`](http://api.exploit.observer/russia/noncve)<br>
+30. Chinese VIDs with no associated CVEs (^CN_NON_CVE) - [`puncia exploit ^CN_NON_CVE`](http://api.exploit.observer/china/noncve)<br>
+31. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
 
 
 ## Noteworthy Mentions
+- [Around 1000 exploitable cybersecurity vulnerabilities that MITRE & NIST ‘might’ have missed but China or Russia didn’t.](https://blog.arpsyndicate.io/over-a-1000-vulnerabilities-that-mitre-nist-might-have-missed-but-china-or-russia-did-not-871b2364a526)
+- [Utilizing GitHub Actions for gathering Subdomain & Exploit Intelligence](https://blog.arpsyndicate.io/utilizing-github-actions-for-gathering-subdomain-exploit-intelligence-bbc79c19bb85)
 - [Introducing Exploit Observer — More than Shodan Exploits, Less than Vulners](https://blog.arpsyndicate.io/introducing-exploit-observer-more-than-shodan-exploits-less-than-vulners-23eaea466e4a)
 - [PUNCIA — The Panthera(P.)uncia of Cybersecurity](https://blog.arpsyndicate.io/puncia-the-panthera-p-uncia-of-cybersecurity-ft-puncia-subdomain-center-exploit-observer-9a9d8cca9576)
 - [Subdomain Enumeration Tool Face-off - 2023 Edition](https://blog.blacklanternsecurity.com/p/subdomain-enumeration-tool-face-off-4e5)
 
 ## More from [A.R.P. Syndicate](https://www.arpsyndicate.io)
 - [Attack Surface Management](https://asm.arpsyndicate.io)
 - [Open Source Intelligence](https://asm.arpsyndicate.io/intelligence.html)
-- [Free Vulnerability Assessment Report](https://asm.arpsyndicate.io/free-vulnerability-scanning.html)
-
+- [Free Vulnerability Assessment Report](https://asm.arpsyndicate.io/free-vulnerability-scanning.html)
```

### Comparing `puncia-0.15/README.md` & `puncia-0.16/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: puncia
+Version: 0.16
+Summary: The Panthera(P.)uncia of Cybersecurity - Official CLI utility for Subdomain Center & Exploit Observer
+Home-page: https://github.com/ARPSyndicate/puncia
+Author: A.R.P. Syndicate
+Author-email: ayush@arpsyndicate.io
+License: MIT
+Project-URL: A.R.P. Syndicate, https://www.arpsyndicate.io
+Project-URL: Subdomain Center, https://subdomain.center
+Project-URL: Exploit Observer, https://exploit.observer
+Keywords: subdomains subdomain exploits exploit arpsyndicate panthera uncia puncia snow leopard
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 #  The Panthera(P.)uncia of Cybersecurity 
 ### Official CLI utility for Subdomain Center & Exploit Observer
 
 [![Downloads](https://pepy.tech/badge/puncia)](https://pepy.tech/project/puncia)
 <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
 <img alt="GitHub stars" src="https://img.shields.io/github/stars/ARPSyndicate/puncia"> 
 <br>
@@ -26,45 +42,58 @@
 {
     "subdomain": [
         "domainA.com",
         "domainB.com"
     ],
     "exploit": [
         "eoidentifierA",
-        "eoidentifierA"
+        "eoidentifierB"
     ]
 }
 ```
 
 ## Supported EOIdentifiers
-1. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
-2. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
-3. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
-4. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
-5. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
-6. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2) 
+1. A.R.P. Syndicate Vulnerability & Exploit Data Aggregation System (VEDAS) - [`puncia exploit VEDAS:OBLIVIONHAWK`](https://api.exploit.observer/?keyword=VEDAS:OBLIVIONHAWK) 
+2. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
+3. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
+4. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
+5. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
+6. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
 7. CSA Global Security Database (GSD) - [`puncia exploit GSD-2021-3450`](https://api.exploit.observer/?keyword=GSD-2021-3450)
-8. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
-9. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
-10. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
-11. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
-12. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
-13. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
-14. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
-15. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
-16. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
-17. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
-18. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
-19. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
-20. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
-21. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
+8. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2)
+9. GitHub Commits (GHCOMMIT) - [`puncia exploit GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00`](https://api.exploit.observer/?keyword=GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00) 
+10. Veracode SourceClear Vulnerability Database (SRCCLR-SID) - [`puncia exploit SRCCLR-SID-3173`](https://api.exploit.observer/?keyword=SRCCLR-SID-3173)
+11. Snyk Vulnerability Database (SNYK) - [`puncia exploit SNYK-JAVA-ORGCLOJURE-5740378`](https://api.exploit.observer/?keyword=SNYK-JAVA-ORGCLOJURE-5740378)
+12. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
+13. 0Day Today (0DAY-ID) - [`puncia exploit 0DAY-ID-24705`](https://api.exploit.observer/?keyword=0DAY-ID-24705)
+14. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
+15. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
+16. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
+17. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
+18. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
+19. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
+20. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
+21. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
+22. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
+23. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
+24. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
+25. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
+26. Zero Science Lab (ZSL) - [`puncia exploit ZSL-2022-5743`](https://api.exploit.observer/?keyword=ZSL-2022-5743)
+27. VARIoT Exploits (VAR-E) - [`puncia exploit VAR-E-201704-0525`](https://api.exploit.observer/?keyword=VAR-E-201704-0525)
+28. VARIoT Vulnerabilities (VAR) - [`puncia exploit VAR-202404-0085`](https://api.exploit.observer/?keyword=VAR-202404-0085)
+29. Russian VIDs with no associated CVEs (^RU_NON_CVE) - [`puncia exploit ^RU_NON_CVE`](http://api.exploit.observer/russia/noncve)<br>
+30. Chinese VIDs with no associated CVEs (^CN_NON_CVE) - [`puncia exploit ^CN_NON_CVE`](http://api.exploit.observer/china/noncve)<br>
+31. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
 
 
 ## Noteworthy Mentions
+- [Around 1000 exploitable cybersecurity vulnerabilities that MITRE & NIST ‘might’ have missed but China or Russia didn’t.](https://blog.arpsyndicate.io/over-a-1000-vulnerabilities-that-mitre-nist-might-have-missed-but-china-or-russia-did-not-871b2364a526)
+- [Utilizing GitHub Actions for gathering Subdomain & Exploit Intelligence](https://blog.arpsyndicate.io/utilizing-github-actions-for-gathering-subdomain-exploit-intelligence-bbc79c19bb85)
 - [Introducing Exploit Observer — More than Shodan Exploits, Less than Vulners](https://blog.arpsyndicate.io/introducing-exploit-observer-more-than-shodan-exploits-less-than-vulners-23eaea466e4a)
 - [PUNCIA — The Panthera(P.)uncia of Cybersecurity](https://blog.arpsyndicate.io/puncia-the-panthera-p-uncia-of-cybersecurity-ft-puncia-subdomain-center-exploit-observer-9a9d8cca9576)
 - [Subdomain Enumeration Tool Face-off - 2023 Edition](https://blog.blacklanternsecurity.com/p/subdomain-enumeration-tool-face-off-4e5)
 
 ## More from [A.R.P. Syndicate](https://www.arpsyndicate.io)
 - [Attack Surface Management](https://asm.arpsyndicate.io)
 - [Open Source Intelligence](https://asm.arpsyndicate.io/intelligence.html)
-- [Free Vulnerability Assessment Report](https://asm.arpsyndicate.io/free-vulnerability-scanning.html)
+- [Free Vulnerability Assessment Report](https://asm.arpsyndicate.io/free-vulnerability-scanning.html)
+
```

### Comparing `puncia-0.15/puncia/__main__.py` & `puncia-0.16/puncia/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,36 +4,56 @@
 import json
 import time
 import re
 
 API_URLS = {
     "subdomain": "http://api.subdomain.center/?domain=",
     "exploit": "http://api.exploit.observer/?keyword=",
+    "russia": "http://api.exploit.observer/russia/",
+    "china": "http://api.exploit.observer/china/",
 }
 
 
-def query_api(mode, query, output_file=None):
-    time.sleep(3)
+def query_api(mode, query, output_file=None, cid=None):
+    time.sleep(6)
     url = API_URLS.get(mode)
+    if "^" in query:
+        if query == "^RU_NON_CVE":
+            url = API_URLS.get("russia")
+            query = "noncve"
+            mode = "spec_exploit"
+            cid = "Russian VIDs with no associated CVEs"
+        if query == "^CN_NON_CVE":
+            url = API_URLS.get("china")
+            query = "noncve"
+            mode = "spec_exploit"
+            cid = "Chinese VIDs with no associated CVEs"
     if not url:
         sys.exit("Invalid Mode")
 
     response = requests.get(url + query).json()
     if not response:
         print("Null response from the API")
         return
     result = json.dumps(response, indent=4, sort_keys=True)
     print(result)
-
+    if mode in ["spec_exploit"]:
+        for reurl in response:
+            query_api(
+                "exploit",
+                reurl.replace("https://api.exploit.observer/?keyword=", ""),
+                output_file,
+                cid,
+            )
+        return
     if output_file:
         existing_data = {}
         if os.path.isfile(output_file):
             with open(output_file, "r") as f:
                 existing_data = json.load(f)
-
         if mode == "subdomain":
             if len(existing_data) == 0:
                 existing_data = []
             existing_data.extend(response)
             existing_data = list(set(existing_data))
         elif mode == "exploit":
             if "entries" in existing_data and len(existing_data["entries"]) > 0:
@@ -42,38 +62,54 @@
                     existing_data_entries = existing_data["entries"].get(lang, [])
                     existing_data["entries"][lang] = list(
                         set(existing_data_entries + response_entries)
                     )
                     existing_data["entries"][lang].sort()
             else:
                 existing_data = response
+            if "clusters" in existing_data:
+                existing_data_clusters = existing_data.get("clusters", [])
+                existing_data_clusters.extend(response.get("clusters", []))
+                existing_data["clusters"] = list(set(existing_data_clusters))
+                existing_data["clusters"].sort()
             total_entries = 0
             for lang in existing_data["entries"]:
                 total_entries = len(existing_data["entries"][lang]) + total_entries
+            if "priority" in existing_data:
+                existing_data["priority"] = (
+                    response.get("priority", 1) + existing_data["priority"]
+                ) / 2
             if len(existing_data["description"]) > 0:
                 if "description" in response and len(response["description"]) > 0:
                     existing_data["description"] = response["description"]
                 existing_data["description"] = re.sub(
                     r"\b(\d+)\s+(?:entries in)\b",
                     str(total_entries) + " entries in",
                     existing_data["description"],
                 )
                 existing_data["description"] = re.sub(
                     r"\b(\d+)\s+(?:file formats)\b",
                     str(len(existing_data["entries"])) + " file formats",
                     existing_data["description"],
                 )
+                if cid:
+                    existing_data["description"] = re.sub(
+                        r"(?<=related to\s)[^.]+(?=\.)",
+                        cid,
+                        existing_data["description"],
+                    )
+
         with open(output_file, "w") as f:
             json.dump(existing_data, f, indent=4, sort_keys=True)
 
 
 def main():
     try:
         print("---------")
-        print("Panthera(P.)uncia [v0.15]")
+        print("Panthera(P.)uncia [v0.16]")
         print("A.R.P. Syndicate [https://arpsyndicate.io]")
         print("Subdomain Center [https://subdomain.center]")
         print("Exploit Observer [https://exploit.observer]")
         print("---------")
 
         if len(sys.argv) < 3:
             sys.exit(
```

### Comparing `puncia-0.15/puncia.egg-info/PKG-INFO` & `puncia-0.16/puncia.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: puncia
-Version: 0.15
+Version: 0.16
 Summary: The Panthera(P.)uncia of Cybersecurity - Official CLI utility for Subdomain Center & Exploit Observer
 Home-page: https://github.com/ARPSyndicate/puncia
 Author: A.R.P. Syndicate
 Author-email: ayush@arpsyndicate.io
-License: UNKNOWN
+License: MIT
 Project-URL: A.R.P. Syndicate, https://www.arpsyndicate.io
 Project-URL: Subdomain Center, https://subdomain.center
 Project-URL: Exploit Observer, https://exploit.observer
 Keywords: subdomains subdomain exploits exploit arpsyndicate panthera uncia puncia snow leopard
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 #  The Panthera(P.)uncia of Cybersecurity 
 ### Official CLI utility for Subdomain Center & Exploit Observer
 
 [![Downloads](https://pepy.tech/badge/puncia)](https://pepy.tech/project/puncia)
 <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
 <img alt="GitHub stars" src="https://img.shields.io/github/stars/ARPSyndicate/puncia"> 
@@ -41,44 +42,56 @@
 {
     "subdomain": [
         "domainA.com",
         "domainB.com"
     ],
     "exploit": [
         "eoidentifierA",
-        "eoidentifierA"
+        "eoidentifierB"
     ]
 }
 ```
 
 ## Supported EOIdentifiers
-1. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
-2. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
-3. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
-4. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
-5. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
-6. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2) 
+1. A.R.P. Syndicate Vulnerability & Exploit Data Aggregation System (VEDAS) - [`puncia exploit VEDAS:OBLIVIONHAWK`](https://api.exploit.observer/?keyword=VEDAS:OBLIVIONHAWK) 
+2. Common Vulnerabilities and Exposures (CVE) - [`puncia exploit CVE-2021-3450`](https://api.exploit.observer/?keyword=CVE-2021-3450) 
+3. Russian Data Bank of Information Security Threats (BDU) - [`puncia exploit BDU:2024-00390`](https://api.exploit.observer/?keyword=BDU:2024-00390)
+4. China National Vulnerability Database (CNVD) - [`puncia exploit CNVD-2024-02713`](https://api.exploit.observer/?keyword=CNVD-2024-02713)
+5. China National Vulnerability Database of Information Security (CNNVD) - [`puncia exploit CNNVD-202312-2255`](https://api.exploit.observer/?keyword=CNNVD-202312-2255)
+6. Japan Vulnerability Notes iPedia (JVNDB) - [`puncia exploit JVNDB-2023-006199`](https://api.exploit.observer/?keyword=JVNDB-2023-006199) 
 7. CSA Global Security Database (GSD) - [`puncia exploit GSD-2021-3450`](https://api.exploit.observer/?keyword=GSD-2021-3450)
-8. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
-9. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
-10. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
-11. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
-12. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
-13. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
-14. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
-15. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
-16. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
-17. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
-18. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
-19. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
-20. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
-21. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
+8. GitHub Security Advisories (GHSA) - [`puncia exploit GHSA-wfh5-x68w-hvw2`](https://api.exploit.observer/?keyword=GHSA-wfh5-x68w-hvw2)
+9. GitHub Commits (GHCOMMIT) - [`puncia exploit GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00`](https://api.exploit.observer/?keyword=GHCOMMIT-102448040d5132460e3b0013e03ebedec0677e00) 
+10. Veracode SourceClear Vulnerability Database (SRCCLR-SID) - [`puncia exploit SRCCLR-SID-3173`](https://api.exploit.observer/?keyword=SRCCLR-SID-3173)
+11. Snyk Vulnerability Database (SNYK) - [`puncia exploit SNYK-JAVA-ORGCLOJURE-5740378`](https://api.exploit.observer/?keyword=SNYK-JAVA-ORGCLOJURE-5740378)
+12. OffSec Exploit Database (EDB) - [`puncia exploit EDB-10102`](https://api.exploit.observer/?keyword=EDB-10102)
+13. 0Day Today (0DAY-ID) - [`puncia exploit 0DAY-ID-24705`](https://api.exploit.observer/?keyword=0DAY-ID-24705)
+14. Knownsec Seebug (SSVID) - [`puncia exploit SSVID-99817`](https://api.exploit.observer/?keyword=SSVID-99817)
+15. Trend Micro Zero Day Initiative (ZDI) - [`puncia exploit ZDI-23-1714`](https://api.exploit.observer/?keyword=ZDI-23-1714) 
+16. Packet Storm Security (PSS) - [`puncia exploit PSS-170615`](https://api.exploit.observer/?keyword=PSS-170615) 
+17. CXSecurity World Laboratory of Bugtraq (WLB) - [`puncia exploit WLB-2024010058`](https://api.exploit.observer/?keyword=WLB-2024010058)
+18. Rapid7 Metasploit Framework (MSF) - [`puncia exploit MSF/auxiliary_admin/2wire/xslt_password_reset`](https://api.exploit.observer/?keyword=MSF/auxiliary_admin/2wire/xslt_password_reset)
+19. ProjectDiscovery Nuclei (PD) - [`puncia exploit PD/http/cves/2020/CVE-2020-12720`](https://api.exploit.observer/?keyword=PD/http/cves/2020/CVE-2020-12720) 
+20. Hackerone Hacktivity (H1) - [`puncia exploit H1-2230915`](https://api.exploit.observer/?keyword=H1-2230915)
+21. Cisco Talos (TALOS) - [`puncia exploit TALOS-2023-1896`](https://api.exploit.observer/?keyword=TALOS-2023-1896)
+22. ProtectAI Huntr (HUNTR) - [`puncia exploit HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5`](https://api.exploit.observer/?keyword=HUNTR-001d1c29-805a-4035-93bb-71a0e81da3e5)
+23. WP Engine WPScan (WPSCAN) - [`puncia exploit WPSCAN-52568abd-c509-411e-8391-c75e7613eb42`](https://api.exploit.observer/?keyword=WPSCAN-52568abd-c509-411e-8391-c75e7613eb42)
+24. Defiant Wordfence (WORDFENCE) - [`puncia exploit WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85`](https://api.exploit.observer/?keyword=WORDFENCE-00086b84-c1ec-447a-a536-1c73eac1cc85)
+25. YouTube (YT) - [`puncia exploit YT/ccqjhUmwLCk`](https://api.exploit.observer/?keyword=YT/ccqjhUmwLCk)
+26. Zero Science Lab (ZSL) - [`puncia exploit ZSL-2022-5743`](https://api.exploit.observer/?keyword=ZSL-2022-5743)
+27. VARIoT Exploits (VAR-E) - [`puncia exploit VAR-E-201704-0525`](https://api.exploit.observer/?keyword=VAR-E-201704-0525)
+28. VARIoT Vulnerabilities (VAR) - [`puncia exploit VAR-202404-0085`](https://api.exploit.observer/?keyword=VAR-202404-0085)
+29. Russian VIDs with no associated CVEs (^RU_NON_CVE) - [`puncia exploit ^RU_NON_CVE`](http://api.exploit.observer/russia/noncve)<br>
+30. Chinese VIDs with no associated CVEs (^CN_NON_CVE) - [`puncia exploit ^CN_NON_CVE`](http://api.exploit.observer/china/noncve)<br>
+31. Technologies/Keywords (No Prefix) - [`puncia exploit grafana`](https://api.exploit.observer/?keyword=grafana)<br>
 
 
 ## Noteworthy Mentions
+- [Around 1000 exploitable cybersecurity vulnerabilities that MITRE & NIST ‘might’ have missed but China or Russia didn’t.](https://blog.arpsyndicate.io/over-a-1000-vulnerabilities-that-mitre-nist-might-have-missed-but-china-or-russia-did-not-871b2364a526)
+- [Utilizing GitHub Actions for gathering Subdomain & Exploit Intelligence](https://blog.arpsyndicate.io/utilizing-github-actions-for-gathering-subdomain-exploit-intelligence-bbc79c19bb85)
 - [Introducing Exploit Observer — More than Shodan Exploits, Less than Vulners](https://blog.arpsyndicate.io/introducing-exploit-observer-more-than-shodan-exploits-less-than-vulners-23eaea466e4a)
 - [PUNCIA — The Panthera(P.)uncia of Cybersecurity](https://blog.arpsyndicate.io/puncia-the-panthera-p-uncia-of-cybersecurity-ft-puncia-subdomain-center-exploit-observer-9a9d8cca9576)
 - [Subdomain Enumeration Tool Face-off - 2023 Edition](https://blog.blacklanternsecurity.com/p/subdomain-enumeration-tool-face-off-4e5)
 
 ## More from [A.R.P. Syndicate](https://www.arpsyndicate.io)
 - [Attack Surface Management](https://asm.arpsyndicate.io)
 - [Open Source Intelligence](https://asm.arpsyndicate.io/intelligence.html)
```

### Comparing `puncia-0.15/setup.py` & `puncia-0.16/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="puncia",
-    version="0.15",
+    version="0.16",
     author="A.R.P. Syndicate",
     author_email="ayush@arpsyndicate.io",
     keywords="subdomains subdomain exploits exploit arpsyndicate panthera uncia puncia snow leopard",
     url="https://github.com/ARPSyndicate/puncia",
     project_urls={
         "A.R.P. Syndicate": "https://www.arpsyndicate.io",
         "Subdomain Center": "https://subdomain.center",
         "Exploit Observer": "https://exploit.observer",
     },
+    license="MIT",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     description="The Panthera(P.)uncia of Cybersecurity - Official CLI utility for Subdomain Center & Exploit Observer",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
```

