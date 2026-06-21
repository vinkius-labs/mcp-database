# AntEater MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/anteater)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/anteater-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/anteater-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Monitor website changes, detect content updates, and receive alerts when key pages are modified across your digital properties.

## Description
Connect your **AntEater** (by AntEater Analytics) account to any AI agent and take full control of your team activity analysis and automated productivity monitoring through natural conversation.

### What you can do

- **Activity Portfolio Orchestration** — List and manage all captured team activities (emails, Slack, Jira) programmatically, retrieving detailed behavioral metadata
- **Search & Discovery Intelligence** — Programmatically search and retrieve high-fidelity insights from your organization's communication channels to maintain a perfectly coordinated knowledge base
- **Productivity Architecture Monitoring** — Access real-time status updates for team workstreams and track time-tracking results directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity collaboration signals and interaction history to maintain a perfectly coordinated audit trail
- **Operational Monitoring** — Verify account-level API connectivity and monitor activity ingestion volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your AntEater Analytics dashboard (Settings > API)
3. Start orchestrating your team knowledge from Claude, Cursor, or any MCP client

No more manual searching for 'who is doing what' or missing critical team progress signals. Your AI acts as your dedicated operations coordinator and activity architect.

### Who is this for?

- **Operations Managers** — instantly retrieve team activity summaries and monitor productivity using natural language commands
- **Product Leads** — verify individual task metadata and track project participation without leaving your workspace
- **Developers** — integrate high-speed AntEater analysis data into custom internal dashboards through simple AI queries


## Available Tools
- **check_anteater_status**: Verify AntEater API connectivity
- **get_contact_history**: Get communication history for a contact
- **get_profile**: Get your authenticated user profile
- **get_user**: Get details of a specific team member
- **list_contacts**: List all shared contacts
- **list_users**: List all team members
- **list_recent_activity**: List recent team activity
- **search_activity**: Search team activity across Slack and email
- **search_contacts**: Search contacts by name or company
- **get_user_activity**: Get activity for a specific team member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AntEater** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Slack discussions related to 'Project X' from yesterday."

**🤖 AI Agent:**
> I've performed the high-fidelity activity search. I found 3 relevant Slack threads matching 'Project X', including an update from @user1 at 2:00 PM. Would you like the detailed message metadata or participants for any of them?

---

**👤 You:**
> "Show the time spent on 'Development' tasks this week."

**🤖 AI Agent:**
> Productivity intelligence orchestrated! For this week, I've identified 40 high-fidelity hours spent on Development across the team. I've retrieved the technical workstream metadata for your review. Need help auditing the task distribution?

---

**👤 You:**
> "Check for any new activity ingestion alerts today."

**🤖 AI Agent:**
> Operational monitoring complete! Your activity ingestion is healthy today, with 1,000 high-fidelity signals processed from Slack and Gmail. Your API connection is healthy. Shall I retrieve the detailed engagement breakdown by rep?


## Installation & Usage

To install and use the **AntEater** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/anteater](https://vinkius.com/mcp/anteater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
