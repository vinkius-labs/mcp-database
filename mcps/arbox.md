# Arbox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arbox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Manage members, schedule, coaches, leads, payments, and CRM for your Arbox-powered fitness studio through natural conversation.

## Description
Connect your **Arbox** studio to any AI agent.

- **Members** — Search with CRM profile, engagement score, attendance
- **Schedule** — Classes with coach, spots left, enrolled members
- **Coaches** — Trainers with specialties and availability
- **Leads** — Sales pipeline: source, status, assigned salesperson
- **Memberships** — Unlimited, limited, punch cards, trials
- **Payments** — Transaction tracking, amounts, methods
- **Products** — Retail: merchandise, supplements, accessories

Arbox is a CRM-first studio management platform popular in Israel and growing globally. Its strength is in lead management and sales pipeline tracking.


## Available Tools
- **search_members**: Returns profile, membership, attendance, and engagement score.

Search studio members
- **get_member**: Get member profile
- **list_schedule**: List class schedule
- **list_memberships**: List membership plans
- **list_coaches**: List coaches/trainers
- **list_leads**: Key for studio sales pipeline.

List sales leads
- **list_payments**: List payments
- **list_products**: List products/retail
- **get_branch_info**: Get branch info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arbox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me our active leads and their status."

**🤖 AI Agent:**
> Active sales pipeline:

🔥 **Hot leads (3)**:
- Sarah M. — Trial class booked for tomorrow, source: Instagram
- Mike T. — Visited twice, interested in monthly plan
- Ana R. — Referred by member Lisa, wants personal training

🟡 **Warm leads (5)**:
- 3 from website form, 2 from walk-ins

🔵 **Cold leads (8)**:
- Last contact > 14 days ago

Conversion rate this month: 42% (8/19 leads converted)


## ❓ FAQ

**Q: What makes Arbox different?**
Arbox is CRM-first — it excels at lead tracking, sales pipeline management, and member engagement scoring. While other platforms focus on scheduling, Arbox treats every member interaction as a CRM touchpoint, making it ideal for studios focused on growth and retention.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arbox](https://vinkius.com/mcp/arbox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Arbox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `arbox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Arbox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "arbox": {
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
