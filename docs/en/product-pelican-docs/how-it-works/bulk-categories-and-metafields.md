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

This walkthrough shows how to use Product Pelican to improve Shopify taxonomy data in two stages:

*   Populate the Shopify product category for products that are uncategorized.
*   Populate category metafields for products that are missing category attributes.

The flow starts by showing what Shopify already supports on an individual product, then moves into **Product Health** in Product Pelican, where you can review and apply suggestions in bulk.

In Product Pelican, the main screens used in this workflow are **Product Health** and **AI Prompts**. On Product Health, the relevant audit checks are **No Category** and **Missing Category Attributes**.

## Why this is important

Product categories and category metafields do more than organize your catalog. They turn basic product details into structured information that Shopify and other sales channels can understand. That structure helps your products appear in the right places, show the right filters, and give shoppers clearer information before they buy.

### Improve product discovery

*   **Better filtering on collection pages:** Category metafields support more specific filters such as color, size, material, neckline, or fabric.
*   **Faster product discovery:** When category data is filled in correctly, Shopify's Search and Discovery tools can turn those attributes into useful storefront filters.
*   **Less admin clutter:** Category metafields only appear for products in the relevant category, so your team sees the fields that matter for that type of product.

### Support SEO and channel accuracy

*   **Standardized product data:** Shopify categories and category metafields align with Shopify's standard product taxonomy, which is designed for use across major commerce platforms and channels.
*   **Stronger search visibility:** Detailed, well-structured attributes can help products surface more accurately in search, both on your storefront and across external channels.
*   **More accurate channel mapping:** Clear product classification makes it easier for marketplaces and ad channels to understand what you are selling.

### Save time and keep data consistent

*   **Relevant fields appear automatically:** Once a product is assigned to a category, Shopify can show the category-specific attributes that belong to that product type.
*   **More consistent catalog data:** Standardized entries such as approved colors, materials, or size types make bulk editing easier and reduce messy variations.
*   **Bulk workflows matter:** Reviewing one product at a time works for a small catalog, but Product Pelican helps you apply the same improvements across many products much faster.

### Create a better shopping experience

*   **Clearer product details:** Specific attributes like fabric, heel height, age group, or watch band material help customers understand exactly what they are buying.
*   **Better merchandising options:** Structured category data can support richer storefront experiences, including visual swatches and more relevant filters.
*   **Higher confidence before purchase:** The more accurate and specific your product data is, the easier it is for customers to compare items and make decisions.

<m-info>In short, categories and category metafields help customers find products faster, help sales channels understand your catalog more accurately, and help your team maintain cleaner product data at scale.</m-info>

## Part 1: Populate the product category

### What this looks like in Shopify on a single product

On the Shopify product editor, an uncategorized product can show a suggested value in the **Category** field. In the example below, Shopify suggests a category for a basic T-shirt product and marks it as **Suggested**.

This works well one product at a time, but it becomes slow when you need to review a large catalog.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ce553609-0cf8-4234-b1c8-269d6d958907/frame_001.jpg" alt="Shopify product editor showing an uncategorized product with a suggested category"></m-frame>

### Open the category audit in Product Pelican

In Shopify admin, open **Product Pelican** and go to **Product Health**. On the **Product Data Quality Dashboard**, look under **Audit Checks** and open **No Category**.

This audit lists products that do not have a Shopify category set. The table shows the product name, the **Suggested Category** column, and an **Actions** column.

 <m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/4c65dce6-f2ab-435b-951c-101d5b2fb9f6/frame_005.jpg" alt="Product Pelican Product Data Quality Dashboard showing the No Category audit check"> </m-frame><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/96c944eb-9436-4467-a840-7793146264a7/frame_006.jpg" alt="No Category audit list in Product Pelican before suggestions are generated"></m-frame>

### Generate category suggestions in bulk

Select **Suggest All** to generate category recommendations for the whole list. Product Pelican uses your product data to populate the **Suggested Category** column and shows a confidence badge, such as **High**.

For each row, you can:

*   Use **Apply** to accept the suggestion.
*   Use **Redo** to request another suggestion.
*   Use **Apply All Selected** when you want to process multiple reviewed suggestions together.

Use the confidence badge to decide how closely to review a suggestion. Higher-confidence matches are usually faster to approve, while weaker matches deserve a manual check.

 <m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ca224630-d3ba-4e87-b450-e0db1a857c53/frame_007.jpg" alt="No Category audit in Product Pelican showing suggested categories with confidence badges and apply actions"> </m-frame><m-tip>Review product titles and images before applying suggestions in bulk. Cleaner product data usually leads to more accurate category recommendations.</m-tip>

### Confirm the category has been applied

After you apply a category, open the product in Shopify and scroll to the **Category metafields** section. You should now see category-specific fields appear for that product type.

