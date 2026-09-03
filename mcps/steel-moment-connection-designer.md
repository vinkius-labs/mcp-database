# Steel Moment Connection Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-moment-connection-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Automated AISC-compliant design for steel moment connections, including plate, bolt, and weld calculations.

## Description
This MCP server provides specialized structural engineering tools to design steel moment connections following AISC standards. It automates the calculation of flange plate dimensions, web plate thickness, bolt requirements, and weld sizes. The toolset accounts for critical structural behaviors such as prying action and panel zone shear to ensure safety and compliance. Use `calculate_connection_design` for full designs, `validate_prying_action` to assess secondary tension forces, and `check_panel_zone_capacity` to verify column web strength.


## Available Tools (4)
- **check_panel_zone_capacity**: Verifies if the column web can withstand the shear force transferred by the moment connection
- **get_material_properties**: Retrieves the mechanical properties of a specific steel grade
- **calculate_connection_design**: Performs the complete structural design for a specific moment connection
- **validate_prying_action**: Determines if prying forces are significant enough to require design adjustments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Moment Connection Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a flange plate connection for a W14x90 beam and a W24x68 column using A992 steel with a moment of 150 kNm and shear of 50 kN."

**🤖 AI Agent:**
> The design for the flange plate connection requires a flange plate width of 12 inches, a thickness of 0.75 inches, and 4 bolts of 3/4 inch diameter with 3-inch spacing. The weld size is calculated at 5/16 inch, and the panel zone check passed.

---

**👤 You:**
> "Check if a 0.5 inch thick plate with 0.75 inch bolts and 1.5 inch edge distance will experience significant prying action under 40 kN of tension."

**🤖 AI Agent:**
> The prying force factor is 1.15, and the prying action is considered significant for this configuration.

---

**👤 You:**
> "What are the yield and ultimate strength properties for A992 steel?"

**🤖 AI Agent:**
> For A992 steel, the yield strength is 50 ksi and the ultimate strength is 65 ksi.


## ❓ FAQ

**Q: What standards does this tool follow?**
The design procedures and capacity checks are based on AISC (American Institute of Steel Construction) standards.

**Q: How does the tool handle prying action?**
The `calculate_connection_design` tool evaluates prying action to adjust effective bolt tension, and you can use `validate_prying_action` for independent verification of secondary forces.

**Q: Can I check the column web strength?**
Yes, use the `check_panel_zone_capacity` tool to verify if the column web can withstand the shear force transferred by the moment connection.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-moment-connection-designer](https://vinkius.com/ai-agent-connect/steel-moment-connection-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Moment Connection Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-moment-connection-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Moment Connection Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-moment-connection-designer": {
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
