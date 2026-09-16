# Video Analysis Metrics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/video-analysis-metrics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports-analytics](../categories/sports-analytics.md)

Generates quantitative metrics from surf video analysis.

## Description
This MCP server provides tools to extract precise performance data from surfing videos. By processing body position coordinates and timestamps, it calculates critical timing metrics using `get_timing_metrics`. It also measures body posture through `get_posture_angles`, accounting for camera perspective distortion. Users can quantify performance gaps by comparing actual posture to professional standards with `get_performance_deviation`, and obtain a complete overview of a maneuver using `get_maneuver_summary`.


## Available Tools (4)
- **get_maneuver_summary**: Provides a high-level quantitative overview of a completed surfing sequence
- **get_performance_deviation**: Compares the surfer's actual posture against professional standards
- **get_posture_angles**: Measures the angular orientation of the surfer's body segments
- **get_timing_metrics**: Calculates the duration of critical phases in a surfing maneuver


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Video Analysis Metrics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the duration of the takeoff phase from these body positions: [{"timestamp": 100, "landmarks": {"head": [10, 20]}}, {"timestamp": 150, "landmarks": {"head": [12, 22]}}, {"timestamp": 200, "landmarks": {"head": [15, 25]}}]."

**🤖 AI Agent:**
> The takeoff phase lasted 100 seconds.

---

**👤 You:**
> "What is the summary of the maneuver with these timing metrics and posture angles?"

**🤖 AI Agent:**
> The total maneuver duration was 12.5 seconds with an average posture accuracy of 88%.

---

**👤 You:**
> "Check the posture angle for frame 45 with a camera correction of 1.1."

**🤖 AI Agent:**
> The torso inclination angle is 42 degrees.


## ❓ FAQ

**Q: How does the tool handle different camera angles?**
The `get_posture_angles` tool accepts a camera correction factor to adjust spatial measurements for perspective distortion.

**Q: What kind of timing data can I get?**
You can use `get_timing_metrics` to calculate the duration of specific phases like the takeoff or the bottom turn.

**Q: Can I compare my performance to professionals?**
Yes, `get_performance_deviation` compares your actual body angles against professional standards to show exactly where you can improve.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/video-analysis-metrics](https://vinkius.com/en/ai-agent-connect/video-analysis-metrics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Video Analysis Metrics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `video-analysis-metrics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Video Analysis Metrics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "video-analysis-metrics": {
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
