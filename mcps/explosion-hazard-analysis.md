# Explosion Hazard Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/explosion-hazard-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Analyze explosion risks, overpressure, and safe standoff distances for flammable materials.

## Description
This MCP server provides critical safety analysis for flammable environments. It allows AI agents to evaluate material flammability using `evaluate_material_hazard`, estimate physical impact with `calculate_explosion_impact`, and determine necessary standoff distances via `determine_safe_distances`. It also assesses ignition potential through `assess_ignition_risk` to ensure personnel and infrastructure safety.


## Available Tools (4)
- **assess_ignition_risk**: Evaluates if existing ignition sources are sufficient to trigger an explosion
- **calculate_explosion_impact**: Estimates the physical intensity of an explosion based on the material and its confinement
- **determine_safe_distances**: Calculates the required standoff distances to protect personnel and infrastructure
- **evaluate_material_hazard**: Determines the fundamental flammability risk of a specific material


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Explosion Hazard Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is a 5% concentration of Hydrogen flammable?"

**🤖 AI Agent:**
> Yes, Hydrogen is highly flammable at a 5% concentration.

---

**👤 You:**
> "What is the safe distance for personnel if the overpressure is 5 kPa?"

**🤖 AI Agent:**
> The required safe distance for personnel is 150 meters.

---

**👤 You:**
> "Will a 2kJ spark ignite Methane at 4% concentration?"

**🤖 AI Agent:**
> Yes, the available energy exceeds the minimum ignition energy for Methane at this concentration.


## ❓ FAQ

**Q: How do I calculate the safe distance for a specific explosion?**
First, use `calculate_explosion_impact` to find the peak overpressure, then pass that value to `determine_safe_distances` specifying your target type.

**Q: Can this tool identify if a material is currently in a flammable range?**
Yes, the `evaluate_material_hazard` tool checks the concentration against the Lower and Upper Flammability Limits to determine risk.

**Q: What types of targets can I protect?**
You can calculate distances for personnel, light structures, and heavy structures.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/explosion-hazard-analysis](https://vinkius.com/ai-agent-connect/explosion-hazard-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Explosion Hazard Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `explosion-hazard-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Explosion Hazard Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "explosion-hazard-analysis": {
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
