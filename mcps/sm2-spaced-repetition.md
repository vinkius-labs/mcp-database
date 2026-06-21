# SM2 Spaced Repetition MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sm2-spaced-repetition)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

High-performance implementation of the SM-2 algorithm for optimal review scheduling.

## Description
This MCP server provides a high-performance implementation of the SM-2 algorithm, the foundation used by systems like Anki. It allows AI agents to calculate optimal review intervals, update easiness factors, and manage card statuses based on user performance. Using tools like `evaluate_review_batch`, agents can process multiple card updates in a single call, ensuring efficient memory retention through scientifically backed scheduling.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **SM2 Spaced Repetition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Update my cards with these scores: ID 1: 5, ID 2: 2"

**🤖 AI Agent:**
> Card 1 is now scheduled for a longer interval, and Card 2 has been reset to a 1-day interval.

---

**👤 You:**
> "What are the default settings for a new card?"

**🤖 AI Agent:**
> New cards start with an initial Easiness Factor of 2.5 and an initial interval of 1 day.

---

**👤 You:**
> "Check if these scores are valid: [6, 3, -1]"

**🤖 AI Agent:**
> The scores 6 and -1 are invalid. All scores must be integers between 0 and 5.


## ❓ FAQ

**Q: How does the SM-2 algorithm work?**
It uses review quality scores (0-5) to adjust the interval between reviews and the Easiness Factor, helping to schedule reviews at the peak of your forgetting curve. Tools available: `your_tool_name`.

**Q: Can I process multiple cards at once?**
Yes, the `evaluate_review_batch` tool allows you to send a batch of card updates in a single request for maximum efficiency.

**Q: What are the supported card statuses?**
The system manages cards through three stages: New, Learning, and Mature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sm2-spaced-repetition](https://vinkius.com/mcp/sm2-spaced-repetition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SM2 Spaced Repetition** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sm2-spaced-repetition` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SM2 Spaced Repetition** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sm2-spaced-repetition": {
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
