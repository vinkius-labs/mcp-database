# Firefish MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/firefish)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/firefish-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/firefish-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage candidates, jobs, and companies through AI agents with Firefish Recruitment CRM.

## Description
Connect your **Firefish** account to any AI agent and automate your recruitment workflows through the Model Context Protocol (MCP). Firefish is a high-performance recruitment CRM that empowers agencies to reach more candidates and close more placements. Now, you can interact with your recruitment data directly through natural conversation.

### What you can do

- **Candidate Management** — List all candidates, fetch detailed profiles, and create new candidate records instantly.
- **Job Tracking** — Monitor active job vacancies and retrieve complete metadata for any job in your system.
- **Company & Contact Insights** — Access your database of client companies and contacts to stay informed before meetings or calls.
- **Placement Monitoring** — Keep track of successful job placements and recruitment progress across your team.
- **Advertising Overview** — List active job advertisements to see where your recruitment efforts are focused.
- **Activity Actions** — Retrieve a list of recent recruiter actions to maintain a clear audit trail of engagement.
- **Seamless Integration** — Securely connect your Firefish environment using your Client ID and Secret for an automated experience.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Firefish Client ID and Secret (found in Settings > Integrations)
3. Start managing your recruitment CRM data from Claude, Cursor, or any MCP client

### Who is this for?

- **Recruiters & Headhunters** — quickly pull candidate details or job specs while discussing requirements with hiring managers.
- **Talent Acquisition Managers** — get a bird's-eye view of active placements and job adverts through simple AI commands.
- **Recruitment Agency Owners** — automate the retrieval of recruiter actions and company data for performance reviews.


## Available Tools
- **create_candidate**: Create a new candidate
- **get_candidate**: Get candidate details
- **get_company**: Get company details
- **get_contact**: Get contact details
- **get_job**: Get job details
- **list_actions**: List actions
- **list_adverts**: List job adverts
- **list_candidates**: List candidates
- **list_companies**: List companies
- **list_contacts**: List contacts
- **list_jobs**: List jobs
- **list_placements**: List placements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Firefish** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job vacancies at Firefish."

**🤖 AI Agent:**
> Fetching jobs... I found 5 active job vacancies, including 'Senior Software Engineer' and 'Recruitment Consultant'. Would you like the full details for any of these?

---

**👤 You:**
> "Search for a candidate named 'John Smith'."

**🤖 AI Agent:**
> Searching candidates... I found a profile for John Smith (ID: cand_456) with status 'Active'. He is currently listed as a 'Project Manager'.

---

**👤 You:**
> "Show me the most recent recruiter actions."

**🤖 AI Agent:**
> Retrieving actions... Here are the latest actions recorded, including 'Email Sent to Candidate cand_123' and 'Interview Scheduled for Job job_789'.


## Installation & Usage

To install and use the **Firefish** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/firefish](https://vinkius.com/mcp/firefish)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
