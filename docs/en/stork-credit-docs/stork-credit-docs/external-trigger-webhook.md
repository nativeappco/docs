---
type: page
title: "External Trigger (Webhook): Issue Store Credit From Any App"
seoTitle: Issue Shopify Store Credit From Any App via Webhook
seoDescription: Use Stork Credit's external trigger to issue Shopify store credit from Klaviyo, your helpdesk, a custom app, or any platform that can send a webhook.
slug: external-trigger-webhook
order: 7
status: draft
---

# External Trigger (Webhook): Issue Store Credit From Any App

## What it does

Lets any third party app or service that can send a webhook issue Shopify store credit directly into a customer's account. No CSV import, no manual entry in Shopify, no custom integration build required on your side.

## Common use cases

*   Reward customers for leaving a review (e.g. via Klaviyo)
*   Issue credit from a support/helpdesk platform (refunds, goodwill credit)
*   Trigger credit from a custom app
*   Issue credit from a POS system that isn't Shopify POS

## How it works

1.  In Stork Credit, open **External Trigger** and copy your webhook URL and the JSON payload template.
2.  In your third party platform, add a webhook / HTTP request action and paste in the webhook URL.
3.  Set the request body using the JSON payload from Stork Credit. This includes:
    *   `amount` - the store credit value to issue
    *   `currency` - the currency of the credit
    *   `message` - shown to the customer alongside the credit
    *   `id` - a unique reference for the transaction
4.  Save and activate.

## Example: rewarding reviews with Klaviyo Flow

1.  In Klaviyo, open (or create) the flow you want to issue credit from, e.g. a "thanks for your review" flow.
2.  Add a new action > Webhook.
3.  Paste in your Stork Credit webhook URL.
4.  Paste in the JSON payload and set the amount, currency, message and ID for this flow.
5.  Save the flow.

Every time a customer enters that flow, they're issued store credit automatically. No manual step, no separate spreadsheet.

## What happens after

Store credit issued via webhook lands in the customer's Shopify account exactly like any other Stork Credit issuance. It appears in their store credit balance, the adjustment is logged as made by Stork Credit, and you can set an expiry date on it, same as manual or template based credit.

## Why it matters

This isn't a workaround bolted on the side. It's native Shopify store credit, issued from wherever your automation already lives, whether that's Klaviyo, your helpdesk, a custom app, or your POS.