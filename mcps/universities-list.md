# Universities List MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/universities-list)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Global university database — search higher education institutions by name and country via AI.

## Description
Equip your AI agent with global academic intelligence via the **Universities List** MCP server. This integration provides access to a comprehensive database of higher education institutions worldwide. Your agent can search for universities by name, filter results by country, and retrieve official website URLs for thousands of entities. Whether you are researching academic programs, verifying institutional details, or exploring international education options, your agent acts as a dedicated academic registrar through natural conversation.

### What you can do

- **University Search** — Find institutions by name or partial string matching.
- **Country Filtering** — Narrow down academic searches to specific countries.
- **Official Links** — Retrieve direct URLs to the official web pages of universities.
- **Global Coverage** — Explore higher education entities across hundreds of sovereign states.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start searching for universities from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Students & Applicants** — explore university options and find official websites for research.
- **Academic Researchers** — identify institutions in specific regions for studies or collaboration.
- **Education Consultants** — quickly verify the existence and details of global higher ed entities.
- **Admissions Officers** — cross-reference institutional data and official domains.


## Available Tools (1)
- **search_universities**: Search for universities by name or country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Universities List** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for universities with 'Technology' in their name in the United States."

**🤖 AI Agent:**
> Searching for technology institutions in the US... I've found several, including the Massachusetts Institute of Technology (MIT) and California Institute of Technology (Caltech). I have their official web links ready for you.

---

**👤 You:**
> "List all universities in 'Portugal'."

**🤖 AI Agent:**
> Retrieving institutions in Portugal... I've found a comprehensive list including the University of Lisbon, University of Porto, and University of Coimbra. Would you like the official website for any of them?

---

**👤 You:**
> "Find universities in Canada that have 'Medical' in their title."

**🤖 AI Agent:**
> Searching Canadian institutions... I've identified several entities such as the Northern Ontario School of Medicine and others associated with medical faculties. I can provide the official domains if you'd like to explore their programs.


## ❓ FAQ

**Q: Can I search for universities in Brazil?**
Yes! Use the `search_universities` tool and set the `country` parameter to 'Brazil'. It will return a list of registered institutions in the country.

**Q: How do I find the official website of a university?**
The search results from the `search_universities` tool include a `web_pages` field containing the official URLs for each institutional record found.

**Q: Is it possible to search for universities in a specific state?**
The underlying database primarily filters by country. You can include state or city names in the `name` search parameter to narrow down results for specific regions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/universities-list](https://vinkius.com/mcp/universities-list)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Universities List** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `universities-list` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Universities List** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "universities-list": {
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
