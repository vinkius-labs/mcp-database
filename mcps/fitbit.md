# Fitbit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fitbit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access Fitbit health data via AI — query activities, sleep, heart rate, SpO2, body weight, and nutrition logs in natural conversation.

## Description
Connect your **Fitbit** account to any AI agent and gain instant access to your comprehensive health and fitness data through natural conversation.

### What you can do

- **Activity Tracking** — Retrieve daily activity summaries including steps, distance, calories, and active minutes for any date
- **Sleep Analysis** — Access detailed sleep logs with stages (deep, light, REM, awake) for individual nights or time series trends
- **Heart Rate Monitoring** — Query resting heart rate, intraday zones, and historical cardiac trends
- **SpO2 & Breathing** — View blood oxygen saturation levels and breathing rate data
- **Body Composition** — Track weight measurements and cardio fitness scores over time
- **Nutrition Logs** — Access water intake and food logging data for dietary tracking
- **Device Management** — Check connected Fitbit devices and their sync status

### How it works

1. Subscribe to this server
2. Generate an OAuth2 access token from your Fitbit Developer Portal
3. Start querying your health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health Enthusiasts** — analyze trends in sleep quality, heart rate variability, and activity levels naturally
- **Healthcare Professionals** — access patient wearable data summaries for informed consultations
- **Developers** — build health-aware AI agents that can reason about biometric data


## Available Tools (14)
- **get_activities_date**: Returns steps, calories burned, distance walked, active minutes, floors climbed, elevation and sedentary minutes. Date format: YYYY-MM-DD or "today".

Get activity summary for a specific date
- **get_activities_timeseries**: Resource paths: "steps", "calories", "distance", "floors", "elevation", "minutesSedentary", "minutesLightlyActive", "minutesFairlyActive", "minutesVeryActive", "activityCalories". Period: 1d, 7d, 30d, 1w, 1m, 3m, 6m, 1y, max or startDate/endDate (YYYY-MM-DD). Detail level: "1min", "5min", "15min", "1day" for intraday data.

Get activity time series data over a date range
- **get_body_weight**: Returns weight in kg, BMI, fat percentage and date logged. Date format: YYYY-MM-DD.

Get body weight log entries for a specific date
- **get_breathing_rate**: Returns breathing rate in breaths per minute. Available on Fitbit devices with SpO2 sensors. Date format: YYYY-MM-DD.

Get breathing rate for a specific date
- **get_cardio_fitness_score**: Returns VO2 Max values and percentile rankings. Date format: YYYY-MM-DD.

Get cardio fitness score (VO2 Max) for a date range
- **get_devices**: Returns device version, MAC address, battery level, last sync time and device type.

Get all Fitbit devices connected to the user's account
- **get_foods_date**: Returns total calories consumed, macros (carbs, protein, fat), water intake and list of logged foods with meal times. Date format: YYYY-MM-DD or "today".

Get food log summary for a specific date
- **get_heart_date**: Returns resting heart rate, heart rate zones (fat burn, cardio, peak, out of range) and calories burned in each zone. Date format: YYYY-MM-DD or "today".

Get heart rate summary for a specific date
- **get_heart_timeseries**: Returns resting heart rate and heart rate zones per day. Detail level: "1min", "5min", "15min", "1day" for intraday BPM data.

Get heart rate time series data over a date range
- **get_profile**: Returns display name, full name, age, height, weight, gender, locale, timezone, avatar URL and member since date.

Get the authenticated user's Fitbit profile
- **get_sleep_date**: Returns sleep start time, duration, minutes asleep, minutes awake, minutes in each sleep stage (light, deep, REM, awake), efficiency score and number of awakenings. Date format: YYYY-MM-DD or "today".

Get sleep log for a specific date
- **get_sleep_timeseries**: Returns daily sleep summaries with start time, duration, minutes asleep, efficiency and sleep stages. Date range format: startDate/endDate (YYYY-MM-DD).

Get sleep log over a date range
- **get_spo2**: Returns average SpO2 percentage and min/max values. Available on Fitbit devices with SpO2 sensors. Date format: YYYY-MM-DD.

Get blood oxygen saturation (SpO2) for a specific date
- **get_water**: Returns water consumption in milliliters and timestamps. Date format: YYYY-MM-DD.

Get water intake log for a specific date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fitbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How did I sleep last night?"

**🤖 AI Agent:**
> You slept 7h 23m total. Deep sleep: 1h 45m (24%), Light: 3h 52m (53%), REM: 1h 20m (18%), Awake: 26m. Your sleep score was 82/100 — above your weekly average of 76.

---

**👤 You:**
> "Show my heart rate trends for the past week."

**🤖 AI Agent:**
> Your average resting heart rate this week was 62 bpm, down from 65 bpm last week. Peak zone time increased to 45 minutes total across 3 workout sessions. Cardio fitness score: 42 (Good).


## ❓ FAQ

**Q: Can I query sleep data for a specific date range?**
Yes! Use the sleep time series tool to query sleep trends across any date range. You can also inspect a single night in detail with the sleep date tool, including all sleep stages.

**Q: What health metrics can I access?**
You can access 14 different health metrics: activities, sleep (date & time series), heart rate (date & time series), SpO2, breathing rate, cardio fitness score, body weight, water intake, food logs, device info, and user profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fitbit](https://vinkius.com/mcp/fitbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fitbit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fitbit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fitbit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fitbit": {
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
