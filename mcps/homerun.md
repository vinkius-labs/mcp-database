# Homerun MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/homerun)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/homerun-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/homerun-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate recruitment workflows via Homerun — manage job applications, track candidates, and oversee vacancies directly from any AI agent.

## Description
Connect your **Homerun** account to any AI agent and streamline your hiring process through natural conversation. Manage your entire talent pipeline without switching between tabs.

### What you can do

- **Application Management** — List all job applications with advanced filtering by stage, vacancy, or disqualification status.
- **Candidate Creation** — Create new job applications directly, including personal info, social profiles, and custom data.
- **Detailed Tracking** — Fetch complete metadata for specific applications, including notes, sources, and question answers.
- **Workflow Updates** — Move candidates between stages (e.g., to 'hired') or update application details on the fly.
- **Data Maintenance** — Keep your ATS clean by deleting or updating records as your recruitment process evolves.

### How it works

1. Subscribe to this server
2. Enter your Homerun API Key
3. Start managing your hiring pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Managers** — quickly filter candidates and update hiring stages without opening the full ATS dashboard.
- **Hiring Managers** — retrieve candidate details and notes directly while reviewing technical assessments or preparing for interviews.
- **Operations Leads** — automate the reporting of candidate flows and vacancy statuses across the organization.


## Available Tools
- **create_job_application**: Create a new job application
- **create_job_application_note**: Create a new note on a job application
- **delete_job_application**: Delete a job application
- **get_job_application**: Get detailed information for a job application
- **get_vacancy**: Get detailed vacancy information
- **list_job_applications**: Get a list of job applications
- **list_vacancies**: Get a list of vacancies
- **ping**: Test Homerun API authentication
- **update_job_application**: Update a job application
- **upload_job_application_file**: Upload a file (resume or assignment) to a job application
- **upload_job_application_photo**: Upload an applicant photo to a job application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Homerun** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job applications for vacancy ID 'vac_123'."

**🤖 AI Agent:**
> I've found 3 active applications for that vacancy. Candidates include John Doe (Stage: Review), Jane Smith (Stage: Interview), and Alex Brown (Stage: Review). Would you like to see the details for any of them?

---

**👤 You:**
> "Get the full details for job application 887766, including notes and sources."

**🤖 AI Agent:**
> Fetching details for application 887766... This is for 'Michael Scott'. He was sourced via LinkedIn. There is one note from the recruiter: 'Strong leadership background, highly recommended for the regional manager position'.

---

**👤 You:**
> "Update application 554433: set the stage to 'hired'."

**🤖 AI Agent:**
> Successfully updated application 554433. The candidate has been moved to the 'hired' stage. Would you like me to check if there are any other pending tasks for this vacancy?


## Installation & Usage

To install and use the **Homerun** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/homerun](https://vinkius.com/mcp/homerun)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
