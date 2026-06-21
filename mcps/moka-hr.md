# Moka HR MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moka-hr)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/moka-hr-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/moka-hr-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Intelligent applicant tracking system (ATS) — manage jobs, candidates, and interviews via AI.

## Description
Empower your AI agent to orchestrate your recruitment lifecycle with **Moka HR**, the premier applicant tracking system for modern high-growth companies. By connecting Moka to your agent, you transform complex candidate tracking, job management, and interview coordination into a natural conversation. Your agent can instantly list open positions, retrieve candidate profiles, monitor interview schedules, and even provide recruitment summaries without you needing to navigate the complex Moka dashboard. Whether you are a hiring manager or a recruiter, your agent acts as a real-time talent assistant, keeping your hiring pipeline organized and your recruitment process efficient.

### What you can do

- **Job Orchestration** — List all active job postings and retrieve detailed requirements for any position.
- **Candidate Management** — Browse recruitment pipelines and manage candidate profiles, including contact details and history.
- **Interview Tracking** — Monitor scheduled interviews and retrieve session details instantly.
- **Application Control** — Manage the relationship between candidates and specific job applications.
- **Hiring Insights** — Retrieve high-level summaries of recruitment activity and pipeline statistics.

### How it works

1. Subscribe to this server
2. Enter your Moka API Key
3. Start managing your recruitment workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — track candidate progress and manage job postings through natural language queries.
- **Hiring Managers** — monitor interview schedules and review candidate details directly from your AI-powered workspace.
- **HR Operations** — oversee multiple recruitment pipelines and audit activity summaries across the organization.
- **Moka Power Users** — integrate your existing recruitment workflows into your AI-driven daily routines.


## Available Tools
- **create_candidate**: Add new candidate
- **get_application**: Get application details
- **get_candidate**: Get candidate details
- **get_hiring_summary**: Get recruitment summary
- **get_interview**: Get interview details
- **get_job**: Get job details
- **list_applications**: List job applications
- **list_candidates**: List candidates
- **list_interviews**: List scheduled interviews
- **list_jobs**: List open job positions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moka HR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open job positions in our organization."

**🤖 AI Agent:**
> I've retrieved the active job postings from Moka. You have 8 open positions, including 'Senior Frontend Engineer' and 'Product Marketing Manager'. Would you like to see the details for any of them?

---

**👤 You:**
> "Show me the recruitment pipeline for candidate 'Mario'."

**🤖 AI Agent:**
> I've found candidate Mario in the system. He is currently in the 'Technical Interview' stage for the 'Backend Developer' position. His last interaction was a coding test review yesterday.

---

**👤 You:**
> "Get a summary of our hiring activity for this month."

**🤖 AI Agent:**
> I've compiled the monthly hiring summary. You've received 150 new applications, scheduled 42 interviews, and made 5 offers. The conversion rate from interview to offer is currently 12%. Would you like a breakdown by department?


## Installation & Usage

To install and use the **Moka HR** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moka-hr](https://vinkius.com/mcp/moka-hr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
