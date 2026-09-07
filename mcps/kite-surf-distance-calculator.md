# Kite-Surf Distance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/kite-surf-distance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate kite-surfing session metrics including total distance, upwind/downwind travel, and active duration.

## Description
This MCP server provides specialized tools for kite-surfers to analyze their session performance. By accounting for environmental factors like tacking angles and operational time like relaunching, it provides precise distance metrics. Use `calculate_session_metrics` to get a full breakdown of total, upwind, and downwind distances, or `get_active_time_only` to isolate actual movement time from rest periods.


## Available Tools (4)
- **calculate_session_metrics**: Provides a comprehensive breakdown of all distance metrics for a specific kite-surfing session
- **compare_session_efficiency**: Compares the total distance of two sessions to determine which was more productive
- **estimate_tacking_penalty**: Calculates how much the tacking angle reduces the efficiency of upwind progress
- **get_active_time_only**: Isolates the actual time spent moving during a session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kite-Surf Distance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my session metrics: I rode for 45 minutes at 6 m/s, with a 5% upwind component and a 30 degree tacking angle. I spent 5 minutes relaunching."

**🤖 AI Agent:**
> Your session metrics are: Total distance: 15.3 km, Upwind distance: 0.77 km, Downwind distance: 14.53 km, and Active duration: 40 minutes.

---

**👤 You:**
> "How much time did I actually spend moving if my session was 60 minutes long, but I rested for 15 minutes and spent 5 minutes relaunching?"

**🤖 AI Agent:**
> Your active duration was 40 minutes.

---

**👤 You:**
> "What is the efficiency factor for a 45 degree tacking angle?"

**🤖 AI Agent:**
> The efficiency factor for a 45 degree angle is 0.707.


## ❓ FAQ

**Q: How does the tool account for time spent on the beach?**
The `calculate_session_metrics` tool allows you to input `restDuration` and `relaunchTime` to ensure only the active movement time is used for distance calculations.

**Q: What is a tacking angle?**
A tacking angle is the zig-zag path taken when traveling upwind. You can use `estimate_tacking_penalty` to see how this angle affects your efficiency.

**Q: Can I compare two different sessions?**
Yes, you can use `compare_session_efficiency` to determine which of two sessions resulted in more total distance covered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/kite-surf-distance-calculator](https://vinkius.com/ai-agent-connect/kite-surf-distance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kite-Surf Distance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kite-surf-distance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kite-Surf Distance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kite-surf-distance-calculator": {
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
