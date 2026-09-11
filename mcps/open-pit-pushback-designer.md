# Open Pit Pushback Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/open-pit-pushback-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design incremental pit expansions by calculating boundaries, material volumes, and production feasibility.

## Description
This MCP server provides essential tools for open pit mine expansion planning. It allows engineers to define new pushback boundaries using `get_pushback_boundaries`, calculate the resulting ore and waste volumes with `calculate_material_volumes`, and verify if the mining sequence meets production targets via `validate_production_schedule`. Additionally, it can adjust designs to meet economic goals using `optimize_stripping_ratio`.


## Available Tools (4)
- **calculate_material_volumes**: Determines the quantity of ore and waste contained within a specific design
- **get_pushback_boundaries**: Identifies the geometric boundaries for a proposed pushback phase
- **optimize_stripping_ratio**: Suggests adjustments to pushback limits to balance waste removal and ore access
- **validate_production_schedule**: Checks if a sequence of pushbacks meets the required annual ore extraction goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Open Pit Pushback Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the ore and waste volumes for the boundary 'PB_01' using the 'MODEL_ALPHA' ore body model."

**🤖 AI Agent:**
> The boundary 'PB_01' contains 500,000 cubic meters of ore and 1,200,000 cubic meters of waste.

---

**👤 You:**
> "Will a sequence of ['PB_01', 'PB_02'] meet an annual ore target of 2,000,000 tons?"

**🤖 AI Agent:**
> Yes, the sequence is feasible and will meet the target over the estimated 3 years.

---

**👤 You:**
> "Find the boundaries for a new pushback where the ultimate pit is 'UP_LIMIT' and the current pit is 'CP_01' with a 45 degree slope."

**🤖 AI Agent:**
> The new pushback boundary is 'PB_NEW_01' with a safety factor of 1.45.


## ❓ FAQ

**Q: How do I define a new expansion phase?**
You can use the `get_pushback_boundaries` tool by providing the ultimate pit boundary, the current pit boundary, and the desired slope angle.

**Q: Can I check if my mine plan meets annual targets?**
Yes, the `validate_production_schedule` tool checks your sequence of pushbacks against your annual ore target to ensure feasibility.

**Q: How is the stripping ratio managed?**
The `optimize_stripping_ratio` tool helps adjust pushback geometries to achieve a specific waste-to-ore ratio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/open-pit-pushback-designer](https://vinkius.com/en/ai-agent-connect/open-pit-pushback-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Open Pit Pushback Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `open-pit-pushback-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Open Pit Pushback Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "open-pit-pushback-designer": {
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
