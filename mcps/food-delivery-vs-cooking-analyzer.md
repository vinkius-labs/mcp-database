# Food Delivery vs. Cooking Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/food-delivery-vs-cooking-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A deterministic cost and time-efficiency analyzer for Singaporean young adults.

## Description
This MCP server provides precise economic modeling to help users decide between ordering food and cooking at home. By analyzing weekly delivery costs and the implicit time-cost of cooking, it calculates the delivery premium and the hourly value of time saved. Use `get_delivery_cost_analysis` to find weekly delivery spending, `get_cooking_cost_analysis` to determine the true economic cost of home cooking, and `get_comparison_and_recommendation` to receive a final lifestyle recommendation based on your primary hourly wage.


## Available Tools (3)
- **get_comparison_and_recommendation**: Compares delivery vs. cooking to determine the financial premium, time saved, and provides a final lifestyle recommendation
- **get_cooking_cost_analysis**: Calculates the total weekly economic cost of cooking at home, including time
- **get_delivery_cost_analysis**: Calculates the total weekly financial commitment for a delivery-heavy lifestyle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Food Delivery vs. Cooking Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I order 5 meals a week at 25 SGD each. How much do I spend on delivery?"

**🤖 AI Agent:**
> Your total weekly delivery cost is 125 SGD.

---

**👤 You:**
> "I spend 100 SGD on groceries and cook 5 meals a week. What is my cooking cost?"

**🤖 AI Agent:**
> Your total weekly cooking cost is 137.50 SGD.

---

**👤 You:**
> "Compare 5 delivery meals at 25 SGD each vs cooking 5 meals with a 100 SGD grocery budget. My hourly wage is 30 SGD."

**🤖 AI Agent:**
> Delivery is Worth It.


## ❓ FAQ

**Q: How is the cost of cooking calculated?**
The cost of cooking includes your weekly grocery budget plus the opportunity cost of the time spent preparing and cleaning up meals.

**Q: What does the recommendation mean?**
If the hourly value of your time saved is lower than your main job's hourly rate, the tool suggests you 'Cook More'. Otherwise, it suggests 'Delivery is Worth It'.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, this MCP server can be connected to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/food-delivery-vs-cooking-analyzer](https://vinkius.com/ai-agent-connect/food-delivery-vs-cooking-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Food Delivery vs. Cooking Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `food-delivery-vs-cooking-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Food Delivery vs. Cooking Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "food-delivery-vs-cooking-analyzer": {
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
