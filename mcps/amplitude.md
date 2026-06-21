# Amplitude MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/amplitude)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/amplitude-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/amplitude-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Analyze product data via Amplitude — get user activity, calculate retention, analyze funnels, and track revenue directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Amplitude** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What's our funnel conversion from 'Landing_Page_View' to 'Sign_Up_Success' for the last 3 days?"

**🤖 AI Agent:**
> I checked the conversion funnel. Over the last 3 days, 14,200 users triggered 'Landing_Page_View'. Of those, 2,840 completed 'Sign_Up_Success'. This represents an overall conversion rate of 20%, which is slightly above our weekly average.

---

**👤 You:**
> "Show the recent user activity for customer email@example.com"

**🤖 AI Agent:**
> I've pulled the activity stream for email@example.com. In the last 2 hours, they logged in, triggered 'Payment_Initiated', but then hit an error on 'Payment_Gateway_Failed'. You might want to review the exact property payload.

---

**👤 You:**
> "What is our Daily Active Users (DAU) count since start of the month?"

**🤖 AI Agent:**
> I fetched the DAU data. Since the 1st of the month, DAU has ranged from 45,000 to 52,000. Yesterday hit a peak at 52,104, reflecting our recent campaign launch. Would you like a breakdown of revenue from this period?


## Installation & Usage

To install and use the **Amplitude** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/amplitude](https://vinkius.com/mcp/amplitude)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
