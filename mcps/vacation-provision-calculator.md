# Vacation Provision Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vacation-provision-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate employee vacation liabilities, including constitutional bonuses and employer taxes.

## Description
This MCP server provides tools to manage the financial and legal risks of employee vacations. Use `calculate_vacation_liability` to determine the total monetary provision (base salary, 1/3 bonus, and taxes) for an individual. Use `check_entitlement_status` to monitor acquisition periods and identify employees in 'warning' or 'expired' status. For large teams, `summarize_workforce_provisions` aggregates total company liability and provides a high-level summary of workforce risk levels.


## Available Tools (3)
- **calculate_vacation_liability**: Calculate vacation provision liability
- **check_entitlement_status**: Check vacation entitlement status
- **summarize_workforce_provisions**: Summarize workforce vacation provisions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vacation Provision Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the vacation provision for an employee with a base salary of $3,000 and a tax rate of 25%."

**🤖 AI Agent:**
> The total vacation provision is $4,000. This includes a base amount of $3,000, a constitutional bonus of $1,000, and employer taxes of $1,000.

---

**👤 You:**
> "Check the status of a vacation period ending on 2024-12-31 with a reference date of 2024-12-15."

**🤖 AI Agent:**
> The employee is in 'warning' status, as the period ends in 16 days.

---

**👤 You:**
> "What is the total liability for an employee with $5,000 salary and 20% tax rate?"

**🤖 AI Agent:**
> $7,000 has been identified as the total provision, consisting of $5,000 base, $1,666.67 bonus, and $333.33 in taxes.


## ❓ FAQ

**Q: How is the vacation provision calculated?**
The calculation includes the employee's base salary, a mandatory 1/3 constitutional bonus, and employer taxes applied to the sum of the salary and bonus.

**Q: What does 'expired' status mean?**
An 'expired' status indicates that the employee's acquisition period has ended, creating a legal and financial risk for the company.

**Q: Can I summarize data for multiple employees at once?**
Yes, use the `summarize_workforce_provisions` tool by providing a JSON array of employee data to get an aggregated view of total liability and risk counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vacation-provision-calculator](https://vinkius.com/mcp/vacation-provision-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vacation Provision Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vacation-provision-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vacation Provision Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vacation-provision-calculator": {
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
