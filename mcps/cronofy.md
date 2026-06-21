# Cronofy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cronofy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cronofy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cronofy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling via Cronofy — unify Google, iCloud, and Exchange calendars to manage events and track multi-user availability directly from any AI agent.

## Description
Connect your **Cronofy** account to any AI agent and take full control of your unified calendar and scheduling workflows through natural conversation.

### What you can do

- **Unified Event Management** — List, retrieve, and create events across aggregated Google, iCloud, and Exchange overlays limitlessly
- **Multi-User Availability** — Query availability for up to 10 participants simultaneously, calculating strict intersections to find the perfect meeting time
- **Free/Busy Auditing** — Execute bulk iterations to map time matrices and return exact available boundaries without exposing event payloads
- **Automated Scheduling** — Generate live-availability links and shared scheduling requests to simplify meeting coordination with external members
- **Identity & Profile Mapping** — Inspect unified account canonical IDs and list distinct identity providers connected natively to your Cronofy profile
- **Sync Control** — Irreversibly vaporize explicit validations and delete events to maintain absolute consistency across all connected upstream providers

### How it works

1. Subscribe to this server
2. Enter your Cronofy Access Token (obtained via OAuth flow at app.cronofy.com)
3. Start managing your unified calendars from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Builders** — embed calendar and scheduling automation into AI-powered tools and applications
- **Recruiters & Sales Ops** — coordinate multi-participant meetings and verify availability across different providers in real-time
- **Executive Assistants** — manage complex schedules and generate scheduling links using natural language
- **DevOps Teams** — monitor calendar sync states and audit organizational scheduling requests


## Available Tools
- **read_events**: cronofy.com/v1/events` pulling unified aggregated Google, iCloud, and Exchange overlays limitlessly.

Identify bounded CRM records inside the Headless Cronofy Engine
- **create_event**: Provision a highly-available JSON Payload generating explicit Sync links
- **delete_event**: Irreversibly vaporize explicit validations extracting rich Provider syncs
- **list_calendars**: Retrieve explicit Cloud logging tracing explicit Payload IDs limitlessly
- **get_free_busy**: Enumerate explicitly attached structured rules exporting active Overlaps
- **query_availability**: Dispatch an automated validation check routing explicit Cross-Provider checks
- **get_account**: Inspect deep internal arrays mitigating specific Sub Provider lists
- **get_user_info**: Identify precise active arrays spanning native Gateway auth bounds
- **list_profiles**: Retrieve the exact structural matching verifying Blueprint directories
- **create_scheduling_request**: Fetch elaborate explicit mapped limits via native forms dispatch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cronofy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my calendar events from tomorrow to next week"

**🤖 AI Agent:**
> Retrieving unified events... I found 8 events across your Google and Exchange calendars. Highlights include 'Client Kickoff' on Tuesday at 10 AM and 'Team Sync' on Thursday at 2 PM.

---

**👤 You:**
> "Find a 30-minute slot for a meeting with john@example.com tomorrow"

**🤖 AI Agent:**
> Analyzing availability... John has three 30-minute slots available tomorrow: 9:30 AM, 1:00 PM, and 4:30 PM. Which one works best for you?

---

**👤 You:**
> "Create a scheduling link for a 'Project Review' meeting"

**🤖 AI Agent:**
> Scheduling request created! Here is the link for the 'Project Review': https://scheduling.cronofy.com/r/abc-123. This link is mapped to your live availability across all connected calendars.


## Installation & Usage

To install and use the **Cronofy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cronofy](https://vinkius.com/mcp/cronofy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
