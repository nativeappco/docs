---
type: page
title: Create Store Credit Automation Using Shopify Flow
description: Create a Shopify Flow workflow that automatically issues store credit using Stork Credit’s “Add Store Credit” action—based on any trigger or condition you choose.
seoTitle: Shopify Flow store credit automation (Stork Credit)
seoDescription: Use Shopify Flow triggers to automatically issue store credit with Stork Credit. Add the “Add Store Credit” action and configure amount, currency, and expiry.
slug: create-store-credit-automation-using-shopify-flow
order: 0
status: draft
---

## Overview

Stork Credit includes a Shopify Flow connector that lets you issue store credit automatically from any Shopify Flow workflow. You can use Shopify Flow’s native triggers (like **Customer created** or **Order paid**) or triggers from other apps, then add the Stork Credit action **Add Store Credit** to issue credit.

<m-note>All setup happens in <strong>Shopify Flow</strong>. Stork Credit provides the <strong>Add Store Credit</strong> action that you add to your workflow.</m-note>

## Before you start

*   Install **Stork Credit** on your Shopify store.
*   Install **Shopify Flow** (Shopify Flow is available on supported Shopify plans).
*   Make sure your workflow has access to a customer email (for example, via `{{customer.email}}`).

## Create a workflow that issues store credit

<m-steps><m-step title="Open Shopify Flow and create a workflow"><p>In your Shopify admin, open <strong>Apps</strong> → <strong>Shopify Flow</strong>, then create a new workflow (or open an existing one you want to edit).</p></m-step><m-step title="Choose a trigger"><p>Select a trigger that matches the behavior you want to reward (for example, <strong>Customer created</strong>, <strong>Order paid</strong>, or a trigger from another installed app).</p><m-tip>If you only want to issue credit for certain cases, add a <strong>Condition</strong> step (for example, check whether the customer accepts marketing).</m-tip></m-step><m-step title="Add the Stork Credit action"><p>Click <strong>+ Add action</strong>, then select <strong>Stork Credit</strong> and choose <strong>Add Store Credit</strong>.</p><p>In the action panel, you’ll configure these fields:</p><ul><li><strong>Email</strong> — the customer’s email address (for example <code>{{customer.email}}</code>).</li><li><strong>Amount</strong> — the store credit amount to add.</li><li><strong>Currency</strong> — the currency of the store credit. If left blank, it defaults to your store’s main currency.</li><li><strong>Expires on</strong> — optional expiry date in <code>YYYY-MM-DD</code> format. Leave blank if the store credit should never expire.</li></ul></m-step><m-step title="Apply and turn on the workflow"><p>When you’re done, click <strong>Apply changes</strong> in Shopify Flow. Then switch the workflow from <strong>Draft</strong> to <strong>On</strong> (depending on your Flow UI) so it starts running.</p></m-step></m-steps><m-frame><img src="https://cdn.heymantle.com/orgs/26a47f7d-a3b9-42a0-97fc-a4835cc43fbe/docs-pages/0ab11742-a66a-457b-8358-b85c572c302f/stork-credit-shopify_flow_example.png" alt="Shopify Flow workflow showing the Stork Credit action 'Add Store Credit' with fields Email, Amount, Currency, and Expires on"></m-frame>

## Common automation examples

<m-accordiongroup><m-accordion title="Issue credit when a new customer signs up"><p>Use the <strong>Customer created</strong> trigger, then add <strong>Add Store Credit</strong> with:</p><ul><li><strong>Email</strong>: <code>{{customer.email}}</code></li><li><strong>Amount</strong>: a fixed welcome credit (for example <code>10</code>)</li><li><strong>Expires on</strong>: optionally set an expiry date to encourage a first purchase</li></ul></m-accordion><m-accordion title="Issue credit only when a condition is met"><p>Add a <strong>Condition</strong> step before <strong>Add Store Credit</strong> (for example, a condition that checks whether the customer accepts marketing). Connect the <strong>True</strong> branch to <strong>Add Store Credit</strong> so only qualifying customers receive credit.</p></m-accordion><m-accordion title="Issue different credit amounts based on behavior"><p>Use multiple <strong>Condition</strong> steps (or branches) in Flow, and add separate <strong>Add Store Credit</strong> actions on each branch with different <strong>Amount</strong> values.</p></m-accordion></m-accordiongroup>

## Troubleshooting

*   **No credit issued:** Confirm the workflow is turned on (not in **Draft**) and that you clicked **Apply changes**.
*   **Wrong customer credited:** Double-check the **Email** field uses the correct variable for your trigger (for example, `{{customer.email}}` for customer-based triggers).
*   **Unexpected currency:** Set the **Currency** field explicitly if you don’t want to rely on your store’s default currency.

<m-warning>Shopify Flow workflows can run many times. If your trigger can fire repeatedly for the same customer, add conditions (or other safeguards) to avoid issuing credit more than intended.</m-warning>