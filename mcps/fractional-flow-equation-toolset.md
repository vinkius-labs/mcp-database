# Fractional Flow Equation Toolset MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fractional-flow-equation-toolset)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate fractional flow curves, breakthrough saturation, and gravity effects in reservoir displacement.

## Description
This MCP server provides specialized reservoir engineering tools to model displacement processes. It allows users to generate fractional flow curves using `calculate_fractional_flow_curve`, determine breakthrough characteristics via `perform_welge_analysis`, and compute gravity corrections with `calculate_gravity_correction`. It also enables comparing displacement efficiency between different scenarios using `compare_displacement_efficiency`.


## Available Tools (4)
- **calculate_fractional_flow_curve**: Generates a series of water cut values across a range of water saturations
- **calculate_gravity_correction**: Computes the specific gravity component for inclined reservoirs
- **compare_displacement_efficiency**: Evaluates how different viscosity ratios or gravity effects impact the sweep efficiency
- **perform_welge_analysis**: Determines the breakthrough characteristics using the tangent method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fractional Flow Equation Toolset** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fractional flow curve for a water-oil system with water viscosity 1.0, oil viscosity 2.0, and a gravity factor of 0.1."

**🤖 AI Agent:**
> The fractional flow curve has been generated with water saturations ranging from 0.2 to 0.8, showing a water cut that increases from 0.05 to 0.85.

---

**👤 You:**
> "What is the breakthrough saturation if the initial water saturation is 0.2 and the flow curve is provided?"

**🤖 AI Agent:**
> The breakthrough saturation is 0.45, with a water cut at breakthrough of 0.32 and an average saturation of 0.55.

---

**👤 You:**
> "Calculate the gravity correction for water density 1000, oil density 800, height 10, angle 30, and permeability 0.1."

**🤖 AI Agent:**
> The calculated gravity factor is 0.0866.


## ❓ FAQ

**Q: How do I calculate the water cut at breakthrough?**
You can use the `perform_welge_analysis` tool. Provide the fractional flow curve data and the initial water saturation to find the water cut at breakthrough.

**Q: Can I account for inclined reservoirs?**
Yes, use `calculate_gravity_correction` to compute the gravity factor based on fluid densities, reservoir height, and inclination angle.

**Q: How do I compare two different displacement scenarios?**
Use the `compare_displacement_efficiency` tool by providing the base flow curve and the comparison flow curve.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fractional-flow-equation-toolset](https://vinkius.com/ai-agent-connect/fractional-flow-equation-toolset)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fractional Flow Equation Toolset** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fractional-flow-equation-toolset` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fractional Flow Equation Toolset** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fractional-flow-equation-toolset": {
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
