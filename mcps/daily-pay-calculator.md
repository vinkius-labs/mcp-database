# Daily Pay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/daily-pay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate daily earnings, including regular and overtime pay.

## Description
This MCP server provides tools to calculate daily wages based on hourly rates and hours worked. It handles regular pay, overtime pay, and provides a full breakdown of earnings. Use `calculate_total_daily_pay` to get the complete sum of earnings, or `get_pay_summary` for a high-level overview including the effective hourly rate.


## Available Tools (4)
- **calculate_overtime_pay**: Calculates the additional premium compensation earned for exceeding the standard working threshold
- **calculate_regular_pay**: Determines the base earnings for hours worked within the standard threshold
- **calculate_total_daily_pay**: Provides the final combined earnings for a single day, including both regular and overtime pay
- **get_pay_summary**: Generates a high-level overview of daily earnings for reporting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Daily Pay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my total pay for working 10 hours at $25 per hour with an 8 hour threshold and 1.5x overtime."

**🤖 AI Agent:**
> Your total daily pay is $287.50 (Regular: $200.00, Overtime: $87.50).

---

**👤 You:**
> "What is my pay summary for 8 hours at $20 per hour?"

**🤖 AI Agent:**
> Total Pay: $160.00, Regular Pay: $160.00, Overtime Pay: $0.00, Effective Hourly Rate: $20.00.

---

**👤 You:**
> "How much is my overtime pay if I work 12 hours at $30 per hour with an 8 hour threshold and 1.5x multiplier?"

**🤖 AI Agent:**
> Your overtime pay is $180.00.


## ❓ FAQ

**Q: How do I calculate my total earnings for the day?**
You can use the `calculate_total_daily_pay` tool to receive the total amount along with a breakdown of regular and overtime pay.

**Q: Can I specify a different overtime threshold?**
Yes, most tools allow you to provide a `standardThreshold` to define when overtime begins.

**Q: What is the effective hourly rate?**
The effective hourly rate is the total daily pay divided by the total hours worked, which can be found using `get_pay_summary`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/daily-pay-calculator](https://vinkius.com/en/ai-agent-connect/daily-pay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Daily Pay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `daily-pay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Daily Pay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "daily-pay-calculator": {
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
