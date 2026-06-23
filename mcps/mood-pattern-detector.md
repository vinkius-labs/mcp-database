# Mood Pattern Detector MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mood-pattern-detector)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Identify recurring emotional trends and correlations between mood fluctuations and lifestyle variables.

## Description
The Mood Pattern Detector analyzes historical mood logs to uncover cyclical patterns and the impact of external factors. Use `analyze_weekly_cycle` to find days associated with specific moods, `evaluate_activity_impact` to measure how variables like exercise or sleep influence your emotional state, and `identify_mood_anomalies` to flag significant deviations from your baseline mood.


## Available Tools (3)
- **analyze_weekly_cycle**: Determine if specific days of the week are associated with better or worse moods
- **evaluate_activity_impact**: Measure how a specific recorded variable influences mood levels
- **identify_mood_anomalies**: Flag specific dates where the mood was significantly different from the norm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mood Pattern Detector** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Are there any specific days of the week where my mood tends to be lower?"

**🤖 AI Agent:**
> The `analyze_weekly_cycle` tool would examine your logs and return the day with the lowest average mood score, such as identifying a 'Monday Slump'.

---

**👤 You:**
> "Does my exercise routine affect my emotional well-being?"

**🤖 AI Agent:**
> By using `evaluate_activity_impact` with 'exercise' as the variable, the tool will compare your average mood on days you exercised versus days you did not.

---

**👤 You:**
> "Check if there were any unusual spikes or drops in my mood recently."

**🤖 AI Agent:**
> The `identify_mood_anomalies` tool will scan your historical data and list specific dates where your mood was significantly higher or lower than your norm.


## ❓ FAQ

**Q: How does the detector identify weekly patterns?**
The `analyze_weekly_pattern` tool calculates the average mood score for each day of the week present in your logs and identifies significant differences between days.

**Q: Can I analyze specific activities like exercise or sleep?**
Yes, using `evaluate_activity_impact`, you can provide the name of any recorded variable to see its correlation with your mood levels.

**Q: What constitutes a mood anomaly?**
An anomaly is flagged by `identify_mood_anomalies` when a specific day's mood score deviates from your historical baseline beyond a defined sensitivity threshold.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mood-pattern-detector](https://vinkius.com/mcp/mood-pattern-detector)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mood Pattern Detector** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mood-pattern-detector` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mood Pattern Detector** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mood-pattern-detector": {
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
