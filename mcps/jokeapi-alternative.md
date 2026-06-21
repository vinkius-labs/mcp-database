# JokeAPI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jokeapi-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access thousands of jokes — audit categories and flags via AI.

## Description
Empower your AI agent to orchestrate your entire entertainment research and humor auditing workflow with **JokeAPI**, the leading source for programmable jokes. By connecting JokeAPI to your agent, you transform complex content searches into a natural conversation. Your agent can instantly retrieve random jokes, audit category distributions, and query specific content flags without you ever touching a humor portal. Whether you are building social applications or conducting research on linguistic humor, your agent acts as a real-time creative assistant, ensuring your content is always fresh and well-categorized.

### What you can do

- **Joke Auditing** — Retrieve random or category-specific jokes and maintain a clear view of content and style distribution.
- **Category Oversight** — Browse available joke categories like 'Programming', 'Misc', or 'Pun' to identify relevant themes for your audience.
- **Filter Discovery** — Query available blacklist flags to maintain strict organizational control over the content served.
- **Linguistic Intelligence** — Retrieve jokes in multiple supported languages to assist in regional humor research.
- **Operational Monitoring** — Check API status to ensure your humor research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (JokeAPI is a free and open service)
3. Start managing your humor intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — monitor humor trends and retrieve fresh jokes straight from your workflow.
- **App Developers** — verify joke availability and audit content filters without manual searching.
- **Linguists & Educators** — perform rapid audits of joke types and identify relevant stylistic markers through natural language.
- **Operations Leads** — automate entertainment data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **check_api_status**: Check if the JokeAPI service is operational
- **get_jokes_by_category**: Get jokes from a specific category (e.g., Programming, Misc, Pun)
- **get_random_joke**: Get a random joke from any category
- **list_joke_categories**: List all available joke categories in the database
- **list_joke_blacklist_flags**: List all available flags for blacklisting content (e.g., nsfw, religious)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JokeAPI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a random 'Programming' joke using JokeAPI."

**🤖 AI Agent:**
> I've retrieved a programming joke! It's currently identified as: "[Setup]... [Delivery]". Would you like to see another one or a different category like 'Pun'?

---

**👤 You:**
> "List all available joke categories."

**🤖 AI Agent:**
> I've scanned the category catalog. There are 6 main categories available, including 'Programming', 'Misc', 'Dark', 'Pun', 'Spooky', and 'Christmas'. I can help you retrieve a random joke for any of these specific themes.

---

**👤 You:**
> "What are the content flags for filtering jokes?"

**🤖 AI Agent:**
> I've retrieved the blacklist flags! You can filter jokes by 'nsfw', 'religious', 'political', 'racist', 'sexist', and 'explicit'. I can assist you with an audit of jokes that avoid any of these specific markers.


## ❓ FAQ

**Q: Is an API Key required for JokeAPI?**
No. JokeAPI is a free and open service. This server works out of the box without any static credentials required.

**Q: Can I filter jokes by language?**
Yes. Use the `getRandomJoke` tool and provide the `lang` parameter (e.g., 'en' or 'de'). Your agent will return matching jokes instantly.

**Q: Does it support setup/delivery format?**
Yes. JokeAPI provides both single-line and two-part (setup and delivery) jokes. Your agent will display them in the appropriate Markdown format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jokeapi-alternative](https://vinkius.com/mcp/jokeapi-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JokeAPI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jokeapi-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JokeAPI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jokeapi-alternative": {
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
