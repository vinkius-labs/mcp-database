# Focus Minutes Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/focus-minutes-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and aggregate total focus time and session metrics.

## Description
This MCP server provides tools to manage and analyze focus session data. It allows AI agents to retrieve the total minutes spent in focus, count completed sessions, calculate average session durations, and list individual session details. Use `get_total_focus_minutes` to find cumulative time or `list_user_sessions` to see specific session logs.


## Available Tools (4)
- **get_average_session_duration**: Get the average duration of focus sessions for a user
- **get_session_count**: Get the total number of focus sessions for a user
- **get_total_focus_minutes**: You can optionally filter by a session ID pattern.

Get the total focus minutes for a user
- **list_user_sessions**: List all focus sessions for a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Focus Minutes Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total minutes has user_123 spent in focus sessions?"

**🤖 AI Agent:**
> User user_123 has spent a total of 450 minutes in focus sessions.

---

**👤 You:**
> "What is the average duration of focus sessions for user_456?"

**🤖 AI Agent:**
> The average focus session duration for user_456 is 25 minutes.

---

**👤 You:**
> "How many focus sessions has user_789 completed?"

**🤖 AI Agent:**
> User user_789 has completed 12 focus sessions.


## ❓ FAQ

**Q: How can I see the total time a user has spent focusing?**
You can use the `get_total_focus_minutes` tool by providing the user's unique ID.

**Q: Can I see a list of all individual sessions?**
Yes, the `list_user_sessions` tool returns an array of all session IDs and their durations for a specific user.

**Q: How is the average session duration calculated?**
The `get_average_session_duration` tool calculates the mean by dividing the total focus minutes by the total number of sessions recorded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/focus-minutes-total](https://vinkius.com/en/ai-agent-connect/focus-minutes-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Focus Minutes Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `focus-minutes-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Focus Minutes Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "focus-minutes-total": {
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
