# Overtime Income Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/overtime-income-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate gross earnings, net take-home pay, and required work hours based on overtime tiers and tax rates.

## Description
The Overtime Income Planner is a precision tool for workers and managers to calculate exact payroll outcomes. It handles complex pay structures including base rates, multiple overtime tiers, and shift differentials. Use `get_payroll_summary` for a complete breakdown of earnings, or `calculate_required_hours` to determine exactly how much you need to work to reach a specific net income goal. This tool accounts for tax rates to ensure your target take-home pay is met accurately.


## Available Tools (4)
- **calculate_required_hours**: Determines how many hours must be worked to reach a specific net income goal
- **get_gross_pay**: Calculates the total gross earnings based on hours worked and pay rates
- **get_net_pay**: Calculates the final take-home amount after taxes
- **get_payroll_summary**: Provides a comprehensive breakdown of a single pay period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Overtime Income Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I take home if I work 40 base hours and 10 overtime hours at $25/hr with a 20% tax rate?"

**🤖 AI Agent:**
> Your total net pay will be $1,200.00.

---

**👤 You:**
> "How many hours do I need to work at $20/hr to take home $1,000 after a 15% tax rate?"

**🤖 AI Agent:**
> You will need to work 5.88 hours.

---

**👤 You:**
> "Give me a summary for 40 base hours, 5 overtime hours at 1.5x, and 2 double time hours at 2.0x, with a $2 shift differential and 25% tax at $30 base rate."

**🤖 AI Agent:**
> Gross Pay: $1,530.00, Tax: $382.50, Net Pay: $1,147.50, Effective Hourly Rate: $27.32.


## ❓ FAQ

**Q: How does the tool handle overtime?**
The tool uses `get_gross_pay` to apply specific multipliers for overtime and double time tiers based on the hours worked.

**Q: Can I calculate how many hours I need to work to reach a specific goal?**
Yes, you can use `calculate_required_hours` to find the total hours needed to achieve your desired net take-home pay.

**Q: Does it include shift differentials?**
Yes, the `get_payroll_summary` tool allows you to include a shift differential that is added to your hourly rates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/overtime-income-planner](https://vinkius.com/en/ai-agent-connect/overtime-income-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Overtime Income Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `overtime-income-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Overtime Income Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "overtime-income-planner": {
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
