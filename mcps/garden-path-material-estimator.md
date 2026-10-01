# Garden Path Material Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/garden-path-material-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculate precise gravel, edging, fabric, and delivery requirements for garden paths.

## Description
This MCP server provides specialized tools for landscaping planning. It calculates the exact volume of gravel needed by accounting for path dimensions and a compaction factor. It also determines the linear length of edging required for segment perimeters, the total surface area for landscape fabric, and the logistics for material delivery based on weight and vehicle capacity. Use `calculate_material_volumes` to find gravel needs, `calculate_edging_requirements` for borders, `calculate_fabric_requirements` for ground cover, and `calculate_delivery_logistics` to plan truck loads.


## Available Tools (4)
- **calculate_delivery_logistics**: Converts volume into weight and determines the number of delivery loads
- **calculate_edging_requirements**: Calculates the total linear length of edging needed
- **calculate_fabric_requirements**: Calculates the total surface area of landscape fabric required
- **calculate_material_volumes**: Calculates the total volume of gravel required for path segments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Garden Path Material Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much gravel do I need for a path with two segments, each 5m long and 1m wide, with a depth of 0.1m and a compaction factor of 1.2?"

**🤖 AI Agent:**
> You will need 1.2 cubic meters of gravel.

---

**👤 You:**
> "How much edging is required for a single path segment that is 10 meters long and 2 meters wide?"

**🤖 AI Agent:**
> You need 24 meters of edging.

---

**👤 You:**
> "If I need 5 cubic meters of gravel with a density of 1600 kg/m3 and my truck can carry 2000 kg, how many deliveries do I need?"

**🤖 AI Agent:**
> You will need 4 delivery loads.


## ❓ FAQ

**Q: How does the compaction factor affect my gravel order?**
The compaction factor accounts for the fact that gravel settles and compresses when installed. Using `calculate_material_volumes` ensures you order enough material to maintain the desired depth after settling.

**Q: Can I calculate how many truckloads I need?**
Yes, by using the `calculate_delivery_logistics` tool, you can determine the total weight and the number of vehicle trips required based on your material density and vehicle capacity.

**Q: Does this tool calculate fabric requirements?**
Yes, the `calculate_fabric_requirements` tool calculates the total surface area of your path segments to ensure you have enough landscape fabric to cover the entire area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/garden-path-material-estimator](https://vinkius.com/en/ai-agent-connect/garden-path-material-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Garden Path Material Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `garden-path-material-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Garden Path Material Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "garden-path-material-estimator": {
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
