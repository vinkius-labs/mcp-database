# Adviceslip MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adviceslip)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access over 10 million pieces of advice directly from your AI agent — get random wisdom, search by keyword, or retrieve specific slips by ID.

## Description
Connect to the **Adviceslip** API to empower your AI agent with a massive database of human wisdom. This server provides tools to fetch random advice, search for specific topics, or look up advice by its unique identifier.

### What you can do

- **Random Advice** — Use `get_random_advice` to receive a spontaneous piece of wisdom to inspire your day.
- **Keyword Search** — Use `search_advice` to find all advice slips containing a specific word or phrase (e.g., 'success', 'friendship', 'coding').
- **Direct Lookup** — Use `get_advice_by_id` to retrieve a specific slip when you know its unique numeric ID.

### How it works

1. Subscribe to this server
2. No authentication is required for this public API
3. Start asking for wisdom in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Integrating 'Advice of the Day' features into apps or terminal workflows.
- **Content Creators** — Looking for quick inspiration, unique prompts, or philosophical nuggets.
- **Daily Users** — Seeking a bit of perspective or a quick mental break during their workflow.


## Available Tools (3)
- **adviceslip_get_by_id**: Get a specific advice slip by ID
- **adviceslip_get_random**: Get a random piece of advice
- **adviceslip_search**: Search for advice slips containing a specific term


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adviceslip** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a random piece of advice."

**🤖 AI Agent:**
> I've fetched a random advice slip for you: 'Remember that as far as anyone else is concerned, you're just another person in the street.' (ID: 142)

---

**👤 You:**
> "Search for advice about 'spiders'."

**🤖 AI Agent:**
> I found an advice slip about spiders: 'If you're ever attacked by a group of clowns, go for the juggler.' Wait, that's a joke! Let me find a real one... 'Never trust a spider.' (ID: 83)

---

**👤 You:**
> "What is the advice slip with ID 50?"

**🤖 AI Agent:**
> Advice slip #50 is: 'Don't always take advice from others.' A bit ironic, isn't it?


## ❓ FAQ

**Q: Can I search for advice about a specific topic like 'work' or 'life'?**
Yes! Use the `search_advice` tool with your keyword. It will return a list of all advice slips in the database that contain that specific term.

**Q: How do I get a completely random piece of wisdom?**
Simply call the `get_random_advice` tool. It requires no arguments and will fetch one random slip from the collection of millions.

**Q: What should I do if I want to retrieve a specific advice slip I've seen before?**
If you have the numeric ID of the slip, use the `get_advice_by_id` tool and pass the ID as the `slip_id` parameter to fetch it directly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adviceslip](https://vinkius.com/mcp/adviceslip)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adviceslip** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adviceslip` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adviceslip** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adviceslip": {
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
