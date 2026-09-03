# Concrete One-Way Slab Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-one-way-slab-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design reinforced concrete one-way slabs with thickness, reinforcement, and serviceability checks.

## Description
This MCP server provides structural engineering tools to design reinforced concrete one-way slabs. It calculates the required slab thickness to satisfy deflection limits, determines the main reinforcement needed to resist bending moments, and calculates temperature reinforcement to control thermal cracking. You can also use `verify_serviceability` to perform a final validation of the design against structural limits. It supports various support conditions including simply supported, continuous, and cantilever spans.


## Available Tools (4)
- **calculate_slab_thickness**: Determines the minimum required thickness of the slab to satisfy structural integrity and deflection limits
- **verify_serviceability**: Performs a final validation of the design against deflection and crack control limits
- **calculate_main_reinforcement**: Calculates the amount of primary steel required to resist bending moments
- **calculate_temperature_reinforcement**: Calculates the secondary steel required to control cracking from thermal effects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete One-Way Slab Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required thickness for a 5m span slab with a 10 kN/m² load, 30 MPa concrete, and 500 MPa steel, assuming it is simply supported."

**🤖 AI Agent:**
> The required slab thickness is 125 mm, and the deflection check is successful.

---

**👤 You:**
> "How much main reinforcement is needed for a 4m span, 150mm thick slab with 12 kN/m² load, 30 MPa concrete, and 500 MPa steel on a continuous support?"

**🤖 AI Agent:**
> The required main reinforcement area is 450 mm² per meter, using 12mm diameter bars spaced at 250mm.

---

**👤 You:**
> "Calculate temperature reinforcement for a 150mm thick slab with 500 MPa steel."

**🤖 AI Agent:**
> The required temperature reinforcement is 220 mm² per meter, using 10mm diameter bars spaced at 360mm.


## ❓ FAQ

**Q: What support conditions are supported?**
The tool supports simply_supported, continuous, and cantilever conditions.

**Q: How do I check if my slab design is safe?**
You can use the `verify_serviceability` tool to validate the design against deflection and crack control limits.

**Q: Does this tool calculate temperature reinforcement?**
Yes, the `calculate_temperature_reinforcement` tool calculates the secondary steel required to control cracking from thermal effects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-one-way-slab-designer](https://vinkius.com/ai-agent-connect/concrete-one-way-slab-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete One-Way Slab Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-one-way-slab-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete One-Way Slab Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-one-way-slab-designer": {
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
