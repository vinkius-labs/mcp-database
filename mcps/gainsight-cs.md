# Gainsight CS MCP Server

Manage customer success, track health scores, and oversee the timeline via AI agents with Gainsight CS.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gainsight-cs)

## Overview
**Category:** customer-support
**Tools Count:** 12

## Description
Connect your **Gainsight Customer Success** (NXT) instance to any AI agent to automate your customer retention and engagement operations through the Model Context Protocol (MCP). Gainsight is the industry-standard platform for customer success, empowering CSMs to manage health scores, track activities, and close CTAs. This MCP server enables you to retrieve company metadata, log timeline events, and oversee cockpit tasks directly through natural conversation.

### Key Features

- **Company Health Oversight** — List all customer companies, retrieve detailed profiles including health scores, and verify CSM assignments instantly.
- **Timeline Activity Management** — Access the customer activity timeline and programmatically log new calls, meetings, or notes directly from your chat interface.
- **People & Contact Data** — Access detailed profile information for customers and partners managed within the Gainsight People object.
- **Cockpit Automation** — List and manage Calls to Action (CTAs) and associated tasks to stay on top of your retention playbook.
- **Workforce Insights** — Verify your own identity and profile details to ensure you are working in the correct account context.
- **Real-time Synchronization** — Keep your customer success strategy accessible to your AI assistant without leaving your primary workspace.
- **NXT API Integration** — Leverage the power of the Gainsight NXT platform with secure header-based authentication.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gainsight Domain and Access Key (found in Administration > Connectors 2.0 > Gainsight API)
3. Start managing your customer success data from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly check an account's health score or log a quick meeting note without navigating the dashboard.
- **CS Operations** — automate the retrieval of CTA metadata or verify company mappings via simple AI commands.
- **Account Executives** — get a real-time overview of customer interaction history before renewal or expansion discussions.


## Available Tools
- **verify_api_connection**: Verify connection
- **log_timeline_activity**: Log new activity
- **get_cta_metadata**: Get CTA details
- **get_company_health**: Get company metadata
- **get_my_identity**: Get current user profile
- **get_person_details**: Get person metadata
- **get_task_metadata**: Get task details
- **list_calls_to_action**: List cockpit CTAs
- **list_customer_companies**: List Gainsight companies
- **list_crm_people**: List Gainsight people
- **list_cockpit_tasks**: List cockpit tasks
- **list_timeline_events**: List timeline activities


## Installation & Usage

To install and use the **Gainsight CS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gainsight-cs](https://vinkius.com/mcp/gainsight-cs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
