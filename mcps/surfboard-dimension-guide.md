# Surfboard Dimension Guide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surfboard-dimension-guide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Get precise surfboard dimensions based on your height, weight, skill, and wave conditions.

## Description
This MCP server provides expert-level surfboard dimension recommendations. By analyzing your physical profile and target environment, you can use `get_recommended_dimensions` to find the ideal length, width, thickness, and volume. You can also use `get_stability_score` to assess how a board will feel, `get_wave_compatibility` to check if a shape fits specific wave types, and `get_volume_by_skill_tier` to understand buoyancy requirements for your skill level.


## Available Tools (4)
- **get_recommended_dimensions**: Provides a complete set of recommended surfboard dimensions for a specific surfer profile
- **get_stability_score**: Calculates a numerical indicator of how stable a suggested surfboard will feel for a specific user
- **get_volume_by_skill_tier**: Retrieves the volume range and characteristic profile for a specific skill level
- **get_wave_compatibility**: Evaluates if a specific surfboard is appropriate for a given wave condition


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surfboard Dimension Guide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am 180cm tall, weigh 80kg, I am an intermediate surfer, and I want to surf small waves. What surfboard should I use?"

**🤖 AI Agent:**
> For your profile, a surfboard with a length of 210cm, width of 54cm, thickness of 5.5cm, and a volume of 52L is recommended, featuring a balanced volume distribution.

---

**👤 You:**
> "How stable will a board with 200cm length, 56cm width, and 6cm thickness be for an 85kg surfer?"

**🤖 AI Agent:**
> That board provides a stability index of 8.5 and is rated as highly stable for your weight.

---

**👤 You:**
> "Is a board that is 220cm long, 45cm wide, and 4cm thick good for large waves?"

**🤖 AI Agent:**
> Yes, this streamlined profile is highly suitable for large waves as it allows for better rail engagement and control.


## ❓ FAQ

**Q: How accurate are these recommendations?**
The recommendations are based on established surfboard design principles that account for surfer weight, height, skill level, and wave energy.

**Q: Can I check if a specific board is good for small waves?**
Yes, you can use the `get_wave_compatibility` tool to evaluate if a specific set of dimensions is suitable for small, medium, or large waves.

**Q: What information do I need to provide?**
To get a full recommendation, you should provide your height, weight, skill level (beginner, intermediate, or advanced), and the type of waves you plan to surf.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surfboard-dimension-guide](https://vinkius.com/en/ai-agent-connect/surfboard-dimension-guide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surfboard Dimension Guide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surfboard-dimension-guide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surfboard Dimension Guide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surfboard-dimension-guide": {
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
