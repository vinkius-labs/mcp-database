# Zenloop MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zenloop)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zenloop-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zenloop-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze NPS feedback and manage customer surveys via the Zenloop API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zenloop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my Zenloop account."

**🤖 AI Agent:**
> I've retrieved your surveys. You have 4 active surveys, including 'Post-Purchase NPS', 'Website Exit Intent', and 'Email Newsletter Feedback'. Would you like to see the responses for any of them?

---

**👤 You:**
> "Show me customer responses for survey ID 'abc123xyz' from last week."

**🤖 AI Agent:**
> I found 25 responses for survey abc123xyz from the last 7 days. The average NPS score is 8.4. Notable comments include 'Excellent service!' and 'Delivery was a bit slow'.

---

**👤 You:**
> "Submit a Link response for survey 'abc123' with score 10 and comment 'Amazing experience!'."

**🤖 AI Agent:**
> Successfully submitted the response to survey 'abc123'. The score of 10 and your comment have been recorded in Zenloop.


## Installation & Usage

To install and use the **Zenloop** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zenloop](https://vinkius.com/mcp/zenloop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
