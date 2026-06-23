# Simples Nacional Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simples-nacional-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate effective tax rates, Fator R eligibility, and monthly DAS amounts for the Brazilian Simples Nacional regime.

## Description
This MCP server provides a precise calculation engine for the Brazilian Simples Nacional taxation system. It allows AI agents to determine complex tax variables by accessing tools like `get_bracket_parameters`, `calculate_effective_rate`, `evaluate_factor_r`, and `compute_monthly_tax_amount`. The server handles progressive revenue tiers across Annexes I through V, calculating the dynamic effective rate based on accumulated revenue (RBT12) and fixed deductions. It also evaluates Fator R eligibility by comparing payroll expenses to gross revenue, enabling accurate estimation of monthly tax liabilities (DAS).


## Available Tools (4)
- **calculate_effective_rate**: Calculate the dynamic effective tax rate
- **compute_monthly_tax_amount**: Calculate the final tax amount due
- **evaluate_factor_r**: Check eligibility for Annex III via Fator R
- **get_bracket_parameters**: Retrieve taxation constants based on activity and revenue


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Simples Nacional Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the effective tax rate for a company with 200,000 BRL accumulated revenue in Annex I, using a nominal rate of 4% and deduction of 0."

**🤖 AI Agent:**
> The effective tax rate is 4.0%.

---

**👤 You:**
> "Check if a company with 100,000 BRL revenue and 30,000 BRL payroll qualifies for Fator R."

**🤖 AI Agent:**
> The company is eligible for the lower taxation tier (Annex III) because the payroll-to-revenue ratio is 30%.

---

**👤 You:**
> "How much tax will I pay this month if my revenue is 5,000 BRL and my effective rate is 6%?"

**🤖 AI Agent:**
> The total tax due (DAS) for this month is 300.00 BRL.


## ❓ FAQ

**Q: How can I find the tax rate for my business activity?**
You can use the `get_bracket_parameters` tool. Provide your accumulated revenue from the last 12 months and the specific Annex type (e.g., Annex I for commerce) to retrieve the nominal rate and deduction amount.

**Q: What is Fator R and how does it affect my taxes?**
Fator R is a rule for certain service activities. By using `evaluate_factor_r`, you can check if your payroll costs relative to revenue allow you to move from Annex V to the more favorable Annex III.

**Q: Can I calculate the exact amount of DAS to pay?**
Yes. After determining your effective rate, use `compute_monthly_tax_amount` with your current month's revenue to get the final currency value of your tax liability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simples-nacional-calculator](https://vinkius.com/mcp/simples-nacional-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Simples Nacional Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simples-nacional-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Simples Nacional Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simples-nacional-calculator": {
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
