# HireVue MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hirevue)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hirevue-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hirevue-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [video-conferencing](../categories/video-conferencing.md)

Streamline your recruitment process via HireVue — manage candidates, schedule interviews, and track positions directly from any AI agent.

## Description
Connect your **HireVue** account to any AI agent to automate and manage your hiring workflows through natural conversation.

### What you can do

- **Candidate Management** — Create, retrieve, and update candidate profiles with ease using `create_candidate`, `get_candidate`, and `update_candidate` tools.
- **Interview Orchestration** — Create interview invitations, check statuses, and cancel interviews when necessary via `create_interview`, `get_interview`, and `cancel_interview`.
- **Position Insights** — List all available job positions and fetch detailed metadata for specific roles using `list_positions` and `get_position`.
- **Workflow Automation** — Integrate hiring steps directly into your AI-driven workflows without switching tabs.

### How it works

1. Subscribe to this server
2. Enter your HireVue API Key and Base URL
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — Quickly check candidate statuses and schedule interviews without leaving the chat
- **Hiring Managers** — Review position details and candidate profiles instantly to make faster decisions
- **HR Operations** — Automate the creation of candidate records and interview invitations across the organization


## Available Tools
- **cancel_interview**: Cancel an interview
- **create_candidate**: Create a new candidate profile
- **create_interview**: Create an interview invitation
- **get_candidate**: Get candidate details
- **get_interview**: Get interview status
- **get_position**: Get position details
- **list_positions**: List all positions
- **update_candidate**: Update an existing candidate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HireVue** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available job positions in HireVue."

**🤖 AI Agent:**
> I've retrieved the available positions. You have active roles such as 'Senior Developer' (ID: pos_123) and 'Sales Lead' (ID: pos_456). Would you like details on a specific one?

---

**👤 You:**
> "Create a candidate: Jane Smith, jane.smith@example.com."

**🤖 AI Agent:**
> Candidate Jane Smith has been created successfully with ID 'cand_789'. I can now help you schedule an interview for her.

---

**👤 You:**
> "Get the details for position pos_123."

**🤖 AI Agent:**
> Fetching details for 'Senior Developer' (pos_123)... This position is active and currently has 12 associated interview templates.


## Installation & Usage

To install and use the **HireVue** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hirevue](https://vinkius.com/mcp/hirevue)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
