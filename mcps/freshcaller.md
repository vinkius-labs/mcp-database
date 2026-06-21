# Freshcaller MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshcaller)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/freshcaller-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/freshcaller-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage your cloud phone system, track calls, and oversee agents via AI agents with Freshcaller.

## Description
Connect your **Freshcaller** (now Freshdesk Contact Center) account to any AI agent to automate your cloud telephony and contact center management through the Model Context Protocol (MCP). Freshcaller is a modern phone system that enables teams to handle customer calls across the globe with zero hardware. This MCP server enables you to track call logs, monitor agent performance, and retrieve recording links directly through natural conversation.

### Key Features

- **Call Oversight** — List all inbound and outbound calls, fetch detailed metadata including duration and status, and monitor recent activity instantly.
- **Agent Management** — Access your database of users and agents to maintain full context of who is online and handling calls.
- **Team Coordination** — List configured agent teams and retrieve metadata for specific groups to optimize your routing.
- **Recording Retrieval** — Get direct links to call recordings for quality assurance and training purposes directly from your chat interface.
- **Performance Metrics** — Access real-time account metrics to understand call volumes and service levels across your organization.
- **Number Inventory** — List owned phone numbers and search for new available numbers to scale your global presence.
- **Data Export** — Monitor initiated export jobs to ensure your historical data is ready for deep analysis.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Freshcaller Domain and API Key (found in your Profile Settings)
3. Start managing your cloud phone system from Claude, Cursor, or any MCP client

### Who is this for?

- **Support Managers** — quickly check missed call counts or list agent statuses without manual dashboard navigation.
- **Customer Success Ops** — get a real-time overview of call center metrics and recording links via simple AI commands.
- **Sales Teams** — track outbound call history and verify durations for lead engagement reporting.


## Available Tools
- **get_call_details**: Get call metadata
- **get_export_status**: Check export job
- **get_call_recording**: Get recording link
- **get_team_details**: Get team metadata
- **get_agent_details**: Get agent metadata
- **list_buyable_numbers**: Search for phone numbers
- **list_calls**: List recent phone calls
- **list_export_jobs**: List data exports
- **list_account_metrics**: Get call center metrics
- **list_my_numbers**: List owned phone numbers
- **list_agent_teams**: List agent teams
- **list_agents**: List call center agents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Freshcaller** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent calls and their duration."

**🤖 AI Agent:**
> Retrieving calls... I found 5 recent entries, including an inbound call from '+1234567890' (Duration: 120s) and an outbound call to '+10987654321' (Duration: 45s).

---

**👤 You:**
> "Show me the status of all agents in my support team."

**🤖 AI Agent:**
> Fetching agents... In your support team, 3 agents are 'Online' (John, Sarah, Mike), 1 is 'On Call' (Emma), and 2 are 'Offline'.

---

**👤 You:**
> "Get the recording link for call 'call_abc123'."

**🤖 AI Agent:**
> Retrieving recording... I've successfully fetched the secure recording link for call 'call_abc123'. You can access it here: [Recording Link].


## Installation & Usage

To install and use the **Freshcaller** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshcaller](https://vinkius.com/mcp/freshcaller)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
