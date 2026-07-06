# Gumroad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gumroad)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate e-commerce via Gumroad — manage products, sales, and license verification directly from any AI agent.

## Description
Connect your **Gumroad** creator account to any AI agent and take full control of your digital store and sales data through natural conversation.

### What you can do

- **Product Management** — List all products in your store, retrieve detailed descriptions, and check pricing information.
- **Sales Monitoring** — Access your sales history, inspect individual transactions, and track revenue growth.
- **License Verification** — Instantly verify license keys for software, courses, or digital assets directly from the chat.
- **Refund Handling** — Process refunds for specific sales efficiently without manual dashboard navigation.
- **Subscriber Insights** — Retrieve your subscriber lists to better understand your audience and growth.
- **Payout Tracking** — Monitor your payout history and account balances seamlessly.

### How it works

1. Subscribe to this server
2. Enter your Gumroad Access Token
3. Start managing your e-commerce store from Claude, Cursor, or any MCP-compatible client

No more manual exporting of CSVs or jumping between store tabs. Your AI assistant acts as a dedicated store manager or operations specialist.

### Who is this for?

- **Digital Creators** — instantly retrieve product performance and verify student/customer licenses.
- **E-commerce Managers** — automate the process of handling refund requests and monitoring daily sales.
- **Customer Support Agents** — quickly check transaction details and license statuses during customer interactions.


## Available Tools (10)
- **list_payers**: List customers who have purchased from you
- **list_payouts**: List your Gumroad payouts history
- **list_products**: List all products in your Gumroad account
- **list_sales**: List all sales/transactions
- **list_subscribers**: List all subscribers to your products or newsletters
- **refund_sale**: Refund a specific sale
- **verify_license**: Verify a license key for a specific product
- **get_my_profile**: Get information about your Gumroad user profile
- **get_product**: Get detailed information about a specific product
- **get_sale**: Get detailed information about a specific sale


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gumroad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products in my Gumroad store."

**🤖 AI Agent:**
> I've retrieved your products. You have 5 active items: 'Mastering AI' ($49.00), 'DevOps Toolkit' ($29.00), 'Python Course' ($99.00), and 2 more. Which one would you like to see more details for?

---

**👤 You:**
> "Show me the sales history for the last 24 hours."

**🤖 AI Agent:**
> Fetching recent transactions... You've had 12 sales in the last 24 hours, totaling $588.00 in gross revenue. The most recent purchase was 'Mastering AI' by customer@example.com. Should I list all individual transactions?

---

**👤 You:**
> "Verify license key ABC-123 for the DevOps Toolkit."

**🤖 AI Agent:**
> Checking license key... The key ABC-123 for 'DevOps Toolkit' is VALID. It has been used 1 time out of a maximum of 3 allowed activations. The customer email is buyer@example.com.


## ❓ FAQ

**Q: How do I get my Gumroad Access Token?**
Log in to your Gumroad account, navigate to **Settings > Advanced**, and scroll down to the 'Application' section to create an application or generate a personal access token.

**Q: Can I verify customer license keys through this integration?**
Yes! Use the `verify_license` tool by providing the `product_id` and the `license_key` provided by the customer. The agent will confirm if the key is valid and how many times it has been used.

**Q: Does this integration support processing refunds?**
Yes, you can use the `refund_sale` tool with a specific sale ID to initiate a refund directly from your AI agent.

**Q: Is my sales data secure?**
Absolutely. The integration uses OAuth 2.0 Bearer tokens and communicates only with Gumroad's official API over HTTPS. Your token is encrypted and stored securely in the Vinkius Cloud.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gumroad](https://vinkius.com/mcp/gumroad)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gumroad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gumroad` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gumroad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gumroad": {
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
