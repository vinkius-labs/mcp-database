# Circadian Rhythm Aligner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/circadian-rhythm-aligner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Gradual sleep and wake time adjustment planner.

## Description
The Circadian Rhythm Aligner helps you transition to a new sleep schedule without the shock of sudden changes. By using tools like `calculate_adjustment_plan`, it generates a day-by-day schedule that shifts your bedtime and wake time by small, manageable increments (15 or 30 minutes). You can also use `analyze_sleep_window_integrity` to ensure your new schedule maintains healthy sleep durations and `calculate_drift_magnitude` to understand the total temporal shift required for your transition.

### Available Tools

`your_tool_name`




## 💬 Prompt Examples

Here are some examples of how you can interact with the **Circadian Rhythm Aligner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I currently sleep at 12:00 AM and wake up at 8:00 AM. I want to move my schedule to 11:00 PM and 7:00 AM using 30-minute increments. Can you make a plan?"

**🤖 AI Agent:**
> To transition from your current schedule to 11:00 PM/7:00 AM, it will take 2 days. Day 1: Sleep at 11:30 PM, Wake at 7:30 AM. Day 2: Sleep at 11:00 PM, Wake at 7:00 AM.

---

**👤 You:**
> "Is a sleep window from 1:00 AM to 6:30 AM healthy if my minimum requirement is 7 hours?"

**🤖 AI Agent:**
> No, that schedule provides only 5.5 hours of sleep, which falls below your 7-hour threshold and poses a risk of sleep deprivation.

---

**👤 You:**
> "How many minutes do I need to shift from 10:00 PM to 12:30 AM?"

**🤖 AI Agent:**
> The total drift magnitude required for this transition is 150 minutes.


## ❓ FAQ

**Q: How does the adjustment plan work?**
The `calculate_adjustment_plan` tool creates a daily schedule that incrementally shifts your sleep and wake times by 15 or 30 minutes until you reach your target routine, minimizing biological disruption. Tools available: `your_tool_name`.

**Q: Can I check if my new schedule is healthy?**
Yes, you can use the `analyze_sleep_window_integrity` tool to evaluate your scheduled sleep duration and ensure it meets a minimum threshold of healthy hours.

**Q: How much drift is required for my change?**
You can use `calculate_drift_magnitude` to find the total number of minutes your biological clock needs to migrate from your current time to your target time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/circadian-rhythm-aligner](https://vinkius.com/mcp/circadian-rhythm-aligner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Circadian Rhythm Aligner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `circadian-rhythm-aligner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Circadian Rhythm Aligner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "circadian-rhythm-aligner": {
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
