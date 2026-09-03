# Steel Connection Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-connection-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design bolted steel connections with limit state analysis.

## Description
This MCP server provides specialized engineering tools for designing bolted steel connections. It uses limit state design principles to calculate bolt configurations, plate dimensions, prying action effects, and weld requirements. Use `bolt_configuration_tool` to determine bolt counts and spacing, `plate_dimensions_tool` for plate sizing, `prying_effects_tool` to assess stability, and `weld_specifications_tool` for reinforcement details.


## Available Tools (4)
- **bolt_configuration_tool**: Determines the minimum number of bolts and the required arrangement to resist applied forces
- **plate_dimensions_tool**: Calculates the physical size of the steel plate required to support the connection
- **prying_effects_tool**: Assesses the additional tension stress placed on bolts due to plate deformation
- **weld_specifications_tool**: Defines the welding requirements for connections that involve welded components or reinforcements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Connection Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the bolt configuration for a SINGLE_LAP connection with 50kN force using BOLT_GRADE_8_8 bolts (16mm diameter) and STEEL_GRADE_S355."

**🤖 AI Agent:**
> The required configuration is 4 bolts arranged in a 2x2 pattern with 50mm spacing and 30mm edge distance.

---

**👤 You:**
> "What size plate is needed for 4 bolts with 50mm spacing and 16mm diameter, using a 12mm thick S355 steel plate?"

**🤖 AI Agent:**
> The required plate dimensions are 120mm in width and 150mm in length.

---

**👤 You:**
> "Determine the weld requirements for an END_PLATE connection with 40kN force and 10mm plate thickness using S235 steel."

**🤖 AI Agent:**
> The required weld is a 6mm fillet weld with a total length of 120mm.


## ❓ FAQ

**Q: What design method does this server use?**
The server uses the limit state design method to ensure structural safety by checking design strength against applied loads.

**Q: How do I calculate the required number of bolts?**
You can use the `bolt_configuration_tool` by providing the connection type, applied force, bolt grade, diameter, and steel grade.

**Q: Does this tool account for prying action?**
Yes, the `prying_effects_tool` specifically assesses additional tension stress caused by plate deformation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-connection-designer](https://vinkius.com/ai-agent-connect/steel-connection-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Connection Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-connection-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Connection Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-connection-designer": {
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
