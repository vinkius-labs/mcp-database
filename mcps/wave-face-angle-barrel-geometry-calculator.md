# Wave Face Angle & Barrel Geometry Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wave-face-angle-barrel-geometry-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate wave face angles, barrel potential, wave speed, and ride duration.

## Description
This MCP server provides precise oceanographic calculations for surfers and oceanographers. Use `calculate_wave_geometry` to get a full profile of a wave, including its face angle and barrel potential. You can also use `get_wave_speed` to find the velocity of the wave front or `evaluate_barrel_quality` to assess surfability based on steepness and seafloor slope.


## Available Tools (3)
- **calculate_wave_geometry**: Calculates a complete suite of wave characteristics including angle, potential, speed, and duration
- **evaluate_barrel_quality**: Determines the qualitative surfability/hollowness of a wave based on its shape and the seafloor
- **get_wave_speed**: Calculates only the velocity of the wave front


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Face Angle & Barrel Geometry Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the wave geometry for a 2m wave breaking in 1.5m of water with a 3 degree beach slope."

**🤖 AI Agent:**
> The wave face angle is 53.13 degrees, the barrel potential is Medium, the wave speed is 12.13 m/s, and the estimated ride duration is 0.33 seconds.

---

**👤 You:**
> "How fast is a wave moving if the breaking depth is 5 meters?"

**🤖 AI Agent:**
> The wave speed is 22.12 m/s.

---

**👤 You:**
> "Is a wave with a 65 degree angle and a 2 degree slope a good barrel?"

**🤖 AI Agent:**
> Yes, the barrel potential is High.


## ❓ FAQ

**Q: How do I calculate the full wave profile?**
Use the `calculate_wave_geometry` tool. Provide the wave height, breaking depth, and beach slope to receive the angle, potential score, speed, and duration.

**Q: Can I just find out how fast a wave is moving?**
Yes, use the `get_wave_speed` tool by providing the breaking depth in meters.

**Q: What determines the barrel potential score?**
The score is determined by the wave face angle and the beach slope. You can use `evaluate_barrel_quality` to check this specifically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wave-face-angle-barrel-geometry-calculator](https://vinkius.com/ai-agent-connect/wave-face-angle-barrel-geometry-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Face Angle & Barrel Geometry Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-face-angle-barrel-geometry-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Face Angle & Barrel Geometry Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-face-angle-barrel-geometry-calculator": {
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
