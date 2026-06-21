# Gamma (AI Presentations) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gamma-ai-presentations)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate AI-powered presentations, documents, and webpages. List, update, and manage your Gamma workspace directly from any AI agent.

## Description
Connect **Gamma** to your AI agent to transform prompts into beautiful presentations, documents, or webpages instantly. Streamline your creative workflow by generating and managing content through natural language.

### What you can do

- **AI Creation** — Use `create_gamma` to generate presentations, documents, or webpages from a simple prompt or a detailed outline.
- **Content Management** — Retrieve specific details of any creation with `get_gamma` or list your entire library using `list_gammas`.
- **Dynamic Updates** — Modify titles and content of existing Gammas on the fly with `update_gamma` to keep your information current.
- **Workspace Cleanup** — Permanently remove outdated or unnecessary content using `delete_gamma`.

### How it works

1. Subscribe to this server
2. Enter your Gamma API Key
3. Start generating professional presentations and documents from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & Marketing** — Quickly generate pitch decks and landing pages from campaign briefs.
- **Educators & Trainers** — Turn lesson outlines into structured presentations in seconds.
- **Product Managers** — Create product documentation and internal wikis directly from project notes.


## Available Tools
- **update_gamma**: Update an existing Gamma
- **create_gamma**: Create a new Gamma (presentation, document, or webpage)
- **delete_gamma**: Delete a Gamma
- **get_gamma**: Get details of a specific Gamma
- **list_gammas**: List all Gammas


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gamma (AI Presentations)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a presentation about the future of renewable energy with a professional theme."

**🤖 AI Agent:**
> I've started creating your presentation using `create_gamma`. The type is set to 'presentation' with your prompt. I'll provide the details once it's ready.

---

**👤 You:**
> "List my 5 most recent Gammas."

**🤖 AI Agent:**
> Fetching your library... I found your 5 most recent Gammas using `list_gammas`. Here they are: [List of Gammas with IDs and Titles].

---

**👤 You:**
> "Get the content and status for Gamma ID gam_12345."

**🤖 AI Agent:**
> Retrieving details for `gam_12345`... The status is 'completed' and the title is 'Q3 Strategy'. Would you like to see the full content outline?


## ❓ FAQ

**Q: What types of content can I create with this server?**
You can create three types of content using the `create_gamma` tool: 'presentation', 'document', or 'webpage'. Simply specify the type and provide a prompt or outline.

**Q: How can I see a list of all my existing Gamma creations?**
Use the `list_gammas` tool. You can also provide an optional 'limit' to control the number of results returned.

**Q: Is it possible to edit the title of a Gamma after it has been generated?**
Yes! Use the `update_gamma` tool with the specific Gamma ID and provide a new 'title'. You can also update the 'content' using the same tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gamma-ai-presentations](https://vinkius.com/mcp/gamma-ai-presentations)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gamma (AI Presentations)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gamma-ai-presentations` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gamma (AI Presentations)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gamma-ai-presentations": {
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
