---
type: page
title: Email Marketing via Shopify Flow
description: Fish Wishlist supports Klaviyo integration via Shopify Flow. This allows you to trigger Klaviyo events when customers add or remove products from their wishlist.
seoTitle: Email Marketing via Shopify Flow | Fish Wishlist
seoDescription: Connect Fish Wishlist to Klaviyo, Dotdigital, Omnisend, or any email platform using Shopify Flow. Trigger and cancel campaigns automatically based on wishlist activity.
slug: shopify-flow-email-marketing
order: 3
status: published
---

# Email Marketing via Shopify Flow

Fish Wishlist fires **Shopify Flow triggers** when customers add or remove products from their wishlist. You can use these triggers to connect to any email or SMS marketing platform — not just Klaviyo.

Supported platforms include Klaviyo, Dotdigital, Omnisend, Attentive, and any other platform that has a Shopify Flow action.

* * *

## How it works

1.  A customer adds or removes a product from their wishlist
2.  Fish Wishlist fires a Shopify Flow trigger
3.  Your Flow sends event data to your email/SMS platform
4.  Your platform triggers or cancels the relevant campaign

* * *

## Prerequisites

*   Fish Wishlist installed and active
*   Your email platform installed and connected to Shopify
*   Shopify Flow installed (free on all Shopify plans)
*   Your platform's API key

* * *

## Klaviyo — Quick Start

We've built ready-to-use Shopify Flow templates for Klaviyo:

👉 [Load Flow Templates](https://admin.shopify.com/apps/flow/editor/templates?apps=157109354497)

### Template 1: Trigger campaign when product is added to wishlist

Sends a custom event to Klaviyo when a product is added. Use this to trigger a reminder flow — e.g. "You saved this — it's still available".

### Template 2: Cancel campaign when product is removed

Sends a cancel event when a product is removed. Stops the reminder flow so customers don't receive emails about items they're no longer interested in.

### Setup

The only field you need to populate is your **Klaviyo Public API Key**. Find it in Klaviyo under **Account > Settings > API Keys**. Add it to the Flow, publish, and you're live.

* * *

## Other email platforms

The same Flow approach works for any platform with a Shopify Flow action. The templates above can be adapted — just swap the Klaviyo action for your platform's equivalent action and add your API credentials.

If you need help setting up a custom Flow for your platform, [contact support](mailto:support@nativeappco.com) and we'll get it done.

* * *

## Available Flow triggers

Fish Wishlist exposes the following triggers in Shopify Flow:

Trigger

When it fires

Product added to wishlist

Customer saves a product

Product removed from wishlist

Customer removes a product

These triggers include product details, customer ID, and wishlist metadata — enough to personalise your campaigns effectively.

* * *

## Notes

*   All integration logic lives in Shopify Flow — no custom code required
*   You can build flows beyond the provided templates
*   Fish Wishlist triggers don't require any additional app configuration