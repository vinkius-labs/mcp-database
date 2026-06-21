# Amplitude MCP Server

Analyze product data via Amplitude — get user activity, calculate retention, analyze funnels, and track revenue directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/amplitude)

## Overview
**Category:** growth-engine
**Tools Count:** 10

## Description
Connect your **Amplitude** account to your AI agent and seamlessly query behavioral data and product analytics using natural language.

### What you can do

- **User Activity & Search** — Search for specific users and track their detailed event stream to diagnose individual journeys
- **Funnels & Conversions** — Request step-by-step conversion funnels to identify where users drop off
- **Retention** — Generate day-over-day retention curves to understand how well features keep users engaged
- **Segmentation** — Query event counts and uniques over time to see clear adoption trends
- **Cohorts** — List your behavioral cohorts, view sizes, and request exports for further targeted analysis
- **Active Users & Revenue** — Instantly pull DAU/WAU/MAU and daily revenue metrics right into your workflow

### How it works

1. Subscribe to this server
2. Enter your Amplitude Project API Key and Secret Key
3. Start answering product questions directly via Claude, Cursor, or any MCP-compatible client

Never break your context to build dashboards. Ask your agent, get real-time data.

### Who is this for?

- **Product Managers** — rapidly test hypotheses by asking for funnel conversions or feature retention without coding
- **Data Analysts** — export raw events, find out user activity, and cross-reference cohorts easily
- **Customer Success** — debug specific user sessions by pulling their exact event activity stream
- **Growth Teams** — monitor daily revenue and active users instantly from your workspace


## Available Tools
- **export_events**: Amplitude is a product analytics platform. Pass start/end as YYYYMMDDTHH (e.g. 2026010100).

Export raw Amplitude event data for a time range
- **get_user_activity**: Useful for diagnosing individual user journeys.

Get Amplitude user activity stream
- **event_segmentation**: Pass event name, start/end as YYYYMMDD.

Query Amplitude event segmentation
- **search_users**: Useful to find specific users before checking their activity.

Search Amplitude users by user ID, device ID, or email
- **get_retention**: Pass start_event (acquisition), return_event, start/end dates. Start/End should be YYYYMMDD.

Query Amplitude retention
- **get_funnel**: Pass comma-separated event names, start/end as YYYYMMDD.

Query Amplitude funnel conversion
- **list_cohorts**: Cohorts group users by behavior.

List Amplitude behavioral cohorts
- **get_cohort**: Depending on the backend this may require polling until ready.

Request an Amplitude cohort download
- **revenue_analysis**: Start/End as YYYYMMDD.

Get Amplitude revenue analysis by day
- **active_users**: Start/End as YYYYMMDD.

Get Amplitude daily/weekly/monthly active users (DAU/WAU/MAU)


## Installation & Usage

To install and use the **Amplitude** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplitude](https://vinkius.com/mcp/amplitude)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
