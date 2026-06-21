# BrightMove MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brightmove)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brightmove-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brightmove-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your hiring pipeline via BrightMove — track jobs, applicants, and references directly from any AI agent.

## Description
Connect your **BrightMove ATS** account to any AI agent and orchestrate your recruitment, talent acquisition, and applicant tracking workflows through natural conversation.

### What you can do

- **Job Oversight** — List all job postings and retrieve detailed requirements and metadata for each role.
- **Applicant Management** — List all candidates in your system and retrieve detailed profiles, including contact info and status.
- **Reference Auditing** — Retrieve and verify references for specific applicants to ensure high-quality hiring.
- **Placement Tracking** — Monitor job placements and recruitment activities across your organization.
- **Team & Company Coordination** — Access core company info and list user accounts managed within the ATS.
- **Dashboard Insights** — Retrieve high-level recruitment metrics directly from your workspace.

### How it works

1. Subscribe to this server
2. Enter your BrightMove Company API Key and User API Key
3. Start managing your talent pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & Sourcers** — quickly find candidate details and check job statuses without manual dashboard work.
- **Hiring Managers** — retrieve applicant lists and reference data straight from their workflow tools.
- **Talent Ops** — monitor placements and activity logs using natural language.


## Available Tools
- **get_applicant**: Get specific applicant details
- **get_company_info**: Retrieve core company information
- **get_recruitment_dashboard**: Retrieve high-level recruitment dashboard data
- **get_job**: Get details of a specific job
- **list_activities**: List recruitment activities
- **list_applicants**: List all applicants/candidates
- **list_jobs**: List all job postings
- **list_placements**: List job placements
- **list_references**: List references for a specific applicant
- **list_user_accounts**: List user accounts in the company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BrightMove** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs in BrightMove."

**🤖 AI Agent:**
> I've retrieved your jobs. You have 3 active postings: 'Senior Java Developer' (ID: job_1), 'Customer Success Manager' (ID: job_2), and 'Accountant' (ID: job_3).

---

**👤 You:**
> "Show the profile for applicant with GUID 12345-abcde."

**🤖 AI Agent:**
> I've found the profile for Jane Smith. She is currently in the 'Interview' stage for the 'Accountant' role. Her contact email is jane.smith@example.com.

---

**👤 You:**
> "List the references for applicant Jane Smith."

**🤖 AI Agent:**
> Retrieving references for Jane Smith... I found 2 references: John Miller (Manager at TechCorp) and Sarah Wilson (HR Director at Global Solutions).


## Installation & Usage

To install and use the **BrightMove** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brightmove](https://vinkius.com/mcp/brightmove)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
