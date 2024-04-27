# Comparing `tmp/pluggy_sdk-1.0.0.post6.tar.gz` & `tmp/pluggy_sdk-1.0.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pluggy_sdk-1.0.0.post6.tar", last modified: Sat Apr 20 01:06:10 2024, max compression
+gzip compressed data, was "pluggy_sdk-1.0.0.post7.tar", last modified: Sat Apr 27 01:05:29 2024, max compression
```

## Comparing `pluggy_sdk-1.0.0.post6.tar` & `pluggy_sdk-1.0.0.post7.tar`

### file list

```diff
@@ -1,333 +1,335 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:10.040759 pluggy_sdk-1.0.0.post6/
--rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-04-20 01:06:10.040759 pluggy_sdk-1.0.0.post6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20409 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:09.992759 pluggy_sdk-1.0.0.post6/pluggy_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:09.996759 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_anticipation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_receivable_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_sale_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/bill_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/bulk_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/category_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41008 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/identity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/income_report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35989 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/investment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54593 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/loan_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_customer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_intent_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    77933 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_recipient_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    94243 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/portfolio_yield_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/smart_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    55525 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:10.016759 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)     9937 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_anticipation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_anticipation_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_data_establishment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_destination_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_related_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_installment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_installment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/aggregated_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/aggregated_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/asset_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/auth_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bill.py
--rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bill_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bills_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bulk_payments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/category.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connect_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connect_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_health_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_or_update_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_customer_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_pix_qr_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_smart_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credential_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credit_card_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/document.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/global_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/i_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/identity_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/income_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/income_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_contracted_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_contracted_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installment_balloon_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installment_balloon_payment_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_interest_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_warranty.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loans_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/merchant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/monthly_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/monthly_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/not_authenticated_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-20 01:06:00.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_anticipations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_receivables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_category_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_investment_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/parameter_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/parameter_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_customers_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_data_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_institution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_intents_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipient_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipients_institution_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipients_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request_callback_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request_receipt_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_requests_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/percentage_over_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/pix_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail_product_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhook_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhooks_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:10.040759 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20822 2024-04-20 01:06:09.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12184 2024-04-20 01:06:09.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 01:06:09.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-20 01:06:09.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-20 01:06:09.000000 pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-20 01:06:01.000000 pluggy_sdk-1.0.0.post6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-20 01:06:10.040759 pluggy_sdk-1.0.0.post6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-20 01:06:07.000000 pluggy_sdk-1.0.0.post6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 01:06:10.040759 pluggy_sdk-1.0.0.post6/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_data_establishment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_destination_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_related_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_sale.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_installment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_installment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_aggregated_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_aggregated_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_asset_distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_auth_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_auth_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_auth_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bank_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bill.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bill_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bill_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bills_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bulk_payment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_bulk_payments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_category.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_category_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_company.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connect_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connect_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_health_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_list_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_connector_user_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_bulk_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_client_category_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_or_update_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_payment_customer_request_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_pix_qr_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_smart_account_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_create_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_credential_select_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_credit_card_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_credit_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_global_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_i_count_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_identity_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_identity_relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_income_report.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_income_report_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_income_reports_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investment_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investment_expenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investment_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investment_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_investments_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_item_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_item_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_item_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_items_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_contracted_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_contracted_finance_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_installment_balloon_payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_installment_balloon_payment_amount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_installments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_interest_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_payment_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel_fee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loan_warranty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_loans_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_merchant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_monthly_portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_monthly_portfolio_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_not_authenticated_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_anticipations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_receivables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_sales.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_category_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_investment_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_page_response_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_parameter_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_parameter_validation_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_customer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_customers_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_data_participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_institution.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_intent_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_intents_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_receipt_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_receipt_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_recipient_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_recipient_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_recipients_institution_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_recipients_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_request_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_request_callback_urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_request_receipt_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_payment_requests_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_percentage_over_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_pix_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_portfolio_yield_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_smart_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_smart_account_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_smart_account_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_smart_account_balance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_smart_accounts_list200_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_status_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_status_detail_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_status_detail_product_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_update_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_update_item_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_update_payment_recipient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_update_payment_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_update_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_webhook_creation_error_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 01:05:23.000000 pluggy_sdk-1.0.0.post6/test/test_webhooks_list200_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.465078 pluggy_sdk-1.0.0.post7/
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-04-27 01:05:29.465078 pluggy_sdk-1.0.0.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20469 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.413078 pluggy_sdk-1.0.0.post7/pluggy_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)    11800 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.421078 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22047 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26206 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_anticipation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26120 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_receivable_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25869 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_sale_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22882 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/bill_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32808 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/bulk_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41577 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/category_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41008 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21602 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/identity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/income_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35989 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/investment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54593 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20840 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54784 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_customer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32020 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_intent_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77933 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_recipient_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94243 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22320 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/portfolio_yield_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43323 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/smart_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37553 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55525 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5953 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.441078 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    10015 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_anticipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_anticipation_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_data_establishment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_destination_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_related_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_installment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_installment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/aggregated_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/aggregated_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/asset_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bill_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bills_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bulk_payments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connect_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connect_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_health_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_or_update_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_customer_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_pix_qr_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_smart_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credential_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4102 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credit_card_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5142 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/global_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/i_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/identity_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/income_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/income_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11050 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_contracted_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_contracted_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installment_balloon_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installment_balloon_payment_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_interest_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_warranty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loans_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/monthly_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/monthly_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/not_authenticated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_anticipations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_receivables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_category_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_investment_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/parameter_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/parameter_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_customers_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_data_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_institution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intent_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intents_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3246 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipient_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipients_institution_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipients_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request_callback_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request_receipt_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_requests_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/percentage_over_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3087 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/pix_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3217 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6906 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail_product_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhook_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhooks_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9385 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.465078 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20882 2024-04-27 01:05:29.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12268 2024-04-27 01:05:29.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-27 01:05:29.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-27 01:05:29.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-27 01:05:29.000000 pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-27 01:05:23.000000 pluggy_sdk-1.0.0.post7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-27 01:05:29.465078 pluggy_sdk-1.0.0.post7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-27 01:05:27.000000 pluggy_sdk-1.0.0.post7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-27 01:05:29.465078 pluggy_sdk-1.0.0.post7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_data_establishment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_destination_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_related_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_sale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_installment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_installment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_aggregated_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_aggregated_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_asset_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_auth_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_auth_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bank_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bill_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bill_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bills_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bulk_payment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_bulk_payments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_category_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connect_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connect_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_health_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_list_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_connector_user_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_bulk_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_client_category_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_or_update_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_payment_customer_request_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_pix_qr_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_smart_account_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_create_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_credential_select_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_credit_card_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_credit_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_global_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_i_count_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_identity_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_identity_relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_income_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_income_report_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_income_reports_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4473 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investment_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investment_expenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investment_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investment_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_investments_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_item_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_item_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_item_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_items_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_contracted_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_contracted_finance_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_installment_balloon_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_installment_balloon_payment_amount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_installments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_interest_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_payment_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel_fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2630 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loan_warranty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_loans_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_merchant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_monthly_portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_monthly_portfolio_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_not_authenticated_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_anticipations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_receivables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_sales.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_category_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_investment_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_page_response_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_parameter_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_parameter_validation_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_customer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_customers_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_data_participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_institution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_intent_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-27 01:05:22.000000 pluggy_sdk-1.0.0.post7/test/test_payment_intent_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_intents_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_receipt_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_receipt_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_recipient_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_recipient_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_recipients_institution_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_recipients_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_request_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_request_callback_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_request_receipt_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_payment_requests_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_percentage_over_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_pix_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_portfolio_yield_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_smart_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_smart_account_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_smart_account_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_smart_account_balance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_smart_accounts_list200_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_status_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_status_detail_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_status_detail_product_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_update_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_update_item_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_update_payment_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_update_payment_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_update_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_webhook_creation_error_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-27 01:05:13.000000 pluggy_sdk-1.0.0.post7/test/test_webhooks_list200_response.py
```

### Comparing `pluggy_sdk-1.0.0.post6/PKG-INFO` & `pluggy_sdk-1.0.0.post7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy-sdk
-Version: 1.0.0.post6
+Version: 1.0.0.post7
 Summary: Pluggy API
 Home-page: https://github.com/diraol/pluggy-python
 Author: Pluggy
 Author-email: hello@pluggy.ai
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Pluggy API
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post6
+- Package version: 1.0.0.post7
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -286,14 +286,15 @@
  - [ParameterValidationResponse](docs/ParameterValidationResponse.md)
  - [PaymentCustomer](docs/PaymentCustomer.md)
  - [PaymentCustomersList200Response](docs/PaymentCustomersList200Response.md)
  - [PaymentData](docs/PaymentData.md)
  - [PaymentDataParticipant](docs/PaymentDataParticipant.md)
  - [PaymentInstitution](docs/PaymentInstitution.md)
  - [PaymentIntent](docs/PaymentIntent.md)
