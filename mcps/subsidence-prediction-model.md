# Subsidence Prediction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/subsidence-prediction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict surface subsidence and movement caused by underground mining activities.

## Description
This MCP server provides technical tools for estimating surface deformation resulting from underground extraction. It allows users to calculate the peak vertical displacement using `calculate_max_subsidence`, visualize the subsidence trough with `generate_subsidence_profile`, estimate the total surface footprint via `estimate_affected_area`, and verify stability using `check_critical_width_threshold`. It is designed for geotechnical analysis and mining impact assessment.


## Available Tools (4)
- **calculate_max_subsidence**: Determines the peak vertical displacement at the center of a mining panel
- **check_critical_width_threshold**: Determines if the current mining width is sufficient to cause surface movement
- **estimate_affected_area**: Calculates the total surface area impacted by mining-induced movement
- **generate_subsidence_profile**: Provides a set of displacement values across a distance from the center of the mine


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Subsidence Prediction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the maximum subsidence for a Longwall mine with 3m thickness at 500m depth and rock stiffness of 50?"

**🤖 AI Agent:**
> The maximum subsidence for this mining configuration is 1.2 meters.

---

**👤 You:**
> "Will a mining width of 40m cause surface movement at 300m depth with these rock properties?"

**🤖 AI Agent:**
> No, the current mining width is below the critical threshold, so the surface is expected to remain stable.

---

**👤 You:**
> "Calculate the total area impacted by a mine with 100m width, 400m depth, and an angle of draw of 35 degrees."

**🤖 AI Agent:**
> The total affected surface area is 15,420 square meters.


## ❓ FAQ

**Q: How do I calculate the maximum surface sinking?**
Use the `calculate_max_subsidence` tool by providing the mining method, extraction thickness, depth, and rock stiffness.

**Q: Can I see the shape of the subsidence trough?**
Yes, the `generate_subsidence_profile` tool provides a set of displacement values across distances to visualize the trough.

**Q: How is the affected area determined?**
The `estimate_affected_area` tool calculates the total surface footprint based on the mining width, depth, and angle of draw.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/subsidence-prediction-model](https://vinkius.com/ai-agent-connect/subsidence-prediction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Subsidence Prediction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `subsidence-prediction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Subsidence Prediction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "subsidence-prediction-model": {
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
