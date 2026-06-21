# LiftedWork MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/liftedwork)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/liftedwork-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/liftedwork-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Connect job seekers with employment opportunities through a platform that matches skills to openings and tracks applications.

## Description
Connect your **LiftedWork** account to any AI agent and manage staffing through natural conversation.

### What you can do

- **Candidate Management** — Browse candidates, inspect profiles, and track status
- **Placement Tracking** — Monitor active placements and contract details
- **Job Listings** — List open positions and their requirements

### How it works

1. Subscribe to this server
2. Enter your LiftedWork API Key
3. Start managing staffing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — manage candidate pipelines and placements
- **HR Teams** — track open positions and applications
- **Staffing Agencies** — monitor active placements


## Available Tools
- **create_project**: Create a new project
- **create_task**: Pass task data as a JSON string.

Create a new task
- **list_clients**: List all clients
- **list_projects**: List all projects
- **list_tasks**: List all agency tasks
- **list_time_entries**: List all time tracking entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LiftedWork** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show open positions and candidate pipeline status."

**🤖 AI Agent:**
> Open positions: 8. 'Senior Developer' (12 applicants), 'UX Designer' (8), 'Project Manager' (15), 'DevOps Engineer' (6), 4 others. Pipeline: 45 total candidates. New (12), Screening (8), Interview (10), Offer (5), Placed (10). Avg time-to-fill: 28 days.

---

**👤 You:**
> "Show candidates for the Senior Developer role."

**🤖 AI Agent:**
> Senior Developer: 12 applicants. Interview stage: 4. Sarah Chen (5 yrs, Python/React, ⭐ top match). Mike Torres (7 yrs, Java/Angular). Lisa Park (4 yrs, Node/Vue). James Lee (6 yrs, Go/React). Screening: 3. New: 5. Offer pending: 0.

---

**👤 You:**
> "Show active placements and contract details."

**🤖 AI Agent:**
> Active placements: 10. Contract: 6, Permanent: 4. By client: Acme Corp (3), TechCo (2), Others (5). Ending within 30 days: 2. 'Ana Costa at Acme' (contract, ends May 15). 'David Kim at TechCo' (contract, ends May 20). Revenue this quarter: $45K.


## Installation & Usage

To install and use the **LiftedWork** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/liftedwork](https://vinkius.com/mcp/liftedwork)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
