---
type: page
title: Product Stitching
description: Create regex-based Product Stitching rules in Product Pelican to automatically link related products by SKU or title, preview matches, sync results, and review logs.
seoTitle: Product Stitching in Product Pelican
seoDescription: Learn how to create Product Stitching rules in Product Pelican using regex to link colour variants, complementary products, and sets.
slug: product-stitching
order: 0
status: draft
---

## Automate related product links with Product Stitching

**Product Stitching** lets you automatically group related products and write those relationships into a product metafield. You can use it for alternate colour options, complementary products, and merchandising experiences like **Pair it With** or **Complete the set**.

In Product Pelican, stitching rules match products using either **SKU** or **Title**. Matching is driven by a **Regex pattern**, which extracts a shared value from each product so matching items can be grouped together.

<m-info>Product Stitching sits in the left navigation under <strong>Product Pelican</strong> as <strong>Stitching</strong>, alongside <strong>Dashboard</strong>, <strong>Product FAQ</strong>, <strong>AI Prompts</strong>, <strong>Settings</strong>, and <strong>Plans</strong>.</m-info><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/5e399cd8-a697-4bf5-a9d9-8712d250aa81/frame_001.jpg" alt="Product Stitching dashboard showing active rules, totals, search, and existing stitching rules"></m-frame>

## Start on the Product Stitching dashboard

The main **Product Stitching** page gives you a quick view of how your rules are performing. At the top of the screen, the dashboard shows:

*   **Active Rules**
*   **Total Groups**
*   **Products Stitched**
*   **Last Sync**

Below the totals, you can filter the list using **All**, **Active**, and **Paused**, and narrow the list with **Search rules**.

Each rule card shows the rule name, its status such as **Active**, the match source such as **SKU**, the regex pattern, the target metafield, the group and stitched counts, whether **Auto-sync** is enabled, and a **Sync** action for running the rule.

In the walkthrough, the dashboard includes rules like **Pair it With** and **Related Products- matched by SKU**.

<m-tip>If you plan to build several stitching rules, start by deciding which product relationship each target metafield should power. For example, keep alternate colours, complementary products, and set-building rules separate so each one writes to the right storefront field.</m-tip>

## Open a rule to review how it works

Select a rule to open its detail page. The walkthrough opens **Pair it With**, which shows the full setup and sync tools for that rule.

The rule page is split into clear sections:

*   **RULE** for the current setup
*   **STATS** for stitched counts and sync timing
*   **GROUPS** for the matched product groups
*   **DRY RUN** for testing the rule before writing metafields
*   **RECENT ACTIVITY** for the latest events

At the top-right of the page, the available actions are **Delete**, **Pause**, **Edit rule**, and **Bulk sync**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/0db0266f-2ea5-4e46-a379-f08905c019ec/frame_002.jpg" alt="Pair it With rule page showing rule setup, stats, dry run, and recent activity"></m-frame>

### What the rule page shows

In the **RULE** section, Product Pelican displays:

*   **Match type**, such as **SKU** or **Regex on SKU**
*   **Pattern**
*   **Target metafield**
*   **Auto-sync on publish**

The **STATS** panel shows values such as:

*   **Products stitched**
*   **Groups**
*   **Avg group size**
*   **Last sync**

The **DRY RUN** panel includes **Run preview**, which lets you test changes against the catalogue without writing metafields yet.

<m-note>Use <strong>Run preview</strong> before a live sync whenever you change the regex pattern or swap the target metafield. It is the safest way to confirm which products will be grouped.</m-note>

## Edit the rule settings

From the rule detail page, click **Edit rule** to update how the rule matches products and where it writes the result.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/a3953c61-35d6-4494-a5c5-e3c06fa984f0/frame_003.jpg" alt="Edit rule screen showing rule name, match options, regex pattern, and target metafield settings"></m-frame>

The edit screen includes two main sections: **RULE DETAILS** and **TARGET**.

### Rule Details

In **RULE DETAILS**, you can set:

*   **Rule name**
*   **Match against**
*   **Regex pattern**

For **Match against**, the walkthrough shows these options:

*   **SKU**
*   **Title**
*   **Tag** _soon_

When matching by SKU, Product Pelican tests each product's primary variant SKU against your regex. When matching by title, it uses the product title instead.

Next to **Regex pattern**, there is a **Suggest with AI** button. The screen also validates the pattern and shows confirmation such as **Valid regex - capture group detected**.

<m-warning>Your regex must include a capture group. Product Pelican uses the captured value as the group key, and products with the same key are stitched together.</m-warning>

### Target

In the **TARGET** section, use the **Metafield** dropdown to choose where the stitched product list should be written. The walkthrough shows targets including custom metafields and Shopify product recommendation metafields.

You can also enable **Auto-sync on product publish** so the rule reruns when a product is published or updated.

## Choosing a regex pattern

