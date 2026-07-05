# Fasting Streak Accumulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fasting-streak-accumulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Validate fasting logs, track success streaks, and calculate compliance percentages.

## Description
The Fasting Streak Accumulator is a specialized validation engine designed to assess fasting performance. By connecting your AI agent to this MCP server, you can precisely evaluate fasting logs against target durations. The server uses `check_fast_entry` to determine if individual fasts met their goals and identify any time deficits in minutes. Use `calculate_compliance_summary` to analyze entire datasets for current consecutive success streaks and overall compliance percentages. Additionally, `summarize_log_deficits` provides a detailed report of all failed attempts, highlighting exactly how much time was missed. This tool is perfect for health-focused AI agents managing intermittent fasting schedules.


## Available Tools (3)
- **summarize_log_deficits**: Generates a report of failed fasting attempts
- **calculate_compliance_summary**: Analyzes fasting logs for streaks and compliance
- **check_fast_entry**: Validates a single fasting event against its target


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fasting Streak Accumulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I fasted from 10:00 PM yesterday to 8:00 AM today. My target is 12 hours. Was I successful?"

**🤖 AI Agent:**
> Yes, your fast lasted 10 hours. Wait, checking... Actually, the duration was 10 hours, which is 2 hours short of your 12-hour target.

---

**👤 You:**
> "Check my compliance for these logs: [{date: '2023-10-01', startTime: '22:00', endTime: '08:00'}, {date: '2023-10-02', startTime: '20:00', endTime: '06:00'}] with a 12 hour target."

**🤖 AI Agent:**
> Your current streak is 2 days, and your total compliance percentage is 100%.

---

**👤 You:**
> "Show me a report of all my failed fasts from this week's logs."

**🤖 AI Agent:**
> The report shows 2 failed attempts: on 2023-10-05 you missed 45 minutes, and on 2023-10-07 you missed 120 minutes.


## ❓ FAQ

**Q: How does the tool handle overnight fasts?**
The `check_fast_entry` tool automatically accounts for periods that cross the midnight boundary, calculating the total elapsed duration accurately.

**Q: What information is needed to check a fasting entry?**
You need to provide the `targetFastHours` and a JSON string containing the date, start time, and end time of the log entry.

**Q: Can I see how many minutes I missed on a failed fast?**
Yes, the `summarize_log_deficits` tool generates a report specifically listing all failed attempts and the exact number of minutes missed for each.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fasting-streak-accumulator](https://vinkius.com/mcp/fasting-streak-accumulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fasting Streak Accumulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fasting-streak-accumulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fasting Streak Accumulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fasting-streak-accumulator": {
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
