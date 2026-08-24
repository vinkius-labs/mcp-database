# Wine Serving Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-serving-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [hospitality](../categories/hospitality.md)

Deterministic wine service planning for events.

## Description
Plan your event's beverage needs with precision. This MCP server provides tools to calculate exact bottle counts, total liquid volume, and necessary ice for chilling. Using `calculate_wine_needs`, you can determine requirements based on guest count, wine type, and event duration. It accounts for declining consumption rates and specific pour sizes for red, white, rosé, sparkling, and dessert wines. You can also use `get_serving_metrics` for detailed glass counts or `get_chilling_requirements` to find the exact ice mass needed for your bottles.


## Available Tools (3)
- **calculate_wine_needs**: Calculates the total number of bottles, volume, and ice required for a specific wine type and event profile
- **get_chilling_requirements**: Calculates the necessary ice mass for a specific number of bottles
- **get_serving_metrics**: Provides specific consumption metrics (total glasses and total milliliters) for a given group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Serving Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many bottles of red wine do I need for 50 guests at a 3-hour event using 750ml bottles?"

**🤖 AI Agent:**
> You will need 15 bottles of red wine. This includes a total volume of 11.25 liters and requires 30kg of ice for chilling.

---

**👤 You:**
> "Calculate the ice needed for 10 bottles of sparkling wine."

**🤖 AI Agent:**
> You will need 20kg of ice to chill 10 bottles.

---

**👤 You:**
> "What are the serving metrics for 20 guests drinking dessert wine for 4 hours?"

**🤖 AI Agent:**
> For 20 guests, you can expect a total of 30 glasses and a total volume of 2700ml.


## ❓ FAQ

**Q: How does the tool calculate wine consumption?**
The tool applies a declining consumption rate: guests are expected to consume one glass per hour for the first two hours, and half a glass per hour for every hour thereafter.

**Q: What pour sizes are used for different wines?**
Standard table wines (red, white, rosé) use a 150ml pour, sparkling wine uses 120ml, and dessert wine uses 90ml.

**Q: How much ice is required for chilling?**
The service requires exactly 2kg of ice for every bottle planned for the event.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-serving-calculator](https://vinkius.com/ai-agent-connect/wine-serving-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Serving Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-serving-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Serving Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-serving-calculator": {
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
