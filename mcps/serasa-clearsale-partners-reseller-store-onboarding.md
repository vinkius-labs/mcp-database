# Serasa ClearSale Partners — Reseller Store Onboarding MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/serasa-clearsale-partners-reseller-store-onboarding)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quote, provision and deactivate ClearSale stores, and read their API credentials.

## Description
ClearSale sells through partners, and this connector automates what a reseller does by hand in the portal: read the product and segment catalogs, quote a new store, provision the entity from the accepted quote, read the API credentials the store will use, and deactivate a store when it churns. The connector keeps the onboarding order correct — the quote's transactionCode is what links the priced profile to the created entity — and renders each step as a short verdict with the ids and credentials on top, so an agent can drive a store from signup to handoff without reading the raw payloads.


## Available Tools (7)
- **create_entity_quote**: Send the store profile honestly — average ticket and monthly order volume drive the price, and misstating them skews the risk calibration later. The response answers a transactionCode only — the priced amount is shown in the ClearSale portal, not in this call.

Quote the price of onboarding a new store (entity) to ClearSale
- **create_entity**: All fields are required by ClearSale; transactionCode must be the one create_entity_quote returned. storeUrl is a list — send at least one storefront URL. On success ClearSale answers 204 with no body; the connector reports the created clientID back from your request. Follow up with get_entity_credentials to read the API credentials the store will use.

Create a new store (entity) in ClearSale from an accepted quote
- **deactivate_entity**: Use it when a store churns or is suspended. Send the clientID you created the entity with.

Deactivate a store (entity) in ClearSale
- **get_entity_credentials**: Hand these to the store — they are the credentials its integration will configure. They are sensitive: do not log or echo them beyond the destination.

Read the API credentials of a store (entity) created through the Partners API
- **list_client_products**: The ids returned here are what create_entity_quote expects as product / segment ids. Each product is a ClearSale anti-fraud product the partner can resell.

List the ClearSale products available to this partner client
- **list_products_with_segments**: Use it to choose a valid product/segment pair for create_entity_quote — sending a segment the product does not support is the usual cause of a 400.

List ClearSale products with the segments (frentes) each one supports
- **list_segments**: g. Calçados). Pick one before quoting — the segment plus the product and the store profile drives the price. Pair this with list_products_with_segments to see which segments each product accepts.

List the market segments a ClearSale entity can operate in


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Serasa ClearSale Partners — Reseller Store Onboarding** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Onboard the store Loja Exemplo, CNPJ 02.668.127/0001-09, average ticket BRL 105, about 10 orders a month. They sell shoes online."

**🤖 AI Agent:**
> Calls list_products_with_segments to pick a valid product/segment pair, then create_entity_quote with the store profile, then create_entity with the returned transactionCode, and finally get_entity_credentials to read the store's API user and password.

---

**👤 You:**
> "Store store-42 churned — deactivate it."

**🤖 AI Agent:**
> Calls deactivate_entity with client_id store-42, which ClearSale answers with an entity disabled confirmation.

---

**👤 You:**
> "What products can I resell, and which segments does each one accept?"

**🤖 AI Agent:**
> Calls list_products_with_segments, which lists each product with its accepted segment ids (frentes); list_client_products and list_segments give the flat catalogs.


## ❓ FAQ

**Q: What is the correct order to onboard a store?**
list_products_with_segments to pick a product/segment pair, then create_entity_quote, then create_entity with the returned transactionCode, then get_entity_credentials to read the keys the store configures. Skipping the quote leaves the created entity unlinked to a priced profile.

**Q: Why did the quote come back as a percentage instead of a fixed price?**
ClearSale answers with either a fixed value (priceType 1) or a percentage of the analyzed volume (priceType 2), depending on the product and the store profile you sent. The rendered quote says which one it is. Both are valid; a percentage is common for marketplace sellers.

**Q: What happens when I deactivate a store?**
The entity stops analyzing immediately. It is reversible only through ClearSale support, so use it for churn or suspension, not for testing. The clientID you deactivate is the one you set at creation time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/serasa-clearsale-partners-reseller-store-onboarding](https://vinkius.com/en/ai-agent-connect/serasa-clearsale-partners-reseller-store-onboarding)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Serasa ClearSale Partners — Reseller Store Onboarding** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `serasa-clearsale-partners-reseller-store-onboarding` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Serasa ClearSale Partners — Reseller Store Onboarding** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "serasa-clearsale-partners-reseller-store-onboarding": {
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
