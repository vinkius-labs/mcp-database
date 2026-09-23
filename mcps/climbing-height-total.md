# Climbing Height Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/climbing-height-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Calculate cumulative vertical gain and analyze climbing pitch data.

## Description
This MCP server provides specialized tools for climbers to manage and analyze route data. You can use `get_total_vertical_gain` to sum up the height of multiple segments, `validate_pitch_data` to ensure measurements meet safety standards, `get_average_pitch_height` to find the mean distance per pitch, and `format_climbing_summary` to generate a natural language summary of the climb.


## Available Tools (4)
- **format_climbing_summary**: 
- **get_average_pitch_height**: 
- **get_total_vertical_gain**: 
- **validate_pitch_data**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Climbing Height Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total vertical gain for pitches of 30m, 50m, and 20m?"

**🤖 AI Agent:**
> The total vertical gain is 100 meters.

---

**👤 You:**
> "Is a 120m single pitch valid?"

**🤖 AI Agent:**
> No, the pitch height exceeds standard maximum single-pitch limits.

---

**👤 You:**
> "What is the average height of three 15m pitches?"

**🤖 AI Agent:**
> The average height is 15 meters.


## ❓ FAQ

**Q: How do I calculate the total height of my route?**
You can use the `get_total_vertical_gain` tool by providing an array of the individual pitch heights.

**Q: Can this tool check if my pitch heights are safe?**
Yes, the `validate_pitch_data` tool checks if pitch heights are positive and within standard climbing limits.

**Q: How can I get a summary of my climb?**
Use the `format_climbing_summary` tool with the total height and pitch count to get a human-readable sentence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/climbing-height-total](https://vinkius.com/en/ai-agent-connect/climbing-height-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Climbing Height Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `climbing-height-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Climbing Height Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "climbing-height-total": {
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
