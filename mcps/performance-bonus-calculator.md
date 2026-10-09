# Performance Bonus Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/performance-bonus-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate professional performance-based bonus payouts including achievement scaling and tax withholding.

## Description
This MCP server provides a suite of tools to calculate professional performance-based bonus payouts. It handles the entire lifecycle from determining the gross bonus using `calculate_gross_bonus` to calculating the final net amount with `calculate_net_bonus`. Users can also use `validate_performance_metrics` to ensure achievement scores are within corporate bounds or `get_bonus_summary` for a complete breakdown of the payout, including tax deductions and cap applications.


## Available Tools (4)
- **calculate_gross_bonus**: Determine the total bonus amount earned before any tax deductions are applied
- **calculate_net_bonus**: Determine the actual amount an employee receives after tax deductions
- **get_bonus_summary**: Provide a complete breakdown of the bonus lifecycle from base salary to net payout
- **validate_performance_metrics**: Verify if the provided achievement and multiplier values are within acceptable corporate bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Performance Bonus Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the gross bonus for a salary of 100,000 with a 10% target and 1.2 achievement score."

**🤖 AI Agent:**
> The gross bonus is 12,000.

---

**👤 You:**
> "What is the net bonus for a 5,000 gross bonus with a 20% tax rate?"

**🤖 AI Agent:**
> The net bonus is 4,000 and the tax amount is 1,000.

---

**👤 You:**
> "Give me a summary for a 120,000 salary, 15% target, 1.0 achievement, and 25% tax rate."

**🤖 AI Agent:**
> The gross bonus is 18,000, the tax amount is 4,500, and the net bonus is 13,500.


## ❓ FAQ

**Q: How do I calculate the final amount an employee receives?**
You can use `calculate_net_bonus` to find the final amount after taxes, or use `get_bonus_summary` to see the full breakdown from base salary to net payout.

**Q: Can I apply a maximum limit to the bonus?**
Yes, the `calculate_gross_bonus` tool allows you to specify a `bonusCap` to ensure the payout does not exceed a certain threshold.

**Q: How are achievement scores handled?**
The achievement score scales the target bonus. You can use `validate_performance_metrics` to verify if a score is within the acceptable corporate range.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/performance-bonus-calculator](https://vinkius.com/en/ai-agent-connect/performance-bonus-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Performance Bonus Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `performance-bonus-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Performance Bonus Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "performance-bonus-calculator": {
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
