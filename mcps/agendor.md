# Agendor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/agendor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

CRM for sales teams — manage leads, organizations, and pipelines via AI.

## Description
Connect your **Agendor** account to your AI agent to unlock professional sales orchestration and CRM management. From creating new leads and organizations to auditing your sales pipeline and managing task workflows, your agent handles your sales ecosystem through natural conversation.

### What you can do

- **Lead & Contact Management** — Create, update, and list people and organizations to keep your CRM data current
- **Pipeline Orchestration** — List active deals, monitor sales funnels, and retrieve details for specific deal stages
- **Task Management** — List and create tasks to ensure your team never misses a follow-up or critical deadline
- **Upsert Capability** — Seamlessly create or update records based on email or CNPJ to prevent duplicate data entry
- **Sales Insights** — Quickly identify high-value opportunities or overdue deals directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your Agendor API Token
3. Start managing your CRM and monitoring your sales pipeline through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — monitor pipeline health and team productivity using simple commands
- **Account Executives** — quickly look up client history and update deal statuses on the fly
- **SDRs & BDRs** — research leads and add new prospects to the CRM without leaving the chat
- **Business Owners** — retrieve sales summaries and identify bottlenecks in the revenue process effortlessly


## Available Tools (6)
- **list_people**: Retrieve a comprehensive directory of person profiles registered in your Agendor CRM
- **create_person**: Can optionally link the person to a company.

Instantiate a new person profile natively within the Agendor CRM
- **list_organizations**: Retrieve a directory of institutional organizations, companies, and business entities in the CRM
- **create_organization**: Instantiate a new organization record securely within Agendor
- **list_deals**: Retrieve highly active sales opportunities and negotiation pipelines tracked in Agendor
- **list_tasks**: Retrieve the chronological queue of upcoming activities and follow-ups scheduled for the team


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Agendor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 people added to my Agendor CRM."

**🤖 AI Agent:**
> I've retrieved the latest 5 contacts. They include John Smith, Maria Silva, and 3 others. Would you like to see the contact details or associated deals for any of them?

---

**👤 You:**
> "Show me all deals in the 'Qualified' stage of my pipeline."

**🤖 AI Agent:**
> I've filtered your pipeline. You have 4 deals in the 'Qualified' stage, totaling $15,000 in potential revenue. Would you like the details for these opportunities?

---

**👤 You:**
> "Create a new organization named 'Tech Innovations' with domain 'techinn.com'."

**🤖 AI Agent:**
> I've successfully created 'Tech Innovations' in Agendor. The organization ID is 98765. Would you like to add a primary contact person to this company?


## ❓ FAQ

**Q: Where do I find my Agendor API Token?**
Log in to Agendor, navigate to **Menu** > **Integrações** (Integrations) > **Token da API**. You can generate and copy your unique token from there. It will be used in the `Authorization` header as `Token your-token`.

**Q: What is an 'Upsert' in Agendor?**
An Upsert is a combination of Update and Insert. It allows you to send contact data, and Agendor will either create a new record or update an existing one if the email or CNPJ already exists, preventing duplicates.

**Q: Can I see my team's tasks via the agent?**
Yes! Use the `list_tasks` tool to retrieve upcoming or pending tasks for any user or organization in your CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/agendor](https://vinkius.com/mcp/agendor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Agendor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `agendor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Agendor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "agendor": {
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
