# Surf Wave Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-wave-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Track wave counts and session density for your surfing sessions.

## Description
This MCP server provides tools to analyze surfing performance. You can use `get_total_wave_count` to find the sum of waves caught in a timeframe, `get_waves_per_session_average` to calculate wave density, `get_session_summary` for specific session details, and `get_wave_activity_by_tier` to view trends over daily or weekly increments.


## Available Tools (4)
- **get_session_summary**: Get details of a specific surfing session
- **get_total_wave_count**: Get the total number of waves caught within a specific timeframe
- **get_wave_activity_by_tier**: Get wave catching trends over daily or weekly increments
- **get_waves_per_session_average**: Get the average wave density per session for a given period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Wave Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many waves did I catch between 2024-01-01 and 2024-01-31?"

**🤖 AI Agent:**
> You caught a total of 42 waves during January 2024.

---

**👤 You:**
> "What was my average wave density last week?"

**🤖 AI Agent:**
> Your average wave density last week was 8 waves per session across 5 sessions.

---

**👤 You:**
> "Show me my wave trends for the last 7 days using daily increments."

**🤖 AI Agent:**
> Your wave activity for the last 7 days was: 2024-05-01: 5 waves, 2024-05-02: 8 waves, 2024-05-03: 4 waves.


## ❓ FAQ

**Q: How do I see my total waves for the month?**
You can use the `get_total_wave_count` tool by providing the start and end timestamps for the month.

**Q: Can I see my wave density?**
Yes, use `get_waves_per_session_average` to find the average number of waves caught per session.

**Q: How do I check a specific session?**
Provide the session ID to the `get_session_summary` tool to retrieve its details.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-wave-analytics](https://vinkius.com/en/ai-agent-connect/surf-wave-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Wave Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-wave-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Wave Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-wave-analytics": {
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
