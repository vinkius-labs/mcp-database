# KnoCommerce MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/knocommerce)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/knocommerce-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/knocommerce-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Analyze post-purchase surveys — list responses, audit customer feedback, and track attribution channels.

## Description
Connect your **KnoCommerce** data to your AI agent to unlock deep insights from your post-purchase surveys.

### Key Features

- **Survey Analysis** — List and audit all active surveys to understand your feedback collection strategy
- **Response Auditing** — Drill down into individual customer responses to see exactly what your buyers are saying
- **Customer Profiles** — View feedback history associated with specific customer IDs to build a complete buyer profile
- **Attribution Reporting** — Access aggregated channel attribution data to see which marketing efforts are actually working
- **Template Discovery** — Browse available survey templates to quickly launch new feedback campaigns

### Simple Setup

1. Get your API Key from the KnoCommerce dashboard
2. Configure the MCP server in your favorite client (Claude, Cursor, etc.)
3. Start querying your survey data using natural language


## Available Tools
- **list_surveys**: Use this to identify survey IDs for analyzing specific campaigns or response sets.

List all KnoCommerce surveys
- **get_survey_details**: Returns survey title, status, and high-level configuration.

Get details for a specific survey
- **list_survey_responses**: You can optionally filter by survey_id to see feedback from a specific post-purchase interaction.

List responses for surveys
- **get_response_details**: Get details for a specific customer response
- **list_knocommerce_customers**: Useful for correlating feedback with specific buyer profiles.

List customers associated with survey data
- **get_customer_feedback_profile**: Get details for a specific customer feedback profile
- **list_survey_questions**: Use this to understand the data structure of the responses.

List all questions in a specific survey
- **get_channel_attribution_report**: This is essential for understanding which marketing channels are driving customer acquisition.

Get the latest channel attribution report
- **list_survey_templates**: List available survey templates
- **check_knocommerce_api_status**: Check the status of the KnoCommerce API integration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KnoCommerce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active surveys in my KnoCommerce account"

**🤖 AI Agent:**
> I've found 3 active surveys: 'Post-Purchase General', 'Holiday Special Feedback', and 'Product Fit Research'. Which one would you like to examine?

---

**👤 You:**
> "Show me the latest responses for survey 'kc_123'"

**🤖 AI Agent:**
> Retrieving responses for 'kc_123'… I've found 15 recent submissions. The overall sentiment seems positive, with most users mentioning 'Fast Shipping' as the primary reason for purchase.

---

**👤 You:**
> "Give me a channel attribution report"

**🤖 AI Agent:**
> The attribution report shows that 45% of your customers found you via 'Instagram Ads', 20% through 'Direct Search', and 15% from 'Email Marketing'.


## Installation & Usage

To install and use the **KnoCommerce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/knocommerce](https://vinkius.com/mcp/knocommerce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
