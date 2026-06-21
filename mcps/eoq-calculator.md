# EOQ Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eoq-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Optimize inventory replenishment by calculating the Economic Order Quantity (EOQ) and reorder points.

## Description
The EOQ Calculator helps businesses minimize total inventory costs by finding the ideal balance between ordering expenses and holding costs. Using the `calculate_eoq_metrics` tool, you can determine your optimal order quantity, frequency of orders per year, and the average days between replenishment cycles. Additionally, use `calculate_reorder_point` to identify exactly when a new order should be placed based on lead time, and `analyze_cost_efficiency` to get a detailed breakdown of annual ordering versus holding costs. This tool is essential for supply chain managers looking to prevent stockouts while reducing unnecessary storage expenditures.


## Available Tools (3)
- **analyze_cost_efficiency**: Provides a granular breakdown of inventory costs to verify the balance between ordering and holding expenses
- **calculate_eoq_metrics**: Calculates the primary optimization metrics including optimal quantity and replenishment frequency
- **calculate_reorder_point**: Determines the specific inventory threshold that triggers a new purchase order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EOQ Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the optimal order quantity for a product with an annual demand of 5000 units, an order cost of $50, a holding cost of 20%, and a unit price of $10."

**🤖 AI Agent:**
> The optimal order quantity is approximately 500 units, with about 10 orders per year and an average of 36.5 days between orders.

---

**👤 You:**
> "What is the reorder point if my annual demand is 1200 units and the lead time is 5 days?"

**🤖 AI Agent:**
> The reorder point is 16.44 units, meaning you should place a new order when your stock reaches this level to cover the daily demand of approximately 3.29 units.

---

**👤 You:**
> "Analyze the cost efficiency for a scenario with 10000 annual demand, $100 order cost, 15% holding cost, and $5 unit price."

**🤖 AI Agent:**
> The annual ordering cost is approximately $1,414.21 and the annual holding cost is approximately $1,414.21, demonstrating a balanced cost structure.


## ❓ FAQ

**Q: What is the Economic Order Quantity (EOQ)?**
EOQ is the ideal order size a company should purchase to minimize its total inventory costs, specifically balancing ordering costs and holding costs.

**Q: How do I use the `calculate_eoq_metrics` tool?**
Provide your annual demand, fixed cost per order, holding cost percentage (as a decimal), and the unit price of the item to receive optimal quantity and frequency metrics.

**Q: Can this tool help prevent stockouts?**
Yes, by using the `calculate_reorder_point` tool with your lead time data, you can determine the exact inventory level that triggers a new order to ensure goods arrive before you run out.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eoq-calculator](https://vinkius.com/mcp/eoq-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EOQ Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `eoq-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EOQ Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "eoq-calculator": {
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
