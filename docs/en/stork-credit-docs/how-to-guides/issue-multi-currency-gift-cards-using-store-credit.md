---
type: page
title: Issue Multi Currency Gift Cards using Store Credit
description: Learn how to use Stork Credit and Shopify Flow to replace gift card codes with store credit that is issued and redeemed in the customer's order currency.
seoTitle: Multi-currency gift cards with Stork Credit
seoDescription: Use Stork Credit instead of Shopify gift cards for Shopify Markets so customers redeem credit in the correct currency.
slug: issue-multi-currency-gift-cards-using-store-credit
order: 0
status: draft
---

## Why use store credit instead of Shopify gift cards?

Shopify gift cards have an important limitation with Shopify Markets: when a gift card is sold, its value ultimately ties back to your store's master currency. That means the value a customer receives can shift between the time the gift card is purchased and the time it is redeemed.

Stork Credit solves this by issuing **store credit in the currency of the order**. If a customer buys the gift card product in AUD, you can issue AUD store credit. If they buy the same product in USD through a market with local pricing, you can issue USD store credit instead.

<m-info>This walkthrough demonstrates replacing a traditional gift card code with store credit, so the customer redeems the correct value in their own currency at checkout.</m-info>

## What this walkthrough shows

In the demo, the same gift card product is purchased twice:

*   once in the store currency
*   once in a Shopify Markets currency with local pricing

Each purchase creates store credit entries in the matching currency, and those balances appear on the customer's Shopify profile under **Store credit**.

## Walkthrough

<m-steps><m-step title="Review the gift card orders"><p>Start in <strong>Shopify admin &gt; Orders</strong>. The walkthrough shows two recent orders on the Orders list, each containing three gift card line items. This confirms the setup can handle multiple gift card values in a single purchase.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/f77c5f4c-8f2f-4f6d-b78f-587e4ccf97ba/frame_001.jpg" alt="Shopify Orders list showing recent gift card orders"></m-frame><p>In the example, one order is placed in the store currency and another is placed in USD.</p></m-step><m-step title="Check the order in the store currency"><p>Open the first order from the <strong>Orders</strong> screen. On the order details page, the <strong>Unfulfilled</strong> section shows three separate <strong>Gift Card</strong> line items for <strong>$25</strong>, <strong>$50</strong>, and <strong>$100</strong>.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/e1113558-5fb5-4d4d-9ea0-8b5ed6ef144e/frame_002.jpg" alt="Shopify order details showing three gift card line items"></m-frame><p>This part of the walkthrough confirms that the automation can issue store credit for each qualifying line item in the order.</p></m-step><m-step title="Check the order in a Shopify Markets currency"><p>Open the second order and review the same gift card product purchased in <strong>USD</strong>. On the order details page, Shopify shows the line item values in USD and the payment section shows the converted amount paid in the store currency.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/48a805db-34eb-4284-b66d-aeee82c27067/frame_003.jpg" alt="Shopify order details showing gift card prices in USD and converted payment amount"></m-frame><p>This is the key difference: instead of converting a gift card back to the master currency later, Stork Credit can issue the balance directly in USD.</p></m-step><m-step title="Open the customer profile and confirm the balances"><p>From the order, open the customer record in <strong>Shopify admin &gt; Customers</strong>. On the right side of the customer profile, the <strong>Store credit</strong> card shows separate balances for each currency.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/27fb5cbf-913b-40c8-b302-8c413d8b535e/frame_006.jpg" alt="Customer profile showing store credit balances in AUD and USD"></m-frame><p>In the demo, the customer has both <strong>AUD</strong> and <strong>USD</strong> balances available.</p></m-step><m-step title="Review the credit transactions on the timeline"><p>Scroll to the customer's <strong>Timeline</strong>. You can see Stork Credit entries such as <strong>Stork Credit credited this customer $100.00 USD in store credit</strong> and equivalent entries in AUD.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ed0a493d-22da-4fa4-acb9-317a8fa5bb39/frame_005.jpg" alt="Customer timeline showing Stork Credit entries in USD and AUD"></m-frame><p>These timeline events are useful for checking that your Shopify Flow automation credited the correct amounts in the correct currency.</p></m-step><m-step title="Understand how redemption works"><p>When the customer reaches checkout, they can redeem store credit in the currency of the order they are placing.</p><ul><li>If they check out in AUD, they can use their AUD balance.</li><li>If they check out in USD, they can use their USD balance.</li></ul><p>The customer cannot combine AUD and USD balances on the same order, which is usually acceptable because most customers shop in one market at a time.</p></m-step></m-steps>

## What you need in your setup

*   **Stork Credit** installed
*   **Shopify Flow** automation that issues store credit when the gift card product is purchased
*   **Shopify Markets** pricing configured if you want the same product to sell in different local currencies

The walkthrough is based on a setup where the same product has local market pricing, and the Flow issues store credit based on the order currency.

<m-tip>If you are already using the gift card product as the purchase trigger, you can keep that product experience for shoppers while delivering store credit instead of a gift card code behind the scenes.</m-tip>

## Important behavior to understand

<m-warning>Store credit balances are currency-specific. A customer can hold multiple balances, but they redeem only the balance that matches the currency of their current checkout.</m-warning>

*   This avoids exchange-rate changes affecting the stored value.
*   It also gives customers a more predictable redemption experience in Shopify Markets.

## Sending credit to a friend

If you want customers to buy this as a gift for someone else, you will need an extra step in your storefront and automation.

1.  Capture the recipient's email address as a **line item property** on the gift card product.
2.  Update your Shopify Flow so the credit is issued to that recipient instead of the purchaser.

This lets you keep the same multi-currency store credit approach while supporting gifting workflows.

## Emailing the recipient

By default, you can rely on Shopify's store credit notification template, but many stores prefer a more polished gift experience.

You can connect an email platform such as **Klaviyo** to send a more customer-friendly email after the credit is issued.

<m-note>This is especially useful if you want branded gifting emails, scheduled sends, or custom messaging for the sender and recipient.</m-note>

## Best use case for this workflow

This setup is a strong fit if you:

*   sell internationally with **Shopify Markets**
*   want customers to receive a fixed value in their purchase currency
*   need a better alternative to Shopify gift cards for multi-currency stores

## Need help?

If you need help setting this up, contact [support@nativeappco.com](mailto:support@nativeappco.com).