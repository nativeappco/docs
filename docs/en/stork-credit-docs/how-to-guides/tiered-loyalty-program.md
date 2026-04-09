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

<iframe src="https://www.youtube.com/embed/jGITvRNEg8I?modestbranding=1&amp;rel=0" class="youtube-iframe" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="true" style="position: absolute; top: 0px; left: 0px; width: 100%; height: 100%; border-radius: 0.375rem;"></iframe>

Build a tiered cash-back loyalty program using native Shopify customer segments, native store credit, and Stork Credit — no points, no databases, no third-party redemption portals.

Shopify's built-in store credit is real monetary value that lives on the customer's account, redeemable natively at checkout, with a full transaction log and automatic notification emails included. Stork Credit handles the automation — issuing credit based on rules that you create.

## Step 1: Create customer segments

In Shopify admin go to **Customers → Segments** and create three segments. Sidekick can generate the queries for you. Make each segment mutually exclusive so a customer only qualifies for one tier at a time.

<table style="min-width: 75px;"><colgroup><col style="min-width: 25px;"><col style="min-width: 25px;"><col style="min-width: 25px;"></colgroup><tbody><tr><th colspan="1" rowspan="1"><p>Example Tier</p></th><th colspan="1" rowspan="1"><p>Segment name</p></th><th colspan="1" rowspan="1"><p>Lifetime spend</p></th></tr><tr><td colspan="1" rowspan="1"><p>Bronze</p></td><td colspan="1" rowspan="1"><p>Bronze Loyalty</p></td><td colspan="1" rowspan="1"><p>$100 – $499</p></td></tr><tr><td colspan="1" rowspan="1"><p>Silver</p></td><td colspan="1" rowspan="1"><p>Silver Loyalty</p></td><td colspan="1" rowspan="1"><p>$500 – $999</p></td></tr><tr><td colspan="1" rowspan="1"><p>Gold</p></td><td colspan="1" rowspan="1"><p>Gold Loyalty</p></td><td colspan="1" rowspan="1"><p>$1,000+</p></td></tr></tbody></table>

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
    

## Advanced options

### Delay issuance with Shopify Flow

By default, credit is issued immediately after an order is placed. If you want to hold it until after a refund window has passed, build a Shopify Flow using the **Order fulfilled** trigger, a **Wait** action for your desired delay period, then the **Issue store credit** Stork Credit action. No code required.

You can also use Flow to layer in more complex logic — for example, only issue credit if the order contains products from a specific collection, or issue a bonus credit amount when a customer first reaches a new tier.

### Run promotions like "double credit weekends"

Because promotions in Stork Credit are just rules you can turn on and off, running a time-limited promotion is straightforward. Create a separate automatic store credit rule with a higher reward rate (e.g. 6% instead of 3%), activate it at the start of the promotion period, and deactivate it when it ends. The best-value logic means eligible customers automatically get the higher rate while the promo is live — no changes needed to your base tier rules.

### Trigger Klaviyo campaigns when credit is earned

Use Shopify Flow to fire a webhook to Klaviyo when store credit is issued. This lets you send a branded "You've earned store credit!" email or SMS through Klaviyo rather than the default Shopify notification — giving you full control over design, copy, and timing. You can also use the trigger to add customers to a Klaviyo segment, enabling follow-up flows like reminding customers they have unspent credit if they haven't purchased in 30 days.