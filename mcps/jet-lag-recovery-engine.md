# Jet Lag Recovery Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/jet-lag-recovery-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A deterministic scheduling engine for personalized jet lag recovery plans.

## Description
This MCP server provides precise, deterministic scheduling to help travelers overcome jet lag. It calculates full recovery timelines, generates daily light exposure schedules to manage circadian rhythms, provides melatonin timing, and creates incremental sleep shift plans. Use `get_recovery_estimate` to find your recovery duration, `get_light_exposure_schedule` to manage light exposure, `get_melatonin_schedule` for supplement timing, and `get_sleep_shift_plan` to adjust your sleep cycle.


## Available Tools (4)
- **get_light_exposure_schedule**: Provides a specific daily schedule of when the user should seek or avoid light
- **get_melatonin_schedule**: Provides the timing for melatonin supplementation to assist with sleep onset
- **get_recovery_estimate**: Calculates the total number of days required for the traveler to achieve full circadian recovery
- **get_sleep_shift_plan**: Generates a daily schedule for adjusting sleep times to match the destination's rhythm


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jet Lag Recovery Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take me to recover if I am 35 years old, traveling east across 5 time zones?"

**🤖 AI Agent:**
> It will take approximately 5 days to achieve full recovery.

---

**👤 You:**
> "Give me a light exposure schedule for traveling west across 3 time zones, arriving in Tokyo on 2024-10-15T10:00:00."

**🤖 AI Agent:**
> To adjust westward, you should seek light in the local evening and avoid light during the local morning.

---

**👤 You:**
> "When should I take melatonin if my target bedtime is 22:00 and I need 3 days of recovery?"

**🤖 AI Agent:**
> You should take melatonin at 21:30 for the next 3 days.


## ❓ FAQ

**Q: How does the recovery estimate work?**
The `get_recovery_estimate` tool calculates recovery days based on your direction of travel, the number of time zones crossed, and your age.

**Q: Can I use this to manage my light exposure?**
Yes, the `get_light_exposure_schedule` tool provides specific instructions on when to seek or avoid light to help your body adjust.

**Q: Does it provide melatonin advice?**
Yes, `get_melatonin_schedule` provides the optimal timing for melatonin supplementation relative to your target bedtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/jet-lag-recovery-engine](https://vinkius.com/ai-agent-connect/jet-lag-recovery-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jet Lag Recovery Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jet-lag-recovery-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jet Lag Recovery Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jet-lag-recovery-engine": {
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
