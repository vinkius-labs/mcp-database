# Zero-Waste Shopping Assistant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/zero-waste-shopping-assistant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Converts shopping items into precise refill quantities based on container capacity and usage.

## Description
This MCP server helps users transition to zero-waste living by calculating exactly how much bulk product to buy. It uses `get_product_refill_info` to check availability and density, `calculate_needed_quantity` to determine purchase amounts based on current stock and usage, and `validate_container_fit` to ensure items fit in reusable jars. You can also use `generate_optimized_shopping_list` to create a complete, optimized plan for your next trip.


## Available Tools (4)
- **generate_optimized_shopping_list**: Gen list
- **get_product_refill_info**: Check refill info
- **calculate_needed_quantity**: Calc quantity
- **validate_container_fit**: Check fit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zero-Waste Shopping Assistant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 200g of lentils, I use 50g a day, and I'll shop in 4 days. How much should I buy for my 500ml jar?"

**🤖 AI Agent:**
> You need to buy 0g of lentils because your current stock of 200g is sufficient to cover the 200g needed for the next 4 days.

---

**👤 You:**
> "Check if oats are available for refill and tell me their density."

**🤖 AI Agent:**
> Yes, oats are available for refill. Their density is 0.45 g/ml.

---

**👤 You:**
> "Will 500g of rice fit in a 600ml container?"

**🤖 AI Agent:**
> Yes, 500g of rice will fit in your 600ml container.


## ❓ FAQ

**Q: How does the tool know if an item is refillable?**
The `get_product_refill_info` tool checks the internal bulk availability catalog to verify if a product can be purchased in a refillable format.

**Q: Can I check if my jar is big enough?**
Yes, use the `validate_container_fit` tool by providing the container volume and the target weight of the product.

**Q: How do I generate a full list for my trip?**
You can use `generate_optimized_shopping_list` with a list of your desired items to get a complete plan including weights and fit status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/zero-waste-shopping-assistant](https://vinkius.com/en/ai-agent-connect/zero-waste-shopping-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zero-Waste Shopping Assistant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zero-waste-shopping-assistant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zero-Waste Shopping Assistant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zero-waste-shopping-assistant": {
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
