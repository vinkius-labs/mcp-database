# Nuclino MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nuclino)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent with full read/write access to your Nuclino workspaces, teams, and items — the unified tool for knowledge, docs, and projects.

## Description
Connect your **Nuclino** account to your AI agent and seamlessly interact with your company's unified workspace for knowledge, docs, and projects.

### What you can do

- **Teams & Workspaces** — Rapidly list all teams you are part of, and enumerate the nested workspaces and collections to understand your organization's hierarchy.
- **Search & Query** — Perform global fuzzy searches using `search_items` to track down specific documents, notes, or project pages across the entire knowledge base.
- **Read Items & Files** — Read the exact content configuration of any item (document) via `get_item`, and list attachments or files uploaded to the platform.
- **Record Creation** — Instantly create new items natively inside your workspace using natural language.
- **Telemetrics** — Enumerate members and structural fields within your Nuclino domain to keep the agent aware of context and owners.

### How it works

1. Subscribe to this server
2. Enter your Nuclino Personal API Key
3. Start querying your company wiki and project trackers from Claude, Cursor, or your preferred AI client

### Who is this for?

- **Knowledge Managers** — quickly search the internal wiki, read past guidelines, and append meeting notes to workspaces automatically.
- **Engineering Teams** — access technical documentation and specs without leaving your IDE.
- **Project Managers** — track deliverables, create new planning documents, and monitor active users.


## Available Tools (12)
- **list_teams**: Use this as the entry point to discover available root organizational unit IDs traversing down into workspaces.

List all organizational Teams the authenticated user belongs to
- **list_workspaces**: Returns internal workspace UUIDs essential for scoping later item queries.

List all isolated Workspaces mapped within a specific Team
- **list_items**: Used to enumerate top-level document UUIDs, titles, and creation metadata natively spanning a specific Workspace layer.

List all standard knowledge items (pages) in a Workspace
- **get_item**: Retrieve the exact Markdown payload and configuration of an Item
- **create_item**: Triggers real-time replication creating permanent Wiki documentation.

Write a brand new knowledge Item / Page into a Workspace
- **update_item**: Alters the sync tree immediately appending new wiki edits.

Overwrite active partial Markdown states inside a listed Item
- **delete_item**: Always confirm with the user heavily before destroying knowledge.

Irreversibly delete a structural Nuclino Item
- **search_items**: Use to uncover unknown UUIDs.

Execute an indexed semantic search globally across a Team
- **list_collections**: Used to trace the document relationship graph paths visually within a target Workspace.

List Collections (grouping directories) segmenting a Workspace
- **list_fields**: Used to understand standard taxonomy dimensions applicable against Items.

Map customizable structured property fields globally binding a Team
- **list_users**: Enumerate human identities attached globally onto a Team
- **list_files**: Exposes pure URL bindings mapping binary data records back to object storage.

List physical attachments explicitly bolted onto an Item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nuclino** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Nuclino for any documentation mentioning 'SSO Security Policies'."

**🤖 AI Agent:**
> I've successfully performed a fuzzy text search and located the page 'SSO Security Implementation Guidelines'. I can extract its contents or share the browser link if needed.

---

**👤 You:**
> "Create an item titled 'Project X Architecture Brief' in the Engineering workspace."

**🤖 AI Agent:**
> I retrieved the Engineering workspace ID and created the new item 'Project X Architecture Brief'. The document is live and awaiting further edits.

---

**👤 You:**
> "List all teams connected to this authentication token."

**🤖 AI Agent:**
> You have access to 3 teams on this environment: Design Ops (`id-1`), Software Engineering (`id-2`), and Executive Planning (`id-3`).


## ❓ FAQ

**Q: How can I explore the hierarchy of my company's Nuclino configuration?**
Your AI agent can progressively drill down by invoking `list_teams`, taking those IDs into `list_workspaces`, checking the clusters via `list_collections`, and finally dumping the granular content using `list_items`.

**Q: Can the agent perform global searches if I don't know the workspace?**
Yes. Instead of manually parsing directories, ask the agent to invoke the `search_items` tool. It queries all permissible areas on Nuclino simultaneously and returns exact contextual matches within seconds.

**Q: Can I automatically append meeting notes as a brand new document?**
Absolutely. Once an AI process finishes an important chat, use the `create_item` tool to generate a fresh target URL holding the transcribed content straight into any specified workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuclino](https://vinkius.com/mcp/nuclino)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nuclino** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nuclino` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nuclino** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nuclino": {
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
