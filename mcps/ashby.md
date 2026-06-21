# Ashby MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ashby)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ashby-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ashby-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage your recruiting pipeline with Ashby — track jobs, candidates, and applications via AI.

## Description
The **Ashby MCP Server** provides a direct natural language interface to your Ashby recruiting platform. Empower your AI agent to manage your hiring pipeline, from job listing analysis to candidate search and application tracking.

### Key Features

- **Job Management** — List all open, closed, and archived jobs, and retrieve detailed metadata for any specific position.
- **Candidate Sourcing** — Search for candidates by name or email and access full profiles, including tags and contact details.
- **Application Tracking** — Monitor the status of job applications and filter by job ID or workflow stage (e.g., Hired, Lead).
- **Interview Oversight** — Retrieve lists of scheduled interviews to stay on top of your recruiting calendar.
- **Search Intelligence** — Use powerful search tools to quickly find the right talent or job openings in your organization.
- **Secure Integration** — Uses secure HTTP Basic Authentication with your Ashby API key.

### Who is this for?

- **Recruiters** — Quickly audit your pipeline and candidate statuses without switching between multiple tabs.
- **Hiring Managers** — Review candidate profiles and job details using AI-assisted summaries during your planning sessions.
- **Talent Ops** — Monitor hiring trends and ensure all applications are being processed efficiently.


## Available Tools
- **get_account_check**: Verify Ashby account connection
- **get_application_info**: Get details for a specific application
- **get_candidate_info**: Get detailed information for a specific candidate
- **get_job_info**: Get detailed information for a specific job
- **list_applications**: List all job applications
- **list_candidates**: List all candidates in Ashby
- **list_interviews**: List all interviews
- **list_jobs**: Supports status filtering.

List all job listings in Ashby
- **search_candidates**: Search for candidates by email or name
- **search_jobs**: Search for jobs by title


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ashby** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all currently opened jobs in Ashby."

**🤖 AI Agent:**
> I've retrieved your open jobs. You have 4 opened positions: 'Senior Frontend Engineer', 'Product Designer', 'Customer Success Manager', and 'Sales Lead'.

---

**👤 You:**
> "Search for a candidate named 'John Doe'."

**🤖 AI Agent:**
> I found 1 candidate matching 'John Doe' (ID: cand_123). He is currently tagged with 'Engineering' and 'Referral'.

---

**👤 You:**
> "Show me the details of application 'app_998877'."

**🤖 AI Agent:**
> Application 'app_998877' is for the 'Senior Frontend Engineer' role. The current status is 'Technical Interview' and it was created on Feb 1st.


## Installation & Usage

To install and use the **Ashby** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ashby](https://vinkius.com/mcp/ashby)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
