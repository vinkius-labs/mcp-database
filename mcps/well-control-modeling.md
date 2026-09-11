# Well Control Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/well-control-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate kill mud weight, generate kill sheets, and simulate pressure profiles for well control operations.

## Description
This MCP server provides critical calculation tools for managing well control during a kick. It allows users to determine the necessary `calculate_kill_mud_weight` to stabilize the well, generate operational parameters for both the Driller's Method via `generate_kill_sheet_driller` and the Wait-and-Weight Method via `generate_kill_sheet_wait_and_weight`, and visualize the vertical pressure distribution using `simulate_pressure_profile`.


## Available Tools (4)
- **calculate_kill_mud_weight**: Determines the required density of the replacement fluid to stabilize the well
- **generate_kill_sheet_driller**: Provides the operational parameters for the Driller's Method (two-stage circulation)
- **generate_kill_sheet_wait_and_weight**: Provides the operational parameters for the Wait-and-Weight Method (single-stage circulation)
- **simulate_pressure_profile**: Visualizes the pressure distribution across the wellbore during a kill operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Control Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the kill mud weight for a well with current mud weight of 10.0 ppg, shut-in drill pipe pressure of 500 psi, and a true vertical depth of 10000 ft."

**🤖 AI Agent:**
> The required kill mud weight is 10.5 ppg with a pressure safety margin of 0.5 ppg.

---

**👤 You:**
> "Generate a kill sheet for the Driller's Method with an influx volume of 50 bbl, gas type, current mud weight of 10.0 ppg, kill mud weight of 11.0 ppg, and drill pipe capacity of 0.015 bbl/ft."

**🤖 AI Agent:**
> Circulation one requires a constant bottomhole pressure of 500 psi. Circulation two requires replacing the mud with 11.0 ppg fluid. Total estimated time is 4 hours.

---

**👤 You:**
> "Simulate the pressure profile for a well with mud densities [10.0, 10.0, 10.0], an influx density of 0.1, at a depth of 5000 ft."

**🤖 AI Agent:**
> The pressure profile shows a total hydrostatic pressure of 5200 psi at the bottom of the well.


## ❓ FAQ

**Q: How do I calculate the required kill mud weight?**
You can use the `calculate_kill_mud_weight` tool by providing the current mud weight, the shut-in drill pipe pressure, and the true vertical depth.

**Q: What is the difference between the two kill methods provided?**
The `generate_kill_sheet_driller` tool provides parameters for the two-stage Driller's Method, while `generate_kill_sheet_wait_and_weight` provides parameters for the single-stage Wait-and-Weight Method.

**Q: Can I visualize the pressure in the wellbore?**
Yes, the `simulate_pressure_profile` tool generates a depth-to-pressure map to visualize the distribution throughout the wellbore.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/well-control-modeling](https://vinkius.com/en/ai-agent-connect/well-control-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Control Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-control-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Control Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-control-modeling": {
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
