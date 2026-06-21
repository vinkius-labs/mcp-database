# Workable MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workable)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/workable-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/workable-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recruit top talent with an ATS that posts to 200+ job boards, screens candidates with AI, and manages the entire hiring flow.

## Description
Connect your **Workable** recruiting account to any AI agent and simplify how you manage your hiring pipelines, track candidates, and coordinate with your team through natural conversation.

### What you can do

- **Job Management** — List all active and archived job openings and retrieve detailed job descriptions and requirements.
- **Candidate Tracking** — List and inspect candidates across all jobs, and drill down into specific profiles for experience and status.
- **Direct Sourcing** — Programmatically register new candidates to specific job openings to accelerate your hiring process.
- **Team Coordination** — List account members and recruiters to understand your hiring team structure.
- **Ecosystem Overview** — List linked accounts and verify your Workable instance configuration via AI.

### How it works

1. Subscribe to this server
2. Enter your Workable Subdomain and API Key
3. Start managing your recruitment machine from Claude, Cursor, or any MCP client

### Who is this for?

- **Recruiters & HR Managers** — quickly check candidate statuses and job metadata via simple AI queries.
- **Hiring Managers** — monitor the progress of specific pipelines and review new applicants without opening the dashboard.
- **Operations Teams** — automate candidate registration and track team activity levels directly from the workspace.


## Available Tools
- **create_candidate**: Register a new candidate to a job
- **get_candidate_profile**: Get details for a specific candidate
- **get_job_details**: Get details for a specific job
- **list_linked_accounts**: List connected accounts
- **list_all_candidates**: List candidates across all jobs
- **list_jobs**: List active job openings
- **list_account_members**: List hiring team members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job openings in our Workable account."

**🤖 AI Agent:**
> I've retrieved your active jobs. You have 4 openings: 'Senior Frontend Engineer', 'Product Designer', 'DevOps Specialist', and 'Marketing Lead'. Which one would you like to see the details for?

---

**👤 You:**
> "Show me the details for the candidate 'John Smith'."

**🤖 AI Agent:**
> I've fetched John Smith's profile. He is currently in the 'Interview' stage for the 'Senior Frontend Engineer' role. He has 8 years of experience and is marked as 'Highly Recommended'.

---

**👤 You:**
> "Add 'Jane Doe' (jane.doe@example.com) as a candidate for the job 'ENG-101'."

**🤖 AI Agent:**
> Success! Jane Doe has been registered as a new candidate for job 'ENG-101' (shortcode: senior-frontend). I've added her email and initiated the application process.


## Installation & Usage

To install and use the **Workable** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workable](https://vinkius.com/mcp/workable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
