# Chuck Norris MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chuck-norris)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access the legendary power of Chuck Norris facts — get random jokes, browse categories, and search the entire database directly from your AI agent.

## Description
Bring the legendary humor of **Chuck Norris** to your AI workspace. This MCP server connects to the official database of Chuck Norris facts, allowing your agent to inject humor, test API connectivity, or simply entertain during long coding sessions.

### What you can do

- **Random Facts** — Fetch a random Chuck Norris joke instantly to lighten the mood.
- **Category Filtering** — Target specific themes like 'dev', 'movie', 'food', or 'science' for contextual humor.
- **Full-Text Search** — Search the vast database for jokes containing specific keywords or phrases.
- **Category Exploration** — Retrieve a complete list of available categories to see the full range of legendary topics.

### How it works

1. Subscribe to this server
2. No complex API keys are required for this public service
3. Start asking for Chuck Norris facts in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Perfect for testing tool-calling capabilities or adding a bit of fun to the terminal.
- **Teams** — Use it to break the ice in collaborative AI environments.
- **AI Enthusiasts** — A simple and reliable way to explore how MCP servers fetch external data.


## Available Tools
- **list_categories**: Retrieve all available joke categories
- **get_random_joke**: Can optionally be filtered by a specific category.

Retrieve a random Chuck Norris joke
- **search_jokes**: Search for Chuck Norris jokes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chuck Norris** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me a random Chuck Norris joke."

**🤖 AI Agent:**
> Chuck Norris doesn't wear a watch. He decides what time it is.

---

**👤 You:**
> "What are the available categories for Chuck Norris facts?"

**🤖 AI Agent:**
> I've retrieved the categories for you. You can choose from: animal, career, celebrity, dev, explicit, fashion, food, history, money, movie, music, political, religion, science, sport, and travel.

---

**👤 You:**
> "Search for Chuck Norris jokes about 'Google'."

**🤖 AI Agent:**
> I found a few! One of them is: 'Chuck Norris doesn't search for things on Google, Google searches for things on Chuck Norris.'


## ❓ FAQ

**Q: Can I get a Chuck Norris joke specifically about developers or coding?**
Yes! Use the `get_random_joke` tool and specify 'dev' as the category. The agent will fetch a random fact tailored to the software engineering world.

**Q: How can I see all the different topics available for jokes?**
You can use the `list_categories` tool. It will return a full list of supported categories such as 'science', 'money', 'fashion', and more.

**Q: Is it possible to find jokes containing a specific word like 'roundhouse'?**
Absolutely. Use the `search_jokes` tool with your desired keyword in the 'query' parameter to find all matching facts in the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chuck-norris](https://vinkius.com/mcp/chuck-norris)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chuck Norris** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chuck-norris` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chuck Norris** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chuck-norris": {
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
