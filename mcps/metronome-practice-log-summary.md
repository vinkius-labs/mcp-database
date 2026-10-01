# Metronome Practice Log Summary MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/metronome-practice-log-summary)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Summarize musical practice sessions by date, BPM, duration, and accuracy.

## Description
This MCP server provides tools to analyze musical practice logs. It allows you to calculate total practice volume, identify peak stable BPM, and track performance metrics for specific musical pieces. Use `get_practice_summary` for high-level period overviews, `get_piece_performance` for detailed stats on a single piece, `get_daily_activity_log` to monitor daily consistency, and `search_logs_by_criteria` to filter sessions by tempo or accuracy.


## Available Tools (4)
- **get_piece_performance**: Calculates specific performance metrics for a single musical piece
- **get_daily_activity_log**: Breaks down practice intensity by day to visualize consistency
- **get_practice_summary**: Provides a high-level overview of total practice volume and peak performance
- **search_logs_by_criteria**: Allows for granular filtering of practice sessions based on specific performance thresholds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Metronome Practice Log Summary** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Give me a summary of my practice from January 1st to January 31st, 2024."

**🤖 AI Agent:**
> In January 2024, you practiced for a total of 120 minutes across 5 sessions, reaching a peak stable BPM of 110.

---

**👤 You:**
> "How has my performance been on 'Moonlight Sonata'?"

**🤖 AI Agent:**
> For 'Moonlight Sonata', you have an average BPM of 60, an average accuracy of 95%, and have spent 45 minutes practicing it.

---

**👤 You:**
> "Show me my daily practice activity for the first week of February."

**🤖 AI Agent:**
> During the first week of February, you practiced on Feb 1st (15 mins, 80 BPM), Feb 3rd (20 mins, 85 BPM), and Feb 5th (10 mins, 82 BPM).


## ❓ FAQ

**Q: How can I see my total practice time for the last month?**
You can use the `get_practice_summary` tool by providing the start and end dates for the last month.

**Q: Can I track how well I am playing a specific song?**
Yes, use `get_piece_performance` with the name of the piece to see average BPM, accuracy, and total time spent.

**Q: How do I find sessions where I played above a certain tempo?**
Use the `search_logs_by_criteria` tool and specify the `minBpm` parameter to filter for those sessions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/metronome-practice-log-summary](https://vinkius.com/en/ai-agent-connect/metronome-practice-log-summary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Metronome Practice Log Summary** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `metronome-practice-log-summary` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Metronome Practice Log Summary** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "metronome-practice-log-summary": {
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
