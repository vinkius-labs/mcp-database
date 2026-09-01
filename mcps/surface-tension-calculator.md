# Surface Tension Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/surface-tension-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates surface tension, capillary rise, and work of cohesion.

## Description
This MCP server provides specialized tools for fluid dynamics analysis. It allows AI agents to calculate the effective surface tension of liquids using `calculate_surface_tension`, determine vertical capillary rise with `calculate_capillary_rise`, compute the energy required for surface separation via `calculate_work_of_cohesion`, and interpret liquid-surface interactions using `analyze_wetting_behavior`.


## Available Tools (4)
- **analyze_wetting_behavior**: g., Perfect Wetting, High Wettability) based on the contact angle.

Interprets the contact angle to describe how the liquid interacts with the tube surface
- **calculate_surface_tension**: Determines the effective surface tension of a liquid, accounting for the presence of surfactants
- **calculate_capillary_rise**: Calculates the vertical height a liquid will rise in a specific tube
- **calculate_work_of_cohesion**: Calculates the energy required to separate the liquid surface


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surface Tension Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the capillary rise for water with a surface tension of 0.072 N/m, density of 1000 kg/m³, and a tube radius of 0.001 m with a contact angle of 0 degrees?"

**🤖 AI Agent:**
> The capillary rise for the water in a 1mm radius tube is approximately 0.0353 meters.

---

**👤 You:**
> "Calculate the work of cohesion for a liquid with a surface tension of 0.05 N/m."

**🤖 AI Agent:**
> The work of cohesion for the liquid is 0.05 J/m².

---

**👤 You:**
> "How would a liquid with a contact angle of 150 degrees interact with a surface?"

**🤖 AI Agent:**
> A liquid with a contact angle of 150 degrees is categorized as Non-Wetting.


## ❓ FAQ

**Q: What can I calculate with this server?**
You can calculate effective surface tension, capillary rise height, work of cohesion, and analyze wetting behavior based on contact angles.

**Q: Does it account for surfactants?**
Yes, the `calculate_surface_tension` tool allows you to input surfactant concentration to find the effective surface tension.

**Q: How do I connect this to my AI client?**
You can connect using your personal Connection Token via Vinkius Edge. It is compatible with Cursor, VS Code, Claude Desktop, and Windsurf.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/surface-tension-calculator](https://vinkius.com/ai-agent-connect/surface-tension-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surface Tension Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surface-tension-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surface Tension Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surface-tension-calculator": {
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
