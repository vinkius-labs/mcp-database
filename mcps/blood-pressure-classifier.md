# Blood Pressure Classifier MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/blood-pressure-classifier)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Classify blood pressure readings, detect trends, and identify hypertensive alerts using AHA/WHO standards.

## Description
This MCP server provides specialized tools for monitoring cardiovascular health. It allows AI agents to `classify_single_reading` based on American Heart Association (AHA) and WHO guidelines, perform `calculate_trend_analysis` on historical measurement data to detect rising or falling patterns, and use `evaluate_health_alert` to identify potential hypertensive crises or dangerous spikes in blood pressure.


## Available Tools (3)
- **evaluate_health_alert**: Identifies potential health alerts from current and historical data
- **classify_single_reading**: Classifies a single blood pressure measurement
- **calculate_trend_analysis**: Analyzes historical blood pressure readings for trends


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blood Pressure Classifier** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Classify a blood pressure reading of 145/92 mmHg."

**🤖 AI Agent:**
> A reading of 145/92 mmHg is classified as Stage 2 Hypertension.

---

**👤 You:**
> "Analyze these readings for trends: [{"systolic": 120, "diastolic": 80}, {"systolic": 125, "diastolic": 82}, {"systolic": 130, "diastolic": 85]."

**🤖 AI Agent:**
> The trend analysis shows a Rising pattern in your blood pressure readings.

---

**👤 You:**
> "Check if a systolic reading of 180/120 is an emergency."

**🤖 AI Agent:**
> ALERT: A reading of 180/120 mmHg indicates a Hypertensive Crisis. Please seek medical attention immediately.


## ❓ FAQ

**Q: What medical standards does this tool use?**
The server uses the American Heart Association (AHA) and World Health Organization (WHO) guidelines for classifying blood pressure readings.

**Q: How can I analyze my blood pressure history?**
You can use the `calculate_trend_analysis` tool by providing a JSON array of your previous systolic and diastolic readings to identify patterns like rising or falling pressure.

**Q: Does this tool provide emergency alerts?**
Yes, the `evaluate_health_alert` tool can identify if a current reading indicates a hypertensive crisis or a significant spike compared to your baseline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/blood-pressure-classifier](https://vinkius.com/mcp/blood-pressure-classifier)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blood Pressure Classifier** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blood-pressure-classifier` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blood Pressure Classifier** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blood-pressure-classifier": {
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
