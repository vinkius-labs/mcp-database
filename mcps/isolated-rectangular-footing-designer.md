# Isolated Rectangular Footing Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/isolated-rectangular-footing-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates dimensions, thickness, and reinforcement for isolated rectangular footings.

## Description
This MCP server provides structural engineering tools to design isolated rectangular footings. It calculates necessary footing dimensions using `get_footing_dimensions`, determines required thickness to resist shear with `get_footing_thickness`, calculates steel reinforcement needs via `get_reinforcement_requirement`, and finds the necessary embedment length using `get_development_length`. It accounts for soil bearing capacity, column loads, moments, and material strengths.


## Available Tools (4)
- **get_development_length**: Calculates the required embedment length for the reinforcement bars
- **get_footing_dimensions**: Calculates the required length and width of the footing based on soil capacity and loads
- **get_footing_thickness**: Determines the required depth of the footing to resist shear forces
- **get_reinforcement_requirement**: Calculates the area and spacing of steel reinforcement needed for bending


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Isolated Rectangular Footing Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the footing dimensions for a 500kN load and 50kNm moment on soil with 150kPa capacity, with a 300x300mm column."

**🤖 AI Agent:**
> The required footing dimensions are 2.1m by 2.1m with an area of 4.41m².

---

**👤 You:**
> "What is the required thickness for a footing with a 500kN load and 50kNm moment, using 25MPa concrete?"

**🤖 AI Agent:**
> The required footing depth is 450mm to satisfy shear requirements.

---

**👤 You:**
> "How much steel is needed for a 2.1m x 2.1m footing with 450mm depth and 460MPa steel?"

**🤖 AI Agent:**
> The required longitudinal steel area is 1250mm² with a suggested bar diameter of 16mm.


## ❓ FAQ

**Q: What inputs are required for footing design?**
You need to provide the column load, bending moment, soil bearing capacity, column dimensions, concrete strength, and steel yield strength.

**Q: How does the tool handle shear checks?**
The `get_footing_thickness` tool evaluates both one-way shear and two-way punching shear to ensure the footing depth is sufficient.

**Q: Can I design for different soil types?**
Yes, simply input the specific soil bearing capacity (kPa) for your site into the dimensioning tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/isolated-rectangular-footing-designer](https://vinkius.com/ai-agent-connect/isolated-rectangular-footing-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Isolated Rectangular Footing Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `isolated-rectangular-footing-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Isolated Rectangular Footing Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "isolated-rectangular-footing-designer": {
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
