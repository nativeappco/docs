---
type: page
title: Tiered Loyalty Program with Store Credit
description: Build a tiered cash-back loyalty program using native Shopify customer segments, native store credit, and Stork Credit — no points, no databases, no third-party redemption portals.
seoTitle: Tiered Loyalty Program with Native Store Credit | Stork Credit
seoDescription: Set up a multi-tiered loyalty program in Shopify using native customer segments and Stork Credit automatic store credit. No points, no databases.
slug: tiered-loyalty-program
order: 7
status: published
---

Build a tiered cash-back loyalty program using native Shopify customer segments, native store credit, and Stork Credit — no points, no databases, no third-party redemption portals.

Shopify's built-in store credit is real monetary value that lives on the customer's account, redeemable natively at checkout, with a full transaction log and automatic notification emails included.

Stork Credit handles the automation — issuing credit based on rules that you create.

<iframe src="https://www.youtube.com/embed/jGITvRNEg8I?modestbranding=1&amp;rel=0" class="youtube-iframe" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="true" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border-radius: 0.375rem;"></iframe>

## Step 1: Create customer segments

In Shopify admin go to **Customers → Segments** and create three segments. Sidekick can generate the queries for you. Make each segment mutually exclusive so a customer only qualifies for one tier at a time.

<colgroup><col style="min-width: 25px;"><col style="min-width: 25px;"><col style="min-width: 25px;"></colgroup>

Example Tier

Segment name

Lifetime spend

Bronze

Bronze Loyalty

$100 – $499

Silver

Silver Loyalty

$500 – $999

Gold

Gold Loyalty

$1,000+

Optional: Add a marketing opt-in condition to each segment, then save.

## Step 2: Set up Automatic Store Credit

In [Stork Credit](http://admin.shopify.com/apps/stork-credit) go to **Automatic Store Credit → Browse Templates** and select the _3% store credit rewards_ template.

*   Set your reward rate per tier (e.g. Bronze 3%, Silver 5%, Gold 7%)
    
*   Under **Eligibility**, choose _Specific customer segment_ and select the matching segment
    
*   Save and activate
    

Repeat for each tier. Stork Credit will apply the best-value promotion if a customer somehow qualifies for more than one (unless you change this in app settings).

## Step 3: Add the checkout widget

In your Shopify checkout editor, add the Stork Credit app block to checkout. This shows customers how much credit they'll earn before they pay — a simple but effective conversion nudge.

## How it works for customers

*   Credit is issued automatically after each qualifying order
    
*   Shopify sends a native store credit email notification
    
*   Customers redeem by ticking the store credit option in the checkout payment section
    

## Advanced: delay issuance with Shopify Flow

To hold credit until after a refund window has passed, build a Shopify Flow using the **Customer added to segment** trigger and the **Issue store credit** Stork Credit action. No code required.