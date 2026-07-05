# Overtime Pay Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/overtime-pay-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US overtime pay based on FLSA and state-specific rules like CA/CO daily thresholds.

## Description
The Overtime Pay Calculator is a specialized engine designed to handle the complexities of US labor laws. It provides precise calculations for federal FLSA standards, as well as state-specific daily overtime thresholds found in jurisdictions like California and Colorado. Use `calculate_weekly_overtime` to determine pay based on the 40-hour weekly threshold, or `calculate_daily_overtime` to check for daily violations. The tool also handles complex regular rate compositions using `calculate_adjusted_regular_rate`, incorporating non-discentionary bonuses and commissions into the weighted average. Additionally, you can use `evaluate_exemption_eligibility` to analyze whether an employee meets the salary and duties requirements for exempt status.


## Available Tools (4)
- **calculate_adjusted_regular_rate**: Calculates the true "Regular Rate of Pay" by incorporating non-discretionary bonuses
- **calculate_daily_overtime**: g., CA/CO 8-hour rule) and calculates excess pay.

Calculates overtime owed for daily shifts that exceed state-mandated thresholds
- **evaluate_exemption_eligibility**: Determines if an e mployee qualifies as "Exempt" from overtime
- **calculate_weekly_overtime**: Determines overtime pay based on the federal 40-hour weekly threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Overtime Pay Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate overtime pay for 45 hours worked at $20/hour."

**🤖 AI Agent:**
> Regular pay: $800.00, Overtime pay: $150.00.

---

**👤 You:**
> "Is an employee earning $60,000/year in an Executive role exempt?"

**🤖 AI Agent:**
> Yes, the employee meets the salary and duties requirements for exemption.

---

**👤 You:**
> "Calculate daily overtime in CA for a shift of 10 hours at $25/hour."

**🤖 AI Agent:**
> Daily overtime pay: $50.00 (based on the 8-hour threshold in CA).


## ❓ FAQ

**Q: How does the tool handle California overtime?**
By using the `calculate_daily_overtime` tool with the state code 'CA', the engine applies the 8-hour daily threshold rule specific to California.

**Q: Does it include bonuses in the overtime rate?**
Yes, you can use `calculate_adjusted_regular_rate` to incorporate non-discretionary earnings like commissions and production bonuses into the calculation.

**Q: Can I check if an employee is exempt?**
Yes, the `evaluate_exemption_eligibility` tool analyzes annual salary and job duties to determine if an employee qualifies for exemption.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/overtime-pay-calculator](https://vinkius.com/mcp/overtime-pay-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Overtime Pay Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `overtime-pay-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Overtime Pay Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "overtime-pay-calculator": {
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
