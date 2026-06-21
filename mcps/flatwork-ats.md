# Flatwork ATS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/flatwork-ats)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/flatwork-ats-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/flatwork-ats-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Streamline your hiring pipeline with an applicant tracking system that organizes candidates, interviews, and offer management.

## Description
Connect your **Flatwork ATS** account to any AI agent and take full control of your recruitment pipeline and candidate management workflows through natural conversation.

### What you can do

- **Job Orchestration** — List all open and closed job postings and retrieve detailed metadata, including hiring teams and job requirements programmatically
- **Candidate Tracking** — Manage your complete directory of applicants and retrieve detailed profiles and contact information programmatically
- **Application Lifecycle** — Monitor active job applications and update candidate hiring stages (Interview, Hired, Rejected) directly through your agent
- **Applicant Discovery** — Programmatically create new candidates in the system using external data to automate your sourcing pipeline
- **System Monitoring** — List configured webhooks to understand real-time data flows and ensure high-fidelity synchronization with your HR tools

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from Flatwork ATS (Settings > API)
3. Start managing your hiring pipeline from Claude, Cursor, or any MCP client

No more manual status checking or digging through candidate lists. Your AI acts as your dedicated talent acquisition and recruitment coordinator.

### Who is this for?

- **Recruiters & HR Managers** — instantly check application statuses and update hiring stages using natural language commands
- **Talent Acquisition Teams** — automate candidate registration from external sources and monitor job posting activity without leaving your workspace
- **Hiring Managers** — retrieve candidate profiles and job details through simple AI queries to prepare for interviews


## Available Tools
- **create_applicant**: Pass applicant data as a JSON string.

Add a new candidate
- **get_applicant**: Get applicant details
- **get_job**: Get job details
- **list_applicants**: List all applicants/candidates
- **list_applications**: List all job applications
- **list_jobs**: List all job postings
- **list_webhooks**: List configured webhooks
- **update_application_status**: Update application hiring stage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flatwork ATS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job postings in Flatwork ATS."

**🤖 AI Agent:**
> I've retrieved your job postings. You have 3 active positions: 'Senior Full Stack Engineer' (ID: 101), 'Product Designer' (ID: 102), and 'Marketing Lead' (ID: 103). Which one would you like to see applicants for?

---

**👤 You:**
> "Add 'John Doe' (john.doe@example.com) as a new applicant."

**🤖 AI Agent:**
> Candidate created! John Doe has been successfully added to your Flatwork database with ID 'cand_456'. Would you like to link him to an active job application now?

---

**👤 You:**
> "Move application ID 'app_987' to the 'Interview' stage."

**🤖 AI Agent:**
> Hiring stage updated! Application 'app_987' has been moved to 'Interview'. The candidate and hiring team have been notified of the stage change in the system.


## Installation & Usage

To install and use the **Flatwork ATS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/flatwork-ats](https://vinkius.com/mcp/flatwork-ats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
