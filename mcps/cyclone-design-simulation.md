# Cyclone Design Simulation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cyclone-design-simulation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design hydrocyclone circuits by calculating dimensions, capacity, and efficiency.

## Description
This MCP server provides a complete suite of tools for hydrocyclone classification design. It allows engineers to determine optimal physical dimensions using `calculate_single_cyclone_dimensions`, calculate the required number of units with `estimate_system_capacity`, evaluate separation performance via `predict_classification_efficiency`, and ensure operational stability with `validate_design_feasibility`. It bridges the gap between slurry properties and physical cyclone geometry.


## Available Tools (4)
- **calculate_single_cyclone_dimensions**: Determines the optimal physical dimensions for a single cyclone unit based on target performance
- **estimate_system_capacity**: Calculates how many cyclones are needed to meet the total process requirement
- **predict_classification_efficiency**: Evaluates the separation sharpness and efficiency of a designed cyclone
- **validate_design_feasibility**: Checks if a specific set of dimensions and slurry properties will result in a stable, non-clogging operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cyclone Design Simulation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a cyclone with a target cut size of 50 microns, slurry density of 1200 kg/m3, viscosity of 0.001 Pa·s, and throughput of 100 m3/h."

**🤖 AI Agent:**
> The calculated cyclone diameter is 450mm, with a vortex finder diameter of 120mm and a spigot diameter of 45mm.

---

**👤 You:**
> "How many cyclones are needed if each unit handles 25 m3/h and the total throughput is 150 m3/h?"

**🤖 AI Agent:**
> You will need 6 cyclones to meet the total throughput of 150 m3/h.

---

**👤 You:**
> "Is a design with a 300mm diameter, 30mm spigot, and 40 micron cut size feasible?"

**🤖 AI Agent:**
> The design is infeasible due to a high risk of clogging because the spigot diameter is too small for the target cut size.


## ❓ FAQ

**Q: How do I determine the size of a single cyclone?**
You can use the `calculate_single_cyclone_dimensions` tool by providing the target cut size, slurry density, viscosity, and required throughput.

**Q: Can I check if my design will clog?**
Yes, use `validate_design_feasibility` to check for clogging risks based on the spigot diameter and target cut size.

**Q: How many cyclones do I need for my process?**
Use the `estimate_system_capacity` tool after you have determined the capacity of a single unit.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cyclone-design-simulation](https://vinkius.com/ai-agent-connect/cyclone-design-simulation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cyclone Design Simulation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cyclone-design-simulation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cyclone Design Simulation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cyclone-design-simulation": {
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
