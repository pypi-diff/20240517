# Comparing `tmp/connectpyse-0.6.0.5.tar.gz` & `tmp/connectpyse-0.6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connectpyse-0.6.0.5.tar", last modified: Fri Jan 26 03:50:45 2024, max compression
+gzip compressed data, was "connectpyse-0.6.0.6.tar", last modified: Fri May 17 21:06:01 2024, max compression
```

## Comparing `connectpyse-0.6.0.5.tar` & `connectpyse-0.6.0.6.tar`

### file list

```diff
@@ -1,199 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.915614 connectpyse-0.6.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-26 03:50:45.915614 connectpyse-0.6.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.887614 connectpyse-0.6.0.5/connectpyse/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.891614 connectpyse-0.6.0.5/connectpyse/company/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/companies_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_management_summary_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_management_summary_reports_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_site.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_teams_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/company_types_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configuration_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configuration_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configuration_type_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configuration_types_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/configurations_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_communications_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_department.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_note.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_track.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contact_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/company/contacts_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/cw_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/cw_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.891614 connectpyse-0.6.0.5/connectpyse/expense/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/expense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/expense/expense_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/expense/expense_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.895614 connectpyse-0.6.0.5/connectpyse/finance/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/accounting_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/accounting_batch_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_expense.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_procurement.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_addition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_additions_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_board_default.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_work_role.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_work_role_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_work_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreement_work_type_exclusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/agreements_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/currency.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/invoice_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/finance/tax_code_x_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.899614 connectpyse-0.6.0.5/connectpyse/marketing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_email_opened.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_form_submitted.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_link_clicked.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/campaign_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/group_company.py
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/marketing/group_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.903614 connectpyse-0.6.0.5/connectpyse/procurement/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/adjustment_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/adjustment_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/catalog_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/catalog_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/catalog_item_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/category.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/manufacturer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/product_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/product_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/product_item_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/product_picking_shipping_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_line_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_line_item_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_status_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/shipment_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/procurement/shipment_methods_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.903614 connectpyse-0.6.0.5/connectpyse/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/project_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/project_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/project_phase.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/project_team_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/project/projects_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/restapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.903614 connectpyse-0.6.0.5/connectpyse/sales/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/activity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/activity_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/activity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_contact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_forecast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_note.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_rating.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_team.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/opportunity_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/order_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/sales/order_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.907614 connectpyse-0.6.0.5/connectpyse/schedule/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_reminder_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_reminder_times_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_statuses_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/schedule/schedule_types_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.911614 connectpyse-0.6.0.5/connectpyse/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_excluded_member.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_sub_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_team.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/board_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/boards_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/code.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/knowledge_base_article.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/priority.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/source.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/survey.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/survey_question.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/survey_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/ticket_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/ticket_notes_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/ticket_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/service/tickets_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.911614 connectpyse-0.6.0.5/connectpyse/system/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/audit_trail.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/callbacks_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/connectwise_hosted_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/document_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/info.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/link.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/members_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/menu_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/product.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/system/user_defined_field.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.915614 connectpyse-0.6.0.5/connectpyse/time/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/activity_stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/charge_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/schedule_stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/ticket_stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/time_entries_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/time_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/time_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/connectpyse/time/time_sheets_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 03:50:45.915614 connectpyse-0.6.0.5/connectpyse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-26 03:50:45.000000 connectpyse-0.6.0.5/connectpyse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 03:50:45.915614 connectpyse-0.6.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-01-26 03:50:38.000000 connectpyse-0.6.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.269121 connectpyse-0.6.0.6/connectpyse/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.277120 connectpyse-0.6.0.6/connectpyse/company/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/companies_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_management_summary_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_management_summary_reports_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_teams_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/company_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configuration_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configuration_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configuration_type_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configuration_types_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/configurations_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_communications_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_department.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contact_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/company/contacts_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/cw_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/cw_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.277120 connectpyse-0.6.0.6/connectpyse/expense/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/expense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/expense/expense_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/expense/expense_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.281121 connectpyse-0.6.0.6/connectpyse/finance/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/accounting_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/accounting_batch_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_expense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_procurement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_addition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_additions_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_board_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_work_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_work_role_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_work_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreement_work_type_exclusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/agreements_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/currency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/invoice_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/finance/tax_code_x_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.285121 connectpyse-0.6.0.6/connectpyse/marketing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_email_opened.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_form_submitted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_link_clicked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/campaign_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/group_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/marketing/group_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.289121 connectpyse-0.6.0.6/connectpyse/procurement/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/adjustment_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/adjustment_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/catalog_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/catalog_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/catalog_item_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/manufacturer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/product_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/product_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/product_item_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/product_picking_shipping_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_line_item_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/shipment_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/procurement/shipment_methods_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.289121 connectpyse-0.6.0.6/connectpyse/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/project_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/project_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/project_phase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/project_team_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/project/projects_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5694 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/restapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.293120 connectpyse-0.6.0.6/connectpyse/sales/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/activity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/activity_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/activity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_forecast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_rating.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/opportunity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/order_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/sales/order_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.293120 connectpyse-0.6.0.6/connectpyse/schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_reminder_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_reminder_times_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_statuses_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/schedule/schedule_types_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.297120 connectpyse-0.6.0.6/connectpyse/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_excluded_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_sub_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/board_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/boards_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/boards_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/knowledge_base_article.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/priority.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/survey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/survey_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/survey_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/ticket_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/ticket_notes_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/ticket_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/service/tickets_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/connectpyse/system/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/audit_trail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/callbacks_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/connectwise_hosted_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/document_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/members_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/menu_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/system/user_defined_field.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/connectpyse/time/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/activity_stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/charge_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/schedule_stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/ticket_stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/time_entries_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/time_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/time_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/connectpyse/time/time_sheets_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/connectpyse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 21:06:01.000000 connectpyse-0.6.0.6/connectpyse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 21:06:01.301121 connectpyse-0.6.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-17 21:05:57.000000 connectpyse-0.6.0.6/setup.py
```

### Comparing `connectpyse-0.6.0.5/LICENSE` & `connectpyse-0.6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/PKG-INFO` & `connectpyse-0.6.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectpyse
-Version: 0.6.0.5
+Version: 0.6.0.6
 Summary: A ConnectWise API tool for the rest of us.
 Home-page: https://github.com/markciecior/ConnectPyse
 Author: Joshua M Smith (original), Mark Ciecior (forked), @wesgann
 Author-email: saether@gmail.com (original), mark@markciecior.com (forked)
 License: MIT
 Keywords: connectwise rest api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `connectpyse-0.6.0.5/README.md` & `connectpyse-0.6.0.6/README.md`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/__init__.py` & `connectpyse-0.6.0.6/connectpyse/__init__.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/companies_api.py` & `connectpyse-0.6.0.6/connectpyse/company/companies_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company.py` & `connectpyse-0.6.0.6/connectpyse/company/company.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_management_summary_report.py` & `connectpyse-0.6.0.6/connectpyse/company/company_management_summary_report.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_management_summary_reports_api.py` & `connectpyse-0.6.0.6/connectpyse/company/company_management_summary_reports_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_site.py` & `connectpyse-0.6.0.6/connectpyse/company/company_site.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_status.py` & `connectpyse-0.6.0.6/connectpyse/company/company_status.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_statuses_api.py` & `connectpyse-0.6.0.6/connectpyse/company/company_statuses_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_team.py` & `connectpyse-0.6.0.6/connectpyse/company/company_team.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_teams_api.py` & `connectpyse-0.6.0.6/connectpyse/company/company_teams_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/company_types_api.py` & `connectpyse-0.6.0.6/connectpyse/company/company_types_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/configuration.py` & `connectpyse-0.6.0.6/connectpyse/company/configuration.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/configuration_type_question.py` & `connectpyse-0.6.0.6/connectpyse/company/configuration_type_question.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/configuration_types_api.py` & `connectpyse-0.6.0.6/connectpyse/company/configuration_types_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/configurations_api.py` & `connectpyse-0.6.0.6/connectpyse/company/configurations_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/contact.py` & `connectpyse-0.6.0.6/connectpyse/company/contact.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/contact_communication.py` & `connectpyse-0.6.0.6/connectpyse/company/contact_communication.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/contact_communications_api.py` & `connectpyse-0.6.0.6/connectpyse/company/contact_communications_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/contact_track.py` & `connectpyse-0.6.0.6/connectpyse/company/contact_track.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/company/contacts_api.py` & `connectpyse-0.6.0.6/connectpyse/company/contacts_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/config.py` & `connectpyse-0.6.0.6/connectpyse/config.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/cw_controller.py` & `connectpyse-0.6.0.6/connectpyse/cw_controller.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/expense/expense_entry.py` & `connectpyse-0.6.0.6/connectpyse/expense/expense_entry.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/expense/expense_type.py` & `connectpyse-0.6.0.6/connectpyse/expense/expense_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/accounting_batch.py` & `connectpyse-0.6.0.6/connectpyse/finance/accounting_batch.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/accounting_batch_transaction.py` & `connectpyse-0.6.0.6/connectpyse/finance/accounting_batch_transaction.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_expense.py` & `connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_expense.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_invoice.py` & `connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_invoice.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/accounting_unposted_procurement.py` & `connectpyse-0.6.0.6/connectpyse/finance/accounting_unposted_procurement.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement_addition.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement_addition.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement_additions_api.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement_additions_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement_type.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement_work_role.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement_work_role.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreement_work_type.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreement_work_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/agreements_api.py` & `connectpyse-0.6.0.6/connectpyse/finance/agreements_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/currency.py` & `connectpyse-0.6.0.6/connectpyse/finance/currency.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/invoice.py` & `connectpyse-0.6.0.6/connectpyse/finance/invoice.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/tax_code.py` & `connectpyse-0.6.0.6/connectpyse/finance/tax_code.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/finance/tax_code_x_ref.py` & `connectpyse-0.6.0.6/connectpyse/finance/tax_code_x_ref.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/marketing/campaign.py` & `connectpyse-0.6.0.6/connectpyse/marketing/campaign.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/marketing/campaign_form_submitted.py` & `connectpyse-0.6.0.6/connectpyse/marketing/campaign_form_submitted.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/adjustment.py` & `connectpyse-0.6.0.6/connectpyse/procurement/adjustment.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/adjustment_detail.py` & `connectpyse-0.6.0.6/connectpyse/procurement/adjustment_detail.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/catalog_component.py` & `connectpyse-0.6.0.6/connectpyse/procurement/catalog_component.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/catalog_item.py` & `connectpyse-0.6.0.6/connectpyse/procurement/catalog_item.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/catalog_item_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/catalog_item_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/category.py` & `connectpyse-0.6.0.6/connectpyse/procurement/category.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/manufacturer_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/manufacturer_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/product_component.py` & `connectpyse-0.6.0.6/connectpyse/procurement/product_component.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/product_item.py` & `connectpyse-0.6.0.6/connectpyse/procurement/product_item.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/product_item_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/product_item_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/product_picking_shipping_detail.py` & `connectpyse-0.6.0.6/connectpyse/procurement/product_picking_shipping_detail.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_line_item.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_line_item.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_line_item_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_line_item_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_status.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_status.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/purchase_order_status_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/purchase_order_status_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/procurement/shipment_methods_api.py` & `connectpyse-0.6.0.6/connectpyse/procurement/shipment_methods_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/project/project.py` & `connectpyse-0.6.0.6/connectpyse/project/project.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/project/project_phase.py` & `connectpyse-0.6.0.6/connectpyse/project/project_phase.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/project/project_team_member.py` & `connectpyse-0.6.0.6/connectpyse/project/project_team_member.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/project/projects_api.py` & `connectpyse-0.6.0.6/connectpyse/project/projects_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/restapi.py` & `connectpyse-0.6.0.6/connectpyse/restapi.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/activity.py` & `connectpyse-0.6.0.6/connectpyse/sales/activity.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/activity_api.py` & `connectpyse-0.6.0.6/connectpyse/sales/activity_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/activity_type.py` & `connectpyse-0.6.0.6/connectpyse/sales/activity_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_api.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_contact.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_contact.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_forecast.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_forecast.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_forecast_api.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_forecast_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_note.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_note.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_status.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_status.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/opportunity_team.py` & `connectpyse-0.6.0.6/connectpyse/sales/opportunity_team.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/order.py` & `connectpyse-0.6.0.6/connectpyse/sales/order.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/sales/order_api.py` & `connectpyse-0.6.0.6/connectpyse/sales/order_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_entries_api.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_entries_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_entry.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_entry.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_reminder_times_api.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_reminder_times_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_statuses_api.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_statuses_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_type.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/schedule/schedule_types_api.py` & `connectpyse-0.6.0.6/connectpyse/schedule/schedule_types_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board.py` & `connectpyse-0.6.0.6/connectpyse/service/board.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board_item.py` & `connectpyse-0.6.0.6/connectpyse/service/board_item.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board_status.py` & `connectpyse-0.6.0.6/connectpyse/service/board_status.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board_sub_type.py` & `connectpyse-0.6.0.6/connectpyse/service/board_sub_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board_team.py` & `connectpyse-0.6.0.6/connectpyse/service/board_team.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/board_type.py` & `connectpyse-0.6.0.6/connectpyse/service/board_type.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/boards_api.py` & `connectpyse-0.6.0.6/connectpyse/service/boards_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/knowledge_base_article.py` & `connectpyse-0.6.0.6/connectpyse/service/knowledge_base_article.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/survey.py` & `connectpyse-0.6.0.6/connectpyse/service/survey.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/survey_question.py` & `connectpyse-0.6.0.6/connectpyse/service/survey_question.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/survey_result.py` & `connectpyse-0.6.0.6/connectpyse/service/survey_result.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/ticket.py` & `connectpyse-0.6.0.6/connectpyse/service/ticket.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/ticket_note.py` & `connectpyse-0.6.0.6/connectpyse/service/ticket_note.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/ticket_notes_api.py` & `connectpyse-0.6.0.6/connectpyse/service/ticket_notes_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/ticket_task.py` & `connectpyse-0.6.0.6/connectpyse/service/ticket_task.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/service/tickets_api.py` & `connectpyse-0.6.0.6/connectpyse/service/tickets_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/callback.py` & `connectpyse-0.6.0.6/connectpyse/system/callback.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/callbacks_api.py` & `connectpyse-0.6.0.6/connectpyse/system/callbacks_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/connectwise_hosted_setup.py` & `connectpyse-0.6.0.6/connectpyse/system/connectwise_hosted_setup.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/document.py` & `connectpyse-0.6.0.6/connectpyse/system/document.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/document_api.py` & `connectpyse-0.6.0.6/connectpyse/system/document_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/member.py` & `connectpyse-0.6.0.6/connectpyse/system/member.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/members_api.py` & `connectpyse-0.6.0.6/connectpyse/system/members_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/menu_entry.py` & `connectpyse-0.6.0.6/connectpyse/system/menu_entry.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/system/user_defined_field.py` & `connectpyse-0.6.0.6/connectpyse/system/user_defined_field.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/activity_stopwatch.py` & `connectpyse-0.6.0.6/connectpyse/time/activity_stopwatch.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/charge_code.py` & `connectpyse-0.6.0.6/connectpyse/time/charge_code.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/schedule_stopwatch.py` & `connectpyse-0.6.0.6/connectpyse/time/schedule_stopwatch.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/ticket_stopwatch.py` & `connectpyse-0.6.0.6/connectpyse/time/ticket_stopwatch.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/time_entries_api.py` & `connectpyse-0.6.0.6/connectpyse/time/time_entries_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/time_entry.py` & `connectpyse-0.6.0.6/connectpyse/time/time_entry.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/time_sheet.py` & `connectpyse-0.6.0.6/connectpyse/time/time_sheet.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse/time/time_sheets_api.py` & `connectpyse-0.6.0.6/connectpyse/time/time_sheets_api.py`

 * *Files identical despite different names*

### Comparing `connectpyse-0.6.0.5/connectpyse.egg-info/PKG-INFO` & `connectpyse-0.6.0.6/connectpyse.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connectpyse
-Version: 0.6.0.5
+Version: 0.6.0.6
 Summary: A ConnectWise API tool for the rest of us.
 Home-page: https://github.com/markciecior/ConnectPyse
 Author: Joshua M Smith (original), Mark Ciecior (forked), @wesgann
 Author-email: saether@gmail.com (original), mark@markciecior.com (forked)
 License: MIT
 Keywords: connectwise rest api
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `connectpyse-0.6.0.5/connectpyse.egg-info/SOURCES.txt` & `connectpyse-0.6.0.6/connectpyse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,20 +133,22 @@
 connectpyse/schedule/schedule_status.py
 connectpyse/schedule/schedule_statuses_api.py
 connectpyse/schedule/schedule_type.py
 connectpyse/schedule/schedule_types_api.py
 connectpyse/service/__init__.py
 connectpyse/service/board.py
 connectpyse/service/board_excluded_member.py
+connectpyse/service/board_info.py
 connectpyse/service/board_item.py
 connectpyse/service/board_status.py
 connectpyse/service/board_sub_type.py
 connectpyse/service/board_team.py
 connectpyse/service/board_type.py
 connectpyse/service/boards_api.py
+connectpyse/service/boards_info_api.py
 connectpyse/service/code.py
 connectpyse/service/knowledge_base_article.py
 connectpyse/service/location.py
 connectpyse/service/priority.py
 connectpyse/service/source.py
 connectpyse/service/survey.py
 connectpyse/service/survey_question.py
```

### Comparing `connectpyse-0.6.0.5/setup.py` & `connectpyse-0.6.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='connectpyse',
-      version='0.6.0.5',
+      version='0.6.0.6',
       description='A ConnectWise API tool for the rest of us.',
       long_description=long_description,
       long_description_content_type="text/markdown",
       classifiers=[
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.5'
```

