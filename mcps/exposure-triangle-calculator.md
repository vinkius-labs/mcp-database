# Exposure Triangle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/exposure-triangle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calculators](../categories/calculators.md)

Deterministic photographic exposure calculator for aperture, shutter speed, and ISO adjustments.

## Description
This MCP server provides precise tools for managing the photographic exposure triangle. Use `calculate_exposure_shift` to find new settings when changing stops, `evaluate_scene_brightness` to determine the current Exposure Value (EV) and Light Value (LV), or `calculate_metering_compensation` to adjust for different metering modes. It handles fractional stops and flags impossible hardware constraints like flash sync limits.


## Available Tools (3)
- **calculate_exposure_shift**: Calculates new exposure settings when a user wants to change one or more parameters by a specific number of stops
- **calculate_metering_compensation**: g., from Matrix to Spot) and needs to adjust exposure.

Calculates the exposure compensation required when switching between different metering modes
- **evaluate_scene_brightness**: Determines the current Exposure Value (EV) and Light Value (LV) based on current settings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Exposure Triangle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am at f/5.6, 1/125s, and ISO 400. I want to open my aperture by 2 stops. What are my new settings?"

**🤖 AI Agent:**
> Your new settings are f/2.8, 1/125s, and ISO 400.

---

**👤 You:**
> "What is the current brightness (EV and LV) for f/8, 1/250s, and ISO 100?"

**🤖 AI Agent:**
> The current Exposure Value (EV) is 11 and the Light Value (LV) is 11.

---

**👤 You:**
> "I'm switching from Matrix to Spot metering and expect a 1.5 stop difference. How much compensation do I need?"

**🤖 AI Agent:**
> You need 1.5 stops of compensation, resulting in a suggested new EV of 12.5.


## ❓ FAQ

**Q: How do I maintain the same exposure when changing one setting?**
You can use the `calculate_exposure_shift` tool. By providing your current settings and specifying the desired change for one parameter, the tool calculates the necessary adjustments for the others to keep the total exposure constant.

**Q: Can this tool handle fractional stops?**
Yes, the calculator supports fractional stop adjustments, including 1/3, 1/2, and 2/3 stops, for precise exposure control.

**Q: What happens if I request an impossible exposure setting?**
If a requested setting violates physical constraints, such as a shutter speed faster than the flash sync speed or an aperture smaller than the lens allows, the tool will flag the combination as impossible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/exposure-triangle-calculator](https://vinkius.com/ai-agent-connect/exposure-triangle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Exposure Triangle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `exposure-triangle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Exposure Triangle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "exposure-triangle-calculator": {
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
