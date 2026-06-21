# Mixpanel (Event Analytics & Insights) MCP Server

Manage product analytics via Mixpanel — query event trends, track conversion funnels, and audit user cohorts.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mixpanel-event-analytics-insights)

## Overview
**Category:** growth-engine
**Tools Count:** 10

## Description
Connect your **Mixpanel** account to any AI agent and take full control of your product analytics, user behavior tracking, and conversion insights through natural conversation.

### What you can do

- **Event Orchestration** — Query aggregate event occurrences and unique user trends over specific date intervals to understand high-level feature engagement directly from your agent
- **Conversion Analysis** — Calculate step-by-step conversion rates and drop-offs for saved 'Funnels' to identify bottlenecks in your user journey securely
- **Retention Monitoring** — Compute user retention curves and recurring action return rates to understand long-term product stickiness and cohort behavior natively
- **Deep Segmentation** — Execute property-based breakdowns to split any event by specific attributes (e.g., plan type, region, device) for granular analytical insights
- **User Profile Audit** — Query distinct user profiles using proprietary JQL expression variables to retrieve detailed company metadata and user traits instantly
- **Behavioral Cohorts** — List and retrieve size metrics for saved user segments (Cohorts) to identify high-value audiences or risky churn segments securely
- **Raw Data Export** — Extract atomic event logs for deep-dive investigations or external reporting pipelines, maintaining literal chronological event fidelity

### How it works

1. Subscribe to this server
2. Enter your Mixpanel Service Account (User/Secret) and Project ID
3. Start exploring your product data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — audit feature adoption and monitor conversion funnels through natural conversation without manual report generation
- **Growth Leads** — track retention trends and experiment with property-based segmentation to optimize user acquisition directly from your workspace
- **Data Analysts** — retrieve raw event logs and query user profiles via JQL for rapid diagnostic investigations efficiently


## Available Tools
- **list_cohorts**: List saved behavioral cohorts
- **list_funnels**: List all saved funnel configurations
- **query_retention**: Calculate user retention curves
- **query_top_events**: Get the top 20 events by volume
- **query_events**: Query aggregate Mixpanel event counts over time
- **export_events**: Note: This API is rate-limited to 60 requests per hour.

Export raw event data logs
- **query_funnel**: Get conversion data for a specific funnel
- **query_insights**: Query complex dashboard insights
- **query_profiles**: g., properties["plan"]=="pro").

Search for specific user profiles
- **query_segmentation**: g., device or region).

Break down an event by specific properties


## Installation & Usage

To install and use the **Mixpanel (Event Analytics & Insights)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mixpanel-event-analytics-insights](https://vinkius.com/mcp/mixpanel-event-analytics-insights)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
