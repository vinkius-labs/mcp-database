# FSRU Design Suite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fsru-design-suite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design Floating Storage and Regasification Units (FSRU) based on import requirements and environmental conditions.

## Description
This MCP server provides a complete design methodology for sizing Floating Storage and Regasification Units (FSRU). It allows AI agents to calculate essential parameters including `calculate_storage_capacity` for LNG volume, `calculate_regasification_capability` for equipment rating, and `design_mooring_system` for structural stability. Users can also use `evaluate_operational_profile` to assess annual gas delivery reliability and risk based on weather and maintenance downtime.


## Available Tools (4)
- **calculate_regasification_capability**: Determines the required regasification equipment rating to meet sendout demands
- **calculate_storage_capacity**: Determines the required liquid LNG storage volume for the FSRU
- **design_mooring_system**: Determines the appropriate mooring type and structural strength requirements
- **evaluate_operational_profile**: Provides a summary of the FSRU's ability to meet annual gas demands


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FSRU Design Suite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the required LNG storage for a daily sendout of 500 units with deliveries every 14 days and a 3-day safety buffer."

**🤖 AI Agent:**
> The required storage volume is 8,500 units, with a safety reserve of 1,500 units.

---

**👤 You:**
> "What mooring type is needed for a site with 5 meter significant wave height and 25 knot wind speed?"

**🤖 AI Agent:**
> A Turret Mooring system is required to maintain stability in these environmental conditions.

---

**👤 You:**
> "Determine the regasification equipment rating for a 400 unit sendout rate with 0.1 weather downtime and 0.05 maintenance downtime."

**🤖 AI Agent:**
> The required equipment rating is 470.59 units to ensure a 400 unit sendout rate is met given the 85% availability.


## ❓ FAQ

**Q: How does the tool account for weather downtime?**
The `calculate_regasification_capability` tool uses a downtime fraction to ensure the equipment rating is high enough to meet target sendout rates during operational windows.

**Q: Can I design mooring systems for harsh environments?**
Yes, `design_mooring_system` evaluates environmental loads like wave height and wind speed to determine if a Spread Mooring or a Turret Mooring is required.

**Q: What determines the required LNG storage volume?**
The `calculate_storage_capacity` tool calculates volume based on the daily sendout requirement, the interval between LNG carrier deliveries, and any requested safety buffer.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fsru-design-suite](https://vinkius.com/en/ai-agent-connect/fsru-design-suite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FSRU Design Suite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fsru-design-suite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FSRU Design Suite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fsru-design-suite": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
