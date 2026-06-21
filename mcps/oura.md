# Oura MCP Server

Access your Oura Ring health data — sleep, activity, readiness, HRV, heart rate and workout metrics from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/oura)

## Overview
**Category:** data-analytics
**Tools Count:** 7

## Description
Connect your **Oura Ring** to any AI agent and access your personal health data through natural conversation.

### What you can do

- **Sleep** — Analyze sleep scores, stages (REM/light/deep/wake), efficiency, latency and timing
- **Activity** — Track daily steps, calories, MET minutes and activity goals
- **Readiness** — Monitor readiness scores, HRV, resting heart rate, body temperature and recovery
- **Tags** — Review your manual entries for mood, energy, behaviors and substances
- **Workouts** — Browse logged workouts with type, duration, calories and heart rate zones
- **Heart Rate** — Access detailed 5-minute heart rate samples and HRV data

### How it works

1. Subscribe to this server
2. Enter your Oura Personal Access Token
3. Start exploring your health data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Health Enthusiasts** — track sleep quality, daily readiness and activity trends over time
- **Athletes** — monitor recovery, HRV and workout performance to optimize training
- **Biohackers** — correlate tags (mood, energy, behaviors) with sleep and readiness scores


## Available Tools
- **get_activity**: Supports date range filtering.

Get your Oura activity data
- **get_heart_rate**: Returns timestamp, heart rate value and HRV for each sample. Supports date range filtering. Note: This endpoint returns high-frequency data; use narrow date ranges.

Get your Oura heart rate data
- **get_readiness**: Supports date range filtering.

Get your Oura readiness data
- **get_sessions**: Includes overall scores, sleep metrics, activity data and readiness indicators. Supports date range filtering.

Get your Oura session data
- **get_sleep**: Supports date range filtering with start_date and end_date (YYYY-MM-DD). Pagination via nextToken.

Get your Oura sleep data
- **get_tags**: ). Tags are user-entered data points that correlate with sleep and readiness scores. Supports date range filtering.

Get your Oura tags
- **get_workouts**: Workouts can be manually logged or auto-detected by the Oura Ring. Supports date range filtering.

Get your Oura workout data


## Installation & Usage

To install and use the **Oura** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oura](https://vinkius.com/mcp/oura)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
