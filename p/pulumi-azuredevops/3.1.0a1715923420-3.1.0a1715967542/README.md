# Comparing `tmp/pulumi_azuredevops-3.1.0a1715923420.tar.gz` & `tmp/pulumi_azuredevops-3.1.0a1715967542.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-3.1.0a1715923420.tar", last modified: Fri May 17 05:28:22 2024, max compression
+gzip compressed data, was "pulumi_azuredevops-3.1.0a1715967542.tar", last modified: Fri May 17 17:43:22 2024, max compression
```

## Comparing `pulumi_azuredevops-3.1.0a1715923420.tar` & `pulumi_azuredevops-3.1.0a1715967542.tar`

### file list

```diff
@@ -1,133 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:28:22.811228 pulumi_azuredevops-3.1.0a1715923420/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-17 05:28:22.811228 pulumi_azuredevops-3.1.0a1715923420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:28:22.807228 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (127)    23402 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   156998 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_work_item_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    29671 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30214 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    35637 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    55861 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_business_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_exclusive_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_required_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:28:22.811228 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    34798 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/elastic_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/environment_resource_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     7954 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_azurecr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22737 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29707 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23886 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/library_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   199720 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/pipeline_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    23664 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20576 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21739 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27779 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    62516 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23777 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    32463 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24022 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (127)    22837 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    25424 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_nuget.py
--rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23121 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/variable_group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:28:22.811228 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-17 05:28:22.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-05-17 05:28:22.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:28:22.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 05:28:22.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-17 05:28:22.000000 pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 05:28:16.000000 pulumi_azuredevops-3.1.0a1715923420/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:28:22.811228 pulumi_azuredevops-3.1.0a1715923420/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.113656 pulumi_azuredevops-3.1.0a1715967542/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-17 17:43:22.113656 pulumi_azuredevops-3.1.0a1715967542/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.109656 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (127)    24210 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158510 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_work_item_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29671 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30214 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35637 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55861 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_business_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_exclusive_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_required_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.113656 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34798 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/elastic_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/environment_resource_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/feed_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_identity_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_identity_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_securityrole_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_azurecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23698 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29707 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23886 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/library_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   205734 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24778 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/pipeline_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23664 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20576 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21739 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/securityrole_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27779 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62516 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23777 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32463 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24022 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22837 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25424 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_nuget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23121 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/variable_group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:43:22.113656 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-17 17:43:22.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-17 17:43:22.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:43:22.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 17:43:22.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-17 17:43:22.000000 pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-17 17:43:15.000000 pulumi_azuredevops-3.1.0a1715967542/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:43:22.113656 pulumi_azuredevops-3.1.0a1715967542/setup.cfg
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/PKG-INFO` & `pulumi_azuredevops-3.1.0a1715967542/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1715923420
+Version: 3.1.0a1715967542
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/README.md` & `pulumi_azuredevops-3.1.0a1715967542/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,28 +21,35 @@
 from .check_branch_control import *
 from .check_business_hours import *
 from .check_exclusive_lock import *
 from .check_required_template import *
 from .elastic_pool import *
 from .environment import *
 from .environment_resource_kubernetes import *
+from .feed import *
+from .feed_permission import *
 from .get_agent_queue import *
 from .get_area import *
 from .get_build_definition import *
 from .get_client_config import *
 from .get_environment import *
+from .get_feed import *
 from .get_git_repository import *
 from .get_group import *
 from .get_groups import *
+from .get_identity_group import *
+from .get_identity_groups import *
+from .get_identity_users import *
 from .get_iteration import *
 from .get_pool import *
 from .get_pools import *
 from .get_project import *
 from .get_projects import *
 from .get_repositories import *
+from .get_securityrole_definitions import *
 from .get_service_endpoint_azure_rm import *
 from .get_service_endpoint_github import *
 from .get_serviceendpoint_azurecr import *
 from .get_serviceendpoint_npm import *
 from .get_serviceendpoint_sonarcloud import *
 from .get_team import *
 from .get_teams import *
@@ -69,14 +76,15 @@
 from .repository_policy_case_enforcement import *
 from .repository_policy_check_credentials import *
 from .repository_policy_file_path_pattern import *
 from .repository_policy_max_file_size import *
 from .repository_policy_max_path_length import *
 from .repository_policy_reserved_names import *
 from .resource_authorization import *
+from .securityrole_assignment import *
 from .service_endpoint_artifactory import *
 from .service_endpoint_aws import *
 from .service_endpoint_azure_dev_ops import *
 from .service_endpoint_azure_ecr import *
 from .service_endpoint_azure_rm import *
 from .service_endpoint_bit_bucket import *
 from .service_endpoint_docker_registry import *
