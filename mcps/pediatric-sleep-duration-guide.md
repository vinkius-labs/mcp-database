# Pediatric Sleep Duration Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pediatric-sleep-duration-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Precision sleep recommendations for children based on AAP guidelines.

## Description
This MCP server provides precise sleep guidance for children using American Academy of Pediatrics (AAP) standards. It calculates total sleep budgets, nap schedules, and ideal bedtimes by analyzing age, developmental stage, and physical activity levels. Use `get_sleep_recommendations` to find core sleep targets, `calculate_nap_schedule` to plan daytime rest, `plan_bedtime` to determine optimal sleep onset, and `get_sleep_budget_summary` for a complete 24-hour overview.


## Available Tools (4)
- **calculate_nap_schedule**: Determine if and when a child should nap
- **get_sleep_budget_summary**: Provide a high-level overview of 24-hour sleep requirements
- **get_sleep_recommendations**: Provide core sleep targets for a child based on age and activity level
- **plan_bedtime**: Calculate the ideal bedtime to meet sleep targets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pediatric Sleep Duration Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the sleep recommendations for a 12-month-old with high activity?"

**🤖 AI Agent:**
> A 12-month-old with high activity requires approximately 13 to 14 hours of total sleep per day.

---

**👤 You:**
> "Help me plan a bedtime for a toddler who needs 12 hours of sleep and wakes up at 07:00."

**🤖 AI Agent:**
> To wake up at 07:00 with 12 hours of sleep, the suggested bedtime is 18:45, with a target asleep time of 19:00.

---

**👤 You:**
> "Does a 24-month-old need naps?"

**🤖 AI Agent:**
> Yes, a 24-month-old typically requires one or more naps to meet their total sleep budget.


## ❓ FAQ

**Q: What standards does this tool follow?**
The tool follows the clinical sleep guidelines established by the American Academy of Pediatrics (AAP).

**Q: How does activity level affect the results?**
Higher physical activity increases the total sleep budget required to support physical recovery.

**Q: Can I use this to plan a daily schedule?**
Yes, you can use `calculate_nap_schedule` and `plan_bedtime` to build a complete daily rest plan.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pediatric-sleep-duration-guide](https://vinkius.com/en/ai-agent-connect/pediatric-sleep-duration-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pediatric Sleep Duration Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pediatric-sleep-duration-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pediatric Sleep Duration Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pediatric-sleep-duration-guide": {
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
