# Proppant Transport Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/proppant-transport-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulates proppant settling and concentration within hydraulic fractures.

## Description
This MCP server provides specialized tools for modeling proppant transport during hydraulic fracturing. It allows AI agents to calculate `calculate_settling_velocity` for specific particles, predict the `calculate_concentration_profile` across fracture lengths, and estimate the `calculate_bank_height` at the bottom of the fracture. For a complete overview of the transport state, use `simulate_transport_dynamics` to aggregate settling and concentration data into a single summary.


## Available Tools (4)
- **calculate_bank_height**: Estimates the thickness of the accumulated proppant bed at the bottom of the fracture
- **calculate_concentration_profile**: Predicts the distribution of proppant concentration across the fracture
- **calculate_settling_velocity**: Determines the speed at which a specific proppant particle falls through a given fluid
- **simulate_transport_dynamics**: Provides a high-level overview of the transport state by combining settling and concentration data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Proppant Transport Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the settling velocity for a proppant with density 2650, diameter 0.0005, fluid viscosity 0.1, and fluid density 1000?"

**🤖 AI Agent:**
> The calculated settling velocity for the specified proppant is 0.025 m/s.

---

**👤 You:**
> "Estimate the proppant bank height for a fracture with width 0.05, height 0.1, concentration 0.2, and volume fraction 0.6."

**🤖 AI Agent:**
> The estimated height of the accumulated proppant bed is 0.02 meters.

---

**👤 You:**
> "Provide a transport summary for a fluid with power-law rheology and proppant data with density 2600 and diameter 0.0004, in a fracture of 100x0.05x0.1."

**🤖 AI Agent:**
> The transport summary shows an average settling velocity of 0.022 m/s, a peak concentration of 0.25, and an estimated bank height of 0.015 meters.


## ❓ FAQ

**Q: What can I calculate with this model?**
You can calculate proppant settling velocity, the concentration profile along the fracture, the height of the proppant bank, and a complete transport summary using `simulate_transport_dynamics`.

**Q: Does the model account for non-Newtonian fluids?**
Yes, the model is designed to handle non-Newtonian fluid rheology profiles to accurately predict how viscosity affects particle settling.

**Q: How do I connect this to my AI client?**
Connect via Vinkius Edge using your personal Connection Token. This works with Cursor, VS Code, Claude Desktop, Windsurf, and any MCP-compatible client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/proppant-transport-model](https://vinkius.com/en/ai-agent-connect/proppant-transport-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Proppant Transport Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `proppant-transport-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Proppant Transport Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "proppant-transport-model": {
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
