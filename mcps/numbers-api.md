# Numbers API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/numbers-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Facts about numbers and dates — access trivia, math, and historical data via AI.

## Description
Equip your AI agent with interesting facts and historical context for any number or date via the **Numbers API**. This server provides instant access to trivia, mathematical properties, and historical events associated with specific numbers and years. Your agent can retrieve date-specific facts, audit mathematical patterns, and provide random interesting context for numerical data without any manual search. Whether you are adding color to a presentation or verifying historical timelines, your agent acts as a dedicated numerical encyclopedia through natural conversation.

### What you can do

- **Trivia Discovery** — Retrieve fun and unusual facts for any integer or random number.
- **Math Intelligence** — Access technical mathematical properties and interesting patterns for specific numbers.
- **Date Auditing** — Fetch historical events that occurred on any specific month and day of the year.
- **Yearly Context** — Retrieve significant historical milestones and facts for any given year.
- **Random Inspiration** — Get a completely random fact across all categories to discover new knowledge.

### How it works

1. Subscribe to this server
2. No API Key required (Free Public API)
3. Start exploring number intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Educators & Students** — find interesting mathematical and historical context for classroom activities.
- **Content Creators** — retrieve trivia and milestones to enrich articles, videos, and social media posts.
- **History Enthusiasts** — explore what happened on specific dates or years throughout human history.
- **Developers** — integrate dynamic and interesting numerical context into their applications.
- **Data Storytellers** — add human-readable context to purely numerical data points.


## Available Tools
- **get_date_fact**: Get a fact about a date
- **get_math_fact**: Get a mathematical fact about a number
- **get_random_fact**: Get a random fact
- **get_trivia_fact**: Get a trivia fact about a number
- **get_year_fact**: Get a fact about a year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Numbers API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Tell me a trivia fact about the number 42."

**🤖 AI Agent:**
> Retrieving trivia for 42... According to Douglas Adams, it's the answer to the ultimate question of life, the universe, and everything. In reality, it's also the atomic number of molybdenum.

---

**👤 You:**
> "What happened on October 24th in history?"

**🤖 AI Agent:**
> Fetching historical events for October 24th... On this day in 1945, the United Nations Charter came into effect. Would you like me to find facts for another significant date?

---

**👤 You:**
> "Give me a random math fact."

**🤖 AI Agent:**
> Retrieving a random mathematical property... Did you know that 1729 is the smallest number expressible as the sum of two cubes in two different ways? It's known as the Hardy-Ramanujan number.


## ❓ FAQ

**Q: Do I need an API key to use this server?**
No, the Numbers API is completely free and does not require any authentication or API keys.

**Q: Can I search for facts about specific dates like my birthday?**
Yes! Use the `get_date_fact` tool and provide the month and day. Your agent will return a historical event associated with that specific calendar day.

**Q: What kind of mathematical facts are available?**
The `get_math_fact` tool provides properties like whether a number is a prime, Fibonacci number, perfect number, or has other unique mathematical characteristics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/numbers-api](https://vinkius.com/mcp/numbers-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Numbers API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `numbers-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Numbers API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "numbers-api": {
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
