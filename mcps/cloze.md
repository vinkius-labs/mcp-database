# Cloze MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloze)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cloze-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cloze-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Smart CRM that automatically tracks your interactions and provides AI-powered insights.

## Description
Cloze is a smart CRM that automatically tracks your interactions and provides AI-powered insights to manage your relationships, projects, and deals. Through this MCP server, your AI agent can effortlessly pull contact histories, lookup custom tags, verify relationship strengths, and update ongoing project states without breaking your workflow.


## Available Tools
- **create_person**: Provide at least name or email.

Create a new person in Cloze
- **create_project**: Create a new project, deal, or property in Cloze
- **get_person**: Retrieve detailed information about a specific person by email
- **list_companies**: Retrieve a list of companies from Cloze
- **list_custom_fields**: Retrieve definitions for custom fields in your Cloze account
- **list_people**: Retrieve a list of people (contacts) from Cloze
- **list_projects**: Retrieve a list of projects, properties, or deals from Cloze
- **search_people_by_tag**: Find contacts that have a specific tag
- **update_person**: Email is used as the match key.

Update an existing person in Cloze (matching by email)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cloze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get all details for the person with email 'sarah@example.com' in Cloze."

**🤖 AI Agent:**
> Contact found: Sarah Johnson (sarah@example.com). Company: TechStart Inc. Stage: Active Lead. Last interaction: March 20, 2025. Score: 85/100. Tags: VIP, Enterprise. Open deals: 2 ($45,000 total pipeline).

---

**👤 You:**
> "Show me my active projects in Cloze."

**🤖 AI Agent:**
> You have 5 active projects:
1. Website Redesign — Due: April 15 (3 tasks remaining)
2. Q2 Marketing Campaign — Due: May 1 (7 tasks)
3. CRM Migration — Due: April 30 (12 tasks)
4. Sales Training — Due: April 10 (1 task)
5. Product Launch — Due: June 1 (15 tasks)

---

**👤 You:**
> "Find all contacts tagged with 'VIP' in Cloze."

**🤖 AI Agent:**
> Found 8 contacts tagged 'VIP':
1. Sarah Johnson — TechStart Inc. (Score: 85)
2. David Chen — FinServe Ltd. (Score: 92)
3. Maria Garcia — CloudFirst (Score: 78)
... Showing 3 of 8. Combined pipeline value: $320,000.


## Installation & Usage

To install and use the **Cloze** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloze](https://vinkius.com/mcp/cloze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