@@ -287,14 +295,30 @@
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/environmentResourceKubernetes:EnvironmentResourceKubernetes": "EnvironmentResourceKubernetes"
   }
  },
  {
   "pkg": "azuredevops",
+  "mod": "index/feed",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/feed:Feed": "Feed"
+  }
+ },
+ {
+  "pkg": "azuredevops",
+  "mod": "index/feedPermission",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/feedPermission:FeedPermission": "FeedPermission"
+  }
+ },
+ {
+  "pkg": "azuredevops",
   "mod": "index/git",
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/git:Git": "Git"
   }
  },
  {
@@ -479,14 +503,22 @@
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/resourceAuthorization:ResourceAuthorization": "ResourceAuthorization"
   }
  },
  {
   "pkg": "azuredevops",
+  "mod": "index/securityroleAssignment",
+  "fqn": "pulumi_azuredevops",
+  "classes": {
+   "azuredevops:index/securityroleAssignment:SecurityroleAssignment": "SecurityroleAssignment"
+  }
+ },
+ {
+  "pkg": "azuredevops",
   "mod": "index/serviceEndpointArtifactory",
   "fqn": "pulumi_azuredevops",
   "classes": {
    "azuredevops:index/serviceEndpointArtifactory:ServiceEndpointArtifactory": "ServiceEndpointArtifactory"
   }
  },
  {
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     'BuildDefinitionPullRequestTriggerOverrideBranchFilterArgs',
     'BuildDefinitionPullRequestTriggerOverridePathFilterArgs',
     'BuildDefinitionRepositoryArgs',
     'BuildDefinitionScheduleArgs',
     'BuildDefinitionScheduleBranchFilterArgs',
     'BuildDefinitionVariableArgs',
     'CheckRequiredTemplateRequiredTemplateArgs',
+    'FeedFeatureArgs',
     'GitInitializationArgs',
     'ServiceEndpointArtifactoryAuthenticationBasicArgs',
     'ServiceEndpointArtifactoryAuthenticationTokenArgs',
     'ServiceEndpointAzureRMCredentialsArgs',
     'ServiceEndpointAzureRMFeaturesArgs',
     'ServiceEndpointGitHubAuthOauthArgs',
     'ServiceEndpointGitHubAuthPersonalArgs',
@@ -2264,14 +2265,53 @@
 
     @repository_type.setter
     def repository_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository_type", value)
 
 
 @pulumi.input_type
+class FeedFeatureArgs:
+    def __init__(__self__, *,
+                 permanent_delete: Optional[pulumi.Input[bool]] = None,
+                 restore: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[bool] permanent_delete: Determines if Feed should be Permanently removed, Defaults to `false`
+        :param pulumi.Input[bool] restore: Determines if Feed should be Restored during creation (if possible), Defaults to `false`
+        """
+        if permanent_delete is not None:
+            pulumi.set(__self__, "permanent_delete", permanent_delete)
+        if restore is not None:
+            pulumi.set(__self__, "restore", restore)
+
+    @property
+    @pulumi.getter(name="permanentDelete")
+    def permanent_delete(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Determines if Feed should be Permanently removed, Defaults to `false`
+        """
+        return pulumi.get(self, "permanent_delete")
+
+    @permanent_delete.setter
+    def permanent_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "permanent_delete", value)
+
+    @property
+    @pulumi.getter
+    def restore(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Determines if Feed should be Restored during creation (if possible), Defaults to `false`
+        """
+        return pulumi.get(self, "restore")
+
+    @restore.setter
+    def restore(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "restore", value)
+
+
+@pulumi.input_type
 class GitInitializationArgs:
     def __init__(__self__, *,
                  init_type: pulumi.Input[str],
                  service_connection_id: Optional[pulumi.Input[str]] = None,
                  source_type: Optional[pulumi.Input[str]] = None,
                  source_url: Optional[pulumi.Input[str]] = None):
         """
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/area_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_definition_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/build_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_approval.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_branch_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_business_hours.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_exclusive_lock.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_exclusive_lock.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/check_required_template.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/check_required_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/__init__.pyi` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/elastic_pool.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/elastic_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/environment_resource_kubernetes.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/environment_resource_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_agent_queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_environment.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_git_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 ]
 
 @pulumi.output_type
 class GetGitRepositoryResult:
     """
     A collection of values returned by getGitRepository.
     """
-    def __init__(__self__, default_branch=None, id=None, is_fork=None, name=None, project_id=None, remote_url=None, size=None, ssh_url=None, url=None, web_url=None):
+    def __init__(__self__, default_branch=None, disabled=None, id=None, is_fork=None, name=None, project_id=None, remote_url=None, size=None, ssh_url=None, url=None, web_url=None):
         if default_branch and not isinstance(default_branch, str):
             raise TypeError("Expected argument 'default_branch' to be a str")
         pulumi.set(__self__, "default_branch", default_branch)
+        if disabled and not isinstance(disabled, bool):
+            raise TypeError("Expected argument 'disabled' to be a bool")
+        pulumi.set(__self__, "disabled", disabled)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if is_fork and not isinstance(is_fork, bool):
             raise TypeError("Expected argument 'is_fork' to be a bool")
         pulumi.set(__self__, "is_fork", is_fork)
         if name and not isinstance(name, str):
@@ -59,14 +62,22 @@
         """
         The ref of the default branch.
         """
         return pulumi.get(self, "default_branch")
 
     @property
     @pulumi.getter
+    def disabled(self) -> bool:
+        """
+        Is the repository disabled?
+        """
+        return pulumi.get(self, "disabled")
+
+    @property
+    @pulumi.getter
     def id(self) -> str:
         """
         The provider-assigned unique ID for this managed resource.
         """
         return pulumi.get(self, "id")
 
     @property
@@ -134,14 +145,15 @@
 class AwaitableGetGitRepositoryResult(GetGitRepositoryResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
             yield self
         return GetGitRepositoryResult(
             default_branch=self.default_branch,
+            disabled=self.disabled,
             id=self.id,
             is_fork=self.is_fork,
             name=self.name,
             project_id=self.project_id,
             remote_url=self.remote_url,
             size=self.size,
             ssh_url=self.ssh_url,
@@ -180,14 +192,15 @@
     __args__['name'] = name
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('azuredevops:index/getGitRepository:getGitRepository', __args__, opts=opts, typ=GetGitRepositoryResult).value
 
     return AwaitableGetGitRepositoryResult(
         default_branch=pulumi.get(__ret__, 'default_branch'),
+        disabled=pulumi.get(__ret__, 'disabled'),
         id=pulumi.get(__ret__, 'id'),
         is_fork=pulumi.get(__ret__, 'is_fork'),
         name=pulumi.get(__ret__, 'name'),
         project_id=pulumi.get(__ret__, 'project_id'),
         remote_url=pulumi.get(__ret__, 'remote_url'),
         size=pulumi.get(__ret__, 'size'),
         ssh_url=pulumi.get(__ret__, 'ssh_url'),
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_iteration.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_azurecr.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_azurecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_npm.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/get_variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,40 +99,44 @@
         pulumi.set(self, "parent_repository_id", value)
 
 
 @pulumi.input_type
 class _GitState:
     def __init__(__self__, *,
                  default_branch: Optional[pulumi.Input[str]] = None,
+                 disabled: Optional[pulumi.Input[bool]] = None,
                  initialization: Optional[pulumi.Input['GitInitializationArgs']] = None,
                  is_fork: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  parent_repository_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  remote_url: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  ssh_url: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  web_url: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering Git resources.
         :param pulumi.Input[str] default_branch: The ref of the default branch. Will be used as the branch name for initialized repositories.
+        :param pulumi.Input[bool] disabled: Is the repository disabled?
         :param pulumi.Input['GitInitializationArgs'] initialization: An `initialization` block as documented below.
         :param pulumi.Input[bool] is_fork: True if the repository was created as a fork.
         :param pulumi.Input[str] name: The name of the git repository.
         :param pulumi.Input[str] parent_repository_id: The ID of a Git project from which a fork is to be created.
         :param pulumi.Input[str] project_id: The project ID or project name.
         :param pulumi.Input[str] remote_url: Git HTTPS URL of the repository
         :param pulumi.Input[int] size: Size in bytes.
         :param pulumi.Input[str] ssh_url: Git SSH URL of the repository.
         :param pulumi.Input[str] url: REST API URL of the repository.
         :param pulumi.Input[str] web_url: Web link to the repository.
         """
         if default_branch is not None:
             pulumi.set(__self__, "default_branch", default_branch)
+        if disabled is not None:
+            pulumi.set(__self__, "disabled", disabled)
         if initialization is not None:
             pulumi.set(__self__, "initialization", initialization)
         if is_fork is not None:
             pulumi.set(__self__, "is_fork", is_fork)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if parent_repository_id is not None:
@@ -160,14 +164,26 @@
 
     @default_branch.setter
     def default_branch(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_branch", value)
 
     @property
     @pulumi.getter
+    def disabled(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Is the repository disabled?
+        """
+        return pulumi.get(self, "disabled")
+
+    @disabled.setter
+    def disabled(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "disabled", value)
+
+    @property
+    @pulumi.getter
     def initialization(self) -> Optional[pulumi.Input['GitInitializationArgs']]:
         """
         An `initialization` block as documented below.
         """
         return pulumi.get(self, "initialization")
 
     @initialization.setter
@@ -464,14 +480,15 @@
                 raise TypeError("Missing required property 'initialization'")
             __props__.__dict__["initialization"] = initialization
             __props__.__dict__["name"] = name
             __props__.__dict__["parent_repository_id"] = parent_repository_id
             if project_id is None and not opts.urn:
                 raise TypeError("Missing required property 'project_id'")
             __props__.__dict__["project_id"] = project_id
+            __props__.__dict__["disabled"] = None
             __props__.__dict__["is_fork"] = None
             __props__.__dict__["remote_url"] = None
             __props__.__dict__["size"] = None
             __props__.__dict__["ssh_url"] = None
             __props__.__dict__["url"] = None
             __props__.__dict__["web_url"] = None
         super(Git, __self__).__init__(
@@ -481,14 +498,15 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             default_branch: Optional[pulumi.Input[str]] = None,
+            disabled: Optional[pulumi.Input[bool]] = None,
             initialization: Optional[pulumi.Input[pulumi.InputType['GitInitializationArgs']]] = None,
             is_fork: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             parent_repository_id: Optional[pulumi.Input[str]] = None,
             project_id: Optional[pulumi.Input[str]] = None,
             remote_url: Optional[pulumi.Input[str]] = None,
             size: Optional[pulumi.Input[int]] = None,
@@ -499,14 +517,15 @@
         Get an existing Git resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] default_branch: The ref of the default branch. Will be used as the branch name for initialized repositories.
+        :param pulumi.Input[bool] disabled: Is the repository disabled?
         :param pulumi.Input[pulumi.InputType['GitInitializationArgs']] initialization: An `initialization` block as documented below.
         :param pulumi.Input[bool] is_fork: True if the repository was created as a fork.
         :param pulumi.Input[str] name: The name of the git repository.
         :param pulumi.Input[str] parent_repository_id: The ID of a Git project from which a fork is to be created.
         :param pulumi.Input[str] project_id: The project ID or project name.
         :param pulumi.Input[str] remote_url: Git HTTPS URL of the repository
         :param pulumi.Input[int] size: Size in bytes.
@@ -515,14 +534,15 @@
         :param pulumi.Input[str] web_url: Web link to the repository.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _GitState.__new__(_GitState)
 
         __props__.__dict__["default_branch"] = default_branch
+        __props__.__dict__["disabled"] = disabled
         __props__.__dict__["initialization"] = initialization
         __props__.__dict__["is_fork"] = is_fork
         __props__.__dict__["name"] = name
         __props__.__dict__["parent_repository_id"] = parent_repository_id
         __props__.__dict__["project_id"] = project_id
         __props__.__dict__["remote_url"] = remote_url
         __props__.__dict__["size"] = size
@@ -537,14 +557,22 @@
         """
         The ref of the default branch. Will be used as the branch name for initialized repositories.
         """
         return pulumi.get(self, "default_branch")
 
     @property
     @pulumi.getter
+    def disabled(self) -> pulumi.Output[bool]:
+        """
+        Is the repository disabled?
+        """
+        return pulumi.get(self, "disabled")
+
+    @property
+    @pulumi.getter
     def initialization(self) -> pulumi.Output['outputs.GitInitialization']:
         """
         An `initialization` block as documented below.
         """
         return pulumi.get(self, "initialization")
 
     @property
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_repository_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/git_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group_entitlement.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group_entitlement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/iterative_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/library_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/library_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     'BuildDefinitionPullRequestTriggerOverrideBranchFilter',
     'BuildDefinitionPullRequestTriggerOverridePathFilter',
     'BuildDefinitionRepository',
     'BuildDefinitionSchedule',
     'BuildDefinitionScheduleBranchFilter',
     'BuildDefinitionVariable',
     'CheckRequiredTemplateRequiredTemplate',
+    'FeedFeature',
     'GitInitialization',
     'ServiceEndpointArtifactoryAuthenticationBasic',
     'ServiceEndpointArtifactoryAuthenticationToken',
     'ServiceEndpointAzureRMCredentials',
     'ServiceEndpointAzureRMFeatures',
     'ServiceEndpointGitHubAuthOauth',
     'ServiceEndpointGitHubAuthPersonal',
@@ -83,18 +84,20 @@
     'GetBuildDefinitionPullRequestTriggerOverrideBranchFilterResult',
     'GetBuildDefinitionPullRequestTriggerOverridePathFilterResult',
     'GetBuildDefinitionRepositoryResult',
     'GetBuildDefinitionScheduleResult',
     'GetBuildDefinitionScheduleBranchFilterResult',
     'GetBuildDefinitionVariableResult',
     'GetGroupsGroupResult',
+    'GetIdentityGroupsGroupResult',
     'GetIterationChildrenResult',
     'GetPoolsAgentPoolResult',
     'GetProjectsProjectResult',
     'GetRepositoriesRepositoryResult',
+    'GetSecurityroleDefinitionsDefinitionResult',
     'GetTeamsTeamResult',
     'GetUsersFeaturesResult',
     'GetUsersUserResult',
     'GetVariableGroupKeyVaultResult',
     'GetVariableGroupVariableResult',
 ]
 
@@ -2344,14 +2347,62 @@
         """
         The type of the repository storing the template. Valid values: `azuregit`, `github`, `githubenterprise`, `bitbucket`. Defaults to `azuregit`.
         """
         return pulumi.get(self, "repository_type")
 
 
 @pulumi.output_type
+class FeedFeature(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "permanentDelete":
+            suggest = "permanent_delete"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in FeedFeature. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        FeedFeature.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        FeedFeature.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 permanent_delete: Optional[bool] = None,
+                 restore: Optional[bool] = None):
+        """
+        :param bool permanent_delete: Determines if Feed should be Permanently removed, Defaults to `false`
+        :param bool restore: Determines if Feed should be Restored during creation (if possible), Defaults to `false`
+        """
+        if permanent_delete is not None:
+            pulumi.set(__self__, "permanent_delete", permanent_delete)
+        if restore is not None:
+            pulumi.set(__self__, "restore", restore)
+
+    @property
+    @pulumi.getter(name="permanentDelete")
+    def permanent_delete(self) -> Optional[bool]:
+        """
+        Determines if Feed should be Permanently removed, Defaults to `false`
+        """
+        return pulumi.get(self, "permanent_delete")
+
+    @property
+    @pulumi.getter
+    def restore(self) -> Optional[bool]:
+        """
+        Determines if Feed should be Restored during creation (if possible), Defaults to `false`
+        """
+        return pulumi.get(self, "restore")
+
+
+@pulumi.output_type
 class GitInitialization(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "initType":
             suggest = "init_type"
         elif key == "serviceConnectionId":
@@ -4519,14 +4570,39 @@
         """
         The unique identifier from the system of origin. Typically a sid, object id or Guid. Linking and unlinking operations can cause this value to change for a user because the user is not backed by a different provider and has a different unique id in the new provider.
         """
         return pulumi.get(self, "origin_id")
 
 
 @pulumi.output_type
+class GetIdentityGroupsGroupResult(dict):
+    def __init__(__self__, *,
+                 id: str,
+                 name: str):
+        """
+        :param str name: This is the non-unique display name of the identity subject. To change this field, you must alter its value in the source provider.
+        """
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "name", name)
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        This is the non-unique display name of the identity subject. To change this field, you must alter its value in the source provider.
+        """
+        return pulumi.get(self, "name")
+
+
+@pulumi.output_type
 class GetIterationChildrenResult(dict):
     def __init__(__self__, *,
                  has_children: bool,
                  id: str,
                  name: str,
                  path: str,
                  project_id: str):
@@ -4697,34 +4773,37 @@
         return pulumi.get(self, "state")
 
 
 @pulumi.output_type
 class GetRepositoriesRepositoryResult(dict):
     def __init__(__self__, *,
                  default_branch: str,
+                 disabled: bool,
                  id: str,
                  name: str,
                  project_id: str,
                  remote_url: str,
                  size: int,
                  ssh_url: str,
                  url: str,
                  web_url: str):
         """
         :param str default_branch: The ref of the default branch.
+        :param bool disabled: Is the repository disabled?
         :param str id: Git repository identifier.
         :param str name: Name of the Git repository to retrieve; requires `project_id` to be specified as well
         :param str project_id: ID of project to list Git repositories
         :param str remote_url: HTTPS Url to clone the Git repository
         :param int size: Compressed size (bytes) of the repository.
         :param str ssh_url: SSH Url to clone the Git repository
         :param str url: Details REST API endpoint for the Git Repository.
         :param str web_url: Url of the Git repository web view
         """
         pulumi.set(__self__, "default_branch", default_branch)
+        pulumi.set(__self__, "disabled", disabled)
         pulumi.set(__self__, "id", id)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "remote_url", remote_url)
         pulumi.set(__self__, "size", size)
         pulumi.set(__self__, "ssh_url", ssh_url)
         pulumi.set(__self__, "url", url)
@@ -4736,14 +4815,22 @@
         """
         The ref of the default branch.
         """
         return pulumi.get(self, "default_branch")
 
     @property
     @pulumi.getter
+    def disabled(self) -> bool:
+        """
+        Is the repository disabled?
+        """
+        return pulumi.get(self, "disabled")
+
+    @property
+    @pulumi.getter
     def id(self) -> str:
         """
         Git repository identifier.
         """
         return pulumi.get(self, "id")
 
     @property
@@ -4800,14 +4887,103 @@
         """
         Url of the Git repository web view
         """
         return pulumi.get(self, "web_url")
 
 
 @pulumi.output_type
+class GetSecurityroleDefinitionsDefinitionResult(dict):
+    def __init__(__self__, *,
+                 allow_permissions: int,
+                 description: str,
+                 display_name: str,
+                 identifier: str,
+                 name: str,
+                 scope: str,
+                 deny_permissions: Optional[int] = None):
+        """
+        :param int allow_permissions: The mask of allowed permissions of the Security Role Definition.
+        :param str description: The description of the Security Role Definition.
+        :param str display_name: The display name of the Security Role Definition.
+        :param str identifier: The identifier of the Security Role Definition.
+        :param str name: The name of the Security Role Definition.
+        :param str scope: Name of the Scope for which Security Role Definitions will be returned.
+               
+               DataSource without specifying any arguments will return all projects.
+        :param int deny_permissions: The mask of the denied permissions of the Security Role Definition.
+        """
+        pulumi.set(__self__, "allow_permissions", allow_permissions)
+        pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "display_name", display_name)
+        pulumi.set(__self__, "identifier", identifier)
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "scope", scope)
+        if deny_permissions is not None:
+            pulumi.set(__self__, "deny_permissions", deny_permissions)
+
+    @property
+    @pulumi.getter(name="allowPermissions")
+    def allow_permissions(self) -> int:
+        """
+        The mask of allowed permissions of the Security Role Definition.
+        """
+        return pulumi.get(self, "allow_permissions")
+
+    @property
+    @pulumi.getter
+    def description(self) -> str:
+        """
+        The description of the Security Role Definition.
+        """
+        return pulumi.get(self, "description")
+
+    @property
+    @pulumi.getter(name="displayName")
+    def display_name(self) -> str:
+        """
+        The display name of the Security Role Definition.
+        """
+        return pulumi.get(self, "display_name")
+
+    @property
+    @pulumi.getter
+    def identifier(self) -> str:
+        """
+        The identifier of the Security Role Definition.
+        """
+        return pulumi.get(self, "identifier")
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        """
+        The name of the Security Role Definition.
+        """
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def scope(self) -> str:
+        """
+        Name of the Scope for which Security Role Definitions will be returned.
+
+        DataSource without specifying any arguments will return all projects.
+        """
+        return pulumi.get(self, "scope")
+
+    @property
+    @pulumi.getter(name="denyPermissions")
+    def deny_permissions(self) -> Optional[int]:
+        """
+        The mask of the denied permissions of the Security Role Definition.
+        """
+        return pulumi.get(self, "deny_permissions")
+
+
+@pulumi.output_type
 class GetTeamsTeamResult(dict):
     def __init__(__self__, *,
                  administrators: Sequence[str],
                  description: str,
                  id: str,
                  members: Sequence[str],
                  name: str,
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/pipeline_authorization.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/pipeline_authorization.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,36 @@
 
 @pulumi.input_type
 class PipelineAuthorizationArgs:
     def __init__(__self__, *,
                  project_id: pulumi.Input[str],
                  resource_id: pulumi.Input[str],
                  type: pulumi.Input[str],
-                 pipeline_id: Optional[pulumi.Input[int]] = None):
+                 pipeline_id: Optional[pulumi.Input[int]] = None,
+                 pipeline_project_id: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a PipelineAuthorization resource.
         :param pulumi.Input[str] project_id: The  ID of the project. Changing this forces a new resource to be created
         :param pulumi.Input[str] resource_id: The ID of the resource to authorize. Changing this forces a new resource to be created
         :param pulumi.Input[str] type: The type of the resource to authorize. Valid values: `endpoint`, `queue`, `variablegroup`, `environment`, `repository`. Changing this forces a new resource to be created
                
                > **Note** `repository` is for AzureDevOps repository. To authorize repository other than
                Azure DevOps like GitHub you need to use service connection(`endpoint`)  to connect and authorize.
                Typical process for connecting to GitHub:
                **Pipeline  <----> Service Connection(`endpoint`) <----> GitHub Repository**
         :param pulumi.Input[int] pipeline_id: The ID of the pipeline. If not configured, all pipelines will be authorized. Changing this forces a new resource to be created.
+        :param pulumi.Input[str] pipeline_project_id: The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
         """
         pulumi.set(__self__, "project_id", project_id)
         pulumi.set(__self__, "resource_id", resource_id)
         pulumi.set(__self__, "type", type)
         if pipeline_id is not None:
             pulumi.set(__self__, "pipeline_id", pipeline_id)
+        if pipeline_project_id is not None:
+            pulumi.set(__self__, "pipeline_project_id", pipeline_project_id)
 
     @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Input[str]:
         """
         The  ID of the project. Changing this forces a new resource to be created
         """
@@ -85,36 +89,52 @@
         """
         return pulumi.get(self, "pipeline_id")
 
     @pipeline_id.setter
     def pipeline_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "pipeline_id", value)
 
+    @property
+    @pulumi.getter(name="pipelineProjectId")
+    def pipeline_project_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
+        """
+        return pulumi.get(self, "pipeline_project_id")
+
+    @pipeline_project_id.setter
+    def pipeline_project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pipeline_project_id", value)
+
 
 @pulumi.input_type
 class _PipelineAuthorizationState:
     def __init__(__self__, *,
                  pipeline_id: Optional[pulumi.Input[int]] = None,
+                 pipeline_project_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering PipelineAuthorization resources.
         :param pulumi.Input[int] pipeline_id: The ID of the pipeline. If not configured, all pipelines will be authorized. Changing this forces a new resource to be created.
+        :param pulumi.Input[str] pipeline_project_id: The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
         :param pulumi.Input[str] project_id: The  ID of the project. Changing this forces a new resource to be created
         :param pulumi.Input[str] resource_id: The ID of the resource to authorize. Changing this forces a new resource to be created
         :param pulumi.Input[str] type: The type of the resource to authorize. Valid values: `endpoint`, `queue`, `variablegroup`, `environment`, `repository`. Changing this forces a new resource to be created
                
                > **Note** `repository` is for AzureDevOps repository. To authorize repository other than
                Azure DevOps like GitHub you need to use service connection(`endpoint`)  to connect and authorize.
                Typical process for connecting to GitHub:
                **Pipeline  <----> Service Connection(`endpoint`) <----> GitHub Repository**
         """
         if pipeline_id is not None:
             pulumi.set(__self__, "pipeline_id", pipeline_id)
+        if pipeline_project_id is not None:
+            pulumi.set(__self__, "pipeline_project_id", pipeline_project_id)
         if project_id is not None:
             pulumi.set(__self__, "project_id", project_id)
         if resource_id is not None:
             pulumi.set(__self__, "resource_id", resource_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
@@ -127,14 +147,26 @@
         return pulumi.get(self, "pipeline_id")
 
     @pipeline_id.setter
     def pipeline_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "pipeline_id", value)
 
     @property
+    @pulumi.getter(name="pipelineProjectId")
+    def pipeline_project_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
+        """
+        return pulumi.get(self, "pipeline_project_id")
+
+    @pipeline_project_id.setter
+    def pipeline_project_id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pipeline_project_id", value)
+
+    @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> Optional[pulumi.Input[str]]:
         """
         The  ID of the project. Changing this forces a new resource to be created
         """
         return pulumi.get(self, "project_id")
 
@@ -174,14 +206,15 @@
 
 class PipelineAuthorization(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  pipeline_id: Optional[pulumi.Input[int]] = None,
+                 pipeline_project_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manage pipeline access permissions to resources.
 
@@ -255,14 +288,15 @@
         ## Relevant Links
 
         - [Azure DevOps Service REST API 7.1 - Pipeline Permissions](https://learn.microsoft.com/en-us/rest/api/azure/devops/approvalsandchecks/pipeline-permissions?view=azure-devops-rest-7.1)
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] pipeline_id: The ID of the pipeline. If not configured, all pipelines will be authorized. Changing this forces a new resource to be created.
+        :param pulumi.Input[str] pipeline_project_id: The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
         :param pulumi.Input[str] project_id: The  ID of the project. Changing this forces a new resource to be created
         :param pulumi.Input[str] resource_id: The ID of the resource to authorize. Changing this forces a new resource to be created
         :param pulumi.Input[str] type: The type of the resource to authorize. Valid values: `endpoint`, `queue`, `variablegroup`, `environment`, `repository`. Changing this forces a new resource to be created
                
                > **Note** `repository` is for AzureDevOps repository. To authorize repository other than
                Azure DevOps like GitHub you need to use service connection(`endpoint`)  to connect and authorize.
                Typical process for connecting to GitHub:
@@ -360,27 +394,29 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  pipeline_id: Optional[pulumi.Input[int]] = None,
+                 pipeline_project_id: Optional[pulumi.Input[str]] = None,
                  project_id: Optional[pulumi.Input[str]] = None,
                  resource_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = PipelineAuthorizationArgs.__new__(PipelineAuthorizationArgs)
 
             __props__.__dict__["pipeline_id"] = pipeline_id
+            __props__.__dict__["pipeline_project_id"] = pipeline_project_id
             if project_id is None and not opts.urn:
                 raise TypeError("Missing required property 'project_id'")
             __props__.__dict__["project_id"] = project_id
             if resource_id is None and not opts.urn:
                 raise TypeError("Missing required property 'resource_id'")
             __props__.__dict__["resource_id"] = resource_id
             if type is None and not opts.urn:
@@ -393,53 +429,64 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             pipeline_id: Optional[pulumi.Input[int]] = None,
+            pipeline_project_id: Optional[pulumi.Input[str]] = None,
             project_id: Optional[pulumi.Input[str]] = None,
             resource_id: Optional[pulumi.Input[str]] = None,
             type: Optional[pulumi.Input[str]] = None) -> 'PipelineAuthorization':
         """
         Get an existing PipelineAuthorization resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] pipeline_id: The ID of the pipeline. If not configured, all pipelines will be authorized. Changing this forces a new resource to be created.
+        :param pulumi.Input[str] pipeline_project_id: The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
         :param pulumi.Input[str] project_id: The  ID of the project. Changing this forces a new resource to be created
         :param pulumi.Input[str] resource_id: The ID of the resource to authorize. Changing this forces a new resource to be created
         :param pulumi.Input[str] type: The type of the resource to authorize. Valid values: `endpoint`, `queue`, `variablegroup`, `environment`, `repository`. Changing this forces a new resource to be created
                
                > **Note** `repository` is for AzureDevOps repository. To authorize repository other than
                Azure DevOps like GitHub you need to use service connection(`endpoint`)  to connect and authorize.
                Typical process for connecting to GitHub:
                **Pipeline  <----> Service Connection(`endpoint`) <----> GitHub Repository**
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _PipelineAuthorizationState.__new__(_PipelineAuthorizationState)
 
         __props__.__dict__["pipeline_id"] = pipeline_id
+        __props__.__dict__["pipeline_project_id"] = pipeline_project_id
         __props__.__dict__["project_id"] = project_id
         __props__.__dict__["resource_id"] = resource_id
         __props__.__dict__["type"] = type
         return PipelineAuthorization(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="pipelineId")
     def pipeline_id(self) -> pulumi.Output[Optional[int]]:
         """
         The ID of the pipeline. If not configured, all pipelines will be authorized. Changing this forces a new resource to be created.
         """
         return pulumi.get(self, "pipeline_id")
 
     @property
+    @pulumi.getter(name="pipelineProjectId")
+    def pipeline_project_id(self) -> pulumi.Output[Optional[str]]:
+        """
+        The ID of the project where the pipeline exists. Defaults to `project_id` if not specified. Changing this forces a new resource to be created
+        """
+        return pulumi.get(self, "pipeline_project_id")
+
+    @property
     @pulumi.getter(name="projectId")
     def project_id(self) -> pulumi.Output[str]:
         """
         The  ID of the project. Changing this forces a new resource to be created
         """
         return pulumi.get(self, "project_id")
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_gcp_terraform.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_gcp_terraform.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jenkins.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jenkins.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_maven.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_maven.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_nexus.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_nexus.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_nuget.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_nuget.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/servicehook_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/servicehook_storage_queue_pipelines.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/servicehook_storage_queue_pipelines.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/tagging_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team_administrators.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/user.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/variable_group_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/variable_group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops/workitem.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.1.0a1715923420
+Version: 3.1.0a1715967542
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-3.1.0a1715967542/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -19,28 +19,35 @@
 pulumi_azuredevops/check_branch_control.py
 pulumi_azuredevops/check_business_hours.py
 pulumi_azuredevops/check_exclusive_lock.py
 pulumi_azuredevops/check_required_template.py
 pulumi_azuredevops/elastic_pool.py
 pulumi_azuredevops/environment.py
 pulumi_azuredevops/environment_resource_kubernetes.py
+pulumi_azuredevops/feed.py
+pulumi_azuredevops/feed_permission.py
 pulumi_azuredevops/get_agent_queue.py
 pulumi_azuredevops/get_area.py
 pulumi_azuredevops/get_build_definition.py
 pulumi_azuredevops/get_client_config.py
 pulumi_azuredevops/get_environment.py
+pulumi_azuredevops/get_feed.py
 pulumi_azuredevops/get_git_repository.py
 pulumi_azuredevops/get_group.py
 pulumi_azuredevops/get_groups.py
+pulumi_azuredevops/get_identity_group.py
+pulumi_azuredevops/get_identity_groups.py
+pulumi_azuredevops/get_identity_users.py
 pulumi_azuredevops/get_iteration.py
 pulumi_azuredevops/get_pool.py
 pulumi_azuredevops/get_pools.py
 pulumi_azuredevops/get_project.py
 pulumi_azuredevops/get_projects.py
 pulumi_azuredevops/get_repositories.py
+pulumi_azuredevops/get_securityrole_definitions.py
 pulumi_azuredevops/get_service_endpoint_azure_rm.py
 pulumi_azuredevops/get_service_endpoint_github.py
 pulumi_azuredevops/get_serviceendpoint_azurecr.py
 pulumi_azuredevops/get_serviceendpoint_npm.py
 pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
 pulumi_azuredevops/get_team.py
 pulumi_azuredevops/get_teams.py
@@ -70,14 +77,15 @@
 pulumi_azuredevops/repository_policy_case_enforcement.py
 pulumi_azuredevops/repository_policy_check_credentials.py
 pulumi_azuredevops/repository_policy_file_path_pattern.py
 pulumi_azuredevops/repository_policy_max_file_size.py
 pulumi_azuredevops/repository_policy_max_path_length.py
 pulumi_azuredevops/repository_policy_reserved_names.py
 pulumi_azuredevops/resource_authorization.py
+pulumi_azuredevops/securityrole_assignment.py
 pulumi_azuredevops/service_endpoint_artifactory.py
 pulumi_azuredevops/service_endpoint_aws.py
 pulumi_azuredevops/service_endpoint_azure_dev_ops.py
 pulumi_azuredevops/service_endpoint_azure_ecr.py
 pulumi_azuredevops/service_endpoint_azure_rm.py
 pulumi_azuredevops/service_endpoint_bit_bucket.py
 pulumi_azuredevops/service_endpoint_docker_registry.py
```

### Comparing `pulumi_azuredevops-3.1.0a1715923420/pyproject.toml` & `pulumi_azuredevops-3.1.0a1715967542/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_azuredevops"
   description = "A Pulumi package for creating and managing Azure DevOps."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "azuredevops"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.1.0a1715923420"
+  version = "3.1.0a1715967542"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-azuredevops"
 
 [build-system]
```