+ - [PaymentIntentParameter](docs/PaymentIntentParameter.md)
  - [PaymentIntentsList200Response](docs/PaymentIntentsList200Response.md)
  - [PaymentReceipt](docs/PaymentReceipt.md)
  - [PaymentReceiptBankAccount](docs/PaymentReceiptBankAccount.md)
  - [PaymentReceiptPerson](docs/PaymentReceiptPerson.md)
  - [PaymentRecipient](docs/PaymentRecipient.md)
  - [PaymentRecipientAccount](docs/PaymentRecipientAccount.md)
  - [PaymentRecipientsInstitutionList200Response](docs/PaymentRecipientsInstitutionList200Response.md)
```

### Comparing `pluggy_sdk-1.0.0.post6/README.md` & `pluggy_sdk-1.0.0.post7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post6
+- Package version: 1.0.0.post7
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -271,14 +271,15 @@
  - [ParameterValidationResponse](docs/ParameterValidationResponse.md)
  - [PaymentCustomer](docs/PaymentCustomer.md)
  - [PaymentCustomersList200Response](docs/PaymentCustomersList200Response.md)
  - [PaymentData](docs/PaymentData.md)
  - [PaymentDataParticipant](docs/PaymentDataParticipant.md)
  - [PaymentInstitution](docs/PaymentInstitution.md)
  - [PaymentIntent](docs/PaymentIntent.md)
