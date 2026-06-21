# OpenCorporates MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opencorporates)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Access the largest open database of companies — audit corporate records and officers via AI.

## Description
Empower your AI agent to orchestrate your entire corporate auditing and due diligence workflow with **OpenCorporates**, the world's largest open database of companies. By connecting OpenCorporates to your agent, you transform complex registration lookups into a natural conversation. Your agent can instantly search for companies across hundreds of jurisdictions, audit officer histories, and retrieve detailed corporate groupings without you ever touching a manual register. Whether you are conducting competitive analysis or background checks, your agent acts as a real-time corporate investigator, ensuring your business intelligence is always grounded in official, verified data.

### What you can do

- **Corporate Auditing** — Search for companies by name across global jurisdictions and retrieve detailed metadata, including registration numbers and current status.
- **Officer Oversight** — Search for directors and corporate officers to maintain a clear view of organizational leadership and history.
- **Jurisdiction Discovery** — List and query all supported jurisdictions to understand the geographic reach of your research.
- **Grouping Intelligence** — Retrieve details for corporate groupings to understand complex ownership structures instantly.
- **Status Monitoring** — Check your API token usage and account metadata to maintain strict control over your research volume.

### How it works

1. Subscribe to this server
2. Enter your OpenCorporates API Token
3. Start managing your corporate intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Due Diligence Analysts** — monitor company registrations and retrieve official metadata straight from your workflow.
- **Legal Researchers** — verify corporate status and audit officer distributions without manual register exports.
- **Journalists** — perform rapid audits of corporate groupings and identify key ownership markers through natural language.
- **Operations Leads** — automate corporate data querying to orchestrate cross-functional strategy teams smoothly.


## Available Tools (6)
- **get_company_details**: Get full details for a specific company by jurisdiction and number
- **get_corporate_grouping**: Get details for a corporate grouping
- **get_api_status**: Check current API token usage and status
- **list_jurisdictions**: List all jurisdictions supported by OpenCorporates
- **search_companies**: Search for companies by name or keyword
- **search_officers**: Search for corporate officers and directors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenCorporates** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for companies named 'Vinkius' using OpenCorporates."

**🤖 AI Agent:**
> I've retrieved several companies named Vinkius. Notable matches include entities in Brazil and Europe. Would you like the full registration metadata for any specific jurisdiction?

---

**👤 You:**
> "Show company details for 'google' in jurisdiction 'us_de' (Delaware)."

**🤖 AI Agent:**
> I've identified Google in Delaware. The company number is 2838522. I can retrieve the full list of officers and corporate groupings for this entity if you'd like.

---

**👤 You:**
> "Find corporate officers named 'John Smith'."

**🤖 AI Agent:**
> I've identified several officers named John Smith across various jurisdictions. Notable roles include directors in tech and finance sectors. Would you like the company details for any specific match?


## ❓ FAQ

**Q: How do I find my OpenCorporates API Token?**
Log in to your [**OpenCorporates account**](https://opencorporates.com/users/account), and you will find your API Token under your account details. Copy and paste it below.

**Q: What jurisdictions are covered?**
OpenCorporates covers over 140 jurisdictions globally, including the US, UK, EU, and many others. Use the `list_jurisdictions` tool to see the full list.

**Q: Can the agent search for specific people?**
Yes. The `search_officers` tool allows your agent to query the database for individual directors and officers by name to audit their corporate history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opencorporates](https://vinkius.com/mcp/opencorporates)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenCorporates** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `opencorporates` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenCorporates** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opencorporates": {
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
