---
type: page
title: Bulk categories and metafields
description: Learn how to assign Shopify product categories in bulk and fill missing category metafields using Product Pelican’s Product Health audits and AI suggestions.
seoTitle: Bulk Shopify categories and metafields
seoDescription: Use Product Pelican to bulk populate Shopify product categories and category metafields with AI suggestions and review tools.
slug: bulk-categories-and-metafields
order: 0
status: draft
---

## Overview

This walkthrough shows how to use **Product Pelican** to improve Shopify taxonomy data in two stages:

1.  **Populate the Shopify product category** for products that are uncategorized.
2.  **Populate category metafields** for products that are missing category attributes.

The flow starts by showing what Shopify already supports on an individual product, then moves into **Product Health** in Product Pelican, where you can review and apply suggestions in bulk.

<m-info>In Product Pelican, the main screens used in this workflow are <strong>Product Health</strong> and <strong>AI Prompts</strong>. On <strong>Product Health</strong>, the relevant audit checks are <strong>No Category</strong> and <strong>Missing Category Attributes</strong>.</m-info>

## Part 1: Populate the product category

### What this looks like in Shopify on a single product

On the Shopify product editor, an uncategorized product can show a suggested value in the **Category** field. In the walkthrough, Shopify suggests a category for a basic T-shirt product and marks it as **Suggested**.

This works well one product at a time, but it becomes slow when you need to review a large catalog.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ce553609-0cf8-4234-b1c8-269d6d958907/frame_001.jpg" alt="Shopify product editor showing an uncategorized product with a suggested category"></m-frame>

### Open the category audit in Product Pelican

In Shopify admin, open **Product Pelican** and go to **Product Health**. On the **Product Data Quality Dashboard**, look under **Audit Checks** and open **No Category**.

This audit lists products that do not have a Shopify category set. The table shows the product name, the **Suggested Category** column, and an **Actions** column.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/4c65dce6-f2ab-435b-951c-101d5b2fb9f6/frame_005.jpg" alt="Product Health dashboard showing the Product Data Quality Dashboard and audit checks including No Category"></m-frame><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/96c944eb-9436-4467-a840-7793146264a7/frame_006.jpg" alt="No Category issue list showing products missing categories with Suggest buttons"></m-frame>

### Generate category suggestions in bulk

Select **Suggest All** to generate category recommendations for the whole list. Product Pelican uses your product data to populate the **Suggested Category** column and shows a confidence badge, such as **High**.

For each row, you can:

*   Use **Apply** to accept the suggestion
*   Use **Redo** to request another suggestion
*   Use **Apply All Selected** when you want to process multiple reviewed suggestions together

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ca224630-d3ba-4e87-b450-e0db1a857c53/frame_007.jpg" alt="No Category audit showing generated category suggestions with confidence badges and Apply actions"></m-frame><m-tip>Use the confidence badge to decide how closely to review a suggestion. Higher-confidence matches are usually faster to approve, while weaker matches deserve a manual check.</m-tip>

### Confirm the category has been applied

After you apply a suggestion, Product Pelican updates the row status. In the walkthrough, applied products are clearly marked as **Applied**, making it easy to see which products are done and which still need review.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/149d0feb-897a-4c14-ba05-a41575f8f998/frame_008.jpg" alt="No Category audit showing a product marked as Applied after categorization"></m-frame><m-steps><m-step title="Open Product Health">In <strong>Product Pelican</strong>, go to <strong>Product Health</strong>.</m-step><m-step title="Open No Category">From <strong>Audit Checks</strong>, select <strong>No Category</strong>.</m-step><m-step title="Generate suggestions">Select <strong>Suggest All</strong> or use <strong>Suggest</strong> on specific rows.</m-step><m-step title="Review the suggested category">Check the taxonomy path and confidence badge.</m-step><m-step title="Apply the category">Select <strong>Apply</strong> for individual products or <strong>Apply All Selected</strong> after reviewing multiple rows.</m-step></m-steps>

## Part 2: Populate category metafields

### What this looks like in Shopify on a single product

Once a Shopify product category is set, Shopify can expose matching **Category metafields** on the product page. In the walkthrough, the product shows attribute chips such as **Color**, **Sleeve length type**, **Age group**, **Neckline**, **Target gender**, **Fabric**, and **Size**.

