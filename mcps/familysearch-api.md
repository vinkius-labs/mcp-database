# FamilySearch API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/familysearch-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Manage genealogical research — audit persons, pedigrees, and records via AI.

## Description
Empower your AI agent to orchestrate your entire genealogical research and ancestry auditing workflow with the **FamilySearch API**, the world's largest platform for family history. By connecting FamilySearch to your agent, you transform complex ancestor searches into a natural conversation. Your agent can instantly retrieve person details, audit pedigree charts, and query historical record collections without you ever touching a genealogy portal. Whether you are building your family tree or conducting deep-dive historical audits, your agent acts as a real-time genealogical consultant, ensuring your data is always verified and precise.

### What you can do

- **Person Auditing** — Search for millions of persons in the FamilySearch global tree and retrieve detailed metadata, including lifespans and birth/death places.
- **Pedigree Oversight** — Audit the ancestry charts for specific individuals to maintain a clear view of lineage distribution and scale.
- **Memories Discovery** — Retrieve photos, stories, and documents associated with specific persons to identify relevant assets instantly.
- **Record Intelligence** — List available historical record collections to understand the organizational reach of global archives.
- **Metadata Intelligence** — Retrieve unique identifiers and display names for any genealogical record to assist in deep-dive classification.

### How it works

1. Subscribe to this server
2. Enter your FamilySearch Access Token
3. Start managing your ancestry intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Genealogists & Historians** — monitor ancestry data and retrieve official metadata straight from your workflow.
- **Family Researchers** — verify person details and audit lineage patterns without manual searching.
- **Librarians & Archivists** — perform rapid audits of historical collections and identify relevant records through natural language.
- **Operations Leads** — automate genealogical data querying to orchestrate cross-functional educational teams smoothly.


## Available Tools (6)
- **check_api_status**: Check if the FamilySearch API is operational
- **get_person_memories**: Get memories (photos, stories) associated with a person
- **get_person_pedigree**: Get the ancestry (pedigree) for a specific person
- **get_person_details**: Get full details for a specific person in the family tree by ID
- **list_historical_collections**: List historical record collections available on FamilySearch
- **search_persons**: Search for persons in the FamilySearch Family Tree


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FamilySearch API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 'George Washington' in FamilySearch."

**🤖 AI Agent:**
> I've retrieved several matches for George Washington! The primary record shows a lifespan of 1732-1799, born in Westmoreland, Virginia. Would you like to see his full pedigree or associated memories?

---

**👤 You:**
> "Show the pedigree for person ID 'KWCX-S58'."

**🤖 AI Agent:**
> I've retrieved the ancestry chart for KWCX-S58. It includes three generations of ancestors, including names and vital dates. I can provide the unique IDs for these ancestors if you'd like to audit them further.

---

**👤 You:**
> "List available memories for person ID 'LZDP-H7Z'."

**🤖 AI Agent:**
> I've identified 5 memories for this individual, including 3 portrait photos and 2 historical documents. I can assist you with the direct metadata for each of these items if you'd like.


## ❓ FAQ

**Q: How do I find my FamilySearch Access Token?**
Log in to the [**FamilySearch Developer portal**](https://www.familysearch.org/developers/), and you can generate a Personal Access Token or use the OAuth flow to obtain one. Copy and paste it below.

**Q: Can the agent show my family tree?**
Yes. Use the `get_person_pedigree` tool providing a starting person ID. Your agent will return the ancestry chart metadata instantly.

**Q: Are photos and stories included?**
Yes. The `get_person_memories` tool retrieves any photos, stories, and documents (memories) associated with a specified person in the tree.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/familysearch-api](https://vinkius.com/mcp/familysearch-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FamilySearch API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `familysearch-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FamilySearch API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "familysearch-api": {
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
