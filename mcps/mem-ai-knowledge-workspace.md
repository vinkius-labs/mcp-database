# Mem AI (Knowledge Workspace) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mem-ai-knowledge-workspace)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your knowledge base via Mem.ai — create notes, run AI semantic search, and organize collections.

## Description
Connect your **Mem.ai** workspace to any AI agent and take full control of your personal and team knowledge through natural conversation.

### What you can do

- **Knowledge Orchestration** — Create new mems (notes) using Markdown directly from your agent, instantly transforming textual ideas into indexed knowledge vectors
- **AI Semantic Search** — Leverage dense semantic similarity to find notes across your entire workspace, identifying relevant information based on meaning rather than explicit keywords
- **Deep Content Retrieval** — Extract the full scalar text body and context metadata for specific mems to retrieve precise project details securely
- **Collection Management** — Establish thematic groupings (Collections) and attach live mems structurally to maintain organized project boundaries natively
- **Quick Capture (Mem It)** — Trigger rapid capture blocks for links, snippets, or raw thoughts, allowing your agent to log ideas without manual dashboard navigation
- **Contextual Updates** — Mutate existing mem content to keep project logs and meeting notes up-to-date while preserving historical knowledge mappings
- **Resource Inventory** — List all available mems or explore specific collections to understand your knowledge distribution and team documentation footprint

### How it works

1. Subscribe to this server
2. Enter your Mem.ai API Key
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Knowledge Workers** — organize research and meeting notes through natural conversation without manual outliner management
- **Project Teams** — sync project documentation and manage shared knowledge collections directly from your workspace
- **Researchers** — leverage AI semantic search to bridge ideas and retrieve relevant context across massive personal knowledge bases efficiently


## Available Tools
- **create_mem**: ai. Converts plain textual knowledge to indexed vectors immediately mapped implicitly via AI.

Create a new mem (note) in Mem.ai using Markdown
- **list_mems**: Returns identifiers and raw bodies. Careful, this returns heavy payloads.

List all raw mems across the global workspace
- **get_mem**: Retrieve explicit full context metadata by target Mem ID
- **update_mem**: Replaces absolute text values so ensure `get_mem` was run to append rather than destroy inadvertently.

Update pre-existing mem content natively swapping strings
- **delete_mem**: No recovery is possible via API.

Irreversibly vaporize a mem document globally
- **search_mems**: AI semantic search looking into all indexed knowledge
- **mem_it**: Quick capture shortcut generating automated blocks
- **list_collections**: Query explicitly tracked thematic Collections arrays
- **create_collection**: Establish new logical thematic groupings mapping notes
- **get_collection**: Inspect specific Collection metadata elements
- **add_mem_to_collection**: Attach live Mems structurally inside explicitly mapped Collections
- **list_collection_mems**: Query ALL explicit Mem bodies inside specific Collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mem AI (Knowledge Workspace)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search my mems for anything related to 'quarterly business review'"

**🤖 AI Agent:**
> Searching semantically… I've identified 3 relevant mems: 1) 'Q1 Review Goals', 2) 'Draft slides for QBR', and 3) a note about 'Revenue projections' that matches the context. Would you like me to retrieve the full content of the QBR slides draft?

---

**👤 You:**
> "Create a new mem with today's standup notes in Markdown"

**🤖 AI Agent:**
> Mem created successfully! I've logged your standup notes into your workspace. New Mem ID: 'mem-12345'. Would you like me to add this mem to your 'Engineering Standups' collection?

---

**👤 You:**
> "List all my thematic collections in Mem"

**🤖 AI Agent:**
> I've retrieved your collections: 'Project Alpha', 'Meeting Archives', 'Personal Research', and 'Reading List'. Which one would you like to explore or add a new note to?


## ❓ FAQ

**Q: How is Mem's AI search different from regular keyword search?**
Mem uses semantic similarity. When your agent uses the `search_mems` tool, it identifies notes based on the meaning of your query. This means you can find relevant context even if you don't remember the exact words used in the original note.

**Q: Can I organize my notes into folders using my agent?**
In Mem, folders are called 'Collections'. Use the `create_collection` and `add_mem_to_collection` tools. Your agent can establish thematic groups and link specific mems to them structurally, maintaining an organized workspace through conversation.

**Q: What is the 'Mem It' tool used for?**
The `mem_it` tool is a quick capture shortcut. Your agent can use it to instantly log raw thoughts, URLs, or snippets into your workspace with automated formatting, perfect for high-speed idea tracking during your workflow.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mem-ai-knowledge-workspace](https://vinkius.com/mcp/mem-ai-knowledge-workspace)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mem AI (Knowledge Workspace)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mem-ai-knowledge-workspace` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mem AI (Knowledge Workspace)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mem-ai-knowledge-workspace": {
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
