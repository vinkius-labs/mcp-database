# Spain IRPF Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/spain-irpf-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Spanish Personal Income Tax (IRPF) liabilities, including taxable base determination and regional tax application.

## Description
This MCP server provides a specialized engine for calculating Spanish Personal Income Tax (IRPF) liabilities. It allows AI agents to determine taxable bases by separating general and savings income, calculate the state tax quota using progressive national brackets, and apply regional tax modifiers for different Autonomous Communities. Additionally, it calculates personal and family reductions based on age, dependents, and disability degree to find the final net tax liability. Use tools like `calculate_taxable_bases`, `compute_state_quota`, and `compute_regional_tax` to perform precise tax computations.


## Available Tools (5)
- **calculate_personal_reductions**: Calculates the total amount of tax relief available based on the taxpayer's personal circumstances
- **compute_state_quota**: Calculates the portion of tax owed specifically to the Spanish State
- **calculate_taxable_bases**: Results cannot be less than zero.

Determines the remaining taxable amounts for both General and Savings pools after accounting for deductions
- **compute_regional_tax**: Calculates the additional tax liability imposed by a specific Autonomous Community
- **get_final_tax_determination**: Net cannot be negative.

Consolidates all previous calculations to find the total gross and net tax liabilities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spain IRPF Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the taxable bases for a gross general income of 30,000 and savings income of 5,000, with 2,000 in general deductions and 500 in savings deductions."

**🤖 AI Agent:**
> The taxable general base is 28,000 and the taxable savings base is 4,500.

---

**👤 You:**
> "What is the state tax liability for a taxable general base of 25,000?"

**🤖 AI Agent:**
> The calculated state tax liability for a taxable general base of 25,000 is 4,250.

---

**👤 You:**
> "Calculate the final tax determination if state liability is 4,000, regional liability is 500, total reductions are 1,200, and taxable general base is 25,000."

**🤖 AI Agent:**
> The gross tax liability is 4,500 and the net tax liability is 3,300.


## ❓ FAQ

**Q: How does the taxable base calculation work?**
The `calculate_taxable_bases` tool takes your gross general and savings income and subtracts any provided deductions. The resulting amounts represent the taxable bases for each category, ensuring neither falls below zero.

**Q: Can I calculate regional taxes for specific Spanish communities?**
Yes. By using the `compute_regional_tax` tool with a valid `regionCode` (such as 'MAD' for Madrid or 'CAT' for Catalonia), you can calculate the additional tax liability imposed by that specific Autonomous Community.

**Q: Does the tool account for personal and family reductions?**
Yes, the `calculate_personal_reductions` tool calculates tax relief based on the taxpayer's age, number of dependents, and degree of disability to help determine the final net tax liability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/spain-irpf-calculator](https://vinkius.com/mcp/spain-irpf-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spain IRPF Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spain-irpf-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spain IRPF Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spain-irpf-calculator": {
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
