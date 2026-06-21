# Jobvite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jobvite)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/jobvite-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/jobvite-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your recruitment pipeline via Jobvite — list candidates, track job requisitions, and update application statuses directly from any AI agent.

## Description
Connect your **Jobvite** account to any AI agent to streamline your hiring process. Manage candidates, job postings, and applications through natural conversation.

### What you can do

- **Candidate Management** — List, retrieve, create, and update candidate profiles with ease.
- **Job Requisitions** — Access active job listings, view detailed job information, and create new requisitions.
- **Application Tracking** — Monitor candidate progress through the hiring workflow and update application statuses instantly.

### How it works

1. Subscribe to this server
2. Enter your Jobvite API Key and API Secret
3. Start managing your recruitment workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — quickly check candidate details and update hiring stages without switching tabs.
- **Hiring Managers** — review job requisitions and candidate profiles directly from their workspace.
- **HR Operations** — automate the creation of candidate records and job postings.


## Available Tools
- **create_candidate**: Create a new Jobvite candidate profile
- **create_job**: Create a new Jobvite job requisition
- **get_candidate**: Get details for a specific Jobvite candidate
- **get_job**: Get detailed information about a specific Jobvite job
- **list_applications**: List Jobvite applications
- **list_candidates**: List Jobvite candidates
- **list_jobs**: List all active Jobvite job requisitions
- **update_application_status**: Update the workflow status of a Jobvite application
- **update_candidate**: Update an existing Jobvite candidate


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jobvite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job requisitions in Jobvite."

**🤖 AI Agent:**
> I've retrieved the active jobs. You have 3 open positions: 'Senior Software Engineer' (ID: j101), 'Product Manager' (ID: j102), and 'UX Designer' (ID: j103). Would you like more details on any of these?

---

**👤 You:**
> "Show me the details for candidate ID 'c5501'."

**🤖 AI Agent:**
> Fetching candidate details... Candidate 'Jane Doe' (ID: c5501) is currently in the 'Interview' stage. Her contact info is jane.doe@example.com. Would you like to update her status or see her application history?

---

**👤 You:**
> "Update the status of application 'app_99' to 'Hired'."

**🤖 AI Agent:**
> Processing update... The application 'app_99' has been successfully updated to 'Hired'. The candidate record and hiring pipeline have been synchronized.


## Installation & Usage

To install and use the **Jobvite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobvite](https://vinkius.com/mcp/jobvite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
