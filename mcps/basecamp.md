# Basecamp MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/basecamp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/basecamp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/basecamp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your Basecamp projects via AI — list tasks, read message boards, track campfire logs, and orchestrate to-dos seamlessly.

## Description
Connect your **Basecamp** account to any AI agent and track team productivity, tasks, and communications through natural conversation.

### O que você pode fazer

- **Project Navigation** — List active projects, map exact internal UUIDs, and discover complete team structures
- **To-Do Lists** — Access Todosets, examine explicit todolists, and track individual pending tasks instantly
- **Message Boards** — Paginate through team announcements extracting conversation metadata reliably
- **Campfire Logs** — Retrieve recent interactive chat lines from project Campfire modules securely
- **People Directory** — Enumerate entire organizational team profiles tracking accurate author histories

### Como funciona

1. Subscribe to this server
2. Enter your Basecamp Access Token and Account ID
3. Gain full remote insights into your projects and to-dos via Claude or Cursor

Keep your work centralized and allow your AI agent to fetch updates or summarize backlogs without opening complex web interfaces.

### Para quem é?

- **Project Managers** — gather immediate daily task digests and campfire chatter summaries from multiple projects simultaneously
- **Development Teams** — search unresolved bug todolists while writing code inside the IDE naturally
- **Agency Owners** — monitor client project health, list overdue tasks, and track assignee distributions globally


## Available Tools
- **list_projects**: List active Basecamp projects
- **get_project**: Get a specific Basecamp project
- **list_todolists**: List Basecamp todolists inside a todoset
- **list_todos**: List todos inside a specific todolist
- **list_messages**: List messages on a project message board
- **list_campfire_lines**: List recent chat lines from a project Campfire
- **list_people**: List all people in the Basecamp account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Basecamp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the latest message board posts in the 'Website Redesign' project?"

**🤖 AI Agent:**
> I found 2 recent messages on the board. 1. 'Final CSS Delivery' by Anna M. (with 3 comments). 2. 'DNS Blockers' by David (with 0 comments). Shall I fetch the Campfire logs as well?

---

**👤 You:**
> "List all pending todos on the 'Launch Day' todolist."

**🤖 AI Agent:**
> You have 4 unfinished todos tracking under Launch Day. 1. Deploy Vinkius Cluster 2. Setup Stripe Billing (Assigned: Sarah) 3. Finalize README. They are active and awaiting resolution natively.

---

**👤 You:**
> "Can you summarize the active projects our team is working on?"

**🤖 AI Agent:**
> I've pulled the Basecamp hierarchy. You have 3 primary explicit team projects: 'Mobile MVP 2026', 'Accounting Integration', and 'HQ General Ops'. Would you like the people directory mapping their team memberships?


## Installation & Usage

To install and use the **Basecamp** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/basecamp](https://vinkius.com/mcp/basecamp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
