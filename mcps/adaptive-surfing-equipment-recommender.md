# Adaptive Surfing Equipment Recommender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/adaptive-surfing-equipment-recommender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [accessibility](../categories/accessibility.md)

Tailored equipment recommendations for adaptive surfers based on physical profiles and goals.

## Description
This MCP server provides specialized guidance for adaptive surfing by connecting AI agents to expert equipment logic. It uses `get_equipment_recommendations` to provide comprehensive modification lists, `calculate_board_adaptations` to determine specific buoyancy and traction needs, and `identify_assistive_devices` to suggest external tools. It also includes `verify_safety_compliance` to ensure all proposed setups meet essential safety standards for various disability categories.


## Available Tools (4)
- **verify_safety_compliance**: Checks if a proposed equipment setup meets standard adaptive surfing safety guidelines
- **calculate_board_adaptations**: Determines specific physical changes needed for a surfboard
- **identify_assistive_devices**: Recommends external tools to supplement the surfboard
- **get_equipment_recommendations**: Provides a comprehensive list of recommended equipment modifications based on a user's profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Adaptive Surfing Equipment Recommender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a mobility impairment and want to achieve independent performance. What equipment do I need?"

**🤖 AI Agent:**
> For independent performance with mobility impairments, we recommend increased board volume for stability, high-traction deck pads, and specialized mounting systems for seating.

---

**👤 You:**
> "What board adaptations are needed for someone with low core stability?"

**🤖 AI Agent:**
> To compensate for low core stability, you should use a board with increased volume and widened rails to maximize buoyancy and equilibrium.

---

**👤 You:**
> "Suggest some assistive devices for a surfer with sensory impairments aiming for assisted entry."

**🤖 AI Agent:**
> For assisted entry with sensory impairments, we suggest using specialized flotation vests and high-visibility markers on the board.


## ❓ FAQ

**Q: How does the tool determine equipment needs?**
The server analyzes the user's disability category, physical ability profile, and surfing goals to generate specific recommendations via `get_equipment_recommendations`.

**Q: Can I check if my gear is safe?**
Yes, you can use the `verify_safety_compliance` tool to check if a proposed set of modifications meets safety guidelines for a specific disability category.

**Q: What kind of board changes can be calculated?**
The `calculate_board_adaptations` tool provides specific details on volume adjustments, traction types, and structural stability features.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/adaptive-surfing-equipment-recommender](https://vinkius.com/en/ai-agent-connect/adaptive-surfing-equipment-recommender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Adaptive Surfing Equipment Recommender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adaptive-surfing-equipment-recommender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Adaptive Surfing Equipment Recommender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adaptive-surfing-equipment-recommender": {
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
