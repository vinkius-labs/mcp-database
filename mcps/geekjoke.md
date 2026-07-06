# GeekJoke MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/geekjoke)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Get random geeky and programming-related jokes to lighten up your development workflow.

## Description
Connect to the **GeekJoke** API to fetch humorous content specifically tailored for developers and tech enthusiasts. Whether you need a quick laugh during a debugging session or want to share a joke with your team, this server provides instant access to a curated collection of geeky humor.

### What you can do

- **Random Jokes** — Fetch a random programming or geek joke instantly using the standard query method.
- **API Metadata** — Access information about the underlying API source, including author details and project links.
- **Alternative Generation** — Use an alternative action-based method to retrieve humor content via POST requests.

### How it works

1. Subscribe to this server
2. No API key is required as the service is public
3. Start asking for jokes in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — to break the tension during long coding sessions or frustrating bugs.
- **Team Leads** — to start standups or meetings with a lighthearted, relatable moment.
- **AI Enthusiasts** — to add personality and humor to their custom AI agents.


## Available Tools (3)
- **generate_random_joke**: Get a random geeky joke via POST
- **get_random_joke**: Get a random geeky joke
- **get_metadata**: Get GeekJoke API metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GeekJoke** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me a random geeky joke."

**🤖 AI Agent:**
> Using `get_random_joke`... 'Why do programmers always mix up Halloween and Christmas? Because Oct 31 == Dec 25.'

---

**👤 You:**
> "Show me the metadata for the GeekJoke API."

**🤖 AI Agent:**
> Fetching metadata via `get_metadata`... The API is authored by Sameer Kumar and the project can be found at https://github.com/sameerkumar18/geek-joke-api.

---

**👤 You:**
> "Generate a joke using the POST method."

**🤖 AI Agent:**
> Executing `generate_random_joke`... 'A SQL query goes into a bar, walks up to two tables, and asks, "Can I join you?"'


## ❓ FAQ

**Q: How do I get a random geeky joke?**
You can use the `get_random_joke` tool. It will fetch a random programming or tech-related joke from the API and display it immediately.

**Q: Can I see the source information and author of these jokes?**
Yes! Use the `get_metadata` tool to retrieve the API's project links and author information.

**Q: Is there an alternative way to generate a joke if the standard query fails?**
Yes, you can use the `generate_random_joke` action, which uses a POST request method to fetch a joke from the root endpoint.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/geekjoke](https://vinkius.com/mcp/geekjoke)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GeekJoke** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `geekjoke` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GeekJoke** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "geekjoke": {
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
