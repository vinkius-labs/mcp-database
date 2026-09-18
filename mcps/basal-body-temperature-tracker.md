# Basal Body Temperature Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/basal-body-temperature-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Analyze menstrual cycle phases and ovulation using BBT data.

## Description
This MCP server provides specialized tools for fertility awareness by analyzing basal body temperature (BBT) fluctuations. It connects AI agents to your temperature data to identify thermal shifts, determine if you are in the follicular or luteal phase, and pinpoint ovulation events. Use `analyze_cycle_phase` to check your current cycle stage, `detect_ovulation_event` to find your ovulation day, `estimate_fertile_window` to predict fertile days, and `calculate_cycle_metrics` for a full summary of your cycle length and phase durations.


## Available Tools (4)
- **analyze_cycle_phase**: Determines the current phase of the user's menstrual cycle based on recent temperature data
- **calculate_cycle_metrics**: Provides high-level summaries of cycle length and phase duration
- **detect_ovulation_event**: Pinpoints the specific day ovulation likely occurred
- **estimate_fertile_window**: Predicts the days when the user is most likely to be fertile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basal Body Temperature Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Based on these readings: [{'temperature': 36.2, 'cycle_day': 1}, {'temperature': 36.1, 'cycle_day': 2}, {'temperature': 36.5, 'cycle_day': 3}], what phase am I in?"

**🤖 AI Agent:**
> You are currently in the follicular phase.

---

**👤 You:**
> "When was my ovulation based on these readings: [{'temperature': 36.2, 'cycle_day': 1}, {'temperature': 36.2, 'cycle_day': 2}, {'temperature': 36.6, 'cycle_day': 3}, {'temperature': 36.7, 'cycle_day': 4}, {'temperature': 36.7, 'cycle_day': 5}]?"

**🤖 AI Agent:**
> Ovulation likely occurred on cycle day 2.

---

**👤 You:**
> "Can you estimate my fertile window using these readings: [{'temperature': 36.1, 'cycle_day': 1}, {'temperature': 36.1, 'cycle_day': 2}, {'temperature': 36.5, 'cycle_day': 3}]?"

**🤖 AI Agent:**
> Your fertile window is estimated to be between cycle day 1 and cycle day 3.


## ❓ FAQ

**Q: How do I use this tool?**
Provide your BBT readings as an array of temperature and cycle day objects. The tools will then process this data to provide insights like ovulation detection or phase analysis.

**Q: What is a thermal shift?**
A thermal shift is a sustained rise in basal body temperature that indicates ovulation has occurred, which `detect_ovulation_event` identifies.

**Q: Can I get a summary of my cycle?**
Yes, you can use `calculate_cycle_metrics` to get an estimate of your total cycle length and the duration of your follicular and luteal phases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/basal-body-temperature-tracker](https://vinkius.com/en/ai-agent-connect/basal-body-temperature-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Basal Body Temperature Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `basal-body-temperature-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Basal Body Temperature Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "basal-body-temperature-tracker": {
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
