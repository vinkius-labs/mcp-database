# Room Dimension & Furniture Fit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/room-dimension-furniture-fit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [interior-design](../categories/interior-design.md)

Validates furniture placement against room dimensions, obstacles, and door swing zones.

## Description
This MCP server provides spatial validation tools to ensure furniture fits within a room's physical boundaries. It checks for overlaps with fixed obstacles, calculates the area blocked by door swing zones using `simulate_door_swing`, and verifies if walkways meet minimum width requirements via `validate_clearance_paths`. You can also use `check_room_capacity` to confirm if a specific item fits and `calculate_usable_space` to determine the remaining floor area.


## Available Tools (4)
- **calculate_usable_space**: Calculates the remaining empty floor space in a room
- **check_room_capacity**: Checks if a specific piece of furniture fits into a room configuration
- **simulate_door_swing**: Simulates the area blocked by a door swing
- **validate_clearance_paths**: Validates if walkways between furniture and walls/obstacles are sufficient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Dimension & Furniture Fit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Will a 2m wide sofa fit in a 5m x 4m room with a cabinet at (1,1) of size 1m x 1m?"

**🤖 AI Agent:**
> Yes, the sofa fits within the room boundaries and does not overlap with the cabinet.

---

**👤 You:**
> "Calculate the remaining space in a 10x10 room with a 2x2 obstacle."

**🤖 AI Agent:**
> The total area is 100, the occupied area is 4, and the usable area is 96.

---

**👤 You:**
> "Where is the area blocked by a 1m wide door on the north wall at position (2,0)?"

**🤖 AI Agent:**
> The door swing blocks a quarter-circle area of approximately 0.785 square meters centered at the hinge.


## ❓ FAQ

**Q: How does the tool handle door openings?**
The `simulate_door_swing` tool calculates the quarter-circle area blocked by a door's movement to prevent furniture from obstructing the entrance.

**Q: Can I check if a specific sofa will fit in my room?**
Yes, use the `check_room_capacity` tool by providing the room dimensions, furniture dimensions, and any fixed obstacles.

**Q: How is usable area calculated?**
The `calculate_usable_space` tool subtracts the area of fixed obstacles and placed furniture from the total room area.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/room-dimension-furniture-fit](https://vinkius.com/en/ai-agent-connect/room-dimension-furniture-fit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Room Dimension & Furniture Fit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `room-dimension-furniture-fit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Room Dimension & Furniture Fit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "room-dimension-furniture-fit": {
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
