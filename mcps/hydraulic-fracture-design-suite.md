# Hydraulic Fracture Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hydraulic-fracture-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Advanced tools for calculating fracture geometry, leakoff, and proppant transport.

## Description
This MCP server provides a specialized toolkit for reservoir engineers to design hydraulic fracturing treatments. It includes tools to `analyze_fracture_geometry` using PKN, KGD, or pseudo-3d models, `calculate_leakoff_loss` based on rock permeability, `simulate_proppant_transport` to predict placement efficiency, and `evaluate_stress_barriers` to assess vertical containment risks.


## Available Tools (4)
- **analyze_fracture_geometry**: 
- **calculate_leakoff_loss**: 
- **evaluate_stress_barriers**: 
- **simulate_proppant_transport**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydraulic Fracture Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fracture dimensions using a PKN model with 40 MPa stress, 50m thickness, and 200m target length."

**🤖 AI Agent:**
> The calculated fracture dimensions are: Length: 200.0m, Width: 0.015m, Height: 50.0m.

---

**👤 You:**
> "What is the risk of vertical growth if target stress is 35 MPa, barrier stress is 45 MPa, and applied pressure is 40 MPa?"

**🤖 AI Agent:**
> The containment risk is low because the barrier stress is significantly higher than the applied pressure.

---

**👤 You:**
> "Estimate fluid loss for a 10 mD permeability rock with 5000 m2 surface area using a fluid with 10 cP viscosity and 0.5 coefficient."

**🤖 AI Agent:**
> The estimated lost volume is 250.0 m³ and the remaining volume is 750.0 m³.


## ❓ FAQ

**Q: Which geometry models are supported?**
The suite supports PKN, KGD, and pseudo-3d models via the `analyze_fracture_geometry` tool.

**Q: How can I check if my fracture will stay within the target zone?**
You can use the `evaluate_stress_barriers` tool to compare target stress against adjacent layer stress to determine containment risk.

**Q: Can I predict proppant settling?**
Yes, the `simulate_proppant_transport` tool calculates settling velocity and placement efficiency based on fluid viscosity and proppant density.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hydraulic-fracture-design-suite](https://vinkius.com/en/ai-agent-connect/hydraulic-fracture-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydraulic Fracture Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydraulic-fracture-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydraulic Fracture Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydraulic-fracture-design-suite": {
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
