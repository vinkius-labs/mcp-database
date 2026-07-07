# Rest Timer Accumulator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rest-timer-accumulator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate total workout duration including rest periods.

## Description
The Rest Timer Accumulator is a specialized utility designed to help you track the true time commitment of your training sessions. By aggregating active work time, intra-set rest periods, and inter-exercise transitions, it provides an accurate total duration for any workout plan. Use `calculate_total_duration` to compute the total elapsed seconds, `format_time_display` to convert raw seconds into a readable HH:MM:SS format, and `verify_workout_integrity` to ensure your exercise parameters are logically sound.


## Available Tools (3)
- **calculate_total_duration**: Calculates the total workout duration in seconds
- **format_time_display**: Converts seconds into HH:MM:SS format
- **verify_workout_integrity**: Validates the workout plan integrity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rest Timer Accumulator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total duration for a workout with 2 exercises: 3 sets of squats (60s each) and 2 sets of lunges (45s each), with 30s rest between sets and 60s rest between exercises."

**🤖 AI Agent:**
> The total workout duration is 00:05:15, with an active work time of 00:03:30.

---

**👤 You:**
> "Convert 3665 seconds into a readable format."

**🤖 AI Agent:**
> 01:01:05

---

**👤 You:**
> "Check if my workout plan is valid: 1 set of pushups with -10s duration."

**🤖 AI Agent:**
> The workout plan is invalid. Error: duration cannot be negative.


## ❓ FAQ

**Q: How does the duration calculation work?**
The `calculate_total_duration` tool iterates through each exercise, summing the time for every set and adding the rest period between sets. It also adds the transition rest duration when moving from one exercise to the next.

**Q: Can I validate my workout plan before calculating?**
Yes, you can use the `verify_workout_integrity` tool to check for errors such as negative durations or missing properties in your exercise list.

**Q: What format is the time output in?**
The `format_time_display` tool converts any number of seconds into a standardized HH:MM:SS string, ensuring all units are properly padded with leading zeros.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rest-timer-accumulator](https://vinkius.com/mcp/rest-timer-accumulator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rest Timer Accumulator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rest-timer-accumulator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rest Timer Accumulator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rest-timer-accumulator": {
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
