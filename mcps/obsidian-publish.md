# Obsidian Publish MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/obsidian-publish)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Empower your AI to read your public or private Obsidian Publish sites. Index files, crawl navigation trees, and retrieve deep markdown knowledge.

## Description
Connect your **Obsidian Publish** environment to your AI agent and construct an intelligent oracle that reads smoothly from your personal or corporate markdown knowledge base.

### What you can do

- **Vault Crawling** — Programmatically fetch your entire published vault structure utilizing `list_files` and `list_navigation` to build contextual trees.
- **Direct Note Access** — Execute `get_file` to stream the complete raw markdown contents of any note directly into your chat workflow for fast summarization.
- **Metadata Operations** — Use `get_metadata` to retrieve frontmatter properties, tags, and internal link logic mapped by Obsidian.
- **Site Auditing** — Easily ping `site_info` to ensure connectivity and verify the deployment status of your target Obsidian publish endpoint.

### How it works

1. Subscribe to this server
2. Enter your Obsidian Publish Site ID (and optional access token for private vaults)
3. Start fetching and analyzing your personal notes directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Researchers & Writers** — seamlessly command an AI to read past chapters, cross-reference characters, or verify published assertions without opening Obsidian.
- **Corporate Teams** — build a highly accessible chatbot that rapidly reads and summarizes your team's documented standard operating procedures (SOPs).
- **Developers** — fetch specific code snippets and technical architectures housed in your digital garden natively within the IDE.


## Available Tools (5)
- **list_files**: List all explicitly published raw file paths across the Obsidian workspace
- **get_file**: Retrieve exact textual file content and binary assets
- **site_info**: Identify global configuration and styling mapping the site
- **list_navigation**: Visualize structurally formatted Markdown navigation trees
- **get_metadata**: Extract internal creation hashes mapping a specific Markdown page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Obsidian Publish** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the vault and list all the files currently publicly available."

**🤖 AI Agent:**
> According to the navigation tree, you have 14 distinct markdown entries published. Key documents include 'Index', 'Machine Learning Setup', and 'Project Specs'.

---

**👤 You:**
> "Read the contents of 'System Requirements 2026.md'."

**🤖 AI Agent:**
> I've pulled the content of 'System Requirements 2026.md'. The document includes heavy focus on horizontal scaling algorithms and Python-centric deployments. Would you like a condensed executive summary?

---

**👤 You:**
> "Fetch the metadata and tags applied to my 'Inbox' note."

**🤖 AI Agent:**
> The 'Inbox' note has the following metadata: generated on May 5th, tagged with `#todo` and `#ideas`, and links heavily to `Projects.md` and `Archived Content.md`.


## ❓ FAQ

**Q: Can the AI accurately recreate the folder structure of my vault?**
Yes. When the model invokes `list_navigation`, it downloads the systematic JSON map of the entire public vault, thereby allowing it to understand the relationships and physical structure of your folders perfectly.

**Q: Does `get_file` automatically render complex Markdown components?**
No rendering is performed on our end. The `get_file` tool returns pure raw Markdown (including frontmatter and obsidian syntax). Fortunately, LLMs (like Claude) are exceptionally adept at reading and reasoning over raw Markdown text structures.

**Q: If my Published site is private and requires a password, does it still work?**
Yes, it works gracefully. If you configured Obsidian Publish with restricted read access, you can manually inject a persistent token into the setup, giving your AI agent the clearance to read securely behind the authentication wall.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/obsidian-publish](https://vinkius.com/mcp/obsidian-publish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Obsidian Publish** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `obsidian-publish` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Obsidian Publish** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "obsidian-publish": {
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
