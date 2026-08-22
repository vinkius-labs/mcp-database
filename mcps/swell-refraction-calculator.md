# Swell Refraction Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/swell-refraction-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Predict wave refraction, height changes, and breaking stability using Snell's and Green's Laws.

## Description
This MCP server provides deterministic oceanographic calculations to model how swell energy transforms as it moves from deep to shallow water. By applying Snell's Law for refraction and Green's Law for height transformation, it allows AI agents to predict wave direction changes, height multipliers, and wave steepness. Use `get_refracted_wave_properties` to calculate full physical transformations, `get_refraction_summary` for quick comparisons, or `validate_swell_stability` to check if a wave is approaching its breaking limit.


## Available Tools (3)
- **get_refracted_wave_properties**: Calculates wave refraction properties
- **get_refraction_summary**: Provides refraction summary
- **validate_swell_stability**: Checks swell stability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swell Refraction Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the properties of a swell with a 20 degree angle in deep water, moving at 15 m/s, into shallow water moving at 5 m/s, with an initial height of 2 meters and a wavelength of 15 meters."

**🤖 AI Agent:**
> The wave will refract to an angle of 9.59 degrees. The predicted shallow water height is 2.58 meters, with a wave steepness of 0.17. Since the steepness is above 0.14, the wave is predicted to break.

---

**👤 You:**
> "Give me a summary of the refraction for a 10m swell at 12 m/s, 30 degrees angle, moving into water with 4 m/s speed."

**🤖 AI Agent:**
> The wave height multiplier is 1.85 and the angle change is 21.45 degrees.

---

**👤 You:**
> "Is a wave with a steepness of 0.12 stable?"

**🤖 AI Agent:**
> Yes, the wave is stable with a safety margin of 0.02.


## ❓ FAQ

**Q: What physical laws does this server use?**
The server utilizes Snell's Law to calculate the refraction angle and Green's Law to approximate the change in wave height as it enters shallower water.

**Q: How is wave breaking determined?**
A wave is flagged as breaking if its calculated steepness exceeds the stability threshold of 0.14.

**Q: Can I use custom stability thresholds?**
Yes, the `validate_swell_stability` tool allows you to provide a custom target threshold for steepness checks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/swell-refraction-calculator](https://vinkius.com/ai-agent-connect/swell-refraction-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swell Refraction Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swell-refraction-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swell Refraction Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swell-refraction-calculator": {
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
