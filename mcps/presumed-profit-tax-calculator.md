# Presumed Profit Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/presumed-profit-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate Corporate Income Tax (CIT) and Social Contribution (SCLL) using the Presumed Profit regime.

## Description
This MCP server provides specialized tools for calculating Brazilian corporate taxes under the 'Presumed Profit' regime. It allows AI agents to determine the taxable base by applying activity-specific presumption rates (8%, 16%, or 32%), calculate the breakdown of Corporate Income Tax (CIT) including the monthly surcharge, and compute Social Contribution on Net Profit (SCLL). Using tools like `get_taxable_base`, `calculate_cit_breakdown`, `calculate_scll_liability`, and `generate_tax_summary_report`, agents can automate complex tax estimations for different business activities.


## Available Tools (4)
- **calculate_cit_breakdown**: Calculate the breakdown of Corporate Income Tax (CIT)
- **calculate_scll_liability**: Calculate the Social Contribution on Net Profit (SCLL) liability
- **generate_tax_summary_report**: Generate a complete, consolidated tax summary report
- **get_taxable_base**: Calculate the taxable base based on gross revenue and activity type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Presumed Profit Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tax for a trade company with 100,000 revenue over 2 months."

**🤖 AI Agent:**
> The calculation using `generate_tax_summary_report` shows a taxable base of 8,000 (8% rate), with total CIT and SCLL liabilities calculated accordingly.

---

**👤 You:**
> "What is the taxable base for professional services with 50,000 revenue?"

**🤖 AI Agent:**
> Using `get_taxable_base`, the taxable base is 16,000 (32% rate).

---

**👤 You:**
> "Calculate SCLL for a taxable base of 30,000."

**🤖 AI Agent:**
> The `calculate_scll_liability` tool returns a total SCLL of 2,700 (9% rate).


## ❓ FAQ

**Q: How can I calculate the taxable base for a specific activity?**
You can use the `get_taxable_base` tool by providing the gross revenue and the business activity type.

**Q: Does this server handle the CIT surcharge?**
Yes. The `calculate_cit_breakdown` tool calculates both the standard 15% rate and the 10% surcharge for amounts exceeding the monthly threshold.

**Q: Can I get a full report of all taxes at once?**
Yes, the `generate_tax_summary_report` tool provides a consolidated view including CIT, surcharge, and SCLL.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/presumed-profit-tax-calculator](https://vinkius.com/mcp/presumed-profit-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Presumed Profit Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `presumed-profit-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Presumed Profit Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "presumed-profit-tax-calculator": {
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
