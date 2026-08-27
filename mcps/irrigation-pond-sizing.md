# Irrigation Pond Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/irrigation-pond-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate required irrigation pond volumes, physical dimensions, and water loss estimates.

## Description
This MCP server provides specialized tools for designing irrigation storage ponds using water balance analysis. It allows AI agents to determine the `calculate_minimum_storage` required to meet crop demand, design physical footprints with `design_pond_dimensions`, and quantify environmental losses using `estimate_losses`. Additionally, it can evaluate pond performance through `analyze_drawdown_and_reliability` to ensure reliable water supply for agricultural operations.


## Available Tools (4)
- **calculate_minimum_storage**: Determines the required volume of the pond to meet irrigation needs
- **analyze_drawdown_and_reliability**: Evaluates how quickly the pond empties and how likely it is to meet demand
- **design_pond_dimensions**: Calculates the physical footprint and depth of the pond
- **estimate_losses**: Quantifies water lost to the environment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Irrigation Pond Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum storage volume needed for a demand of 5000m3, a peak rate of 50m3/h, a supply rate of 10m3/h, and a refill every 24 hours?"

**🤖 AI Agent:**
> The required volume for these parameters is 5000m3 with a net storage capacity of 4500m3.

---

**👤 You:**
> "Calculate the dimensions for a pond that needs to hold 1000m3 with a maximum depth of 4m and a side slope of 2."

**🤖 AI Agent:**
> The pond will have a surface area of 312.5m2, a bottom area of 125m2, and an average depth of 4m.

---

**👤 You:**
> "If my pond has 500m3 of water and I am withdrawing 20m3/h while receiving 5m3/h, how long until it is empty?"

**🤖 AI Agent:**
> The drawdown rate is 15m3/h, and the pond will be empty in 33.33 hours.


## ❓ FAQ

**Q: How do I calculate the necessary pond volume?**
You can use the `calculate_minimum_storage` tool by providing the total irrigation demand, peak irrigation rate, water supply rate, and refill frequency.

**Q: Can I estimate water loss due to evaporation?**
Yes, the `estimate_losses` tool calculates both evaporation and seepage losses based on surface area and environmental rates.

**Q: How is pond reliability determined?**
Reliability is calculated using the `analyze_drawdown_and_reliability` tool, which compares available volume against the target demand cycle.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/irrigation-pond-sizing](https://vinkius.com/ai-agent-connect/irrigation-pond-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Irrigation Pond Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `irrigation-pond-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Irrigation Pond Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "irrigation-pond-sizing": {
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
