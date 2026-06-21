# StatHat MCP Server

Track custom metrics and statistics effortlessly via StatHat — post counters, values, and batch updates directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/stathat)

## Overview
**Category:** developer-tools
**Tools Count:** 4

## Description
Connect your **StatHat** account to any AI agent to monitor your application's performance and business metrics through simple commands.

### What you can do

- **EZ Statistics** — Post stats using just a name (e.g., "User Signups"). StatHat automatically creates the metric if it doesn't exist.
- **Classic Counters** — Increment specific metrics using unique Stat Keys for precise tracking.
- **Value Tracking** — Send numerical values (like response times or temperatures) to specific stat keys.
- **Batch Processing** — Use the JSON API to send multiple statistics in a single request for high-efficiency logging.

### How it works

1. Subscribe to this server
2. Enter your StatHat EZ Key or User Key
3. Start logging metrics from Claude, Cursor, or any MCP-compatible client

No more manual dashboard entries or complex SDK configurations for quick tracking. Your AI acts as a bridge to your data observability stack.

### Who is this for?

- **Developers** — log errors, function execution counts, or performance metrics directly from the IDE.
- **Data Analysts** — quickly update business KPIs or experimental results via natural language.
- **DevOps Engineers** — monitor system health and event counts without leaving the terminal or chat interface.


## Available Tools
- **post_classic_counter**: Post a counter stat using the StatHat Classic API
- **post_classic_value**: Post a value stat using the StatHat Classic API
- **post_ez_stat**: Creates the stat automatically if it does not exist.

Post a stat using the StatHat EZ API
- **post_json_stats**: Pass a JSON array of objects containing stat/key, count/value, and optional t (timestamp).

Post multiple stats using the StatHat JSON API


## Installation & Usage

To install and use the **StatHat** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stathat](https://vinkius.com/mcp/stathat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
