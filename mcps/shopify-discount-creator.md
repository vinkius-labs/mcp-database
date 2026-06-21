# Shopify Discount Creator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shopify-discount-creator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

This MCP does exactly one thing: it creates unique percentage discount codes in your Shopify store on the fly. Incredible for giving your AI agent the power to prevent cart abandonment during a chat.

## Description
We refused to build a bloated Shopify integration that requires reading your entire product catalog, modifying inventory, and accessing your customer's personal data. Instead, this MCP server provides a surgical, zero-trust bridge: **just creating discount codes.**

Your AI agent gains the immediate ability to act as a real-time sales closer. If a customer is hesitating in the chat because of the price, the agent doesn't need to ask for human approval—it instantly generates a unique 10% off code and drops it in the chat to secure the sale.

### The Superpowers

- **Real-Time Closing:** End cart abandonment friction. The AI can sense hesitation and automatically generate a custom discount code (e.g., `VIP_SAVE_15`) exactly when needed.
- **Zero-Bloat Integration:** No massive Shopify SDKs. It uses a direct `POST` to the Shopify Admin REST API. You only need a Custom App token with `write_discounts` permission.
- **Absolute Containment:** Because this is strictly a "Push-only" creation tool scoped only to discounts, the agent cannot read your orders, cannot delete products, and cannot access customer data. It only generates codes. A completely secure, one-way funnel.


## Available Tools
- **create_shopify_discount**: Provide the desired code name (e.g. VIP_10) and the percentage amount to discount (e.g. 10 for 10% off). Send the resulting code directly to the customer.

Generates a new percentage-based discount code in Shopify on the fly


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shopify Discount Creator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The customer is hesitating. Create a 15% discount code called AI_VIP_15 and give it to them."

**🤖 AI Agent:**
> I've generated the discount code AI_VIP_15. You can use it at checkout for 15% off!


## ❓ FAQ

**Q: Can the agent change the price of products with this?**
No. This MCP only accesses the endpoint to create Discount Codes. It does not have the `write_products` permission, meaning it is physically impossible for the AI to alter your catalog prices or delete products.

**Q: Does it support fixed amount discounts (e.g. $10 off)?**
To maintain maximum simplicity and safety for the AI, this specific tool is hardcoded to generate 'percentage-based' discounts applied to the entire cart. This prevents currency confusion issues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shopify-discount-creator](https://vinkius.com/mcp/shopify-discount-creator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shopify Discount Creator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `shopify-discount-creator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shopify Discount Creator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shopify-discount-creator": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
