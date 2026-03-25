---
type: page
title: Set Up a Tiered Loyalty Program with Store Credit
seoTitle: Set Up a Tiered Loyalty Program with Shopify Store Credit | Stork Credit
seoDescription: Learn how to create a multi-tiered loyalty program in Shopify using native customer segments and Stork Credit automatic store credit — no points, no databases.
slug: tiered-loyalty-program-setup
order: 7
status: draft
---

This guide walks you through setting up a multi-tiered loyalty program in Shopify that rewards customers with store credit based on their lifetime spend. It uses native Shopify customer segments, native Shopify store credit, and Stork Credit's automatic store credit feature.

No points. No third-party databases. No clunky redemption portals.

## Step 1: Create your customer segments in Shopify

In your Shopify admin, go to **Customers → Segments** and create three segments. You can use Sidekick to generate the queries, or create them manually.

Each segment should be mutually exclusive — a customer should only qualify for one tier at a time.

Tier

Segment name

Lifetime spend range

Bronze

Bronze Loyalty

$100 – $499

Silver

Silver Loyalty

$500 – $999

Gold

Gold Loyalty

$1,000+

Add a condition to only include customers who have opted into marketing. Save each segment with a clear name (e.g. Bronze Loyalty).

> **Tip:** Shopify provides a library of segment templates — browse these for additional ideas, such as segments based on order frequency or product category purchases.

## Step 2: Set up automatic store credit in Stork Credit

In the Stork Credit app, go to **Automatic Store Credit** and click **Browse Templates**. Select the _3% store credit rewards_ template as your starting point.

Configure the promotion:

*   Set the reward rate (e.g. 3% cash back on every order)
*   Optionally restrict to specific collections or products
*   Optionally set a minimum purchase requirement
*   Under **Eligibility**, select _Specific customer segment_ and choose **Bronze Loyalty**

Save the promotion, then activate it. Repeat this process to create separate promotions for Silver Loyalty and Gold Loyalty — you can vary the reward rate per tier (e.g. Bronze 3%, Silver 5%, Gold 7%).

> **Tip:** Stork Credit will automatically apply the best-value promotion when a customer qualifies for multiple segments. To keep things clean, use mutually exclusive segments so only one promotion applies per order.

## Step 3: Enable the store credit widget at checkout

In your Shopify theme editor, add the Stork Credit **app block** to your checkout. This displays a message showing how much store credit the customer will earn from the current order — visible before they complete their purchase.

> **Tip:** This "earn" message is a great conversion nudge — customers can see the reward before they pay.

## Step 4: How it works at checkout for customers

Once set up, the experience is fully native. When a customer places an order:

*   Stork Credit issues the store credit automatically based on the order total
*   Shopify sends the customer a native store credit notification email
*   The customer's store credit balance is updated in their account
*   At future checkouts, customers can apply their store credit in the payment section

## Step 5: Advanced — delay issuance with Shopify Flow

If you want to delay store credit issuance — for example, to wait until the refund window has passed — you can build a Shopify Flow using the **Customer added to segment** trigger and the **Issue store credit** action from Stork Credit. This gives you full control over timing and conditional logic without any custom code.