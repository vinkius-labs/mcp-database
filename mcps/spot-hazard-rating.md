# Spot Hazard Rating MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spot-hazard-rating)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Quantify kitesurfing environmental risks and safety.

## Description
This MCP server provides a specialized assessment engine for kitesurfing enthusiasts. It uses a risk assessment matrix to evaluate environmental factors like water depth, current speed, and wave height against a user's skill level. Use `calculate_hazard_rating` to get a total risk score, `identify_primary_hazard` to find the main threat, `get_safety_guidelines` for actionable protocols, and `check_spot_suitability` to determine if a location is safe for your experience.


## Available Tools (4)
- **calculate_hazard_rating**: Calculates the overall risk level for a specific kitesurfing session
- **check_spot_suitability**: Determines if a specific spot is appropriate for a kiter's current skill level
- **get_safety_guidelines**: Provides specific safety protocols based on the identified hazard and user skill
- **identify_primary_hazard**: Isolates the single most dangerous element of a specific spot


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spot Hazard Rating** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is this spot safe? Obstacles: rocks, water depth: 1m, current speed: 2 knots, wave height: 0.5m, distance to shore: 50m, skill level: beginner."

**🤖 AI Agent:**
> No, the spot is not suitable. The shallow water depth of 1m poses a high impact risk for a beginner.

---

**👤 You:**
> "What is the main danger here? Obstacles: none, water depth: 5m, current speed: 5 knots, wave height: 1.5m, distance to shore: 200m, skill level: intermediate."

**🤖 AI Agent:**
> The primary hazard is the high current speed of 5 knots.

---

**👤 You:**
> "Give me safety advice for a hazard rating of 4 with waves as the primary hazard for an advanced kiter."

**🤖 AI Agent:**
> Protocol: Monitor wave frequency and avoid breaking zones. Equipment Advice: Ensure your harness and leash are in peak condition. Prohibited Actions: Do not attempt to kite in heavy swell if visibility decreases.


## ❓ FAQ

**Q: How is the hazard rating calculated?**
The rating is determined by cross-referencing environmental severity (waves, currents, depth) with the user's specific skill level using a risk assessment matrix.

**Q: Can I use this for any water sport?**
This engine is specifically optimized for kitesurfing environmental variables.

**Q: What skill levels are supported?**
The system supports beginner, intermediate, advanced, and expert skill levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spot-hazard-rating](https://vinkius.com/ai-agent-connect/spot-hazard-rating)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spot Hazard Rating** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spot-hazard-rating` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spot Hazard Rating** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spot-hazard-rating": {
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
