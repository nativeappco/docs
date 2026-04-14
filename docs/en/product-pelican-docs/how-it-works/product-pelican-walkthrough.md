---
type: page
title: Product Pelican walkthrough
description: A walkthrough-based overview of Product Pelican, including the Product Health dashboard, GEO Score, audit workflows, bulk fixes, and AI Prompts.
seoTitle: Product Pelican walkthrough and features
seoDescription: See how Product Pelican audits product data, fixes issues in bulk, and uses AI Prompts to improve titles, descriptions, alt text, and categories.
slug: product-pelican-walkthrough
order: 0
status: draft
---

## What Product Pelican does

Product Pelican helps you review catalog quality, spot missing or weak product data, and apply improvements without opening every product in Shopify one by one. The app starts by auditing your catalog across 12 checks, then gives you action panels where you can fix issues directly.

The walkthrough shown here follows the main flow most merchants use: start on **Product Health**, review **Audit Checks** and **GEO Score**, fix issues in bulk, then fine-tune output from the **AI Prompts** page.

<m-info>In the Shopify admin navigation shown in the walkthrough, Product Pelican includes <strong>Product Health</strong>, <strong>AI Prompts</strong>, and <strong>Plans</strong>.</m-info><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/6c1fb509-dbb3-438e-9e24-6e0d1771a4a8/frame_001.jpg" alt="Shopify App Store listing for Product Pelican"></m-frame>

## Start on Product Health

The main workspace in the walkthrough is **Product Health**. At the top of the **Product Data Quality Dashboard**, you can quickly see:

*   **Active Products**
*   **Total Variants**
*   **Products with Issues**
*   **Clean Products**

Below that, the dashboard has two main tabs:

*   **Audit Checks** for issue-based cleanup workflows
*   **GEO Score** for product scoring, filtering, and prioritization

The walkthrough shows these audit cards on the dashboard:

*   **No Images**
*   **Only 1 Image**
*   **Missing Alt Text**
*   **No Category**
*   **Vague Titles**
*   **Short Titles**
*   **No Description**
*   **Short Description**
*   **Ambiguous Language**
*   **Unclear Options**
*   **Missing SKUs**
*   **Zero Price Variants**

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5f075391-8b16-48b6-996a-24ab27d42e4d/frame_002.jpg" alt="Product Health dashboard with summary cards and audit checks"></m-frame><m-tip>Start with the audit cards that show the highest counts. This is usually the fastest way to improve a large number of products.</m-tip>

## Use GEO Score to prioritize products

The **GEO Score** tab gives you another way to work through your catalog. Instead of focusing on one issue type at a time, it scores products and groups them by quality band so you can decide what needs attention first.

In the walkthrough, the score view includes:

*   Band filters for **All**, **Poor**, **Needs work**, **Solid**, and **AI-ready**
*   Sortable columns such as **Product**, **Score**, and **Band**
*   Per-product score badges that help explain where quality is strong or weak

This view is useful if you want to improve the weakest products first before moving through every audit type.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/67f9665f-043b-4e1b-bc48-530db26fa85a/frame_003.jpg" alt="GEO Score tab with score bands and sortable product table"></m-frame>

## Fix missing product images

The walkthrough first moves into image-related audits. Opening **No Images** shows a list of affected products and an **Add Images** area for each row.

In the video, the image uploader supports adding files directly inside the audit panel, so you can fix missing product images without opening each product page separately.

*   Each row shows the product name
*   The upload area includes an **Add files** button
*   Accepted files are image files

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/36e77244-7f59-4692-97fb-d2abeec7a6fc/frame_004.jpg" alt="No Images audit with product list and image upload fields"></m-frame><m-note>The walkthrough also mentions the <strong>Only 1 Image</strong> check, which helps you find products that may need more than a single image even if they are not completely missing media.</m-note>

## Generate and save alt text

The **Missing Alt Text** audit is one of the most detailed workflows in the app. When you open it, Product Pelican shows product image cards with the current status, a generated alt text suggestion, and actions for reviewing and saving the result.

In the walkthrough, this panel includes:

*   Tabs for **Missing / Poor** and **All Images**
*   Bulk actions **Generate All** and **Save All**
*   A row-level action **Generate Alt Text**
*   Status labels such as **No alt text**
*   A visible character count under the suggested copy

