# Paddle Stroke Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/paddle-stroke-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate total paddling strokes and session intensity.

## Description
This MCP server provides tools to quantify paddling effort. Use `get_total_strokes` to find the total number of strokes, `get_cadence_intensity` to determine rhythm intensity, `get_session_summary` for a full report, or `validate_paddling_stats` to check if metrics are physically plausible.


## Available Tools (4)
- **get_cadence_intensity**: Determine the intensity level of the paddling rhythm
- **get_session_summary**: Get a complete breakdown of the paddling session
- **get_total_strokes**: Calculate total strokes performed during a session
- **validate_paddling_stats**: Validate if the provided paddling metrics are physically plausible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paddle Stroke Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many total strokes did I perform if I paddled for 30 minutes at 45 strokes per minute?"

**🤖 AI Agent:**
> You performed a total of 1,350 strokes.

---

**👤 You:**
> "What was the intensity of my 15-minute paddle at 60 strokes per minute?"

**🤖 AI Agent:**
> Your paddling intensity was High.

---

**👤 You:**
> "Give me a summary for a 20 minute session with 50 strokes per minute."

**🤖 AI Agent:**
> Your session included 1,000 total strokes with an average cadence of 50 strokes per minute over 20 minutes, resulting in Moderate intensity.


## ❓ FAQ

**Q: How do I calculate my total strokes?**
You can use the `get_total_strokes` tool by providing your total duration in minutes and your cadence in strokes per minute.

**Q: Can I verify if my recorded data is accurate?**
Yes, the `validate_paddling_stats` tool checks if your duration, cadence, and total strokes are physically consistent.

**Q: What information is included in the session summary?**
The `get_session_summary` tool provides the total strokes, average cadence, session duration, and the calculated intensity level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/paddle-stroke-counter](https://vinkius.com/en/ai-agent-connect/paddle-stroke-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paddle Stroke Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paddle-stroke-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paddle Stroke Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paddle-stroke-counter": {
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
