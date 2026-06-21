# Loopio MCP Server

Connect your Loopio RFP platform to AI — search approved answers, manage proposal projects, and automate questionnaire responses naturally via chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/loopio)

## Overview
**Category:** productivity
**Tools Count:** 8

## Description
Connect your **Loopio** RFP management platform to your AI agent to transform proposal workflows into intelligent, conversational processes.

### What you can do

- **Browse Projects** — List all your active RFPs, RFIs, and security questionnaires. Check progress, due dates, and completion status at a glance.
- **Search the Knowledge Library** — Query your master library of pre-approved answers. Find exactly what you need before drafting new responses.
- **Review Questionnaire Responses** — Fetch individual questions and their current answers from any project. Track what has been answered and what still needs attention.
- **Create New Submissions** — Spin up new RFP projects instantly with name, deadline, company context, and owner assignment.
- **Manage Teams** — List team members to identify who is available for project assignments and collaboration.

### How it works

1. Add this integration to your workspace.
2. Provide your Loopio Access Token from Settings -> API.
3. Chat with your RFP data using Claude, Cursor, or any compatible AI agent.

### Who is this for?

- **Proposal Managers** — ask the agent to search the library for approved answers about 'SOC 2 compliance' and instantly pull them into an active project.
- **Sales Teams** — have the agent list all overdue RFPs, check their completion percentage, and identify which ones need immediate attention.
- **Security & Compliance** — query existing security questionnaire responses to ensure consistency across vendor assessments without reinventing the wheel.


## Available Tools
- **create_submission**: Requires a project name. Optionally accepts a description, company name, due date, project type, and owner ID. The project will be created in "Not Started" status and ready for team collaboration.

Create a new RFP project/submission in Loopio
- **get_project**: Use this to check the state of a specific RFP response.

Get details of a specific Loopio project by ID
- **get_questionnaire_responses**: If no entryId is provided, returns all entries and their current responses. Use this to review what answers have been drafted or finalized for RFP questions.

Get responses for a specific questionnaire entry or all entries in a project
- **list_libraries**: Each stack contains approved Q&A entries organized by category. Use this to discover which knowledge bases are available for searching.

List all library stacks available in Loopio
- **list_projects**: Each project represents an active RFP response or questionnaire. Use this to discover all ongoing and recent response initiatives. Optionally limit results with the limit parameter.

List all Loopio projects (RFPs, RFIs, questionnaires) in your workspace
- **list_questionnaires**: Each entry represents a question from an RFP, RFI, or security questionnaire that needs to be answered. Use this to understand the scope of a project and track which questions have been answered.

List all questionnaire entries (questions) for a specific Loopio project
- **list_team_members**: Use this to identify who is assigned to projects, find user IDs for assigning project ownership, or understand team composition.

List all team members in your Loopio workspace
- **search_library**: This is the primary way to find existing approved responses before drafting new answers. You can refine results with optional filters like tags, category, stack, and whether to search in questions or answers. Always use this before creating new library entries.

Search the Loopio knowledge library for approved Q&A entries


## Installation & Usage

To install and use the **Loopio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loopio](https://vinkius.com/mcp/loopio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
