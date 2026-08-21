# Ride-Hail Surge Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/ride-hail-surge-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Predict ride-hailing surge multipliers and total fares based on weather and peak hours.

## Description
This MCP server provides deterministic surge multiplier and fare estimation for ride-hailing services. It calculates price adjustments by analyzing rain intensity, peak commuting windows, and CBD location status. Use `estimate_surge_multiplier` to get a full breakdown of factors and the final estimated fare, or `get_peak_status` to check if a specific time falls within high-demand periods.


## Available Tools (3)
- **get_peak_status**: 
- **estimate_surge_multiplier**: 
- **validate_environmental_inputs**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ride-Hail Surge Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the total fare be for a 15 SGD base fare if it is raining at 10mm/hr at 18:30 in the CBD?"

**🤖 AI Agent:**
> The rain factor is 0.4, the peak factor is 1.2, and the CBD factor is 1.1. The final multiplier is capped at 2.5, resulting in an estimated total fare of 37.5 SGD.

---

**👤 You:**
> "Is 08:15 considered a peak hour?"

**🤖 AI Agent:**
> Yes, 08:15 is within the morning peak window.

---

**👤 You:**
> "Calculate the surge for a 10 SGD fare with no rain at 12:00 in a non-CBD area."

**🤖 AI Agent:**
> The final multiplier is 1.0, and the estimated total fare is 10.0 SGD.


## ❓ FAQ

**Q: How is the surge multiplier calculated?**
The multiplier starts at 1.0 and increases based on rain intensity, peak hour timing, and whether the location is in a CBD during peak hours, up to a maximum cap of 2.5.

**Q: Can I check if it is currently peak hour?**
Yes, you can use the `get_peak_status` tool to determine if a specific time falls within the high-demand morning or evening windows.

**Q: Does rain affect the price?**
Yes, the `estimate_surge_multiplier` tool adds a factor of 0.2 for every 5mm/hr of rainfall intensity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/ride-hail-surge-estimator](https://vinkius.com/ai-agent-connect/ride-hail-surge-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ride-Hail Surge Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ride-hail-surge-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ride-Hail Surge Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ride-hail-surge-estimator": {
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
