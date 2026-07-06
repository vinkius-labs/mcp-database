# FishBase MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fishbase)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Access the world's largest database of fish species. Query common names, database versions, and technical documentation for FishBase and SeaLifeBase.

## Description
Connect to **FishBase** and **SeaLifeBase**, the premier global information systems on fishes and marine organisms. This MCP server allows AI agents to query extensive biological data, common names, and database schema documentation directly.

### What you can do

- **Species Common Names** — Search and list common names of fishes with support for pagination and species filtering using `list_comnames`.
- **Database Versions** — Access different versions of the FishBase/SeaLifeBase databases to track historical records via `get_versions`.
- **Technical Documentation** — Retrieve metadata and documentation for specific database tables to understand the underlying schema with `get_docs_by_table`.
- **Dual Database Support** — Seamlessly switch between FishBase and SeaLifeBase using a simple toggle in any query.
- **API Health Monitoring** — Check the real-time status and heartbeat of the API to ensure connectivity.

### How it works

1. Subscribe to this server
2. Enter your FishBase API Key (if required by your provider)
3. Start exploring ichthyological data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marine Biologists & Researchers** — Quickly verify species data and common names across different regions.
- **Data Scientists** — Understand the FishBase schema and available versions for large-scale data analysis.
- **Educators & Students** — Access reliable, peer-reviewed information about fish species for academic projects.


## Available Tools (5)
- **get_docs_by_table**: Get documentation for a specific database table
- **get_docs**: Get documentation metadata for the FishBase API
- **get_heartbeat**: The root URL redirects here.

Get the current status and time of the FishBase API
- **get_versions**: g., v3, v4) which correspond to specific dates.

List available database versions
- **list_comnames**: Supports pagination and field filtering.

Access common names data for fishes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FishBase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the FishBase API is currently online."

**🤖 AI Agent:**
> I've checked the FishBase API status using `get_heartbeat`. The API is up and running, returning a successful heartbeat signal.

---

**👤 You:**
> "List the common names for 'Gadus morhua' in FishBase."

**🤖 AI Agent:**
> I've retrieved the common names for *Gadus morhua* (Atlantic cod) using `list_comnames`. Results include various regional names such as 'Cod', 'Morue', and 'Bacalao'.

---

**👤 You:**
> "Show me the documentation for the 'species' table in SeaLifeBase."

**🤖 AI Agent:**
> Using `get_docs_by_table` with `use_sealifebase` set to true, I've fetched the documentation for the 'species' table. This table contains primary taxonomic information and species-level metadata.


## ❓ FAQ

**Q: Can I switch between FishBase and SeaLifeBase data?**
Yes. Most tools include a `use_sealifebase` parameter. Set it to `true` to query the SeaLifeBase database instead of the default FishBase.

**Q: How do I find the common names for a specific fish species?**
Use the `list_comnames` tool and provide the species name in the `species` parameter. You can also limit the results or filter specific fields.

**Q: Where can I find documentation for the database tables?**
You can use `get_docs` for general metadata or `get_docs_by_table` to get detailed documentation for a specific table name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fishbase](https://vinkius.com/mcp/fishbase)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FishBase** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fishbase` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FishBase** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fishbase": {
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
