# Houseplant Light Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/houseplant-light-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate light deficits and optimal plant placement using DLI and lux measurements.

## Description
This MCP server provides precision tools for indoor gardeners to manage plant health through light analysis. By using `calculate_dli`, you can convert lux measurements into Daily Light Integral (DLI) to understand the total energy available for photosynthesis. Use `check_plant_suitability` to determine if a specific species is receiving enough light, or `estimate_window_distance_impact` to predict how moving a plant further from a window will affect its light levels based on the inverse square law. Finally, `get_placement_recommendation` provides direct instructions on whether to move a plant closer to a light source or supplement with grow lights.


## Available Tools (4)
- **calculate_dli**: Converts a single light intensity measurement and duration into the total daily energy received
- **check_plant_suitability**: Compares measured light against a plant's requirements to identify if the environment is sufficient
- **estimate_window_distance_impact**: Predicts how much light will be lost if a plant is moved further away from a light source
- **get_placement_recommendation**: Provides a deterministic instruction for where to move a plant based on its current light deficit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Houseplant Light Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My plant is getting 5000 lux for 8 hours a day. What is the DLI?"

**🤖 AI Agent:**
> The total Daily Light Integral (DLI) for your plant is 40.0.

---

**👤 You:**
> "I have a plant that needs 400 DLI, but it's only getting 250 DLI. It is currently near the window. What should I do?"

**🤖 AI Agent:**
> Move closer to the light source.

---

**👤 You:**
> "If I move my plant from 20cm to 40cm away from the window, how much light will it lose?"

**🤖 AI Agent:**
> The light intensity will decrease by 75%.


## ❓ FAQ

**Q: How do I use the DLI tool?**
You can use `calculate_dli` by providing the measured lux and the number of hours the light is maintained to find the total daily energy.

**Q: Can I predict light loss from moving my plant?**
Yes, `estimate_window_distance_impact` uses the inverse square law to predict how much light intensity will decrease as you move the plant away from the window.

**Q: What if my plant is not getting enough light?**
Use `get_placement_recommendation` to receive specific instructions, such as moving the plant closer to the window or using artificial grow lights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/houseplant-light-estimator](https://vinkius.com/en/ai-agent-connect/houseplant-light-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Houseplant Light Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `houseplant-light-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Houseplant Light Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "houseplant-light-estimator": {
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
