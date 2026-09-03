# Steel Plate Girder Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/steel-plate-girder-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Design welded plate girders by calculating web dimensions, flange sizes, and stability.

## Description
This MCP server provides structural engineering tools to design welded plate girders. It allows AI agents to calculate essential components including web and flange dimensions using `calculate_girder_geometry`. It also assesses structural stability via `calculate_web_stability` to determine if stiffeners are required, calculates necessary weld sizes with `calculate_weld_requirements`, and verifies safety against repetitive loading using `validate_fatigue_life`.


## Available Tools (4)
- **calculate_weld_requirements**: To determine the size of the welds connecting the web to the flanges
- **calculate_web_stability**: To determine if the web requires stiffeners and what the spacing between them should be
- **calculate_girder_geometry**: To determine the basic dimensions of the web and flanges based on primary loading and span requirements
- **validate_fatigue_life**: To assess if the designed girder meets safety standards regarding repetitive loading


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Steel Plate Girder Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the dimensions for a 10m girder with a 20 kN/m load, a 0.02m deflection limit, and S355 steel."

**🤖 AI Agent:**
> The designed girder has a web height of 0.8m, web thickness of 0.012m, flange width of 0.3m, and flange thickness of 0.025m.

---

**👤 You:**
> "Check if a web with 0.8m height and 0.012m thickness under a 20 kN/m load needs stiffeners."

**🤖 AI Agent:**
> Yes, stiffeners are required. The recommended stiffener spacing is 0.6 meters.

---

**👤 You:**
> "What weld size is needed for a 0.3m flange and 0.012m web using S355 steel?"

**🤖 AI Agent:**
> The required weld size is 8mm, using a fillet weld type.


## ❓ FAQ

**Q: What can I design with this tool?**
You can design welded plate girders by calculating web height, flange width, stiffener spacing, and weld requirements.

**Q: How does the tool handle web buckling?**
The `calculate_web_stability` tool checks if the web slenderness requires vertical stiffeners to prevent buckling.

**Q: Does it account for material properties?**
Yes, you must provide the steel grade (such as S235 or S355) to ensure accurate strength and fatigue calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/steel-plate-girder-designer](https://vinkius.com/ai-agent-connect/steel-plate-girder-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Steel Plate Girder Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `steel-plate-girder-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Steel Plate Girder Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "steel-plate-girder-designer": {
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
