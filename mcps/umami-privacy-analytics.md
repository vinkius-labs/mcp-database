# Umami (Privacy Analytics) MCP Server

Manage your Umami analytics — track events, manage websites, and oversee users directly through your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/umami-privacy-analytics)

## Overview
**Category:** marketing-automation
**Tools Count:** 53

## Description
Connect your **Umami** instance to any AI agent to monitor your privacy-focused analytics and manage your infrastructure through natural language. Umami is the open-source, privacy-friendly alternative to Google Analytics, and this MCP server gives you full control over your data.

### What you can do

- **Event Tracking** — Send custom events and page views directly to your Umami instance using the `send_event` tool.
- **Website Management** — List and manage all websites associated with your account or the entire instance using `get_me_websites` or `admin_list_websites`.
- **User & Team Administration** — Perform administrative tasks like creating, updating, or deleting users and managing teams with tools like `create_user` and `admin_list_teams`.
- **Session Insights** — Retrieve information about your current session and authorized access levels using `get_me`.
- **Self-Hosted Support** — Seamlessly connect to your own infrastructure using the `login` tool to authenticate and retrieve tokens.

### How it works

1. Subscribe to this server
2. Provide your Umami Instance URL and API Key (or use the login tool)
3. Start querying your analytics data or managing users from Claude, Cursor, or any MCP client

### Who is this for?

- **Data Analysts** — quickly pull website lists and verify tracking status without leaving the chat interface.
- **DevOps & Admins** — automate user provisioning and team management on self-hosted Umami instances.
- **Growth Marketers** — trigger test events and verify analytics pipelines during development.


## Available Tools
- **add_team_user**: Add user to team
- **admin_list_teams**: Returns all teams (Admin only)
- **admin_list_users**: Returns all users (Admin only)
- **admin_list_websites**: Returns all websites (Admin only)
- **create_attribution_report**: Marketing attribution report
- **create_funnel_report**: Conversion funnel report
- **create_link**: Creates a link
- **create_pixel**: Creates a pixel
- **create_report**: Creates a report
- **create_retention_report**: User retention report
- **create_revenue_report**: Revenue report
- **create_team**: Creates a team
- **create_user**: Creates a user (Admin only)
- **create_website**: Creates a website
- **delete_user**: Deletes a user (Admin only)
- **delete_website**: Deletes a website
- **get_me_teams**: Get all teams for the current user
- **get_me**: Get information about the current session
- **get_me_websites**: Get all websites for the current user
- **get_realtime_stats**: Realtime stats within the last 30 minutes
- **get_session_activity**: Activity for a session
- **get_session**: Individual session details
- **get_team_users**: Get team members
- **get_team_websites**: Get team websites
- **get_user_teams**: Gets all teams belonging to a user (Admin only)
- **get_user**: Gets a user by ID (Admin only)
- **get_user_websites**: Gets all websites belonging to a user (Admin only)
- **get_website_active**: Active users in the last 5 minutes
- **get_website_daterange**: Available data date range
- **get_website_event_data_events**: Event data names and counts
- **get_website_event_data_fields**: Property and value counts
- **get_website_event_data**: Event data grouped by event
- **get_website_events_stats**: Aggregated event statistics
- **get_website_events**: Website event details
- **get_website_metrics_expanded**: Expanded metrics including bounces and total time
- **get_website_metrics**: Metrics for a given time range (type: path, browser, os, etc.)
- **get_website_pageviews**: Pageviews and sessions series data
- **get_website_sessions_stats**: Summarized session statistics
- **get_website_sessions**: Website session details
- **get_website_stats**: Summarized website statistics (pageviews, visitors, etc.)
- **get_website**: Gets a website by ID
- **join_team**: Join a team via access code
- **list_links**: Returns all user links
- **list_pixels**: Returns all user pixels
- **list_reports**: Get all reports by website ID
- **list_teams**: Returns all teams
- **list_websites**: Returns all user websites
- **login**: Login to self-hosted Umami to get a token
- **reset_website**: Removes all data related to the website
- **send_event**: Send an event to Umami
- **update_user**: Updates a user (Admin only)
- **update_website**: Updates a website
- **verify_token**: Verify if the current token is still valid


## Installation & Usage

To install and use the **Umami (Privacy Analytics)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umami-privacy-analytics](https://vinkius.com/mcp/umami-privacy-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
