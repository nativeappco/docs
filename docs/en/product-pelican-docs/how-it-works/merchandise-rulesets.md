---
type: page
title: Merchandise Rulesets
seoTitle: Merchandise Rulesets in Product Pelican
seoDescription: Create Merchandise Rulesets in Product Pelican to sort collections automatically, promote or demote products by tag, push out-of-stock and image-less products down, and schedule re-sorts.
slug: merchandise-rulesets
order: 0
status: draft
---

## Automate collection sorting with Merchandise Rulesets

**Merchandise Rulesets** let you decide how products are ordered inside your collections, then apply that order automatically on a schedule. A ruleset combines a **sort rule**, optional **promote and demote** rules, **stock and visibility** controls, and a **schedule**, and you assign it to one or more collections.

Every ruleset you create is stored as a native Shopify **Metaobject**, so the data lives in your own store rather than locked away in an external database.

<m-info><p>Merchandise Rulesets sit in the left navigation under <strong>Product Pelican</strong> as <strong>Rulesets</strong>, alongside <strong>Products</strong>, <strong>Collections</strong>, <strong>GEO Score</strong>, <strong>Product FAQ</strong>, <strong>AI Prompts</strong>, <strong>Stitching</strong>, <strong>Settings</strong>, and <strong>Plans</strong>.</p></m-info><m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/01-rulesets-list.jpg" alt="Merchandise Rulesets list showing the Standard and All Products rulesets with schedule, collection count, and last run"></p></m-frame>

## Start on the Rulesets list

The main **Merchandise Rulesets** page lists every ruleset you have created. The banner at the top reminds you what rulesets do: they define how collections are sorted, you assign them to collections, and you can optionally schedule automatic re-sorts.

Each ruleset card shows:

*   The **ruleset name**
    
*   A **Default** badge, if it is the default ruleset
    
*   The **schedule**, such as **Every 6 hours**
    
*   The number of **collections** it is assigned to
    
*   The **Last run** time
    
*   **Edit** and **Delete** actions
    

To build a new one, click **New Ruleset** in the top right.

## Name the ruleset and choose a sort rule

Give the ruleset a clear **Ruleset name** so you can recognise it later, for example **New Products**.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/02-new-ruleset-sort.jpg" alt="New Ruleset form with Sort by set to Publish date and Direction set to Newest first"></p></m-frame>

In the **SORT** section, open **Sort by** to choose the rule that orders products in the collection. It starts on **No sort rule**. When you pick a rule such as **Publish date**, a **Direction** dropdown appears so you can set the order, for example **Newest first**.

<m-tip><p>The sort rule is the backbone of the ruleset. Promote, demote, and stock rules all adjust the order on top of this baseline, so set your sort rule first.</p></m-tip>

## Promote or demote products by tag

The **PROMOTE & DEMOTE** section starts empty with **No rules added yet**. Open **Add rule...** to add one.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/03-promote-by-tag.jpg" alt="Promote by tag rule with the value set to featured"></p></m-frame>

When you add a **Promote by tag** rule, a **PROMOTE BY TAG** block appears with a **Value** field. Start typing and Product Pelican suggests existing product tags from your store, so you can pick one such as **featured**. Products carrying that tag are lifted towards the top of the collection.

To remove a rule, use the red **✕** next to its block.

<m-note><p>The tag value matches the product tags already on your products. If a promote rule does nothing, check that the tag is spelled exactly as it appears on your products in Shopify.</p></m-note>

## Push out-of-stock and image-less products down

The **STOCK & VISIBILITY** section has two toggles that keep weaker products out of the way:

*   **Push out of stock to bottom** moves sold-out products to the end of the collection.
    
*   **Push products without images to bottom** moves products with no image to the end.
    

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/04-stock-schedule.jpg" alt="Stock and visibility toggles enabled, with the schedule set to Every 24 hours"></p></m-frame><m-tip><p>Turning both of these on is a quick win for almost any collection. Shoppers rarely want to land on a sold-out product or one with no photo, and it costs you nothing to push them down.</p></m-tip>

## Set the schedule

The **SCHEDULE** section controls how often the ruleset re-sorts its collections. Choose from:

*   **Not scheduled**
    
*   **Every 6 hours**
    
*   **Every 12 hours**
    
*   **Every 24 hours**
    

When a schedule is selected, Product Pelican confirms that the cron job applies this ruleset automatically to all assigned collections on the configured interval.

<m-note><p>Choose <strong>Not scheduled</strong> if you only want the ruleset to run when you trigger it manually. Pick an interval if your catalogue, stock levels, or tags change often and you want the order to keep itself up to date.</p></m-note>

