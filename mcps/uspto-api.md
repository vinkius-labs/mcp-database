# USPTO API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uspto-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Search US patents and trademarks — audit intellectual property via AI.

## Description
Empower your AI agent to orchestrate your entire intellectual property research workflow with **USPTO API**, the official source for United States patent and trademark data. By connecting the USPTO Open Data API to your agent, you transform complex legal lookups into a natural conversation. Your agent can instantly search for active patents, audit trademark registrations, and retrieve detailed abstract metadata without you ever touching a government portal. Whether you are conducting prior art research or monitoring brand protection, your agent acts as a real-time IP consultant, ensuring your data is always grounded in official, government-verified records.

### What you can do

- **Patent Auditing** — Search for thousands of United States patents by keyword and retrieve detailed metadata, including abstracts and filing dates.
- **Trademark Oversight** — Audit active and pending trademark registrations to maintain a clear view of brand protection trends.
- **IP Discovery** — Retrieve full details for specific patent numbers or trademark serial numbers to assist in legal research.
- **Classification Intelligence** — List patent classification codes to understand the technological hierarchy of innovations instantly.
- **Operational Monitoring** — Check API status to ensure your IP research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (USPTO Open Data is a public and free service)
3. Start managing your IP intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Patent Attorneys & Agents** — monitor filings and retrieve official metadata straight from your workflow.
- **Innovation Researchers** — verify prior art and audit technological trends without manual database searches.
- **Brand Managers** — perform rapid audits of trademark registrations and identify potential conflicts through natural language.
- **Operations Leads** — automate IP data querying to orchestrate cross-functional legal teams smoothly.


## Available Tools
- **check_api_status**: Check if the USPTO Open Data API is operational
- **get_patent_details**: Get full details for a specific patent number
- **get_trademark_details**: Get full details for a specific trademark serial number
- **list_patent_classes**: List all available patent classification codes
- **search_patents**: Search for United States patents by keyword
- **search_trademarks**: Search for United States trademarks by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **USPTO API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for US patents related to 'Artificial Intelligence' using USPTO API."

**🤖 AI Agent:**
> I've retrieved 10 recent patents related to AI. Notable matches include innovations in machine learning and neural networks. Would you like the abstracts for the top 5 records?

---

**👤 You:**
> "Check the status of trademark serial number '88123456'."

**🤖 AI Agent:**
> I've retrieved the trademark details. Serial number 88123456 is currently active and registered to a major tech company. I can provide the filing history and mark description if you'd like.

---

**👤 You:**
> "List all patent classification codes available."

**🤖 AI Agent:**
> I've scanned the classification catalog. It includes hundreds of codes covering diverse technological sectors from mechanics to biotechnology. I can help you filter the list by keyword.


## ❓ FAQ

**Q: Is an API Key required for USPTO API?**
No. The USPTO Open Data API is a public and free service. This server works out of the box without any static credentials required.

**Q: What types of patents can be audited?**
You can search for utility, design, and plant patents registered in the United States, as well as patent applications and publications.

**Q: Is trademark image data included?**
The API primarily returns text-based metadata. For visual trademark records, your agent will retrieve the official USPTO link to the record where visual data can be viewed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uspto-api](https://vinkius.com/mcp/uspto-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **USPTO API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `uspto-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **USPTO API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uspto-api": {
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
