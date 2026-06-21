# Ashby MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ashby-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ashby-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ashby-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Hire top talent faster with an all-in-one recruiting platform that combines ATS, scheduling, and hiring analytics.

## Description
Connect your **Ashby** account to any AI agent and take full control of your recruiting pipeline and candidate experience through natural conversation.

### What you can do

- **Candidate Orchestration** — List and manage candidate profiles programmatically, including creating new records and retrieving high-fidelity profile metadata
- **Application Lifecycle Management** — Monitor job applications and retrieve detailed status metrics for specific candidates to coordinate your hiring funnel in real-time
- **Interview Intelligence** — Access scheduled interviews and retrieve submitted high-fidelity feedback reports to summarize performance and sentiment
- **Job & Department Visibility** — Retrieve complete directories of open jobs, departments, and hiring managers to maintain a perfectly coordinated organizational view
- **User & Location Monitoring** — Access your internal recruiter directory and physical office locations directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from the Ashby dashboard (Admin > API Keys)
3. Start managing your talent pipeline from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to check a candidate's status or feedback. Your AI acts as your dedicated talent coordinator and recruiting architect.

### Who is this for?

- **Recruiters & Sourcers** — instantly retrieve candidate summaries and update application stages using natural language commands
- **Hiring Managers** — check interview feedback and pipeline health across departments without leaving your creative workspace
- **HR Operations** — automate the oversight of job postings and user permissions through simple AI queries


## Available Tools
- **create_ashby_candidate**: Create candidate
- **get_ashby_application**: Get application details
- **get_ashby_candidate**: Get candidate details
- **get_ashby_job**: Get job details
- **list_ashby_applications**: List applications
- **list_ashby_candidates**: List candidates
- **list_ashby_feedback**: List feedback
- **list_ashby_interviews**: List interviews
- **list_ashby_jobs**: List jobs
- **list_ashby_users**: List users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ashby** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active candidates in my Ashby recruiting pipeline."

**🤖 AI Agent:**
> I've retrieved your candidate directory. You currently have 12 active candidates, including @user1 and @user2. Would you like to see the application status for a specific person?

---

**👤 You:**
> "Show the latest interview feedback for candidate ID 'cand_123'."

**🤖 AI Agent:**
> Fetching feedback records... For candidate cand_123, the last interview report from @user3 highlights strong technical skills and a 'Recommend' rating. Need the high-fidelity detailed summary?

---

**👤 You:**
> "Create a new candidate profile for 'Jane Smith' (jane@example.com)."

**🤖 AI Agent:**
> Candidate created! Jane Smith has been successfully added to your Ashby account (ID: cand_456). She is now available for job linking and interview scheduling. Shall I list your open jobs for her?


## Installation & Usage

To install and use the **Ashby** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ashby-alternative](https://vinkius.com/mcp/ashby-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
