# Withings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/withings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Access comprehensive health and fitness data — track weight, blood pressure, sleep cycles, steps, workouts, and heart rate directly from Withings devices.

## Description
Connect your **Withings** account to any AI agent to unlock deep insights into your health, wellness, and fitness data collected by Withings smart scales, watches, and medical devices.

### What you can do

- **Medical Measurements** — Track weight, body fat %, systolic/diastolic blood pressure, and heart pulse trends over time
- **Sleep Analytics** — Access daily sleep scores, deep/light/REM sleep stage durations, and sleep efficiency metrics
- **Activity Tracking** — Analyze daily step counts, active calories burned, and precise intraday activity levels
- **Workout Logging** — Review distinct workout sessions (running, swimming, cycling) with categorizations and duration
- **Device Management** — Check the battery status and connection status of your Withings hardware fleet
- **Real-time Notifications** — Configure webhooks to receive instant alerts when new measurements (like a morning weigh-in) are recorded

### How it works

1. Subscribe to this server
2. Navigate to the [Withings Developer Portal](https://developer.withings.com/) and register an app to get an OAuth Access Token
3. Start querying your physiological data directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Quantified Self Enthusiasts** — use AI to correlate health metrics (e.g., how late workouts affect sleep scores)
- **Health Tech Developers** — prototype integrations with connected medical hardware
- **Personal Trainers & Coaches** — programmatically review client compliance with activity and weight goals
- **Medical Researchers** — analyze physiological trends and adherence across study participants


## Available Tools
- **get_activity**: Get daily activity summaries (steps, calories)
- **get_heart_rate**: Get specific heart rate measurements
- **get_intraday_activity**: Get high-frequency intraday activity data
- **get_measurements**: Use meastype to filter (1=Weight, 4=Height, 9=Diastolic BP, 10=Systolic BP, 11=Heart Pulse, 71=Body Temp). Dates should be YYYY-MM-DD.

Get physiological measurements (weight, blood pressure, etc)
- **get_sleep_details**: Get detailed sleep data (stages and states)
- **get_sleep_summary**: Get daily sleep summaries
- **get_user_devices**: List user's Withings devices
- **get_user_goals**: Get user health and fitness goals
- **get_workouts**: g., running, swimming, cycling) with their specific duration, calorie burn, distance, and activity category.

Get recorded workouts and exercises
- **subscribe_notifications**: g. immediately after a user steps on a scale). Appli codes: 1(weight), 4(BP), 16(activity), 44(sleep).

Subscribe to Withings webhook notifications


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Withings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Retrieve my weight and body fat measurements for the last 30 days."

**🤖 AI Agent:**
> I've retrieved your measurements. Your weight started at 82.5kg 30 days ago and is currently 81.2kg. Your body fat mass trended down from 19.4% to 18.8%.

---

**👤 You:**
> "What was my sleep score and total sleep time last night?"

**🤖 AI Agent:**
> Last night you slept for a total of 7 hours and 12 minutes, achieving a Sleep Score of 88 (Good). You fell asleep in just 8 minutes but woke up 3 times during the night.

---

**👤 You:**
> "Analyze my activity levels over the weekend. Did I hit my step goals?"

**🤖 AI Agent:**
> Looking at your activity data: On Saturday you took 12,450 steps and burned 2,400 calories (Goal met!). On Sunday, you took 6,200 steps and logged a 45-minute Cycling workout burning 450 calories, keeping your activity high despite lower steps.


## ❓ FAQ

**Q: How do I filter for specific measurements like Body Fat or Blood Pressure?**
Use the `meastype` parameter with the `get_measurements` tool. Common types: 1 (Weight), 4 (Height), 8 (Fat Mass), 9 (Diastolic BP), 10 (Systolic BP), 11 (Heart Pulse), 71 (Body Temperature).

**Q: What is the difference between sleep summary and sleep details?**
`get_sleep_summary` returns one overall score and total duration per night. `get_sleep_details` returns high-frequency intraday data, detailing exactly what time you entered REM, deep sleep, or woke up throughout the night.

**Q: Can I receive real-time notifications when I step on the scale?**
Yes, use the `subscribe_notifications` tool with an `appli` ID of 1 (Weight). Withings will then send a POST webhook to the callback URL you specify the moment a new weight measurement is synced.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/withings](https://vinkius.com/mcp/withings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Withings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `withings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Withings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "withings": {
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
