# RevenueCat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/revenuecat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Run your in-app subscription infrastructure from your AI agent — look up RevenueCat customers, grant and revoke entitlements, and manage subscriptions, offerings, products and discounts.

## Description
Connect **RevenueCat** to your AI agent to operate your in-app purchase and subscription infrastructure directly through the RevenueCat REST API v2. No more context-switching to the dashboard for support tickets and lifecycle actions.

### What you can do

- **Customer lookup** — find a customer by email or id with `rc_list_customers` / `rc_get_customer`, and read their attributes with `rc_set_customer_attributes`.
- **Access decisions** — grant or revoke a promotional entitlement (`rc_grant_entitlement`, `rc_revoke_granted_entitlement`) to hand out trials, win-backs or make-goods, and move purchases between accounts with `rc_transfer_customer`.
- **Subscription lifecycle** — read, extend, cancel and refund subscriptions, and pull a signed store management URL when a store plan must be handled in the store itself.
- **Catalog & configuration** — inspect entitlements, offerings, products and discounts, and attach or detach products from entitlements so purchases grant the right access.

### How it works

1. Subscribe to this server
2. Enter your **V2 secret API key** and **project ID**
3. Ask in natural language — "customer john@example.com, is pro still active?" — and the agent routes to the right tool

### Who is this for?

- **App founders** — answer subscription support questions without leaving the chat.
- **Revenue engineers** — grant trials and extend periods without touching the dashboard.
- **Support teams** — look up a customer's access state and act on it in one flow.


## Available Tools (31)
- **rc_attach_products_to_entitlement**: When a customer owns any attached product, they hold the entitlement. Use rc_list_products to find product ids. This is a configuration change that affects live access for new purchases — confirm scope before running.

Attach one or more products to an entitlement so that purchasing them grants it
- **rc_cancel_subscription**: Apple and Google Play cancellations must happen in the store (or via the store API / management URL), and this call will reject them. Cancel means the subscription stops renewing at the end of the current period; it does not refund. Use rc_refund_subscription for refunds.

Cancel an active Web Billing (RevenueCat-managed) subscription
- **rc_create_customer**: Attributes are reserved (e.g. $email) or custom names, at most 50. If the customer already exists the call creates nothing new — RevenueCat treats customer ids as stable identities.

Create a customer with a given id, optionally seeding attributes
- **rc_create_entitlement**: Attach products to it afterwards with rc_attach_products_to_entitlement so purchases of those products grant the entitlement.

Create a new entitlement in the project
- **rc_detach_products_from_entitlement**: After detaching, new purchases of those products no longer grant the entitlement (existing grants keep their own expiry). Confirm before running — this can revoke access for customers buying those products.

Detach one or more products from an entitlement
- **rc_extend_subscription**: Provide either extend_by_days (Apple caps this at 90 days) or extend_until_ms (an absolute epoch-ms target after the current period end). For Apple Store subscriptions, extend_reason_code is required (one of: undeclared, customer_satisfaction, other, service_issue_or_outage). Works for store and web billing subscriptions.

Extend the current billing period of a subscription, by a number of days or to an absolute date
- **rc_get_customer**: Pass expand="attributes" to include custom/reserved attributes like $email. Use rc_list_customers to find a customer by email or search term when you only know those.

Get one RevenueCat customer (subscriber) by id, with their attributes when expanded
- **rc_get_discount**: It shows the discount type, amount, duration mode and eligibility, so you can verify a coupon a customer tried to use actually exists and is enabled. Its codes are a separate sub-resource in the API.

Get one discount by id, including its discount codes
- **rc_get_entitlement**: Entitlement ids look like entla1b2c3d4e5; the lookup_key (e.g. "pro") is what your app code references.

Get one entitlement by id, optionally with its attached products
- **rc_get_offering**: Pass expand="package,package.product" to see the packages and products the offering exposes.

Get one offering by id, optionally with its packages and products
- **rc_get_product**: The store_identifier (e.g. the App Store sku "com.app.monthly") is what store listings show. Pass expand="app,indicative_price" for richer detail.

Get one product by its RevenueCat product id
- **rc_get_purchase**: Shows status, revenue, quantity, store and product. Use rc_search_purchases when you only have the store-side identifier.

Get one one-time purchase by its RevenueCat purchase id
- **rc_get_subscription**: Pass expand="redemption" to include the most recent redemption-link info when the subscription was redeemed from a link. Use rc_search_subscriptions when you only have the store-side identifier.

Get one subscription by its RevenueCat subscription id
- **rc_grant_entitlement**: expires_at is milliseconds since epoch and must be in the future. If another promotional grant for the same entitlement expires within two hours of this value, RevenueCat ignores the request as a duplicate. Use it to hand out trials, win-backs or support make-goods.

Grant an entitlement to a customer until a given time — the classic trial or promotional grant
- **rc_list_apps**: ) and an app id used to scope product lookups.

List the apps in the configured RevenueCat project (App Store, Play Store, web billing, etc.)
- **rc_list_customers**: Use it when the user gives you an email instead of a customer id. limit is clamped to 1..100 by the API.

