# Chargebee MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargebee)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate recurring billing via Chargebee — manage subscriptions, customers, invoices, and hosted checkouts natively with any AI agent.

## Description
Connect your **Chargebee** environment to any AI agent and take absolute control of your SaaS revenue operations by simply chatting. Bypass massive spreadsheets and complex financial dashboards.

### What you can do

- **Customers** — List existing accounts, retrieve specific financial details (outstanding balances), or create brand new B2B accounts instantly
- **Subscriptions** — Inspect active, trailing, or cancelled plans. Pause renewals, trace MRR, or irreversibly cancel subscriptions mid-term
- **Invoices** — Retrieve active billing logs and check if a payment gateway approved or declined a specific charge
- **Checkout & Catalog** — Enumerate product lines and generate ephemeral, secure Hosted Checkout URLs to capture customer cards on the fly

### How it works

1. Subscribe to this server
2. Provide your Chargebee Site ID and API Key
3. Start managing your revenue pipelines natively via Claude, Cursor, or any MCP-compatible platform

### Who is this for?

- **Support agents** — easily verify if a user's subscription is paused, cancelled, or in trial without opening the billing platform
- **Sales teams** — generate an instant, exact checkout URL for a specific product plan while still talking to the prospect
- **Founders & Ops** — ask your agent to pull a list of recent failed invoices or immediately pause a delinquent account


## Available Tools (10)
- **cancel_subscription**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **create_customer**: Provision a highly-available JSON Payload generating hard Customer records
- **generate_hosted_checkout**: Dispatch an automated validation check routing explicit Payment UI
- **get_customer_details**: Perform structural extraction of properties driving active Account logic
- **get_subscription_details**: Inspect deep internal arrays mitigating specific Plan Math
- **list_customers**: Identify bounded CRM records inside the Headless Chargebee Platform
- **list_invoices**: Enumerate explicitly attached structured rules exporting active Billing
- **list_catalog_items**: Retrieve the exact structural matching verifying Product mapping
- **list_subscriptions**: Retrieve explicit Cloud logging tracing explicit Recurring limits
- **pause_subscription**: Identify precise active arrays spanning native Pause tracking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chargebee** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new customer profile for John Doe at john@acme.com."

**🤖 AI Agent:**
> Customer 'John Doe' (john@acme.com) successfully provisioned into your Chargebee vault! The new Customer ID generated is 'cust_9AxYv23L'. Do you wish to generate a hosted checkout URL for them?

---

**👤 You:**
> "Cancel subscription sub_4001, but wait until the end of the term."

**🤖 AI Agent:**
> Executed! Subscription `sub_4001` has received the irreversible boolean 'end_of_term' cancellation switch. Service remains active precisely until the current billing period expires, avoiding prorated refunds.

---

**👤 You:**
> "Review my invoices and point out any recent declines."

**🤖 AI Agent:**
> I iterated through your active billing ledger. I found 1 out of the 10 recent limits flagged as 'Payment Declined'. It belongs to customer 'cust_0102'. The gateway declined their card due to insufficient funds. Should I pause their software subscription?


## ❓ FAQ

**Q: Can my AI automatically detect a declining card and cancel the recurring subscription?**
Yes. Ask the agent to pull the most recent invoices and find the specific declined charges. Once identified, command the agent to cancel the associated subscription ID completely, putting an end to the service. All done natively through chat.

**Q: How does the Hosted Checkout generation work?**
When asked, the AI fetches your catalog items, finds the needed Plan ID, and hits the `generate_hosted_checkout` endpoint. It replies instantly with an ephemeral, safe URL you can copy-paste to your customer, capturing their payment securely before destroying the link lifespan.

**Q: Can I halt billing charges for a specific timeframe?**
Certainly. The `pause_subscription` command instructs Chargebee to freeze active charges and renewals on the provided subscription ID until you deliberately tell the AI to resume it later. Brilliant for seasonal B2B accounts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargebee](https://vinkius.com/mcp/chargebee)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chargebee** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chargebee` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chargebee** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chargebee": {
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
