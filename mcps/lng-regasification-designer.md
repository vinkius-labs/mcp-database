# LNG Regasification Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/lng-regasification-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design LNG regasification systems by calculating vaporizer types, heat duties, and seawater flow.

## Description
This MCP server provides specialized engineering tools for designing Liquefied Natural Gas (LNG) regasification systems. It allows users to determine the most efficient technology for their specific environment using `select_vaporizer_type`. Engineers can calculate the total thermal energy required via `calculate_heat_duty` and determine necessary seawater volumes with `calculate_seawater_flow`. Additionally, the tool accounts for seasonal demand shifts using `analyze_seasonal_variation` to ensure system reliability throughout the year.


## Available Tools (4)
- **analyze_seasonal_variation**: Adjusts design parameters to account for changes in demand and environmental conditions across different seasons
- **calculate_heat_duty**: Determines the total thermal energy required for the regasification process
- **calculate_seawater_flow**: Calculates the necessary seawater flow rate to satisfy the heat duty
- **select_vaporizer_type**: Determines the most appropriate regasification technology based on environmental conditions and demand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LNG Regasification Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What vaporizer type should I use if the seawater is 15°C and the air is 25°C with a sendout of 500 units?"

**🤖 AI Agent:**
> The recommended vaporizer type is ORV with a suitability score of 0.85.

---

**👤 You:**
> "Calculate the heat duty for 1000 units of gas, moving from -160°C to 15°C."

**🤖 AI Agent:**
> The total heat duty required is 450.5 MW.

---

**👤 You:**
> "How much seawater flow is needed for a 300 MW heat duty if seawater enters at 20°C and leaves at 10°C?"

**🤖 AI Agent:**
> The required seawater flow rate is 12500 m3/h.


## ❓ FAQ

**Q: How do I choose the right vaporizer?**
You can use the `select_vaporizer_type` tool, which evaluates seawater and ambient air temperatures to recommend an ORV, SCV, or AAV.

**Q: Can I account for winter demand increases?**
Yes, the `analyze_seasonal_variation` tool adjusts your base sendout requirements based on seasonal factors and temperature deltas.

**Q: What inputs are needed for heat duty calculations?**
To use `calculate_heat_duty`, you need the sendout requirement, the target gas temperature, and the initial LNG inlet temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/lng-regasification-designer](https://vinkius.com/en/ai-agent-connect/lng-regasification-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LNG Regasification Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `lng-regasification-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LNG Regasification Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lng-regasification-designer": {
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
