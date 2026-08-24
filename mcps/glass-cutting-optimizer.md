# Glass Cutting Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/glass-cutting-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [optimization](../categories/optimization.md)

Deterministic 2D guillotine-style cutting optimizer for industrial glass fabrication.

## Description
This MCP server provides precise 2D cutting optimization for glass fabrication. It uses deterministic guillotine-style algorithms to ensure every cut is a straight line from edge to edge, matching physical glass cutting constraints. Use `calculate_material_requirements` to determine total sheets and weight, `optimize_cutting_layout` to generate specific 2D layouts and cut sequences, or `suggest_stock_sizes` to find the most efficient raw material dimensions to minimize waste.


## Available Tools (3)
- **calculate_material_requirements**: Determines the total number of stock sheets needed and the total weight of the order
- **optimize_cutting_layout**: Generates the specific 2D layout and cutting sequence for a given set of materials
- **suggest_stock_sizes**: Recommends alternative stock sheet dimensions to minimize wasted material


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Glass Cutting Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many 2440x1830mm sheets do I need for 10 pieces of 500x500mm glass with a 2mm kerf and 10mm edge clearance?"

**🤖 AI Agent:**
> You will need 1 sheet of 2440x1830mm glass. The total weight for the 10 pieces will be approximately 25.0 kg.

---

**👤 You:**
> "Generate a cutting layout for 5 pieces of 600x400mm glass using a 2500x1500mm sheet."

**🤖 AI Agent:**
> The optimal layout requires 1 sheet. The pieces are placed at coordinates (10,10), (612,10), (1214,10), (1816,10), and (10,412). The waste percentage is 18.4%.

---

**👤 You:**
> "What stock sizes should I use for these pieces: 3 pieces of 1200x800mm?"

**🤖 AI Agent:**
> To minimize waste, it is recommended to use a stock sheet of 3650x820mm or a standard 2440x1830mm sheet depending on availability.


## ❓ FAQ

**Q: What are guillotine cuts?**
Guillotine cuts are straight lines that span from one edge of a piece of material to the opposite edge. This ensures the optimizer follows the physical limitations of glass cutting tools.

**Q: How is waste calculated?**
Waste percentage is the ratio of the total area of all required pieces to the total area of all stock sheets used, accounting for the saw kerf and edge clearance.

**Q: Can I use this to calculate glass weight?**
Yes, by using the `calculate_material_requirements` tool, you can determine the total weight of the order based on the provided thickness and dimensions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/glass-cutting-optimizer](https://vinkius.com/ai-agent-connect/glass-cutting-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Glass Cutting Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `glass-cutting-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Glass Cutting Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "glass-cutting-optimizer": {
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
