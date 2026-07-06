# Polar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polar-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access your Polar Flow data — training sessions, daily activity, sleep metrics, and physical info directly from your AI agent.

## Description
Connect your **Polar AccessLink** account to any AI agent to analyze your fitness journey and health metrics through natural conversation.

### What you can do

- **Training Analysis** — List exercises from the last 30 days and fetch detailed data including heart rate zones and routes using `list_exercises` and `get_exercise`.
- **Activity Tracking** — Monitor daily activity summaries, step counts, and specific daily metrics with `list_activities` and `get_activity_by_date`.
- **Recovery & Sleep** — Access comprehensive sleep records and Nightly Recharge™ status to optimize your rest via `list_sleep` and `list_nightly_recharge`.
- **Data Export** — Download your exercise data in FIT, TCX, or GPX formats for external analysis using `get_exercise_fit`, `get_exercise_tcx`, or `get_exercise_gpx`.
- **Physical Metrics** — Retrieve your latest physical info such as weight, height, and maximum heart rate with `get_physical_info`.

### How it works

1. Subscribe to this server
2. Enter your Polar Access Token
3. Start querying your health and fitness data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Athletes & Fitness Enthusiasts** — track your progress and recovery trends without manually exporting files.
- **Health Coaches** — quickly review client metrics and training consistency through an AI assistant.
- **Data Nerds** — easily pull raw biometric data for custom analysis or logging.


## Available Tools (27)
- **delete_webhook**: Remove a webhook
- **get_activity_by_date**: Get activity for a specific date
- **get_biosensing_body_temperature**: Get body temperature data
- **get_biosensing_ecg**: Get wrist ECG test results
- **get_biosensing_skin_temperature**: Get sleep skin temperature
- **get_biosensing_spo2**: Get SpO2 test results
- **get_cardio_load**: Retrieve training strain and recovery data
- **get_continuous_heart_rate**: Get continuous heart rate samples
- **get_exercise_fit**: Download exercise in FIT format
- **get_exercise_gpx**: Download exercise in GPX format
- **get_exercise_tcx**: Download exercise in TCX format
- **get_exercise**: Get detailed exercise data
- **get_notifications**: Check for available data for all registered users
- **get_physical_info**: Retrieve user physical metrics
- **get_sleepwise_alertness**: Get alertness period data
- **get_sleepwise_circadian_bedtime**: Get circadian bedtime data
- **get_user**: Retrieve basic user information
- **get_webhooks**: Get current webhook configuration
- **list_activities**: List activity summaries
- **list_activity_samples**: List activity samples
- **list_exercises**: List exercises from the last 30 days
- **list_nightly_recharge**: List Nightly Recharge status
- **list_sleep**: List sleep data
- **register_user**: Register a user after authorization
- **delete_user**: De-register a user and revoke access
- **activate_webhook**: Re-activate a deactivated webhook
- **create_webhook**: Create a webhook


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my training sessions from the last 30 days."

**🤖 AI Agent:**
> I've found 12 exercises in the last 30 days. Your most recent was a 'Running' session on Oct 26th with a duration of 45 minutes. Would you like the details for this session?

---

**👤 You:**
> "Show me my sleep data and nightly recharge status."

**🤖 AI Agent:**
> Your sleep score for last night was 82 (Good). Your Nightly Recharge status is 'Very Restorative' with an ANS charge of +4.2. You seem well-recovered!

---

**👤 You:**
> "Get my activity summary for 2023-10-25."

**🤖 AI Agent:**
> On Oct 25th, you reached 115% of your activity goal with 12,450 steps and 2,840 calories burned. You had 1 hour and 20 minutes of high-intensity activity.


## ❓ FAQ

**Q: Can I download my training sessions in FIT or GPX format for other apps?**
Yes! You can use `get_exercise_fit`, `get_exercise_tcx`, or `get_exercise_gpx` with a specific Exercise ID to retrieve the raw file data for your training sessions.

**Q: How do I check my recovery and sleep quality from last night?**
Simply ask the agent to run `list_sleep` or `list_nightly_recharge`. It will provide the latest metrics recorded by your Polar device, including sleep scores and recharge levels.

**Q: Can I see my physical metrics like weight and heart rate max?**
Yes, the `get_physical_info` tool retrieves your current physical settings from Polar Flow, including weight, height, and HR max.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polar-alternative](https://vinkius.com/mcp/polar-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polar-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polar-alternative": {
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
