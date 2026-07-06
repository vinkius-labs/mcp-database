# Home Affordability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/home-affordability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate your maximum home purchase price and verify mortgage DTI compliance.

## Description
The Home Affordability Calculator connects AI agents to precise financial modeling for real estate. Using tools like `calculate_housing_costs` and `validate_dti`, you can determine the total monthly impact of PITI+H (Principal, Interest, Taxes, Insurance, and HOA) and ensure your mortgage scenario meets lender standards for front-end and back-end Debt-to-Income (DTI) ratios. It accounts for complex variables like PMI (Private Mortgage Insurance) based on down payment levels and compares 15-year vs 30-year loan terms to help you plan your next property purchase.


## Available Tools (2)
- **validate_dti**: Validate Debt-to-Income ratio
- **calculate_housing_costs**: Calculate monthly housing expenses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Affordability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will my total monthly housing expenses be for a $500,000 home with a 10% down payment at a 6.5% interest rate?"

**🤖 AI Agent:**
> Your total monthly housing expense will be $3,452.50, which includes $2,528.31 for principal and interest, plus taxes, insurance, and an estimated $120 in PMI.

---

**👤 You:**
> "Can I afford a $450,000 home if my gross monthly income is $8,000 and I have $500 in monthly car loan payments?"

**🤖 AI Agent:**
> Based on a 36% back-end DTI limit, your maximum allowable total debt is $2,880. With your current car loan, your housing costs must stay below $2,380 to remain compliant.

---

**👤 You:**
> "Calculate the monthly cost for a 15-year mortgage on a $350,000 property with 20% down at 5.5%."

**🤖 AI Agent:**
> The monthly principal and interest payment is $2,851.43. Including taxes and insurance, your total monthly housing cost is estimated at $3,210.00.


## ❓ FAQ

**Q: How does the calculator determine my maximum home price?**
It uses your gross monthly income and existing debts to solve for the highest property value that satisfies both front-end and back-end DTI limits.

**Q: Does this tool account for PMI?**
Yes, if your down payment percentage is below the required threshold, the calculator automatically includes the monthly Private Mortgage Insurance cost in your total housing expenses.

**Q: What DTI ratios are used for validation?**
By default, it checks against the standard 28% front-end and 36% back-end DTI limits, but these can be customized for specific lender requirements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/home-affordability-calculator](https://vinkius.com/mcp/home-affordability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Affordability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-affordability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Affordability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-affordability-calculator": {
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
