# Crop Yield Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/crop-yield-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Estimates agricultural production by synthesizing planting metrics and soil constraints.

## Description
This MCP server provides a specialized engine for calculating expected crop yields. It bridges the gap between biological potential and environmental reality by processing planting parameters, survival rates, and soil-specific physiological constraints. Users can use `calculate_biological_yield` to determine theoretical potential, `apply_soil_corrections` to adjust for pH, organic matter, and CEC, and `get_production_confidence` to establish statistical yield ranges based on historical variance.


## Available Tools (4)
- **apply_soil_corrections**: Adjusts a biological yield estimate based on the physiological constraints of the specific soil type and crop
- **calculate_biological_yield**: Determines the theoretical yield based solely on planting and survival metrics
- **get_production_confidence**: Provides a statistical range for the estimated yield to account for environmental uncertainty
- **query_crop_metadata**: Retrieves the standard coefficients and variance data for a specific crop


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crop Yield Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the biological yield for 50 hectares with a seed density of 300, a germination rate of 0.9, a survival rate of 0.8, and an average grain weight of 0.5kg."

**🤖 AI Agent:**
> The expected yield per hectare is 108 kg/ha, and the total harvest for 50 hectares is 5,400 kg.

---

**👤 You:**
> "Adjust a base yield of 2000 kg/ha for Maize using a soil pH of 6.5, organic matter of 3%, and CEC of 15."

**🤖 AI Agent:**
> The corrected yield for Maize after soil adjustments is 2,150 kg/ha.

---

**👤 You:**
> "What is the confidence interval for a Wheat yield of 3500 kg/ha?"

**🤖 AI Agent:**
> The expected yield range for Wheat is between 3,150 kg/ha and 3,850 kg/ha.


## ❓ FAQ

**Q: How does the engine account for soil quality?**
The engine uses `apply_soil_corrections` to adjust the base biological yield using specific coefficients for pH, organic matter, and Cation Exchange Capacity (CEC) tailored to the selected crop type.

**Q: Can I get a range for my yield estimates?**
Yes, by using `get_production_confidence`, you can retrieve a lower and upper bound for your estimated yield based on historical variance for that specific crop.

**Q: What inputs are required for the initial yield calculation?**
To use `calculate_biological_yield`, you need the planted area, seed density, germination rate, survival rate, and the average grain weight per plant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/crop-yield-estimator](https://vinkius.com/ai-agent-connect/crop-yield-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crop Yield Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crop-yield-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crop Yield Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crop-yield-estimator": {
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
