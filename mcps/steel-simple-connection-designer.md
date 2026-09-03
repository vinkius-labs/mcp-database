# Steel Simple Connection Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-simple-connection-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design AISC-compliant simple shear connections for steel structures.

## Description
This MCP server provides specialized tools for designing AISC-compliant simple shear connections in steel structures. It allows engineers to calculate bolt requirements, determine connection geometry for single plates or double angles, and verify the total connection capacity. Use `calculate_bolt_requirements` to find the necessary bolt count for a given reaction and `design_connection_geometry` to get physical dimensions for plates or angles. The tool accounts for eccentricity and bolt shear capacity to ensure structural safety.


## Available Tools (4)
- **calculate_bolt_requirements**: Determine how many bolts are needed to resist a specific shear load
- **design_connection_geometry**: Determine the physical dimensions of the connection components (plates or angles)
- **get_bolt_properties**: Retrieve technical specifications for available bolt sizes based on a chosen diameter
- **validate_connection_capacity**: Perform the final verification that the designed connection safely carries the load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Simple Connection Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many bolts do I need for a 50kN reaction using 20mm bolts and A325 steel grade?"

**🤖 AI Agent:**
> You will need 4 bolts to resist the 50kN reaction with the specified parameters.

---

**👤 You:**
> "What are the dimensions for a single plate connection for a W12x26 beam and W14x22 column using 3 bolts?"

**🤖 AI Agent:**
> The single plate will have a thickness of 12mm and a width of 100mm.

---

**👤 You:**
> "Is a connection with 4 bolts of 22mm diameter and 120kN capacity safe for a 100kN reaction?"

**🤖 AI Agent:**
> Yes, the connection is safe with a utilization ratio of 0.83.


## ❓ FAQ

**Q: What standards does this tool follow?**
The connection design follows AISC (American Institute of Steel Construction) standards for simple shear connections.

**Q: How do I know if my connection is safe?**
You can use the `validate_connection_capacity` tool to check if the designed connection safely carries the applied load and to see the utilization ratio.

**Q: Can I design double angle connections?**
Yes, the `design_connection_geometry` tool supports both single plate and double angle connection types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-simple-connection-designer](https://vinkius.com/ai-agent-connect/steel-simple-connection-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Simple Connection Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-simple-connection-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Simple Connection Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-simple-connection-designer": {
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
