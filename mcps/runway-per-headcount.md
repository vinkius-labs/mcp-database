# Runway Per Headcount MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runway-per-headcount)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Simulate the impact of new hires on your company's cash runway and zero-cash date.

## Description
The Runway Per Headcount MCP server provides powerful financial forecasting tools to help you understand how hiring decisions affect your company's survival. Using `calculate_current_burn`, you can determine your current monthly expenditure. With `simulate_hiring_plan`, you can project your runway length and zero-cash date based on specific hiring schedules, including salaries and benefits. Finally, use `compare_hiring_scenarios` to visualize the trade-off between aggressive growth and capital preservation by comparing two different hiring strategies.


## Available Tools (3)
- **simulate_hiring_plan**: Projects the runway length and zero-cash date based on a specific hiring schedule
- **calculate_current_burn**: Determines the current monthly expenditure before any new hires are considered
- **compare_hiring_scenarios**: Compares two different hiring strategies to visualize the trade-off between growth and survival


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runway Per Headcount** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current monthly burn if my fixed costs are $10,000 and I have one employee earning $5,000 with a 1.2 benefits multiplier?"

**🤖 AI Agent:**
> Your total monthly burn is $16,000. This consists of $10,000 in fixed costs and $6,000 in personnel costs ($5,000 salary + $1,000 benefits).

---

**👤 You:**
> "If I start with $500,000 in cash and $20,000 monthly revenue, how long will my runway last if my fixed costs are $30,000 and I hire someone in 3 months at $5,000 salary (1.1 multiplier)?"

**🤖 AI Agent:**
> Your runway will last approximately 42 months. Your zero-cash date is projected to be in 3 years and 6 months.

---

**👤 You:**
> "Compare a scenario where I hire no one vs a scenario where I hire two engineers next month at $8,000 each (1.2 multiplier)."

**🤖 AI Agent:**
> The scenario with no new hires results in a longer runway. The difference is approximately 12 months compared to the aggressive hiring plan.


## ❓ FAQ

**Q: How does the simulation account for new hires?**
The `simulate_hiring_plan` tool calculates costs starting from the specified hire month. Each hire's impact is based on their base salary and benefits multiplier.

**Q: Can I compare two different growth strategies?**
Yes, the `compare_hiring_scenarios` tool allows you to input two separate plans and see which one results in a longer runway and the difference in months.

**Q: What is included in the monthly burn calculation?**
The `calculate_current_burn` tool sums your fixed monthly costs (like rent and software) with the total personnel costs (salaries plus benefits) for all existing staff.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runway-per-headcount](https://vinkius.com/mcp/runway-per-headcount)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runway Per Headcount** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `runway-per-headcount` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runway Per Headcount** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runway-per-headcount": {
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
