# In-Situ Stress Measurement MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/in-situ-stress-measurement)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Interprets in-situ stress measurement data from overcoring, hydraulic fracturing, or acoustic emission.

## Description
This MCP server provides specialized tools to interpret in-situ stress states in rock masses. It allows AI agents to process complex geotechnical data and derive critical engineering parameters. Using `analyze_overcoring_data`, agents can calculate full 3D stress tensors from strain gauge readings. The `interpret_hydraulic_fracture` tool determines principal stress magnitudes and orientations from borehole fracture data. For seismic monitoring, `process_acoustic_emission` infers stress field characteristics from energy release distributions. Finally, `calculate_stress_regime` classifies the tectonic environment (Normal, Strike-Slip, or Thrust) based on calculated principal stresses.


## Available Tools (4)
- **analyze_overcoring_data**: Calculates the full 3D stress tensor from overcoring strain gauge measurements
- **calculate_stress_regime**: Classifies the tectonic stress environment based on existing principal stress calculations
- **interpret_hydraulic_fracture**: Determines principal stress magnitudes and orientations based on fracture occurrence
- **process_acoustic_emission**: Infers stress field characteristics from the spatial distribution of acoustic energy releases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **In-Situ Stress Measurement** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the stress tensor from these strain readings: [{'gauge': 1, 'strain': 0.0001}, {'gauge': 2, 'strain': 0.00015}] and rock elasticity {'E': 50e9, 'nu': 0.25}."

**🤖 AI Agent:**
> The calculated principal stresses are: Max: 45.2 MPa, Mid: 30.1 MPa, Min: 15.5 MPa, with an azimuth of 120 degrees and dip of 45 degrees.

---

**👤 You:**
> "What is the stress regime if the principal stresses are 50 MPa, 45 MPa, and 10 MPa?"

**🤖 AI Agent:**
> The stress regime is classified as Strike-Slip because the intermediate principal stress (45 MPa) is the vertical component.

---

**👤 You:**
> "Determine the stress from a hydraulic fracture with orientation {'azimuth': 90, 'dip': 0}, breakdown pressure 30 MPa, and depth 500m."

**🤖 AI Agent:**
> The minimum principal stress is 30 MPa, and the maximum horizontal stress orientation is 90 degrees.


## ❓ FAQ

**Q: What kind of data can I provide for stress analysis?**
You can provide strain readings from overcoring, fracture orientation and pressure from hydraulic fracturing, or acoustic emission event logs.

**Q: Can this tool account for rock anisotropy?**
Yes, the `analyze_overcoring_data` tool includes an optional anisotropy factor to adjust stress tensor calculations for directional stiffness variations.

**Q: How is the tectonic stress regime determined?**
The `calculate_stress_regime` tool classifies the environment as Normal, Strike-Slip, or Thrust based on the relative magnitudes of the three principal stresses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/in-situ-stress-measurement](https://vinkius.com/ai-agent-connect/in-situ-stress-measurement)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **In-Situ Stress Measurement** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `in-situ-stress-measurement` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **In-Situ Stress Measurement** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "in-situ-stress-measurement": {
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
