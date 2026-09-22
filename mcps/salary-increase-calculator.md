# Salary Increase Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/salary-increase-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate new salaries and compare percentage increases.

## Description
This MCP server provides tools to calculate salary adjustments. Use `calculate_new_salary` to find a future salary after a raise, `calculate_salary_difference` to compare two amounts, `compare_two_increases` to evaluate different percentage options, or `get_salary_summary` for a full financial breakdown.


## Available Tools (4)
- **calculate_new_salary**: Calculate the new salary after a percentage increase
- **calculate_salary_difference**: Calculate the difference between two salaries
- **compare_two_increases**: Compare two different percentage increases
- **get_salary_summary**: Get a summary of the salary increase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salary Increase Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my new salary be if I earn 50000 and get a 10% increase?"

**🤖 AI Agent:**
> Your new salary will be 55000, with an absolute increase of 5000.

---

**👤 You:**
> "Compare a 5% increase and a 7% increase for a salary of 60000."

**🤖 AI Agent:**
> A 7% increase results in a higher salary of 64200 compared to 63000 from a 5% increase.

---

**👤 You:**
> "Give me a summary for a 45000 salary with a 15% raise."

**🤖 AI Agent:**
> Current Salary: 45000, New Salary: 51750, Absolute Increase: 6750, Percentage Change: 15%.


## ❓ FAQ

**Q: How do I calculate my new salary after a raise?**
You can use the `calculate_new_salary` tool by providing your current salary and the percentage increase you expect.

**Q: Can I compare two different raise offers?**
Yes, the `compare_two_increases` tool allows you to input your current salary and two different percentages to see which results in a higher pay.

**Q: What information is included in the summary?**
The `get_salary_summary` tool provides your current salary, the new salary, the absolute monetary increase, and the percentage change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/salary-increase-calculator](https://vinkius.com/en/ai-agent-connect/salary-increase-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salary Increase Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `salary-increase-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salary Increase Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salary-increase-calculator": {
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
