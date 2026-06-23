# Indiegogo Crowdfunding API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/indiegogo-crowdfunding-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Access crowdfunding data — audit campaigns, funding, and categories via AI.

## Description
Empower your AI agent to orchestrate your entire market research and crowdfunding auditing workflow with the **Indiegogo Crowdfunding API**, the comprehensive source for project funding data. By connecting the Indiegogo API to your agent, you transform complex campaign searches into a natural conversation. Your agent can instantly retrieve active project details, audit funding progress against goals, and query specific category metadata without you ever touching a crowdfunding portal. Whether you are conducting product market research or managing regional investment constraints, your agent acts as a real-time venture consultant, ensuring your data is always verified and precise.

### What you can do

- **Campaign Auditing** — Search for thousands of crowdfunding campaigns by keyword and retrieve detailed metadata, including status and funding levels.
- **Funding Oversight** — Audit the raised amount against funding goals for specific projects to understand the current industry lead in market validation instantly.
- **Category Discovery** — Browse all project categories available on Indiegogo to identify relevant thematic markers for your research.
- **Investment Intelligence** — Retrieve unique campaign identifiers and currency metadata to assist in deep-dive financial classification.
- **Operational Monitoring** — Check API status to ensure your crowdfunding research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your Indiegogo API Token
3. Start managing your investment intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Entrepreneurs & Market Researchers** — monitor project trends and retrieve official metadata straight from your workflow.
- **Investors & Analysts** — verify funding progress and audit campaign distributions without manual searching.
- **Product Developers** — perform rapid audits of successfully funded projects and identify relevant market markers through natural language.
- **Operations Leads** — automate crowdfunding data querying to orchestrate cross-functional development teams smoothly.


## Available Tools (4)
- **check_api_status**: Check if the Indiegogo service is operational
- **get_campaign_details**: Get full details and status for a specific Indiegogo campaign by ID
- **list_indiegogo_categories**: List all project categories available on Indiegogo
- **search_indiegogo_campaigns**: Search for crowdfunding campaigns on Indiegogo


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Indiegogo Crowdfunding API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for campaigns related to 'smart home' using Indiegogo."

**🤖 AI Agent:**
> I've retrieved several smart home campaigns! Notable entries include [Project Title] which has raised [Amount]. Would you like the full details or the funding goal metadata for any of these projects?

---

**👤 You:**
> "What is the status of campaign ID '12345'?"

**🤖 AI Agent:**
> I've retrieved the details for campaign 12345! It is currently identified as 'Live' and has raised 75% of its [Amount] goal. I can assist you with the currency metadata and category for this site.

---

**👤 You:**
> "List all project categories on Indiegogo."

**🤖 AI Agent:**
> I've retrieved the category catalog from Indiegogo! Notable groups include 'Tech & Innovation', 'Creative Works', and 'Community Projects'. I can help you search for specific campaigns in any of these thematic clusters.


## ❓ FAQ

**Q: How do I find my Indiegogo API Token?**
Log in to your [**Indiegogo account**](https://www.indiegogo.com/), go to your settings or developer section, and generate a new API token. Copy and paste it below.

**Q: Does it support real-time funding status?**
Yes. The `get_campaign_details` tool retrieves the most recent funding metadata, including current amount raised and campaign status.

**Q: Can the agent show project categories?**
Yes. The `list_indiegogo_categories` tool retrieves the full list of available project categories used to classify data on Indiegogo.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/indiegogo-crowdfunding-api](https://vinkius.com/mcp/indiegogo-crowdfunding-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Indiegogo Crowdfunding API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `indiegogo-crowdfunding-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Indiegogo Crowdfunding API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "indiegogo-crowdfunding-api": {
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
