# Lever MCP Server

Manage recruitment postings, candidate opportunities, and hiring stages via the Lever API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/lever)

## Overview
**Category:** human-resources
**Tools Count:** 10

## Description
Connect your **Lever** account to any AI agent to streamline your recruitment and talent acquisition workflows. This MCP server enables your agent to interact with job postings, manage candidate opportunities, and move applications through your hiring pipeline directly.

### What you can do

- **Posting Oversight** — List and retrieve detailed configurations for all your active job advertisements
- **Opportunity Management** — Manage candidate applications (Opportunities), track their status, and move them through hiring stages
- **Candidate Insight** — Access complete candidate profiles, contact details, and interaction histories
- **Pipeline Control** — List hiring stages and automate the archiving of applications with specific reasons
- **Workflow Automation** — Create new job postings or candidate records directly from natural language interfaces

### How it works

1. Subscribe to this server
2. Enter your Lever API Key
3. Start managing your hiring pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & Sourcers** — Quickly update candidate statuses and job notes without leaving your development environment
- **Hiring Managers** — Monitor the progress of applicants for specific roles via natural language commands
- **HR Operations** — Automate the creation of job drafts and maintain clean recruitment data effortlessly


## Available Tools
- **archive_hiring_opportunity**: Archive a candidate opportunity
- **create_hiring_opportunity**: Requires a JSON body with opportunity details.

Create a new candidate opportunity
- **create_job_posting**: Requires a JSON body with posting details.

Create a new job posting
- **get_candidate_profile**: Get details for a specific candidate (person)
- **get_opportunity_details**: Get details for a specific candidate opportunity
- **get_posting_details**: Get details for a specific job posting
- **list_hiring_opportunities**: List all candidate opportunities (applications)
- **list_job_postings**: List all job postings
- **list_hiring_stages**: g., Screen, Interview) configured in your Lever account.

List all defined hiring pipeline stages
- **update_opportunity_stage**: g., move to "Interview" or "Offer").

Move a candidate to a different hiring stage


## Installation & Usage

To install and use the **Lever** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/lever](https://vinkius.com/mcp/lever)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
