# Five9 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/five9)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/five9-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/five9-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor agents, manage call states, and track real-time contact center stats via AI agents with Five9.

## Description
Connect your **Five9** account to any AI agent and automate your contact center management through the Model Context Protocol (MCP). Five9 is a leading cloud contact center solution, and with this server, supervisors and administrators can monitor agent states, manage active interactions, and fetch real-time performance statistics directly through natural conversation.

### What you can do

- **Agent State Monitoring** — List the operational states of all agents and retrieve detailed state information for specific individuals.
- **Campaign & Skill Overview** — Access all configured campaigns and skills to understand your contact center's distribution and capacity.
- **Interaction Management** — List all active call or digital interactions and force-terminate sessions when necessary.
- **Real-time Statistics** — Fetch high-level contact center metrics to keep your pulse on performance without leaving your chat interface.
- **Remote Agent Control** — Update an agent's state (e.g., force to READY or LOGOUT) remotely to manage floor coverage efficiently.
- **User & Group Discovery** — List all users and agent groups defined in your organization for better context and reporting.
- **Seamless Session Management** — The server handles secure login and session token management automatically.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Five9 VCC Username and Password
3. Start managing your contact center operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Contact Center Supervisors** — quickly check agent availability and interaction counts while managing floor operations.
- **Operations Managers** — get a real-time overview of campaign performance and skill distribution through simple AI commands.
- **Support Leads** — monitor active support interactions and update agent states to ensure optimal customer service levels.


## Available Tools
- **get_agent_state**: Get specific agent state
- **get_statistics**: Get real-time statistics
- **list_active_interactions**: List active interactions
- **list_agent_groups**: List agent groups
- **list_agent_states**: List all agent states
- **list_campaigns**: List all campaigns
- **list_skills**: List all skills
- **list_users**: List all users
- **logout_session**: Logout supervisor session
- **terminate_interaction**: Terminate an interaction
- **update_agent_state**: g., READY, NOT_READY, LOGOUT).

Force update agent state


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Five9** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the current state of all agents."

**🤖 AI Agent:**
> Fetching agent states... Currently, 12 agents are 'READY', 5 are 'NOT_READY', and 3 are on 'BREAK'. Would you like the specific details for any individual agent?

---

**👤 You:**
> "Get real-time contact center statistics."

**🤖 AI Agent:**
> Retrieving statistics... Your organization has an Average Handle Time (AHT) of 4:30, Service Level is at 85%, and there are currently 15 calls waiting in the queue.

---

**👤 You:**
> "Force agent 'agent_123' to 'LOGOUT' state."

**🤖 AI Agent:**
> Action successful! Agent 'agent_123' has been remotely transitioned to the 'LOGOUT' state. Their supervisor session has been updated.


## Installation & Usage

To install and use the **Five9** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/five9](https://vinkius.com/mcp/five9)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
