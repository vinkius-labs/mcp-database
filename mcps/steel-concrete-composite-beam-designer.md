# Steel-Concrete Composite Beam Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-concrete-composite-beam-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design composite steel-concrete beams using AISC methodologies, calculating moment capacity, shear studs, and deflection.

## Description
This MCP server provides structural engineering tools for designing composite steel-concrete beams according to AISC standards. It allows engineers to calculate the `get_moment_capacity` for a specific steel section and concrete slab combination, determine the necessary `calculate_shear_studs` requirements for desired composite action, and compute `get_beam_deflection` under applied loads. Finally, use `validate_design_compliance` to ensure the design meets serviceability and strength limits.


## Available Tools (4)
- **get_beam_deflection**: Calculates the maximum vertical displacement of the beam under the specified load
- **get_moment_capacity**: Determines the maximum bending moment the composite beam can resist
- **calculate_shear_studs**: Determines the required number and spacing of shear studs to achieve the desired level of composite action
- **validate_design_compliance**: Checks if the current design meets standard AISC serviceability and strength limits


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel-Concrete Composite Beam Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the moment capacity for a 10m beam with a 20 kN/m load, using a W12X26 steel section, 150mm concrete slab, and 30 MPa concrete strength."

**🤖 AI Agent:**
> The composite moment capacity for the specified W12X26 beam is 450 kNm.

---

**👤 You:**
> "How much deflection will a 12m beam with a 15 kN/m load experience if it uses a W14X30 section and a 120mm concrete slab (35 MPa)?"

**🤖 AI Agent:**
> The maximum vertical deflection for this beam is 18.5 mm.

---

**👤 You:**
> "How many shear studs are needed for a 8m beam with 25 kN/m load, W18X35 section, 100mm slab, and 25 MPa concrete for full composite action?"

**🤖 AI Agent:**
> To achieve full composite action, 42 shear studs are required with a minimum spacing of 150 mm.


## ❓ FAQ

**Q: What design standards does this tool follow?**
The tool follows AISC methodologies for composite steel-concrete beam design.

**Q: Can I design for partial composite action?**
Yes, you can use `calculate_shear_studs` with a target degree of composite between 0 and 1 to design for partial action.

**Q: How do I check if my beam is safe?**
You can use the `validate_design_compliance` tool to check if your applied moment and deflection are within AISC limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-concrete-composite-beam-designer](https://vinkius.com/ai-agent-connect/steel-concrete-composite-beam-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel-Concrete Composite Beam Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-concrete-composite-beam-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel-Concrete Composite Beam Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-concrete-composite-beam-designer": {
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
