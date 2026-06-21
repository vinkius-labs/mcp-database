# Junip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/junip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage product reviews, questions, and campaigns via Junip API.

## Description
Empower your AI agents with Junip's scalable product review platform. This MCP server allows you to list and retrieve product reviews, track customer questions and answers, manage display themes, and view review request campaigns directly through the Junip API. Ideal for automating social proof and customer feedback analysis for Shopify stores.


## Available Tools (10)
- **get_account**: Use to verify account identity and access levels.

Retrieves details about your Junip account
- **get_product**: Essential for providing a summary of a product's performance within the store.

Retrieves details for a specific product
- **get_question**: Use this before crafting an official response.

Retrieves details for a specific question
- **get_review**: Returns metadata, custom question responses, and photo/video links (if applicable). Use this when analyzing a specific customer testimonial.

Retrieves details for a specific review
- **list_answers**: Use this to audit response quality and ensure all customer queries are being addressed correctly.

Lists all answers to questions
- **list_campaigns**: Use this to analyze active efforts to collect new customer reviews and feedback.

Lists active review request campaigns
- **list_products**: Includes product names, IDs, and aggregate review metrics. Use this to identify which items have reviews.

Lists all products in your store
- **list_questions**: Returns question text, status, and associated products. Use this to find customer inquiries that require a merchant response.

Lists all customer questions
- **list_reviews**: Returns ratings, review content, and reviewer names. Use this to monitor brand sentiment and identify high-quality social proof.

Lists all product reviews
- **list_themes**: Useful for auditing the visual presentation of reviews on the storefront.

Lists all review display themes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Junip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all recent product reviews in Junip."

**🤖 AI Agent:**
> I'll fetch the latest reviews from your Junip account.

---

**👤 You:**
> "Show me the questions asked for product ID '123'."

**🤖 AI Agent:**
> I'll retrieve the customer questions associated with that specific product.

---

**👤 You:**
> "Check my active review campaigns."

**🤖 AI Agent:**
> I'll look up the list of configured review request campaigns in Junip.


## ❓ FAQ

**Q: How do I get Junip API credentials?**
Log in to your Junip admin dashboard, navigate to Settings > API, and generate a new Access Token for a Private App.

**Q: Can I see customer questions?**
Yes, you can list and retrieve customer questions and answers using the corresponding tools in this MCP.

**Q: Does it support review campaigns?**
Yes, the list_campaigns tool allows you to retrieve information about your active review request campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/junip](https://vinkius.com/mcp/junip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Junip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `junip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Junip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "junip": {
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
