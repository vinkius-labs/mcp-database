# Alcohol Quantity Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alcohol-quantity-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [inventory-management](../categories/inventory-management.md)

Calculate exact alcohol inventory needed for events based on guests, duration, and preferences.

## Description
The Alcohol Quantity Planner helps event organizers determine precise beverage requirements. By using `calculate_total_servings`, you can estimate total consumption based on guest count and event duration. Then, use `split_servings_by_preference` to distribute those drinks into wine, beer, and liquor categories. Finally, `calculate_procurement_quantities` provides the exact number of bottles and units to purchase, including a recommended safety buffer.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alcohol Quantity Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 100 guests, 4 hours of event time, and 80% are drinkers. How many total servings will be consumed?"

**🤖 AI Agent:**
> For 100 guests with an 80% drinker rate over 4 hours, the total alcoholic servings expected is 200.

---

**👤 You:**
> "If I have 200 servings and want a split of 50% wine, 30% beer, and 20% liquor, how many servings of each do I need?"

**🤖 AI Agent:**
> You will need 100 wine servings, 60 beer servings, and 40 liquor servings.

---

**👤 You:**
> "How many bottles of wine and liquor should I buy for 50 wine servings and 34 liquor servings, including a 10% buffer?"

**🤖 AI Agent:**
> You should purchase 11 bottles of wine and 3 bottles of liquor.


## ❓ FAQ

**Q: How does the consumption rate work?**
The tool uses a tiered approach: 1.5 drinks per person per hour for the first two hours, and 1 drink per person per hour thereafter. Tools available: `your_tool_name`.

**Q: Does it include a safety margin?**
Yes, `calculate_procurement_quantities` includes a 10% buffer by default to prevent running out of drinks.

**Q: What beverage types are supported?**
The planner calculates requirements for wine, beer, and liquor/cocktails based on standard pour sizes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alcohol-quantity-planner](https://vinkius.com/mcp/alcohol-quantity-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alcohol Quantity Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alcohol-quantity-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alcohol Quantity Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alcohol-quantity-planner": {
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
