# Well Log Interpretation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/well-log-interpretation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Interprets open-hole well logs to evaluate formation properties and identify hydrocarbons.

## Description
This MCP server provides specialized tools for formation evaluation using open-hole well logs. It allows AI agents to process gamma ray, resistivity, density, and sonic data to determine critical reservoir characteristics. Using `get_shale_volume`, agents can assess lithology by calculating shale volume. The `calculate_porosity` tool estimates void space in the rock, while `evaluate_water_saturation` identifies potential hydrocarbon zones by calculating the water-filled pore fraction. Finally, `calculate_hydrocarbon_thickness` computes the net vertical thickness of hydrocarbon-bearing intervals, facilitating precise reservoir quality assessment.


## Available Tools (4)
- **calculate_hydrocarbon_thickness**: Computes the net thickness of the hydrocarbon-bearing interval
- **calculate_porosity**: Estimates the rock porosity using available density or sonic data
- **evaluate_water_saturation**: Calculates the fraction of pore space filled with water to identify potential oil or gas zones
- **get_shale_volume**: Determines the volume of shale within a specific depth interval to assess lithology


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Log Interpretation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shale volume for these gamma ray readings: [20, 25, 30, 80, 90]. Use 10 as the clean minimum and 100 as the pure shale maximum."

**🤖 AI Agent:**
> [0.1, 0.16, 0.22, 0.77, 0.88]

---

**👤 You:**
> "Estimate the porosity using density log values [2.3, 2.4, 2.2] with a matrix density of 2.65 and fluid density of 1.0."

**🤖 AI Agent:**
> [0.136, 0.113, 0.173]

---

**👤 You:**
> "What is the total hydrocarbon thickness if porosity is [0.2, 0.2], water saturation is [0.3, 0.3], and depth intervals are [5, 5]?"

**🤖 AI Agent:**
> 7.0


## ❓ FAQ

**Q: What kind of log data can I use with this server?**
You can use gamma ray, resistivity, density, and sonic log data to perform various formation evaluation calculations.

**Q: How do I calculate the shale volume?**
Use the `get_shale_volume` tool by providing the gamma ray log readings along with the minimum and maximum gamma ray benchmarks for clean and pure shale formations.

**Q: Can this tool help identify oil or gas zones?**
Yes, by using `evaluate_water_saturation` to find low water saturation zones and `calculate_hydrocarbon_thickness` to determine the net thickness of the hydrocarbon-bearing interval.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/well-log-interpretation](https://vinkius.com/en/ai-agent-connect/well-log-interpretation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Log Interpretation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-log-interpretation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Log Interpretation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-log-interpretation": {
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
