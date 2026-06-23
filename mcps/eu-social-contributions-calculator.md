# EU Social Contributions Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eu-social-contributions-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate employee and employer social security contributions for France, Germany, Spain, Italy, and Portugal.

## Description
This MCP server provides a precise calculation engine for estimating payroll-related social taxes across selected European economies. Using tools like `calculate_contribution_breakdown`, you can determine the exact monetary split between employee deductions and employer overheads for branches such as Health, Pension, and Unemployment. The server also allows for comparing tax burdens between different nations using `compare_tax_burden` to understand the total cost of employment in countries like France (FR), Germany (DE), Spain (ES), Italy (IT), and Portugal (PT).


## Available Tools (3)
- **calculate_contribution_breakdown**: Calculates the specific monetary amounts for both employee and employer portions across all branches
- **compare_tax_burden**: Compares the total social security overhead between two different countries for the same salary
- **get_country_rates**: Retrieves the raw percentage rates for all social security branches within a specific country


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EU Social Contributions Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the social security rates for Germany?"

**🤖 AI Agent:**
> For Germany (DE), the rates are: Health (Employee: 7.3%, Employer: 7.3%), Pension (Employee: 9.3%, Employer: 9.3%), and Unemployment (Employee: 1.4%, Employer: 1.4%).

---

**👤 You:**
> "Calculate the breakdown for a €3,000 salary in France."

**🤖 AI Agent:**
> For a €3,000 salary in France (FR), the total employer contribution is €XXX and the employee deduction is €XXX, covering Health, Pension, and Unemployment branches.

---

**👤 You:**
> "Compare the tax burden of Spain vs Italy for a €5,000 salary."

**🤖 AI Agent:**
> The total social security burden in Spain (ES) is €XXX, while in Italy (IT) it is €XXX, resulting in a difference of €XXX.


## ❓ FAQ

**Q: Which countries are supported?**
The calculator currently supports France (FR), Germany (DE), Spain (ES), Italy (IT), and Portugal (PT).

**Q: How can I see the specific tax rates for a country?**
You can use the `get_country_rates` tool by providing the ISO alpha-2 country code to retrieve the percentage rates for Health, Pension, and Unemployment branches.

**Q: Can I compare the cost of hiring in two different countries?**
Yes, use the `compare_tax_burden` tool. By providing a salary amount and two country codes, you can see the difference in total social security overhead between them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eu-social-contributions-calculator](https://vinkius.com/mcp/eu-social-contributions-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EU Social Contributions Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eu-social-contributions-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EU Social Contributions Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eu-social-contributions-calculator": {
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
