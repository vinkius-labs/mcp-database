# Local Delivery Price Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/local-delivery-price-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

A precision pricing engine for calculating delivery fees based on operational costs and profit targets.

## Description
This MCP server provides a precision pricing engine to calculate accurate delivery fees. It aggregates distance-based costs, driver compensation, fuel, time, and packaging to determine a total operational cost, then applies a desired margin. Use `get_cost_breakdown` to see a full itemization of costs, `calculate_margin_impact` to see how profit settings change the final price, `validate_pricing_parameters` to ensure delivery logic is sound, and `optimize_fee_for_target` to reverse-engineer the margin needed to hit a specific price point.


## Available Tools (4)
- **calculate_margin_impact**: Determines how changing the margin (percentage or fixed) affects the final price for a given set of costs
- **get_cost_breakdown**: Provides a detailed itemization of all individual cost components for a specific delivery configuration
- **optimize_fee_for_target**: Reverse-engineers the required margin or cost adjustments needed to reach a specific target delivery fee
- **validate_pricing_parameters**: Checks if a set of proposed delivery parameters is logically sound and within reasonable bounds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Local Delivery Price Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the delivery fee for a 15km trip with a $20 driver pay, $0.15 fuel per km, 30 minutes of time, and $2 packaging, using a 20% margin."

**🤖 AI Agent:**
> The total delivery fee is $28.80, which includes a total cost of $24.00 and a margin of $4.80.

---

**👤 You:**
> "What is the impact on the final fee if I change the margin from a 10% margin to a 15% margin on a base cost of $50?"

**🤖 AI Agent:**
> Increasing the margin from 10% to 15% on a $50 base cost increases the final fee from $55.00 to $57.50.

---

**👤 You:**
> "I want to charge exactly $45.00 for a delivery that costs $35.00 to fulfill. What margin should I use?"

**🤖 AI Agent:**
> To reach a target fee of $45.00 with a base cost of $35.00, you should use a fixed margin of $10.00 or a percentage margin of approximately 28.57%.


## ❓ FAQ

**Q: How does the pricing engine calculate the final fee?**
The engine sums all operational costs--including distance, driver pay, fuel, time, and packaging--and then adds the specified margin (either a fixed amount or a percentage) to reach the final fee.

**Q: Can I check if my delivery parameters are realistic?**
Yes, you can use the `validate_pricing_parameters` tool to check if the distance, time, and driver pay are logically sound and within reasonable bounds.

**Q: How can I find the margin needed to reach a specific price?**
You can use the `optimize_fee_for_target` tool. It reverse-engineers the required margin or cost adjustments needed to hit your target delivery fee.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/local-delivery-price-plan](https://vinkius.com/en/ai-agent-connect/local-delivery-price-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Local Delivery Price Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `local-delivery-price-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Local Delivery Price Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "local-delivery-price-plan": {
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
