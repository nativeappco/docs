---
type: page
title: Manual price history tag
description: Learn how to manually place the Omnibus Owl price history tag on product and collection pages using your Shopify theme code or a custom Liquid block.
seoTitle: Manual price history tag for Shopify
seoDescription: Add the Omnibus Owl price history tag to any Shopify product or collection page using theme code or a Liquid block.
slug: manual-price-history-tag
order: 0
status: draft
---

## Manual price history tag

If you want to show the Omnibus Owl price history message somewhere other than the standard product block placement, you can manually add the tag to your Shopify theme.

This is useful when you want to show the lowest price message on collection pages, custom product cards, featured product sections, or anywhere else in your storefront layout.

<m-note>You should already have Omnibus Owl installed and your theme setup completed. If you have not enabled the app yet, start with <a href="/theme-installation">Theme Installation</a>.</m-note>

## What this tag does

Omnibus Owl provides a custom HTML element that loads the price history message for a specific product and variant:

    <omnibus-lowest-price data-product-id="10453038334288" data-variant-id="52866454126928"></omnibus-lowest-price>

When this tag is rendered on your storefront, Omnibus Owl replaces it with the correct lowest-price text and amount for that product variant.

## Before you start

*   Make sure the **Omnibus app embed** is turned on in the **Shopify Theme Editor**.
*   Make sure you are editing the correct theme, especially if you have both a live theme and a draft theme.
*   You need access to the product ID and variant ID for the item you want to show.

<m-tip>If the widget text needs to match your brand voice, update it in the app on the <strong>Languages</strong> page. You can change the <strong>Main Label</strong>, tooltip text, and date format there. See <a href="/language-settings">Language Settings</a>.</m-tip>

## Add the tag in your theme code

Use this method if you want to place the tag directly inside a Liquid template, snippet, or section.

<m-steps><m-step title="Open your Shopify theme code"><p>In Shopify admin, go to <strong>Online Store</strong> &gt; <strong>Themes</strong>. Find the theme you want to edit, click <strong>...</strong>, then click <strong>Edit code</strong>.</p></m-step><m-step title="Find the file that renders the product or card"><p>Open the file where you want the price history message to appear. On collection pages, this is usually the product card snippet or product grid item. On product pages, it may be the main product section or product information snippet.</p></m-step><m-step title="Paste the Omnibus Owl tag"><p>Add the tag where you want the message to appear:</p><pre><code>&lt;omnibus-lowest-price data-product-id="{{ product.id }}" data-variant-id="{{ product.selected_or_first_available_variant.id }}"&gt;&lt;/omnibus-lowest-price&gt;</code></pre><p>If you are inside a product card on a collection page, your theme may use a different product variable such as <code>card_product</code> or <code>item</code>. In that case, use that variable instead.</p></m-step><m-step title="Save and test the storefront"><p>Click <strong>Save</strong>, then preview the theme. Visit a product page or collection page where you added the tag and confirm the price history message appears.</p></m-step></m-steps>

## Add the tag in a Custom Liquid block

Use this method if your theme supports a **Custom Liquid** block in the Shopify Theme Editor.

<m-steps><m-step title="Open the Shopify Theme Editor"><p>In Shopify admin, go to <strong>Online Store</strong> &gt; <strong>Themes</strong>, then click <strong>Customize</strong> on the theme you want to edit.</p></m-step><m-step title="Open the template or section"><p>Navigate to the template where you want the message to appear. This could be a product template, featured product section, or another area of your storefront that supports Liquid blocks.</p></m-step><m-step title="Add a Custom Liquid block"><p>Click <strong>Add block</strong> and choose <strong>Custom Liquid</strong>.</p></m-step><m-step title="Paste the tag"><p>Paste this code into the block:</p><pre><code>&lt;omnibus-lowest-price data-product-id="{{ product.id }}" data-variant-id="{{ product.selected_or_first_available_variant.id }}"&gt;&lt;/omnibus-lowest-price&gt;</code></pre></m-step><m-step title="Save and preview"><p>Click <strong>Save</strong>, then preview the storefront to make sure the widget appears in the right place.</p></m-step></m-steps>

## Collection page example

If you want to show the lowest price message inside each product card on a collection page, place the tag inside the snippet or section that renders each card.

A common pattern looks like this:

    <omnibus-lowest-price data-product-id="{{ card_product.id }}" data-variant-id="{{ card_product.selected_or_first_available_variant.id }}"></omnibus-lowest-price>

The exact Liquid variable depends on your theme. Some themes use `product`, others use names like `card_product`, `collection_product`, or `item`.

<m-warning>The tag must receive a real product ID and variant ID for the product being rendered. If the wrong variable is used, the price history message will not load correctly.</m-warning>

## How to find the right product and variant values

In most cases, you should use Liquid variables from the theme instead of hardcoded IDs. That keeps the tag dynamic so it works for every product on the page.

If you want to test with a single hardcoded product first, you can use this format:

    <omnibus-lowest-price data-product-id="10453038334288" data-variant-id="52866454126928"></omnibus-lowest-price>

Replace those numbers with your own product ID and variant ID.

## When the widget appears

By default, Omnibus Owl only shows the price history on products that are actively on sale. If you do not see anything on the storefront, the app may be working as expected.

You can review your app behavior and tracked products from the **Dashboard**, including product search and price history timelines. See [Dashboard Screen](/dashboard-screen).

<m-info>Omnibus Owl tracks price changes from the time the app is installed. It cannot show price history from before installation.</m-info>

## Troubleshooting

### The tag shows nothing

*   Check that the **Omnibus app embed** is enabled.
*   Confirm the product is currently on sale if your store is using the default display behavior.
*   Check that the product ID and variant ID are being passed correctly.
*   Make sure you saved the theme and are previewing the same theme you edited.

### The message appears on the wrong product

*   Your collection card may be using a different Liquid variable than `product`.
*   Update the code to use the variable used by that snippet, such as `card_product`.

### The text needs to be changed

*   Open the app and go to the **Languages** page.
*   Edit the **Main Label** or tooltip text.

## Related pages

<m-cardgroup><m-card title="Theme Installation" href="/theme-installation">Enable the app embed and install the standard storefront widget.</m-card><m-card title="Language Settings" href="/language-settings">Customize the widget label, tooltip text, and translations.</m-card><m-card title="Dashboard Screen" href="/dashboard-screen">Review tracked products and inspect individual price history timelines.</m-card></m-cardgroup>