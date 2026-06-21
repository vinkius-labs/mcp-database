# Zenloop MCP Server

Analyze NPS feedback and manage customer surveys via the Zenloop API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zenloop)

## Overview
**Category:** customer-support
**Tools Count:** 8

## Description
Connect your **Zenloop** account to any AI agent to streamline your Net Promoter System (NPS) and customer feedback management. This MCP server enables your agent to interact with surveys, responses (answers), and account metadata directly from natural language.

### What you can do

- **Survey Oversight** — List all your active and historical surveys and retrieve their detailed summaries
- **Feedback Extraction** — List customer answers and responses for any survey, filtered by date range
- **Response Generation** — Programmatically create new survey answers across Link, Email, and Website channels
- **Performance Monitoring** — Access NPS scores and comments to track customer sentiment in real-time
- **Account Visibility** — Retrieve high-level account configuration and metadata for your Zenloop project

### How it works

1. Subscribe to this server
2. Enter your Zenloop API Token
3. Start managing your customer feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — Monitor real-time feedback and NPS trends without opening the dashboard
- **Product Managers** — Quickly retrieve customer comments related to specific product features or updates
- **Data Analysts** — Automate the extraction of survey responses for sentiment analysis and reporting


## Available Tools
- **get_account_details**: Get Zenloop account information
- **list_survey_answers**: Can be filtered by date.

List answers (responses) for a survey
- **create_email_answer**: Create a new survey response for an Email Embed channel
- **create_embed_answer**: Create a new survey response for a Website Embed channel
- **create_link_answer**: Create a new survey response for a Link channel
- **create_overlay_answer**: Create a new survey response for a Website Overlay channel
- **get_survey_details**: Get details for a specific survey
- **list_surveys**: List all configured surveys


## Installation & Usage

To install and use the **Zenloop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenloop](https://vinkius.com/mcp/zenloop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
