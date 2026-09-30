# Party Budget Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/party-budget-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate complete event budgets including taxes, tips, and contingency buffers.

## Description
Plan your next event with precision using the Party Budget Builder. This MCP server provides specialized tools to aggregate costs across venue, food, drinks, decor, and entertainment. You can use `calculate_subtotal` to find your base costs, `apply_fees_and_taxes` to handle service charges, and `calculate_contingency` to ensure you have a safety net. For a complete overview, `generate_full_budget` provides a comprehensive breakdown of every expense, tax, tip, and contingency amount in one go.


## Available Tools (4)
- **apply_fees_and_taxes**: Calculates the extra costs stemming from taxes and gratuities based on the subtotal
- **calculate_subtotal**: Calculates the sum of all primary event expenses before any additional fees are applied
- **generate_full_budget**: Provides a complete breakdown of every cost component for a single event
- **calculate_contingency**: Determines the amount of extra money needed to protect against unexpected expenses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Party Budget Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a full budget for a wedding with a $5000 venue, $3000 food, $1000 drinks, 8% tax, 15% tip, and 10% contingency."

**🤖 AI Agent:**
> The total budget for your wedding is $10,450.00, which includes a subtotal of $9,000.00, $720.00 in taxes, $1,350.00 in tips, and $980.00 for contingency.

---

**👤 You:**
> "What is the subtotal for a small dinner costing $200 for food and $50 for drinks?"

**🤖 AI Agent:**
> The subtotal for your dinner is $250.00.

---

**👤 You:**
> "I have a running total of $1200. How much should I set aside for a 15% contingency?"

**🤖 AI Agent:**
> A 15% contingency on $1,200.00 is $180.00.


## ❓ FAQ

**Q: How do I calculate the total cost of my party?**
You can use the `generate_full_budget` tool to provide all your costs and rates, which will return a complete breakdown including the grand total.

**Q: Can I calculate taxes and tips separately?**
Yes, use the `apply_fees_and_taxes` tool to calculate specific tax and tip amounts based on your subtotal.

**Q: What is a contingency buffer?**
A contingency is a safety fund. You can use `calculate_contingency` to determine how much extra money to set aside based on your running total to cover unexpected costs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/party-budget-builder](https://vinkius.com/en/ai-agent-connect/party-budget-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Party Budget Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `party-budget-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Party Budget Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "party-budget-builder": {
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
