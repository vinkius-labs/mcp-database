# Sliding Window Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sliding-window-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Deterministic engine for sliding window metric aggregation, trend analysis, and anomaly detection.

## Description
This MCP server provides a deterministic engine for processing timestamped metric streams into sliding windows. It enables precise monitoring by calculating windowed aggregations like sum, average, and percentiles. Use `process_metrics` to transform raw data into windowed results, `analyze_trends` to determine the direction of metric movement via linear regression, and `check_alerts` to identify sustained threshold violations. The engine also detects sensor malfunctions and data gaps automatically.


## Available Tools (3)
- **check_alerts**: Checks for threshold violations
- **analyze_trends**: Calculates trend direction
- **process_metrics**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sliding Window Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Process these metrics: [{'timestampMs': 1672531200000, 'value': 10}, {'timestampMs': 1672531260000, 'value': 20}] with a window size of 60000 and slide interval of 60000 using avg aggregation."

**🤖 AI Agent:**
> { "windows": [{ "startMs": 1672531200000, "endMs": 1672531260000, "value": 15, "isGap": false, "isMalfunction": false }] }

---

**👤 You:**
> "Check if these windows trigger an alert for a threshold of 50: [{'timestampMs': 1000, 'value': 60}, {'timestampMs': 2000, 'value': 65}, {'timestampMs': 3000, 'value': 70}]."

**🤖 AI Agent:**
> { "isAlerting": true, "consecutiveViolations": 3 }

---

**👤 You:**
> "Analyze the trend for these window values: [{'timestampMs': 1000, 'value': 10}, {'timestampMs': 2000, 'value': 20}]."

**🤖 AI Agent:**
> { "slope": 10, "direction": "increasing", "isStable": false }


## ❓ FAQ

**Q: How does the engine handle window overlaps?**
Overlaps occur when the window size is larger than the slide interval. The engine calculates these windows deterministically based on your provided parameters.

**Q: What triggers an alert?**
An alert is triggered via `check_alerts` if a metric exceeds the specified threshold for three consecutive windows.

**Q: How is a sensor malfunction detected?**
A malfunction flag is set if more than 50% of the data points in a window are identified as statistical outliers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sliding-window-aggregator](https://vinkius.com/ai-agent-connect/sliding-window-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sliding Window Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sliding-window-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sliding Window Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sliding-window-aggregator": {
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
