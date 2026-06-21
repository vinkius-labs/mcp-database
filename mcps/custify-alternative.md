# Custify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/custify-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/custify-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/custify-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Predict and prevent customer churn with health scores, lifecycle tracking, and automated playbooks for your CS team.

## Description
Connect your **Custify** customer success account to any AI agent and simplify how you manage your product users, track account health, and monitor churn risk through natural conversation.

### What you can do

- **User & Company Oversight** — List all managed people and organizations and retrieve detailed metadata and health scores.
- **Health Monitoring** — Query health score metrics and values to identify at-risk customers and churn signals instantly.
- **Event Tracking** — Record custom user actions and events programmatically to feed your success analytics.
- **Segment Analysis** — List and query defined customer segments to understand your user distribution.
- **CRM Control** — Create new person records and update profile data directly via AI commands.
- **Engagement Insights** — Fetch engagement history and metadata for individual accounts directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Custify API Key (found in your account settings)
3. Start managing your customer success lifecycle from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers (CSMs)** — quickly check account health and track recent user events via simple AI queries.
- **Success Operations** — monitor segment distributions and verify company metadata directly from the workspace.
- **Product Teams** — track custom feature adoption events and monitor user profile quality via the AI assistant.


## Available Tools
- **create_person**: Create a new person record
- **get_company_details**: Get details for a specific company
- **get_person_details**: Get details for a specific person
- **list_companies**: List customer companies
- **list_health_scores**: List customer health scores
- **list_people**: List product users (people)
- **list_user_segments**: List user segments
- **track_user_event**: Track a custom event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Custify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active companies in my Custify account."

**🤖 AI Agent:**
> I've retrieved your companies list. You have 25 managed accounts including 'Acme Corp', 'Tech Giant', and 'Global Logistics'. Which one would you like to see the health score for?

---

**👤 You:**
> "Show me the details and health for person 'john.doe@example.com'."

**🤖 AI Agent:**
> Fetching profile... John Doe currently has a Health Score of 92/100 (Healthy). His last recorded event was 'Feature X Usage' 2 hours ago. Would you like to see his full engagement history?

---

**👤 You:**
> "Track a 'Button Clicked' event for user 'user_88231'."

**🤖 AI Agent:**
> Event tracked! I've recorded the 'Button Clicked' action for user user_88231 in Custify. This data will be used to update their health score and engagement metrics.


## Installation & Usage

To install and use the **Custify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/custify-alternative](https://vinkius.com/mcp/custify-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
