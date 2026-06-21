# Oura MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oura)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/oura-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/oura-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access your Oura Ring health data — sleep, activity, readiness, HRV, heart rate and workout metrics from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oura** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How did I sleep last night?"

**🤖 AI Agent:**
> Last night: Sleep score 85/100. Total: 7h 42m. Deep: 2h 10m, REM: 1h 45m, Light: 3h 15m, Awake: 32m. Efficiency: 92%. Onset: 15min. Restlessness: Low.

---

**👤 You:**
> "What is my readiness score today?"

**🤖 AI Agent:**
> Today's readiness: 82/100 (Good). HRV: 65ms, Resting HR: 51 bpm, Body temp: 36.6°C. Sleep balance: 8h 5min. Activity balance: Well recovered. Previous day strain: 14.

---

**👤 You:**
> "Show me my activity from yesterday."

**🤖 AI Agent:**
> Yesterday's activity: Score 75/100. Steps: 8,450. Calories: 2,340 (active: 520). MET minutes: 145. Average HR: 72 bpm. Inactivity: 11h 20m. Daily goal: 85% achieved.


## Installation & Usage

To install and use the **Oura** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oura](https://vinkius.com/mcp/oura)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
