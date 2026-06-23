# LeadDyno MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leaddyno)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Empower your AI to process LeadDyno affiliate links, manage program members, and track generated commission sales instantly.

## Description
Combine **LeadDyno** affiliate logic with your everyday AI tools. Automatically monitor external influencers sharing your links, verify accurate commission ledgers, and list brand ambassadors globally.

### What you can do

- **Affiliate Management:** Check individual partner links and status logs.
- **Sales Pipelines:** Search registered new commissions scaling inside LeadDyno.
- **Visitor Metrics:** Quantify engagement of links to verify brand partner impact.

### How it works

1. Install this MCP Server base
2. Fill out your LeadDyno personal API token
3. Engage your virtual assistant locally via Claude/Cursor

### Who is this for?

- **Performance Marketers** — trace links individually
- **Marketing Analysts** — audit the overall platform commissions in the background
- **Brand Executives** — compile specific influencer performance without dashboards


## Available Tools (9)
- **create_affiliate**: Create a new affiliate in LeadDyno
- **create_lead**: Record a new lead in LeadDyno
- **create_purchase**: Record a new purchase in LeadDyno
- **get_affiliate**: Retrieve details for a specific affiliate
- **list_affiliates**: Retrieve a list of affiliates from LeadDyno
- **list_commissions**: Retrieve a list of commissions
- **list_leads**: Retrieve a list of all tracked leads
- **list_purchases**: Retrieve a list of all tracked purchases
- **list_visitors**: Retrieve a list of website visitors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LeadDyno** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List overall active brand affiliates signed in the program."

**🤖 AI Agent:**
> Pulling affiliates securely... I observed 5 new marketers integrated into LeadDyno with confirmed track links active tonight.

---

**👤 You:**
> "Retrieve the total daily generated commissions for this week."

**🤖 AI Agent:**
> Scanning ledger... There have been 12 logged conversion clicks representing 3 closed sales this week so far.

---

**👤 You:**
> "Which influencers brought in the most lead visitors today?"

**🤖 AI Agent:**
> I matched visitor history to their referral identifiers. Affiliate A holds highest traffic directly pulling 89 unique URL clicks.


## ❓ FAQ

**Q: How do I authenticate?**
Use the standard Private Key you generate under settings directly within LeadDyno dashboard and place it below.

**Q: Can I process affiliate payouts through the tool?**
For security reasons, this agent isolates data tracking and metric retrievals only, handling read requests rather than disbursing cash.

**Q: How fast are clicks attributed?**
The tool retrieves clicks exactly as recorded live on your platform engine's internal cache natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leaddyno](https://vinkius.com/mcp/leaddyno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LeadDyno** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leaddyno` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LeadDyno** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leaddyno": {
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
