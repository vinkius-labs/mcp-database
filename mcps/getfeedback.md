# GetFeedback MCP Server

Manage online surveys, track real-time responses, and oversee feedback data via AI agents with GetFeedback.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/getfeedback)

## Overview
**Category:** customer-support
**Tools Count:** 12

## Description
Connect your **GetFeedback** account to any AI agent to automate your customer feedback and survey reporting workflows through the Model Context Protocol (MCP). GetFeedback is a powerful, mobile-friendly survey platform that helps brands collect and analyze customer sentiment in real-time. This MCP server enables you to retrieve survey results, monitor completion statuses, and trigger survey invitations directly through natural conversation.

### Key Features

- **Survey Orchestration** — List all active surveys in your account and fetch detailed structural metadata for each form.
- **Real-time Response Tracking** — Retrieve customer feedback as it arrives, including detailed answer payloads and completion timestamps.
- **Advanced Filtering** — List survey responses filtered by status (started, completed) or created after a specific date for targeted reporting.
- **Automated Invitations** — Trigger survey emails to a list of recipients programmatically from your chat interface.
- **Identity Oversight** — Access global profile information for the authenticated GetFeedback user to ensure correct account context.
- **Data Connectivity** — Verify your API connection and account health to maintain seamless feedback loops.
- **Asynchronous Monitoring** — Fetch high-level response counts and status metrics to track survey performance instantly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GetFeedback Access Token (found in your Account Settings)
3. Start managing your customer feedback from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Experience (CX) Managers** — quickly check for new survey completions or fetch high-level sentiment summaries without manual exports.
- **Support Leads** — get a real-time overview of feedback associated with recent customer interactions via simple AI commands.
- **Marketing Analysts** — automate the retrieval of survey data for weekly reporting and brand health tracking.


## Available Tools
- **check_api_limits**: Verify connectivity
- **verify_api_connection**: Check connection
- **get_my_identity**: Get user identity
- **get_response_details**: Get response metadata
- **get_survey_stats**: Get response count
- **get_survey_details**: Get survey metadata
- **list_completed_feedback**: Filter for completed
- **list_feedback_page**: Paginated responses
- **list_recent_feedback**: Filter by date
- **list_survey_responses**: List feedback data
- **list_surveys**: List all surveys
- **send_survey_invites**: Trigger survey email


## Installation & Usage

To install and use the **GetFeedback** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getfeedback](https://vinkius.com/mcp/getfeedback)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
