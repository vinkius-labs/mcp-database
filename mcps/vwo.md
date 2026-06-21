# VWO MCP Server

Manage A/B tests, feature flags, and conversion goals on VWO — the leading experience optimization platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vwo)

## Overview
**Category:** growth-engine
**Tools Count:** 10

## Description
Connect your **VWO (Visual Website Optimizer)** account to any AI agent and take control of your experimentation and feature rollout workflows through natural conversation.

### What you can do

- **Optimization Campaigns** — List and monitor active A/B tests and personalization campaigns directly from your agent
- **Feature Management** — List all feature flags and toggle their status across different environments for instant rollouts
- **Experiment Results** — Retrieve statistical results for any campaign, including performance metrics and significance levels
- **Conversion Tracking** — Browse conversion goals and KPIs being tracked to understand your optimization impact
- **Audience Segmentation** — List pre-defined segments to see how you are targeting different user groups
- **Environment Control** — Manage features across staging, production, and other configured VWO environments

### How it works

1. Subscribe to this server
2. Enter your VWO API Token and Account ID
3. Start managing your experiments and feature flags through Claude, Cursor, or any MCP-compatible client

No more jumping between experiment dashboards to check test results. Your AI agent becomes your optimization engine.

### Who is this for?

- **Growth Managers** — monitor experiment results and statistical significance without manual data exports
- **Product Managers** — manage feature rollouts and toggle flags across environments during launches
- **Data Analysts** — quickly surface conversion goal metrics and audience segment performance
- **CRO Specialists** — audit active campaigns and identify optimization opportunities through simple chat commands


## Available Tools
- **get_vwo_account_info**: Retrieves details about the authenticated VWO account
- **get_campaign_details**: Retrieves details for a specific VWO campaign
- **get_feature_flag_details**: Retrieves configuration for a specific VWO feature flag
- **get_campaign_results**: Retrieves statistical results for a VWO campaign
- **list_optimization_campaigns**: Lists all VWO A/B test and personalization campaigns
- **list_vwo_environments**: g. Production, Staging) for feature flag management.

Lists all configured VWO environments
- **list_feature_flags**: Lists all VWO feature flags
- **list_conversion_goals**: g. clicks, revenue) are being tracked.

Lists all conversion goals and metrics
- **list_audience_segments**: Lists all audience segments
- **toggle_feature_flag**: Provide the feature ID and the desired enabled status (true/false).

Enables or disables a VWO feature flag


## Installation & Usage

To install and use the **VWO** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vwo](https://vinkius.com/mcp/vwo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
