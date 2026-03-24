---
type: page
title: App Configuration
description: Before you set up Fish Wishlist on your store, you should visit the Settings page and configure it to meet your needs.  You can change these settings any time.
seoTitle: App Configuration | Fish Wishlist
seoDescription: Configure Fish Wishlist settings including icons, guest wishlists, multiple lists, abandoned cart, previously purchased, wishlist sharing, marketing opt-ins, and tag actions.
slug: app-configuration
order: 1
status: published
---

Open Fish Wishlist in Shopify Admin and go to [**Settings**](https://admin.shopify.com/apps/fish-wishlist/app/settings). You can change these settings at any time.

* * *

## Wishlist Icon

Choose how the wishlist button looks on your store:

*   **Heart** — default
*   **Bookmark**
*   **Custom SVG** — upload separate icons for the empty state and added state (24 x 24px)

* * *

## Wishlist Display

*   **Layout** — show the wishlist drawer as a vertical list or a two-column grid
*   **Currency codes** — choose whether currency codes display next to prices
*   **Wishlist name** — rename "Wishlist" to anything you like (e.g. "Saved Items", "Favourites", "Requisition List"). See [Copy & Translations](/copy-and-translations) for full language options.

* * *

## Guest Wishlists

Allow customers to add items to a wishlist without logging in first.

*   **On** — customers can start saving immediately. When they log in, their wishlist data syncs to their Shopify customer account automatically.
*   **Off** — forces account creation upfront. All wishlist data goes straight into the customer's Shopify profile.

* * *

## Multiple Wishlists

Let customers create and name up to 15 wishlists each. All lists are stored as individual metafields within the customer profile in Shopify.

*   Admin teams can view and edit any customer's wishlist directly from the Shopify backend
*   All data is stored at the **product variant level** — this means it syncs cleanly with other platforms and enables features like price drop alerts and back-in-stock notifications

* * *

## Recently Purchased Products

When enabled, Fish Wishlist automatically captures products from completed orders and stores them in a dedicated wishlist slot (`wishlist_11`) on the customer's profile.

Use this to:

*   Surface a "Buy Again" section on your homepage or account page using the [Wishlist Page Section](/wishlist-section-on-any-page)
*   Trigger re-purchase email campaigns via Shopify Flow

* * *

## Abandoned Cart

When a customer abandons their cart, Fish Wishlist uses a Shopify webhook to capture those products and store them in a dedicated wishlist slot — automatically.

Use this to:

*   Show abandoned products in the wishlist drawer when the customer returns
*   Surface them on a dedicated recovery page using the [Wishlist Page Section](/wishlist-section-on-any-page)

* * *

## Wishlist Sharing

Allow customers to generate a shareable link to their wishlist. Shared wishlists are stored as **Shopify Metaobjects**, meaning you can view and edit them directly from Shopify Admin under **Content > Metaobjects**.

*   Customers must be signed in to share
*   Use this for gift registries, or create curated influencer/celebrity wishlists by editing the metaobject in Shopify admin

See [Wishlist Sharing](/wishlist-sharing) for full setup details.

* * *

## Integrations

Enable one-click integrations directly from the settings page:

*   **GA4** — wishlist events flow into Google Analytics 4 automatically
*   **Meta** — wishlist add/remove events sent to Meta for retargeting and audience building

For Klaviyo and other email platforms, see [Email Marketing via Shopify Flow](/shopify-flow-email-marketing).

* * *

## Marketing Opt-ins

Display email and/or SMS marketing opt-in checkboxes on the wishlist. Useful if you're using the wishlist as part of an account creation or sign-up flow — you capture consent at exactly the right moment.

* * *

## Tag Actions

Tag Actions let you control how specific wishlist elements behave based on product tags — without touching your theme code.

See [Tag Actions](/tag-actions) for full documentation.

* * *

## CSS Selectors

Use CSS selectors to define where wishlist icons are automatically injected on your site. Most useful for header icon placement. See [Header Button](/header-button) for details.

* * *

## Button Classes

Tell Fish Wishlist to use your theme's existing button CSS classes instead of its own default styles — keeps everything on-brand without stylesheet conflicts.

* * *

## Custom CSS Editor

Add minor CSS overrides directly in the app. Useful for small tweaks specific to the wishlist without modifying your theme files.