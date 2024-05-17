# Comparing `tmp/snakemake_executor_plugin_lsf-0.2.4.tar.gz` & `tmp/snakemake_executor_plugin_lsf-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.4.tar", max compression
+gzip compressed data, was "snakemake_executor_plugin_lsf-0.2.5.tar", max compression
```

## Comparing `snakemake_executor_plugin_lsf-0.2.4.tar` & `snakemake_executor_plugin_lsf-0.2.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1076 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/LICENSE
--rw-r--r--   0        0        0     5668 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/README.md
--rw-r--r--   0        0        0     1193 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/pyproject.toml
--rw-r--r--   0        0        0    25647 2024-04-23 20:37:48.484738 snakemake_executor_plugin_lsf-0.2.4/snakemake_executor_plugin_lsf/__init__.py
--rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/LICENSE
+-rw-r--r--   0        0        0     5668 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/README.md
+-rw-r--r--   0        0        0     1193 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0    25828 2024-05-17 01:12:53.285130 snakemake_executor_plugin_lsf-0.2.5/snakemake_executor_plugin_lsf/__init__.py
+-rw-r--r--   0        0        0     6714 1970-01-01 00:00:00.000000 snakemake_executor_plugin_lsf-0.2.5/PKG-INFO
```

### Comparing `snakemake_executor_plugin_lsf-0.2.4/LICENSE` & `snakemake_executor_plugin_lsf-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_lsf-0.2.4/README.md` & `snakemake_executor_plugin_lsf-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_executor_plugin_lsf-0.2.4/pyproject.toml` & `snakemake_executor_plugin_lsf-0.2.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-executor-plugin-lsf"
-version = "0.2.4"
+version = "0.2.5"
 description = "A Snakemake executor plugin for submitting jobs to a LSF cluster."
 authors = [
     "Brian Fulton-Howard <brian.fulton-howard@mssm.edu>",
     "Christian Meesters <meesters@uni-mainz.de>",
     "David Lähnemann <david.laehnemann@dkfz-heidelberg.de>",
     "Johannes Koester <johannes.koester@uni-due.de>",
 ]
```

### Comparing `snakemake_executor_plugin_lsf-0.2.4/snakemake_executor_plugin_lsf/__init__.py` & `snakemake_executor_plugin_lsf-0.2.5/snakemake_executor_plugin_lsf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,16 +157,16 @@
         # MPI job
         if job.resources.get("mpi", False):
             if job.resources.get("ptile", False):
                 call += f" -R span[ptile={job.resources.get('ptile', 1)}]"
         else:
             call += " -R span[hosts=1]"
 
-        if job.resources.get("lsf_extra"):
-            call += f" {job.resources.lsf_extra}"
+        if job.resources.get("lsf_extra", False):
+            call += f" {job.resources.get('lsf_extra')}"
 
         exec_job = self.format_job_exec(job)
 
         # ensure that workdir is set correctly
         call += f" -cwd {self.workflow.workdir_init}"
         # and finally the job to execute with all the snakemake parameters
         # TODO do I need an equivalent to --wrap?
@@ -177,15 +177,20 @@
             out = subprocess.check_output(
                 call, shell=True, text=True, stderr=subprocess.STDOUT
             ).strip()
         except subprocess.CalledProcessError as e:
             raise WorkflowError(
                 f"LSF job submission failed. The error message was {e.output}"
             )
-        lsf_jobid = out.split(" ")[1][1:-1]
+
+        lsf_jobid = re.search(r"Job <(\d+)>", out)[1]
+        if not lsf_jobid:
+            raise WorkflowError(
+                f"Could not extract LSF job ID. The submission message was\n{out}"
+            )
         lsf_logfile = lsf_logfile.replace("%J", lsf_jobid)
         self.logger.info(
             f"Job {job.jobid} has been submitted with LSF jobid {lsf_jobid} "
             f"(log: {lsf_logfile})."
         )
         self.report_job_submission(
             SubmittedJobInfo(
```

### Comparing `snakemake_executor_plugin_lsf-0.2.4/PKG-INFO` & `snakemake_executor_plugin_lsf-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-executor-plugin-lsf
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Snakemake executor plugin for submitting jobs to a LSF cluster.
 Home-page: https://github.com/befh/snakemake-executor-plugin-lsf
 License: MIT
 Keywords: snakemake,plugin,executor,cluster,lsf
 Author: Brian Fulton-Howard
 Author-email: brian.fulton-howard@mssm.edu
 Requires-Python: >=3.11,<4.0
```

