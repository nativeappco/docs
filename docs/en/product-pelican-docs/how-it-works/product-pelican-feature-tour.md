---
type: page
title: Product Pelican feature tour
description: A guided walkthrough of Product Pelican’s main screens and workflows, including Product Health, GEO Score, audit fixes, bulk AI actions, and AI Prompts.
seoTitle: Product Pelican feature tour demo
seoDescription: See every major Product Pelican feature in one walkthrough, from Product Health audits and GEO Score to AI Prompts and bulk fixes.
slug: product-pelican-feature-tour
order: 0
status: draft
---

## What this walkthrough covers

This page follows the same flow as the Product Pelican screencast, so you can see how the app is typically used from first review through to bulk fixes and prompt customization.

In Product Pelican, the main workspace is **Product Health**. This is where you review your catalog, open individual audit checks, generate AI suggestions, and apply improvements without working through products one by one in Shopify.

<m-info>Product Pelican combines catalog audits with action buttons such as <strong>Generate All</strong>, <strong>Suggest All</strong>, <strong>Write All</strong>, <strong>Apply</strong>, <strong>Save All</strong>, and <strong>Redo</strong> so you can fix issues in place.</m-info><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/40a9f110-2179-4cca-91fc-e0ec5f73348f/frame_001.jpg" alt="Product Health dashboard showing summary cards and audit checks"></m-frame>

## Start on Product Health

When you open the app, Product Pelican lands on **Product Health** and shows the **Product Data Quality Dashboard**. At the top of the page you can review the store-wide totals for:

*   **Active Products**
*   **Total Variants**
*   **Products with Issues**
*   **Clean Products**

Below those totals, the dashboard is split into two tabs:

*   **Audit Checks**
*   **GEO Score**

The **Audit Checks** tab shows the full set of issue cards visible in the app:

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

<m-tip>Start with the highest-count cards first. Those usually give you the biggest catalog improvement in the shortest time.</m-tip>

## Review products by GEO Score

The **GEO Score** tab gives you a product-level scoring view instead of an issue-count summary. Products are grouped into score bands so you can quickly focus on listings that need the most work.

In the walkthrough, the tab shows band filters including **All**, **Poor**, **Needs work**, **Solid**, and **AI-ready**. The table also includes columns such as **Product**, **Score**, and **Band**, plus score chips for individual content areas.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2922c975-3ce1-45a8-aea9-7650ae39f038/frame_002.jpg" alt="GEO Score tab showing products grouped by score band"></m-frame>

Use this view when you want to sort and prioritize products by overall quality, not just by one specific audit.

## Fix image issues

### No Images

Opening the **No Images** card expands a product list directly below the dashboard. In the walkthrough, each affected product has an upload area in the **Add Images** column with an **Add files** button.

This makes it possible to work through missing product media from one screen instead of opening each product separately in Shopify.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/b3def2c0-3706-4a26-b06c-ed23edd08b5b/frame_003.jpg" alt="No Images panel showing products with Add files upload areas"></m-frame>

### Missing Alt Text

The **Missing Alt Text** workflow is one of the most detailed screens in the app. When you open it, Product Pelican shows image cards with:

*   The product name
*   The image filename
*   A status such as **No alt text**
*   A suggested alt text field
*   A visible character count
*   Action buttons including **Generate Alt Text**, **Apply**, **Regen**, and **Copy**

At the top of the section, you can switch between **Missing / Poor** and **All Images**. For bulk work, use **Generate All** and then **Save All**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5a0455fc-7287-4c40-bd01-8584a9343286/frame_004.jpg" alt="Missing Alt Text panel with image cards and generated suggestions"></m-frame><m-steps><m-step title="Open the audit">Select <strong>Missing Alt Text</strong> from the <strong>Audit Checks</strong> grid.</m-step><m-step title="Generate suggestions">Use <strong>Generate Alt Text</strong> on one image or <strong>Generate All</strong> for the visible list.</m-step><m-step title="Review the wording">Check the suggested text and edit it if needed before saving.</m-step><m-step title="Save your updates">Use <strong>Apply</strong> for one image or <strong>Save All</strong> to commit multiple reviewed changes.</m-step></m-steps>

## Fill missing Shopify categories

The **No Category** audit checks whether the Shopify category field has been populated. When expanded, the screen shows a table with **Product**, **Suggested Category**, and **Actions**.

You can run **Suggest All** to generate recommendations for the whole list, or use **Suggest** row by row.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/87f921d0-ae86-404b-8082-2dd8c406da69/frame_005.jpg" alt="No Category panel with Suggest All and category suggestion actions"></m-frame>

After suggestions are generated, Product Pelican shows the proposed taxonomy path and a confidence label such as **Low** or **High**. Once you accept a recommendation, the row updates to show that the category has been **Applied**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/bf300cdb-7ab6-4d2e-8431-7f491515b259/frame_006.jpg" alt="No Category results showing suggested taxonomy paths and applied statuses"></m-frame><m-note>This workflow is especially useful if your products were imported from CSVs or another system and the Shopify taxonomy field was left blank.</m-note>

## Improve short product titles

The **Short Titles** audit highlights titles that are too brief to be descriptive. Each row shows the current product, the issue text such as **Title is only 19 chars**, a **Suggested Title**, and action buttons.

Depending on the row state, you may see **Suggest**, **Apply**, or **Redo**. For bulk generation, use **Suggest All**, then save accepted changes with **Save All**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/11ab7091-f150-433e-9183-1112e0c1e711/frame_007.jpg" alt="Short Titles panel with AI-generated title suggestions and apply buttons"></m-frame>

