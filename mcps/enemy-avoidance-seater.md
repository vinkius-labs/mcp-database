# Enemy Avoidance Seater MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enemy-avoidance-seater)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Automated seating engine that assigns guests to tables while strictly enforcing social constraints and enemy proximity rules.

## Description
The Enemy Avoidance Seater is a specialized tool designed for event planners and organizers who need to manage complex guest lists. It uses a deterministic algorithm to assign guests to tables while respecting two critical constraints: table capacity and social distance between enemies. By using the `execute_seating_algorithm` tool, you can provide a list of guests, available tables with their capacities, and a set of enemy constraints (defining how many tables apart certain individuals must be). The system will attempt to find a valid arrangement or identify exactly which guests are causing a bottleneck if an 'IMPOS and impossible' state is reached. Additionally, the `verify_integrity` tool allows you to audit existing seating plans to ensure no capacity limits are exceeded and no proximity rules are violated.


## Available Tools (2)
- **execute_seating_algorithm**: Calculates a seating arrangement that avoids placing enemies too close
- **verify_integrity**: Verifies if a seating arrangement follows all constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enemy Avoidance Seater** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you seat Alice, Bob, and Charlie at Table 1 (capacity 2) and Table 2 (capacity 2), knowing that Alice and Bob are enemies with a distance of 1?"

**🤖 AI Agent:**
> Alice is assigned to Table 1, Bob is assigned to Table 2, and Charlie is assigned to Table 1.

---

**👤 You:**
> "Check if this plan is valid: Guest X at Table 1, Guest Y at Table 2, where X and Y are enemies with minDistanceTables of 1."

**🤖 AI Agent:**
> The arrangement is valid because the guests are in non-adjacent tables.

---

**👤 You:**
> "Try to seat 5 people at a single table with capacity 2."

**🤖 AI Agent:**
> IMPOSSIBLE: The following guests could not be seated due to capacity constraints: Guest 3, Guest 4, Guest 5.


## ❓ FAQ

**Q: How does the tool handle conflicts between guests?**
The tool uses a `minDistanceTables` parameter. If set to 1, enemies cannot share a table or be at adjacent tables. The `execute_seating_algorithm` checks this for every placement.

**Q: What happens if a valid seating arrangement cannot be found?**
If the algorithm fails, it returns an 'IMPOSSIBLE' status and provides a detailed error message listing the specific guests that are causing the bottleneck.

**Q: Can I verify an existing seating plan?**
Yes, you can use the `verify_integrity` tool to audit any proposed assignment against your table capacities and enemy constraints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enemy-avoidance-seater](https://vinkius.com/mcp/enemy-avoidance-seater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enemy Avoidance Seater** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enemy-avoidance-seater` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enemy Avoidance Seater** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enemy-avoidance-seater": {
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
