# Hotjar (Behavior Analytics) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hotjar-behavior-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hotjar-behavior-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hotjar-behavior-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Analyze user behavior via Hotjar — list sites, retrieve survey responses, and manage feedback widgets.

## Description
Connect your **Hotjar** account to any AI agent and take full control of your behavior analytics and user feedback through natural conversation.

### What you can do

- **Site Management** — List all registered sites and extract high-level details including tracking status and plan information directly from your agent
- **Survey Analysis** — Retrieve individual responses from active surveys, including detailed answers, timestamps, and device metadata to understand user sentiment
- **Feedback Monitoring** — Enumerate feedback widgets and pull discrete ratings, comments, and screenshots to identify friction points in your user journey
- **GDPR Compliance** — Look up specific user profiles and session counts, and execute right-to-erasure requests to delete user data securely
- **Organization Audit** — Navigate across different Hotjar organizations and retrieve site lists and member counts to manage multi-tenant environments efficiently

### How it works

1. Subscribe to this server
2. Enter your Hotjar Client ID, Client Secret, and Site ID
3. Start analyzing user behavior from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **UX Researchers** — audit survey responses and analyze user feedback through natural conversation without manual data exports
- **Product Managers** — monitor feedback widgets and tracking statuses across multiple sites to ensure data quality and user alignment
- **Data Privacy Officers** — automate user lookup and data deletion requests to maintain GDPR compliance with ease


## Available Tools
- **list_sites**: List all tracked sites
- **list_funnels**: List conversion funnels
- **get_site**: Get current site details
- **list_heatmaps**: List all heatmaps
- **get_heatmap**: Get heatmap details
- **list_surveys**: List all surveys
- **get_survey**: Get survey details
- **list_survey_responses**: List survey responses
- **list_feedback**: List incoming feedback
- **list_recordings**: List session recordings


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotjar (Behavior Analytics)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all surveys for our main marketing site"

**🤖 AI Agent:**
> I've found 3 active surveys on your main marketing site: 'Post-Purchase Feedback' (ID: 123), 'Feature Request Poll' (ID: 456), and 'Homepage NPS' (ID: 789). Which one would you like to see responses for?

---

**👤 You:**
> "Show me the last 5 responses for survey ID 123"

**🤖 AI Agent:**
> Retrieving survey responses… The last 5 respondents gave an average rating of 4.2/5. Common feedback includes 'Easy to use checkout' and 'Would like more payment options'. Would you like to see the full text for any response?

---

**👤 You:**
> "How many responses has our 'NPS Widget' received so far?"

**🤖 AI Agent:**
> Your 'NPS Widget' (ID: fb-987) has received a total of 1,245 responses with an average rating of 8.4. I can retrieve the detailed comments and device metadata if you'd like to analyze the trends.


## Installation & Usage

To install and use the **Hotjar (Behavior Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hotjar-behavior-analytics](https://vinkius.com/mcp/hotjar-behavior-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
