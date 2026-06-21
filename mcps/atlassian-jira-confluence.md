# Atlassian (Jira & Confluence) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/atlassian-jira-confluence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/atlassian-jira-confluence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/atlassian-jira-confluence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The ultimate AI bridge for Jira and Confluence — manage projects, agile boards, and wikis via AI.

## Description
Transform your **Atlassian Jira** and **Confluence** instance into a conversational command center for your AI agent. This integration bridges the gap between complex agile workflows and actionable intelligence, allowing your agent to audit Jira issues, manage active sprints, and retrieve deep knowledge from Confluence wikis through natural language. Whether you're tracking a bug's lifecycle or auditing enterprise documentation, your agent acts as a direct, real-time navigator across your Atlassian ecosystem, ensuring your team stays aligned and data-driven without manual dashboard hopping.

### What you can do

- **Jira Issues & Search** — Search issues using complex JQL, view exact tickets, or manage epics and stories seamlessly through your agent.
- **Agile Boards & Sprints** — List active boards, explore historical sprints, and get an overarching view of project health effortlessly.
- **Confluence Wikis & Pages** — Search across enterprise documentation using CQL, list spaces, and extract the full textual content of rich wiki pages.
- **Project & Identity Oversight** — Browse available projects and see the identity mappings of the current user automatically.
- **Knowledge Retrieval** — Stream rendered HTML or textual properties of specific Confluence pages directly into your conversation context.

### How it works

1. Subscribe to this secure MCP Server
2. Enter your Atlassian Domain, Email, and API Token
3. Start managing your tickets and documents natively from Claude, Cursor, or any compatible AI client

### Who is this for?

- **Engineering Teams** — check current sprint bugs, retrieve spec documents from Confluence, and trace tickets without leaving your IDE.
- **Product Managers** — pull exact criteria from tickets, summarize complete epics, and draft release notes dynamically.
- **Scrum Masters** — audit sprints, aggregate blockers across boards, and build real-time project views effortlessly.
- **Customer Support** — quickly query Confluence for troubleshooting guides and documentation before replying to customer inquiries.


## Available Tools
- **list_projects**: Useful for discovering project keys needed for querying specific domains or boards.

List all Jira projects
- **search_issues**: Search Jira issues with JQL
- **get_issue**: Get Jira issue details by exact key
- **list_boards**: Often used before retrieving backlogs or active sprints.

List all Jira agile boards
- **list_sprints**: List sprints for a specific Jira board
- **get_myself**: Get current authenticated user information
- **list_spaces**: List all Confluence spaces
- **search_content**: Search Confluence content with CQL
- **get_page**: Get Confluence page rich text content


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atlassian (Jira & Confluence)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get my active Jira sprint tickets related to frontend errors."

**🤖 AI Agent:**
> Executing JQL... I've found 3 `In Progress` high-priority tickets assigned to you mentioning 'frontend' or 'react'. Namely: `ENG-402`, `ENG-489`, and `ENG-501`. Shall I pull the full description of `ENG-402`?

---

**👤 You:**
> "Find Confluence wiki pages detailing the 'Payment Gateway API' architecture."

**🤖 AI Agent:**
> I've searched Confluence (CQL) and surfaced two relevant documentation pages: `Payment Gateway v2` and `Legacy Stripe Migration Docs`. I can stream the complete text of either page now.

---

**👤 You:**
> "List all active boards and the sprints currently running in them."

**🤖 AI Agent:**
> You currently have 4 active Jira Boards. Expanding Board `CORE-BACKEND` reveals an active 'Sprint 44' closing in 2 days. Board `MOBILE-REVAMP` holds 'Sprint 12' with 49 open tasks. Which one would you like to inspect?


## Installation & Usage

To install and use the **Atlassian (Jira & Confluence)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/atlassian-jira-confluence](https://vinkius.com/mcp/atlassian-jira-confluence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
