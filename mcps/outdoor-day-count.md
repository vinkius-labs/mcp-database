# Outdoor Day Count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/outdoor-day-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify your outdoor engagement by analyzing activity date logs.

## Description
This MCP server provides tools to analyze chronological logs of outdoor activities. It helps you understand your engagement patterns through unique day counts, date range analysis, monthly frequency breakdowns, and consecutive activity streaks. Use `get_total_outdoor_days` to find your total unique active days, `get_outdoor_days_in_range` for specific periods, `get_activity_frequency_by_month` to identify peak activity months, and `get_activity_streak` to track your longest consecutive runs of outdoor time.


## Available Tools (4)
- **get_activity_frequency_by_month**: Answers in which months outdoor activity was highest
- **get_activity_streak**: Answers the longest consecutive streak of outdoor activity days
- **get_outdoor_days_in_range**: Answers how many days were spent outdoors between two specific dates
- **get_total_outdoor_days**: Answers how many unique days were spent outdoors in total


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Outdoor Day Count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many unique days was I outdoors in total based on these dates: ['2023-05-01', '2023-05-01', '2023-05-02']?"

**🤖 AI Agent:**
> You were outdoors for a total of 2 unique days.

---

**👤 You:**
> "What is my longest outdoor activity streak for these dates: ['2023-06-01', '2023-06-02', '2023-06-03', '2023-06-05']?"

**🤖 AI Agent:**
> Your longest consecutive streak is 3 days.

---

**👤 You:**
> "How many days was I outdoors between 2023-01-01 and 2023-01-10 given these dates: ['2023-01-01', '2023-01-05', '2023-01-15']?"

**🤖 AI Agent:**
> You were outdoors for 2 days within that range.


## ❓ FAQ

**Q: How does the tool handle multiple activities on the same day?**
The tools count unique calendar days. If you record multiple activities on the same date, it only counts as one unique day of outdoor activity.

**Q: What date format should I use?**
All dates must be provided in ISO 8601 format (e.g., YYYY-MM-DD).

**Q: Can I check my activity for a specific month?**
Yes, you can use `get_activity_frequency_by_month` to see how many unique days you were active in each month for a given year.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/outdoor-day-count](https://vinkius.com/en/ai-agent-connect/outdoor-day-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Outdoor Day Count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `outdoor-day-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Outdoor Day Count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "outdoor-day-count": {
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