For example, a T-shirt can show fields like **Color**, **Sleeve length type**, **Neckline**, and **Fabric**. This confirms the product now has a Shopify category assigned.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/411a2582-da9e-4808-b241-57320a3b3bc4/frame_002.jpg" alt="Shopify product editor showing category metafields after a product category has been applied"></m-frame>

## Part 2: Populate missing category metafields

### Open the missing attributes audit

Return to **Product Health** in Product Pelican and open **Missing Category Attributes**.

This audit shows products that already have a Shopify category but still have missing category-specific details. Each row includes the product category and the number of attributes still to fill.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/149d0feb-897a-4c14-ba05-a41575f8f998/frame_008.jpg" alt="Missing Category Attributes audit in Product Pelican showing products with category-specific fields to complete"></m-frame>

### Review attributes before generating suggestions

Select **Show attributes** on a row to expand the missing fields for that product. Product Pelican displays the exact category attributes Shopify expects for that item.

You can leave a field as **skip** if you do not want to populate it, or choose a value manually if you already know the correct answer.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5d6fc861-925c-4d14-92b9-a963c148c38d/frame_011.jpg" alt="Expanded category attributes in Product Pelican showing dropdown fields ready for review"></m-frame>

### Generate AI suggestions for category attributes

Use **Suggest** on an individual row, or **Suggest All** to generate recommendations more broadly. Product Pelican will propose values for supported category attributes, such as:

*   Color
*   Pattern
*   Age group
*   Target gender
*   Fabric or material
*   Category-specific feature fields

Suggested values are labeled so you can distinguish AI recommendations from manual selections.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ed6036fd-5215-4c88-842a-4165a45d935c/frame_010.jpg" alt="Product Pelican showing AI-generated suggestions for category attributes such as pattern and age group"></m-frame>

### Manually choose a value when needed

If a suggestion is incomplete or you want to override it, open the dropdown for that attribute and choose the correct option from Shopify's allowed values.

This is especially useful for attributes with controlled options, such as **Fabric**, **Age group**, or other standardized lists.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/8edd12b6-3707-450c-ab3d-943f8397278f/frame_012.jpg" alt="Dropdown menu in Product Pelican for choosing a standardized category attribute value"></m-frame>

### Apply the reviewed values

After reviewing the populated fields, use **Apply** on the row to write the selected values back to Shopify. If you have reviewed several products, use **Apply All Selected** to process them together.

If a write fails, Product Pelican shows a retry state so you can attempt the update again after reviewing the affected fields.

<m-note>If you see an error on a specific row, review the selected values and try again. This is usually limited to the affected product rather than the whole batch.</m-note>

### Confirm the metafields in Shopify

Open the product in Shopify and return to the **Category metafields** section. The selected values should now be filled in on the product record.

In the example below, fields like **Color** and **Sleeve length type** are now populated.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/85bfe6e7-e3d0-4980-b16e-f71227fc94a9/frame_003.jpg" alt="Shopify category metafields with populated values such as color and sleeve length type"></m-frame>

These values can improve filtering, product discovery, and storefront presentation. On compatible themes and product setups, structured attributes can also support richer experiences such as color swatches and more precise filtering.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ba188504-aca0-4aed-9d0f-3bdf865234f2/frame_004.jpg" alt="Shopify product editor showing saved category metafields after review"></m-frame>

## Recommended workflow

<m-steps><m-step title="Fix uncategorized products first">Start with <strong>No Category</strong> in Product Health. Products need a Shopify category before category metafields can be completed. </m-step><m-step title="Apply categories in bulk">Use <strong>Suggest All</strong> to generate recommendations, then review high-impact products and apply approved categories. </m-step><m-step title="Fill missing category attributes">Move to <strong>Missing Category Attributes</strong> and use Product Pelican to suggest or manually select values for the remaining fields. </m-step><m-step title="Spot-check results in Shopify">Open a few updated products in Shopify to confirm that the right fields and values were written back successfully.</m-step></m-steps>

## Best practices

*   Assign categories before working on category metafields.
*   Review lower-confidence category suggestions more carefully.
*   Use manual selection when a standardized attribute value is obvious and important.
*   Prioritize bestsellers and high-traffic collections first if you are cleaning up a large catalog.
*   Re-run Product Health audits periodically to catch new products with missing taxonomy data.

<m-tip>If you import products from multiple sources, make taxonomy cleanup part of your regular merchandising workflow. Running these audits often keeps category data from drifting over time.</m-tip>

## What Product Pelican helps you do

*   Find products with no Shopify category.
*   Generate category suggestions in bulk.
*   Identify products with missing category-specific attributes.
*   Suggest values for category metafields using AI.
*   Apply reviewed taxonomy updates back to Shopify faster than editing products one by one.