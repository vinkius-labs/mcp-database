# Change Order Impact Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/change-order-impact-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the financial and schedule consequences of scope changes in construction projects.

## Description
This MCP server provides essential tools for construction and project managers to manage scope creep. Use `calculate_change_order_prce` to determine the total price impact of a single change by applying overhead and profit margins to direct costs. With `calculate_cumulative_impact`, you can track how multiple changes affect the overall contract value and project timeline. Additionally, use `assess_project_risk_level` to identify if scope drift has pushed your project into high-risk territory based on cumulative change order volume.


## Available Tools
- **assess_project_risk_level**: Categorizes the financial health of the project based on scope drift
- **calculate_change_order_price**: Determines the total price charged to the client for a single specific scope change
- **calculate_cumulative_impact**: Calculates the total financial and schedule impact on a project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Change Order Impact Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the price for a change order with $5000 direct cost and 20% markup."

**🤖 AI Agent:**
> The total change order price is $6,000.00, which includes a markup amount of $1,000.00.

---

**👤 You:**
> "What is the cumulative impact if my original contract was $100,000, I have $15,000 in previous changes, and this new change is $5,000 with a 2-day delay?"

**🤖 AI Agent:**
> The updated contract value is $120,000.00. The total change order volume is 20% of the original contract, and the estimated project delay is 2 days.

---

**👤 You:**
> "Assess risk for a $50,000 contract with $10,000 in total change orders."

**🤖 AI Agent:**
> The project is at medium risk level because the percentage drift is 20.00%.


## ❓ FAQ

**Q: How does the tool calculate the total price of a change order?**
The `calculate_change_order_price` tool takes the direct cost and an overhead/profit rate (e.g., 0.20 for 20%) to calculate the final price charged to the client.

**Q: Can I track the total impact of all changes on my project timeline?**
Yes, using `calculate_cumulative_impact`, you can input your original contract value and previous change orders to see the updated contract total and estimated project delay in days.

**Q: How is project risk determined?**
The `assess_project_risk_level` tool compares the total volume of change orders against the original contract value to categorize the project as low, medium, or high risk.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/change-order-impact-calculator](https://vinkius.com/mcp/change-order-impact-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Change Order Impact Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `change-order-impact-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Change Order Impact Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "change-order-impact-calculator": {
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
