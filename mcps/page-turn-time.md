# Page Turn Time MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/page-turn-time)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Estimate reading duration based on page count and speed.

## Description
Page Turn Time provides precise reading duration estimates. Use `get_reading_profiles` to find standard speeds, `calculate_estimated_time` to find total duration for a document, `compare_reading_speeds` to see the difference between two speeds, or `validate_document_feasibility` to check if a reading task fits within your schedule.


## Available Tools (4)
- **calculate_estimated_time**: Calculates total time required to read a document
- **compare_reading_speeds**: Determines the difference in time between two reading speeds
- **get_reading_profiles**: Provides standard reading speed constants
- **validate_document_feasibility**: Checks if a reading task is realistic within a time constraint


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Page Turn Time** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take to read 150 pages if I spend 3 minutes per page?"

**🤖 AI Agent:**
> It will take 450 minutes, which is 7.5 hours.

---

**👤 You:**
> "What is the time difference between reading 50 pages at 2 minutes per page versus 5 minutes per page?"

**🤖 AI Agent:**
> The difference is 150 minutes.

---

**👤 You:**
> "I have 60 minutes. Can I read 30 pages at 2 minutes per page?"

**🤖 AI Agent:**
> Yes, you can finish the reading task with 0 minutes remaining.


## ❓ FAQ

**Q: How do I know which reading speed to use?**
You can use `get_reading_profiles` to retrieve standard speed constants for different reading styles.

**Q: Can I include a buffer for interruptions?**
Yes, when using `calculate_estimated_time`, you can set the buffer option to include a safety margin.

**Q: How do I check if I have enough time to finish a book?**
Use `validate_document_feasibility` to compare your total pages and estimated speed against your available minutes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/page-turn-time](https://vinkius.com/en/ai-agent-connect/page-turn-time)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Page Turn Time** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `page-turn-time` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Page Turn Time** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "page-turn-time": {
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