Search customers in the project, by email or free-text, with pagination
- **rc_list_discounts**: Use this to see which discounts exist so you can reason about a coupon a customer expected. Discount codes live under a discount and are listed separately by the API.

List the discounts (promo offers / coupons) defined in the project
- **rc_list_entitlements**: g. "pro"). Use this to find the entitlement ids used by rc_grant_entitlement / rc_revoke_granted_entitlement. Pass expand="items.product" to see which products grant each entitlement.

List the entitlements defined in the project, optionally with their products
- **rc_list_offerings**: Use this to find offering ids for rc_assign_offering. Pass expand="items.package,items.package.product" to see which products each offering bundles.

List the offerings in the project, optionally with their packages and products
- **rc_list_products**: Filter by app_id to look at one app. Pass expand="items.app" or "items.indicative_price" to enrich each product with its app or a USD/US indicative price.

List products in the project, optionally scoped to one app and with price/app expansion
- **rc_list_projects**: If you are unsure which project ID to configure, call this first and pick the right one from the result.

List the projects visible to this API key. Useful to find the project ID to use as the REVENUECAT_PROJECT_ID credential
- **rc_refund_purchase**: Store-purchased items are refunded through the store, not here. This is a money-moving operation — confirm with the user before calling it.

Refund a one-time Web Billing (RevenueCat-managed) purchase
- **rc_refund_subscription**: Apple and Google Play refunds go through the store, not this endpoint. This is a money-moving operation — confirm with the user before calling it.

Refund an active Web Billing (RevenueCat-managed) subscription
- **rc_restore_purchase_by_order_id**: The order id looks like GPA.1234-5678-9012-34567. This is Google Play only — Apple receipts are restored through the SDK or app store, not this endpoint.

Restore a Google Play purchase to a customer by its order id
- **rc_revoke_granted_entitlement**: Only promotional grants can be revoked — store-purchased entitlements are managed by the store. If the customer holds a store purchase that also grants the same entitlement, revoking the grant does not remove access.

Revoke a promotional entitlement grant from a customer
- **rc_search_purchases**: This is what receipts and support tickets usually carry. Pass expand="items.redemption" to include redemption-link details.

Find one-time purchases by their store purchase identifier
- **rc_search_subscriptions**: This is usually what support tickets carry, rather than the RevenueCat subscription id. include_scheduled=true also returns subscriptions scheduled to start in the future.

Find subscriptions by their store subscription identifier (e.g. an Apple transaction id)
- **rc_set_customer_attributes**: g. $email, $displayName, $pushToken). Custom attribute names must not start with $. Pass a null value to delete an attribute. Up to 50 attributes per call.

Set (or delete, with a null value) a customer's attributes
- **rc_subscription_management_url**: The URL is short-lived — hand it to the customer promptly. Use rc_cancel_subscription / rc_refund_subscription only for web billing subscriptions.

Get a signed URL that takes the customer to the store management page for a subscription
- **rc_transfer_customer**: g. signed in with a different email on the same store account). Optionally scope the transfer to specific app ids. This is a support operation — confirm intent before running it, because the original customer loses access to the transferred purchases.

Transfer a customer's subscriptions and one-time purchases to another customer
- **rc_assign_offering**: Pass an offering id to assign it, or leave offering_id empty to clear the override (the API accepts null). Use rc_list_offerings to find offering ids.

Assign an offering override to a customer, or clear the current override


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RevenueCat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is the customer with email john@example.com still active on Pro?"

**🤖 AI Agent:**
> Found one matching customer. Their entitlements show Pro is currently active and renews automatically. If you want, I can pull their full subscription record or grant an extension.

---

**👤 You:**
> "Grant the pro entitlement to customer 19b8de26 for 14 days as a win-back."

**🤖 AI Agent:**
> Granted. The pro entitlement is now active for that customer for 14 days from now. Note: if they already hold a store purchase of pro, access continues from the store on its own terms.

---

**👤 You:**
> "Extend this web subscription by 14 days for customer satisfaction."

**🤖 AI Agent:**
> Extended the current billing period by 14 days with reason customer_satisfaction. The next charge is now pushed out by two weeks.


## ❓ FAQ

**Q: Which API key type do I need?**
A **V2 secret key**. Create it in your project's Settings > API keys > + New, pick version V2 and the permissions you need. v1 keys do not work against the v2 API, so create a fresh v2 key if you only have v1 ones.

**Q: Do I need more than the API key?**
Yes — the project ID too. It scopes every call. Find it in your dashboard URL (app.revenuecat.com/projects/<id>) or call `rc_list_projects` to see which projects your key can see and copy the right one.

**Q: Can it cancel or refund an Apple or Google Play subscription?**
Only for web-billing (RevenueCat-managed) subscriptions. For store plans, use `rc_subscription_management_url` to hand the customer a signed link to the store's own management flow, or the store API. Cancel/refund tools are explicitly limited to `rc_billing`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/revenuecat](https://vinkius.com/en/ai-agent-connect/revenuecat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RevenueCat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `revenuecat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RevenueCat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "revenuecat": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