You can generate alt text one image at a time, edit the suggestion if needed, and then apply it directly to the product image. If you are cleaning up many products at once, use the bulk actions instead.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/b1ade114-8c92-4fc6-a0c7-09d2d6417fe7/frame_005.jpg" alt="Missing Alt Text panel with image cards and bulk actions"></m-frame><m-steps><m-step title="Open Missing Alt Text">From <strong>Product Health</strong>, select the <strong>Missing Alt Text</strong> card.</m-step><m-step title="Generate suggestions">Choose <strong>Generate Alt Text</strong> for one item or <strong>Generate All</strong> for the full set.</m-step><m-step title="Review the text">Check the suggested wording and edit it if you want more precise wording.</m-step><m-step title="Save changes">Use <strong>Apply</strong> on individual items or <strong>Save All</strong> after reviewing multiple suggestions.</m-step></m-steps>

## Fill in missing Shopify categories

The **No Category** audit checks whether the Shopify category field has been set on each product. This is especially useful for catalogs imported from CSV files or external systems where taxonomy data may be missing.

The walkthrough shows two stages of this workflow.

### Stage 1: Request category suggestions

Before suggestions have been generated, the panel lists products with the note **No Shopify category set**. You can request recommendations one product at a time with **Suggest** or run **Suggest All**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/48d5c1fd-6daa-4055-b9dd-19eaaf56548d/frame_006.jpg" alt="No Category audit before suggestions are generated"></m-frame>

### Stage 2: Review and apply suggestions

After Product Pelican returns recommendations, the table shows a **Suggested Category** and confidence labels such as **Low**. You can then use **Apply** to accept a suggestion or **Redo** to generate another one. The walkthrough also shows **Apply All Selected** for bulk approval and **Applied** status labels once a category has been saved.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5f61d166-042b-4952-8159-5b0384232658/frame_007.jpg" alt="No Category results view with suggested taxonomy and apply actions"></m-frame><m-tip>If a suggestion is marked with lower confidence, review it before applying. Product Pelican makes the recommendation process faster, but you still control what is written back to the product.</m-tip>

## Improve short titles with AI suggestions

The **Short Titles** audit finds titles that are not descriptive enough. In the walkthrough, each row shows the product, the issue, a **Suggested Title** column, and action buttons.

The title workflow includes:

*   **Suggest** to generate one title
*   **Suggest All** to generate titles in bulk
*   **Apply** to accept a suggestion
*   **Redo** to generate a new variation
*   **Save All** for bulk approval

The video also shows why review matters: one suggestion includes unwanted wording based on the current prompt rules. This is a good reminder that AI suggestions are meant to speed up editing, not replace review.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/e715e6c5-6337-4fd4-b7d8-eee970f9437f/frame_008.jpg" alt="Short Titles audit showing suggested titles with Apply and Redo actions"></m-frame><m-warning>Always review generated titles before applying them in bulk. The walkthrough specifically shows that prompt settings can introduce wording you may not want in live product titles.</m-warning>

## Write fuller product descriptions

Product Pelican can also help with products that have no description or a description that is too short. In the walkthrough, the main example focuses on **Short Description**.

This panel includes:

*   **Write All** for bulk generation
*   **Write** for individual rows
*   **Apply** to save a generated description
*   **Redo** if you want another version
*   A visible issue note such as **Description is only 96 chars**

The suggested description appears in the **Suggested Description** column so you can review the text before writing it back to Shopify.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/4c6d7505-5796-4f22-b38c-e7556891b398/frame_009.jpg" alt="Short Description audit with generated product description suggestions"></m-frame>

## Watch the dashboard update after changes

After fixes are applied, the walkthrough returns to **Product Health** and shows updated issue counts on the audit cards. This makes it easy to see whether your cleanup work is reducing the number of products with problems.

From there, the next step in the walkthrough is to open **AI Prompts** from the app navigation.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2da62005-aba3-4b12-88f2-d9b8c4221b02/frame_010.jpg" alt="Updated Product Health dashboard with revised issue counts and AI Prompts in the sidebar"></m-frame>

## Customize AI Prompts

The **AI Prompts** page lets you control how Product Pelican generates content for your store. Prompt changes are saved per shop, so you can tailor results to your catalog, brand voice, and business rules.

In the walkthrough, this page includes editable sections for:

*   **Title Prompt**
*   **Description Prompt**
*   **Alt Text Prompt**
*   **Category Prompt**

It also includes a **Reset All to Defaults** button if you want to remove custom instructions and return to the standard prompt set.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2b481867-b98a-4cfb-95d7-f2a49c1741ec/frame_011.jpg" alt="AI Prompts page with Title Prompt and Description Prompt sections"></m-frame>

### Title Prompt

The walkthrough edits the **Title Prompt** to change how title suggestions are generated. This is where you can define rules such as:

*   Whether to include vendor names
*   How to treat color information
*   Target title length
*   Formatting rules like avoiding ALL CAPS

