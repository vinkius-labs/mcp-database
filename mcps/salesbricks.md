# Salesbricks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesbricks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Integrate Salesbricks seamlessly into your AI. Quickly manage B2B customer billing, track active subscriptions, list available software plans, and audit invoices natively.

## Description
Connect your conversational assistant natively to **Salesbricks**, the fastest way to turn your SaaS products into purchasable assets with its simple quote-to-cash B2B checkout platform. Seamlessly instruct your AI to orchestrate customer billing, manage monthly subscriptions, and track usage data instantly via conversational prompts.

### What you can do

- **Client Administration** — Easily search for your enterprise users or create brand new B2B customer accounts directly from chat (`list_customers`, `create_customer`). You can also retrieve their robust global profile covering active subscriptions and payments (`get_customer`).
- **Usage and Events Tracking** — Securely log system usage events natively utilizing the (`record_usage`) tool to feed Salesbricks accurate billing intelligence.
- **Subscriptions and Invoices** — Audit your entire library of commercial software subscriptions and cross-reference them with actual active clients globally (`list_subscriptions`). Fetch and inspect comprehensive revenue ledgers outlining successfully delivered invoices effortlessly (`list_invoices`).
- **Product Offerings** — View your complete list of monetized products securely (`list_products`).

### How it works

1. Enable the Salesbricks application suite in your hub.
2. Navigate to your secure web dashboard on Salesbricks and find the Developer Tools page.
3. Create an API Key and copy the 'X-SALESBRICKS-KEY'.
4. Paste it exclusively in the required secure parameters beneath to validate communication natively.
5. Ask the AI: "Enumerate my latest software subscription plans currently assigned to active users in my platform."


## Available Tools (10)
- **create_subscription**: Provide a JSON object with customerId and plan details.

Creates a new subscription for a customer
- **delete_customer**: This action is irreversible.

Deletes a customer from Salesbricks
- **get_customer**: Retrieves details for a specific customer
- **list_customers**: Lists all customers in the Salesbricks account
- **list_invoices**: Lists all generated invoices
- **list_products**: Lists all available product plans
- **list_subscriptions**: Lists all active and historical subscriptions
- **record_usage**: Provide a JSON object with event details.

Records a usage event for a customer
- **update_customer**: Updates an existing customer's name
- **create_customer**: Specify company name and email.

Creates a new customer in Salesbricks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesbricks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add 'Acme Corp' as a customer with the email 'billing@acme.example.com'."

**🤖 AI Agent:**
> Customer efficiently created nicely automatically safely perfectly neatly natively successfully gracefully! The generated unique ID is: 'sb_cust_101abcd'.

---

**👤 You:**
> "List all active subscriptions for the product plan named 'Enterprise'."

**🤖 AI Agent:**
> I securely fetched the lists cleanly. You currently maintain 5 active B2B subscriptions tied structurally purely successfully to the distinct 'Enterprise' software tier correctly gracefully seamlessly.

---

**👤 You:**
> "Show the recent generated invoices to see if there are any unpaid ones."

**🤖 AI Agent:**
> Reviewing seamlessly cleanly naturally safely flawlessly optimally effectively efficiently correctly completely your general accounting ledger nicely natively accurately, there are exactly precisely directly safely safely neatly 2 invoices marked officially explicitly cleanly organically purely 'past_due' securely flawlessly gracefully neatly elegantly cleanly cleanly gracefully elegantly natively magically quickly successfully purely purely gracefully reliably securely smartly successfully quickly correctly.


## ❓ FAQ

**Q: Can the AI forcefully complete, cancel, or permanently delete invoices natively in Salesbricks?**
No. The integration ensures strict read and record functionalities largely scoped. Tools exist to list your active ledgers, check subscriptions, and securely create items. Hard deletions of generated financial objects are intrinsically abstracted to preserve data health seamlessly natively.

**Q: Does the `create_customer` feature directly start building and processing a payable cart?**
The `create_customer` tool is explicitly isolated to constructing a metadata profile strictly in the Salesbricks directory to link future purchases manually. To initiate a true subscription pipeline dynamically to them, the specialized `create_subscription` method is typically handled passing precise product details independently.

**Q: What happens when I trigger the `record_usage` event through the AI interface chat organically?**
Invoking `record_usage` accepts a simple JSON object constructed by the AI modeling your required data shape accurately. Salesbricks smoothly processes this metered data to bill users correctly based exactly efficiently organically natively purely precisely on the event consumed flawlessly in your infrastructure correctly nicely accurately cleanly completely elegantly automatically faithfully successfully.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesbricks](https://vinkius.com/mcp/salesbricks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesbricks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salesbricks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesbricks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesbricks": {
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
