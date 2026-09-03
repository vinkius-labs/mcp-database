# Concrete Transfer Slab Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-transfer-slab-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design reinforced concrete transfer slabs using strut-and-tie modeling.

## Description
This MCP server provides specialized structural engineering tools for designing heavy-duty transfer slabs. It uses the strut-and-tie method to model internal force flow, ensuring stability under heavy column loads. Use `analyze_load_path` to identify critical stress zones, `calculate_slab_thickness` to determine required depth, `design_reinforcement_layout` for steel tie specifications, and `calculate_shear_reinforcement` to prevent shear failure near column heads.


## Available Tools (4)
- **calculate_shear_reinforcement**: Determine the specific steel needed to prevent shear failure near column heads or high-stress zones
- **calculate_slab_thickness**: Determine the minimum required depth of the slab to satisfy strength and serviceability
- **design_reinforcement_layout**: Specify the steel reinforcement required to act as the ties in the strut-and-tie model
- **analyze_load_path**: Determine how forces migrate through the slab and identify critical stress zones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Transfer Slab Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the load path for a slab with a 6m span and these loads: [{"loadValue": 500, "position": "(0,0)"}, {"loadValue": 500, "position": "(6,0)"}] with a column layout of 'grid 2x2'."

**🤖 AI Agent:**
> The load path is direct with a low risk level. No critical stress zones were identified for this configuration.

---

**👤 You:**
> "What is the required thickness for a 5m span slab with 1000kN loads and 30MPa concrete?"

**🤖 AI Agent:**
> The required thickness is 650mm using the strength-based control method.

---

**👤 You:**
> "Design the reinforcement for a 500mm thick slab with 30MPa concrete and these loads: [{"loadValue": 800, "position": "(2,2)"}]."

**🤖 AI Agent:**
> The reinforcement layout requires a 20mm bar diameter with 150mm spacing.


## ❓ FAQ

**Q: What design method is used for the slab?**
The server utilizes the strut-and-tie method to model the internal force flow as a truss system of concrete struts and steel ties.

**Q: How do I determine the required slab depth?**
You can use the `calculate_slab_thickness` tool, providing the column layout, transferred loads, span, concrete strength, and deflection limits.

**Q: Can this tool help prevent shear failure?**
Yes, the `calculate_shear_reinforcement` tool calculates the specific stirrup diameter and spacing needed to prevent shear failure in high-stress zones.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-transfer-slab-designer](https://vinkius.com/ai-agent-connect/concrete-transfer-slab-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Transfer Slab Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-transfer-slab-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Transfer Slab Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-transfer-slab-designer": {
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
