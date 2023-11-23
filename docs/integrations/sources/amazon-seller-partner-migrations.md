# Amazon Seller Partner Migration Guide

## Upgrading to 2.0.0

This change removes Brand Analytics and permanently removes deprecated FBA reports (from Airbyte Cloud).
Customers who have those streams must refresh their schema OR disable the following streams:
* GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT
* GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT
* GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT
* GET_BRAND_ANALYTICS_ALTERNATE_PURCHASE_REPORT
* GET_BRAND_ANALYTICS_ITEM_COMPARISON_REPORT
* GET_SALES_AND_TRAFFIC_REPORT
* GET_VENDOR_SALES_REPORT
* GET_VENDOR_INVENTORY_REPORT

Customers, who have the following streams, will have to disable them:
* GET_FBA_FULFILLMENT_INVENTORY_ADJUSTMENTS_DATA
* GET_FBA_FULFILLMENT_CURRENT_INVENTORY_DATA
* GET_FBA_FULFILLMENT_INVENTORY_RECEIPTS_DATA
* GET_FBA_FULFILLMENT_INVENTORY_SUMMARY_DATA
* GET_FBA_FULFILLMENT_MONTHLY_INVENTORY_DATA