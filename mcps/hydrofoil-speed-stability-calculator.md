# Hydrofoil Speed & Stability Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/hydrofoil-speed-stability-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate lift-off, stall, and optimal cruising speeds for hydrofoil setups.

## Description
This MCP server provides precise hydrodynamic calculations for hydrofoil enthusiasts. Use `calculate_lift_speeds` to determine the minimum speed required for lift-off, the stall speed, and the most efficient cruising velocity based on wing geometry and rider weight. You can also use `analyze_stability_envelope` to evaluate how anhedral and mast angles affect control, or `get_design_recommendations` to find the ideal wing configuration for racing, cruising, or beginner activities.


## Available Tools (4)
- **analyze_stability_envelope**: Evaluates how geometry (anhedral and mast angle) affects the rider's control range and stability
- **calculate_lift_speeds**: Determines the primary speed thresholds (lift-off, stall, and cruise) for a specific foil setup
- **compare_foil_configurations**: Allows a user to compare two different wing setups to see which provides a better speed or stability profile for a specific weight
- **get_design_recommendations**: Provides high-level guidance on which wing type to choose based on the user's goal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hydrofoil Speed & Stability Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the lift-off speed for a 75kg rider using a 1200cm2 wing with a 5 aspect ratio and 40cm fuselage?"

**🤖 AI Agent:**
> The required lift-off speed for your setup is 12.4 m/s.

---

**👤 You:**
> "Is a setup with 5 degrees of anhedral and 2 degrees of mast angle stable?"

**🤖 AI Agent:**
> The stability rating is Stable with Easy control difficulty.

---

**👤 You:**
> "Recommend a wing setup for a 80kg rider who wants to go racing."

**🤖 AI Agent:**
> For racing, a recommended front wing area is 950cm2 with an aspect ratio of 7.5 to maximize speed.


## ❓ FAQ

**Q: How do I calculate my lift-off speed?**
You can use the `calculate_lift_speeds` tool by providing the front wing area, aspect ratio, rider weight, and fuselage length.

**Q: Can I compare two different foil setups?**
Yes, use the `compare_foil_configurations` tool to see which setup provides a better speed or stability profile for your weight.

**Q: What should I choose for beginner riding?**
Use `get_design_recommendations` with the target activity set to 'beginner' to receive specific wing area and aspect ratio suggestions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/hydrofoil-speed-stability-calculator](https://vinkius.com/en/ai-agent-connect/hydrofoil-speed-stability-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hydrofoil Speed & Stability Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hydrofoil-speed-stability-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hydrofoil Speed & Stability Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hydrofoil-speed-stability-calculator": {
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
