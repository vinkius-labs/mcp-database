# Thermal Analysis Interpreter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/thermal-analysis-interpreter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Analyzes TGA, DSC, and DTA data to identify decomposition, phase transitions, and enthalpy.

## Description
This MCP server provides specialized tools for interpreting thermal analysis data. It allows AI agents to process Thermogravimetric Analysis (TGA), Differential Scanning Calorimetry (DSC), and Differential Thermal Analysis (DTA) datasets. Using `analyze_tga_stability`, agents can identify mass loss events and decomposition temperatures. The `calculate_phase_transitions` tool detects melting points and phase changes, while `quantify_enthalpy` calculates the energy associated with specific thermal events. For kinetic studies, `estimate_kinetics` provides activation energy and reaction order based on heating rates.


## Available Tools (4)
- **estimate_kinetics**: Estimates the kinetic parameters of a decomposition process
- **analyze_tga_stability**: Identifies mass loss events and decomposition temperatures from TGA data
- **calculate_phase_transitions**: Detects phase changes and melting points from DSC or DTA data
- **quantify_enthalpy**: Calculates the energy associated with a specific thermal event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thermal Analysis Interpreter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze this TGA data: [{'temp': 100, 'mass': 1.0}, {'temp': 200, 'mass': 0.95}, {'temp': 300, 'mass': 0.7}]."

**🤖 AI Agent:**
> The TGA analysis shows a significant decomposition event starting near 200°C, with a total mass loss of 30%.

---

**👤 You:**
> "What is the enthalpy for the transition between 150 and 180 degrees in this DSC data?"

**🤖 AI Agent:**
> The calculated enthalpy for the transition between 150 and 180 degrees is 45.2 J/g.

---

**👤 You:**
> "Detect phase transitions in this DSC data: [{'temp': 50, 'heatFlow': 0.1}, {'temp': 150, 'heatFlow': 5.0}, {'temp': 250, 'heatFlow': 0.1}]."

**🤖 AI Agent:**
> A phase transition was detected at 150°C.


## ❓ FAQ

**Q: What types of thermal data can this server process?**
The server processes TGA, DSC, and DTA data to extract stability, phase transition, and kinetic information.

**Q: How do I use the TGA stability tool?**
You can use `analyze_tga_stability` by providing the temperature program as an array of temperature and mass points.

**Q: Can I calculate enthalpy for a specific temperature range?**
Yes, the `quantify_enthalpy` tool calculates the energy associated with a transition between a specified start and end temperature.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/thermal-analysis-interpreter](https://vinkius.com/ai-agent-connect/thermal-analysis-interpreter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thermal Analysis Interpreter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thermal-analysis-interpreter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thermal Analysis Interpreter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thermal-analysis-interpreter": {
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
