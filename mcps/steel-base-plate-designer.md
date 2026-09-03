# Steel Base Plate Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-base-plate-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates steel column base plate dimensions, thickness, and anchor bolt requirements using AISC standards.

## Description
This MCP server provides structural engineering tools to design steel column base plates. It reconciles concentrated column loads with concrete bearing capacity following AISC procedures. Use `design_base_plate` to determine required plate geometry and thickness, `validate_anchor_layout` to check stability against moments, `calculate_bearing_capacity` for concrete limits, and `get_bolt_specifications` for recommended anchor bolt sizes and embedment depths.


## Available Tools (4)
- **design_base_plate**: Performs the primary structural calculation to determine the required geometry of the base plate
- **get_bolt_specifications**: Recommends standard anchor bolt sizes and embedment depths based on calculated tension requirements
- **validate_anchor_layout**: Checks if a specific anchor bolt configuration can effectively resist the tension caused by the applied moment
- **calculate_bearing_capacity**: Determines the maximum allowable axial load the concrete can support given the base plate area


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Base Plate Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a base plate for a column with 500kN axial load and 50kNm moment, column size 300x300mm, concrete strength 30MPa, and a square bolt pattern."

**🤖 AI Agent:**
> The required base plate dimensions are 550mm x 550mm with a thickness of 25mm. The recommended anchor bolt diameter is 24mm.

---

**👤 You:**
> "What is the maximum axial load for a 400x400mm plate on 25MPa concrete?"

**🤖 AI Agent:**
> The maximum allowable axial load for a 400mm x 400mm plate on 25MPa concrete is 1250kN.

---

**👤 You:**
> "Will 20mm bolts spaced 150mm apart handle a 30kNm moment?"

**🤖 AI Agent:**
> No, the current anchor bolt configuration is unstable for a 30kNm moment; increasing spacing or bolt diameter is required.


## ❓ FAQ

**Q: What standards does this tool follow?**
The calculations follow the AISC (American Institute of Steel Construction) standards for base plate design.

**Q: How do I determine the required plate thickness?**
You can use the `design_base_plate` tool, which calculates the necessary thickness to ensure the plate remains in the elastic range under bearing pressure.

**Q: Can I check if my anchor bolts are sufficient for the moment?**
Yes, the `validate_anchor_layout` tool checks if your specific bolt spacing and diameter can resist the tension induced by the applied moment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-base-plate-designer](https://vinkius.com/ai-agent-connect/steel-base-plate-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Base Plate Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-base-plate-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Base Plate Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-base-plate-designer": {
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