+ - [PaymentIntentParameter](docs/PaymentIntentParameter.md)
  - [PaymentIntentsList200Response](docs/PaymentIntentsList200Response.md)
  - [PaymentReceipt](docs/PaymentReceipt.md)
  - [PaymentReceiptBankAccount](docs/PaymentReceiptBankAccount.md)
  - [PaymentReceiptPerson](docs/PaymentReceiptPerson.md)
  - [PaymentRecipient](docs/PaymentRecipient.md)
  - [PaymentRecipientAccount](docs/PaymentRecipientAccount.md)
  - [PaymentRecipientsInstitutionList200Response](docs/PaymentRecipientsInstitutionList200Response.md)
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/__init__.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Contact: hello@pluggy.ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "1.0.0.post6"
+__version__ = "1.0.0.post7"
 
 # import apis into sdk package
 from pluggy_sdk.api.account_api import AccountApi
 from pluggy_sdk.api.acquirer_anticipation_api import AcquirerAnticipationApi
 from pluggy_sdk.api.acquirer_receivable_api import AcquirerReceivableApi
 from pluggy_sdk.api.acquirer_sale_api import AcquirerSaleApi
 from pluggy_sdk.api.auth_api import AuthApi
@@ -150,14 +150,15 @@
 from pluggy_sdk.models.parameter_validation_response import ParameterValidationResponse
 from pluggy_sdk.models.payment_customer import PaymentCustomer
 from pluggy_sdk.models.payment_customers_list200_response import PaymentCustomersList200Response
 from pluggy_sdk.models.payment_data import PaymentData
 from pluggy_sdk.models.payment_data_participant import PaymentDataParticipant
 from pluggy_sdk.models.payment_institution import PaymentInstitution
 from pluggy_sdk.models.payment_intent import PaymentIntent
+from pluggy_sdk.models.payment_intent_parameter import PaymentIntentParameter
 from pluggy_sdk.models.payment_intents_list200_response import PaymentIntentsList200Response
 from pluggy_sdk.models.payment_receipt import PaymentReceipt
 from pluggy_sdk.models.payment_receipt_bank_account import PaymentReceiptBankAccount
 from pluggy_sdk.models.payment_receipt_person import PaymentReceiptPerson
 from pluggy_sdk.models.payment_recipient import PaymentRecipient
 from pluggy_sdk.models.payment_recipient_account import PaymentRecipientAccount
 from pluggy_sdk.models.payment_recipients_institution_list200_response import PaymentRecipientsInstitutionList200Response
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/__init__.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/account_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_anticipation_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_anticipation_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_receivable_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_receivable_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/acquirer_sale_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/acquirer_sale_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/auth_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/bill_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/bill_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/bulk_payment_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/bulk_payment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/category_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/category_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/connector_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/connector_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/identity_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/identity_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/income_report_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/income_report_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/investment_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/investment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/items_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/items_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/loan_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/loan_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_customer_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_customer_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_intent_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_intent_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_recipient_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_recipient_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/payment_request_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/payment_request_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/portfolio_yield_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/portfolio_yield_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/smart_account_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/smart_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/transaction_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/transaction_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api/webhook_api.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api/webhook_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api_client.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0.post6/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.0.post7/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         pass
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/api_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/api_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/configuration.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,15 +396,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
-               "SDK Package Version: 1.0.0.post6".\
+               "SDK Package Version: 1.0.0.post7".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/exceptions.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/__init__.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 from pluggy_sdk.models.parameter_validation_response import ParameterValidationResponse
 from pluggy_sdk.models.payment_customer import PaymentCustomer
 from pluggy_sdk.models.payment_customers_list200_response import PaymentCustomersList200Response
 from pluggy_sdk.models.payment_data import PaymentData
 from pluggy_sdk.models.payment_data_participant import PaymentDataParticipant
 from pluggy_sdk.models.payment_institution import PaymentInstitution
 from pluggy_sdk.models.payment_intent import PaymentIntent