One useful detail shown in the walkthrough is that you are not locked into the AI output. If a suggestion is close but not right, you can edit the title before applying it.

Later in the screencast, the presenter returns to **Short Titles** after changing the title prompt. The refreshed suggestions list shows how prompt edits affect future results, with the same row-level actions still available: **Apply** and **Redo**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/0bcda9b8-9bda-4a67-8ec2-9ed4c2659b4c/frame_013.jpg" alt="Short Titles suggestions list showing Apply and Redo actions after prompt changes"></m-frame>

## Write longer product descriptions

The **Short Description** and **No Description** checks help you improve product copy in bulk. In the walkthrough, the **Short Description** panel shows each affected product, the current issue text, a **Suggested Description** area, and actions.

Use **Write All** to generate descriptions in bulk, then **Save All** once you have reviewed the results. Individual rows can also use **Write**, **Apply**, and **Redo**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/85fa3afa-86f8-44a9-abbc-eeb8890074f9/frame_008.jpg" alt="Short Description panel showing generated description suggestions and bulk actions"></m-frame>

This is useful when descriptions are missing entirely or are present but too short to explain the product clearly.

## See updated counts after changes

After applying fixes, Product Pelican returns you to the main dashboard so you can see how the audit counts have changed. In the walkthrough, several counts drop after updates are made, which gives you a quick way to confirm progress.

You may also see a banner such as **Load full catalogue** with text like **Showing 200 most recently updated products**, depending on the current dashboard state.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5bfeab38-529c-4847-b974-188d3d97ba04/frame_009.jpg" alt="Refreshed Product Health dashboard showing revised audit counts"></m-frame>

## Customize the AI Prompts

In the left navigation, Product Pelican includes an **AI Prompts** page directly under **Product Health**. This is where you control how future AI suggestions are written.

The page includes editable prompt sections for:

*   **Title Prompt**
*   **Description Prompt**
*   **Alt Text Prompt**
*   **Category Prompt**

There is also a **Reset All to Defaults** button at the top of the page.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/189d9510-b14c-496c-bd07-415d25ef74fe/frame_010.jpg" alt="AI Prompts page with editable prompt sections"></m-frame>

### Title Prompt

The walkthrough zooms in on **Title Prompt**, which is labeled **Used when generating product title suggestions**. The prompt includes store rules such as title style, product detail usage, and formatting requirements.

This is where you can change how Product Pelican builds new title suggestions. For example, the screencast shows the impact of a rule that tells the AI to mention a vendor, and then demonstrates how removing or changing that rule affects the next round of generated titles.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2014fa9a-7c04-4d0b-9b2a-70fa404c66c7/frame_011.jpg" alt="Close-up of the Title Prompt editor with detailed title rules"></m-frame>

### Prompt edits create unsaved changes

When you edit any of the prompt fields, Product Pelican shows an **Unsaved changes** banner across the top of the page with **Discard** and **Save** actions.

This makes it clear when your prompt instructions have been changed but not yet committed.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/fa3007cd-26c2-46e0-81fb-5d659c455f2e/frame_015.jpg" alt="AI Prompts page showing an Unsaved changes banner with Discard and Save buttons"></m-frame>

### Alt Text Prompt and Category Prompt

The lower part of the **AI Prompts** page includes **Alt Text Prompt** and **Category Prompt**. These sections let you tune how alt text is written and how Shopify taxonomy suggestions are selected.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/8ff828ad-2b63-47a5-8fd0-f29a01fe4a1b/frame_016.jpg" alt="AI Prompts page close-up showing Alt Text Prompt and Category Prompt sections"></m-frame><m-tip>If your store has very specific brand rules, shipping language, category restrictions, or formatting requirements, add them to the relevant prompt before generating a large batch of suggestions.</m-tip><m-warning>Prompt changes only affect future generations. If you want the new rules to appear in titles, descriptions, alt text, or categories, return to the audit and generate new suggestions after saving.</m-warning>

## Other audits on the dashboard

The walkthrough focuses most heavily on images, categories, titles, descriptions, and prompts, but the dashboard also includes checks for:

*   **Ambiguous Language**
*   **Unclear Options**
*   **Missing SKUs**
*   **Zero Price Variants**
*   **Vague Titles**
*   **No Description**

Together, these checks make Product Pelican a single place to review content quality, merchandising completeness, and missing product data.

## The typical Product Pelican workflow

<m-steps><m-step title="Review overall catalog health">Open <strong>Product Health</strong> and look at the totals and audit counts on the <strong>Product Data Quality Dashboard</strong>.</m-step><m-step title="Prioritize by issue or score">Choose either <strong>Audit Checks</strong> for a specific problem type or <strong>GEO Score</strong> for an overall quality view.</m-step><m-step title="Generate improvements">Use the relevant bulk or row-level action, such as <strong>Generate All</strong>, <strong>Suggest All</strong>, <strong>Write All</strong>, <strong>Suggest</strong>, or <strong>Write</strong>.</m-step><m-step title="Review and apply">Check the generated result, edit it if needed, and then use <strong>Apply</strong> or <strong>Save All</strong>.</m-step><m-step title="Refine future output">Go to <strong>AI Prompts</strong>, update the instructions, click <strong>Save</strong>, and regenerate suggestions where needed.</m-step></m-steps>

## Why merchants use Product Pelican

Product Pelican is built to help you review your product data, make improvements in bulk, and use AI suggestions without losing control over the final result. Instead of working product by product in several different Shopify screens, you can move from one audit to the next, apply changes directly, and then adjust the AI prompts when you want more tailored output.