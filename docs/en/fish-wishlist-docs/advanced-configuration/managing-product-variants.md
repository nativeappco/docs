---
type: page
title: Managing Product Variants
description: Fish Wishlist doesn't just save products; it saves the exact version of the product your customer wants.
seoTitle: Managing Product Variants | Fish Wishlist
seoDescription: Fish Wishlist stores data at the variant level, enabling price drop alerts, back-in-stock notifications, and accurate platform syncing.
slug: managing-product-variants
order: 1
status: published
---

Fish Wishlist stores all wishlist data at the **product variant level**, not the master product level.

* * *

## Why variants?

Storing at the variant level means:

*   **Platform sync** — variant data flows cleanly to other platforms (email tools, ERPs, analytics)
*   **Price drop alerts** — you can trigger notifications when a specific variant's price drops
*   **Back-in-stock alerts** — trigger notifications when a specific variant comes back into stock
*   **Accurate order data** — when a customer requests a quote or adds to cart, the exact variant (size, colour, etc.) is captured

* * *

## What this looks like in Shopify

In a customer's profile under **Metafields**, you'll see:

*   `fish_wishlist_user = true` — flags this customer as a Fish Wishlist user (useful for segmentation)
*   Individual wishlist metafields — each list stores an array of variant IDs

Admin teams can view and edit these metafields directly from the customer profile in Shopify Admin — useful if you want to manually curate a customer's list.

* * *

## Variant selectors on the wishlist

On the Trade plan, you can enable **variant selectors** directly on the wishlist, letting customers change their selected option (size, colour, etc.) without going back to the product page. See [B2B & Trade Features](/b2b-features) for details.