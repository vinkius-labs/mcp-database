# Wave Forecast Interpreter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-forecast-interpreter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Translates raw oceanographic data into actionable surf conditions.

## Description
This MCP server acts as a bridge between raw oceanographic forecast data and surfers. It interprets the complex interactions between swell height, wave period, swell direction, and wind to provide accurate surf quality ratings. By accounting for local bathymetry and coastline orientation, it uses tools like `analyze_swell_quality` and `find_best_surf_windows` to predict breaking wave heights and identify the best time windows for surfing. It also helps determine how seafloor types like reef or sand affect wave energy via `calculate_bathymetry_adjustment` and evaluates wind impact using `check_wind_alignment`.


## Available Tools (4)
- **analyze_swell_quality**: Answers "How good will the surf be at a specific location during a given time?"
- **calculate_bathymetry_adjustment**: Answers "How will the local seafloor change the raw swell height?"
- **check_wind_alignment**: Answers "Is the wind helping or hurting the surf quality?"
- **find_best_surf_windows**: Answers "When is the best time to go surfing within a given forecast period?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Forecast Interpreter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How good will the surf be with a 2m swell, 14s period, 180 degree swell direction, 190 degree wind direction, 5 knot wind, and a 170 degree coastline?"

**🤖 AI Agent:**
> The surf will be Epic. The high period and offshore wind alignment will create excellent, clean waves with an expected height of 2.2 meters.

---

**👤 You:**
> "Is the wind helping or hurting the surf if the wind is from 270 degrees and the coast faces 90 degrees?"

**🤖 AI Agent:**
> The wind is Offshore, which will help groom the wave faces and improve surf quality.

---

**👤 You:**
> "How will a 1.5m swell with a 10s period change if it hits a reef bottom?"

**🤖 AI Agent:**
> On a reef bottom, the expected breaking wave height will increase to 1.8 meters due to the concentrated energy.


## ❓ FAQ

**Q: How accurate are the surf quality ratings?**
The ratings are calculated by analyzing the synergy of swell period, height, and wind alignment relative to the coastline, providing a highly reliable estimate of surf conditions.

**Q: Can I use this to find the best time to surf?**
Yes, you can use the `find_best_surf_windows` tool to scan forecast data and identify specific time intervals where conditions are optimal.

**Q: Does it account for different types of ocean floors?**
Yes, the `calculate_bathymetry_adjustment` tool adjusts expected wave heights based on whether the seafloor is reef, sand, or rock.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-forecast-interpreter](https://vinkius.com/en/ai-agent-connect/wave-forecast-interpreter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Forecast Interpreter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-forecast-interpreter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Forecast Interpreter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-forecast-interpreter": {
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
