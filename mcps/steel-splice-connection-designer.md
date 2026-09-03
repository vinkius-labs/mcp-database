# Steel Splice Connection Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-splice-connection-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design column splice connections for axial and moment loads.

## Description
This MCP server provides structural engineering tools to design column splice connections. Use `design_bearing_splice` to calculate requirements for axial compression loads, or `design_moment_splice` for connections handling both axial loads and bending moments. You can also use `validate_connection_capacity` to verify if existing plates, bolts, and welds meet specific load requirements, or `get_steel_properties` to retrieve material constants for various steel grades.


## Available Tools (4)
- **get_steel_properties**: Retrieves the material constants for a specific steel grade
- **design_bearing_splice**: Calculates requirements for a splice connection intended primarily to transfer axial compression loads
- **design_moment_splice**: Calculates requirements for a connection intended to transfer both axial loads and bending moments
- **validate_connection_capacity**: Verifies if an existing splice design is sufficient for a specific set of loads


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Splice Connection Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a bearing splice for an axial load of 500 kN on a column with a 200mm flange width and 300mm depth using S355 steel."

**🤖 AI Agent:**
> The required splice plate width is 220mm with a thickness of 15mm, requiring 4 bolts and a weld length of 450mm.

---

**👤 You:**
> "Calculate a moment splice for 100 kN axial load and 50 kNm moment on a 250x250mm column with S355 steel."

**🤖 AI Agent:**
> The design requires a plate width of 260mm, 6 bolts of M20 diameter, and a weld size of 8mm.

---

**👤 You:**
> "Is a connection with a 10mm plate, 4 M16 bolts (shear capacity 50kN each), and 100mm weld (size 6mm) safe for 200 kN axial load and 10 kNm moment?"

**🤖 AI Agent:**
> Yes, the connection is safe with a utilization ratio of 0.75.


## ❓ FAQ

**Q: What is the difference between bearing and moment splices?**
A bearing splice is designed to transfer axial compression loads, while a moment splice is designed to transfer both axial loads and bending moments.

**Q: How can I check if my current design is safe?**
You can use the `validate_connection_capacity` tool by providing the applied loads and the dimensions of your plates, bolts, and welds.

**Q: Which steel grades are supported?**
The tool supports standard grades such as S235, S275, S355, and ASTM A36 via the `get_steel_properties` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-splice-connection-designer](https://vinkius.com/ai-agent-connect/steel-splice-connection-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Splice Connection Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-splice-connection-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Splice Connection Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-splice-connection-designer": {
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