The right regex depends on how your catalogue is structured. A good pattern removes the part of the SKU or title that changes between related products and keeps the part they share.

Common examples include:

*   Removing a colour name from product titles so different colour variants group together
*   Matching products using the number that appears before the first hyphen in the SKU
*   Extracting a shared style code from the start of the SKU

<m-tip>If you need help writing a regex, use an AI tool such as Gemini or ChatGPT and describe exactly what you want. For example: <code>remove the colour name from my product titles using regex</code> or <code>match products using the number that appears before the first hyphen in the SKU</code>.</m-tip>

## Save the updated rule

After choosing the correct target metafield and confirming the regex, click **Save changes**.

The walkthrough shows the rule being updated from a custom target to a Shopify recommendations target, then saved using **Save changes** at the bottom of the page.

If you do not want to keep the edits, use **Cancel**.

## Preview and sync the rule

Once the rule is saved, return to the rule detail page and test it. Product Pelican supports both a preview and a live sync:

*   **Run preview** in the **DRY RUN** panel to see what the rule would produce
*   **Bulk sync** to write the stitched relationships to the selected metafield

When a sync is queued, the page can show a status banner such as **Bulk sync pending**, explaining that the cron picks up pending runs every minute.

## Review the sync results

After the sync completes, the rule page updates with live stats and the generated groups.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/d266ce74-85e0-4f53-9bd2-e434b55c03e9/frame_005.jpg" alt="Rule detail page showing stitched products, groups created, and recent sync activity"></m-frame>

In the walkthrough, the updated rule page shows:

*   **Products stitched**
*   **Groups**
*   **Avg group size**
*   **Last sync**

The **GROUPS** section expands to show the matched group key and the products inside that group. This is where you confirm that the expected products were stitched together.

The **DRY RUN** panel also summarizes the last scan, including counts such as scanned products, groups created, and unmatched products.

On the right side, **RECENT ACTIVITY** logs important milestones such as **Bulk sync complete**, **Group synced**, and **Rule updated**.

<m-note>If the group looks too broad or too narrow, go back to <strong>Edit rule</strong>, adjust the <strong>Regex pattern</strong>, run another preview, and sync again.</m-note>

## Check the rule logs

For a fuller event history, open the logs view for the rule. In the walkthrough, the page title is **Logs: Pair it With**.

<m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/54bcb6c9-36e8-4e10-a16f-ae406285a332/frame_006.jpg" alt="Logs page for a Product Stitching rule showing sync and update events"></m-frame>

The logs table includes these columns:

*   **TIME**
*   **ACTION**
*   **GROUP**
*   **PRODUCTS**
*   **DETAIL**

Typical events include:

*   **Sync complete**
*   **Group synced**
*   **Rule updated**
*   **Sync started**
*   **Rule created**

Use this screen to confirm what happened during a run, when it happened, and how many products were affected.

## Typical Product Stitching workflow

<m-steps><m-step title="Open Stitching"><p>In the Shopify admin, go to <strong>Product Pelican</strong> and select <strong>Stitching</strong>.</p></m-step><m-step title="Review existing rules"><p>Use the <strong>Product Stitching</strong> dashboard to check <strong>Active Rules</strong>, <strong>Total Groups</strong>, <strong>Products Stitched</strong>, and <strong>Last Sync</strong>.</p></m-step><m-step title="Open or create a rule"><p>Select an existing rule such as <strong>Pair it With</strong>, or click <strong>New rule</strong> to create a new one.</p></m-step><m-step title="Choose what to match"><p>Set <strong>Match against</strong> to <strong>SKU</strong> or <strong>Title</strong>, then enter a <strong>Regex pattern</strong> with a capture group.</p></m-step><m-step title="Choose the destination metafield"><p>In <strong>TARGET</strong>, pick the <strong>Metafield</strong> that should store the stitched product list.</p></m-step><m-step title="Preview before writing"><p>Use <strong>Run preview</strong> in <strong>DRY RUN</strong> to confirm the groups the rule will create.</p></m-step><m-step title="Save and sync"><p>Click <strong>Save changes</strong>, then run <strong>Bulk sync</strong> or <strong>Sync</strong> to write the relationships.</p></m-step><m-step title="Review results and logs"><p>Check <strong>STATS</strong>, inspect the <strong>GROUPS</strong> section, and review the <strong>Logs</strong> page for the full event history.</p></m-step></m-steps>

## Best practices for cleaner matches

*   Use **SKU** matching when your catalogue has consistent SKU structure.
*   Use **Title** matching when titles are more reliable than SKUs.
*   Keep one rule focused on one relationship type, such as alternate colours or complementary products.
*   Always test with **Run preview** before a live sync after changing the pattern.
*   Review unmatched product counts after a dry run to spot gaps in your regex.

<m-warning>If you point a rule at the wrong target metafield, the stitched relationships may show in the wrong storefront feature. Double-check the <strong>Metafield</strong> before saving.</m-warning>