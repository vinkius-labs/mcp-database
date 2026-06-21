# Lactate Threshold Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/lactate-threshold-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimate metabolic lactate thresholds using effort-based metrics or heart rate drift analysis.

## Description
The Lactate Threshold Estimator provides a non-invasive way to identify your physiological limits without laboratory testing. Using the `estimate_mlss` tool, you can calculate threshold parameters based on a sustainable one-hour effort (MLSS). Alternatively, use `detect_hr_drift` to find the metabolic threshold point from time-series heart rate and workload data by identifying cardiovascular decoupling. Once your threshold is identified, use `generate_zones` to produce five specific training zones (from recovery to anaerobic) recalibrated to your current fitness level and athlete classification.


## Available Tools
- **detect_hr_drift**: Detect the HR drift threshold from time-series data
- **estimate_mlss**: Estimate MLSS parameters based on a sustainable effort
- **generate_zones**: Generate training zones based on a discovered threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Lactate Threshold Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I held a pace of 4:30 min/km for 60 minutes and my VO2max is 50. What is my threshold?"

**🤖 AI Agent:**
> Based on your 60-minute effort, your estimated threshold pace is approximately 4:30 min/km, representing a specific intensity percentage of your 50 ml/kg/min VO2max.

---

**👤 You:**
> "Generate training zones for an advanced athlete with a threshold heart rate of 160 bpm."

**🤖 AI Agent:**
> Your recalibrated training zones are: Zone 1 (Recovery): 128-136 bpm; Zone 2 (Aerobic Base): 137-144 bpm; Zone 3 (Tempo): 145-151 bpm; Zone 4 (Threshold): 152-156 bpm; Zone 5 (Anaerobic): 157-160 bpm.

---

**👤 You:**
> "Analyze this heart rate data for drift: HR [140, 142, 145], Workload [200, 200, 200], Time [0, 60, 120]."

**🤖 AI Agent:**
> The analysis identified a threshold heart rate of approximately 145 bpm at the point where workload stability and heart rate decoupling were detected.


## ❓ FAQ

**Q: How does the MLSS estimation work?**
The `estimate_mlss` tool uses a sustainable effort (like a pace or power you can hold for about an hour) to calculate your threshold intensity, pace, and power relative to your VO2max.

**Q: What is required for HR drift detection?**
To use `detect_hr_drift`, you need sequential arrays of heart rate, workload (power or pace), and elapsed time in seconds recorded during a steady-state exercise session.

**Q: Can I update my training zones automatically?**
Yes. After identifying a threshold via MLSS or drift, you can use `generate_zones` to recalculate five specific intensity ranges based on your athlete level (Beginner, Intermediate, or Advanced).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lactate-threshold-estimator](https://vinkius.com/mcp/lactate-threshold-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Lactate Threshold Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `lactate-threshold-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Lactate Threshold Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "lactate-threshold-estimator": {
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
