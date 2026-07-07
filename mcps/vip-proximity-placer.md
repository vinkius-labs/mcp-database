# VIP Proximity Placer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vip-proximity-placer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Automated event seating engine that prioritizes VIP constraints before distributing general attendees.

## Description
The VIP Proximity Placer MCP server manages complex event seating by prioritizing VIP guests with absolute constraints. Using the `check_assignment_feasibility` tool, you can verify if a seating plan is possible before execution. The `simulate_vip_phase` tool allows you to see how VIPs are seated and which seats become locked. Finally, use `execute_full_seating_plan` to generate a complete seat map for all guests using a two-phase algorithm.


## Available Tools (3)
- **check_feasibility**: Check if VIP assignments are feasible for a given table size
- **execute_seating_plan**: Execute the full seating algorithm
- **simulate_vip_phase**: Simulate the VIP placement phase of seating


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VIP Proximity Placer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it possible to seat 5 VIPs at a table of 4?"

**🤖 AI Agent:**
> No, this would result in an overcapacity conflict.

---

**👤 You:**
> "Run the VIP phase for Alice and Bob at a table of 6 where Alice must be next to Bob."

**🤖 AI Agent:**
> Seated VIPs: Alice, Bob. Locked seats: 0, 1. Remaining empty seats: 4.

---

**👤 You:**
> "Generate a full plan for 2 VIPs (Alice at seat 0) and 2 regular guests (Charlie, David) at a table of 4."

**🤖 AI Agent:**
> Seat Map: [0: Alice, 1: Charlie, 2: David, 3: Empty]


## ❓ FAQ

**Q: How does the seating algorithm work?**
It uses a two-phase approach: first, it places VIPs with constraints and locks their seats; second, it fills remaining seats with regular guests using round-robin distribution.

**Q: Can I check if my VIP requirements are possible?**
Yes, use the `check_assignment_feasibility` tool to detect conflicts like overcapacity or impossible adjacency before you start the full plan.

**Q: What happens if a seat is locked?**
A locked seat is occupied by a VIP and cannot be changed by the `execute_full_seating_plan` process.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vip-proximity-placer](https://vinkius.com/mcp/vip-proximity-placer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VIP Proximity Placer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vip-proximity-placer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VIP Proximity Placer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vip-proximity-placer": {
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
