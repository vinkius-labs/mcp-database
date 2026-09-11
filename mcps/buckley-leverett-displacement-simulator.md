# Buckley-Leverett Displacement Simulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/buckley-leverett-displacement-simulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Models waterflood displacement using Buckley-Leverett theory to predict saturation profiles and breakthrough.

## Description
This MCP server provides advanced simulation capabilities for reservoir engineering. It implements the Buckley-Leverett theory to model how water displaces oil in porous media. Users can use `analyze_saturation_profile` to visualize the spatial distribution of water saturation, `calculate_breakthrough` to predict when water will reach the production well, and `estimate_sweep_efficiency` to evaluate displacement effectiveness. The engine accounts for shock fronts and fractional flow dynamics based on provided relative permeability data.


## Available Tools (4)
- **analyze_saturation_profile**: Predicts the spatial distribution of water saturation across the reservoir at a given time
- **calculate_breakthrough**: Determines when the water front will reach the production end of the reservoir
- **estimate_sweep_efficiency**: Evaluates the effectiveness of the displacement process at a specific time
- **get_fractional_flow_curve**: Generates the fractional flow values for a range of water saturations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buckley-Leverett Displacement Simulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the water saturation profile for a 100m reservoir with an injection rate of 5, viscosities of 1 and 5, and specific permeability data at time 10."

**🤖 AI Agent:**
> The water saturation profile shows a shock front at 45.2m with a saturation of 0.65, followed by a trailing edge saturation of 0.25.

---

**👤 You:**
> "When will water breakthrough occur in a 500m reservoir with these fluid properties?"

**🤖 AI Agent:**
> Breakthrough is predicted to occur at 1250.5 units of time with a breakthrough saturation of 0.42.

---

**👤 You:**
> "What is the sweep efficiency after 50 units of time?"

**🤖 AI Agent:**
> The volumetric sweep efficiency is 0.35 and the oil recovery factor is 0.28.


## ❓ FAQ

**Q: How can I predict when water will reach my production well?**
You can use the `calculate_breakthrough` tool. By providing the reservoir length, injection rate, and fluid viscosities, the tool determines the exact breakthrough time and saturation.

**Q: Can I visualize the water saturation movement?**
Yes, the `analyze_saturation_profile` tool calculates the spatial distribution of water saturation across the reservoir at any given time.

**Q: What parameters are required for the simulation?**
The simulation requires the reservoir length, injection rate, water and oil viscosities, and a JSON string containing the relative permeability data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/buckley-leverett-displacement-simulator](https://vinkius.com/en/ai-agent-connect/buckley-leverett-displacement-simulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buckley-Leverett Displacement Simulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buckley-leverett-displacement-simulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buckley-Leverett Displacement Simulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buckley-leverett-displacement-simulator": {
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
