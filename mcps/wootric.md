# Wootric MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wootric)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wootric-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wootric-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Manage Wootric customer feedback — track end users, survey responses, and declines directly from your AI agent.

## Description
Connect **Wootric** to your AI agent to streamline your customer experience workflows. Monitor Net Promoter Score (NPS), Customer Satisfaction (CSAT), and Customer Effort Score (CES) data through natural conversation.

### What you can do

- **End User Management** — List, create, and update customer profiles and their custom properties to keep your CRM in sync.
- **Response Tracking** — Query survey scores and comments to understand customer sentiment in real-time.
- **Decline Monitoring** — Track survey declines to optimize your sampling and outreach strategy.
- **Feedback History** — Retrieve user-specific feedback history for deep sentiment analysis and reporting.

### How it works

1. Subscribe to this server
2. Enter your Wootric Access Token
3. Start analyzing customer feedback from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Customer Success Managers** — quickly retrieve a user's feedback history before a call to personalize the conversation.
- **Product Managers** — analyze survey comments and scores to prioritize the product roadmap based on user pain points.
- **Data Analysts** — query response data directly to build reports without manual CSV exports.


## Available Tools
- **update_project**: Update a project
- **update_response**: Update a response
- **update_tag**: Update a tag
- **create_decline**: Create a decline for an end user
- **create_end_user**: Create a new end user
- **create_import**: Create an import
- **create_project**: Create a project
- **create_response**: Create a response for an end user
- **create_tag**: Create a tag
- **delete_decline**: Delete a decline
- **delete_end_user**: Delete an end user
- **delete_response**: Delete a response
- **delete_tag**: Delete a tag
- **get_end_user**: Get a specific end user by ID
- **list_declines**: Get all declines
- **list_end_user_responses**: Get responses for a specific end user
- **list_end_users**: Get all end users
- **list_projects**: Get all projects
- **list_responses**: Get all responses
- **list_tags**: Get all tags
- **onboard_cxi**: Onboard account for CXI features
- **update_end_user**: Update an end user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wootric** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recent end users from Wootric."

**🤖 AI Agent:**
> I've retrieved the end users. Here are the latest profiles, including 'customer_99' (ID: 12345) and 'user_alpha' (ID: 67890). Would you like to see the details for one of them?

---

**👤 You:**
> "Show me all survey responses for user ID 12345."

**🤖 AI Agent:**
> User 12345 has submitted 2 responses. The latest was an NPS score of 9 with the comment: 'Great service!'. The previous one was a score of 7.

---

**👤 You:**
> "Create a new survey response for user 67890 with a score of 10 and the text 'Amazing experience'."

**🤖 AI Agent:**
> Successfully created the response for user 67890. The score of 10 and your comment have been recorded in Wootric.


## Installation & Usage

To install and use the **Wootric** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wootric](https://vinkius.com/mcp/wootric)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
