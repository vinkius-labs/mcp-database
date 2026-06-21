# LeadSquared MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leadsquared)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/leadsquared-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/leadsquared-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage leads, sales activities, and opportunities via the LeadSquared CRM API.

## Description
Connect your **LeadSquared** account to any AI agent to automate your sales execution and CRM workflows. This MCP server enables your agent to interact with leads, capture new prospects, track activities, and manage sales opportunities directly.

### What you can do

- **Lead Management** — Search, retrieve, and capture leads while maintaining a clean database with automatic deduplication
- **Activity Tracking** — List and record interactions like calls, meetings, and emails associated with specific leads
- **Opportunity Oversight** — Create and monitor sales opportunities and their associated activity histories
- **Custom Field Support** — Access full profile details and custom attributes for all your CRM entities
- **Workflow Automation** — Identify activity types and update prospect statuses via natural language commands

### How it works

1. Subscribe to this server
2. Enter your regional API Host, Access Key, and Secret Key
3. Start managing your sales pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Professionals** — Quickly update lead notes and opportunity statuses during your daily workflow
- **Marketing Teams** — Monitor lead capture performance and activity trends without opening the CRM
- **Operations Managers** — Automate prospect synchronization and maintain CRM data hygiene easily


## Available Tools
- **list_activity_types**: g., Phone Call, Meeting) configured in LeadSquared.

List all lead activity types
- **capture_lead**: Capture or update a lead
- **create_prospect_activity**: g., call log, email sent) to a lead profile.

Record a new activity for a lead
- **create_opportunity**: Create a new sales opportunity
- **create_or_update_lead**: Uses email or phone as the matching criteria.

Create or update a lead profile
- **get_lead_details**: Get details for a specific lead
- **list_lead_activities**: List activities for a specific lead
- **list_opportunities**: List sales opportunities
- **list_opportunity_activities**: List activities for a specific opportunity
- **search_leads**: Search for leads with criteria


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LeadSquared** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a lead with email 'test@example.com' in LeadSquared."

**🤖 AI Agent:**
> I've searched your LeadSquared CRM and found 'John Doe' (ID: 12345). He has a score of 85 and is currently in the 'Lead' stage. Would you like to see his recent activities?

---

**👤 You:**
> "List all sales opportunities in the pipeline."

**🤖 AI Agent:**
> I've retrieved 12 sales opportunities. Recent deals include 'Enterprise Upgrade' ($5,000) and 'Cloud Migration Project' ($12,000). Which one would you like to inspect?

---

**👤 You:**
> "Capture a new lead: Name 'Alice Smith', Email 'alice@corp.com'."

**🤖 AI Agent:**
> Successfully captured Alice Smith as a new lead in your LeadSquared CRM. Her profile has been created with ID '98765'.


## Installation & Usage

To install and use the **LeadSquared** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leadsquared](https://vinkius.com/mcp/leadsquared)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
