# Drilling Hydraulics Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/drilling-hydraulics-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Compute critical drilling parameters like ECD, pressure losses, and hole cleaning efficiency.

## Description
This MCP server provides a technical toolset for calculating essential drilling hydraulics. It allows AI agents to determine total pressure losses using `calculate_pressure_losses`, compute annular velocity via `calculate_annular_velocity`, and evaluate formation integrity with `calculate_ecd`. Additionally, it assesses hole cleaning effectiveness through `calculate_hole_cleaning` based on fluid rheology and wellbore geometry.


## Available Tools (4)
- **calculate_ecd**: Computes the Equivalent Circulating Density (ECD) to ensure formation integrity
- **calculate_hole_cleaning**: Evaluates the effectiveness of the fluid in removing cuttings from the wellbore
- **calculate_annular_velocity**: Calculates the speed of fluid movement in the annular space
- **calculate_pressure_losses**: Determines the total pressure drop in the system caused by fluid friction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Drilling Hydraulics Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total pressure loss for a system with a flow rate of 500 gpm using a Bingham Plastic model."

**🤖 AI Agent:**
> The total pressure loss for the specified system is 450 psi, consisting of 300 psi pipe loss and 150 psi annulus loss.

---

**👤 You:**
> "What is the annular velocity if the flow rate is 600 gpm and the wellbore diameter is 8.5 inches with a 5 inch drillpipe?"

**🤖 AI Agent:**
> The annular velocity is 185.4 ft/min with a flow area of 0.185 sq ft.

---

**👤 You:**
> "Calculate the ECD for a static mud density of 10 ppg and an annulus pressure loss of 200 psi at a depth of 10,000 ft."

**🤖 AI Agent:**
> The Equivalent Circulating Density (ECD) is 10.37 ppg.


## ❓ FAQ

**Q: What rheology models are supported?**
The tool supports both Bingham Plastic and Power-Law models for fluid rheology calculations.

**Q: How is ECD calculated?**
The `calculate_ecd` tool computes the Equivalent Circulating Density by combining static mud density with the pressure loss in the annulus relative to the true vertical depth.

**Q: Can I calculate hole cleaning efficiency?**
Yes, use `calculate_hole_cleaning` to evaluate how effectively the fluid removes cuttings based on annular velocity and cuttings properties.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/drilling-hydraulics-calculator](https://vinkius.com/en/ai-agent-connect/drilling-hydraulics-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Drilling Hydraulics Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `drilling-hydraulics-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Drilling Hydraulics Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "drilling-hydraulics-calculator": {
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
