---
type: page
title: Tag Actions
seoTitle: Tag Actions | Fish Wishlist
seoDescription: Use Tag Actions to control wishlist behaviour per product tag — rename buttons, hide prices, suppress social proof widgets, and run custom JavaScript.
slug: tag-actions
order: 9
status: published
---

# Tag Actions

Tag Actions let you change how specific wishlist elements behave based on product tags — without touching your theme code. It's one of the most flexible and underused features in Fish Wishlist.

* * *

## How to access

Go to **Fish Wishlist > Settings > Tag Actions** and click **Add Action**.

* * *

## How it works

Each tag action has two parts:

1.  **The target** — which element you're modifying (e.g. the Add to Cart button)
2.  **The condition** — a product tag that triggers the behaviour, or a wildcard `*` to apply to all products

* * *

## Available actions

### Add to Cart Button

Modify the Add to Cart button that appears next to each item on the wishlist.

Option

What it does

Rename label

Change the button text — e.g. show "Pre-order" instead of "Add to Cart" on pre-order tagged products

Disable button

Button is visible but non-clickable

Hide button

Button is not shown at all

Redirect after click

Send the customer to a URL after clicking (e.g. back to the product page)

Run JavaScript

Execute custom JS after the cart action — useful for custom cart properties or triggering other site events

### Social Proof Widget

Hide the social proof widget on specific products.

**Example:** Tag coming soon products with `coming-soon` and hide the widget so you're not showing a wishlist count on products customers can't buy yet.

### Wishlist Item — Hide Price

Hide the price on wishlist items.

*   Set a specific tag to hide price on certain products
*   Use the wildcard `*` to hide all prices across the entire wishlist — useful for stores that don't display prices publicly

* * *

## Using wildcards

Instead of a product tag, enter `*` in the tag field to apply the action to **all products** on the wishlist. Useful for store-wide rules like hiding all prices.

* * *

## Examples

Goal

Action type

Tag

Setting

Show "Pre-order" on pre-order items

Add to Cart Button

`pre-order`

Rename label → "Pre-order"

Hide button on sold-out items

Add to Cart Button

`sold-out`

Hide button

Hide social proof on new arrivals

Social Proof Widget

`coming-soon`

Hide widget

Hide all prices site-wide

Wishlist Item

`*`

Hide price

* * *

## Adding custom actions

Most of the tag actions in Fish Wishlist came from customer requests. If you need a behaviour that isn't listed here, [contact support](mailto:support@nativeappco.com) — we can usually add it.