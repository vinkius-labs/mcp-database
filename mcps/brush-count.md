# brush-count MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/brush-count)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Quantify and categorize painting brushes in your inventory.

## Description
Manage your studio supplies with precision. This MCP server provides tools to audit brush health, count specific brush types, and analyze size distributions. Use `count_brushes_by_type` to find specific categories, `audit_brush_condition` to check the health of your collection, `calculate_size_distribution` for size analysis, and `get_inventory_tier_summary` for high-level reports.


## Available Tools (4)
- **count_brushes_by_type**: Count brushes of a specific type
- **audit_brush_condition**: Audit the overall health status of the brush collection
- **calculate_size_distribution**: Calculate the distribution of brush sizes
- **get_inventory_tier_summary**: Get a high-level breakdown of inventory across categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **brush-count** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many synthetic brushes do I have in my inventory?"

**🤖 AI Agent:**
> You have 12 synthetic brushes in your inventory.

---

**👤 You:**
> "What is the health status of my brushes?"

**🤖 AI Agent:**
> Your collection consists of 15 pristine brushes, 8 used brushes, 3 damaged brushes, and 2 broken brushes.

---

**👤 You:**
> "What is the average size of my brushes?"

**🤖 AI Agent:**
> The average size of the brushes in your inventory is 0.5 inches.


## ❓ FAQ

**Q: How can I check if my brushes are ready for use?**
You can use the `audit_brush_condition` tool to get a summary of the health status of your brushes, including pristine and used states.

**Q: Can I filter brushes by their size?**
Yes, the `calculate_size_distribution` tool allows you to specify a minimum and maximum size to count brushes within a specific range.

**Q: How do I get a summary of my brush types?**
Use the `get_inventory_tier_summary` tool with the 'type-based' tier level to see a breakdown of your brushes by category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/brush-count](https://vinkius.com/en/ai-agent-connect/brush-count)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **brush-count** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `brush-count` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **brush-count** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "brush-count": {
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
