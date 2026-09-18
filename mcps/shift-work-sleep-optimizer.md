# Shift Work Sleep Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shift-work-sleep-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize sleep, light exposure, and caffeine timing for shift workers.

## Description
This MCP server provides specialized tools to manage circadian rhythms for shift workers. It uses biological principles to calculate optimal sleep windows via `calculate_sleep_schedule`, manage alertness through `optimize_light_exposure`, determine safe caffeine windows with `generate_caffeine_protocol`, and manage sleep debt using `plan_napping_strategy`.


## Available Tools (4)
- **calculate_sleep_schedule**: Provides the primary window of time when the user should attempt to sleep to maximize rest and minimize circadian misalignment
- **generate_caffeine_protocol**: Determines the safe window for caffeine consumption to ensure it does not interfere with the planned sleep windows
- **optimize_light_exposure**: Tells the user exactly when to seek bright light to stay alert and when to avoid light to prepare for sleep
- **plan_napping_strategy**: Recommends specific nap timings to manage sleep pressure during or around shifts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shift Work Sleep Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I work a night shift from 10 PM to 6 AM and have a 30 minute commute. I prefer split sleep. When should I sleep?"

**🤖 AI Agent:**
> Your optimal sleep windows are from 7:30 AM to 11:30 AM and a secondary nap from 4:00 PM to 4:30 PM.

---

**👤 You:**
> "When should I stop drinking coffee if my shift ends at 6 AM and I want to sleep by 7:30 AM?"

**🤖 AI Agent:**
> You should stop all caffeine consumption by 12:00 AM to ensure it is cleared from your system before your 7:30 AM sleep time.

---

**👤 You:**
> "I'm on a rotating shift starting at 8 PM. When should I use bright light?"

**🤖 AI Agent:**
> You should seek bright light between 7:00 PM and 10:00 PM to boost alertness for your shift.


## ❓ FAQ

**Q: How does this help with rotating shifts?**
The `calculate_sleep_schedule` tool provides more conservative windows for rotating shifts to account for higher circadian misalignment.

**Q: Can I use this to manage my caffeine intake?**
Yes, `generate_caffeine_protocol` calculates a safe cutoff time to ensure caffeine does not interfere with your planned sleep.

**Q: Does it recommend when to use light?**
Yes, `optimize_light_exposure` tells you exactly when to seek bright light for alertness and when to avoid it to protect melatonin.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shift-work-sleep-optimizer](https://vinkius.com/en/ai-agent-connect/shift-work-sleep-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shift Work Sleep Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shift-work-sleep-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shift Work Sleep Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shift-work-sleep-optimizer": {
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
