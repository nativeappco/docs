---
type: page
title: Edit FAQs in Shopify metaobjects
description: Learn how to open Product Pelican FAQs in Shopify’s native Metaobjects editor, edit an FAQ entry, and update the Product FAQs assigned to a product.
seoTitle: Edit product FAQs in Shopify metaobjects
seoDescription: Access Product Pelican FAQs in Shopify's native Metaobjects editor, update FAQ entries, and change which questions are assigned to a product.
slug: edit-faqs-in-shopify-metaobjects
order: 0
status: draft
---

## Manage Product Pelican FAQs inside Shopify

Product Pelican is still the best place to manage your FAQs day to day. The **Product FAQ** screen is faster, more tailored, and easier to work with when you are adding, reordering, reusing, and reviewing FAQs across products.

<m-note>This guide shows the alternative workflow in <strong>Shopify admin</strong> using Shopify's native <strong>Metaobjects</strong> and product <strong>metafields</strong>. It is useful if you specifically want to work in Shopify's built-in editor.</m-note>

This page follows the same order as the screencast walkthrough: first you open the FAQ entries in **Content** → **Metaobjects**, then you edit an individual **FAQ Item**, and finally you update the **Product FAQs** assigned to a product.

## Before you start

*   Product Pelican must already be installed and set up in your store.
*   Your FAQs should already exist as Product Pelican entries inside Shopify.
*   You should be comfortable editing products in Shopify admin.

<m-tip>If your goal is to manage FAQs efficiently, use the <strong>Product FAQ</strong> screen in Product Pelican instead. Use this Shopify-native flow when you specifically want to work directly with Shopify metaobjects and metafields.</m-tip>

## Open the Product Pelican FAQ definitions

<m-steps><m-step title="Go to Shopify Metaobjects"><p>In Shopify admin, open <strong>Content</strong> → <strong>Metaobjects</strong>. In the definitions list, you will see Product Pelican's entries, including <strong>Product FAQ</strong> and <strong>FAQ Item</strong>.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2c76f287-9e5b-4d78-ae46-38a044857426/frame_001.jpg" alt="Shopify Metaobjects page showing Product FAQ and FAQ Item definitions added by Product Pelican"></m-frame><p><strong>FAQ Item</strong> is where the individual question-and-answer entries live. <strong>Product FAQ</strong> is the definition used for the product FAQ setup created by Product Pelican.</p></m-step><m-step title="Open the FAQ Item entries list"><p>Click <strong>FAQ Item</strong> to open the list of saved FAQ entries. This screen shows all available questions in Shopify's native Metaobjects editor.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/09378695-5488-488a-8fd3-bea9306e867e/frame_002.jpg" alt="FAQ Item entries list in Shopify showing available FAQ questions"></m-frame><p>Use the <strong>Question</strong> column to find the entry you want to update.</p></m-step></m-steps>

## Edit an existing FAQ entry

<m-steps><m-step title="Open the FAQ item you want to change"><p>From the <strong>FAQ Item</strong> list, click the entry you want to edit. The entry editor shows the two main fields used by Product Pelican:</p><ul><li><strong>Question</strong></li><li><strong>Answer</strong></li></ul><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/9e3d4ada-8628-43f9-bfaf-b7fc8001629a/frame_003.jpg" alt="Shopify FAQ Item editor showing Question and Answer fields"></m-frame></m-step><m-step title="Update the answer or question"><p>Edit the text in the <strong>Question</strong> or <strong>Answer</strong> field as needed. In the walkthrough, the answer is expanded with more detail and then saved.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/d4bb5ca5-4f24-4c98-b8ff-2d38894c4d57/frame_004.jpg" alt="Updated FAQ Item entry after saving changes in Shopify"></m-frame></m-step><m-step title="Confirm the entry was updated"><p>Return to the <strong>FAQ Item</strong> list and check the <strong>Updated</strong> column. The edited entry should show a fresh timestamp such as <strong>Just now</strong>, confirming that your change has been saved.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/b30cfad3-a4f5-4322-95b4-b3da6de457b2/frame_005.jpg" alt="FAQ Item list showing a recently updated timestamp after editing an entry"></m-frame></m-step></m-steps><m-info>Because Product Pelican stores FAQs as Shopify metaobjects, editing an <strong>FAQ Item</strong> here changes the underlying FAQ entry used by the app.</m-info>

## Change which FAQs are assigned to a product

After updating an FAQ entry, you can also change which FAQs are attached to a specific product using the product's **Product FAQs** metafield.

<m-steps><m-step title="Open the product in Shopify admin"><p>Go to <strong>Products</strong> and open the product you want to update. Scroll down to the <strong>Product metafields</strong> area.</p><p>In the walkthrough, the product page shows a <strong>Product FAQs</strong> field before expanding the full metafields view.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/71dcd4e8-cffd-45b0-ba40-46ce2a7e60bd/frame_006.jpg" alt="Shopify product page showing the Product FAQs metafield before opening all metafields"></m-frame></m-step><m-step title="Open the full metafields view if needed"><p>If the full list is not already visible, open <strong>View all</strong> in the product metafields area. In the expanded view, Shopify shows the selected FAQ entries inside the <strong>Product FAQs</strong> metafield as metaobject references.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/2436d17b-86ef-4a54-a1d0-332df4c277fb/frame_007.jpg" alt="Expanded Shopify product metafields view showing Product FAQs assigned to the product"></m-frame></m-step><m-step title="Open the Product FAQs selector"><p>Click into the <strong>Product FAQs</strong> field to open the selector. Shopify displays the available <strong>FAQ Item</strong> entries, with checkboxes for the questions currently assigned to the product.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/3bdbb3aa-d218-4c59-b865-d1c90a8c2025/frame_008.jpg" alt="Product FAQs selector in Shopify showing checked FAQ items assigned to a product"></m-frame><p>From here, you can:</p><ul><li>Check a question to assign it to the product</li><li>Uncheck a question to remove it from the product</li><li>Review the currently selected entries in the field</li></ul></m-step><m-step title="Save the product changes"><p>Once the right FAQs are selected, save the product. After saving, the <strong>Product FAQs</strong> metafield will show the updated set of assigned entries.</p><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/video-frames/3daeff0b-3c57-495a-8d8e-f953d60b5388/frame_009.jpg" alt="Shopify product metafields view showing the updated Product FAQs assigned to the product"></m-frame></m-step></m-steps>

## What this workflow is good for

*   Making a quick wording change to an existing FAQ in Shopify admin
*   Checking which FAQ entries Product Pelican created in **Metaobjects**
*   Changing the set of FAQ items attached to a single product through **Product FAQs**

## When to use Product Pelican instead

The Shopify-native route works, but Product Pelican is still the recommended place to manage FAQs at scale.

*   The **Product FAQ** screen is faster for editing multiple products
*   You can use **Add FAQ**, **Connect existing**, **Suggest FAQs**, and **Import FAQs** in one place
*   It is easier to review, reuse, and organize FAQs without switching between Shopify screens

<m-tip>For routine FAQ work, start in <a href="/set-up-product-faqs">Set up Product FAQs</a>. If you just want to review FAQs from a product page in Shopify admin, see <a href="/view-product-faqs-in-shopify-admin">View product FAQs in Shopify admin</a>.</m-tip>

## Quick recap

1.  Go to **Content** → **Metaobjects**.
2.  Open **FAQ Item**.
3.  Edit the **Question** or **Answer** for the FAQ entry you want to change.
4.  Confirm the updated timestamp in the entries list.
5.  Open the product in **Products**.
6.  Use the **Product FAQs** metafield to add or remove assigned FAQ items.
7.  Save the product.