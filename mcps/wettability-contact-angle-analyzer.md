# Wettability & Contact Angle Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wettability-contact-angle-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculate surface energy, work of adhesion, and spreading coefficients using contact angle data.

## Description
This MCP server provides specialized computational tools for surface science. It uses the Owens-Wendt and Fowkes models to determine the total surface energy and its dispersive and polar components from contact angle measurements. Users can calculate the work of adhesion and the spreading coefficient for specific liquid-solid pairs, and categorize the resulting wettability regime. Key tools include `calculate_surface_energy` for component breakdown, `calculate_adhesion_metrics` for adhesion strength, and `analyze_wettability_regime` for behavior classification.


## Available Tools (4)
- **analyze_wettability_regime**: Categorizes the wettability behavior of a liquid-solid pair
- **calculate_surface_energy**: Determines the total surface energy and its component breakdown using the OWRK/Fowkes models
- **calculate_adhesion_metrics**: Calculates the work of adhesion and the spreading coefficient for a specific liquid on a known surface
- **validate_measurement_consistency**: Checks if the provided contact angle measurements and surface tension components are physically consistent with the OWRK model


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wettability & Contact Angle Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the surface energy using two liquids: Water (total 72.8, dispersive 21.8, polar 51.0) and Diiodomethane (total 50.8, dispersive 50.8, polar 0.0) with contact angles of 45 and 10 degrees."

**🤖 AI Agent:**
> The calculated total surface energy is 42.5 mN/m, with a dispersive component of 28.2 mN/m and a polar component of 14.3 mN/m.

---

**👤 You:**
> "What is the spreading coefficient for a liquid with total surface tension 30, dispersive 25, and polar 5 on a solid with surface energy 50, dispersive 40, and polar 10, given a contact angle of 20 degrees?"

**🤖 AI Agent:**
> The spreading coefficient is 15.0 and the work of adhesion is 42.4 mN/m.

---

**👤 You:**
> "Determine the wettability regime for a contact angle of 110 degrees and a spreading coefficient of -15."

**🤖 AI Agent:**
> The wettability regime is Non-wetting.


## ❓ FAQ

**Q: What models are used for surface energy calculation?**
The server implements the Owens-Wendt-Rabel-Kaelble (OWRK) and Fowkes models to solve for dispersive and polar components.

**Q: How many liquids are required for surface energy determination?**
At least two liquids with known surface tension components are required to solve the OWRK equations via `calculate_surface_energy`.

**Q: Can I check if my measurements are physically consistent?**
Yes, the `validate_measurement_consistency` tool checks if your contact angles and surface tension components align with the OWRK model.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wettability-contact-angle-analyzer](https://vinkius.com/ai-agent-connect/wettability-contact-angle-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wettability & Contact Angle Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wettability-contact-angle-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wettability & Contact Angle Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wettability-contact-angle-analyzer": {
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
