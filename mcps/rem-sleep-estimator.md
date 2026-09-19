# REM Sleep Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rem-sleep-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Estimates REM sleep distribution, timing, and intensity throughout the night.

## Description
This MCP server provides biological sleep architecture modeling to estimate REM sleep patterns. Use `get_rem_schedule` to map out specific REM periods, `get_rem_summary` for aggregate metrics like REM percentage and debt, `get_dream_windows` to find high-intensity dreaming intervals, and `validate_sleep_parameters` to ensure sleep configurations are biologically plausible for a given age.


## Available Tools (4)
- **get_dream_windows**: Identifies time intervals most likely to feature intense dreaming
- **get_rem_schedule**: Determines the predicted timing and duration of each REM period throughout the night
- **get_rem_summary**: Calculates aggregate REM metrics for the entire sleep session
- **validate_sleep_parameters**: Validates if a sleep configuration is biologically plausible for the given age


## 💬 Prompt Examples

Here are some examples of how you can interact with the **REM Sleep Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you show me my REM sleep schedule for 8 hours of sleep starting at 11:00 PM for a 30-year-old?"

**🤖 AI Agent:**
> Your REM sleep periods are scheduled for 01:15 AM - 01:45 AM, 03:20 AM - 03:55 AM, and 06:10 AM - 07:00 AM.

---

**👤 You:**
> "What is my REM percentage and debt if I sleep for 6 hours at age 25?"

**🤖 AI Agent:**
> Your total REM duration is 90 minutes, resulting in a REM percentage of 25.0% and a REM debt indicator of 0.15.

---

**👤 You:**
> "Is it biologically plausible for a 70-year-old to sleep for 14 hours?"

**🤖 AI Agent:**
> Yes, a 14-hour sleep duration is considered plausible for a 70-year-old.


## ❓ FAQ

**Q: How accurate are these REM estimates?**
Estimates are based on biological sleep architecture models and age-related REM scaling principles.

**Q: What is REM debt?**
REM debt is the deficit between the predicted ideal REM sleep for your age and the actual REM sleep achieved.

**Q: Can I use this to find my best dreaming times?**
Yes, you can use `get_dream_windows` to identify specific time intervals most likely to feature intense dreaming.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rem-sleep-estimator](https://vinkius.com/en/ai-agent-connect/rem-sleep-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **REM Sleep Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rem-sleep-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **REM Sleep Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rem-sleep-estimator": {
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
