# Kombo MCP Server

Unified API for HRIS, ATS, and LMS — manage employees, job openings, and training courses across 50+ platforms through a single interface.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/kombo)

## Overview
**Category:** human-resources
**Tools Count:** 21

## Description
Connect your entire HR and recruitment stack to any AI agent using **Kombo**. This server provides a unified interface to interact with HRIS, ATS, and LMS systems, allowing you to manage the entire employee lifecycle through natural conversation.

### What you can do

- **HRIS Management** — Retrieve employee records, track absences (vacation/sick leave), and list organizational groups or locations.
- **Recruitment (ATS)** — Query job openings, manage candidate profiles, and track applications or interview stages across different providers.
- **Learning & Training (LMS)** — List available courses, manage user enrollments, and sync training data in bulk.
- **Assessments** — Handle assessment packages and update order results directly from your agent.
- **Unified Access** — Use a single API key to interact with multiple integrations without worrying about individual provider schemas.

### How it works

1. Subscribe to this server
2. Enter your Kombo API Key
3. (Optional) Provide a specific Integration ID to target a connection
4. Start managing your workforce data from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Operations** — quickly pull employee lists or absence reports without logging into multiple HR portals.
- **Recruiters** — check job statuses and candidate details directly from your workflow tools.
- **L&D Managers** — monitor course catalogs and user progress across learning platforms.


## Available Tools
- **put_assessment_order_result**: Write back results for an assessment order
- **put_assessment_packages**: Define available assessment/background check packages
- **get_ats_applications**: Retrieve job applications from the ATS
- **get_ats_candidates**: Retrieve candidate profiles from the ATS
- **create_ats_application**: Create a new application and candidate for a job
- **get_ats_interviews**: List scheduled interviews from the ATS
- **get_ats_jobs**: Retrieve all job openings from the ATS
- **get_ats_rejection_reasons**: List reasons for rejecting applications in the ATS
- **get_ats_roles**: List system and job roles in the ATS
- **get_ats_users**: List ATS users (recruiters, hiring managers)
- **get_hris_absence_types**: List available absence types in the HRIS
- **get_hris_absences**: Retrieve employee absences (vacation, sick leave, etc.)
- **create_hris_employee_form**: Create an employee using a tool-specific form
- **get_hris_employees**: Supports pagination and filtering.

Retrieve all employees from the HRIS
- **get_hris_groups**: Retrieve organizational groups (teams, departments)
- **get_hris_legal_entities**: List legal entities in the HRIS
- **get_hris_locations**: List work locations in the HRIS
- **get_lms_courses**: Retrieve available courses from the LMS
- **upsert_lms_courses_bulk**: Asynchronously upsert courses into the LMS
- **get_lms_users**: Retrieve learners from the LMS
- **passthrough_request**: Call the native API of the underlying tool directly


## Installation & Usage

To install and use the **Kombo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kombo](https://vinkius.com/mcp/kombo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
