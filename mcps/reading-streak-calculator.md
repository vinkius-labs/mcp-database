# Reading Streak Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reading-streak-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze reading patterns by calculating current and longest consecutive day streaks.

## Description
This MCP server provides tools to analyze reading consistency and patterns. Use `calculate_streaks` to find your current ongoing streak and your all-time longest streak from a list of reading dates. You can also use `get_streak_gap_analysis` to identify specific breaks in your reading history, `validate_date_consistency` to check for duplicate entries, and `get_streak_metadata` to view activity density and total days read. It is designed to help readers track their progress and maintain reading habits.


## Available Tools (4)
- **calculate_streaks**: Calculates the current ongoing streak and the all-time highest streak from a history of reading dates
- **get_streak_gap_analysis**: Identifies the specific breaks or gaps in a reading history
- **get_streak_metadata**: Provides summary statistics about the frequency and distribution of reading days
- **validate_date_consistency**: Ensures the provided list of dates contains no duplicate entries and follows chronological logic


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reading Streak Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my reading streaks for these dates: 2024-05-01, 2024-05-02, 2024-05-03, 2024-05-05."

**🤖 AI Agent:**
> Your current streak is 1 day and your longest streak is 3 days.

---

**👤 You:**
> "How many gaps are in my reading history for: 2024-01-01, 2024-01-02, 2024-01-04, 2024-01-05?"

**🤖 AI Agent:**
> There is 1 gap in your reading history, with a gap length of 1 day.

---

**👤 You:**
> "Check if these reading dates are consistent: 2024-06-01, 2024-06-01, 2024-06-02."

**🤖 AI Agent:**
> The dates are not consistent. There is 1 duplicate entry found.


## ❓ FAQ

**Q: How is the current streak calculated?**
The current streak is active if your most recent reading date is either today or yesterday. If there is a gap of more than one day, the current streak is reset to zero.

**Q: What format should the dates be in?**
All dates must be provided as ISO 8601 strings in the format YYYY-MM-DD.

**Q: Can I see where I missed reading days?**
Yes, you can use the `get_streak_gap_analysis` tool to identify the number of breaks and the length of each gap in your reading history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reading-streak-calculator](https://vinkius.com/en/ai-agent-connect/reading-streak-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reading Streak Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reading-streak-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reading Streak Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reading-streak-calculator": {
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
