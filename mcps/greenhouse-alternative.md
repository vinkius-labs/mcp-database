# Greenhouse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/greenhouse-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/greenhouse-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/greenhouse-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Hire the right people with structured interviewing, customizable pipelines, and data-driven recruiting that scales with your team.

## Description
Connect your **Greenhouse** account to any AI agent and take full control of your hiring pipeline and recruitment workflows through natural conversation.

### What you can do

- **Candidate Orchestration** — List and manage candidate records programmatically, including contact info, current company, and professional titles
- **Application Lifecycle** — Monitor job applications and take immediate action by advancing candidates to the next stage or marking rejections with reasons
- **Job Management** — Access detailed metadata for all active job openings, including hiring teams and department structures
- **Organizational Visibility** — Retrieve complete company department lists and office locations to coordinate recruitment logistics
- **System Monitoring** — Check API connectivity and Harvest API status directly through your agent for reliable data operations

### How it works

1. Subscribe to this server
2. Retrieve your **Harvest API Key** from Greenhouse (Configure > Dev Center > API Credential Management)
3. Note a valid **User ID** to perform actions 'On-Behalf-Of' for auditing purposes
4. Start managing your talent acquisition from Claude, Cursor, or any MCP client

No more manual status updates or digging through candidates in the ATS. Your AI acts as your dedicated recruitment coordinator.

### Who is this for?

- **Recruiters & Sources** — instantly identify candidate statuses and advance top talent through the pipeline using natural language
- **Hiring Managers** — retrieve job opening details and department structures without leaving your planning tools
- **HR Operations** — manage office locations and department organization through automated queries


## Available Tools
- **advance_application**: Move candidate to next stage
- **create_candidate**: Can include first name, last name, and company.

Add new candidate
- **get_api_status**: Get account connectivity
- **get_candidate_details**: Get candidate info
- **get_job_details**: Get job metadata
- **list_applications**: List job applications
- **list_candidates**: List recruitment candidates
- **list_departments**: List company departments
- **list_open_jobs**: List active job openings
- **list_offices**: List office locations
- **reject_application**: Requires a reason ID.

Reject job application
- **update_candidate**: Modify candidate info


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Greenhouse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find candidate with email 'candidate@example.com' and show their status."

**🤖 AI Agent:**
> I've located the candidate record for 'candidate@example.com' (ID: can_123). They are currently in the 'Technical Interview' stage for the 'Senior Engineer' role. Would you like to see their feedback history?

---

**👤 You:**
> "List all active job openings for the 'Engineering' department."

**🤖 AI Agent:**
> Scanning jobs... I found 5 active openings in Engineering: 'Full Stack Dev' (ID: job_401), 'Site Reliability Engineer' (ID: job_402), and 3 others. Which one should I provide details for?

---

**👤 You:**
> "Advance application ID 'app_987' to the next stage."

**🤖 AI Agent:**
> Action complete! Application 'app_987' has been advanced to the 'Onsite Interview' stage. The hiring team has been notified of the stage change in Greenhouse.


## Installation & Usage

To install and use the **Greenhouse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/greenhouse-alternative](https://vinkius.com/mcp/greenhouse-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
