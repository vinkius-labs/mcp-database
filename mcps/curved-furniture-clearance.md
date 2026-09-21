# Curved Furniture Clearance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/curved-furniture-clearance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

Analyze spatial placement and clearance for curved furniture.

## Description
This MCP server provides advanced spatial analysis for non-linear furniture. It allows AI agents to evaluate the placement of curved sofas, tables, and counters within architectural constraints. Use `analyze_furniture_placement` to detect collisions, `validate_pathway_accessibility` to ensure human transit widths, `simulate_door_clearance` to prevent door interference, and `find_optimal_orientations` to resolve placement conflicts.


## Available Tools (4)
- **analyze_furniture_placement**: Check if a specific piece of curved furniture can be placed at a given coordinate and orientation without causing collisions
- **find_optimal_orientations**: Identify alternative rotations for a piece of furniture that resolve existing collisions
- **simulate_door_clearance**: Check if a proposed furniture placement blocks the functional opening of doors
- **validate_pathway_accessibility**: Verify if the movement paths between furniture clusters meet minimum width requirements for human transit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Curved Furniture Clearance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the curved sofa at position x:10, y:20 with 45 degree rotation hits anything."

**🤖 AI Agent:**
> The placement is valid with a minimum path width of 1.2 meters and no collisions detected.

---

**👤 You:**
> "Is the path in room R-101 wide enough for a person?"

**🤖 AI Agent:**
> The path is accessible with a narrowest point of 0.9 meters.

---

**👤 You:**
> "Will placing the counter at x:5, y:5 block the main entrance door?"

**🤖 AI Agent:**
> No, the counter placement does not intersect with the door swing arc.


## ❓ FAQ

**Q: How do I check if a sofa fits in a room?**
You can use the `analyze_furniture_placement` tool by providing the furniture ID, its x/y position, and its rotation.

**Q: Can I check if a door will be blocked?**
Yes, use the `simulate_door_clearance` tool to check if furniture placement interferes with a door's swing arc.

**Q: How do I find a better angle for my furniture?**
The `find_optimal_orientations` tool will iterate through possible angles to find a position that satisfies all clearance rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/curved-furniture-clearance](https://vinkius.com/en/ai-agent-connect/curved-furniture-clearance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Curved Furniture Clearance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `curved-furniture-clearance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Curved Furniture Clearance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "curved-furniture-clearance": {
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
