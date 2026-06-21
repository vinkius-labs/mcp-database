# Ninehire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ninehire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ninehire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ninehire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Hire smarter with a recruitment platform that posts jobs, screens applicants, and moves the best candidates through your pipeline.

## Description
Connect your **Ninehire** account to any AI agent and take full control of your talent acquisition and applicant tracking orchestration through natural conversation. Ninehire (나인하이어) provides a modern recruitment platform, and this integration allows you to retrieve job metadata, manage candidate profiles, and monitor interview evaluations directly from your chat interface.

### What you can do

- **Job & Requirement Orchestration** — List all active job openings and retrieve detailed requirements programmatically to ensure your hiring roadmap is always synchronized.
- **Applicant & Pipeline Intelligence** — Access and monitor candidate profiles and retrieve detailed application history directly from the AI interface to maintain high-fidelity talent pools.
- **Evaluation & Feedback Control** — List interview scores and comments via natural language to drive better hiring decisions and team alignment.
- **Manual Applicant Ingestion** — Register new applicants and manage department or location metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage recruitment webhooks to ensure your hiring workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Ninehire API Key from your integration settings
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the ATS for candidate updates. Your AI acts as a dedicated recruitment coordinator or HR lead.

### Who is this for?

- **Recruiters & HR Specialists** — quickly retrieve candidate summaries and monitor job performance without switching apps.
- **Hiring Managers** — automate the retrieval of evaluations and track pipeline progress via natural conversation.
- **Growth Teams** — streamline the ingestion of new candidates and monitor organizational hiring health directly within the chat.


## Available Tools
- **check_api_health**: Verify Ninehire API status
- **register_new_applicant**: Requires essential info like name and email.

Add a candidate manually
- **get_applicant_profile**: Get details for a specific candidate
- **get_job_details**: Get details for a specific job
- **get_authenticated_user_info**: Get current account profile
- **list_job_applicants**: List candidates and applicants
- **list_organization_departments**: List company departments
- **list_candidate_evaluations**: Get evaluations for a candidate
- **list_job_postings**: Supports filtering by title, job group, and employment type.

List all job openings
- **list_job_locations**: List hiring locations
- **list_hiring_teams**: List internal hiring teams
- **list_configured_webhooks**: List active webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ninehire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job postings in Ninehire."

**🤖 AI Agent:**
> I've retrieved your jobs. You have 4 active roles including 'Senior Software Engineer' and 'Marketing Lead'. Which one would you like to see applicant counts for?

---

**👤 You:**
> "Show me all candidates who applied for the Senior Developer position."

**🤖 AI Agent:**
> I found 23 applicants for the Senior Developer position (Job ID: j_4821). 8 candidates are in the screening stage, 5 passed the technical assessment, 3 are scheduled for final interviews, and 7 were rejected. The most recent applicant is Elena Vasquez, submitted 2 hours ago.

---

**👤 You:**
> "List all departments and hiring locations configured in my organization."

**🤖 AI Agent:**
> Your organization has 5 departments: Engineering (12 open roles), Marketing (3 open roles), Sales (7 open roles), Design (2 open roles), and Operations (1 open role). Hiring locations include San Francisco (HQ), London, Berlin, and Remote. Engineering has the most active postings across all locations.


## Installation & Usage

To install and use the **Ninehire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ninehire](https://vinkius.com/mcp/ninehire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
