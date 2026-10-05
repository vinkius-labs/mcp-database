# Custom Gift Cost Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/custom-gift-cost-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate comprehensive costs for custom gifts, including base price, personalization, shipping, and taxes.

## Description
This MCP server provides a complete pricing engine for custom gift orders. It allows AI agents to calculate the full cost of a gift by aggregating the base item price, personalization fees, shipping costs, gift wrapping, rush fees, and applicable taxes. Use `get_total_gift_quote` to retrieve a complete breakdown of the final price, or use individual tools like `get_base_item_price` and `calculate_fulfillment_fees` for granular cost analysis.


## Available Tools (4)
- **calculate_personalization_cost**: 
- **get_base_item_price**: 
- **get_total_gift_quote**: 
- **calculate_fulfillment_fees**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Custom Gift Cost Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost for item 'gift_001' with standard personalization, express shipping, gift wrap, and a 5% tax rate?"

**🤖 AI Agent:**
> The total cost for the custom gift is $45.50, which includes the base price, personalization, express shipping, gift wrap, and 5% tax.

---

**👤 You:**
> "How much does it cost to add intricate personalization to item 'luxury_vase_99'?"

**🤖 AI Agent:**
> The personalization fee for intricate customization on the luxury vase is $25.00.

---

**👤 You:**
> "Calculate the fulfillment fees for a standard shipping order that includes gift wrap but no rush processing."

**🤖 AI Agent:**
> The fulfillment fees are $12.00, consisting of $10.00 for standard shipping and $2.00 for gift wrapping.


## ❓ FAQ

**Q: How does the tool calculate the final price?**
The tool sums the base price, personalization fee, gift wrap cost, and rush fee to create a subtotal. It then applies the tax rate to that subtotal and adds the shipping cost to reach the final total.

**Q: Can I calculate shipping costs separately?**
Yes, you can use `calculate_fulfillment_fees` to get specific costs for shipping, gift wrapping, and rush processing without generating a full quote.

**Q: What complexity levels are supported for personalization?**
The system supports 'standard' and 'intricate' complexity levels for calculating personalization fees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/custom-gift-cost-planner](https://vinkius.com/en/ai-agent-connect/custom-gift-cost-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Custom Gift Cost Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `custom-gift-cost-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Custom Gift Cost Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "custom-gift-cost-planner": {
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
