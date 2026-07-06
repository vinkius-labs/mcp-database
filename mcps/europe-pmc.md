# Europe PMC MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/europe-pmc)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access over 33 million life science publications and research grants. Search PubMed, Agricola, and more directly from your AI agent.

## Description
Connect to **Europe PMC**, the comprehensive database for biomedical and life sciences literature. This MCP server allows your AI agent to query millions of articles, preprints, and grants to provide evidence-based answers.

### What you can do

- **Article Search** — Query over 33 million publications from PubMed, PMC, and other major sources with advanced filtering.
- **Grant Discovery** — Search the Grist database for details on research grants awarded by Europe PMC funders.
- **Metadata Exploration** — Retrieve available search fields to build precise and complex queries.
- **Flexible Results** — Choose between 'lite', 'core', or 'idlist' result types to get exactly the data you need.

### How it works

1. Subscribe to this server
2. No API key is required for public access
3. Start querying scientific literature from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Scientists** — quickly find relevant literature and citations without leaving your workspace.
- **Medical Professionals** — access the latest clinical studies and biomedical data via natural language.
- **Data Analysts** — gather publication and grant data for bibliometric analysis.


## Available Tools (3)
- **search_articles**: Search Europe PMC articles
- **search_grants**: Search Europe PMC grants (Grist API)
- **get_article_fields**: Get available search fields for articles


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Europe PMC** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for articles about malaria vaccine trials from the last 5 years."

**🤖 AI Agent:**
> I've found several recent articles on malaria vaccine trials. Notable results include 'Safety and efficacy of R21/Matrix-M' and 'Phase 3 trial of RTS,S/AS01'. Would you like the core details for these?

---

**👤 You:**
> "List all available search fields for Europe PMC articles."

**🤖 AI Agent:**
> I've retrieved the available fields. You can filter by 'AUTH' (Author), 'JOURNAL' (Journal Name), 'FIRST_PDATE' (Publication Date), 'ABSTRACT', and many more. Which field would you like to use for your query?

---

**👤 You:**
> "Find research grants awarded by the Wellcome Trust related to genomics."

**🤖 AI Agent:**
> Searching the Grist database... I found several grants from Wellcome Trust. For example, grant GID:206194 for 'Human Functional Genomics'. Would you like to see the institution details or the abstract?


## ❓ FAQ

**Q: Can I sort article search results by citation count?**
Yes. When using the `search_articles` tool, you can include sorting parameters in your query, such as `sort_cited:y` to prioritize highly cited publications.

**Q: How do I know which specific fields I can use to filter my searches?**
You can use the `get_article_fields` tool. It returns a comprehensive list of all available search fields that can be used as parameters in your queries.

**Q: Is it possible to find funding information for specific researchers?**
Yes! Use the `search_grants` tool and provide the investigator's name (e.g., `pi:name`) in the query to find details of grants awarded to them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/europe-pmc](https://vinkius.com/mcp/europe-pmc)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Europe PMC** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `europe-pmc` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Europe PMC** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "europe-pmc": {
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
