# Polar MCP Server

Access your Polar Flow data — training sessions, daily activity, sleep metrics, and physical info directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/polar-alternative)

## Overview
**Category:** data-analytics
**Tools Count:** 27

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


## Available Tools
- **activate_webhook**: Re-activate a deactivated webhook
- **create_webhook**: Create a webhook
- **delete_user**: De-register a user and revoke access
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


## Installation & Usage

To install and use the **Polar** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polar-alternative](https://vinkius.com/mcp/polar-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
