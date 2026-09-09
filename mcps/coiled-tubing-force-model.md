# Coiled Tubing Force Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/coiled-tubing-force-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates mechanical and hydraulic forces for coiled tubing operations.

## Description
This MCP server provides specialized engineering calculations for coiled tubing (CT) operations. It allows AI agents to determine axial forces using `calculate_mechanical_loads`, evaluate structural stability with `check_buckling_stability`, determine circulation pressures via `calculate_hydraulic_profile`, and calculate the final net force at the bottom of the hole using `calculate_weight_on_bit`.


## Available Tools (4)
- **calculate_hydraulic_profile**: Determines the pressures required for fluid circulation
- **calculate_mechanical_loads**: Determines the axial forces (tension and compression) acting along the length of the coiled tubing
- **calculate_weight_on_bit**: Provides the final net force being applied to the tool at the bottom of the hole
- **check_buckling_stability**: Evaluates if the coiled tubing is at risk of losing structural stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coiled Tubing Force Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the weight on bit if the effective weight is 5000, axial force is 1000, and the tubing is buckled?"

**🤖 AI Agent:**
> The weight on bit is 1000 with a significantly reduced weight transfer efficiency due to the buckled state.

---

**👤 You:**
> "Calculate the mechanical loads for a tripping in operation with specific CT dimensions and wellbore geometry."

**🤖 AI Agent:**
> The axial force is 4500, with a tension of 4500 and an effective weight of 4500.

---

**👤 You:**
> "Check if the tubing will buckle with an axial force of 2000."

**🤖 AI Agent:**
> The tubing is stable with a safety factor of 1.5 and no buckling detected.


## ❓ FAQ

**Q: How does the model handle friction?**
The model adjusts the effective weight by subtracting friction during tripping in and adding it during tripping out, as calculated by `calculate_mechanical_loads`.

**Q: Can I check for buckling risks?**
Yes, you can use `check_buckling_stability` to evaluate if the tubing is at risk of sinusoidal or helical buckling.

**Q: What is included in the hydraulic profile?**
The `calculate_hydraulic_profile` tool provides circulation pressure, pressure drops inside the tubing and annulus, and the bottom hole pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/coiled-tubing-force-model](https://vinkius.com/ai-agent-connect/coiled-tubing-force-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coiled Tubing Force Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coiled-tubing-force-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coiled Tubing Force Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coiled-tubing-force-model": {
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
