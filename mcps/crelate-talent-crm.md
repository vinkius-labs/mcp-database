# Crelate Talent CRM MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crelate-talent-crm)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/crelate-talent-crm-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/crelate-talent-crm-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to manage candidates, jobs, and client companies directly via the Crelate API.

## Description
Integrate **Crelate**, the specialized recruiting CRM and applicant tracking system (ATS), directly into your AI workflow. Manage your talent pipeline, monitor job orders, and track candidate activities using natural language.

### What you can do

- **Candidate Management** — List, search, and retrieve full profiles for candidates and contacts.
- **Job Tracking** — Monitor open and past job opportunities and their current status.
- **Activity Logging** — Review recent recruiting activities including calls, emails, and internal notes.
- **Client Relationship** — Manage company records and associated client data seamlessly.

### How it works

1. Connect the Crelate integration to your AI assistant.
2. Authorize using your Crelate API Key (found in Settings > API).
3. Optimize your recruiting operations through intuitive conversation.

### Who is this for?

- **Recruiters & Headhunters** — Quickly find candidate details and log notes after interviews.
- **Talent Acquisition Teams** — Monitor job pipeline progress and candidate engagement.
- **Agency Owners** — Get a quick overview of agency-wide activities and job statuses via chat.


## Available Tools
- **create_contact**: Add a new candidate or contact to the database
- **get_contact_notes**: List internal notes for a specific contact
- **get_contact_details**: Get detailed profile for a specific candidate or contact
- **get_job_details**: Get detailed information for a specific job order
- **list_recent_activities**: List recent recruiting activities (calls, emails, notes)
- **list_companies**: List all companies and client records
- **list_contacts**: List all candidate and contact records in Crelate
- **list_jobs**: List open and past job opportunities
- **list_crelate_users**: List internal recruiters and team members
- **search_contacts_by_name**: Search for contacts by name keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crelate Talent CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all candidates who applied for the 'Senior Developer' job."

**🤖 AI Agent:**
> I've found 8 candidates for the 'Senior Developer' position, including 'John Smith' and 'Sarah Jones'. Would you like to see the internal notes for any of them?

---

**👤 You:**
> "Show me the recent activity for candidate 'Sarah Jones'."

**🤖 AI Agent:**
> Sarah Jones had a screening call on April 1st and an interview with the technical lead today. I've also found 2 internal notes regarding her coding test. Should I list the note details?

---

**👤 You:**
> "List all open jobs in the 'Engineering' department."

**🤖 AI Agent:**
> There are currently 4 open jobs in Engineering: 'Full Stack Dev', 'QA Engineer', 'DevOps Specialist', and 'Backend Architect'. Which one would you like to manage?


## Installation & Usage

To install and use the **Crelate Talent CRM** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crelate-talent-crm](https://vinkius.com/mcp/crelate-talent-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
