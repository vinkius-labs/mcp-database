# Plant Count Per Bed MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/plant-count-per-bed)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate maximum plant capacity based on bed area and spacing requirements.

## Description
This MCP server provides precise tools for garden planning. Use `validate_area` to determine total surface area from dimensions, `calculate_capacity` to find how many plants fit in a specific space, `compare_plans` to evaluate different spacing options, and `get_bulk_capacity` to see a range of density estimates.


## Available Tools (4)
- **calculate_capacity**: Calculate plant capacity
- **compare_plans**: Compare two plans
- **get_bulk_capacity**: Get bulk estimates
- **validate_area**: Validate dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plant Count Per Bed** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many plants can I fit in a 10 square meter bed if each plant needs 0.5 square meters?"

**🤖 AI Agent:**
> You can fit 20 plants in a 10 square meter bed.

---

**👤 You:**
> "I have a bed that is 5 meters long and 2 meters wide. What is the total area?"

**🤖 AI Agent:**
> The total area of the bed is 10 square meters.

---

**👤 You:**
> "Which is better for a 50sqm bed: spacing plants at 2sqm each or 3sqm each?"

**🤖 AI Agent:**
> Spacing plants at 2sqm each is better, as it allows for 25 plants compared to 16 plants with the 3sqm spacing.


## ❓ FAQ

**Q: How is the plant count calculated?**
The count is determined by dividing the total bed area by the required spacing area for a single plant, then rounding down to the nearest whole number.

**Q: Can I compare two different planting layouts?**
Yes, you can use the `compare_plans` tool to see which spacing option allows for a higher number of plants in your bed.

**Q: What happens if the plant spacing area is larger than the bed area?**
The calculation will result in zero plants, as the space is insufficient for even one plant to grow optimally.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/plant-count-per-bed](https://vinkius.com/en/ai-agent-connect/plant-count-per-bed)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plant Count Per Bed** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `plant-count-per-bed` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plant Count Per Bed** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plant-count-per-bed": {
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
