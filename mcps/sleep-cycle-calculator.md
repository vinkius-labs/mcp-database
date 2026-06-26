# Sleep Cycle Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sleep-cycle-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimize your rest by finding the perfect wake-up times based on natural 90-minute sleep cycles.

## Description
The Sleep Cycle Calculator helps you align your sleep schedule with your body's biological rhythms. By calculating wake-up windows based on 90-minute cycles and accounting for a 15-minute sleep latency, this tool ensures you wake up at the end of a cycle to minimize grogginess. Use `calculate_wake_times` to find when to wake up after a planned bedtime, `calculate_bedtimes` to plan your night around a required wakeup time, or `assess_sleep_window` to check if your sleep duration falls into optimal or insufficient categories.


## Available Tools (3)
- **calculate_bedtimes**: Calculate ideal bedtimes based on a wakeup time
- **calculate_wake_times**: Calculate ideal wake up times based on a bedtime
- **assess_sleep_window**: Assess if a sleep duration is optimal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sleep Cycle Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I want to go to sleep at 23:00. When should I wake up?"

**🤖 AI Agent:**
> Based on a 23:00 bedtime, your ideal wake-up times are 00:45, 02:15, 03:45, 05:15, and 06:45.

---

**👤 You:**
> "I need to wake up at 07:00. What time should I go to bed?"

**🤖 AI Agent:**
> To wake up at 07:00, you should aim to fall asleep at 23:15, 01:45, or 04:15.

---

**👤 You:**
> "Is 420 minutes of sleep enough?"

**🤖 AI Agent:**
> A duration of 420 minutes is classified as Optimal for your sleep window.


## ❓ FAQ

**Q: How does the calculator determine wake-up times?**
The tool adds a 15-minute sleep latency to your bedtime and then calculates subsequent 90-minute intervals to suggest the best moments to wake up.

**Q: Can I check if my current sleep duration is healthy?**
Yes, you can use the `assess_sleep_window` tool by providing your total minutes of sleep to see if it falls into optimal, insufficient, or excessive categories.

**Q: What format should I use for times?**
Please use the 24-hour notation (HH:mm), such as '23:00' or '07:30', for all time-related inputs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sleep-cycle-calculator](https://vinkius.com/mcp/sleep-cycle-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sleep Cycle Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sleep-cycle-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sleep Cycle Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sleep-cycle-calculator": {
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
