# CourtListener MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/courtlistener)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage your legal research — search court opinions, dockets, and citations via AI.

## Description
Empower your AI agent to orchestrate your entire legal research workflow with **CourtListener**, the world's leading free and open platform for legal data. By connecting CourtListener to your agent, you transform complex legal searches into a natural conversation. Your agent can instantly search for opinions, audit court dockets, and retrieve detailed judge information without you ever touching a technical portal. Whether you are conducting case law research or monitoring judicial activity, your agent acts as a real-time legal assistant, ensuring your research is always grounded in open and accessible data.

### What you can do

- **Opinion Auditing** — Search for legal opinions by keyword and retrieve detailed metadata, including court name and date filed.
- **Docket Oversight** — Query court dockets to stay on top of ongoing litigation and case filings in real-time.
- **Judicial Intelligence** — Retrieve detailed information about judges and their financial disclosures to maintain strict control over your research context.
- **Citation Discovery** — List citations for specific opinions to understand the legal network and precedents.
- **Court Governance** — List all available courts and their metadata to ensure your jurisdictional research is accurate.

### How it works

1. Subscribe to this server
2. Enter your CourtListener API Key
3. Start managing your legal research through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — monitor case law and docket updates straight from your workflow.
- **Researchers & Journalists** — verify judicial metadata and financial disclosures without manual searches.
- **Law Students** — perform rapid audits of legal citations and opinions through natural language.
- **Operations Leads** — automate legal data querying to orchestrate cross-functional research teams smoothly.


## Available Tools (10)
- **get_judge**: Get details for a specific judge
- **list_citations**: List citations for an opinion
- **list_financial_disclosures**: List judge financial disclosures
- **list_judges**: List judges
- **list_opinions**: List opinions
- **get_opinion**: Get details for a specific opinion
- **search_dockets**: Search for court dockets
- **search_opinions**: Search for legal opinions
- **get_court**: Get details for a specific court
- **list_courts**: List all courts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CourtListener** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for court opinions about 'copyright fair use'."

**🤖 AI Agent:**
> I've retrieved recent opinions. Top results include cases from the 2nd and 9th Circuits regarding digital media and transformation. Would you like the full citations for any of them?

---

**👤 You:**
> "Show me details for judge ID 1234."

**🤖 AI Agent:**
> I've retrieved the judge profile. He has served on the Federal Court since 2010. I can also check for recent financial disclosures if you'd like.

---

**👤 You:**
> "Check for dockets related to 'SpaceX' in 2024."

**🤖 AI Agent:**
> I've found 3 active dockets for 'SpaceX' filed this year. They include a civil matter in Texas and an administrative appeal. Would you like the case numbers and court details?


## ❓ FAQ

**Q: How do I find my CourtListener API Key?**
Log in to your [**CourtListener account**](https://www.courtlistener.com/profile/api/), and you will find your API Key under the **API Tokens** section. Copy and paste it below.

**Q: Can the agent search for both opinions and dockets?**
Yes. Use the `search_opinions` tool for legal judgments and `search_dockets` for case records. Your agent will return matching results from the Free Law Project database.

**Q: Is it possible to list judicial citations via the agent?**
Yes. The `list_citations` tool allows your agent to retrieve all precedents and subsequent citations for any opinion by providing its Opinion ID, helping you map the legal landscape.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/courtlistener](https://vinkius.com/mcp/courtlistener)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CourtListener** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `courtlistener` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CourtListener** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "courtlistener": {
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
