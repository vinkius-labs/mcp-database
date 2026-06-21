# Circadian REM Sleep Cycle Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circadian-rem-sleep-cycle-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Harmonize your workflow with biological data. Calculate optimal wake-up times and bedtimes respecting 90-minute REM sleep phases for peak chronotype management.

## Description
Managing sleep debt requires biological precision. Artificial Intelligence models generally lack an understanding of human circadian rhythms, suggesting arbitrary '8 hours of sleep' that interrupt deep REM phases and cause morning grogginess. The Circadian REM Optimizer processes strict chronobiology rules natively.

### Core Value Add
- **REM Phase Harmonization:** Computes exact timestamps mapped to natural 90-minute sleep cycles (from 3 to 6 cycles), ensuring you always wake up during light sleep stages.
- **Latency Buffering Engine:** Standard sleep math ignores sleep latency. This MCP integrates an adjustable 'fall asleep' buffer (default 15 minutes) into the backward/forward timeline progression.
- **Bidirectional Architecture:** Supports both 'wake_up_at' (backward deduction) and 'sleep_at' (forward projection) modes to fit rigid alarm schedules or flexible weekend chronotypes.
- **Zero-Dependency Native Code:** The mathematical projection happens securely within the V8 engine, maintaining high-speed responsiveness for health-tech AI workflows.


## Available Tools
- **calculate_circadian_rhythm**: Maps out energy peaks and troughs throughout the day based on wake time
- **calculate_nap_times**: Requires wake-up time in HH:mm.

Calculates the ideal window for power naps based on wake-up time
- **calculate_sleep_cycles**: Provide a targetTimeStr (HH:mm) and the mode (sleep_at or wake_up_at).

Calculates optimal wake-up or bedtimes aligned with 90-minute REM sleep phases, incorporating latency buffers for circadian rhythm optimization
- **calculate_sleep_debt**: Requires daily required hours and an array of actually slept hours.

Calculates accumulated sleep debt and provides an actionable recovery strategy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian REM Sleep Cycle Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to wake up at 06:30 for work. What are the best times to go to sleep?"

**🤖 AI Agent:**
> Using the calculate_sleep_cycles tool (mode: wake_up_at): The optimal time to get into bed for 6 complete REM cycles is 21:15. For 5 cycles, aim for 22:45. Both times account for a 15-minute sleep latency buffer.

---

**👤 You:**
> "I am going to sleep right now at 23:00. When should I set my alarm?"

**🤖 AI Agent:**
> Using the calculate_sleep_cycles tool (mode: sleep_at): To align with optimal REM phases, you should set your alarm for 06:45 (5 cycles) or 08:15 (6 cycles).

---

**👤 You:**
> "Calculate a wake-up schedule for 05:00 assuming it takes me 30 minutes to fall asleep."

**🤖 AI Agent:**
> Using the calculate_sleep_cycles tool: The circadian engine confirms that for a 05:00 wake-up with a 30-minute latency, you must get into bed exactly at 21:00 for 5 complete REM cycles.


## ❓ FAQ

**Q: What is the 90-minute REM rule?**
Human sleep cycles last approximately 90 minutes. Waking up in the middle of a deep REM phase causes 'sleep inertia' (grogginess). This algorithm targets wake-up times strictly at the end of a cycle, meaning sleeping 7.5 hours (5 cycles) often feels more refreshing than sleeping 8 hours.

**Q: Why use an MCP for sleep math?**
Because calculating multiple backward chronobiological subtraction paths in base-60 time causes frequent LLM errors. By offloading it to this deterministic timeline engine, the calculations are mathematically flawless.

**Q: Does it account for the time it takes to fall asleep?**
Yes. The algorithm incorporates a 'fallAsleepBufferMinutes' parameter (which defaults to 15 minutes). If you need to wake up at 07:00, the 5-cycle target recommends getting into bed at 23:15, allowing exactly 15 minutes to fall asleep before the cycles commence.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circadian-rem-sleep-cycle-optimizer](https://vinkius.com/mcp/circadian-rem-sleep-cycle-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian REM Sleep Cycle Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `circadian-rem-sleep-cycle-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian REM Sleep Cycle Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-rem-sleep-cycle-optimizer": {
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
