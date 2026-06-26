# Yield Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/yield-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Calculate usable ingredient mass and waste after preparation.

## Description
The Yield Calculator MCP server helps culinary professionals estimate the amount of usable material remaining after cleaning, peeling, or trimming ingredients. By using tools like `calculate_ingredient_yield`, you can determine expected waste and usable mass based on specific yield factors for various items. You can also use `calculate_batch_loss` to aggregate losses across multiple ingredients at once, or `search_ingredients` to find available items in the registry.


## Available Tools (3)
- **calculate_batch_loss**: Calculate total waste and usable mass for a collection of ingredients
- **search_ingredients**: Search the ingredient registry for matches
- **calculate_ingredient_yield**: Calculate expected usable mass and waste for an ingredient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Yield Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much usable meat will I have from 5kg of whole chicken?"

**🤖 AI Agent:**
> From 5kg of whole chicken, you can expect approximately 3.4kg of usable meat and 1.6kg of waste.

---

**👤 You:**
> "Calculate the total waste for 2kg of onions and 3kg of potatoes."

**🤖 AI Agent:**
> The total waste produced from 2kg of onions and 3kg of potatoes is approximately 0.7kg.

---

**👤 You:**
> "Search for any ingredients related to 'beef'."

**🤖 AI Agent:**
> The registry contains the following beef items: Beef Ribeye (85% yield), Beef Brisket (70% yield).


## ❓ FAQ

**Q: How do I calculate the yield for a specific ingredient?**
Use the `calculate_ingredient_yield` tool by providing the ingredient name and its initial mass in kilograms.

**Q: Can I calculate waste for multiple ingredients at once?**
Yes, use the `calculate_batch_loss` tool by passing a JSON array of objects containing ingredient names and their initial masses.

**Q: How can I see which ingredients are available in the registry?**
You can use the `search_ingredients` tool to search through the ingredient catalog for specific names or patterns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/yield-calculator](https://vinkius.com/mcp/yield-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Yield Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `yield-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Yield Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "yield-calculator": {
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
