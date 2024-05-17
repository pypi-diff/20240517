# Comparing `tmp/ops_py_azure_key_vault_report-5.0.5.tar.gz` & `tmp/ops_py_azure_key_vault_report-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ops_py_azure_key_vault_report-5.0.5.tar", last modified: Thu Apr 25 10:51:31 2024, max compression
+gzip compressed data, was "ops_py_azure_key_vault_report-6.0.0.tar", last modified: Fri May 17 21:12:36 2024, max compression
```

## Comparing `ops_py_azure_key_vault_report-5.0.5.tar` & `ops_py_azure_key_vault_report-6.0.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:51:31.690344 ops_py_azure_key_vault_report-5.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 10:51:29.000000 ops_py_azure_key_vault_report-5.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-25 10:51:31.690344 ops_py_azure_key_vault_report-5.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:51:31.690344 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/
--rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/az_cmd.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    25749 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/azure_key_vault_report.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/html_table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/markdown.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/ms_teams_json.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/set_timestamp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7390 2024-04-25 10:51:26.000000 ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/slack_payloads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 10:51:31.690344 ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-04-25 10:51:31.000000 ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-25 10:51:31.000000 ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 10:51:31.000000 ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-25 10:51:31.000000 ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-25 10:51:29.000000 ops_py_azure_key_vault_report-5.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-04-25 10:51:29.000000 ops_py_azure_key_vault_report-5.0.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 10:51:31.690344 ops_py_azure_key_vault_report-5.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-25 10:51:29.000000 ops_py_azure_key_vault_report-5.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:12:36.071880 ops_py_azure_key_vault_report-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-17 21:12:34.000000 ops_py_azure_key_vault_report-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-17 21:12:36.071880 ops_py_azure_key_vault_report-6.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:12:36.067880 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      120 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2848 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/az_cmd.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28151 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/azure_key_vault_report.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2298 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/html_table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/markdown.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3185 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/ms_teams_json.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1114 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/set_timestamp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7390 2024-05-17 21:12:30.000000 ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/slack_payloads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:12:36.071880 ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8268 2024-05-17 21:12:36.000000 ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 21:12:36.000000 ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:12:36.000000 ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 21:12:36.000000 ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-17 21:12:34.000000 ops_py_azure_key_vault_report-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6846 2024-05-17 21:12:34.000000 ops_py_azure_key_vault_report-6.0.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:12:36.071880 ops_py_azure_key_vault_report-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-17 21:12:34.000000 ops_py_azure_key_vault_report-6.0.0/setup.py
```

### Comparing `ops_py_azure_key_vault_report-5.0.5/LICENSE` & `ops_py_azure_key_vault_report-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/PKG-INFO` & `ops_py_azure_key_vault_report-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.5
+Version: 6.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.5
+Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 6.0.0
 Summary: Output a Key Vault Secrets report License: MIT License Copyright (c)
 2024 Equinor Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/az_cmd.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/az_cmd.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/azure_key_vault_report.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/azure_key_vault_report.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         The summary of the report as dict
     report_md : str
         The text Markdown version of the report
     summary_md : str
         The text Markdown version of the summary
     report_summary_md : str
         The text Markdown version of the summary and report combined
-    slack_rows_md : list
+    slack_alert_rows : list
         The list of Slack messages formatted as Slack Markdown
     report_full : dict
         The full report, including the summary, as dict
 
     Methods
     -------
     parse_results()
@@ -57,15 +57,15 @@
         For each result in the results new item is created and added to the items list.
         Each item contains the following data:
         - Date objects, created from the 'updated', 'created' and 'expires' values and stored as values
           in new X_ts keys.
         - The age (in days) is calculated from each of the date objects and stored as values in new X_age keys.
         - 'vault_name' and 'record_type
 
