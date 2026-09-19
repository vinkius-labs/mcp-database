# Blue Light Exposure Timer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/blue-light-exposure-timer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize sleep quality by calculating ideal light exposure and screen cutoff times.

## Description
This MCP server helps you manage your circadian rhythm by calculating optimal light exposure windows. Use `get_sleep_schedule_recommendations` to find your ideal screen cutoff time and evening light guidance. You can also use `get_exposure_risk_assessment` to evaluate melatonin suppression risks, `get_morning_alertness_plan` to anchor your morning alertness, and `get_filter_requirements` to determine if you need software or hardware blue light mitigations.


## Available Tools (4)
- **get_exposure_risk_assessment**: Evaluates the physiological risk of sleep disruption based on specific device usage behavior
- **get_filter_requirements**: Determines if technical mitigations (software/hardware) are required
- **get_morning_alertness_plan**: Creates a plan to optimize morning alertness and circadian anchoring
- **get_sleep_schedule_recommendations**: Provides a complete schedule of light-related activities based on a user's sleep goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Blue Light Exposure Timer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to bed at 22:30 and wake up at 06:30. I use my phone with medium brightness. What is my light schedule?"

**🤖 AI Agent:**
> Your screen cutoff time is 21:00. For the evening, use dim warm lights only. Your morning light window is from 06:30 to 07:30, and you should use natural sunlight if possible.

---

**👤 You:**
> "I use my laptop at high brightness just 30 minutes before my 23:00 bedtime. What is my risk?"

**🤖 AI Agent:**
> Your melatonin suppression risk is high, and you may experience significant sleep onset delay. It is highly recommended to use blue light blocking glasses.

---

**👤 You:**
> "I wake up at 07:00 and don't have access to the outdoors. How can I stay alert?"

**🤖 AI Agent:**
> Your optimal light window is from 07:00 to 07:45. Since you lack outdoor access, a High-LUX Light Box is the recommended light source.


## ❓ FAQ

**Q: How does this tool help my sleep?**
It calculates specific times to avoid blue light and when to seek morning light to ensure your melatonin production is not suppressed.

**Q: Can I use this to plan my morning routine?**
Yes, by using `get_morning_alertness_plan`, you can receive a specific window for light exposure to help you wake up feeling alert.

**Q: What if I use high-brightness screens at night?**
You can use `get_exposure_risk_assessment` to see how much your device usage might delay your sleep onset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/blue-light-exposure-timer](https://vinkius.com/en/ai-agent-connect/blue-light-exposure-timer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Blue Light Exposure Timer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `blue-light-exposure-timer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Blue Light Exposure Timer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "blue-light-exposure-timer": {
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
