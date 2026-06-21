# WHOOP MCP Server

Track your WHOOP health metrics — workouts, sleep, recovery, strain, HRV and body measurements from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/whoop)

## Overview
**Category:** productivity
**Tools Count:** 11

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


## Installation & Usage

To install and use the **WHOOP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/whoop](https://vinkius.com/mcp/whoop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
