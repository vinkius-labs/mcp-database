# Reservoir Limit Test MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/reservoir-limit-test)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Identify geological boundaries, drainage areas, and aquifer support using pressure transient analysis.

## Description
This MCP server provides specialized tools for reservoir engineering. It allows AI agents to analyze pressure transient data to determine reservoir limits. Use `get_boundary_type` to identify no-flow or constant pressure boundaries, `calculate_drainage_area` to estimate the active drainage volume, `detect_faults_and_channels` to find linear geological features, and `evaluate_aquifer_support` to quantify water drive influence.


## Available Tools (4)
- **calculate_drainage_area**: Estimates the total area of the reservoir currently being drained by the well
- **detect_faults_and_channels**: Identifies the presence of linear features like faults or narrow channel geometries
- **evaluate_aquifer_support**: Quantifies the degree to which an external water source is maintaining reservoir pressure
- **get_boundary_type**: Identifies the nature of the reservoir limits based on pressure trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Reservoir Limit Test** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the boundary type for this pressure data?"

**🤖 AI Agent:**
> The reservoir exhibits a no-flow boundary with a confidence score of 0.85.

---

**👤 You:**
> "Calculate the drainage area for the current well."

**🤖 AI Agent:**
> The estimated drainage area is 450 acres with a shape factor of radial.

---

**👤 You:**
> "Are there any faults detected in this flow regime?"

**🤖 AI Agent:**
> Yes, a linear fault has been detected with an orientation of 45 degrees.


## ❓ FAQ

**Q: How can I identify if a reservoir has a no-flow boundary?**
You can use the `get_boundary_type` tool. By providing pressure data and production history, the tool analyzes the pressure derivative to detect sudden increases that indicate a no-flow boundary.

**Q: Can this tool detect faults in the reservoir?**
Yes, the `detect_faults_and_channels` tool identifies linear features like faults or narrow channel geometries by analyzing the pressure derivative and the identified flow regime.

**Q: How is the drainage area calculated?**
The `calculate_drainage_area` tool estimates the area by correlating the rate of pressure depletion with fluid transmissibility and viscosity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/reservoir-limit-test](https://vinkius.com/en/ai-agent-connect/reservoir-limit-test)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Reservoir Limit Test** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `reservoir-limit-test` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Reservoir Limit Test** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "reservoir-limit-test": {
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
