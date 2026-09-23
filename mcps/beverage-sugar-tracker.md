# Beverage Sugar Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/beverage-sugar-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate cumulative sugar content from various beverage selections.

## Description
This MCP server provides tools to monitor dietary sugar intake by calculating the sugar mass in different beverages. You can use `get_beverage_catalog` to see available drinks, `calculate_single_beverage_sugar` for individual servings, or `calculate_cumulative_sugar_total` to sum up all sugar consumed from a list of drinks. It also includes `search_high_sugar_beverages` to identify drinks with high sugar density.


## Available Tools (4)
- **search_high_sugar_beverages**: Answers the question "Which available beverages have the highest sugar concentrations?"
- **calculate_single_beverage_sugar**: Answers the question "How much sugar is in one specific serving of a chosen beverage?"
- **get_beverage_catalog**: Answers the question "What beverages are available in the system?"
- **calculate_cumulative_sugar_total**: Answers the question "What is the total amount of sugar I have consumed from a list of drinks?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Beverage Sugar Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What beverages are available in the system?"

**🤖 AI Agent:**
> The available beverages include Cola (high density), Orange Juice (moderate density), and Milk (low density).

---

**👤 You:**
> "How much sugar is in 500ml of Cola?"

**🤖 AI Agent:**
> 500ml of Cola contains 55 grams of sugar.

---

**👤 You:**
> "What is the total sugar from 200ml of Juice and 300ml of Cola?"

**🤖 AI Agent:**
> The total sugar consumed is 62 grams.


## ❓ FAQ

**Q: How do I see which drinks are available?**
You can use the `get_beverage_catalog` tool to retrieve a list of all supported beverages and their sugar profiles.

**Q: Can I calculate the total sugar for multiple drinks at once?**
Yes, use the `calculate_cumulative_sugar_total` tool by providing a list of beverage IDs and their respective volumes.

**Q: How can I find drinks with high sugar content?**
Use the `search_high_sugar_beverages` tool to find beverages that exceed a specific sugar density threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/beverage-sugar-tracker](https://vinkius.com/en/ai-agent-connect/beverage-sugar-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Beverage Sugar Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `beverage-sugar-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Beverage Sugar Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "beverage-sugar-tracker": {
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
