# US Quarterly Tax Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-quarterly-tax-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate exact US federal quarterly estimated tax payments and deadlines using Safe Harbor rules.

## Description
This MCP server provides AI agents with the tools to calculate precise US federal quarterly estimated tax payments (Form 1040-ES). By inputting projected annual income and prior year tax liability, agents can use `estimate_quarterly_payments` to generate a complete schedule of four payment amounts and their respective deadlines. Additionally, the `evaluate_safe_harbor_compliance` tool allows for checking if current withholdings meet the 90% or 110% Safe Harbor thresholds, while `calculate_marginal_tax_bracket` identifies applicable tax rates based on income levels.


## Available Tools (3)
- **evaluate_safe_harbor_compliance**: Check if current tax payments meet Safe Harbor requirements
- **estimate_quarterly_payments**: Calculate required US quarterly tax payments
- **calculate_marginal_tax_bracket**: Calculate the marginal tax rate for a given income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Quarterly Tax Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my quarterly tax payments for an annual income of $100,000 and a prior year tax of $15,000."

**🤖 AI Agent:**
> Based on your inputs, the `estimate_quarterly_payments` tool has calculated your four installments. Each payment is due on April 15, June 15, September 15, and January 15, with specific amounts distributed to satisfy Safe Harbor requirements.

---

**👤 You:**
> "What is my marginal tax rate if I earn $80,000?"

**🤖 AI Agent:**
> The `calculate_marginal_tax_bracket` tool identifies your top federal tax bracket and the corresponding percentage rate for an income of $80,000.

---

**👤 You:**
> "Am I compliant with Safe Harbor if I've paid $5,000 so far this year?"

**🤖 AI Agent:**
> By using `evaluate_safe_harbor_compliance`, the system checks your $5,000 payment against the 90% current year or 100%/110% prior year threshold to determine if you are at risk of underpayment penalties.


## ❓ FAQ

**Q: How can I find my quarterly payment deadlines?**
Use the `estimate_quarterly_payments` tool. It returns a list of all four quarterly deadlines along with the specific amount due for each period.

**Q: What is the Safe Harbor rule?**
The Safe Harbor rule allows you to avoid underpayment penalties by paying either 90% of your current year's tax or 100% (or 110% for high earners) of your prior year's tax.

**Q: Can I check if my current payments are enough to avoid penalties?**
Yes. The `evaluate_safe_harbor_compliance` tool compares your total paid to date against the required Safe Harbor thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-quarterly-tax-estimator](https://vinkius.com/mcp/us-quarterly-tax-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Quarterly Tax Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-quarterly-tax-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Quarterly Tax Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-quarterly-tax-estimator": {
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
