# Markdown Utilities Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/markdown-utilities-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI with programmatic Markdown tools. Deterministically generate Table of Contents (TOC) with correct anchor links and format perfect Markdown tables from JSON.

## Description
LLMs often struggle to construct long, structurally sound Markdown elements. Generating a 50-row Markdown table from raw data often leads to broken pipes (`|`), misaligned columns, or omitted rows. Creating a Table of Contents for a massive README is similarly tedious and error-prone for AI. The Markdown Utilities MCP solves this by delegating the heavy lifting to a precise JavaScript formatting engine.

### The Superpowers
- **Flawless Tables:** Instantly convert any complex array of JSON objects into a perfectly aligned Markdown table. No broken columns or missing separators.
- **Automated TOC:** Parses huge Markdown documents and generates a nested Table of Contents with mathematically accurate GitHub-style URL slugs.
- **Zero-Latency Execution:** Runs 100% locally on your machine, ensuring immediate response times for rendering huge documentation blocks.
- **Privacy First:** Since it's a local utility, your proprietary internal documentation never leaves your infrastructure.


## Available Tools
- **generate_table_from_json**: It will automatically extract headers and format rows.

Converts a JSON array of objects into a beautifully formatted Markdown table
- **generate_toc**: It will return a nested list of bullet links pointing to the header slugs.

Generates a perfect, linked Table of Contents (TOC) from a raw Markdown text


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Markdown Utilities Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a Table of Contents for this massive README text I pasted below."

**🤖 AI Agent:**
> Using the generate_toc tool: 
- [Introduction](#introduction)
  - [Features](#features)
- [Deployment](#deployment)

---

**👤 You:**
> "Here is the raw database output JSON: `[{"id": 1, "name": "John", "role": "Admin"}, {"id": 2, "name": "Jane", "role": "User"}]`. Convert this into a Markdown table."

**🤖 AI Agent:**
> Using the generate_table_from_json tool:
| id | name | role |
|---|---|---|
| 1 | John | Admin |
| 2 | Jane | User |


## ❓ FAQ

**Q: Why use an MCP for Markdown tables?**
When generating large Markdown tables, AI models commonly drop rows to save tokens or accidentally break the table structure by forgetting column separators. This MCP guarantees an absolutely perfect conversion from JSON.

**Q: How does the TOC generator calculate URL slugs?**
It follows standard GitHub Flavored Markdown rules. It parses every Header (e.g. `### My Title`), strips special characters, replaces spaces with hyphens, and outputs `- [My Title](#my-title)` with accurate indentation.

**Q: Does this tool send my internal documents to the cloud?**
No. The `markdown-utilities` engine executes completely locally using V8. Your proprietary documentation data is processed safely and privately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/markdown-utilities-engine](https://vinkius.com/mcp/markdown-utilities-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Markdown Utilities Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `markdown-utilities-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Markdown Utilities Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "markdown-utilities-engine": {
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