You can add values manually on the product page, for example selecting **Blue** for color and **Short** for sleeve length type, then saving the product.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/411a2582-da9e-4808-b241-57320a3b3bc4/frame_002.jpg" alt="Shopify product editor showing category metafield attribute chips"></m-frame><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/85bfe6e7-e3d0-4980-b16e-f71227fc94a9/frame_003.jpg" alt="Shopify category metafields form with selected values and sleeve length type picker open"></m-frame><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ba188504-aca0-4aed-9d0f-3bdf865234f2/frame_004.jpg" alt="Completed Shopify category metafields showing saved color and sleeve length values"></m-frame>

This is manageable for one product, but not for dozens or hundreds of products.

### Open the missing category attributes audit

Back in **Product Health**, open the **Missing Category Attributes** audit. This view lists products that already have a category but still need category-specific attributes filled in.

Each row shows the product, its category path, and the number of attributes left to complete. Use **Show 16 attributes**, **Show 7 attributes**, or similar buttons to expand the editable fields for a product.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2c85b37c-30a6-4b29-9964-272e60864a6a/frame_009.jpg" alt="Missing Category Attributes list showing products, categories, attribute counts, and Suggest buttons"></m-frame>

### Generate AI suggestions for category attributes

Use **Suggest** on a product row to generate attribute values. Product Pelican fills what it can and labels suggested values with AI indicators such as **AI: Birds** or **AI: Adults** in the walkthrough.

When a row is expanded, you can review each field individually. Some attributes may remain set to **skip** if Product Pelican cannot determine a confident answer.

At that point, you can either accept the suggested values as-is or manually choose values from the dropdowns before saving.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ed6036fd-5215-4c88-842a-4165a45d935c/frame_010.jpg" alt="Expanded category attributes with AI-recommended values and Apply action"></m-frame><m-tip>If a field stays on <strong>skip</strong>, that usually means there is not enough product information for a safe suggestion. You can fill only the fields you know and leave the rest for later.</m-tip>

### Review and complete any missing fields manually

The expanded row acts like a compact editor. You can open dropdowns for fields such as **Fabric**, **Age group**, **Target gender**, and other category-specific attributes, then select the right value directly in Product Pelican.

This gives you a faster bulk workflow than opening each Shopify product page one by one.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/8edd12b6-3707-450c-ab3d-943f8397278f/frame_012.jpg" alt="Expanded category attribute fields ready for manual input inside Product Pelican"></m-frame>

### Apply the attribute values

When the row looks correct, select **Apply** to write the category attribute values back to Shopify. If you want a fresh set of suggestions first, use **Redo**.

If Product Pelican cannot save a row successfully, the audit can show a retry state. In the walkthrough, a failed row displays **Retry**, making it clear which products still need attention.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5d6fc861-925c-4d14-92b9-a963c148c38d/frame_011.jpg" alt="Missing Category Attributes audit showing a retry state after an apply attempt"></m-frame><m-steps><m-step title="Open Missing Category Attributes">From <strong>Product Health</strong>, select <strong>Missing Category Attributes</strong>.</m-step><m-step title="Expand a product row">Use <strong>Show X attributes</strong> to display the missing fields.</m-step><m-step title="Generate suggested values">Select <strong>Suggest</strong> for the product.</m-step><m-step title="Review and edit">Check each attribute, replace <strong>skip</strong> values where needed, and choose manual values from dropdowns.</m-step><m-step title="Apply the updates">Select <strong>Apply</strong> to save the category attribute values.</m-step></m-steps>

## Improve suggestions with AI Prompts

If you want category or attribute suggestions to better match your catalog rules, open **AI Prompts** from the Product Pelican navigation. This page lets you customize how Product Pelican generates future AI output.

For taxonomy work, the most relevant section is **Category Prompt**. You can use it to give the app clearer rules about your catalog, such as preferred category logic or store-wide patterns that should influence suggestions.

<m-note>Changes on <strong>AI Prompts</strong> affect future suggestions. After saving prompt updates, go back to <strong>Product Health</strong> and generate fresh suggestions in <strong>No Category</strong> or <strong>Missing Category Attributes</strong>.</m-note>

## Recommended workflow

1.  Start in **Product Health** and open **No Category**.
2.  Run **Suggest All** and apply the category suggestions you approve.
3.  Then open **Missing Category Attributes**.
4.  Expand products with **Show X attributes**, run **Suggest**, and complete any remaining fields manually.
5.  Use **Apply** to save the completed attribute values.
6.  If suggestions need improvement, update your rules in **AI Prompts** and regenerate.

<m-warning>Product Pelican helps speed up category and category metafield work, but you should still review suggestions before applying them at scale, especially when product titles or descriptions are vague.</m-warning>