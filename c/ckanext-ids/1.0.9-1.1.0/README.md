# Comparing `tmp/ckanext-ids-1.0.9.tar.gz` & `tmp/ckanext-ids-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ids-1.0.9.tar", last modified: Fri Mar 24 12:59:04 2023, max compression
+gzip compressed data, was "ckanext-ids-1.1.0.tar", last modified: Fri May 17 07:48:02 2024, max compression
```

## Comparing `ckanext-ids-1.0.9.tar` & `ckanext-ids-1.1.0.tar`

### file list

```diff
@@ -1,137 +1,148 @@
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/LICENSE
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      153 2022-10-27 10:57:45.000000 ckanext-ids-1.0.9/MANIFEST.in
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4289 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/PKG-INFO
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3742 2023-03-16 15:37:20.000000 ckanext-ids-1.0.9/README.md
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      219 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/ckanext/__init__.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/ckanext/ids/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1770 2022-06-01 12:48:01.000000 ckanext-ids-1.0.9/ckanext/ids/activity.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/assets/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/assets/css/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      324 2023-03-23 08:21:23.000000 ckanext-ids-1.0.9/ckanext/ids/assets/css/resource-upload.css
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/assets/js/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     9149 2021-04-29 11:39:34.000000 ckanext-ids-1.0.9/ckanext/ids/assets/js/resource-upload.js
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      116 2021-04-29 08:42:02.000000 ckanext-ids-1.0.9/ckanext/ids/assets/resource.config
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      265 2021-04-29 08:41:43.000000 ckanext-ids-1.0.9/ckanext/ids/assets/webassets.yml
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    35674 2023-03-15 15:12:30.000000 ckanext-ids-1.0.9/ckanext/ids/blueprints.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2021-11-26 10:03:19.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    10498 2022-11-16 13:39:53.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/connector.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     5725 2022-05-06 09:24:51.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/contract.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2022-05-05 15:35:58.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/idsapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4963 2022-12-07 13:09:13.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/offer.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1335 2022-05-06 09:24:51.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/resource.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     8512 2022-12-14 16:31:34.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/resourceapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     5923 2022-12-15 14:19:46.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/subscribe.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2022-04-22 07:36:30.000000 ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/subscriptionapi.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6380 2021-06-01 14:57:13.000000 ckanext-ids-1.0.9/ckanext/ids/harvester.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3525 2022-12-07 15:33:28.000000 ckanext-ids-1.0.9/ckanext/ids/helpers.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/i18n/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1988 2021-04-20 10:59:19.000000 ckanext-ids-1.0.9/ckanext/ids/i18n/ckanext-ids.pot
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.226085 ckanext-ids-1.0.9/ckanext/ids/i18n/en/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/i18n/en/LC_MESSAGES/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2037 2021-04-20 10:59:22.000000 ckanext-ids-1.0.9/ckanext/ids/i18n/en/LC_MESSAGES/ckanext-ids.po
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/logic/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2021-12-06 13:10:56.000000 ckanext-ids-1.0.9/ckanext/ids/logic/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      840 2022-03-17 11:38:41.000000 ckanext-ids-1.0.9/ckanext/ids/logic/action.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/metadatabroker/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-02-14 12:09:52.000000 ckanext-ids-1.0.9/ckanext/ids/metadatabroker/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    27153 2023-03-22 10:47:11.000000 ckanext-ids-1.0.9/ckanext/ids/metadatabroker/client.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3159 2022-02-14 12:09:52.000000 ckanext-ids-1.0.9/ckanext/ids/metadatabroker/translations_broker_ckan.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/model/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     5464 2022-05-06 09:23:39.000000 ckanext-ids-1.0.9/ckanext/ids/model/__init__.py
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)    17556 2023-03-24 12:57:09.000000 ckanext-ids-1.0.9/ckanext/ids/plugin.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.226085 ckanext-ids-1.0.9/ckanext/ids/public/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.226085 ckanext-ids-1.0.9/ckanext/ids/public/api/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/public/api/swagger/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    25273 2022-10-27 14:17:32.000000 ckanext-ids-1.0.9/ckanext/ids/public/api/swagger/ckan_ids_openapi.json
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/recomm/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-05-06 09:24:51.000000 ckanext-ids-1.0.9/ckanext/ids/recomm/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    17071 2022-05-10 12:02:18.000000 ckanext-ids-1.0.9/ckanext/ids/recomm/recomm.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/schemes/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     2934 2023-03-17 20:33:18.000000 ckanext-ids-1.0.9/ckanext/ids/schemes/application.yml
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3650 2023-03-17 20:33:18.000000 ckanext-ids-1.0.9/ckanext/ids/schemes/dataset.yml
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1103 2023-03-17 20:33:18.000000 ckanext-ids-1.0.9/ckanext/ids/schemes/organization.yml
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      983 2023-03-17 20:33:18.000000 ckanext-ids-1.0.9/ckanext/ids/schemes/presets.json
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3174 2023-03-17 20:33:18.000000 ckanext-ids-1.0.9/ckanext/ids/schemes/service.yml
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/smart_contracts/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2022-06-01 06:44:38.000000 ckanext-ids-1.0.9/ckanext/ids/smart_contracts/__init__.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1499 2022-06-01 06:44:38.000000 ckanext-ids-1.0.9/ckanext/ids/smart_contracts/smart_contract_client.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      903 2022-10-27 14:42:39.000000 ckanext-ids-1.0.9/ckanext/ids/swagger.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      170 2021-04-29 08:40:56.000000 ckanext-ids-1.0.9/ckanext/ids/templates/base.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/form-snippets/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     1222 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/ckanext/ids/templates/form-snippets/slug.html
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      336 2023-03-23 08:20:39.000000 ckanext-ids-1.0.9/ckanext/ids/templates/header.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1483 2022-10-27 10:56:47.000000 ckanext-ids-1.0.9/ckanext/ids/templates/index.template.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/macros/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    20397 2021-04-29 12:24:44.000000 ckanext-ids-1.0.9/ckanext/ids/templates/macros/custom_form.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/organization/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      575 2022-03-10 10:42:18.000000 ckanext-ids-1.0.9/ckanext/ids/templates/organization/read.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/organization/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2635 2021-04-20 10:59:07.000000 ckanext-ids-1.0.9/ckanext/ids/templates/organization/snippets/organization_item.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/package/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2541 2022-03-08 14:26:14.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/base_form_page.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      723 2021-12-14 14:18:34.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/contracts.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1966 2023-03-15 16:09:49.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/contracts_external.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      242 2021-12-14 14:00:58.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/edit_base.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      852 2022-09-09 14:25:05.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/publish.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1631 2022-12-07 16:12:54.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/contract_item.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2848 2022-09-09 15:02:59.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/contracts_list.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2302 2023-03-23 12:42:09.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/package_form.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4746 2023-03-23 12:42:09.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/resource_form.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1936 2022-02-14 12:09:52.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/resources_list.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1473 2021-11-25 09:46:40.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/stages.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    14446 2022-09-09 13:53:30.000000 ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/storepublisher_publish_form.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2111 2021-12-13 14:15:45.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/datetime_tz.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      652 2022-12-09 03:59:13.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/disabled.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      735 2021-12-14 12:06:13.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/duration.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      624 2021-12-09 14:18:25.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/number.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      649 2021-04-29 04:47:53.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/upload.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/organization/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      201 2022-03-10 12:33:07.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/organization/group_form.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/package/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/package/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2326 2021-12-01 08:25:52.000000 ckanext-ids-1.0.9/ckanext/ids/templates/scheming/package/snippets/resource_form.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/activities/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      940 2022-06-01 12:59:00.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/activities/created_contract.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      954 2022-06-01 13:21:59.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/activities/pushed_to_dataspace_connector.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      234 2021-04-20 12:32:57.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/add_dataset.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      810 2021-04-20 11:06:57.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/organization.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      474 2023-03-23 08:18:01.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/package_item.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1205 2021-04-28 15:53:37.000000 ckanext-ids-1.0.9/ckanext/ids/templates/snippets/resource_fields.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates/user/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      257 2023-03-22 14:55:12.000000 ckanext-ids-1.0.9/ckanext/ids/templates/user/dashboard_organizations.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1511 2022-05-06 09:24:51.000000 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/layout1.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2460 2022-05-10 12:02:18.000000 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/snippets/recomm_homepage.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.230085 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2241 2022-05-10 12:02:18.000000 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/snippets/recomm_entity_sidebar.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3800 2022-05-06 09:24:51.000000 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/snippets/resource_item.html
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/snippets/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1696 2022-05-10 12:02:18.000000 ckanext-ids-1.0.9/ckanext/ids/templates_recommender/snippets/search_form.html
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2021-04-28 09:51:42.000000 ckanext-ids-1.0.9/ckanext/ids/test.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext/ids/tests/
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/ckanext/ids/tests/__init__.py
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     1253 2021-04-16 12:41:49.000000 ckanext-ids-1.0.9/ckanext/ids/tests/test_plugin.py
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7004 2022-09-09 14:13:15.000000 ckanext-ids-1.0.9/ckanext/ids/usage_control.json
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1777 2022-06-01 12:59:00.000000 ckanext-ids-1.0.9/ckanext/ids/validator.py
-drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/ckanext_ids.egg-info/
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4289 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/PKG-INFO
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3942 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/SOURCES.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/dependency_links.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      455 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/entry_points.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/namespace_packages.txt
--rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2023-03-24 12:59:04.000000 ckanext-ids-1.0.9/ckanext_ids.egg-info/top_level.txt
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      257 2023-03-13 09:11:49.000000 ckanext-ids-1.0.9/requirements.txt
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      505 2023-03-24 12:59:04.234084 ckanext-ids-1.0.9/setup.cfg
--rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     4034 2023-03-24 12:57:30.000000 ckanext-ids-1.0.9/setup.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)    34500 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/LICENSE
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      166 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/MANIFEST.in
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4269 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/PKG-INFO
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3742 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/README.md
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      219 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/__init__.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1770 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/activity.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/assets/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/assets/css/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      324 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/assets/css/resource-upload.css
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/assets/js/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     9149 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/assets/js/resource-upload.js
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      116 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/assets/resource.config
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      265 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/assets/webassets.yml
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    42727 2024-05-14 11:51:21.000000 ckanext-ids-1.1.0/ckanext/ids/blueprints.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    10556 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/connector.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     5725 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/contract.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3087 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/idsapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4963 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/offer.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1335 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/resource.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     9704 2024-05-07 16:27:40.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/resourceapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6078 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/subscribe.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1535 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/subscriptionapi.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6380 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/harvester.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3525 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/helpers.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/i18n/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1988 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/i18n/ckanext-ids.pot
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.705909 ckanext-ids-1.1.0/ckanext/ids/i18n/en/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/i18n/en/LC_MESSAGES/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2037 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/i18n/en/LC_MESSAGES/ckanext-ids.po
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/logic/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/logic/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      840 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/logic/action.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/metadatabroker/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/metadatabroker/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    27590 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/metadatabroker/client.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3159 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/metadatabroker/translations_broker_ckan.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/model/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7413 2024-04-24 17:19:30.000000 ckanext-ids-1.1.0/ckanext/ids/model/__init__.py
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)    19721 2024-05-07 19:06:05.000000 ckanext-ids-1.1.0/ckanext/ids/plugin.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.705909 ckanext-ids-1.1.0/ckanext/ids/public/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.705909 ckanext-ids-1.1.0/ckanext/ids/public/api/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/public/api/swagger/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    25273 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/public/api/swagger/ckan_ids_openapi.json
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     6550 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/public/api/swagger/ckan_ids_openapi.yaml
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/public/images/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)    18423 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/public/images/TrustsLogo.png
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/recomm/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/recomm/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    17071 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/recomm/recomm.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.713909 ckanext-ids-1.1.0/ckanext/ids/schemes/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     2934 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/schemes/application.yml
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3650 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/schemes/dataset.yml
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1103 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/schemes/organization.yml
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      983 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/schemes/presets.json
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     3174 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/schemes/service.yml
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/smart_contracts/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/smart_contracts/__init__.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1499 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/smart_contracts/smart_contract_client.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      903 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/swagger.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/admin/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      425 2024-05-07 19:06:05.000000 ckanext-ids-1.1.0/ckanext/ids/templates/admin/config.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      170 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/base.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/form-snippets/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     1222 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/form-snippets/slug.html
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      336 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/header.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1483 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/index.template.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/macros/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    20397 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/macros/custom_form.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/organization/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      575 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/organization/read.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/organization/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2635 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/organization/snippets/organization_item.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/package/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2541 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/base_form_page.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      723 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/contracts.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4302 2024-04-24 16:28:28.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/contracts_external.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      242 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/edit_base.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      847 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/publish.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4124 2024-05-07 23:17:51.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/agreements_table.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1683 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/contract_item.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2848 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/contracts_list.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2302 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/package_form.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4746 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/resource_form.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      403 2024-04-23 16:31:20.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/resource_item.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1947 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/resources_list.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1473 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/stages.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)    14446 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/storepublisher_publish_form.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2753 2024-05-07 23:13:36.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/workflows_table.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     8267 2024-05-07 23:43:34.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/workflow_configuration.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2616 2024-05-07 23:20:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/package/workflows.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2111 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/datetime_tz.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      652 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/disabled.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      735 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/duration.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      624 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/number.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      649 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/upload.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.717909 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/organization/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      201 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/organization/group_form.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/package/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/package/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      408 2024-04-08 07:00:28.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/package/snippets/additional_info.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2326 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/scheming/package/snippets/resource_form.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/activities/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      940 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/activities/created_contract.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      954 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/activities/pushed_to_dataspace_connector.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      234 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/add_dataset.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      810 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/organization.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      474 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/package_item.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1205 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/snippets/resource_fields.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates/user/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      257 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates/user/dashboard_organizations.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1511 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/layout1.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2460 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/snippets/recomm_homepage.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.709909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     2241 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/snippets/recomm_entity_sidebar.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     3800 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/snippets/resource_item.html
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/snippets/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1696 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/templates_recommender/snippets/search_form.html
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/test.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext/ids/tests/
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/tests/__init__.py
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     1253 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/tests/test_plugin.py
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     7004 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/usage_control.json
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     1777 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/ckanext/ids/validator.py
+drwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)        0 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/ckanext_ids.egg-info/
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4269 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/PKG-INFO
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)     4427 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/SOURCES.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        1 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/dependency_links.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)      433 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/entry_points.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/namespace_packages.txt
+-rw-rw-r--   0 karampatakiss  (1001) karampatakiss  (1001)        8 2024-05-17 07:48:02.000000 ckanext-ids-1.1.0/ckanext_ids.egg-info/top_level.txt
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      236 2023-11-09 07:27:13.000000 ckanext-ids-1.1.0/requirements.txt
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)      505 2024-05-17 07:48:02.721909 ckanext-ids-1.1.0/setup.cfg
+-rwxrwxr-x   0 karampatakiss  (1001) karampatakiss  (1001)     4082 2024-05-17 07:40:15.000000 ckanext-ids-1.1.0/setup.py
```

### Comparing `ckanext-ids-1.0.9/LICENSE` & `ckanext-ids-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/PKG-INFO` & `ckanext-ids-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ckanext-ids
-Version: 1.0.9
+Version: 1.1.0
 Summary: IDS data model extension for CKAN
 Home-page: https://github.com/semantic-web-company/ckanext-ids
 Author: Sotiris Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN IDS
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/semantic-web-company/ckanext-ids/workflows/Tests/badge.svg?branch=main)](https://github.com/semantic-web-company/ckanext-ids/actions)
@@ -140,9 +139,7 @@
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
 
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
-
-
```

### Comparing `ckanext-ids-1.0.9/README.md` & `ckanext-ids-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/activity.py` & `ckanext-ids-1.1.0/ckanext/ids/activity.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/assets/js/resource-upload.js` & `ckanext-ids-1.1.0/ckanext/ids/assets/js/resource-upload.js`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/blueprints.py` & `ckanext-ids-1.1.0/ckanext/ids/blueprints.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import copy
 import datetime
 import json
 import logging
+import uuid
 from collections import defaultdict
 from urllib.parse import urlsplit
 
 import ckan.lib.base as base
 import ckan.lib.helpers as h
 import ckan.lib.navl.dictization_functions as dict_fns
 import ckan.logic as logic
 import ckan.model as model
 import ckan.plugins as plugins
 import ckan.plugins.toolkit as toolkit
 import requests
+import yaml
 from ckan.common import _, config
 from dateutil import tz
 from flask import Blueprint, request
 from flask import Response, stream_with_context
 from werkzeug.datastructures import ImmutableMultiDict
 
 from ckanext.ids.dataspaceconnector.connector import Connector
 from ckanext.ids.dataspaceconnector.contract import Contract
 from ckanext.ids.dataspaceconnector.offer import Offer
 from ckanext.ids.dataspaceconnector.resource import Resource
 from ckanext.ids.dataspaceconnector.subscribe import Subscription
 from ckanext.ids.metadatabroker.client import graphs_to_artifacts
 from ckanext.ids.metadatabroker.client import graphs_to_ckan_result_format
 from ckanext.ids.metadatabroker.client import graphs_to_contracts
-from ckanext.ids.model import IdsResource, IdsAgreement, IdsSubscription
+from ckanext.ids.model import IdsResource, IdsAgreement, IdsSubscription, WorkflowExecution
 from ckanext.ids.activity import create_pushed_to_dataspace_connector_activity, create_created_contract_activity
 
 #dtheiler start
 from ckanext.ids.recomm.recomm import recomm_store_view_interaction
 from ckanext.ids.recomm.recomm import recomm_store_accept_contract_interaction
 from ckanext.ids.recomm.recomm import recomm_store_publish_interaction
 from ckanext.ids.recomm.recomm import recomm_store_download_interaction
@@ -75,14 +77,16 @@
 )
 
 log = logging.getLogger(__name__)
 
 trusts_recommender_plugin_name = "trusts_recommender"
 trusts_blockchain_plugin_name = "trusts_blockchain"
 
+input_parameter_pattern = "input-art-"
+
 def request_contains_mandatory_files():
     return request.files[
                'Deployment file (docker-compose.xml) - mandatory-upload'].filename != ''
 
 
 @ids.route('/dataset/<id>/resources/create', methods=['POST'])
 def create(id):
@@ -300,16 +304,16 @@
             #dtheiler end
     else:
         message = "This resource doesn't have any contracts, not pushing to broker"
         result = {"pushed" : False, "message": message}
         log.warn(message)
         return result
 
-    create_pushed_to_dataspace_connector_activity(context, data["id"])
-    message = "Asset successfully pushed to the TRUSTS Platform"
+    #create_pushed_to_dataspace_connector_activity(context, data["id"])
+    message = "Asset's metadata successfully pushed to the Metadata Broker"
     result = {"pushed": True, "message": message}
     log.info(message)
     return result
 
 
 def transform_url_internal_network(url: str,
                                    container_name: str = "local-ckan",
@@ -323,26 +327,25 @@
 
 def delete_from_dataspace_connector(data):
     c = plugins.toolkit.g
     context = {'model': model, 'session': model.Session,
                'user': c.user or c.author, 'auth_user_obj': c.userobj,
                }
     local_resource_dataspace_connector = Connector().get_resource_api()
-    catalog = config.get("ckanext.ids.connector_catalog_iri")
     offer = Offer(data)
     for value in data["resources"]:
         # this has also to run for every resource
         resource = Resource(value)
         if resource.representation_iri is not None:
             local_resource_dataspace_connector.delete_representation(resource)
         if resource.artifact_iri is not None:
             local_resource_dataspace_connector.delete_artifact(
                 resource.artifact_iri, data={})
     if offer.offer_iri is not None:
-        local_resource_dataspace_connector.delete_offered_resource(offer)
+        local_resource_dataspace_connector.delete_offered_resource(offer.offer_iri)
     return
 
 
 def transform_url(url):
     site_url = toolkit.config.get('ckan.site_url')
     log.info("Transforming url: %s", url)
     log.debug("ckan.site_url is set to: %s", site_url)
@@ -495,19 +498,16 @@
         dataset = toolkit.get_action('package_show')(context, {'id': id})
         log.info("Pushing to the local DSC, Done!")
         resource_id = dataset["offer_iri"]
     local_connector_resource_api.add_contract_to_resource(resource=resource_id,
 
                                                           contract=contract_id)
     log.debug("Contract added to resource")
-    log.info("Sending resource to broker")
-    bs = local_connector.send_resource_to_broker(resource_uri=resource_id)
-    log.info("Resource was sent to broker.")
-    create_created_contract_activity(context, dataset["id"])
-    return {"broker success": bs}
+    #create_created_contract_activity(context, dataset["id"])
+    return True
 
 
 @ids_actions.route('/ids/view/publish/<id>', methods=['GET', 'POST'])
 def publish(id, offering_info=None, errors=None):
     c = plugins.toolkit.g
     context = {'model': model, 'session': model.Session,
                'user': c.user or c.author, 'auth_user_obj': c.userobj,
@@ -713,14 +713,28 @@
         stream_with_context(data_response.iter_content(chunk_size=1024)),
         content_type=data_response.headers.get("Content-Type"),
         status=data_response.status_code
     )
     response.headers["Content-Disposition"] = "attachment;filename="+filename
     return response
 
+@ids_actions.route('/ids/actions/get_representations', methods=['GET'])
+def get_representations():
+    local_connector = Connector()
+    local_connector_resource_api = local_connector.get_resource_api()
+    resource_uri= request.args.get("resource_uri")
+    return local_connector_resource_api.get_representations_for_resource(resource_uri)
+
+@ids_actions.route('/ids/actions/get_artifacts', methods=['GET'])
+def get_artifacts():
+    local_connector = Connector()
+    local_connector_resource_api = local_connector.get_resource_api()
+    representation_uri= request.args.get("representation_uri")
+    return local_connector_resource_api.get_artifacts_for_representation(representation_uri)
+
 # endpoint to create a subscription
 @ids_actions.route('/ids/actions/subscribe', methods=['GET'])
 def subscribe():
     g = plugins.toolkit.g
     offer_url= request.args.get("offer_url")
     subscriber_email= g.userobj.email
 
@@ -758,14 +772,131 @@
 
 @ids_actions.route('/ids/actions/unsubscribe', methods=['GET'])
 def unsubscribe():
     subscription_url = request.args.get("subscription_url")
     subscription = IdsSubscription.get(subscription_url)
     subscription.delete()
 
+@ids_actions.route('/ids/actions/agreement/<id>/workflow/configure')
+def workflow_configuration(id):
+    resources = []
+    local_connector = Connector()
+    local_dsc_api = local_connector.get_resource_api()
+    agreement_uri = local_connector.url + "/api/agreements/" + id
+    artifacts = local_dsc_api.get_artifacts_for_agreement(agreement_uri)
+    workflow_artifact = [artifact for artifact in artifacts["_embedded"]["artifacts"] if artifact["title"]=="workflow.yml"][0]
+    service_artifact = [artifact for artifact in artifacts["_embedded"]["artifacts"] if artifact["title"]=="service_base_access_url"][0]
+    workflow_definition = yaml.load(local_dsc_api.get_data(workflow_artifact["_links"]["self"]["href"]).text, Loader=yaml.SafeLoader)
+    input_parameters = list(filter(input_parameters_filter, workflow_definition["spec"]["arguments"]["parameters"]))
+    requested_resources = local_dsc_api.get_requested_resources(size=100)
+    offered_resources = local_dsc_api.get_offered_resources(size=100)
+    resources = list(filter(dataset_resource_filter,requested_resources["_embedded"]["resources"])) + list(filter(dataset_resource_filter,offered_resources["_embedded"]["resources"]))
+
+    resource_options = [ {"value": resource["_links"]["self"]["href"], "text": resource["title"]} for resource in resources]
+    resource_options.insert(0, {"value":"", "text":""})
+    return toolkit.render("package/workflow_configuration.html",
+                          extra_vars={
+                              u'pkg_dict': {"type":"service", "name":"configure-workflow"},
+                              u'agreement': id,
+                              u'workflow_definition': workflow_definition,
+                              u'input_parameters':input_parameters,
+                              u'resource_options':resource_options,
+                              u'service_artifact':service_artifact
+                          })
+
+@ids_actions.route('/ids/actions/agreement/<id>/workflows', methods=['GET'])
+def workflow_executions_view(id):
+    local_connector = Connector()
+    local_dsc_api = local_connector.get_resource_api()
+    agreement_uri = local_connector.url + "/api/agreements/" + id
+    agreement = IdsAgreement.get(agreement_uri)
+    artifacts = local_dsc_api.get_artifacts_for_agreement(agreement_uri)
+    service_artifact = [artifact for artifact in artifacts["_embedded"]["artifacts"] if artifact["title"]=="service_base_access_url"][0]
+    workflows = agreement.get_workflows()
+    return toolkit.render("package/workflows.html",
+                          extra_vars={
+                              u'pkg_dict': {"type":"service", "name":"executions"},
+                              u'agreement':id,
+                              u'workflows':workflows,
+                              u'artifacts':artifacts,
+                              u'service_artifact':service_artifact
+                          })
+
+def input_artifacts_filter(key):
+    if input_parameter_pattern in key:
+        return True
+    else:
+        return False
+
+def input_parameters_filter(parameter):
+    if input_parameter_pattern in parameter["name"]:
+        return True
+    else:
+        return False
+
+def dataset_resource_filter(resource):
+    #TODO: fix the mapping, there should be only one normalized value
+    if (resource["additional"]["https://www.trusts-data.eu/ontology/asset_type"] == '{@id=https://www.trusts-data.eu/ontology/Dataset}') or (resource["additional"]["https://www.trusts-data.eu/ontology/asset_type"] == 'https://www.trusts-data.eu/ontology/Dataset'):
+        return True
+    else:
+        return False
+
+@ids_actions.route('/ids/actions/trigger_workflow', methods=['POST'])
+def workflow_trigger():
+
+    local_connector = Connector()
+    local_dsc_api = local_connector.get_resource_api()
+
+    agreement_id = request.form["agreementId"]
+    agreement_uri = local_connector.url + "/api/agreements/" + agreement_id
+    agreement = IdsAgreement.get(agreement_uri)
+    artifacts = local_dsc_api.get_artifacts_for_agreement(agreement_uri)
+
+    workflow_service_url = request.form["workflowTriggerArtifactId"]
+    input_keys = [form_input for form_input in request.form if input_parameter_pattern in form_input]
+    log.debug("Input Keys")
+    log.debug(input_keys)
+    log.debug("Creating workflow Execution")
+    workflow_artifact = [artifact for artifact in artifacts["_embedded"]["artifacts"] if artifact["title"]=="workflow.yml"][0]
+    workflow_definition = local_dsc_api.get_data(workflow_artifact["_links"]["self"]["href"])
+    files = {
+        "workflow":("workflow.yml", workflow_definition.text, "application/octet-stream")
+    }
+
+    for key in input_keys:
+        file = local_dsc_api.get_data(request.form[key])
+        file_description = local_dsc_api.get_artifact(request.form[key])
+        files[key] = (file_description["title"], file.content, "application/octet-stream")
+    workflow_execution_response = local_dsc_api.post_data(artifact=workflow_service_url, proxyPath="/submit", proxyFiles=files)
+
+    workflow_execution_object = workflow_execution_response.json()
+    workflow_execution = WorkflowExecution(str(uuid.uuid4()), agreement, None, workflow_execution_object["metadata"]["name"])
+    log.debug("Workflow execution created!")
+    workflow_execution.save()
+    log.debug("Workflow execution persisted!")
+    return "True"
+
+@ids_actions.route('/ids/actions/service_access', methods=['POST', 'GET'])
+def service_access():
+
+    service_access_url = request.args["service_access_url"]
+    workflow_name = request.args["workflowname"]
+    proxy_path = request.args["proxypath"]
+    local_connector = Connector()
+    local_dsc_api = local_connector.get_resource_api()
+    parameters = {"workflowname":workflow_name}
+    data_response = local_dsc_api.get_data(service_access_url,proxyPath=proxy_path, parameters=parameters)
+    response = Response(
+        stream_with_context(data_response.iter_content(chunk_size=1024)),
+        content_type=data_response.headers.get("Content-Type"),
+        status=data_response.status_code
+    )
+    response.headers["Content-Disposition"] = "attachment;filename="+proxy_path
+    return response
+
 
 def create_external_package(data):
     # get clean data from the form, data will hold the common meta for all resources
 
     # iterate through all resources and add them on the package
     # for resource in resources:
     #    toolkit.get_action('resource_create')(None, resource)
@@ -821,20 +952,14 @@
     External resources should have as URL this endpoint
     """
 
     c = plugins.toolkit.g
     context = {'model': model, 'session': model.Session,
                'user': c.user or c.author, 'auth_user_obj': c.userobj,
                }
-
-    # ToDo For now it assumes the DSC is accessible in the same hostname
-    # as the CKAN, but with port 8282
-    _dscbaseurl = config.get("ckan.site_url")
-    _dsc_hostname = urlsplit(_dscbaseurl).hostname.split(":")[0]
-    basedscurl = _dsc_hostname + ":8282"
     log.error("-:-:-:-:~~~~~~~~~~~~~~~~------------------------------>\n\n\n")
 
     # Ger from broker info for this ID
     resource_uri = request.args.get("uri")
     local_connector = Connector()
 
     graphs = local_connector.ask_broker_for_description(
@@ -862,21 +987,47 @@
             dataset["type"]) #entityType
         #dtheiler end
 
     try:
         local_agreements = local_resource.get_agreements()
     except AttributeError:
         local_agreements = []
+    agreements = get_agreements(local_agreements, local_connector)
+    local_artifacts = get_local_artifacts(local_agreements, local_connector)
+    if len(local_artifacts):
+        c.local_artifacts = local_artifacts
+        c.agreements=agreements
+    c.data = dataset
+    return toolkit.render('package/contracts_external.html',
+                          extra_vars={
+                              u'pkg_dict': dataset,
+                              u'dataset_type': dataset["type"]
+                          })
+
 
+def get_agreements(local_agreements, local_connector):
+    local_dsc_API = local_connector.get_resource_api()
+    agreements = []
+    for local_agreement in local_agreements:
+        agreement = local_dsc_API.get_agreement(local_agreement.id)
+        agreement["parsed_value"] = json.loads(agreement["value"])
+        agreements.append(agreement)
+    return agreements
+
+def get_local_artifacts(local_agreements, local_connector):
+    # as the CKAN, but with port 8282
+    _dscbaseurl = config.get("ckan.site_url")
+    _dsc_hostname = urlsplit(_dscbaseurl).hostname.split(":")[0]
+    basedscurl = _dsc_hostname + ":8282"
     local_dsc_API = local_connector.get_resource_api()
     local_artifacts = []
+
     for local_agreement in local_agreements:
         if local_agreement is not None:
             site_url = str(toolkit.config.get('ckan.site_url'))
-
             artifacts = local_dsc_API.get_artifacts_for_agreement(
                 local_agreement.id)
             log.debug("~~~~~~~~~~~\n|~\n|~\n|~")
             log.debug("\tagreement_uri: \t" + local_agreement.id)
             if "_embedded" in artifacts.keys():
                 for ar in artifacts["_embedded"]["artifacts"]:
 
@@ -890,32 +1041,19 @@
                     if "service_base_access_url" in arttitle:
                         url = basedscurl + "/api/artifacts/" + artifactuuid
                         accessurl = url + "/data"
                     else:
                         accessurl = \
                             site_url + "/ids/actions/get_data?artifact_id=" \
                                        "" + artifactuuid
-
-                    # log.debug("\t|\n\t\n\t|~~~~~~~~~~~>")
-                    # log.debug("\t\tartifact_uri :\t" + artifacturi)
-                    # log.debug("\t\taccessurl: \t" + accessurl)
-                    # log.debug("\t\ttitle: \t" + arttitle)
-                    # log.debug("\t\tdescription: \t" + artdesc)
-
                     artifact_description = {"url": accessurl}
                     artifact_description["title"] = arttitle
                     artifact_description["description"] = artdesc
                     if "title" in ar.keys() and len(ar["title"]) > 0:
                         artifact_description["title"] = ar["title"]
                     if "description" in ar.keys() and len(
                             ar["description"]) > 0:
                         artifact_description["description"] = ar["description"]
 
                     local_artifacts.append(artifact_description)
-
-    if len(local_artifacts):
-        c.local_artifacts = local_artifacts
-    c.data = dataset
-    return toolkit.render('package/contracts_external.html',
-                          extra_vars={
-                              u'pkg_dict': dataset
-                          })
+                return local_artifacts
+    return local_artifacts
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/connector.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,12 +245,12 @@
                 log.error("Something went wrong when sending announcment to "
                           "broker, retrying in 1s")
                 log.debug("\n| Will first force announce")
                 self.announce_to_broker(force=True)
                 log.debug("----------------\n|\n|\n")
                 time.sleep(1)
 
-            if attempts > 3:
-                log.error("10 attempts not push to broker failed")
+            if attempts > self.broker_knows_us_limit:
+                log.error("{} attempts not push to broker failed", str(self.broker_knows_us_limit))
                 return False
 
         return response.status_code < 299
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/contract.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/contract.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/idsapi.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/idsapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/offer.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/offer.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/resource.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/resource.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/resourceapi.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/resourceapi.py`

 * *Files 3% similar despite different names*

```diff
@@ -183,26 +183,51 @@
 
     def toListIfNeeded(self, obj):
         if isinstance(obj, list):
             return obj
         else:
             return [obj]
 
-    def get_data(self, artifact):
-        return self.session.get(artifact + "/data")
+    def get_data(self, artifact, proxyPath="", parameters=None):
+        if not "/data" in artifact:
+            proxyPath = "/data" + proxyPath
+        return self.session.get(artifact + proxyPath, params=parameters)
+
+    def post_data(self, artifact, proxyHeaders=None, proxyBody=None, proxyFiles=None, proxyPath=None, proxyData=None):
+        path = artifact + proxyPath
+        return self.session.post(path, data=proxyData, files=proxyFiles)
+
+    def get_agreement(self, agreement):
+        return json.loads(self.session.get(agreement).text)
+
+    def get_requested_resources(self, page=0, size=10):
+        parameters = {"page":page, "size":size}
+        url = self.recipient + "/api/requests"
+        return json.loads(self.session.get(url, params=parameters).text)
+
+    def get_offered_resources(self, page=0, size=10):
+        parameters = {"page":page, "size":size}
+        url = self.recipient + "/api/offers"
+        return json.loads(self.session.get(url, params=parameters).text)
 
     def get_artifacts_for_agreement(self, agreement):
         return json.loads(self.session.get(agreement + "/artifacts").text)
 
     def get_representations_for_artifact(self, artifact):
         return json.loads(self.session.get(artifact + "/representations").text)
 
     def get_requests_for_representation(self, representation):
         return json.loads(self.session.get(representation + "/requests").text)
 
+    def get_representations_for_resource(self, resource):
+        return json.loads(self.session.get(resource + "/representations").text)
+
+    def get_artifacts_for_representation(self, representation):
+        return json.loads(self.session.get(representation + "/artifacts").text)
+
     def descriptionRequest(self, recipient, elementId):
         url = self.recipient + "/api/ids/description"
         params = {}
         if recipient is not None:
             params["recipient"] = recipient
         if elementId is not None:
             params["elementId"] = elementId
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/subscribe.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/subscribe.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 from urllib.parse import urlparse
 from ckanext.ids.dataspaceconnector.resourceapi import ResourceApi
 from ckanext.ids.dataspaceconnector.subscriptionapi import SubscriptionApi
 from ckanext.ids.dataspaceconnector.idsapi import IdsApi
 
 log = logging.getLogger("ckanext.ids.dsc.subscribe")
 
-consumerUrl = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_url') + ":" + toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_port')
-username = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_username')
-password = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_password')
-consumer_alias = consumerUrl
-
-consumer = IdsApi(consumerUrl, auth=(username, password))
-local_node = toolkit.config.get("ckanext.ids.trusts_local_dataspace_connector_url")
+consumerUrl = None
+local_node = None
+consumer = None
+username = None
+password = None
+consumer_alias = None
 
 
 class Subscription:
     offer_url = None
     provider_alias = None
     agreement_url = None
     first_artifact = None
@@ -31,14 +30,21 @@
     route = None
 
 
     def __init__(self, offer_url, agreement, user_email):
         self.offer_url = offer_url
         self.agreement = agreement
         self.user_email = user_email
+        consumerUrl = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_url') + ":" + toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_port')
+        username = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_username')
+        password = toolkit.config.get('ckanext.ids.trusts_local_dataspace_connector_password')
+        consumer_alias = consumerUrl
+
+        consumer = IdsApi(consumerUrl, auth=(username, password))
+        local_node = toolkit.config.get("ckanext.ids.trusts_local_dataspace_connector_url")
 
         parsed_url = urlparse(offer_url)
         self.provider_alias = parsed_url.scheme + "://" + parsed_url.netloc
 
 
 # Consumer
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/dataspaceconnector/subscriptionapi.py` & `ckanext-ids-1.1.0/ckanext/ids/dataspaceconnector/subscriptionapi.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/harvester.py` & `ckanext-ids-1.1.0/ckanext/ids/harvester.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/helpers.py` & `ckanext-ids-1.1.0/ckanext/ids/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/i18n/ckanext-ids.pot` & `ckanext-ids-1.1.0/ckanext/ids/i18n/ckanext-ids.pot`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/i18n/en/LC_MESSAGES/ckanext-ids.po` & `ckanext-ids-1.1.0/ckanext/ids/i18n/en/LC_MESSAGES/ckanext-ids.po`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/logic/action.py` & `ckanext-ids-1.1.0/ckanext/ids/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/metadatabroker/client.py` & `ckanext-ids-1.1.0/ckanext/ids/metadatabroker/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,15 +101,15 @@
       SELECT ?resultUri ?type ?title ?description ?assettype ?externalname ?license ?creationDate
       WHERE
       { ?resultUri a ?type . 
         ?conn <https://w3id.org/idsa/core/offeredResource> ?resultUri .
         ?resultUri ids:title ?title .
         ?resultUri ids:description ?description .
         ?resultUri owl:sameAs ?externalname .
-        ?resultUri ids:standardLicense ?license .
+        OPTIONAL {  ?resultUri ids:standardLicense ?license . }
         OPTIONAl {  ?resultUri ids:created ?creationDateTemp . }
         BIND (str(coalesce(?creationDateTemp, "Not Specified")) as ?creationDate)
         FILTER (!regex(str(?externalname),\"""" + config.get(
         'ckanext.ids.local_node_name') + """\",\"i\"))
         """
     facet_filters = build_facet_filters(fq, facet_fields, dataset_schema)
     for facet_filter in facet_filters:
@@ -190,14 +190,15 @@
           WHERE
           { graph ?g
             {  
                 ?conn     ids:offeredResource   ?resultUri .
                 ?resultUri  owl:sameAs            ?externalname .
                 FILTER (!regex(str(?externalname),\"""" + config.get('ckanext.ids.local_node_name') + """\",\"i\"))               
                 OPTIONAL { ?resultUri ?facet ?facet_value }
+                OPTIONAL { ?resultUri ids:description ?description }
                 VALUES ?facet { """ + " ".join(facet_properties) + """ } """
     facet_filters = build_facet_filters(fq, facet_fields, dataset_schema)
     for facet_filter in facet_filters:
         query += facet_filter
     if resource_type is None or resource_type == "None":
         query += "\n ?resultUri " + URI(type_pred).n3() + " ?assettype."
     else:
@@ -286,16 +287,16 @@
         perms = cg["permission"]
         if not isinstance(perms, list):
             perms = [perms]
         r = dict()
         r["policies"] = [
             {"type": permission_graph_dict[per]["action"].upper().replace(
                 "-", "_")} for per in perms]
-        r["contract_start"] = cg["contractStart"]
-        r["contract_end"] = cg["contractEnd"]
+        r["start"] = cg["contractStart"]
+        r["end"] = cg["contractEnd"]
         r["title"] = clean_multilang(resource_graphs[0]["title"])
         r["errors"] = {}
         r["provider_url"] = providing_base_url
         r["resourceId"] = resource_uri
         r["artifactId"] = artifact_graphs[0]["sameAs"]
         r["artifactIds"] = [x["sameAs"] for x in artifact_graphs]
         r["contractId"] = cg["sameAs"]
@@ -342,22 +343,22 @@
 
     lictit = ""
     if "http://" or "https://" in license:
         lictit = license.split("/")[-1]
 
     packagemeta = deepcopy(empty_result)
     packagemeta["id"] = resultUri
-    packagemeta["license_id"] = license + "LICENSE"
-    packagemeta["license_url"] = license + "LICENSE"
+    packagemeta["license_id"] = license
+    packagemeta["license_url"] = license
     packagemeta["license_title"] = lictit
     packagemeta["metadata_created"] = creationDate
     packagemeta["metadata_modified"] = datetime.datetime.now().isoformat()
     packagemeta["name"] = title
     packagemeta["title"] = title
-    packagemeta["description"] = description + "DESCRIPTION"
+    packagemeta["description"] = description
     packagemeta["type"] = assetType.split("/")[
         -1].lower()
     packagemeta["theme"] = "THEME"
     packagemeta["version"] = "VERSION"
 
     # These are the values we will use in succesive steps
     packagemeta["external_provider_name"] = organization_name
@@ -367,15 +368,15 @@
                                              resultUri)
     packagemeta["provider_base_url"] = providing_base_url
 
     packagemeta["creator_user_id"] = "X"
     packagemeta["isopen"]: None
     packagemeta["maintainer"] = None
     packagemeta["maintainer_email"] = None
-    packagemeta["notes"] = None
+    packagemeta["notes"] = description
     packagemeta["num_tags"] = 0
     packagemeta["private"] = False
     packagemeta["state"] = "active"
     packagemeta["relationships_as_object"] = []
     packagemeta["relationships_as_subject"] = []
     packagemeta["url"] = providing_base_url
     packagemeta["tags"] = []  # (/)
@@ -427,16 +428,14 @@
         return str(astring["@value"])
     return str(astring)
 
 
 def graphs_to_ckan_result_format(raw_jsonld: Dict):
     g = raw_jsonld["@graph"]
     resource_graphs = [x for x in g if x["@type"] == "ids:Resource"]
-    if "theme" not in resource_graphs[0].keys():
-        return None
     representation_graphs = [x for x in g if
                              x["@type"] == "ids:Representation"]
     artifact_graphs = [x for x in g if x["@type"] == "ids:Artifact"]
 
     resource_uri = resource_graphs[0]["sameAs"]
 
     """
@@ -478,30 +477,44 @@
         "standardLicense"] if "standardLicense" in resource_graphs[0] else None
     packagemeta["metadata_created"] = resource_graphs[0]["created"]
     packagemeta["metadata_modified"] = resource_graphs[0]["modified"]
     packagemeta["name"] = clean_multilang(resource_graphs[0]["title"])
     packagemeta["title"] = clean_multilang(resource_graphs[0]["title"])
     packagemeta["type"] = resource_graphs[0]["asset_type"].split("/")[
         -1].lower()
-    packagemeta["theme"] = resource_graphs[0]["theme"].split("/")[-1]
+
+    schema_fields = scheming_get_schema("dataset", packagemeta["type"], True)
+    excluded_fields = [
+        'id',
+        'title',
+        'name',
+        'notes',
+        'tag_string',
+        'license_id',
+        'owner_org',
+    ]
+    for field in schema_fields["dataset_fields"]:
+        field_name = field["field_name"]
+        if field_name not in excluded_fields and field_name in resource_graphs[0]:
+            packagemeta[field_name] = clean_multilang(resource_graphs[0][field_name])
     packagemeta["version"] = resource_graphs[0]["version"]
 
     # These are the values we will use in succesive steps
     packagemeta["external_provider_name"] = organization_name
     packagemeta["to_process_external"] = config.get(
         "ckan.site_url") + "/ids/processExternal?uri=" + \
                                          urllib.parse.quote_plus(
                                              resource_uri)
     packagemeta["provider_base_url"] = providing_base_url
 
     packagemeta["creator_user_id"] = "X"
     packagemeta["isopen"]: None
     packagemeta["maintainer"] = None
     packagemeta["maintainer_email"] = None
-    packagemeta["notes"] = None
+    packagemeta["notes"] = clean_multilang(resource_graphs[0]["description"])
     packagemeta["num_tags"] = 0
     packagemeta["private"] = False
     packagemeta["state"] = "active"
     packagemeta["relationships_as_object"] = []
     packagemeta["relationships_as_subject"] = []
     packagemeta["url"] = providing_base_url
     packagemeta["tags"] = []  # (/)
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/metadatabroker/translations_broker_ckan.py` & `ckanext-ids-1.1.0/ckanext/ids/metadatabroker/translations_broker_ckan.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/plugin.py` & `ckanext-ids-1.1.0/ckanext/ids/plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from ckanext.ids.recomm.recomm import recomm_recomm_services_sidebar
 #dtheiler end
 
 from ckanext.ids.helpers import check_if_contract_offer_exists, has_more_facets, get_facet_items_dict, string_to_json
 from ckanext.scheming.helpers import scheming_get_schema, scheming_field_by_name
 from ckanext.vocabularies.helpers import skos_choices_sparql_helper, skos_choices_get_label_by_value
 
+## Take a look in https://github.com/ckan/ckan/issues/5865 and https://github.com/ckan/ckan/blob/master/ckanext/activity/logic/validators.py
+#from ckan.logic import validators as core_validators
+
 # ToDo make sure this logger is set higher
 log = logging.getLogger("ckanext")
 
 #dtheiler start
 def recomm_datasets_homepage(count):
     return recomm_recomm_datasets_homepage(count)
 
@@ -75,33 +78,39 @@
             "trusts_url_validator": validator.trusts_url_validator,
             "object_id_validator": validator.object_id_validator,
             "activity_type_exists": validator.activity_type_exists
         }
 
     from ckanext.ids.model import setup as db_setup
 
+
     db_setup()
 
     # IConfigurer
     def update_config(self, config_):
         toolkit.add_template_directory(config_, 'templates')
         toolkit.add_public_directory(config_, 'public')
         toolkit.add_resource('assets',
                              'ckanext-ids')
 
+        #core_validators.object_id_validators['created contract'] = core_validators.package_id_exists
+        #core_validators.object_id_validators['pushed to dataspace connector'] = core_validators.package_id_exists
+
     def update_config_schema(self, schema):
         ignore_missing = toolkit.get_validator('ignore_missing')
         is_boolean = toolkit.get_validator('boolean_validator')
+        is_positive_integer = toolkit.get_validator('is_positive_integer')
 
         schema.update({
             # This is an existing CKAN core configuration option, we are just
             # making it available to be editable at runtime
             'ckan.search.show_all_types': [ignore_missing, is_boolean],
             'ckanext.ids.connector_catalog_iri': [ignore_missing],
             'ckanext.ids.usage_control_policies': [ignore_missing]
+            #'ckan.max_resource_size': [ignore_missing, is_positive_integer]
 
         })
 
         return schema
     # before rendering organization view
     def before_view(self, organization):
         log.debug("\n................ Before View ................\n+")
@@ -273,21 +282,23 @@
     def before_dataset_search(self, search_params):
         return search_params
 
     def after_dataset_search(self, search_results, search_params):
         context = plugins.toolkit.g
 
         if context.view == "search":
+            if context.blueprint == "dataset":
+                search_params["fq"].append("+dataset_type:dataset +state:(active)")
             results_from_broker = self.retrieve_results_from_broker(search_params)
             if len(results_from_broker) > 0:
                search_results["results"] = results_from_broker["results"]
                search_results["count"] = results_from_broker["count"]
                search_results["facets"] = results_from_broker["facets"]
                search_results["search_facets"] = self.retrieve_facet_labels(results_from_broker["search_facets"])
-        #TODO: check if this is still needed, for now it does not work on CKAN 2.10.0
+        #TODO: check if this is still needed, for now it does not work on CKAN 2.10.0 sss
         #if context.view == "read":
         #    results_from_broker = self.retrieve_results_from_broker(search_params)
         #    if len(results_from_broker) > 0:
         #        search_results["results"].extend(results_from_broker["results"])
         #        search_results["count"] += results_from_broker["count"]
         #        search_results["facets"] = self.merge_facets(search_results["facets"], results_from_broker["facets"])
         #        search_results["search_facets"] = self.merge_search_facets(search_results["search_facets"], results_from_broker["search_facets"])
@@ -412,8 +423,43 @@
     plugins.implements(plugins.IBlueprint)
 
     def get_blueprint(self):
         return [blueprints.trusts_recommender]
 
 
 class TrustsBlockchainPlugin(plugins.SingletonPlugin):
-    pass
+    pass
+
+
+class DevPlugin(plugins.SingletonPlugin):
+    """Development plugin.
+    This plugin provides:
+    - Start remote debugger (if correct library is present) during update_config call
+    """
+
+    plugins.implements(plugins.IConfigurer, inherit=True)
+
+    def update_config(self, config):
+        self._start_debug_client(config)
+
+    def _start_debug_client(self, config):
+        try:
+            log.info("Trying to load the pydevd library.")
+            import pydevd
+        except ImportError:
+            log.error("Failed to load the pydedv library.")
+            pass
+
+        host_ip = config.get('debug.remote.host.ip', '172.20.0.1')
+        host_port = config.get('debug.remote.host.port', '64342')
+        stdout = toolkit.asbool(config.get('debug.remote.stdout_to_server', 'True'))
+        stderr = toolkit.asbool(config.get('debug.remote.stderr_to_server', 'True'))
+        suspend = toolkit.asbool(config.get('debug.remote.suspend', 'False'))
+
+        try:
+            log.info("Initiating remote debugging session to {}:{}".format(host_ip, host_port))
+            pydevd.settrace(host_ip, port=int(host_port), stdoutToServer=stdout, stderrToServer=stderr, suspend=suspend)
+            log.info("Successfully started debugging session...")
+        except NameError:
+            log.warning("debug.enabled set to True, but pydevd is missing.")
+        except SystemExit:
+            log.warning("Failed to connect to debug server; is it started?")
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/public/api/swagger/ckan_ids_openapi.json` & `ckanext-ids-1.1.0/ckanext/ids/public/api/swagger/ckan_ids_openapi.json`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/recomm/recomm.py` & `ckanext-ids-1.1.0/ckanext/ids/recomm/recomm.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/schemes/application.yml` & `ckanext-ids-1.1.0/ckanext/ids/schemes/application.yml`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/schemes/dataset.yml` & `ckanext-ids-1.1.0/ckanext/ids/schemes/dataset.yml`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/schemes/organization.yml` & `ckanext-ids-1.1.0/ckanext/ids/schemes/organization.yml`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/schemes/presets.json` & `ckanext-ids-1.1.0/ckanext/ids/schemes/presets.json`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/schemes/service.yml` & `ckanext-ids-1.1.0/ckanext/ids/schemes/service.yml`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/smart_contracts/smart_contract_client.py` & `ckanext-ids-1.1.0/ckanext/ids/smart_contracts/smart_contract_client.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/swagger.py` & `ckanext-ids-1.1.0/ckanext/ids/swagger.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/form-snippets/slug.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/form-snippets/slug.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/index.template.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/index.template.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/macros/custom_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/macros/custom_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/organization/read.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/organization/read.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/organization/snippets/organization_item.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/organization/snippets/organization_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/base_form_page.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/base_form_page.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/contracts.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/contracts.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/publish.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/publish.html`

 * *Files 15% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 {% block title %}Publish {{ dataset_type }} - {{ super() }}{% endblock %}
 
 {% block secondary_content %}
 
     {{ super() }}
 
     <section class="module module-narrow module-shallow">
-        <h2 class="module-heading"><i class="icon-info-sign fa fa-info-circle"></i>{% trans %}Publish Dataset in the TRUSTS Dataspace{% endtrans %}</h2>
+        <h2 class="module-heading"><i class="icon-info-sign fa fa-info-circle"></i> {% trans %}Create a new Contract{% endtrans %}</h2>
         <div class="module-content">
             <p>
-                A resource is published on the TRUSTS broker only after having at least one contract offer. Please use the form to create one.
+                Asset's metadata can be published on the Metadata Broker only after having at least one contract offer. Please use the form to create one.
             </p>
         </div>
     </section>
 
 {% endblock %}
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/contract_item.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/contract_item.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <li class="resource-item" data-id="{{ contract.id }}">
     {% set contract_url = url if not 'external_provider_name' in pkg else "#" %}
-    {% set policies = h.string_to_json(contract.additional.policies) %}
+    {% set policies = h.string_to_json(contract.additional.policies) if "additional" in contract else contract.policies  %}
     {% block contract_item_title %}
         <a class="heading" href="{{ contract_url }}" title="{{ contract.title }}">
             {{ contract.title    }}
         </a>
     {% endblock %}
     {% block contract_dates %}
         <div> <b>Start date:</b> {{ contract.start }}</div>
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/contracts_list.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/contracts_list.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/package_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/package_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/resource_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/resource_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/resources_list.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/resources_list.html`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
   {% snippet "package/snippets/resources_list.html", pkg=pkg, resources=pkg.resources %}
 
 #}
 <section id="dataset-resources" class="resources">
     {% if not 'external_provider_name' in pkg %}
         {% if h.check_access('resource_create', {'package_id': pkg['id']}) and not is_activity_archive %}
-            {% link_for _('Push to TRUSTS platform'),
+            {% link_for _('Push metadata to the Medata Broker'),
         named_route='ids_actions.push_package_view', id=pkg['id'], class_='btn btn-success', icon='layer-forward' %}
         {% endif %}
     {% endif %}
     <h2>{{ _('Data and Resources') }}</h2>
     {% block resource_list %}
         {% if resources %}
             <ul class="{% block resource_list_class %}resource-list{% endblock %}">
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
 {# Renders a list of resources with icons and view links. resources - A list of
 resources (dicts) to render pkg - A package dict that the resources belong to.
 is_activity_archive - Whether this is an old version of the dataset (and
 therefore read-only) Example: {% snippet "package/snippets/
 resources_list.html", pkg=pkg, resources=pkg.resources %} #} {% if not
 'external_provider_name' in pkg %} {% if h.check_access('resource_create',
 {'package_id': pkg['id']}) and not is_activity_archive %} {% link_for _('Push
-to TRUSTS platform'), named_route='ids_actions.push_package_view', id=pkg
-['id'], class_='btn btn-success', icon='layer-forward' %} {% endif %} {% endif
-%}
+metadata to the Medata Broker'), named_route='ids_actions.push_package_view',
+id=pkg['id'], class_='btn btn-success', icon='layer-forward' %} {% endif %} {%
+endif %}
 ********** {{{{ __((''DDaattaa aanndd RReessoouurrcceess'')) }}}} **********
 {% block resource_list %} {% if resources %}
     * {% block resource_list_inner %} {% set can_edit = h.check_access
       ('package_update', {'id':pkg.id }) and not is_activity_archive %} {% for
       resource in resources %} {% snippet 'package/snippets/
       resource_item.html', pkg=pkg, res=resource, can_edit=can_edit,
       is_activity_archive=is_activity_archive %} {% endfor %} {% endblock %}
```

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/stages.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/stages.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/package/snippets/storepublisher_publish_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/package/snippets/storepublisher_publish_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/datetime_tz.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/datetime_tz.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/disabled.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/disabled.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/duration.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/duration.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/number.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/number.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/form_snippets/upload.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/form_snippets/upload.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/scheming/package/snippets/resource_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/scheming/package/snippets/resource_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/snippets/activities/created_contract.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/snippets/activities/created_contract.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/snippets/activities/pushed_to_dataspace_connector.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/snippets/activities/pushed_to_dataspace_connector.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/snippets/organization.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/snippets/organization.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates/snippets/resource_fields.html` & `ckanext-ids-1.1.0/ckanext/ids/templates/snippets/resource_fields.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/layout1.html` & `ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/layout1.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates_recommender/home/snippets/recomm_homepage.html` & `ckanext-ids-1.1.0/ckanext/ids/templates_recommender/home/snippets/recomm_homepage.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/snippets/recomm_entity_sidebar.html` & `ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/snippets/recomm_entity_sidebar.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates_recommender/package/snippets/resource_item.html` & `ckanext-ids-1.1.0/ckanext/ids/templates_recommender/package/snippets/resource_item.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/templates_recommender/snippets/search_form.html` & `ckanext-ids-1.1.0/ckanext/ids/templates_recommender/snippets/search_form.html`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/tests/test_plugin.py` & `ckanext-ids-1.1.0/ckanext/ids/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/usage_control.json` & `ckanext-ids-1.1.0/ckanext/ids/usage_control.json`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext/ids/validator.py` & `ckanext-ids-1.1.0/ckanext/ids/validator.py`

 * *Files identical despite different names*

### Comparing `ckanext-ids-1.0.9/ckanext_ids.egg-info/PKG-INFO` & `ckanext-ids-1.1.0/ckanext_ids.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: ckanext-ids
-Version: 1.0.9
+Version: 1.1.0
 Summary: IDS data model extension for CKAN
 Home-page: https://github.com/semantic-web-company/ckanext-ids
 Author: Sotiris Karampatakis
 Author-email: sotiris.karampatakis@semantic-web.com
 License: AGPL
 Keywords: CKAN IDS
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Tests](https://github.com/semantic-web-company/ckanext-ids/workflows/Tests/badge.svg?branch=main)](https://github.com/semantic-web-company/ckanext-ids/actions)
@@ -140,9 +139,7 @@
 
 [AGPL](https://www.gnu.org/licenses/agpl-3.0.en.html)
 
 ## Funding
 This code was created as part of project TRUSTS: Trusted secure data sharing space.
 
 This project has received funding from the European Union's Horizon 2020 research and innovation programme under grant agreement [No 871481](https://cordis.europa.eu/project/id/871481).
-
-
```

### Comparing `ckanext-ids-1.0.9/ckanext_ids.egg-info/SOURCES.txt` & `ckanext-ids-1.1.0/ckanext_ids.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,48 +33,57 @@
 ckanext/ids/logic/__init__.py
 ckanext/ids/logic/action.py
 ckanext/ids/metadatabroker/__init__.py
 ckanext/ids/metadatabroker/client.py
 ckanext/ids/metadatabroker/translations_broker_ckan.py
 ckanext/ids/model/__init__.py
 ckanext/ids/public/api/swagger/ckan_ids_openapi.json
+ckanext/ids/public/api/swagger/ckan_ids_openapi.yaml
+ckanext/ids/public/images/TrustsLogo.png
 ckanext/ids/recomm/__init__.py
 ckanext/ids/recomm/recomm.py
 ckanext/ids/schemes/application.yml
 ckanext/ids/schemes/dataset.yml
 ckanext/ids/schemes/organization.yml
 ckanext/ids/schemes/presets.json
 ckanext/ids/schemes/service.yml
 ckanext/ids/smart_contracts/__init__.py
 ckanext/ids/smart_contracts/smart_contract_client.py
 ckanext/ids/templates/base.html
 ckanext/ids/templates/header.html
 ckanext/ids/templates/index.template.html
+ckanext/ids/templates/admin/config.html
 ckanext/ids/templates/form-snippets/slug.html
 ckanext/ids/templates/macros/custom_form.html
 ckanext/ids/templates/organization/read.html
 ckanext/ids/templates/organization/snippets/organization_item.html
 ckanext/ids/templates/package/base_form_page.html
 ckanext/ids/templates/package/contracts.html
 ckanext/ids/templates/package/contracts_external.html
 ckanext/ids/templates/package/edit_base.html
 ckanext/ids/templates/package/publish.html
+ckanext/ids/templates/package/workflow_configuration.html
+ckanext/ids/templates/package/workflows.html
+ckanext/ids/templates/package/snippets/agreements_table.html
 ckanext/ids/templates/package/snippets/contract_item.html
 ckanext/ids/templates/package/snippets/contracts_list.html
 ckanext/ids/templates/package/snippets/package_form.html
 ckanext/ids/templates/package/snippets/resource_form.html
+ckanext/ids/templates/package/snippets/resource_item.html
 ckanext/ids/templates/package/snippets/resources_list.html
 ckanext/ids/templates/package/snippets/stages.html
 ckanext/ids/templates/package/snippets/storepublisher_publish_form.html
+ckanext/ids/templates/package/snippets/workflows_table.html
 ckanext/ids/templates/scheming/form_snippets/datetime_tz.html
 ckanext/ids/templates/scheming/form_snippets/disabled.html
 ckanext/ids/templates/scheming/form_snippets/duration.html
 ckanext/ids/templates/scheming/form_snippets/number.html
 ckanext/ids/templates/scheming/form_snippets/upload.html
 ckanext/ids/templates/scheming/organization/group_form.html
+ckanext/ids/templates/scheming/package/snippets/additional_info.html
 ckanext/ids/templates/scheming/package/snippets/resource_form.html
 ckanext/ids/templates/snippets/add_dataset.html
 ckanext/ids/templates/snippets/organization.html
 ckanext/ids/templates/snippets/package_item.html
 ckanext/ids/templates/snippets/resource_fields.html
 ckanext/ids/templates/snippets/activities/created_contract.html
 ckanext/ids/templates/snippets/activities/pushed_to_dataspace_connector.html
```

### Comparing `ckanext-ids-1.0.9/setup.py` & `ckanext-ids-1.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='''ckanext-ids''',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # http://packaging.python.org/en/latest/tutorial.html#version
-    version='1.0.9',
+    version='1.1.0',
 
     description='''IDS data model extension for CKAN''',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://github.com/semantic-web-company/ckanext-ids',
@@ -86,14 +86,15 @@
         [ckan.plugins]
         ids=ckanext.ids.plugin:IdsPlugin
         ids_job=ckanext.ids.plugin:IdsDummyJobPlugin
         ids_resources=ckanext.ids.plugin:IdsResourcesPlugin
         trusts_harvester=ckanext.ids.harvester:TrustsHarvester
         trusts_recommender=ckanext.ids.plugin:TrustsRecommenderPlugin
         trusts_blockchain=ckanext.ids.plugin:TrustsBlockchainPlugin
+        trusts_dev=ckanext.ids.plugin:DevPlugin
         [babel.extractors]
         ckan = ckan.lib.extract:extract_ckan
     ''',
 
     # If you are changing from the default layout of your extension, you may
     # have to change the message extractors, you can read more about babel
     # message extraction at
```

