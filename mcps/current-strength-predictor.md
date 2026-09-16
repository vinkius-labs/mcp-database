# Current Strength Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/current-strength-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Predict water movement, rip currents, and drift at surf breaks.

## Description
This MCP server provides precise oceanographic predictions for surfers and coastal observers. By analyzing the interaction between swell direction, tide stages, and coastal geometry, it calculates critical water movement patterns. Use `predict_longshore_flow` to determine parallel water speed, `locate_rip_currents` to identify dangerous outgoing channels, `calculate_drift_vector` to find the net movement of water, and `analyze_coastal_influence` to see how headlands and reefs affect current intensity.


## Available Tools (4)
- **analyze_coastal_influence**: Analyzes how landmasses like headlands and reefs impact current strength
- **calculate_drift_vector**: Calculates the net movement of water by combining longshore and rip currents
- **locate_rip_currents**: Locates potential rip current positions based on coastal features
- **predict_longshore_flow**: Predicts the speed and direction of the longshore current


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Current Strength Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where are the rip currents located if the swell is at 180 degrees and there is a reef with a gap at 190 degrees?"

**🤖 AI Agent:**
> The rip current is located at a bearing of 190 degrees with an intensity of 0.8.

---

**👤 You:**
> "How fast is the water moving parallel to the beach with a 150 degree swell, a 45 degree coastline, and high tide?"

**🤖 AI Agent:**
> The longshore current speed is 1.2 meters per second at a direction of 135 degrees.

---

**👤 You:**
> "What is the net movement if the longshore speed is 1.0 at 90 degrees and the rip speed is 0.5 at 180 degrees?"

**🤖 AI Agent:**
> The net drift speed is 1.12 meters per second at a direction of 105 degrees.


## ❓ FAQ

**Q: How accurate are the rip current predictions?**
Predictions are based on the interaction of swell direction and coastal features like reefs or headlands using `locate_rip_currents` to identify high-probability zones.

**Q: Can I calculate the total water movement?**
Yes, you can use `calculate_drift_vector` to combine longshore and rip current data into a single net movement vector.

**Q: Does the tide affect the results?**
Yes, the `tideStage` is a required input for `predict_longshore_flow` as tidal volume significantly impacts current speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/current-strength-predictor](https://vinkius.com/en/ai-agent-connect/current-strength-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Current Strength Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `current-strength-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Current Strength Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "current-strength-predictor": {
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
