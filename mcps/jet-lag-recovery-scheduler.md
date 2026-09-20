# Jet Lag Recovery Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/jet-lag-recovery-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates personalized circadian recovery protocols including light, melatonin, and sleep schedules.

## Description
This MCP server provides specialized tools to help travelers synchronize their biological clocks with new time zones. By analyzing travel direction and time zone offsets, it generates precise recovery plans. Use `get_adaptation_timeline` to estimate recovery duration, `get_light_exposure_schedule` to find optimal light windows, `get_melatonin_timing_plan` for dosing schedules, and `get_sleep_schedule` for daily routines.


## Available Tools (4)
- **get_adaptation_timeline**: Determines how long it will take for the user to fully recover from jet lag
- **get_light_exposure_schedule**: Provides a specific plan for when the user should seek bright light to facilitate clock adjustment
- **get_melatonin_timing_plan**: Schedules the optimal times to take melatonin to assist in shifting the circadian rhythm
- **get_sleep_schedule**: Provides a daily sleep/wake routine to help the user align with the destination's local time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jet Lag Recovery Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I am traveling from New York (UTC-5) to London (UTC+0) heading east for a 5-day trip. How long will it take to recover?"

**🤖 AI Agent:**
> It will take approximately 3 days to reach full circadian synchrony with London time.

---

**👤 You:**
> "Give me a light exposure plan for traveling west from Los Angeles (UTC-8) to Tokyo (UTC+9)."

**🤖 AI Agent:**
> To adjust to Tokyo time, you should seek bright light during the late afternoon and evening of your arrival days to delay your biological clock.

---

**👤 You:**
> "When should I take melatonin for a trip from Berlin (UTC+1) to New York (UTC-5) traveling west?"

**🤖 AI Agent:**
> You should take melatonin in the late evening local time of your destination to help signal the biological night and facilitate sleep onset.


## ❓ FAQ

**Q: How accurate are the recovery timelines?**
The timelines are calculated using circadian phase shift models based on your specific travel direction and time zone offsets.

**Q: Can I use this for short trips?**
Yes, the `get_sleep_schedule` tool accounts for your `lengthOfStayDays` to provide relevant advice for both short and long trips.

**Q: Does this provide medical advice?**
No, this tool provides scheduling suggestions based on biological models. Always consult a medical professional before starting new supplement routines.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/jet-lag-recovery-scheduler](https://vinkius.com/en/ai-agent-connect/jet-lag-recovery-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jet Lag Recovery Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jet-lag-recovery-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jet Lag Recovery Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jet-lag-recovery-scheduler": {
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
