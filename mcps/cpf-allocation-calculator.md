# CPF Allocation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cpf-allocation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact CPF contributions and account allocations for Singapore Citizens and PRs.

## Description
This MCP server provides precise calculations for Central Provident Fund (CPF) contributions in Singapore. It determines the exact monetary breakdown of employee and employer contributions and calculates how funds are distributed into the Ordinary Account (OA), Special Account (SA), and Medisave Account (MA) based on regulatory age brackets. Use `calculate_monthly_contributions` to get a full breakdown or `get_contribution_rates` to find specific percentage rates for a given age.


## Available Tools (3)
- **calculate_monthly_contributions**: Calculate exact monetary breakdown of CPF contributions and account allocations
- **get_account_allocation_ratios**: Retrieve the percentage distribution for the OA, SA, and MA accounts for a given age
- **get_contribution_rates**: Retrieve specific percentage rates for employees and employers based on age and residency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CPF Allocation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the CPF contribution for a 30-year-old Singapore Citizen earning 5000 SGD monthly."

**🤖 AI Agent:**
> For a 30-year-old Singapore Citizen earning 5000 SGD, the employee contribution is 1000 SGD and the employer contribution is 850 SGD. The total contribution is 1850 SGD, distributed into OA, SA, and MA based on the age-specific ratios.

---

**👤 You:**
> "What are the CPF contribution rates for a 55-year-old PR?"

**🤖 AI Agent:**
> For a 55-year-old Permanent Resident, the employee contribution rate is 20% and the employer contribution rate is 17%.

---

**👤 You:**
> "How much goes to the Medisave account for a 40-year-old earning 6800 SGD?"

**🤖 AI Agent:**
> At a monthly salary of 6800 SGD for a 40-year-old, the Medisave (MA) allocation is calculated based on the fixed percentage for that age bracket applied to the total contribution.


## ❓ FAQ

**Q: How does the Ordinary Wage (OW) ceiling affect my calculation?**
The tool automatically applies the current Ordinary Wage (OW) ceiling. Any salary earned above this limit is not included in the CPF contribution calculation.

**Q: Does this tool support non-Singapore Citizens or PRs?**
The current version of this tool is specifically designed for Singapore Citizens and Permanent Residents (PRs).

**Q: Can I see the specific percentage rates for my age group?**
Yes, you can use the `get_contribution_rates` tool to retrieve the specific employee and employer percentage rates for your age and residency status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cpf-allocation-calculator](https://vinkius.com/ai-agent-connect/cpf-allocation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CPF Allocation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cpf-allocation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CPF Allocation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cpf-allocation-calculator": {
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