+from pluggy_sdk.models.payment_intent_parameter import PaymentIntentParameter
 from pluggy_sdk.models.payment_intents_list200_response import PaymentIntentsList200Response
 from pluggy_sdk.models.payment_receipt import PaymentReceipt
 from pluggy_sdk.models.payment_receipt_bank_account import PaymentReceiptBankAccount
 from pluggy_sdk.models.payment_receipt_person import PaymentReceiptPerson
 from pluggy_sdk.models.payment_recipient import PaymentRecipient
 from pluggy_sdk.models.payment_recipient_account import PaymentRecipientAccount
 from pluggy_sdk.models.payment_recipients_institution_list200_response import PaymentRecipientsInstitutionList200Response
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/account.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/accounts_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_anticipation.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_anticipation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_anticipation_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_anticipation_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_data_establishment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_data_establishment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_destination_account.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_destination_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_receivable_related_sale.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_receivable_related_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_installment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_installment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/acquirer_sale_installment_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/acquirer_sale_installment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/address.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/aggregated_portfolio.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/aggregated_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/aggregated_portfolio_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/aggregated_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/asset_distribution.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/asset_distribution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/auth_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/auth_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/auth_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/auth_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bank_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bank_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bill.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bill.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bill_finance_charge.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bill_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bills_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bills_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bulk_payment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bulk_payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,16 +41,16 @@
     payment_requests: List[PaymentRequest] = Field(description="List of payment requests associated with the bulk payment", alias="paymentRequests")
     smart_account: SmartAccount = Field(alias="smartAccount")
     __properties: ClassVar[List[str]] = ["id", "totalAmount", "status", "createdAt", "updatedAt", "callbackUrls", "paymentUrl", "paymentRequests", "smartAccount"]
 
     @field_validator('status')
     def status_validate_enum(cls, value):
         """Validates the enum"""
-        if value not in set(['CREATED', 'PAYMENT_IN_PROGRESS', 'TOP_UP_IN_PROGRESS', 'COMPLETED', 'ERROR']):
-            raise ValueError("must be one of enum values ('CREATED', 'PAYMENT_IN_PROGRESS', 'TOP_UP_IN_PROGRESS', 'COMPLETED', 'ERROR')")
+        if value not in set(['CREATED', 'PAYMENT_IN_PROGRESS', 'TOP_UP_IN_PROGRESS', 'COMPLETED', 'PARTIALLY_COMPLETED', 'ERROR']):
+            raise ValueError("must be one of enum values ('CREATED', 'PAYMENT_IN_PROGRESS', 'TOP_UP_IN_PROGRESS', 'COMPLETED', 'PARTIALLY_COMPLETED', 'ERROR')")
         return value
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/bulk_payments_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/bulk_payments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/category.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/category.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/client_category_rule.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/company.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/company.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connect_token_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connect_token_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connect_token_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connect_token_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_credential.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_credential.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_health.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_health.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_health_details.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_health_details.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_list_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_list_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/connector_user_action.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/connector_user_action.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_bulk_payment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_client_category_rule.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_item.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_item_parameters.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_or_update_payment_customer.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_or_update_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_customer_request_body.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_intent.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intent_parameter.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
-from pydantic import BaseModel, ConfigDict, Field, StrictFloat, StrictInt, StrictStr
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from pydantic import BaseModel, ConfigDict, Field, StrictStr
+from typing import Any, ClassVar, Dict, List, Optional
 from typing import Optional, Set
 from typing_extensions import Self
 
-class CreatePaymentIntent(BaseModel):
+class PaymentIntentParameter(BaseModel):
     """
-    Request with information to create a payment intent
+    Credentials neccesary to create a payment intent
     """ # noqa: E501
-    payment_request_id: Optional[StrictStr] = Field(default=None, description="Primary identifier of the payment request associated to the payment intent", alias="paymentRequestId")
-    bulk_payment_id: Optional[StrictStr] = Field(default=None, description="Primary identifier of the bulk payment associated to the payment intent", alias="bulkPaymentId")
-    connector_id: Union[StrictFloat, StrictInt] = Field(description="Primary identifier of the connector associated to the payment intent", alias="connectorId")
-    parameters: Dict[str, StrictStr] = Field(description="Key-Value credentials neccesary to create an item")
-    __properties: ClassVar[List[str]] = ["paymentRequestId", "bulkPaymentId", "connectorId", "parameters"]
+    cpf: StrictStr = Field(description="CPF of the payer")
+    cnpj: Optional[StrictStr] = Field(default=None, description="CNPJ of the payer")
+    __properties: ClassVar[List[str]] = ["cpf", "cnpj"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
         protected_namespaces=(),
     )
 
@@ -47,15 +45,15 @@
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         # TODO: pydantic v2: use .model_dump_json(by_alias=True, exclude_unset=True) instead
         return json.dumps(self.to_dict())
 
     @classmethod
     def from_json(cls, json_str: str) -> Optional[Self]:
-        """Create an instance of CreatePaymentIntent from a JSON string"""
+        """Create an instance of PaymentIntentParameter from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,23 +70,21 @@
             exclude=excluded_fields,
             exclude_none=True,
         )
         return _dict
 
     @classmethod
     def from_dict(cls, obj: Optional[Dict[str, Any]]) -> Optional[Self]:
-        """Create an instance of CreatePaymentIntent from a dict"""
+        """Create an instance of PaymentIntentParameter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
-            "paymentRequestId": obj.get("paymentRequestId"),
-            "bulkPaymentId": obj.get("bulkPaymentId"),
-            "connectorId": obj.get("connectorId"),
-            "parameters": obj.get("parameters")
+            "cpf": obj.get("cpf"),
+            "cnpj": obj.get("cnpj")
         })
         return _obj
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_recipient.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_recipient.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 from typing import Any, ClassVar, Dict, List, Optional
 from pluggy_sdk.models.payment_recipient_account import PaymentRecipientAccount
 from typing import Optional, Set
 from typing_extensions import Self
 
 class CreatePaymentRecipient(BaseModel):
     """
-    Request with information to create a payment recipient
+    Request with information to create a payment recipient, there is two form to create a payment recipient, one with pixKey and other with taxNumber, name, paymentInstitutionId and account
     """ # noqa: E501
