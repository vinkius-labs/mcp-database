# Shift Swap Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shift-swap-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Matches requested shift swaps using employee availability, skills, and labor limits.

## Description
Shift Swap Planner manages the exchange of work shifts between employees. It ensures operational continuity by checking employee availability, skill matching, and labor constraints. Use `find_eligible_recipients` to identify potential candidates for a shift, `validate_swap_constraints` to ensure the swap follows labor rules, and `evaluate_approval_policy` to see if a manager needs to intervene. You can also use `get_employee_workload` to check an employee's remaining capacity.


## Available Tools (4)
- **get_employee_workload**: Provides a summary of an employee's current assigned hours and upcoming availability
- **validate_swap_constraints**: Checks if a proposed swap between two specific employees violates any labor or availability rules
- **evaluate_approval_policy**: Determines if a validated swap requires manual manager approval based on organizational rules
- **find_eligible_recipients**: Identifies which employees are capable of taking over a specific requested shift


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shift Swap Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who is eligible to take shift SHIFT-123?"

**🤖 AI Agent:**
> The following employees are eligible for shift SHIFT-123: John Doe (Match Score: 0.95) and Jane Smith (Match Score: 0.88).

---

**👤 You:**
> "Is it okay for employee EMP-001 to swap shift SHIFT-456 with EMP-002?"

**🤖 AI Agent:**
> The swap is valid and meets all labor constraints and availability requirements.

---

**👤 You:**
> "Does the swap for SHIFT-789 require manager approval?"

**🤖 AI Agent:**
> This swap requires manual manager approval because the recipient will reach their maximum weekly hour threshold.


## ❓ FAQ

**Q: How do I find someone to take my shift?**
You can use the `find_eligible_recipients` tool by providing the specific shift ID to see a list of qualified employees.

**Q: Will my shift swap be automatically approved?**
It depends on the organizational rules. Use `evaluate_approval_policy` to determine if the swap is auto-approved or requires manager intervention.

**Q: How can I check if an employee has enough hours left for a shift?**
Use the `get_employee_workload` tool to view an employee's total hours worked this week and their remaining allowed hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shift-swap-planner](https://vinkius.com/en/ai-agent-connect/shift-swap-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shift Swap Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shift-swap-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shift Swap Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shift-swap-planner": {
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
