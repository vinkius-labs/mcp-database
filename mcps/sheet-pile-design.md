# Sheet Pile Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sheet-pile-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Structural and geotechnical design for cantilever and anchored sheet pile walls.

## Description
This MCP server provides essential engineering calculations for sheet pile wall design. It allows AI agents to determine structural requirements for both cantilever and anchored configurations. Use `calculate_cantilever_wall` for unsupported walls, `calculate_anchored_wall` to find waling forces and embedment for anchored systems, `evaluate_seepage_risk` to assess piping stability, and `get_pile_section_modulus` to select appropriate steel profiles from the catalog.


## Available Tools (4)
- **calculate_anchored_wall**: Calculates the requirements for a sheet pile wall supported by a horizontal anchor system
- **calculate_cantilever_wall**: Calculates the structural and depth requirements for a single, unsupported sheet pile wall
- **evaluate_seepage_risk**: Assesses the stability of the wall against water flow and piping
- **get_pile_section_modulus**: Identifies suitable commercial sheet pile sections based on a required capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sheet Pile Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the requirements for a cantilever sheet pile wall with a height of 5m, soil density of 18 kN/m³, and friction angle of 30 degrees."

**🤖 AI Agent:**
> The required embedment depth is 4.2 meters and the required section modulus is 1250 cm³.

---

**👤 You:**
> "What is the risk of piping if the water level front is 2m, back is 0.5m, permeability is 1e-4 m/s, and embedment is 3m?"

**🤖 AI Agent:**
> The exit gradient is 0.15 and the piping risk is low with a safety factor of 2.5.

---

**👤 You:**
> "Find available steel profiles for a required section modulus of 800 cm³."

**🤖 AI Agent:**
> Available profiles include Profile-A (950 cm³, 85 kg/m) and Profile-B (1100 cm³, 92 kg/m).


## ❓ FAQ

**Q: What is the difference between cantilever and anchored wall calculations?**
A cantilever wall is self-supporting and relies on embedment depth, while an anchored wall uses a horizontal support to reduce bending moments and required depth.

**Q: How can I find a suitable steel profile for my design?**
After calculating the required capacity, use the `get_pile_section_modulus` tool to retrieve a list of available steel profiles that meet your minimum section modulus.

**Q: Can this tool account for water-induced soil instability?**
Yes, the `evaluate_seepage_risk` tool assesses the stability of the wall against water flow and calculates the risk of piping.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sheet-pile-design](https://vinkius.com/ai-agent-connect/sheet-pile-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sheet Pile Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sheet-pile-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sheet Pile Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sheet-pile-design": {
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