-    add_report(expire_threshold=None, critical_threshold=None,
+    add_report(expire_threshold=None, alert_threshold=None,
                ignore_no_expiration=True, include_all=False, teams_json=False):
         Creates detailed 'column and rows' reports with comment according to the parameters passed.
 
         The column names are defined in the 'config.py' file.
 
         The values for the "Comment" column is generated according to the age of 'updated', 'created' and 'expires'.
         If missing 'expires' then a comment concerning that is added.
@@ -79,22 +79,22 @@
         The heading / keys are defined in the config.py file.
 
         The 'summary' dict is also added to the 'report_full' dict.
 
     sort_items():
         Returns a sorted list of all the records
 
-    get_teams_payload()
+    get_teams_payloads()
         Create and returns an MS Teams payload. The HTML table is added as a part of the payload, if no other
         text is provided as argument.
 
     get_html_table()
         Returns the HTML table which is used in the MS Teams payload.
 
-    get_slack_md(rows)
+    slack_alert_payload(rows)
         Creates a Slack Markdown of the provided list of rows.
 
     create_kv_rows()
         Creates key/value pairs of the items in the report rows
 
     get_report_full()
         Returns the dict version of the full report were all the rows are included and a dict of the summary.
@@ -131,15 +131,16 @@
         self.vaults = []        # The unique list of vaults processed
         self.html_table = None  # HTML table object. Used for MS Teams
         self.report_md = ""
         self.report = []
         self.summary = {}
         self.summary_md = ""
         self.report_summary_md = ""
-        self.slack_rows_md = []
+        self.slack_alert_rows = []
+        self.teams_alert_rows = []
         self.summary_values = config.get("summary")
         self.report_values = config.get("report")
         self.report_full = {
             "created_at": datetime.datetime.utcnow().isoformat(),
             "summary": {},
             "report": {}
         }
@@ -273,15 +274,15 @@
                     self.summary[text] = value
 
         md = Markdown(rows)
         md.set_widths()
         self.summary_md = md.get_output(1)
         self.report_full["summary"]["rows"] = [self.summary]
 
-    def add_report(self, expire_threshold=None, critical_threshold=None, ignore_no_expiration=True,
+    def add_report(self, expire_threshold=None, alert_threshold=None, ignore_no_expiration=True,
                    include_all=False, teams_json=False):
         """Creates a detailed 'column and rows' reports with comment.
 
         The column names are defined in the 'config.py' file.
 
         The values for the "Comment" column is generated according to the age of 'updated', 'created' and 'expires'.
         If missing 'expires' then a comment concerning that is added.
@@ -290,18 +291,18 @@
         A json object of a completed row is ALWAYS created.
 
         Parameters
         ----------
         expire_threshold : int
             Ignore to report the record if days till the secret will expire are more than this 'expire_threshold' value
             NOTE: Secrets expiring today or already expired will always be reported.
-        critical_threshold : int
+        alert_threshold : int
             If specified, a Slack Markdown post of the row will be created, IF the row contains a record which days to
-            expiring/expired (+/-) are within the value of 'critical_threshold' value.
-            The markdown post will then be added to a 'slack_rows_md' list.
+            expiring/expired (+/-) are within the value of 'alert_threshold' value.
+            The markdown post will then be added to a 'slack_alert_rows' list.
         ignore_no_expiration : bool
             Reports all records if set to False. If set to True only secrets with Expiration Date set will be reported.
         include_all : bool
             If set to True all records are included in the output.
         teams_json : bool
             If set to True then a report in json format containing a html table will also be generated.
         """
@@ -385,37 +386,42 @@
             # Skip records with no Expiration Date set, only if 'ignore_no_expiration' and not 'include_all'
             if not expires:
                 if ignore_no_expiration and not include_all:
                     continue
 
             # If the record has Expiration Date set, check if it should be alerted and/or reported on
             if isinstance(expires_age, int):
-                # Check if soon expiring OR expired recently (the critical_threshold range)
+                # Check if soon expiring OR expired recently (the alert_threshold range)
                 # If so, a Slack Markdown Payload of current row will be created
                 # and added to the list of Slack Markdown payloads,
-                if isinstance(critical_threshold, int):
-                    slack_md = False
+                if isinstance(alert_threshold, int):
+                    alert = False
 
-                    # The record has not expired, but is within the critical_threshold range
-                    if 0 >= expires_age >= -critical_threshold:
+                    # The record has not expired, but is within the alert_threshold range
+                    if 0 >= expires_age >= -alert_threshold:
                         logging.info(f"{record_name} - expiring in {abs(expires_age)} days.")
-                        slack_md = True
+                        alert = True
 
-                    # The record has expired and is within the critical_threshold range
-                    if 0 < expires_age <= critical_threshold:
+                    # The record has expired and is within the alert_threshold range
+                    if 0 < expires_age <= alert_threshold:
                         logging.info(f"{record_name} - expired {expires_age} days ago.")
-                        slack_md = True
+                        alert = True
 
-                    if slack_md:
-                        logging.info(f"{record_name} - critical_threshold is set to '{critical_threshold}'.")
+                    if alert:
+                        logging.info(f"{record_name} - alert_threshold is set to '{alert_threshold}'.")
                         logging.info(f"{record_name} - will be alerted to Slack.")
-                        slack_md_payload = self.get_slack_md(row)
-                        if slack_md_payload:
-                            logging.info(f"{record_name} - Slack Markdown payload created.")
-                            self.slack_rows_md.append(slack_md_payload)
+                        slack_payload = self.slack_alert_payload(row)
+                        if slack_payload:
+                            logging.info(f"{record_name} - Slack alert payload created.")
+                            self.slack_alert_rows.append(slack_payload)
+
+                        teams_payload = self.teams_alert_payload(row)
+                        if teams_payload:
+                            logging.info(f"{record_name} - MS Teams alert payload created.")
+                            self.teams_alert_rows.append(teams_payload)
 
                 if expires_age < 0:
                     # The record has not expired yet
                     logging.info(f"{record_name} - has not expired yet. "
                                  f"It will expire in {abs(expires_age)} days ({expires}).")
 
                     # Handle those within the valid 'expire_threshold' range
@@ -483,57 +489,99 @@
             if i > 0:
                 j = {}
                 for n, v in enumerate(self.report_values.get("heading")):
                     j[v] = r[n]
                 kv_rows.append(j)
         return kv_rows
 
-    def get_slack_md(self, row):
-        """Creates a Slack Markdown of the row.
+    def slack_alert_payload(self, row):
+        """Creates a Slack alert payload of the row.
 
         Returns
         -------
         A dict of the Slack item.
         """
 
         if not row:
             return
 
         item = {
-                "blocks": [
-                    {
-                        "type": "header",
-                        "text": {
-                            "type": "plain_text",
-                            "text": f"{row[0]}"
-                        }
-                    },
-                    {
-                        "type": "section",
-                        "text": {
-                            "type": "mrkdwn",
-                            "text": f"*{row[-1]}*"
-                        }
-                    },
-                    {
-                        "type": "section",
-                        "fields": []
+            "blocks": [
+                {
+                    "type": "header",
+                    "text": {
+                        "type": "plain_text",
+                        "text": f"{row[0]}"
                     }
-                ]
-            }
+                },
+                {
+                    "type": "section",
+                    "text": {
+                        "type": "mrkdwn",
+                        "text": f"*{row[-1]}*"
+                    }
+                },
+                {
+                    "type": "section",
+                    "fields": []
+                }
+            ]
+        }
 
         blocks = item.get("blocks")
         for i in range(1, len(row)-1):
             x = {"type": "mrkdwn",
                  "text": f"*{self.report_values['heading'][i]}:*\n{row[i]}"
                  }
             blocks[-1]["fields"].append(x)
         blocks.append({"type": "divider"})
         return item
 
+    def teams_alert_payload(self, row):
+        """Creates an MS Teams alert payload of the row.
+
+        Returns
+        -------
+        MS Teams payload.
+        """
+        if not row:
+            return
+
+        item = {"type": "message",
+                "attachments": [{"contentType": "application/vnd.microsoft.card.adaptive",
+                                 "content": {
+                                     "type": "AdaptiveCard",
+                                     "body": [
+                                         {
+                                             "type": "TextBlock",
+                                             "size": "large",
+                                             "weight": "Bolder",
+                                             "text": row[0]
+                                         },
+                                         {
+                                             "type": "TextBlock",
+                                             "size": "medium",
+                                             "weight": "Bolder",
+                                             "text": row[-1]
+                                         },
+                                         {
+                                             "type": "TextBlock",
+                                             "text": ""
+                                         }
+                                     ]
+                                 }
+                                 }
+                                ]
+                }
+
+        for i in range(1, len(row) - 1):
+            item['attachments'][0]['content']['body'][-1]["text"] += f"**{self.report_values['heading'][i]}:** {row[i]}\n\n"
+
+        return item
+
     def get_report_full(self):
         """Returns the dict version of the full report were all the rows are included and a dict of the summary."""
 
         return self.report_full
 
     def get_report(self):
         """Returns a list of dict versions of the filtered rows."""
@@ -561,29 +609,37 @@
         if self.report_md:
             self.report_summary_md = f"{self.summary_md}\n\n{self.report_md}"
         else:
             self.report_summary_md = self.summary_md
 
         return self.report_summary_md
 
-    def get_teams_payload(self, title, text=""):
+    def get_teams_payloads(self, title, text="", alert=False):
         """Initiate the MSTeamsPayload class to build and return an MS Teams payload.
 
         Parameters
         ----------
         title : string
             The 'activityTitle' of the MS Teams payload
         text : string
             The 'text' part of the payload. If not provided, the generated 'html_table' will be used instead.
+        alert : boolean
+            If set to True, the 'teams_alert_rows' will be returned, which is a list of Teams payloads (dicts) to be
+            posted to MS Teams.
+            This list has only been populated if the 'add_report' method has not been executed with a value for the
+            'alert_threshold' and the record in the row has met the 'alert_threshold' filter.
 
         Returns
         -------
         A json dump (string) of the complete payload.
         """
 
+        if alert:
+            return self.teams_alert_rows
+
         if not isinstance(self.results, list):
             return
 
         if len(self.items) == 0:
             return
 
         if not text:
@@ -597,38 +653,38 @@
         """Returns the 'html_table as string'
 
         None is returned if the 'add_report' method has not been executed with 'teams_json' argument set to True"""
 
         if self.html_table:
             return self.html_table.get_table()
 
-    def get_slack_payloads(self, title, max_chars=3500, md=False, app=True):
+    def get_slack_payloads(self, title, max_chars=3500, alert=False, app=True):
         """Returns a list of Slack messages to be used in Slack posts.
 
         Parameters
         ----------
         title : string
             Title/heading of the message.
         max_chars : int
             Message above this limit will be split into multiple parts
             (default: 3500)
-        md : boolean
-            If set to True, the 'slack_rows_md' will be returned, which is a list of Slack items (dicts) to be posted to Slack.
+        alert : boolean
+            If set to True, the 'slack_alert_rows' will be returned, which is a list of Slack items (dicts) to be posted to Slack.
             This list has only been populated if the 'add_report' method has not been executed with a value for the
-            'critical_threshold' and the record in the row has met the 'critical_threshold' filter.
+            'alert_threshold' and the record in the row has met the 'alert_threshold' filter.
         app : boolean
             If True, a list of Slack items (dicts) to be used as payload for a Slack App is returned
             If False, a list of Slack items in tuple pairs is returned. To be used to post to a Slack Workflow.
 
             Note: Not relevant if 'md' is set to True
 
         """
 
-        if md:
-            return self.slack_rows_md
+        if alert:
+            return self.slack_alert_rows
 
         self.get_summary_markdown()
         self.get_report_summary_markdown()
         self.get_report_markdown()
 
         p = SlackPayloads(title, self.summary_md, self.report_md, self.report_summary_md, max_chars=max_chars)
         if app:
```

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/config.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/config.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/html_table.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/html_table.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/markdown.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/markdown.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/ms_teams_json.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/ms_teams_json.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/set_timestamp.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/set_timestamp.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/azure_key_vault_report/slack_payloads.py` & `ops_py_azure_key_vault_report-6.0.0/azure_key_vault_report/slack_payloads.py`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/PKG-INFO` & `ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ops-py-azure-key-vault-report
-Version: 5.0.5
+Version: 6.0.0
 Summary: Output a Key Vault Secrets report
 License: MIT License
         
         Copyright (c) 2024 Equinor
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 5.0.5
+Metadata-Version: 2.1 Name: ops-py-azure-key-vault-report Version: 6.0.0
 Summary: Output a Key Vault Secrets report License: MIT License Copyright (c)
 2024 Equinor Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
 "Software"), to deal in the Software without restriction, including without
 limitation the rights to use, copy, modify, merge, publish, distribute,
 sublicense, and/or sell copies of the Software, and to permit persons to whom
 the Software is furnished to do so, subject to the following conditions: The
```

### Comparing `ops_py_azure_key_vault_report-5.0.5/ops_py_azure_key_vault_report.egg-info/SOURCES.txt` & `ops_py_azure_key_vault_report-6.0.0/ops_py_azure_key_vault_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ops_py_azure_key_vault_report-5.0.5/readme.md` & `ops_py_azure_key_vault_report-6.0.0/readme.md`

 * *Files identical despite different names*

