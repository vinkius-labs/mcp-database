# Heart Rate Variability Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/heart-rate-variability-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Analyze physiological recovery and training readiness using HRV metrics.

## Description
This MCP server provides advanced physiological analysis by connecting AI agents to Heart Rate Variability (HRV) data. It allows agents to determine recovery status, calculate training readiness, and identify physiological trends. Using tools like `get_recovery_status` and `get_training_readiness`, agents can interpret RMSSD, SDNN, and RHR to provide actionable health insights. It also includes `process_raw_intervals` to convert raw RR interval data into usable metrics.


## Available Tools (4)
- **analyze_hrv_trend**: Identifies whether the user's physiological state is improving or declining over time
- **get_recovery_status**: Determines the current physiological recovery state
- **get_training_readiness**: Calculates how much training load an individual can safely absorb
- **process_raw_intervals**: Converts raw RR interval data into standard HRV metrics (RMSSD and SDNN)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heart Rate Variability Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "My RMSSD is 50ms, my RHR is 60 bpm, I am 30 years old, and my baseline RMSSD is 55ms. I took this measurement in the morning. What is my recovery status?"

**🤖 AI Agent:**
> Your current status is Recovered with a readiness score of 75. You should proceed with moderate intensity training.

---

**👤 You:**
> "Calculate HRV metrics from these RR intervals: [800, 810, 790, 820, 805, 795, 815, 800, 810, 790]"

**🤖 AI Agent:**
> The processed metrics are RMSSD: 12.5ms and SDNN: 10.2ms from 10 samples.

---

**👤 You:**
> "My recent RMSSD values are [45, 42, 40] and my baseline is 50. My recent RHR values are [60, 62, 65] and my baseline is 60. What is my trend?"

**🤖 AI Agent:**
> Your physiological state is Declining with a Strong trend, suggesting accumulating fatigue.


## ❓ FAQ

**Q: What metrics are required for recovery analysis?**
To use `get_recovery_status`, you need to provide the RMSSD value, resting heart rate (RHR), age, and the measurement type (overnight or morning).

**Q: Can I process raw heartbeat data?**
Yes, the `process_raw_intervals` tool converts a sequence of RR intervals into RMSSD and SDNN metrics.

**Q: How is training readiness determined?**
The `get_training_readiness` tool evaluates current RMSSD, SDNN, and RHR against your historical baselines to suggest an appropriate intensity level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/heart-rate-variability-analyzer](https://vinkius.com/en/ai-agent-connect/heart-rate-variability-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heart Rate Variability Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heart-rate-variability-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heart Rate Variability Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heart-rate-variability-analyzer": {
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
