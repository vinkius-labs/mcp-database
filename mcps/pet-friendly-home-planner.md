# Pet-Friendly Home Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-friendly-home-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [pet-care](../categories/pet-care.md)

Optimizes room layouts to balance human furniture needs with pet-specific spatial requirements.

## Description
This MCP server provides a specialized layout engine for creating pet-friendly living spaces. It uses deterministic placement logic to ensure that human furniture requirements are met while maintaining essential pet zones like feeding areas, sleeping zones, and unobstructed movement paths. Use `plan_room_layout` to generate initial configurations, `validate_pet_safety` to check for collisions or blocked paths, and `suggest_alternative_placement` to find new layouts if the initial plan fails. You can also use `calculate_spatial_efficiency` to analyze how well the room utilizes available space for both humans and pets.


## Available Tools (4)
- **plan_room_layout**: Generates a complete room layout plan based on dimensions and requirements
- **suggest_alternative_placement**: Provides a different layout configuration when the initial plan fails or has too many collisions
- **validate_pet_safety**: Checks a specific layout for safety violations regarding pet movement and zone accessibility
- **calculate_spatial_efficiency**: Analyzes how well the room is being used by both humans and pets


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet-Friendly Home Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a layout for a 500x400cm room with a sofa (200x90cm) and a coffee table (100x50cm), requiring a feeding zone and a 100cm movement path."

**🤖 AI Agent:**
> The room layout has been successfully planned. The sofa is placed at (0,0) and the coffee table at (210,0). The feeding zone is established in the quiet corner at (400,300), and a clear 100cm movement path is maintained throughout the center.

---

**👤 You:**
> "Check if this layout is safe: Room 300x300cm, Sofa at (0,0) size 200x100cm, Feeding zone at (250,250)."

**🤖 AI Agent:**
> The layout is safe. There are no collisions between the sofa and the feeding zone, and the movement path remains unobstructed.

---

**👤 You:**
> "Suggest an alternative layout for a small room where the furniture is blocking the pet's path."

**🤖 AI Agent:**
> A new layout has been generated with HIGH constraint strictness. The furniture has been shifted to the perimeter to prioritize a wide, unobstructed movement path for the pet.


## ❓ FAQ

**Q: How does the planner ensure pet safety?**
The engine uses `validate_pet_safety` to check for collisions between furniture and pet zones, ensuring that movement paths remain unobstructed and feeding/sleeping areas are accessible.

**Q: What happens if my furniture doesn't fit in the room?**
If a layout fails, you can use `suggest_alternative_placement` with different strictness levels to prioritize either pet movement or human furniture fitting.

**Q: Can I measure how efficiently the room is used?**
Yes, the `calculate_spatial_efficiency` tool provides metrics on furniture utilization, pet access ratios, and wasted space.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-friendly-home-planner](https://vinkius.com/en/ai-agent-connect/pet-friendly-home-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet-Friendly Home Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-friendly-home-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet-Friendly Home Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-friendly-home-planner": {
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
