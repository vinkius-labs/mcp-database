# Employee Option Pool Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/employee-option-pool-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate optimal equity option pool sizes for future hiring plans.

## Description
This MCP server provides specialized tools to help companies plan their equity needs. Use `calculate_pool_requirement` to determine the total equity needed for upcoming hires, `simulate_dilution` to understand the impact on current shareholders, `project_grant_allocation` to see how equity is distributed across cohorts, and `estimate_attrition_buffer` to adjust for expected employee departures.


## Available Tools (4)
- **calculate_pool_requirement**: Determines the total percentage of equity needed for the upcoming hiring plan
- **estimate_attrition_buffer**: Adjusts the required pool size by accounting for expected employee departures
- **project_grant_allocation**: Breaks down how much equity is allocated to different hiring cohorts
- **simulate_dilution**: Calculates how much existing shareholders will be diluted by the new option pool


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Employee Option Pool Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required option pool for 10 current employees with 5 planned hires at 0.5% grant each over 6 months."

**🤖 AI Agent:**
> The total required pool size is 2.5% based on your hiring plan.

---

**👤 You:**
> "What will be the dilution if I create a 10% option pool and I currently own 80%?"

**🤖 AI Agent:**
> Your post-dilution ownership will be 72.73%.

---

**👤 You:**
> "Show me the equity breakdown for a hiring plan with 2 Junior hires at 0.1% and 1 Senior hire at 0.5%."

**🤖 AI Agent:**
> The total allocated equity is 0.7%, with 0.2% for the Junior cohort and 0.5% for the Senior cohort.


## ❓ FAQ

**Q: How do I calculate the total pool size needed?**
You can use the `calculate_pool_requirement` tool by providing your current headcount, a list of planned hires with their grant percentages, and your recruiting timeline.

**Q: Can I account for employee departures?**
Yes, the `estimate_attrition_buffer` tool allows you to adjust your required pool size by factoring in expected attrition rates over your hiring period.

**Q: How is dilution calculated?**
The `simulate_dilution` tool calculates the reduction in ownership for existing shareholders by comparing current ownership against the new total equity including the pool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/employee-option-pool-calculator](https://vinkius.com/en/ai-agent-connect/employee-option-pool-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Employee Option Pool Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `employee-option-pool-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Employee Option Pool Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "employee-option-pool-calculator": {
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
