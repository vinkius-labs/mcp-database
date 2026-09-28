# School Supplies Distribution Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-supplies-distribution-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [education](../categories/education.md)

Optimizes school supply allocation using reuse-first logic and budget tracking.

## Description
This MCP server acts as an intelligent logistics engine for school supply distribution. It implements a 'Reuse-First' principle to minimize waste by checking existing inventory before suggesting new purchases. The system calculates necessary `get_purchase_plan` actions within budget constraints, generates detailed `get_packing_lists` for individual children, identifies `get_labeling_tasks` for distribution accuracy, and provides a `get_inventory_summary` to track remaining stock.


## Available Tools (4)
- **get_inventory_summary**: Provides a follow-up report on what remains in storage after the distribution plan is executed
- **get_labeling_tasks**: Identifies which items need labels to ensure they reach the correct children during distribution
- **get_purchase_plan**: Determines exactly what items must be bought to fulfill all children's requirements after using available stock
- **get_packing_lists**: Generates specific instructions for packing individual supply bags for each child


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Supplies Distribution Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have 50 students needing pencils and notebooks. I have 20 pencils in stock. My budget is $100. What should I buy?"

**🤖 AI Agent:**
> You need to purchase 30 additional pencils and 50 notebooks to fulfill the requirements for all 50 students.

---

**👤 You:**
> "Generate a packing list for Maria from Lincoln Elementary."

**🤖 AI Agent:**
> Maria's bag should include: 2 pencils, 1 notebook, and 1 eraser.

---

**👤 You:**
> "What items need labels for the distribution?"

**🤖 AI Agent:**
> You need to create 50 labels for notebooks and 50 labels for pencil sets.


## ❓ FAQ

**Q: How does the system handle existing stock?**
The system uses the 'Reuse-First' principle, meaning it will always attempt to use items from your `existingSupplies` before adding items to the `get_purchase_plan`.

**Q: Can I track my budget?**
Yes, the `get_purchase_plan` tool evaluates the total cost of required items against your provided budget and reports if you are within budget or facing a shortfall.

**Q: How are items assigned to children?**
Supplies are assigned per child via `get_packing_lists` to ensure every student receives their specific required items accurately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-supplies-distribution-planner](https://vinkius.com/en/ai-agent-connect/school-supplies-distribution-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Supplies Distribution Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-supplies-distribution-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Supplies Distribution Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-supplies-distribution-planner": {
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
