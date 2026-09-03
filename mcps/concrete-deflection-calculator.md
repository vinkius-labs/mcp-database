# Concrete Deflection Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/concrete-deflection-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate immediate, long-term, and total deflection for reinforced concrete members using ACI standards.

## Description
This MCP server provides structural engineering tools to analyze reinforced concrete beam deflections. It calculates immediate elastic deflection, time-dependent effects like creep and shrinkage, and the final cumulative deflection. Use `get_section_stiffness_analysis` to determine if a section is cracked, and `get_immediate_deflection` to find the initial movement under load. It is designed for engineers following ACI methodologies to ensure serviceability compliance.


## Available Tools (4)
- **get_long_term_deflection**: Calculates the additional deflection caused by time-dependent effects (creep and shrinkage)
- **get_section_stiffness_analysis**: Provides a diagnostic analysis of the beam's resistance to bending
- **get_total_deflection**: Calculates the cumulative deflection (immediate + long-term)
- **get_immediate_deflection**: Calculates the initial deflection caused by a specific load


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Concrete Deflection Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the immediate deflection for a beam with a 5m span, 10kN/m load, 300mm width, 500mm height, 450mm effective depth, 30MPa concrete, and 0.01 reinforcement ratio."

**🤖 AI Agent:**
> The immediate deflection for the specified beam is 12.45 mm.

---

**👤 You:**
> "What is the total deflection if the immediate deflection is 10mm and the long-term deflection is 5mm?"

**🤖 AI Agent:**
> The total deflection is 15.0 mm.

---

**👤 You:**
> "Analyze the stiffness of a section with 300mm width, 500mm height, 450mm effective depth, 30MPa concrete, and 0.01 reinforcement ratio."

**🤖 AI Agent:**
> The section is Cracked. Gross Moment of Inertia: 1.875e10 mm4, Cracked Moment of Inertia: 8.42e9 mm4.


## ❓ FAQ

**Q: How does this tool handle cracked sections?**
The tool uses `get_section_stiffness_analysis` to identify the cracking status and calculates the cracked moment of inertia to ensure deflection values reflect the reduced stiffness of the concrete section.

**Q: What is included in the long-term deflection calculation?**
The `get_long_term_deflection` tool accounts for time-dependent effects by applying a creep coefficient and a shrinkage factor to the initial deflection.

**Q: Which AI clients can use this MCP?**
You can connect this tool to Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/concrete-deflection-calculator](https://vinkius.com/ai-agent-connect/concrete-deflection-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Concrete Deflection Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `concrete-deflection-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Concrete Deflection Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "concrete-deflection-calculator": {
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
