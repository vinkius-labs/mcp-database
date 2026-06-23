# PartnerStack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/partnerstack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage affiliate and partner programs via PartnerStack — list partners, track leads, and monitor rewards directly from any AI agent.

## Description
Connect your **PartnerStack** account to any AI agent and take full control of your partnership and ecosystem workflows through natural conversation.

### What you can do

- **Partner Oversight** — List all partners and retrieve detailed metadata to manage your ecosystem relationships.
- **Lead Tracking** — List and retrieve details for leads submitted by your partners to monitor the sales pipeline.
- **Customer Management** — List customers associated with specific partners to understand attribution.
- **Reward Monitoring** — List generated rewards and payouts to ensure your partners are incentivized correctly.
- **Campaign & Group Analysis** — List partner groups and campaigns to maintain a clear view of your program structure.

### How it works

1. Subscribe to this server
2. Enter your PartnerStack API Key
3. Start managing your partnership program directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Partnership Managers** — quickly check the status of a specific partner or review recent leads.
- **Channel Operations** — monitor rewards and payouts while auditing program performance.
- **Sales Teams** — lookup customer attribution and partner metadata without leaving your workflow.


## Available Tools (10)
- **get_partner_customer**: Get details for a specific customer
- **get_partner**: Get details for a specific partner
- **list_partner_campaigns**: List all partner campaigns
- **list_partner_customers**: List all customers associated with partners
- **list_partner_groups**: List all partner groups
- **list_partner_leads**: List all leads submitted by partners
- **list_partners**: List all partners
- **list_partner_rewards**: List all generated rewards
- **list_partner_transactions**: List all partner transactions
- **list_partner_webhooks**: List all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PartnerStack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active partners in my account."

**🤖 AI Agent:**
> I've retrieved 15 active partners, including 'Referral King', 'Global Affiliates', and 'Tech Connect'. Would you like details for any specific partner?

---

**👤 You:**
> "Show me the last 5 leads submitted by our partners."

**🤖 AI Agent:**
> I've fetched the latest leads. Recent submissions include 'John Smith' from partner 'AffiliateOne' and 'Acme Corp' from 'Growth Partners'. Would you like the full details?

---

**👤 You:**
> "What is the status of the rewards for the 'Summer Campaign'?"

**🤖 AI Agent:**
> I've retrieved the rewards log. For the 'Summer Campaign', there are 12 rewards 'pending_approval' and 8 'paid' rewards. Would you like a list of the pending ones?


## ❓ FAQ

**Q: How do I find my PartnerStack API Key?**
In your PartnerStack dashboard, go to **Settings** > **Integrations** and look for the API Key section. You may need to generate a new key if one doesn't exist.

**Q: Can I see leads submitted by a specific partner?**
Yes! Use the `list_partner_leads` tool. You can ask the AI agent to filter the results for a particular partner name or ID from the retrieved list.

**Q: Does this support reward tracking?**
Absolutely. Use the `list_partner_rewards` tool to see a log of all generated rewards and their current status across your partner ecosystem.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/partnerstack](https://vinkius.com/mcp/partnerstack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PartnerStack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `partnerstack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PartnerStack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "partnerstack": {
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
