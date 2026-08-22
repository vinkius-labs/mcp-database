# Wind Direction & Beach Orientation Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wind-direction-beach-orientation-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Analyze wind conditions and beach orientation to determine surfing suitability.

## Description
This MCP server provides deterministic tools to evaluate how wind direction and speed affect surfing conditions relative to a beach's orientation. Use `analyze_wind_conditions` to get a full assessment including wind type, quality score, and a surf verdict. You can also use `get_wind_type_metadata` to understand the impact of specific wind types like Offshore or Onshore, or `calculate_raw_quality_score` to find the base score for a given wind classification.


## Available Tools (3)
- **analyze_wind_conditions**: Provides a complete assessment of surf suitability based on wind and beach orientation
- **calculate_raw_quality_score**: Determines the base quality score before wind speed penalties are applied
- **get_wind_type_metadata**: Answers what specific angular ranges correspond to which wind type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wind Direction & Beach Orientation Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "The wind is coming from 200 degrees at 10 knots, and the beach faces 20 degrees. How are the surfing conditions?"

**🤖 AI Agent:**
> The angular difference is 180 degrees, which is an Offshore wind. The wind quality score is 100, providing excellent surfing conditions.

---

**👤 You:**
> "What is the impact of an Onshore wind?"

**🤖 AI Agent:**
> Onshore wind blows from the land toward the ocean, creating choppy and turbulent water conditions, which is not ideal for surfing.

---

**👤 You:**
> "The wind is 270 degrees at 20 knots, and the beach faces 90 degrees. What is the verdict?"

**🤖 AI Agent:**
> The angular difference is 180 degrees (Offshore). However, because the wind speed is 20 knots, a 20-point penalty is applied. The final wind quality score is 80.


## ❓ FAQ

**Q: How do I know if the wind is good for surfing?**
You can use the `analyze_wind_conditions` tool. It will tell you if the wind is Offshore (ideal), Cross-shore, or Onshore (choppy) based on the wind direction and the beach facing angle.

**Q: What does an Offshore wind mean?**
Offshore wind blows from the ocean toward the land, which helps smooth the wave faces, making it the ideal condition for surfing.

**Q: Does wind speed affect the score?**
Yes, if the wind speed exceeds 15 knots, a penalty is applied to the wind quality score, reducing the overall surf suitability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wind-direction-beach-orientation-analyzer](https://vinkius.com/ai-agent-connect/wind-direction-beach-orientation-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wind Direction & Beach Orientation Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wind-direction-beach-orientation-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wind Direction & Beach Orientation Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wind-direction-beach-orientation-analyzer": {
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
