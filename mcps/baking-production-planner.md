# Baking Production Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/baking-production-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Orchestrate bakery production from orders to packaging.

## Description
This MCP server synchronizes the entire bakery production flow. It translates customer orders into batches using `plan_batches_for_orders`, schedules oven usage with `schedule_oven_cycles`, calculates necessary cooling rack space via `calculate_cooling_requirements`, estimates raw material needs with `estimate_ingredient_needs`, and ensures final logistics are feasible using `verify_packaging_capacity`.


## Available Tools (5)
- **calculate_cooling_requirements**: 
- **estimate_ingredient_needs**: 
- **plan_batches_for_orders**: 
- **schedule_oven_cycles**: 
- **verify_packaging_capacity**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baking Production Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Convert order IDs ORD-101 and ORD-102 into production batches."

**🤖 AI Agent:**
> Batch ORD-101-A (50 units) starts at 08:00 and Batch ORD-102-A (30 units) starts at 09:00.

---

**👤 You:**
> "How many ingredients do I need for batches B-55 and B-56?"

**🤖 AI Agent:**
> You need 50kg of Flour, 20kg of Sugar, and 10kg of Butter for these batches.

---

**👤 You:**
> "Will my packaging station handle the output from these cooling requirements?"

**🤖 AI Agent:**
> Yes, the packaging capacity is sufficient for the predicted volume.


## ❓ FAQ

**Q: How do I start a production run?**
Start by using `plan_batches_for_orders` to convert your active orders into a sequence of production batches.

**Q: Can I check if I have enough ingredients?**
Yes, use `estimate_ingredient_needs` with your planned batch IDs to see the total raw materials required.

**Q: How is oven capacity managed?**
The `schedule_oven_cycles` tool assigns batches to specific ovens while respecting their capacity and time constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/baking-production-planner](https://vinkius.com/en/ai-agent-connect/baking-production-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baking Production Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baking-production-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baking Production Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baking-production-planner": {
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
