# Surf Session Efficiency Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/surf-session-efficiency-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Analyze surfing session performance and efficiency.

## Description
This MCP server provides deterministic tools to calculate key performance indicators for surfing sessions. Use `analyze_session_efficiency` to get a full breakdown of metrics including active surf time, waves per hour, and a qualitative session quality score. You can also use `get_session_summary_stats` for a quick overview or `validate_session_data` to ensure your session parameters are logically sound.


## Available Tools (3)
- **analyze_session_efficiency**: Calculates all primary efficiency and quality metrics for a single surfing session
- **get_session_summary_stats**: Provides a high-level summary of session throughput
- **validate_session_data**: Verifies if the provided session parameters are physically possible and logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Session Efficiency Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a 60 minute session where I paddled out for 10 minutes, caught 5 waves, and each ride lasted 20 seconds."

**🤖 AI Agent:**
> Active surf time: 100 seconds. Efficiency ratio: 0.027. Waves per hour: 5.0. Paddle-to-ride ratio: 6.0. Session quality: Crowded/Flat.

---

**👤 You:**
> "Give me a quick summary for a 30 minute session with 10 waves caught."

**🤖 AI Agent:**
> Waves per hour: 20.0. Active surf time: 100 seconds (assuming 10s average ride).

---

**👤 You:**
> "Is it possible to have a 20 minute session with 30 minutes of paddling?"

**🤖 AI Agent:**
> No, the session data is invalid because paddle time cannot exceed total session time.


## ❓ FAQ

**Q: What metrics does this server provide?**
It provides active surf time, efficiency ratio, waves per hour, paddle-to-ride ratio, and a session quality score using `analyze_session_efficiency`.

**Q: How is the session quality determined?**
Quality is based on the efficiency ratio: above 0.15 is 'Epic', 0.05-0.15 is 'Good', and below 0.05 is 'Crowded/Flat'.

**Q: Can I validate my session data before analysis?**
Yes, use the `validate_session_data` tool to check if your session parameters are physically possible.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/surf-session-efficiency-metrics](https://vinkius.com/ai-agent-connect/surf-session-efficiency-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Session Efficiency Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-session-efficiency-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Session Efficiency Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-session-efficiency-metrics": {
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
