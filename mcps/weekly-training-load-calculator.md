# Weekly Training Load Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weekly-training-load-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Calculate physiological training stress using TRIMP and TSS methodologies to track athlete fatigue and fitness.

## Description
This MCP server provides specialized tools for athletes and coaches to quantify physical exertion. By connecting your AI agent to this service via Vinkius Edge, you can use `calculate_total_weekly_load` to compute cumulative training stress using TRIMP (based on heart rate) or TSS (based on intensity factor). You can also utilize `get_training_zone_distribution` to see how much load is accumulated in specific intensity zones like `ZONE_1_RECOVERY` or `ZONE_5_ANAEROBIC`. For long-term monitoring, `get_fitness_fatigue_metrics` calculates Acute Training Load (ATL) and Chronic Training Load (CTL), allowing you to monitor your training balance and prevent overtraining.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weekly Training Load Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total weekly load for these sessions using TRIMP: [{ 'duration': 60, 'averageHeartRate': 140, 'zone': 'ZONE_2_AEROBIC', 'date': '2024-07-01' }, { 'duration': 45, 'averageHeartRate': 165, 'zone': 'ZONE_4_THRESHOLD', 'date': '2024-07-03' }]"

**🤖 AI Agent:**
> The total weekly TRIMP load is 18,900.

---

**👤 You:**
> "What is the training zone distribution for these TSS sessions: [{ 'duration': 120, 'intensityFactor': 0.85, 'zone': 'ZONE_2_AEROBIC', 'date': '2024-07-01' }, { 'duration': 90, 'intensityFactor': 1.1, 'zone': 'ZONE_4_THRESHOLD', 'date': '2024-07-02' }]"

**🤖 AI Agent:**
> The distribution is: ZONE_2_AEROBIC: 86.7, ZONE_4_THRESHOLD: 108.9.

---

**👤 You:**
> "Check my fitness and fatigue metrics based on these sessions: [{ 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-07-05' }, { 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-07-04' }, { 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-07-03' }, { 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-07-02' }, { 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-07-01' }, { 'duration': 60, 'averageHeartRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-06-30' }, { 'duration': 60, 'averageHeartেরRate': 130, 'zone': 'ZONE_1_RECOVERY', 'date': '2024-06-29' }]"

**🤖 AI Agent:**
> Your acute load (ATL) is 780.0, your chronic load (CTL) is 780.0, and your training balance is 0.0.


## ❓ FAQ

**Q: What is the difference between TRIMP and TSS?**
TRIMP (Training Impulse) uses heart rate and duration to estimate physiological stress, while TSS (Training Stress Score) is used for power-based efforts using the intensity factor. Tools available: `your_tool_name`.

**Q: How can I track my fatigue levels?**
Use the `get_fitness_fatigue_metrics` tool. It calculates your ATL (acute fatigue) and CTL (long-term fitness) to show your training balance.

**Q: Does this tool support different intensity zones?**
Yes, it supports five standard zones: `ZONE_1_RECOVERY`, `ZONE_2_AEROBIC`, `ZONE_3_TEMPO`, `ZONE_4_THRESHOLD`, and `ZONE_5_ANAEROBIC`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weekly-training-load-calculator](https://vinkius.com/mcp/weekly-training-load-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weekly Training Load Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weekly-training-load-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weekly Training Load Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weekly-training-load-calculator": {
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