## Assign collections

In the **COLLECTIONS** section, tick the collections this ruleset should apply to. You can search by name, and each collection shows its product count. A running **selected** count appears in the top right of the section.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/05-collections-default.jpg" alt="Collections list with All Products selected and the default ruleset checkbox ticked, showing the default change warning"></p></m-frame>

## Decide whether this is the default ruleset

The **DEFAULT** section has one checkbox: **Make this the default ruleset for new collections**. The default ruleset applies to any collection that is not assigned to a ruleset of its own.

If another ruleset is already the default, Product Pelican warns you before you save, for example **Saving will remove "Standard" as the current default**. Only one ruleset can be the default at a time.

<m-warning><p>Setting a new default reassigns every unassigned collection to this ruleset on the next run. If you only want this ruleset on a specific set of collections, leave this unchecked and assign those collections in the section above instead.</p></m-warning>

## Save the ruleset

When you are happy with the setup, click **Save Ruleset**. Product Pelican shows a **Saved** confirmation and returns you to the list, where your new ruleset now appears with its collection count.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/06-saved-list.jpg" alt="Rulesets list after saving, now showing the new New Products ruleset"></p></m-frame>

To change a ruleset later, click **Edit** on its card. The form reopens with every field pre-filled, for example **Edit: New Products**, so you can adjust the sort rule, tags, stock options, schedule, or collections and save again.

## Typical Merchandise Rulesets workflow

<m-steps><m-step title="Open Rulesets"><p>In the Shopify admin, go to <strong>Product Pelican</strong> and select <strong>Rulesets</strong>.</p></m-step><m-step title="Create a ruleset"><p>Click <strong>New Ruleset</strong> and give it a clear <strong>Ruleset name</strong>.</p></m-step><m-step title="Choose a sort rule"><p>In <strong>SORT</strong>, pick a <strong>Sort by</strong> rule and set the <strong>Direction</strong>.</p></m-step><m-step title="Add promote or demote rules"><p>Use <strong>Add rule...</strong> to promote products by tag, such as <strong>featured</strong>.</p></m-step><m-step title="Set stock and visibility"><p>Turn on <strong>Push out of stock to bottom</strong> and <strong>Push products without images to bottom</strong>.</p></m-step><m-step title="Set the schedule"><p>Choose <strong>Not scheduled</strong> or an interval such as <strong>Every 24 hours</strong>.</p></m-step><m-step title="Assign collections"><p>Tick the collections the ruleset should sort.</p></m-step><m-step title="Set the default if needed"><p>Optionally make this the default ruleset for unassigned collections.</p></m-step><m-step title="Save"><p>Click <strong>Save Ruleset</strong> and confirm the <strong>Saved</strong> message.</p></m-step></m-steps>

## Where the data is stored

Every ruleset is saved as a native Shopify **Metaobject**, written and owned by Product Pelican. You manage rulesets from inside the app, but it is worth knowing where the underlying data lives. You will find it in the Shopify admin under **Content > Metaobjects > Merchandise Ruleset**.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/07-metaobject-entries.jpg" alt="Merchandise Ruleset metaobject entries listed in the Shopify admin"></p></m-frame>

Each ruleset is a single entry. The list shows the **Display name**, the ruleset **Name**, its **Schedule**, whether it **Is Default**, the **Last Run**, who added it, and when it was updated.

Open an entry to see the stored fields: **Name**, **Rules** (the sort, promote, and demote logic stored as JSON), **Schedule**, **Is Default**, **Last Run**, and the assigned **Collections**, along with the metaobject **Handle**.

<m-frame><p><img class="tiptap-image" src="https://REPLACE-IN-EDITOR/08-metaobject-detail.jpg" alt="A Merchandise Ruleset metaobject entry showing the Name, Rules JSON, Schedule, Is Default, Last Run, and Collections fields"></p></m-frame><m-note><p>You can edit these fields directly in the Shopify admin if you ever need to, but in day-to-day use you should manage everything from the <strong>Rulesets</strong> screen in Product Pelican. The app keeps the metaobject in sync for you. This is the Native way: your data stays in your own Shopify store, in a structure you can read, export, and own.</p></m-note>

## Best practices

*   Set your **Sort by** rule first, then layer promote, demote, and stock rules on top.
    
*   Keep **tag values** consistent with the tags already on your products so promote rules actually match.
    
*   Turn on both **stock and visibility** toggles for most collections as an easy quality win.
    
*   Use **Not scheduled** for one-off sorts and an interval for collections that change often.
    
*   Only set a **default ruleset** when you genuinely want it to catch every unassigned collection.