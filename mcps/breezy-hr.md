# Breezy HR MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/breezy-hr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/breezy-hr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/breezy-hr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your recruitment process via Breezy HR — track candidates, positions, and stages directly from any AI agent.

## Description
Connect your **Breezy HR** account to any AI agent and orchestrate your hiring and candidate management workflows through natural conversation.

### What you can do

- **Position Oversight** — List and retrieve detailed metadata for all your active and draft job positions.
- **Candidate Management** — Create new candidate profiles, move them through your pipeline, and retrieve full applicant histories.
- **Pipeline Coordination** — List and monitor stages for specific positions to ensure a smooth hiring flow.
- **Administrative Access** — Retrieve company information and task templates straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Breezy HR API Key and Company ID
3. Start managing your talent acquisition from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Leads** — quickly check candidate statuses and move applicants without manual dashboard work.
- **Hiring Managers** — retrieve position details and applicant lists straight from their editor.
- **Talent Ops** — monitor hiring pipelines and task templates using natural language.


## Available Tools
- **create_candidate**: Add a candidate to a position
- **create_position**: Create a new job position
- **get_candidate**: Get specific candidate details
- **get_company**: Get details of the authenticated company
- **get_position**: Get details of a specific position
- **list_candidates**: List candidates for a specific position
- **list_positions**: List all job positions
- **list_stages**: List pipeline stages for a position
- **list_task_templates**: List available task templates
- **move_candidate**: Move a candidate to a different pipeline stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breezy HR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job positions in Breezy HR."

**🤖 AI Agent:**
> I've retrieved your positions. You have 3 active jobs: 'Senior Developer' (ID: pos_1), 'Product Manager' (ID: pos_2), and 'Sales Exec' (ID: pos_3).

---

**👤 You:**
> "Show the candidates for the 'Senior Developer' role."

**🤖 AI Agent:**
> Retrieving candidates for 'Senior Developer'... I found 5 applicants, including John Doe (Applied) and Sarah Smith (Sourced). Which one would you like to inspect?

---

**👤 You:**
> "Move candidate cand_123 to the 'Interview' stage."

**🤖 AI Agent:**
> Candidate cand_123 has been successfully moved to the 'Interview' stage in your Breezy HR pipeline.


## Installation & Usage

To install and use the **Breezy HR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/breezy-hr](https://vinkius.com/mcp/breezy-hr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
