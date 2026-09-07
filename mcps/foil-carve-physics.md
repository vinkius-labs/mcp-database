# Foil Carve Physics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/foil-carve-physics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate hydrofoil carving mechanics, bank angles, and structural loads.

## Description
This MCP server provides precise physics calculations for hydrofoil riders. Use `calculate_carve_physics` to determine the required bank angle, g-force, and mast load for any maneuver. You can also use `analyze_stability_limits` to check if a turn is stable, `estimate_rider_effort` to gauge physical demand, and `get_structural_safety_check` to evaluate equipment risk based on mast loading.


## Available Tools (4)
- **get_structural_safety_check**: Evaluates the risk of equipment failure based on mast loading
- **analyze_stability_limits**: Determines if a specific turn is stable based on the equipment configuration
- **calculate_carve_physics**: Provides a complete physics profile of a specific carving maneuver
- **estimate_rider_effort**: Estimates the physical demand on the rider for a given maneuver


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Foil Carve Physics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the physics for a turn at 5 m/s with a 10m radius, 120cm mast, 80kg rider, and 5.0 aspect ratio."

**🤖 AI Agent:**
> The required bank angle is 15.4 degrees, the rider will experience 1.2g, and the mast load is 980 N.

---

**👤 You:**
> "Is a turn with a 5m radius, 4 m/s speed, 4.0 aspect ratio, and 1.0 stabilizer factor stable?"

**🤖 AI Agent:**
> No, the maneuver is unstable with a stability margin of -0.15.

---

**👤 You:**
> "What is the safety rating for a mast load of 2500N on a 90cm mast?"

**🤖 AI Agent:**
> The safety rating is Caution, with a load percentage of 75%.


## ❓ FAQ

**Q: How do I calculate the required tilt for a turn?**
Use the `calculate_carve_physics` tool with your speed, turn radius, mast length, weight, and aspect ratio to find the necessary bank angle.

**Q: Can I check if my equipment is safe for a high-G turn?**
Yes, use `get_structural_safety_check` by providing the calculated mast load and mast length to receive a safety rating.

**Q: How is rider effort determined?**
The `estimate_rider_effort` tool calculates a normalized score based on the g-force, rider weight, and the radius of the turn.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/foil-carve-physics](https://vinkius.com/ai-agent-connect/foil-carve-physics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Foil Carve Physics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `foil-carve-physics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Foil Carve Physics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "foil-carve-physics": {
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
