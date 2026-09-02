# Zeta Potential Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/zeta-potential-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate zeta potential, surface charge, and colloidal stability from electrophoretic mobility.

## Description
This MCP server provides specialized tools for colloid science. Use `calculate_zeta_potential` to determine electrokinetic potential from mobility, viscosity, and dielectric constant. You can also use `estimate_surface_charge` to find physical charge values and `predict_colloidal_stability` to assess if a suspension will remain dispersed or aggregate. For common solvents, use `get_medium_properties` to retrieve standardized physical constants.


## Available Tools (4)
- **predict_colloidal_stability**: Evaluates whether a particle suspension is likely to be stable or prone to aggregation
- **estimate_surface_charge**: Converts the measured zeta potential into a physical surface charge value
- **calculate_zeta_potential**: Provide particle radius for Henry correction.

Determines the zeta potential of a particle based on its movement in a fluid
- **get_medium_properties**: Retrieves standardized physical constants for common solvents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zeta Potential Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the zeta potential for a particle with mobility 2.5e-8 m^2/Vs, viscosity 0.001 Pa·s, and dielectric constant 78.5."

**🤖 AI Agent:**
> The calculated zeta potential is -45.2 mV, assuming the Smoluchowski limit.

---

**👤 You:**
> "Is a suspension with a zeta potential of -35 mV stable?"

**🤖 AI Agent:**
> The suspension is classified as Highly Stable with a stability score of 0.85.

---

**👤 You:**
> "What are the properties of water?"

**🤖 AI Agent:**
> For water, the dielectric constant is 78.5 and the dynamic viscosity is 0.001 Pa·s.


## ❓ FAQ

**Q: How do I calculate zeta potential?**
You can use the `calculate_zeta_potential` tool by providing the electrophoretic mobility, viscosity, and dielectric constant of the medium.

**Q: Can I predict if my suspension is stable?**
Yes, use the `predict_colloidal_stability` tool with your calculated zeta potential to get a stability status and score.

**Q: What is Henry's correction?**
Henry's correction is applied via the `calculate_zeta_potential` tool when a particle radius is provided, adjusting the calculation between the Smoluchowski and Hückel limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/zeta-potential-calculator](https://vinkius.com/ai-agent-connect/zeta-potential-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zeta Potential Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zeta-potential-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zeta Potential Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zeta-potential-calculator": {
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
