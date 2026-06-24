# Planting Window Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/planting-window-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Determine optimal planting windows, insurance deadlines, and climate risks for crops.

## Description
The Planting Window Calculator connects AI agents to precise agricultural zoning data. Use `get_planting_window` to find the ideal planting dates and critical insurance deadlines for specific regions. Evaluate seasonal weather threats using `fetch_climate_risks` to identify potential frost or drought periods. Discover suitable crop varieties with `get_cultivar_recommendations` based on their maturation groups, and estimate productivity impacts of late planting with `calculate_yield_loss`.


## Available Tools (4)
- **fetch_climate_risks**: Evaluates the probability of adverse weather events
- **get_cultivar_recommendations**: Provides a list of recommended crop varieties
- **get_planting_window**: Retrieves the recommended planting period and insurance deadline
- **calculate_yield_loss**: Estimates the productivity loss caused by planting delays


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Planting Window Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When is the best time to plant Corn in Iowa, Polk County?"

**🤖 AI Agent:**
> The recommended planting window for Corn in Polk County, Iowa, is from May 10th to May 30th. The critical insurance deadline is June 5th.

---

**👤 You:**
> "What are the climate risks for Wheat in France, Seine-et-Marne during the second fortnight of May?"

**🤖 AI Agent:**
> For the specified period, there is a Medium risk level with the primary threat being Heatwave.

---

**👤 You:**
> "How much yield will I lose if my Soybean planting is 3 weeks late?"

**🤖 AI Agent:**
> A 3-week delay in Soybean planting is estimated to cause a 12.5% reduction in yield, which is considered a Significant impact.


## ❓ FAQ

**Q: How do I find the best time to plant my crops?**
Use the `get_planting_window` tool by providing your crop type, state, and municipality to retrieve the recommended start and end dates.

**Q: Can I check for potential weather risks during the season?**
Yes, use `fetch_climate_risks` with a specific fortnight index to see the probability of threats like frost or heatwaves.

**Q: What happens if I plant after the recommended window?**
You can estimate the potential reduction in yield using the `calculate_yield_loss` tool by specifying how many weeks you are delayed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/planting-window-calculator](https://vinkius.com/mcp/planting-window-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Planting Window Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `planting-window-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Planting Window Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "planting-window-calculator": {
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
