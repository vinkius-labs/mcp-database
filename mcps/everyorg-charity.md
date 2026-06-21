# Every.org Charity MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everyorg-charity)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Universal charity intelligence — search non-profits, causes, and mission data via AI.

## Description
Equip your AI agent with the primary source for non-profit and charitable intelligence via the **Every.org** MCP server. This integration provides instant access to a database of thousands of registered non-profits across various causes like education, animal welfare, and health. Your agent can search for organizations by keyword or cause, retrieve detailed metadata including EINs and slugs, and find direct profile links for donations or research. Whether you are conducting philanthropic research, identifying charities for a campaign, or exploring social causes, your agent acts as a dedicated philanthropic advisor through natural conversation.

### What you can do

- **Charity Search** — Find non-profit organizations by name, keyword, or social cause.
- **Mission Retrieval** — Access descriptions and mission statements for thousands of entities.
- **Detailed Metadata** — Fetch official EINs, slugs, and profile URLs for precise identification.
- **Cause Exploration** — Discover organizations working on specific themes like environment or human rights.
- **Philanthropic Auditing** — Summarize multiple non-profits to compare their impact and focus areas.

### How it works

1. Subscribe to this server
2. Optional: Enter your Every.org API Key
3. Start querying charity data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Philanthropists & Donors** — find verified organizations matching their values and causes.
- **Social Impact Researchers** — analyze the non-profit landscape for specific regions or themes.
- **Corporate Responsibility Officers** — identify potential partners for charitable initiatives.
- **Community Organizers** — quickly list local or thematic non-profits for advocacy.


## Available Tools
- **get_charity_details**: Get details for a specific charity
- **search_charities**: Search for non-profits and charities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Every.org Charity** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find non-profits focused on education in the US."

**🤖 AI Agent:**
> Searching for education-focused non-profits... I've found several organizations including 'Room to Read' and 'Khan Academy'. I have their profile links and descriptions ready for you.

---

**👤 You:**
> "Search for environmental charities with high impact."

**🤖 AI Agent:**
> I've scanned the database for environmental organizations. I found groups like 'The Nature Conservancy' and 'Environmental Defense Fund'. Would you like to see their mission statements or donation links?

---

**👤 You:**
> "Get details for the charity 'Doctors Without Borders'."

**🤖 AI Agent:**
> Retrieving data for Doctors Without Borders (Médecins Sans Frontières)... They are a world-renowned medical humanitarian organization. I have their official EIN, mission overview, and Every.org profile link available.


## ❓ FAQ

**Q: Can I search for charities related to 'ocean conservation'?**
Yes! Use the `search_charities` tool with the query 'ocean conservation'. It will return a list of registered non-profits working in that area.

**Q: What is an EIN?**
EIN stands for Employer Identification Number. It is a unique nine-digit number assigned by the IRS to business entities, including non-profits, for identification in the US.

**Q: How do I find organizations by a specific cause?**
Use the `search_charities` tool and include the cause name (like 'education' or 'health') in the query. The database will filter for organizations matching that mission focus.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everyorg-charity](https://vinkius.com/mcp/everyorg-charity)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Every.org Charity** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `everyorg-charity` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Every.org Charity** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "everyorg-charity": {
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
