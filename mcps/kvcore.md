# kvCORE MCP Server

Manage real estate leads — search contacts, track listings, and audit agent tasks.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kvcore)

## Overview
**Category:** real-estate
**Tools Count:** 10

## Description
Connect your AI agent to **kvCORE**, the primary platform for real estate professionals to manage their entire business.

### Key Features

- **Lead Management** — Search and audit lead profiles, update statuses, and add manual notes through natural language
- **Listing Intelligence** — Access active property listings and detailed metadata including features and pricing
- **Marketing Visibility** — List and monitor smart campaigns and automated marketing sequences
- **Agent Workflow** — Audit pending tasks, reminders, and recent lead activities to stay on top of follow-ups
- **Profile Insights** — Fetch agent profile data and high-level account configuration

### Simple Setup

1. Subscribe to this server
2. Log in to kvCORE, go to **Settings** > **API**, and generate an API Key
3. Enter your key in the configuration panel
4. Start managing your real estate business via chat


## Available Tools
- **search_kvcore_leads**: Returns lead IDs and basic contact info.

Search for leads in kvCORE
- **get_lead_details**: Get details for a specific lead
- **list_property_listings**: List active property listings
- **get_listing_details**: Get metadata for a specific listing
- **list_marketing_campaigns**: List all marketing campaigns
- **list_agent_tasks**: List pending tasks for the agent
- **get_agent_profile**: Get current agent information
- **update_lead_info**: g., status, phone). Provide data as a JSON string.

Update an existing lead
- **list_lead_activity**: List recent activity for a lead
- **create_lead_note**: Add a note to a lead profile


## Installation & Usage

To install and use the **kvCORE** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kvcore](https://vinkius.com/mcp/kvcore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
