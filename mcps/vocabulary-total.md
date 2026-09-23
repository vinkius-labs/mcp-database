# Vocabulary Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vocabulary-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Aggregate and manage English vocabulary learned across multiple sessions.

## Description
Vocabulary Total acts as a central hub for tracking language acquisition. It allows you to consolidate words from various learning sessions into a single master list. Use `add_session_vocabulary` to record new terms, `get_session_summary` to review specific sessions, or `get_total_vocabulary` to see your complete English word bank. You can also use `getMasteryStatistics` to track your progress through different mastery tiers.


## Available Tools (4)
- **add_session_vocabulary**: Ensure the sessionId is unique and words are English.

Adds a new set of learned words from a specific learning session to the master vocabulary
- **get_mastery_statistics**: Analyzes the distribution of vocabulary across different mastery levels
- **get_session_summary**: Retrieves a summary of vocabulary learned within a specific session
- **get_total_vocabulary**: Provides the complete, aggregated list of all English vocabulary learned across all sessions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vocabulary Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add these words from my session 'session_123': 'serendipity' (noun, a fortunate accident) and 'ephemeral' (adjective, lasting a short time). Mark them as new."

**🤖 AI Agent:**
> Successfully added 2 words from session 'session_123'. Total vocabulary count is now 45.

---

**👤 You:**
> "What is the summary for session 'session_123'?"

**🤖 AI Agent:**
> Session 'session_123' contains 2 words: serendipity (noun) and ephemeral (adjective).

---

**👤 You:**
> "Show me all the nouns I have learned."

**🤖 AI Agent:**
> You have learned 12 nouns: serendipity, ocean, mountain, and 9 others.


## ❓ FAQ

**Q: How do I add new words?**
You can use the `add_session_vocabulary` tool to submit a list of words, their definitions, and their parts of speech from a specific session.

**Q: Can I filter my vocabulary list?**
Yes, the `get_total_vocabulary` tool allows you to filter your master list by part of speech or by a specific search term.

**Q: How is mastery tracked?**
Mastery is tracked via the verdict assigned during word entry. You can view the distribution of your words using `getMasteryStatistics`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vocabulary-total](https://vinkius.com/en/ai-agent-connect/vocabulary-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vocabulary Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vocabulary-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vocabulary Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vocabulary-total": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
