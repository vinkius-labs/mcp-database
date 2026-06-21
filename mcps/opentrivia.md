# OpenTrivia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opentrivia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [learning-training](../categories/learning-training.md)

Access a massive database of trivia questions — fetch quizzes by category, manage session tokens, and track global question statistics.

## Description
Connect to the **Open Trivia Database** (OpenTDB) and transform any AI agent into a trivia master or educational assistant. This server provides seamless access to thousands of verified user-contributed questions.

### What you can do

- **Fetch Questions** — Retrieve trivia questions with granular filters for amount (up to 50), category, difficulty (easy, medium, hard), and type (multiple choice or true/false).
- **Session Management** — Use session tokens to ensure you never receive the same question twice within a 6-hour window.
- **Category Discovery** — Browse the full list of trivia categories and their corresponding IDs to target specific knowledge areas.
- **Database Insights** — Query real-time statistics on question counts per category or global database health (verified vs. pending questions).
- **Token Control** — Request and reset session tokens to manage long-running trivia sessions or restart a quiz cycle.

### How it works

1. Subscribe to this server
2. Use the tools to fetch categories or start a session
3. Generate quizzes directly in your AI chat interface

### Who is this for?

- **Developers** — Build trivia bots, games, or learning apps without managing a backend database.
- **Educators** — Instantly generate classroom quizzes or study materials across dozens of subjects.
- **Trivia Fans** — Challenge yourself or others with fresh questions from a community-driven source.


## Available Tools
- **get_categories**: Lookup all trivia categories
- **get_category_count**: Get question count for a category
- **get_global_count**: Get global question count
- **get_questions**: Retrieve trivia questions
- **request_token**: Tokens expire after 6 hours of inactivity.

Retrieve a session token
- **reset_token**: Reset a session token


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenTrivia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get 5 medium difficulty multiple choice questions about Geography."

**🤖 AI Agent:**
> I've retrieved 5 medium-difficulty Geography questions for you. Topics include European capitals and world landmarks. Ready to start the quiz?

---

**👤 You:**
> "List all available trivia categories and their IDs."

**🤖 AI Agent:**
> Here are the available categories: General Knowledge (9), Entertainment: Books (10), Science & Nature (17), History (23), and many more. Which one interests you?

---

**👤 You:**
> "Show me the global question statistics for the entire database."

**🤖 AI Agent:**
> The global database currently contains over 4,000 verified questions, with several hundred pending review. Total questions across all categories are distributed between multiple choice and true/false formats.


## ❓ FAQ

**Q: How do I ensure I don't get the same trivia question twice?**
First, use the `request_token` tool to generate a session token. Then, include this token in your `get_questions` requests. The API will track your history and exclude previously seen questions for 6 hours.

**Q: How can I find the ID for a specific category like 'Science & Nature'?**
Use the `get_categories` tool. It returns a complete list of all available trivia categories along with their unique numerical IDs, which you can then use to filter your questions.

**Q: Is there a way to check how many questions are available in a specific category?**
Yes, use the `get_category_count` tool and provide the category ID. It will return the total number of questions available for that specific topic, including difficulty breakdowns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opentrivia](https://vinkius.com/mcp/opentrivia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenTrivia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opentrivia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenTrivia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opentrivia": {
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
