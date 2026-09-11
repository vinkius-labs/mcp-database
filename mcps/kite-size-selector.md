# Kite Size Selector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kite-size-selector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Calculates optimal kite dimensions based on rider weight, wind, and equipment.

## Description
This MCP server provides precise kite sizing recommendations for kiteboarders. By analyzing rider mass, wind velocity, skill level, and board type, it calculates the ideal kite surface area. Use `get_recommended_kite_size` for a single optimal size, `get_gust_resilience_range` to prepare for wind fluctuations, `compare_equipment_requirements` to see how switching from a twin-tip to a foil changes your needs, and `validate_safety_threshold` to confirm if a specific kite is safe for your current profile.


## Available Tools (4)
- **compare_equipment_requirements**: Shows how the recommended kite size changes when switching between different board types in the same wind
- **get_gust_resilience_range**: Helps a rider prepare for fluctuating wind speeds by providing a range of suitable kite sizes
- **get_recommended_kite_size**: Provides the single most appropriate kite size for the current conditions
- **validate_safety_threshold**: Checks if a specific kite size is safe to use given the current wind and rider profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kite Size Selector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 80kg, the wind is 15 knots, I am an intermediate rider, and I am using a twin-tip. What kite size should I use?"

**🤖 AI Agent:**
> Based on your profile, the recommended kite size is 11.5 m².

---

**👤 You:**
> "What is the safe kite size range for an 70kg beginner using a surfboard in 12 knots of wind?"

**🤖 AI Agent:**
> For your conditions, the suitable kite size range is between 12.5 m² and 14.0 m².

---

**👤 You:**
> "Is a 9 m² kite safe for an 85kg advanced rider on a foil in 20 knots of wind?"

**🤖 AI Agent:**
> Yes, a 9 m² kite is safe for your current conditions.


## ❓ FAQ

**Q: How does board type affect kite size?**
Different boards have different drag profiles. For example, a foil has very low drag, so you need a smaller kite compared to a surfboard which has higher drag.

**Q: Can I use this to check if my kite is safe?**
Yes, you can use `validate_safety_threshold` to check if a specific kite size is safe given your weight, wind speed, and skill level.

**Q: Does skill level matter for the calculation?**
Yes, skill level determines the safety margin. Beginners require more stability and larger kites, while advanced riders can handle smaller, more reactive kites.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kite-size-selector](https://vinkius.com/en/ai-agent-connect/kite-size-selector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kite Size Selector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kite-size-selector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kite Size Selector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kite-size-selector": {
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
