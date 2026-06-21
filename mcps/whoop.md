# WHOOP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/whoop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track your WHOOP health metrics — workouts, sleep, recovery, strain, HRV and body measurements from any AI agent.

## Description
Connect your **WHOOP** account to any AI agent and access your personal health data through natural conversation.

### What you can do

- **Profile** — View your WHOOP profile and body measurements (height, weight, max HR)
- **Cycles** — Browse your 24-hour WHOOP cycles combining sleep, strain and recovery
- **Sleep** — Analyze sleep data with stages (light, deep, REM), duration and performance
- **Recovery** — Track recovery scores, HRV, resting heart rate and sleep balance
- **Workouts** — Review workout data with strain, heart rate zones, duration and calories
- **Pagination** — Navigate through historical data with date ranges and pagination tokens

### How it works

1. Subscribe to this server
2. Enter your WHOOP Client ID, Client Secret and Access Token
3. Start exploring your health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Athletes** — review workout strain, recovery scores and sleep quality to optimize training
- **Health Enthusiasts** — track daily recovery, HRV trends and sleep patterns over time
- **Coaches** — monitor athlete workload, recovery status and sleep data remotely


## Available Tools
- **get_body_measurement**: Useful for tracking physical metrics alongside your WHOOP data.

Get your body measurement data
- **get_cycle**: Includes sleep, recovery, strain and heart rate metrics for that 24-hour period.

Get a specific WHOOP cycle by ID
- **get_cycle_recovery**: Includes recovery score, resting heart rate, HRV (heart rate variability), sleep balance and strain balance.

Get recovery data for a specific WHOOP cycle
- **get_cycle_sleep**: Includes sleep duration, stages (light, deep, REM, awake), disturbances and sleep performance percentage.

Get sleep data for a specific WHOOP cycle
- **get_cycles**: Cycles represent 24-hour periods of recovery and strain data. Each cycle includes sleep, recovery, strain and heart rate metrics. Supports date range filtering with start/end in ISO 8601 format. Pagination: max 25 results, use nextToken for more.

Get your WHOOP cycle data
- **get_profile**: Use this to verify your authentication is working and get your user ID for other endpoints.

Get your WHOOP profile info
- **get_recovery**: Supports date range filtering. Pagination: max 25 results per request.

Get your WHOOP recovery data
- **get_sleep**: Supports date range filtering. Pagination: max 25 results.

Get your WHOOP sleep data
- **get_sleep_by_id**: Includes full sleep stages, disturbances, respiratory rate and sleep performance.

Get a specific WHOOP sleep record by ID
- **get_workout**: Includes strain score, duration, heart rate zones, calories burned and GPS data if available.

Get a specific WHOOP workout by ID
- **get_workouts**: Supports date range filtering. Pagination: max 25 results.

Get your WHOOP workout data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WHOOP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recovery score from today."

**🤖 AI Agent:**
> Today's recovery: 78% (Good). Resting HR: 52 bpm, HRV: 68ms, sleep balance: 8h 12m. You're well recovered and ready for high strain today.

---

**👤 You:**
> "How did I sleep last night?"

**🤖 AI Agent:**
> Last night's sleep: 7h 45m total. Sleep performance: 85%. Light sleep: 3h 20m, Deep sleep: 2h 10m, REM: 1h 45m, Awake: 30m. Respiratory rate: 14 breaths/min. 2 disturbances.

---

**👤 You:**
> "Show me my workouts from this week."

**🤖 AI Agent:**
> This week's workouts: 1. Running (45min, strain 14.2, avg HR 152, 520 cal) — 2. Weight Training (60min, strain 12.8, avg HR 138, 410 cal) — 3. Cycling (30min, strain 10.5, avg HR 145, 350 cal). Total weekly strain: 37.5.


## ❓ FAQ

**Q: How do I get WHOOP API credentials?**
Visit [**developer.whoop.com**](https://developer.whoop.com/), create an app to get a Client ID and Client Secret. Then complete the OAuth2 flow to obtain an Access Token. All three are required for API access.

**Q: What is a WHOOP cycle?**
A WHOOP cycle represents a 24-hour period combining your sleep, strain and recovery data. Each cycle starts when you wake up and includes the previous night's sleep, the day's strain, and your recovery score for the next day.

**Q: How much historical data can I access?**
You can access all historical data recorded by your WHOOP device. Use the start and end date parameters (ISO 8601 format) to filter results. Pagination returns up to 25 records per request; use the nextToken to retrieve more.

**Q: Does the API include heart rate data?**
Yes! Heart rate data (average and max) is included in the cycle, workout and recovery responses. There's no dedicated heart rate endpoint, but the data is nested within these resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whoop](https://vinkius.com/mcp/whoop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WHOOP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `whoop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WHOOP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "whoop": {
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