-    tax_number: StrictStr = Field(description="Account owner tax number. Can be CPF or CNPJ (only numbers). Send only when the pixKey is not sent.", alias="taxNumber")
-    name: StrictStr = Field(description="Account owner name. Send only this when the pixKey is not sent.")
-    payment_institution_id: StrictStr = Field(description="Primary identifier of the institution associated to the payment recipient. Send only when the pixKey is not sent.", alias="paymentInstitutionId")
-    account: PaymentRecipientAccount
+    tax_number: Optional[StrictStr] = Field(default=None, description="Account owner tax number. Can be CPF or CNPJ (only numbers). Send only when the pixKey is not sent.", alias="taxNumber")
+    name: Optional[StrictStr] = Field(default=None, description="Account owner name. Send only this when the pixKey is not sent.")
+    payment_institution_id: Optional[StrictStr] = Field(default=None, description="Primary identifier of the institution associated to the payment recipient. Send only when the pixKey is not sent.", alias="paymentInstitutionId")
+    account: Optional[PaymentRecipientAccount] = None
     is_default: Optional[StrictBool] = Field(default=None, description="Indicates if the recipient is the default one", alias="isDefault")
     pix_key: Optional[StrictStr] = Field(default=None, description="Pix key associated with the payment recipient", alias="pixKey")
     __properties: ClassVar[List[str]] = ["taxNumber", "name", "paymentInstitutionId", "account", "isDefault", "pixKey"]
 
     model_config = ConfigDict(
         populate_by_name=True,
         validate_assignment=True,
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_payment_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_pix_qr_payment_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_pix_qr_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_smart_account_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_smart_account_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/create_webhook.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/create_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credential_select_option.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credential_select_option.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credit_card_metadata.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credit_card_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/credit_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/credit_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/document.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/document.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/email.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/email.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/global_error_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/global_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/i_count_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/i_count_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/identity_relation.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/identity_relation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/identity_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/identity_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/income_report.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/income_report.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/income_reports_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/income_reports_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_expenses.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_expenses.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_metadata.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investment_transaction.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investment_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/investments_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/investments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_creation_error_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_error.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/item_options.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/item_options.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_contracted_fee.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_contracted_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_contracted_finance_charge.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_contracted_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installment_balloon_payment.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installment_balloon_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installment_balloon_payment_amount.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installment_balloon_payment_amount.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_installments.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_installments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_interest_rate.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_interest_rate.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payment_release_over_parcel_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_payments.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_payments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loan_warranty.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loan_warranty.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/loans_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/loans_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/merchant.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/merchant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/monthly_portfolio.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/monthly_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/monthly_portfolio_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/monthly_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/not_authenticated_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/not_authenticated_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_anticipations.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_anticipations.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_receivables.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_receivables.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_acquirer_sales.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_acquirer_sales.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_category_rules.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_category_rules.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_investment_transactions.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_investment_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/page_response_transactions.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/page_response_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/parameter_validation_error.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/parameter_validation_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/parameter_validation_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/parameter_validation_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_customer.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_customers_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_customers_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_data_participant.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_data_participant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_institution.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_institution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_intent.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_intents_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_intents_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt_bank_account.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt_bank_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_receipt_person.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_receipt_person.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipient.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipient_account.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipient_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipients_institution_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipients_institution_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_recipients_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_recipients_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request_callback_urls.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request_callback_urls.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_request_receipt_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_request_receipt_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/payment_requests_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/payment_requests_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/percentage_over_index.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/percentage_over_index.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/phone_number.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/phone_number.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/pix_data.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/pix_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account_address.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_account_balance.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_account_balance.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/smart_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/smart_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail_product.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail_product.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/status_detail_product_warning.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/status_detail_product_warning.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/transaction.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_item.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_item_parameters.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_payment_recipient.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_payment_request.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/update_transaction.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/update_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhook.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhook_creation_error_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhook_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/models/webhooks_list200_response.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/models/webhooks_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk/rest.py` & `pluggy_sdk-1.0.0.post7/pluggy_sdk/rest.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/PKG-INFO` & `pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pluggy-sdk
-Version: 1.0.0.post6
+Version: 1.0.0.post7
 Summary: Pluggy API
 Home-page: https://github.com/diraol/pluggy-python
 Author: Pluggy
 Author-email: hello@pluggy.ai
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,Pluggy API
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 
 # pluggy-sdk
 Pluggy's main API to review data and execute connectors
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 - API version: 1.0.0
-- Package version: 1.0.0.post6
+- Package version: 1.0.0.post7
 - Generator version: 7.6.0-SNAPSHOT
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://pluggy.ai](https://pluggy.ai)
 
 ## Requirements.
 
 Python 3.7+
@@ -286,14 +286,15 @@
  - [ParameterValidationResponse](docs/ParameterValidationResponse.md)
  - [PaymentCustomer](docs/PaymentCustomer.md)
  - [PaymentCustomersList200Response](docs/PaymentCustomersList200Response.md)
  - [PaymentData](docs/PaymentData.md)
  - [PaymentDataParticipant](docs/PaymentDataParticipant.md)
  - [PaymentInstitution](docs/PaymentInstitution.md)
  - [PaymentIntent](docs/PaymentIntent.md)
+ - [PaymentIntentParameter](docs/PaymentIntentParameter.md)
  - [PaymentIntentsList200Response](docs/PaymentIntentsList200Response.md)
  - [PaymentReceipt](docs/PaymentReceipt.md)
  - [PaymentReceiptBankAccount](docs/PaymentReceiptBankAccount.md)
  - [PaymentReceiptPerson](docs/PaymentReceiptPerson.md)
  - [PaymentRecipient](docs/PaymentRecipient.md)
  - [PaymentRecipientAccount](docs/PaymentRecipientAccount.md)
  - [PaymentRecipientsInstitutionList200Response](docs/PaymentRecipientsInstitutionList200Response.md)
```

### Comparing `pluggy_sdk-1.0.0.post6/pluggy_sdk.egg-info/SOURCES.txt` & `pluggy_sdk-1.0.0.post7/pluggy_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 pluggy_sdk/models/parameter_validation_response.py
 pluggy_sdk/models/payment_customer.py
 pluggy_sdk/models/payment_customers_list200_response.py
 pluggy_sdk/models/payment_data.py
 pluggy_sdk/models/payment_data_participant.py
 pluggy_sdk/models/payment_institution.py
 pluggy_sdk/models/payment_intent.py
+pluggy_sdk/models/payment_intent_parameter.py
 pluggy_sdk/models/payment_intents_list200_response.py
 pluggy_sdk/models/payment_receipt.py
 pluggy_sdk/models/payment_receipt_bank_account.py
 pluggy_sdk/models/payment_receipt_person.py
 pluggy_sdk/models/payment_recipient.py
 pluggy_sdk/models/payment_recipient_account.py
 pluggy_sdk/models/payment_recipients_institution_list200_response.py
@@ -283,14 +284,15 @@
 test/test_payment_customer_api.py
 test/test_payment_customers_list200_response.py
 test/test_payment_data.py
 test/test_payment_data_participant.py
 test/test_payment_institution.py
 test/test_payment_intent.py
 test/test_payment_intent_api.py
+test/test_payment_intent_parameter.py
 test/test_payment_intents_list200_response.py
 test/test_payment_receipt.py
 test/test_payment_receipt_bank_account.py
 test/test_payment_receipt_person.py
 test/test_payment_recipient.py
 test/test_payment_recipient_account.py
 test/test_payment_recipient_api.py
```

### Comparing `pluggy_sdk-1.0.0.post6/pyproject.toml` & `pluggy_sdk-1.0.0.post7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pluggy_sdk"
-version = "1.0.0.post6"
+version = "1.0.0.post7"
 description = "Pluggy API"
 authors = ["Pluggy <hello@pluggy.ai>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/GIT_USER_ID/GIT_REPO_ID"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Pluggy API"]
 include = ["pluggy_sdk/py.typed"]
```

### Comparing `pluggy_sdk-1.0.0.post6/setup.py` & `pluggy_sdk-1.0.0.post7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "pluggy-sdk"
-VERSION = "1.0.0.post6"
+VERSION = "1.0.0.post7"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 2",
     "typing-extensions >= 4.7.1",
 ]
```

### Comparing `pluggy_sdk-1.0.0.post6/test/test_account.py` & `pluggy_sdk-1.0.0.post7/test/test_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_account_api.py` & `pluggy_sdk-1.0.0.post7/test/test_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation_api.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_anticipation_data.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_anticipation_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_data.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_api.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_data.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_data_establishment.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_data_establishment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_destination_account.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_destination_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_receivable_related_sale.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_receivable_related_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_sale.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_sale.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_api.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_data.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_installment.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_installment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_acquirer_sale_installment_data.py` & `pluggy_sdk-1.0.0.post7/test/test_acquirer_sale_installment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_address.py` & `pluggy_sdk-1.0.0.post7/test/test_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_aggregated_portfolio.py` & `pluggy_sdk-1.0.0.post7/test/test_aggregated_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_aggregated_portfolio_response.py` & `pluggy_sdk-1.0.0.post7/test/test_aggregated_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_asset_distribution.py` & `pluggy_sdk-1.0.0.post7/test/test_asset_distribution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_auth_api.py` & `pluggy_sdk-1.0.0.post7/test/test_auth_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_auth_request.py` & `pluggy_sdk-1.0.0.post7/test/test_auth_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_auth_response.py` & `pluggy_sdk-1.0.0.post7/test/test_auth_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bank_data.py` & `pluggy_sdk-1.0.0.post7/test/test_bank_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bill.py` & `pluggy_sdk-1.0.0.post7/test/test_bill.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bill_api.py` & `pluggy_sdk-1.0.0.post7/test/test_bill_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bill_finance_charge.py` & `pluggy_sdk-1.0.0.post7/test/test_bill_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bills_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_bills_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bulk_payment.py` & `pluggy_sdk-1.0.0.post7/test/test_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bulk_payment_api.py` & `pluggy_sdk-1.0.0.post7/test/test_bulk_payment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_bulk_payments_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_bulk_payments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_category.py` & `pluggy_sdk-1.0.0.post7/test/test_category.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_category_api.py` & `pluggy_sdk-1.0.0.post7/test/test_category_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_client_category_rule.py` & `pluggy_sdk-1.0.0.post7/test/test_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_company.py` & `pluggy_sdk-1.0.0.post7/test/test_company.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connect_token_request.py` & `pluggy_sdk-1.0.0.post7/test/test_connect_token_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connect_token_response.py` & `pluggy_sdk-1.0.0.post7/test/test_connect_token_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector.py` & `pluggy_sdk-1.0.0.post7/test/test_connector.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_api.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_credential.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_credential.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_health.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_health.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_health_details.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_health_details.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_list_response.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_list_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_connector_user_action.py` & `pluggy_sdk-1.0.0.post7/test/test_connector_user_action.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_bulk_payment.py` & `pluggy_sdk-1.0.0.post7/test/test_create_bulk_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_client_category_rule.py` & `pluggy_sdk-1.0.0.post7/test/test_create_client_category_rule.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_item.py` & `pluggy_sdk-1.0.0.post7/test/test_create_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_item_parameters.py` & `pluggy_sdk-1.0.0.post7/test/test_create_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_or_update_payment_customer.py` & `pluggy_sdk-1.0.0.post7/test/test_create_or_update_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_payment_customer_request_body.py` & `pluggy_sdk-1.0.0.post7/test/test_create_payment_customer_request_body.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_payment_intent.py` & `pluggy_sdk-1.0.0.post7/test/test_create_payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_payment_recipient.py` & `pluggy_sdk-1.0.0.post7/test/test_create_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_payment_request.py` & `pluggy_sdk-1.0.0.post7/test/test_create_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_pix_qr_payment_request.py` & `pluggy_sdk-1.0.0.post7/test/test_create_pix_qr_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_smart_account_request.py` & `pluggy_sdk-1.0.0.post7/test/test_create_smart_account_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_create_webhook.py` & `pluggy_sdk-1.0.0.post7/test/test_create_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_credential_select_option.py` & `pluggy_sdk-1.0.0.post7/test/test_credential_select_option.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_credit_card_metadata.py` & `pluggy_sdk-1.0.0.post7/test/test_credit_card_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_credit_data.py` & `pluggy_sdk-1.0.0.post7/test/test_credit_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_document.py` & `pluggy_sdk-1.0.0.post7/test/test_document.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_email.py` & `pluggy_sdk-1.0.0.post7/test/test_email.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_global_error_response.py` & `pluggy_sdk-1.0.0.post7/test/test_global_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_i_count_response.py` & `pluggy_sdk-1.0.0.post7/test/test_i_count_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_identity_api.py` & `pluggy_sdk-1.0.0.post7/test/test_identity_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_identity_relation.py` & `pluggy_sdk-1.0.0.post7/test/test_identity_relation.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_identity_response.py` & `pluggy_sdk-1.0.0.post7/test/test_identity_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_income_report.py` & `pluggy_sdk-1.0.0.post7/test/test_income_report.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_income_report_api.py` & `pluggy_sdk-1.0.0.post7/test/test_income_report_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_income_reports_response.py` & `pluggy_sdk-1.0.0.post7/test/test_income_reports_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investment.py` & `pluggy_sdk-1.0.0.post7/test/test_investment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investment_api.py` & `pluggy_sdk-1.0.0.post7/test/test_investment_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investment_expenses.py` & `pluggy_sdk-1.0.0.post7/test/test_investment_expenses.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investment_metadata.py` & `pluggy_sdk-1.0.0.post7/test/test_investment_metadata.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investment_transaction.py` & `pluggy_sdk-1.0.0.post7/test/test_investment_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_investments_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_investments_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_item.py` & `pluggy_sdk-1.0.0.post7/test/test_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_item_creation_error_response.py` & `pluggy_sdk-1.0.0.post7/test/test_item_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_item_error.py` & `pluggy_sdk-1.0.0.post7/test/test_item_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_item_options.py` & `pluggy_sdk-1.0.0.post7/test/test_item_options.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_items_api.py` & `pluggy_sdk-1.0.0.post7/test/test_items_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan.py` & `pluggy_sdk-1.0.0.post7/test/test_loan.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_api.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_contracted_fee.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_contracted_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_contracted_finance_charge.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_contracted_finance_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_installment_balloon_payment.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_installment_balloon_payment.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_installment_balloon_payment_amount.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_installment_balloon_payment_amount.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_installments.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_installments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_interest_rate.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_interest_rate.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_payment_release.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_payment_release.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel_charge.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel_charge.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_payment_release_over_parcel_fee.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_payment_release_over_parcel_fee.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_payments.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_payments.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loan_warranty.py` & `pluggy_sdk-1.0.0.post7/test/test_loan_warranty.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_loans_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_loans_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_merchant.py` & `pluggy_sdk-1.0.0.post7/test/test_merchant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_monthly_portfolio.py` & `pluggy_sdk-1.0.0.post7/test/test_monthly_portfolio.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_monthly_portfolio_response.py` & `pluggy_sdk-1.0.0.post7/test/test_monthly_portfolio_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_not_authenticated_response.py` & `pluggy_sdk-1.0.0.post7/test/test_not_authenticated_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_anticipations.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_anticipations.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_receivables.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_receivables.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_acquirer_sales.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_acquirer_sales.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_category_rules.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_category_rules.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_investment_transactions.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_investment_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_page_response_transactions.py` & `pluggy_sdk-1.0.0.post7/test/test_page_response_transactions.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_parameter_validation_error.py` & `pluggy_sdk-1.0.0.post7/test/test_parameter_validation_error.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_parameter_validation_response.py` & `pluggy_sdk-1.0.0.post7/test/test_parameter_validation_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_customer.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_customer.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_customer_api.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_customer_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_customers_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_customers_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_data.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_data_participant.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_data_participant.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_institution.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_institution.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_intent.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_intent_api.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_intent_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_intents_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_intents_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_receipt.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_receipt.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_receipt_bank_account.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_receipt_bank_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_receipt_person.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_receipt_person.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_recipient.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_recipient_account.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_recipient_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_recipient_api.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_recipient_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_recipients_institution_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_recipients_institution_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_recipients_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_recipients_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_request.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_request_api.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_request_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_request_callback_urls.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_request_callback_urls.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_request_receipt_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_request_receipt_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_payment_requests_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_payment_requests_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_percentage_over_index.py` & `pluggy_sdk-1.0.0.post7/test/test_percentage_over_index.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_phone_number.py` & `pluggy_sdk-1.0.0.post7/test/test_phone_number.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_pix_data.py` & `pluggy_sdk-1.0.0.post7/test/test_pix_data.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_portfolio_yield_api.py` & `pluggy_sdk-1.0.0.post7/test/test_portfolio_yield_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_smart_account.py` & `pluggy_sdk-1.0.0.post7/test/test_smart_account.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_smart_account_address.py` & `pluggy_sdk-1.0.0.post7/test/test_smart_account_address.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_smart_account_api.py` & `pluggy_sdk-1.0.0.post7/test/test_smart_account_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_smart_account_balance.py` & `pluggy_sdk-1.0.0.post7/test/test_smart_account_balance.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_smart_accounts_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_smart_accounts_list200_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_status_detail.py` & `pluggy_sdk-1.0.0.post7/test/test_status_detail.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_status_detail_product.py` & `pluggy_sdk-1.0.0.post7/test/test_status_detail_product.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_status_detail_product_warning.py` & `pluggy_sdk-1.0.0.post7/test/test_status_detail_product_warning.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_transaction.py` & `pluggy_sdk-1.0.0.post7/test/test_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_transaction_api.py` & `pluggy_sdk-1.0.0.post7/test/test_transaction_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_update_item.py` & `pluggy_sdk-1.0.0.post7/test/test_update_item.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_update_item_parameters.py` & `pluggy_sdk-1.0.0.post7/test/test_update_item_parameters.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_update_payment_recipient.py` & `pluggy_sdk-1.0.0.post7/test/test_update_payment_recipient.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_update_payment_request.py` & `pluggy_sdk-1.0.0.post7/test/test_update_payment_request.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_update_transaction.py` & `pluggy_sdk-1.0.0.post7/test/test_update_transaction.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_webhook.py` & `pluggy_sdk-1.0.0.post7/test/test_webhook.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_webhook_api.py` & `pluggy_sdk-1.0.0.post7/test/test_webhook_api.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_webhook_creation_error_response.py` & `pluggy_sdk-1.0.0.post7/test/test_webhook_creation_error_response.py`

 * *Files identical despite different names*

### Comparing `pluggy_sdk-1.0.0.post6/test/test_webhooks_list200_response.py` & `pluggy_sdk-1.0.0.post7/test/test_webhooks_list200_response.py`

 * *Files identical despite different names*

