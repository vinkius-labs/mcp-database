# Wizehire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wizehire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wizehire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wizehire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage candidates, job postings, and hiring stages via Wizehire directly from your AI agent.

## Description
Connect your **Wizehire** hiring platform to any AI agent to streamline your recruitment lifecycle and candidate discovery. Wizehire provides a comprehensive ATS for managing applicant pipelines and assessments.

### What you can do

- **Candidate Orchestration** — List applicants and retrieve detailed contact profiles with DISC+ assessment data.
- **Job Oversight** — Monitor active job postings and retrieve technical requirements and descriptions directly.
- **Pipeline Automation** — Move candidates between hiring stages like Interview or Hired via natural conversation.
- **Team Management** — List hiring team members and manage available recruitment stages programmatically.
- **Workflow Intelligence** — Get a comprehensive overview of your active hiring pipelines using natural language.

### How it works

1. Subscribe to this server
2. Enter your Wizehire API Key from your account settings
3. Start managing your recruitment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — quickly retrieve candidate info and screening results without switching tabs.
- **HR Managers** — monitor job posting statuses and hiring progress via natural conversation.
- **Business Owners** — streamline the recruitment process and update candidate stages efficiently.


## Available Tools
- **check_api_health**: Verify Wizehire API connectivity
- **create_new_candidate**: Requires name and email.

Add a new candidate manually
- **get_candidate_details**: Get details for a specific candidate
- **get_job_details**: Get details for a specific job
- **get_current_user**: Get authenticated user profile
- **list_candidates**: List all recruitment candidates
- **list_active_job_postings**: List all active job openings
- **list_office_locations**: List business office locations
- **list_hiring_stages**: List defined hiring stages
- **list_hiring_team**: List hiring managers and team members
- **list_configured_webhooks**: List active webhooks
- **update_candidate_hiring_stage**: g., Interview, Hired).

Move a candidate to a different stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wizehire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active job postings in Wizehire."

**🤖 AI Agent:**
> I've retrieved 3 active job postings, including 'Senior Project Manager' and 'Sales Executive'. Would you like the details for any of them?

---

**👤 You:**
> "Show the latest candidates for the 'Sales Executive' role."

**🤖 AI Agent:**
> Fetching applicants... I've found 5 recent candidates for the Sales Executive role. Notable ones include John Doe (DISC+: High D). Should I pull his full profile?


## Installation & Usage

To install and use the **Wizehire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wizehire](https://vinkius.com/mcp/wizehire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
