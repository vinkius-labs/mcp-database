# Tank Farm Optimization MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tank-farm-optimization)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Optimize refinery tank farm operations including tank allocation, blending schedules, and inventory buffers.

## Description
This MCP server provides specialized tools for managing refinery tank farm operations. It enables AI agents to perform precise tank allocation, generate complex blending schedules, and calculate necessary inventory buffers to prevent stockouts. By using `get_inventory_status`, agents can monitor real-time tank volumes and capacities. The `calculate_allocation_plan` tool ensures products are assigned to tanks while strictly adhering to product segregation rules. For quality control, `generate_blending_schedule` plans the sequence of product additions to meet specific target specifications. Finally, `optimize_inventory_buffer` uses shipping schedules and safety factors to determine minimum inventory levels, ensuring operational stability.


## Available Tools (4)
- **calculate_allocation_plan**: Generates an optimized plan for assigning products to tanks based on current inventory and upcoming demands
- **generate_blending_schedule**: Determines the sequence of product additions required to meet specific product quality targets
- **get_inventory_status**: Provides a real-time snapshot of the current state of all tanks in the farm
- **optimize_inventory_buffer**: Calculates the necessary minimum inventory levels to prevent stockouts based on shipping schedules and demand


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tank Farm Optimization** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of the tanks in farm ID 'REF-001'?"

**🤖 AI Agent:**
> Tank REF-001-A is active with 5,000m3 of Diesel (Capacity: 10,000m3). Tank REF-001-B is in cleaning status.

---

**👤 You:**
> "Generate an allocation plan for farm 'REF-001' with a demand for 2000m3 of Gasoline and segregation rules ['Gasoline', 'Diesel']."

**🤖 AI Agent:**
> Allocation plan generated: Tank REF-001-C has been assigned 2000m3 of Gasoline starting 2024-05-20T08:00:00Z.

---

**👤 You:**
> "Calculate the required inventory buffer for farm 'REF-001' with a safety factor of 1.2 and an upcoming shipment of 5000m3 of Fuel Oil on 2024-06-01."

**🤖 AI Agent:**
> The required minimum inventory for Fuel Oil is 6000m3 to be secured by 2024-06-01.


## ❓ FAQ

**Q: How does the tool handle product contamination?**
The `calculate_allocation_plan` tool uses provided segregation rules to ensure incompatible products are never assigned to the same tank, preventing contamination.

**Q: Can I check the current status of my tanks?**
Yes, you can use the `get_inventory_status` tool to retrieve real-time data on tank volumes, capacities, and current product types.

**Q: How are safety buffers calculated?**
The `optimize_inventory_buffer` tool calculates minimum levels by analyzing upcoming shipping schedules and applying a user-defined safety factor to account for volatility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tank-farm-optimization](https://vinkius.com/en/ai-agent-connect/tank-farm-optimization)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tank Farm Optimization** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tank-farm-optimization` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tank Farm Optimization** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tank-farm-optimization": {
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
