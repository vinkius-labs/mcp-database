# Vesting Schedule Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/vesting-schedule-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate equity vesting timelines, cliff impacts, and acceleration outcomes.

## Description
This MCP server provides a computational engine for determining equity vesting timelines, cliff thresholds, and acceleration event outcomes. It allows AI agents to model complex equity scenarios using tools like `get_monthly_vesting_schedule` for month-by-month breakdowns, `calculate_cliff_impact` for threshold analysis, `calculate_acceleration_outcome` for simulating change-in-control events, and `get_vesting_status_summary` for high-level equity standing.


## Available Tools (4)
- **calculate_acceleration_outcome**: Calculates how many shares vest immediately when acceleration triggers are met
- **calculate_cliff_impact**: Determines the specific volume of shares that vest exactly at the cliff threshold
- **get_monthly_vesting_schedule**: Provides a month-by-month breakdown of how many shares vest over the entire term
- **get_vesting_status_summary**: Provides a high-level summary of an individual's current equity standing at a specific point in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vesting Schedule Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the monthly vesting schedule for 1200 shares over 48 months with a 12-month cliff."

**🤖 AI Agent:**
> The schedule shows 0 shares vested for the first 11 months. At month 12 (the cliff), 300 shares vest. Thereafter, 25 shares vest each month until month 48.

---

**👤 You:**
> "What is my current vesting status for 5000 shares, 36 month period, 6 month cliff, after 10 months?"

**🤖 AI Agent:**
> You have 0 shares vested. You are currently in the PRE_CLIFF stage and have 5000 unvested shares remaining.

---

**👤 You:**
> "Calculate the outcome of a single trigger acceleration for 1000 total shares if 400 are already vested and 50% of unvested shares accelerate."

**🤖 AI Agent:**
> With a single trigger event, 300 additional shares will accelerate, bringing your total vested shares to 700.


## ❓ FAQ

**Q: How do I calculate the impact of a cliff?**
You can use the `calculate_cliff_impact` tool to determine the specific volume of shares that vest exactly at the cliff threshold.

**Q: Can I simulate a double trigger acceleration event?**
Yes, use the `calculate_acceleration_outcome` tool and set the acceleration type to 'double' to simulate scenarios involving both a corporate event and a qualifying secondary event.

**Q: How can I see a full breakdown of my vesting over time?**
The `get_monthly_vesting_schedule` tool provides a complete month-by-month breakdown of how many shares vest over the entire term.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/vesting-schedule-engine](https://vinkius.com/en/ai-agent-connect/vesting-schedule-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vesting Schedule Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vesting-schedule-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vesting Schedule Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vesting-schedule-engine": {
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
