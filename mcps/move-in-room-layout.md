# Move-in Room Layout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/move-in-room-layout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize furniture placement in rectangular rooms with physical constraints.

## Description
This MCP server provides a spatial planning engine to organize furniture within rectangular rooms. It respects physical constraints like doors and windows, ensures walking paths remain unobstructed, and manages clearance requirements for each piece of furniture. Use `find_optimal_layout` to generate complete arrangements, `check_clearance_violation` to validate usage space, `calculate_room_density` to monitor floor occupancy, and `get_wall_alignment_options` to identify suitable wall segments for placement.


## Available Tools (4)
- **calculate_room_density**: Determines how crowded a room is and how much usable floor space remains
- **check_clearance_violation**: Validates if a specific piece of furniture violates the required usage space around it
- **find_optimal_layout**: Generates a complete spatial arrangement of all provided furniture within the room constraints
- **get_wall_alignment_options**: Identifies available wall segments where furniture can be placed according to user preferences


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Move-in Room Layout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the best way to place a bed (2x2) and a desk (1x1.5) in a 4x5 room with a door at the north wall, 1 unit from the corner."

**🤖 AI Agent:**
> The bed has been placed at (0,0) and the desk at (0,2), leaving a clear walking path and respecting the door position.

---

**👤 You:**
> "Is there enough space around the chair with ID 'chair_01' if I add a 0.5 unit buffer?"

**🤖 AI Agent:**
> No, the chair 'chair_01' violates the clearance requirement because it overlaps with the dining table.

---

**👤 You:**
> "What is the occupancy percentage of a 10x10 room containing furniture totaling 40 square units?"

**🤖 AI Agent:**
> The room occupancy is 40% and there are 60 square units of free area remaining.


## ❓ FAQ

**Q: How does the tool handle walking paths?**
The `find_optimal_layout` tool ensures that movement corridors between doors and furniture clusters remain unobstructed based on the specified minimum walking path width.

**Q: Can I check if a desk has enough space to be used?**
Yes, you can use `check_clearance_violation` to verify if a specific piece of furniture has sufficient clearance from walls, doors, or other objects.

**Q: How do I know if a room is too crowded?**
You can use `calculate_room_density` to get the occupancy percentage and the remaining free area of the room.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/move-in-room-layout](https://vinkius.com/en/ai-agent-connect/move-in-room-layout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Move-in Room Layout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `move-in-room-layout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Move-in Room Layout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "move-in-room-layout": {
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
