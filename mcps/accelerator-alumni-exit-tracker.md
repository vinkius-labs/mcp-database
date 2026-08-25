# Accelerator Alumni Exit Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-alumni-exit-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze alumni performance metrics, exit rates, and exit type distributions for accelerator cohorts.

## Description
This MCP server provides specialized tools for accelerator programs to monitor and analyze the realized performance of their alumni companies. It tracks key liquidity events such as Acquisitions and IPOs, while also accounting for shutdowns. By using tools like `get_exit_summary`, `get_exit_distribution`, and `get_exit_type_breakdown`, managers can calculate exit rates, average exit values, and the velocity of exits within specific cohorts. The engine accounts for equity dilution from follow-on rounds to provide accurate realized value calculations.


## Available Tools (3)
- **get_exit_distribution**: g., Acquisition, IPO, etc.)

Provides the distribution of exit types for a specific accelerator cohort
- **get_exit_summary**: Provides high-level performance metrics for a specific accelerator cohort
- **get_exit_type_breakdown**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Alumni Exit Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the performance summary for cohort '2021-spring'?"

**🤖 AI Agent:**
> For the 2021-spring cohort, the exit rate is 45%, the average exit value is $12,500,000, and the total realized value is $5,625,000.

---

**👤 You:**
> "Show me the breakdown of exit types for cohort 'alpha-v1'."

**🤖 AI Agent:**
> Cohort 'alpha-v1' has 5 Acquisitions, 1 IPO, and 2 Shutdowns, resulting in a success rate of 83.3%.

---

**👤 You:**
> "How are exits distributed over time for cohort 'beta-2022'?"

**🤖 AI Agent:**
> In cohort 'beta-2022', 2 exits occurred within 1-3 years, and 3 exits occurred within the 3-5 year range.


## ❓ FAQ

**Q: How does the tool handle equity dilution?**
The engine calculates realized value by applying the final, diluted equity percentage held at the time of exit, accounting for all follow-on funding rounds.

**Q: What metrics can I get for a specific cohort?**
You can use `get_exit_summary` to retrieve the exit rate, average exit value, and total realized value for any given cohort ID.

**Q: Can I see the timing of exits?**
Yes, the `get_exit_distribution` tool allows you to analyze the velocity of exits by grouping them into custom time buckets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-alumni-exit-tracker](https://vinkius.com/ai-agent-connect/accelerator-alumni-exit-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Alumni Exit Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-alumni-exit-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Alumni Exit Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-alumni-exit-tracker": {
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
