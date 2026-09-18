# Wim Hof Breathing Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wim-hof-breathing-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A specialized timing engine for structured Wim Hof Method breathing sessions.

## Description
This MCP server provides precise timing and sequencing for the Wim Hof Method. It helps users manage the cyclical nature of breathing rounds by calculating specific durations for breathing phases, breath retention, and recovery breaths. Use `calculate_session_schedule` to generate a full timeline, `get_breathing_parameters` to find rhythmic settings, `estimate_recovery_needs` for recovery durations, and `validate_session_viability` to ensure session safety based on experience levels.


## Available Tools (4)
- **calculate_session_schedule**: Generates a complete, round-by-round timing schedule for a full breathing session
- **estimate_recovery_needs**: Calculates the required duration for the recovery breath based on intensity
- **get_breathing_parameters**: Determines the specific rhythmic settings for the active breathing phase
- **validate_session_viability**: Checks if the requested session parameters are safe or appropriate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wim Hof Breathing Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you create a 3-round breathing schedule for a beginner with a 1-minute retention goal?"

**🤖 AI Agent:**
> Round 1: Breathing for 30s, Retention for 60s, Recovery for 15s. Round 2: Breathing for 30s, Retention for 60s, Recovery for 15s. Round 3: Breathing for 30s, Retention for 60s, Recovery for 15s.

---

**👤 You:**
> "What are the breathing parameters for an advanced user?"

**🤖 AI Agent:**
> For an advanced user, the breathing phase includes a higher number of breaths per round with a faster, more aggressive pace to facilitate CO2 depletion.

---

**👤 You:**
> "Is a 3-minute retention goal safe for a beginner?"

**🤖 AI Agent:**
> No, a 3-minute retention goal is not recommended for the beginner level as it may cause physiological distress.


## ❓ FAQ

**Q: How do I know if my session is safe?**
You can use the `validate_session_viability` tool to check if your requested retention goal and experience level are appropriate and safe.

**Q: Can I plan a full session at once?**
Yes, the `calculate_session_schedule` tool generates a complete, round-by-round timing schedule including breathing, retention, and recovery phases.

**Q: What experience levels are supported?**
The server supports Beginner, Intermediate, and Advanced experience levels to tailor the breathing intensity and pace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wim-hof-breathing-timer](https://vinkius.com/en/ai-agent-connect/wim-hof-breathing-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wim Hof Breathing Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wim-hof-breathing-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wim Hof Breathing Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wim-hof-breathing-timer": {
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
