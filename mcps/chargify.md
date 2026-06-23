# Chargify MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chargify)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Automate recurring billing via Chargify (Maxio) — manage subscriptions, customers, plans, and revenue holds directly via AI agents.

## Description
Connect your **Chargify (Maxio)** site to any AI agent and take absolute control of your SaaS revenue operations by simply chatting. Bypass massive spreadsheets, complex API docs, and tedious financial dashboards.

### What you can do

- **Customers** — Query your B2B accounts, retrieve specific financial details, or formulate brand new CRM customer records instantly
- **Subscriptions** — Inspect active and canceled states, trace billing cycles, past-due flags, or irreversibly cancel subscriptions documenting specific churn reasons
- **Planes & Upgrades** — Browse your active product catalog and seamlessly upgrade or modify a customer's plan mid-cycle with a single command
- **Holds & Resumes** — Place an absolute freeze/hold on a subscription forbidding next billing, and resume it seamlessly when ready

### How it works

1. Subscribe to this server
2. Provide your unique Chargify Subdomain and API Key
3. Start commanding your billing platform natively via Claude, Cursor, or any MCP client

### Who is this for?

- **Support agents** — easily verify if a user's subscription is locked or suspended, and resume it without leaving your Helpdesk workflow
- **Sales teams** — effortlessly upgrade a client to a new Enterprise tier with one text command 
- **Ops & Founders** — ask your agent to parse the product catalog or apply a mass cancellation to a delinquent account immediately


## Available Tools (10)
- **cancel_subscription**: Irreversibly vaporize explicit validations extracting rich Churn flags
- **create_customer**: json` tracking exact Name and Email strings tied to the B2B engine.

Provision a highly-available JSON Payload generating hard Customer bindings
- **get_customer_details**: json` checking exactly what references exist per SaaS consumer.

Perform structural extraction of properties driving active Account logic
- **get_subscription_details**: json` tracking exact billing cycle, MRR, and past-due flags.

Inspect deep internal arrays mitigating specific Plan Math
- **hold_subscription**: json` clamping the subscription entirely forbidding next billing until cleared.

Identify precise active arrays spanning native Pause tracking
- **list_customers**: json` mapping exact user email arrays inside a Chargify site.

Identify bounded CRM records inside the Headless Chargify/Maxio Platform
- **list_catalog_products**: json` grabbing precisely the valid handles needed to trigger a plan switch.

Retrieve the exact structural matching verifying Product mapping
- **list_subscriptions**: json` dropping exact state strings resolving whether active or canceled.

Retrieve explicit Cloud logging tracing explicit Recurring limits
- **resume_subscription**: json` ripping a Hold state unlocking MRR engine immediately.

Dispatch an automated validation check routing explicit Resume logic
- **update_subscription_product**: Identify precise active arrays spanning native Plan tracking/Upgrades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chargify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We promised Acme Corp a grace period. Put a hold on subscription 4040 immediately."

**🤖 AI Agent:**
> Hold placed effectively. Subscription `4040` matches the Acme bounds and is now in a clamped state. No further billing will process until you instruct me to actively resume it.

---

**👤 You:**
> "List our product catalog. I need to know the IDs to upgrade an account."

**🤖 AI Agent:**
> Here is the active product catalog. We mapped 3 product tiers:
- Basic Plan (ID: 101)
- Pro Plan (ID: 102)
- Enterprise (ID: 103)
Would you like me to update a customer's subscription to one of these IDs?

---

**👤 You:**
> "Customer sub_899 just requested cancellation via email. Reason: 'budget cuts'. Please process it."

**🤖 AI Agent:**
> Subscription `sub_899` stands irreversibly canceled. I mapped 'budget cuts' internally as the churn tracking reason for your financial analysts. The billing stream is officially terminated.


## ❓ FAQ

**Q: How can I pause billing for a client who needs a break?**
Just tell your agent to 'Place a hold on subscription ID `123`'. It hits the `/holds.json` endpoint, clamping the account and completely forbidding the next billing cycle from firing until you choose to resume it.

**Q: Can my agent upgrade a customer to a higher pricing tier instantly?**
Absolutely. You can ask for a list of products to find the new Plan ID, then prompt the agent to update the subscription target. The platform handles the mid-cycle prorations automatically while your agent executes the switch.

**Q: What happens when I cancel a subscription through the AI?**
When you execute a cancellation, you can include a 'message' documenting the churn logic (e.g., 'Moving to competitor'). The AI executes an irreversible DELETE call stopping the MRR securely and appending your specific reason for analytics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chargify](https://vinkius.com/mcp/chargify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chargify** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `chargify` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chargify** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chargify": {
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
