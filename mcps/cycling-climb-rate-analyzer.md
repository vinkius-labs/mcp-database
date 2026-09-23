# Cycling Climb Rate Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cycling-climb-rate-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [performance](../categories/performance.md)

Calculate vertical ascent rate (VAM) and analyze climbing performance.

## Description
This MCP server provides specialized tools for cycling performance analysis. It allows AI agents to calculate the vertical ascent rate (VAM) using `get_climb_rate`, verify segment data with `validate_climb_segment`, categorize climbing intensity with `get_climb_intensity_tier`, and compare different climbing attempts using `compare_climb_segments`.


## Available Tools (4)
- **compare_climb_segments**: Compares two different climb attempts to identify performance changes
- **get_climb_intensity_tier**: Categorizes a climb rate into standard performance intensity levels
- **get_climb_rate**: Calculates the vertical ascent rate (VAM) for a specific segment
- **validate_climb_segment**: Checks if a recorded climb segment is mathematically valid for analysis


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling Climb Rate Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my climb rate if I gained 500 meters in 1200 seconds?"

**🤖 AI Agent:**
> Your climb rate (VAM) is 1500 meters per hour.

---

**👤 You:**
> "Is a climb rate of 1200 VAM considered high intensity?"

**🤖 AI Agent:**
> A climb rate of 1200 VAM is categorized as High intensity.

---

**👤 You:**
> "Compare a climb of 300m in 1000s to a climb of 350m in 900s."

**🤖 AI Agent:**
> The second climb showed an improvement with a performance increase of approximately 11.11%.


## ❓ FAQ

**Q: What is VAM?**
VAM (Velocità Ascensionale Media) is the vertical meters gained per hour, a standard metric for measuring climbing intensity in cycling.

**Q: How can I compare two different climbs?**
You can use the `compare_climb_segments` tool by providing the elevation gain and duration for both attempts.

**Q: Can I check if my climb data is valid?**
Yes, the `validate_climb_segment` tool checks if your elevation gain and duration are mathematically valid for analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cycling-climb-rate-analyzer](https://vinkius.com/en/ai-agent-connect/cycling-climb-rate-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling Climb Rate Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-climb-rate-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling Climb Rate Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-climb-rate-analyzer": {
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
