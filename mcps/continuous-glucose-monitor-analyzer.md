# Continuous Glucose Monitor Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/continuous-glucose-monitor-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Analyze CGM data to track glucose variability, meal impact, and metabolic health.

## Description
This MCP server provides advanced tools for analyzing Continuous Glucose Monitor (CGM) data. It allows AI agents to calculate key metabolic indicators such as Time in Range (TIR), glucose variability, and the impact of lifestyle factors. Use `get_glucose_summary` to get a high-level overview of glucose status, `analyze_postprandial_impact` to see how meals affect glucose levels, `evaluate_exercise_response` to measure exercise sensitivity, `assess_sleep_stability` to monitor overnight glucose, and `calculate_metabolic_health_score` for a comprehensive health assessment.


## Available Tools (5)
- **get_glucose_summary**: Get general glucose status over a period
- **analyze_postprandial_impact**: Analyze how meals affect glucose levels
- **assess_sleep_stability**: Assess glucose stability during sleep
- **calculate_metabolic_health_score**: Calculate overall metabolic health score
- **evaluate_exercise_response**: Evaluate glucose response to exercise


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Continuous Glucose Monitor Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my general glucose status for these readings: [{"timestamp": "2023-10-01T08:00:00Z", "value": 110}, {"timestamp": "2023-10-01T08:05:00Z", "value": 115}]?"

**🤖 AI Agent:**
> Your average glucose was 112.5 mg/dL, with a variability index of 2.5 and 100% time in range.

---

**👤 You:**
> "How much did my meal at 12:00 PM affect my glucose? Readings: [{"timestamp": "2023-10-01T11:55:00Z", "value": 95}, {"timestamp": "2023-10-01T12:00:00Z", "value": 100}, {"timestamp": "2023-10-01T12:30:00Z", "value": 140}]"

**🤖 AI Agent:**
> The meal caused a spike magnitude of 40 mg/dL, reaching a peak at 12:30 PM with a recovery time of 45 minutes.

---

**👤 You:**
> "Did my exercise at 5:00 PM help stabilize my glucose? Readings: [{"timestamp": "2023-10-01T16:55:00Z", "value": 120}, {"timestamp": "2023-10-01T17:05:00Z", "value": 110}]"

**🤖 AI Agent:**
> Yes, the exercise resulted in a glucose drop magnitude of 10 mg/dL and improved your sensitivity score.


## ❓ FAQ

**Q: What kind of data can I analyze?**
You can analyze raw glucose readings, meal timestamps, exercise logs, and sleep windows to get detailed metabolic insights.

**Q: How do I calculate my metabolic health score?**
You can use the `calculate_metabolic_health_score` tool by providing a glucose summary and lifestyle factor data.

**Q: Can I see how my meals affect my glucose?**
Yes, the `analyze_postprandial_impact` tool calculates spike magnitude and recovery time following meal timestamps.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/continuous-glucose-monitor-analyzer](https://vinkius.com/en/ai-agent-connect/continuous-glucose-monitor-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Continuous Glucose Monitor Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `continuous-glucose-monitor-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Continuous Glucose Monitor Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "continuous-glucose-monitor-analyzer": {
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
