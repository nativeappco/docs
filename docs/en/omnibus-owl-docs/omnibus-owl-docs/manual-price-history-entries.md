---
type: page
title: Add Manual Price History Entries
description: Learn how to add, edit, and remove manual price history entries in Omnibus Owl using the Product Price History block for products with custom promotions.
seoTitle: Manual price history entries in Omnibus Owl
seoDescription: Add manual price history entries in Omnibus Owl using the Product Price History block so custom promotions stay compliant and transparent.
slug: manual-price-history-entries
order: 0
status: draft
---

## When to use manual price history entries

Omnibus Owl automatically tracks most product price changes, but some promotions do not create a standard tracked price change in Shopify. When that happens, you can add a manual entry so your storefront still reflects the correct lowest-price history for compliance and customer transparency.

This is especially useful for custom promotions that need to be represented in a product's price history even though they were not captured automatically.

<m-info>Use manual entries only when you need to fill in a real pricing event that Omnibus Owl could not track automatically. They are designed to support accurate disclosures, not to replace normal price tracking.</m-info>

## Where to add a manual price edit

Manual entries are added from the **Product Price History** block that appears alongside each product in your store.

In Omnibus Owl, you can first locate the product from the **Dashboard** using the **Search variants...** field. The dashboard also shows helpful columns like **Current Price**, **Lowest Price**, **Price Changes**, and **Status**, so you can confirm you are working on the correct item.

<m-note>Omnibus Owl may also refer to this storefront disclosure as the <strong>Price history</strong> or lowest-price widget. The manual editing area shown in the product-side block is labeled <strong>Price history</strong> in the UI.</m-note><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/68d69096-9c4d-48ab-8fbe-29c163410f5e/image__18_.png" alt="Omnibus Owl Product Price History block showing Market, Date, Time, Price, Add entry, and edit and delete controls"></m-frame>

## Add a manual price history entry

<m-steps><m-step title="Open the product's Price history block"><p>Go to the product you want to update and find the <strong>Price history</strong> block shown alongside that product.</p></m-step><m-step title="Choose the market"><p>Use the <strong>Market</strong> dropdown to select the correct storefront market, such as <strong>United States (US)</strong>. Manual entries are market-specific, so make sure you are updating the same market customers will shop in.</p></m-step><m-step title="Review the current lowest price"><p>At the top of the block, Omnibus Owl shows the current summary, such as <strong>Lowest price (last 30 days)</strong> and the date and time of that lowest price. Review this first so you understand how your manual entry may affect the displayed history.</p></m-step><m-step title="Enter the historical price change"><p>Fill in the three input fields:</p><ul><li><strong>Date</strong> — enter the date of the price event</li><li><strong>Time</strong> — enter the time the price took effect</li><li><strong>Price</strong> — enter the product price for that moment in the selected market currency</li></ul></m-step><m-step title="Click Add entry"><p>Select <strong>Add entry</strong> to save the manual price edit. The new row will appear in the list below the form with its timestamp and price.</p></m-step></m-steps>

## How the saved entry appears

After you click **Add entry**, the entry is listed in the history table underneath the form. Each row shows the recorded date and time on the left and the saved price on the right.

If the new record becomes the lowest qualifying price in the last 30 days, the summary at the top of the block updates to reflect it.

<m-tip>If you are documenting a promotion that ran for a specific market only, always check the <strong>Market</strong> selector before saving. The same product can have different price histories across markets.</m-tip>

## Edit an existing manual entry

If you entered the wrong date, time, or price, you can update the record directly from the same block.

<m-steps><m-step title="Find the entry in the list"><p>Locate the saved row you want to change in the history list.</p></m-step><m-step title="Click the edit icon"><p>Select the pencil icon on that row.</p></m-step><m-step title="Update the details"><p>Correct the <strong>Date</strong>, <strong>Time</strong>, or <strong>Price</strong> values as needed.</p></m-step><m-step title="Save the change"><p>Confirm the update in the block so the corrected value appears in the price history list.</p></m-step></m-steps>

## Delete a manual entry

If a manual entry was added by mistake, you can remove it from the same list.

<m-steps><m-step title="Find the incorrect entry"><p>Locate the row you want to remove.</p></m-step><m-step title="Click the delete icon"><p>Select the trash icon on that row.</p></m-step><m-step title="Confirm the removal"><p>Remove the entry so it no longer affects the product's displayed price history.</p></m-step></m-steps><m-warning>Delete entries carefully. Removing a valid historical price record can change the <strong>Lowest price (last 30 days)</strong> shown to customers.</m-warning>

## Best practices for manual price edits

*   Only add entries for real historical pricing events.
*   Match the entry to the correct **Market**.
*   Use the exact date and time the promotional price became active.
*   Double-check the currency and amount before clicking **Add entry**.
*   Review the updated lowest-price summary after saving.

## How this fits with automatic tracking

Manual entries are most useful for exceptions. Omnibus Owl still handles normal tracking in the background, and your main controls remain in the app navigation:

*   **Dashboard** for auditing tracked products and using **Search variants...**
*   **Settings** for rules like **Show only on discounted products**, **Include current price when calculating lowest price**, and **Show info tooltip**
*   **Languages** for editing the storefront label and tooltip copy
*   **Price Insights** for reviewing price timelines by product and **Market**

<m-note>Omnibus Owl tracks price history from the date the app was installed. Manual entries help you maintain accurate records for cases the app could not capture automatically, but they do not reconstruct all historic data from before installation.</m-note>

## Related pages

<m-cardgroup><m-card title="Dashboard Screen" href="/dashboard-screen">Use the dashboard to find products, review tracking status, and inspect recorded price changes.</m-card><m-card title="Settings" href="/settings">Control how the lowest-price widget behaves across your storefront.</m-card><m-card title="Language Settings" href="/language-settings">Customize the lowest-price label and info tooltip text shown to shoppers.</m-card><m-card title="Manual price history tag" href="/manual-price-history-tag">Place the Omnibus Owl lowest-price message in custom storefront locations.</m-card></m-cardgroup>