# JobScore MCP Server

Manage jobs, candidates, and hiring teams via JobScore ATS API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/jobscore)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Empower your AI agents with JobScore's comprehensive applicant tracking system. This MCP server allows you to list and retrieve job postings, track candidates, manage hiring teams and departments, and view hiring sources directly through the JobScore API. Ideal for automating recruitment workflows and talent acquisition.


## Available Tools
- **get_candidate**: Returns contact history, resume highlights (if available), and current application status. Use this before an interview or when evaluating an applicant.

Retrieves details for a specific candidate
- **get_job**: Includes job descriptions, requirements, and hiring team identifiers. Use this to provide detailed information about a specific opening.

Retrieves details for a specific job
- **get_me**: Use this to verify connection status and identity.

Gets current authenticated user info
- **list_candidates**: Includes candidate names, current stage, and IDs. Essential for monitoring the talent pool and identifying new applications.

Lists all candidates
- **list_departments**: g., Engineering, Marketing) used to categorize jobs in JobScore. Useful for filtering hiring data by business unit.

Lists all departments
- **list_hiring_teams**: Useful for identifying recruiters and hiring managers associated with specific jobs.

Lists all hiring teams
- **list_jobs**: Returns job titles, IDs, and departments. Use this to identify active positions or find a job ID for candidate management.

Lists all jobs in JobScore
- **list_locations**: Useful for understanding the geographical scope of hiring efforts.

Lists all office locations
- **list_sources**: g., "LinkedIn", "Referral", "Job Board") from which candidates are originating. Essential for analyzing the effectiveness of hiring channels.

Lists all candidate sources
- **list_users**: Useful for identifying team members and their roles.

Lists all users in the account


## Installation & Usage

To install and use the **JobScore** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobscore](https://vinkius.com/mcp/jobscore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
