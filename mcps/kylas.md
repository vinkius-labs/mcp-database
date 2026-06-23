# Kylas MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kylas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Scale your Indian SMB sales team with a CRM that combines lead management, pipeline tracking, and WhatsApp integration natively.

## Description
Connect your **Kylas** account to any AI agent and manage your sales CRM through natural conversation.

### What you can do

- **Lead Management** — List, create, and inspect leads with status tracking
- **Deal Pipeline** — Browse deals across pipeline stages with values
- **Contact Database** — Manage contacts with activity and communication history
- **Pipeline Monitoring** — Track conversion rates and deal velocity

### How it works

1. Subscribe to this server
2. Enter your Kylas API Key
3. Start managing sales from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — manage leads and deals without opening the CRM
- **Sales Managers** — monitor pipeline health and team performance
- **BDRs** — track prospects and follow-up activities


## Available Tools (7)
- **create_contact**: Create a new contact
- **create_lead**: Pass data as a JSON string.

Create a new lead
- **get_lead**: Get specific lead details
- **list_contacts**: List all CRM contacts
- **list_deals**: List all CRM deals
- **list_leads**: List all Kylas leads
- **list_tasks**: List CRM tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kylas** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show the sales pipeline and deals closing this week."

**🤖 AI Agent:**
> Pipeline: 45 active deals ($890K total). Prospecting (12, $180K), Qualification (8, $120K), Proposal (10, $240K), Negotiation (8, $200K), Closing (7, $150K). Closing this week: 3 deals. 'Acme Corp' ($45K, 90% prob), 'TechCo' ($35K, 80%), 'GlobalInc' ($28K, 75%). Win rate: 32%.

---

**👤 You:**
> "Create a new lead and show all contacts at acmecorp.com."

**🤖 AI Agent:**
> Lead created! 'NovaTech — API Integration'. Source: Website. Status: New. Assigned: Sarah. Contacts at acmecorp.com: 3. John Smith (CTO, 4 deals, $120K), Lisa Park (VP Eng, 2 deals), Mike Torres (Director, 1 deal). Last activity: today.

---

**👤 You:**
> "Show team performance and pipeline conversion metrics."

**🤖 AI Agent:**
> Team: 4 reps. Sarah — 18 deals ($320K), 38% win rate, avg cycle: 22 days. Mike — 12 deals ($210K), 30% win rate. Lisa — 10 deals ($190K), 35%. James — 5 deals ($170K), 28%. Pipeline conversion: Lead→Qualified: 45%. Qualified→Proposal: 60%. Proposal→Won: 32%. Avg deal: $19.8K.


## ❓ FAQ

**Q: Can I manage leads and track deals?**
Yes. List, create, and update leads with status tracking. Browse deals across pipeline stages with deal values and probability.

**Q: Can I monitor pipeline conversion rates?**
Yes. Track pipeline metrics including deal counts per stage, conversion rates, average deal size, and velocity.

**Q: What API endpoint does Kylas use?**
Bearer authentication against `api.kylas.io/v1`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kylas](https://vinkius.com/mcp/kylas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kylas** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kylas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kylas** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kylas": {
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