The video shows a concrete example: a rule telling the AI to always mention the vendor led to titles that were not ideal. After adjusting the prompt, future suggestions become more useful.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/cd23425e-706f-4677-9a37-06b013ef7585/frame_012.jpg" alt="Edited Title Prompt with custom rules for generating product titles"></m-frame>

### Description Prompt

The **Description Prompt** controls how product descriptions are written. In the walkthrough, custom instructions are added so generated descriptions mention shipping details such as free shipping in Australia for orders over $150.

This is useful when you want the AI to include store-specific information consistently, instead of writing generic marketing copy.

### Alt Text Prompt

The **Alt Text Prompt** lets you guide how image descriptions are created. In the walkthrough, the prompt includes rules for character count, avoiding phrases like “image of,” and describing what is actually visible in the image.

### Category Prompt

The **Category Prompt** controls how Shopify taxonomy suggestions are chosen. The walkthrough shows that you can add restrictions and catalog-specific rules so category recommendations better match the types of products you sell.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/0dac188e-c4aa-46d1-a2bd-ba5129d0ba33/frame_015.jpg" alt="AI Prompts page showing Alt Text Prompt and Category Prompt sections"></m-frame>

## Use prompt tuning to improve future suggestions

One of the most useful parts of the walkthrough is that it shows both good and bad outcomes. After changing the title rules in an intentionally unhelpful way, the next set of short-title suggestions becomes clearly worse. This illustrates how directly prompt settings affect the results you see in audits.

In other words, if title, description, alt text, or category suggestions feel off, the best next step is often to refine the relevant prompt and then generate fresh suggestions.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/ff16f8b0-a9ac-4b04-991c-371a3509af0d/frame_013.jpg" alt="Short Titles results showing poor AI suggestions after prompt changes"></m-frame><m-warning>Prompt changes affect future generations. If you update a prompt, go back to the related audit and run <strong>Suggest</strong>, <strong>Suggest All</strong>, <strong>Write</strong>, <strong>Write All</strong>, or <strong>Generate All</strong> again to see the new behavior.</m-warning>

## Save prompt changes

When you edit prompt text, the page shows an **Unsaved changes** banner with **Discard** and **Save** actions. Make sure you save your changes before leaving the page if you want them to apply to future AI suggestions.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/8853d1b7-0989-4314-99d1-f0c37ad42236/frame_016.jpg" alt="AI Prompts page with unsaved changes banner and save controls"></m-frame>

## Feature summary

<m-accordiongroup><m-accordion title="Product Health dashboard">A store-wide overview of catalog quality with summary cards, 12 audit checks, and quick access to cleanup workflows.</m-accordion><m-accordion title="GEO Score">A scoring view that groups products by quality band so you can filter, sort, and prioritize improvements.</m-accordion><m-accordion title="No Images and Only 1 Image">Flags products with weak image coverage so you can add missing product media more efficiently.</m-accordion><m-accordion title="Missing Alt Text">Generates image alt text suggestions, supports bulk generation with <strong>Generate All</strong>, and saves approved changes with <strong>Save All</strong>.</m-accordion><m-accordion title="No Category">Suggests Shopify taxonomy categories, shows confidence labels, and lets you apply results one by one or in bulk.</m-accordion><m-accordion title="Short Titles">Creates stronger product title suggestions with options to <strong>Suggest</strong>, <strong>Suggest All</strong>, <strong>Apply</strong>, <strong>Redo</strong>, and <strong>Save All</strong>.</m-accordion><m-accordion title="Short Description and No Description">Writes fuller product descriptions using <strong>Write</strong> and <strong>Write All</strong>, then lets you review before applying changes.</m-accordion><m-accordion title="AI Prompts">Lets you customize how titles, descriptions, alt text, and category suggestions are generated for your specific store.</m-accordion></m-accordiongroup>

## Typical workflow

<m-steps><m-step title="Review your catalog health">Open <strong>Product Health</strong> and check the summary cards and audit counts.</m-step><m-step title="Choose an issue type">Open a card such as <strong>Missing Alt Text</strong>, <strong>No Category</strong>, <strong>Short Titles</strong>, or <strong>Short Description</strong>.</m-step><m-step title="Generate suggestions">Use the row-level or bulk actions shown in the panel.</m-step><m-step title="Review before applying">Check each suggestion and use <strong>Apply</strong>, <strong>Save All</strong>, or <strong>Apply All Selected</strong> where available.</m-step><m-step title="Tune AI Prompts if needed">If suggestions are off-brand or incomplete, update the prompt rules and generate again.</m-step><m-step title="Measure progress">Return to <strong>Product Health</strong> and confirm that issue counts are dropping.</m-step></m-steps>