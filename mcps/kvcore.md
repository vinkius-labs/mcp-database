# kvCORE MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kvcore)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kvcore-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kvcore-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage real estate leads — search contacts, track listings, and audit agent tasks.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **kvCORE** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a lead named 'Alice' in my kvCORE"

**🤖 AI Agent:**
> I've found one lead matching 'Alice': Alice Williams (Email: alice@example.com). She is currently in the 'Prospect' status. Would you like to see her recent property views?

---

**👤 You:**
> "Show me details for the property at '123 Maple St'"

**🤖 AI Agent:**
> Retrieved listing details for 123 Maple St. It's a 3-bed, 2-bath home listed at $450,000. It has been on the market for 15 days. Would you like to see the full description?

---

**👤 You:**
> "List my tasks for today"

**🤖 AI Agent:**
> You have 5 follow-up tasks for today, including calling John Doe about the new listing and sending a contract to Jane Smith. Which one would you like to mark as complete?


## Installation & Usage

To install and use the **kvCORE** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kvcore](https://vinkius.com/mcp/kvcore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
