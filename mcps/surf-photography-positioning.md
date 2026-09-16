# Surf Photography Positioning MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-photography-positioning)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Determine optimal camera placement, distance, and timing for surf photography.

## Description
This MCP server provides specialized tools for surf photographers to calculate the perfect shot. By analyzing wave break characteristics, sun angle, and water clarity, it provides precise technical setups. Use `calculate_positioning` to find the exact camera angle and distance, `analyze_lighting_conditions` to manage glare and silhouettes, `assess_visibility_constraints` to optimize for water clarity, and `optimize_background_placement` to frame the perfect composition.


## Available Tools (4)
- **analyze_lighting_conditions**: Analyze sun position for glare and silhouette risks
- **calculate_positioning**: Determine physical coordinates and technical setup for a surf shot
- **optimize_background_placement**: Suggest camera positioning to utilize or avoid background elements
- **assess_visibility_constraints**: Adjust positioning based on water clarity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Photography Positioning** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm shooting a wide landscape shot on a steep left-hander wave with a sun angle of 45 degrees. What is my setup?"

**🤖 AI Agent:**
> For a wide landscape shot on a steep left-hander, you should position your camera at a distance of 45 meters with a low camera angle and a timing offset of 2 seconds before the peak.

---

**👤 You:**
> "The water is very turbid. What lens should I use for an action close-up?"

**🤖 AI Agent:**
> In turbid water for an action close-up, a wide-angle lens is recommended, and you should stay within 5 meters of the subject.

---

**👤 You:**
> "Will I have issues with silhouettes if the sun is at 10 degrees?"

**🤖 AI Agent:**
> With a sun angle of 10 degrees, there is a high probability of silhouettes when shooting toward the light.


## ❓ FAQ

**Q: How do I get the best camera distance?**
You can use the `calculate_positioning` tool with your desired shot type to receive the exact distance in meters.

**Q: Can this help with lens flare?**
Yes, the `analyze_lighting_conditions` tool identifies glare risks and suggests the best filter to use.

**Q: What if the water is very murky?**
The `assess_visibility_constraints` tool will adjust the maximum effective distance and suggest a suitable lens for low visibility.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-photography-positioning](https://vinkius.com/en/ai-agent-connect/surf-photography-positioning)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Photography Positioning** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-photography-positioning` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Photography Positioning** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-photography-positioning": {
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
