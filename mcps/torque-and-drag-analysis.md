# Torque and Drag Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/torque-and-drag-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates hook load, surface torque, side forces, and buckling risk for wellbore operations.

## Description
This MCP server provides critical mechanical analysis for drilling and completion operations. It connects AI agents to specialized models that calculate `get_hook_load` to determine surface weight, `get_surface_torque` for rotational resistance, `get_side_forces` to identify contact forces, and `check_buckling_risk` to evaluate structural stability. The tools account for wellbore trajectory, pipe properties, mud weight, and friction factors across drilling, casing, and completion phases.


## Available Tools (4)
- **check_buckling_risk**: Evaluates the likelihood of the drill string or completion assembly undergoing buckling
- **get_hook_load**: Determines the total weight experienced at the surface hook for a given string
- **get_side_forces**: Calculates the contact forces between the pipe and the wellbore wall at various points
- **get_surface_torque**: Calculates the rotational resistance applied at the surface during drilling operations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Torque and Drag Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected hook load for my current drilling string?"

**🤖 AI Agent:**
> The calculated hook load for the specified trajectory and pipe properties is 250,000 lbs.

---

**👤 You:**
> "Is there a risk of the drill string buckling under this load?"

**🤖 AI Agent:**
> The analysis shows a safety factor of 1.5 against sinusoidal buckling, indicating low risk.

---

**👤 You:**
> "Calculate the surface torque for the current drilling operation."

**🤖 AI Agent:**
> The surface torque is calculated at 15,000 ft-lbs.


## ❓ FAQ

**Q: What operations are supported?**
The tools support drilling, casing, and completion operations.

**Q: How is buckling risk assessed?**
The `check_buckling_risk` tool evaluates the likelihood of sinusoidal or helical buckling by comparing axial loads against critical thresholds based on wellbore geometry.

**Q: Can I calculate surface torque during casing?**
No, the `get_surface_torque` tool is specifically designed for drilling operations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/torque-and-drag-analysis](https://vinkius.com/en/ai-agent-connect/torque-and-drag-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Torque and Drag Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `torque-and-drag-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Torque and Drag Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "torque-and-drag-analysis": {
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
