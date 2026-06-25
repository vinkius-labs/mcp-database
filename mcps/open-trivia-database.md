# Open Trivia Database MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/open-trivia-database)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access 13,000+ community-curated trivia questions from OpenTDB � filter by category, difficulty, and type with session-based deduplication.

## Description
Empower your AI agent to orchestrate your entire entertainment research and trivia auditing workflow with **The Trivia API**, the comprehensive source for high-quality quiz data. By connecting The Trivia API to your agent, you transform complex content searches into a natural conversation. Your agent can instantly retrieve random trivia questions, audit category distributions, and query specific difficulty levels without you ever touching a trivia portal. Whether you are building social applications or conducting research on general knowledge, your agent acts as a real-time creative assistant, ensuring your content is always engaging and well-categorized.

### What you can do

- **Question Auditing** — Retrieve random trivia questions instantly and maintain a clear view of content and choice distribution.
- **Category Oversight** — Browse available trivia categories like 'Arts & Literature', 'Film & TV', or 'Science' to identify relevant themes for your audience.
- **Difficulty Discovery** — Query questions by specific difficulty levels (easy, medium, hard) to understand the cognitive scale of the content.
- **Tag Intelligence** — Retrieve available trivia tags to identify relevant stylistic markers for your quiz applications.
- **Operational Monitoring** — Check API status to ensure your trivia research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (The Trivia API is a free and open service)
3. Start managing your trivia intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — monitor trivia trends and retrieve fresh questions straight from your workflow.
- **App Developers** — verify question availability and audit category distributions without manual searching.
- **Educators & Gamers** — perform rapid audits of trivia content and identify relevant markers through natural language.
- **Operations Leads** — automate entertainment data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools (6)
- **get_global_question_count**: Get total number of questions in the entire OpenTDB database
- **get_trivia_questions**: Supports category, difficulty, and type filters. No API key required.

Get random trivia questions from the Open Trivia Database
- **list_categories**: List all available trivia categories with their IDs
- **request_session_token**: Use the token in subsequent get_trivia_questions calls to guarantee unique questions. Tokens expire after 6 hours of inactivity.

Request a new session token to avoid duplicate questions
- **reset_session_token**: Reset a session token to start receiving all questions again
- **get_category_question_count**: Get the number of questions available in a specific category


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Trivia Database** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get 5 random trivia questions from the 'Science' category using Trivia API."

**🤖 AI Agent:**
> I've retrieved 5 science trivia questions for you! They cover topics from biology to physics and are identified as having varied difficulties. Would you like the correct answers or another set of questions?

---

**👤 You:**
> "Show me easy trivia questions about 'Geography'."

**🤖 AI Agent:**
> I've identified several easy geography questions! Notable entries include queries about major world capitals and landmarks. I can provide the full list of choices for each question if you'd like.

---

**👤 You:**
> "List all available trivia categories."

**🤖 AI Agent:**
> I've scanned the category catalog. There are 10 main groups available, including 'Arts & Literature', 'Film & TV', 'Food & Drink', 'General Knowledge', and 'Geography'. I can help you retrieve questions for any of these specific themes.


## ❓ FAQ

**Q: Is an API Key required for The Trivia API?**
No. The Trivia API provides a free and open service. This server works out of the box without any static credentials required.

**Q: Can I filter questions by difficulty?**
Yes. Use the `get_trivia_questions` tool and provide the `difficulties` parameter (e.g., 'easy' or 'hard'). Your agent will return matching questions instantly.

**Q: What format are the answers in?**
The API provides a correct answer and a list of incorrect answers. Your agent automatically combines and sorts these into a list of choices for each question.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/open-trivia-database](https://vinkius.com/mcp/open-trivia-database)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Trivia Database** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-trivia-database` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Trivia Database** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-trivia-database": {
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
