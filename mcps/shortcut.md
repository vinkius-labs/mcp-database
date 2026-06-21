# Shortcut MCP Server

Equip your AI agent to radically manage your Shortcut workspace. Search stories, track epics and iterations, fetch team members, and audit workflows from your IDE.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/shortcut)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Grant your AI agent (like Claude or Cursor) absolute administrative dominion over your Shortcut project management environment. The **Shortcut MCP** equips your LLM to act as a fully autonomous scrum master and project auditor. Forget clicking through endless boards—now you can interrogate task backlogs, audit iterations, and orchestrate developers exclusively via natural conversational prompts deeply integrated with the REST API.

### What you can do

- **Deep Story Infiltration** — Rip through dense backlogs via `search_stories`. Need the grit on a specific ticket? Drill down violently with `get_story_details` directly from your IDE to extract every description and sub-task effortlessly
- **Strategic Epic & Sprint Surveillance** — Audit high-level roadmaps invoking `list_epics` and monitor ongoing sprints by extracting `list_iterations` to forecast roadmap failure or success without opening a single tab
- **Team & Workflow Cartography** — Interrogate the hierarchy applying `list_projects`, isolate specific developer IDs using `list_members`, and trace custom state mappings across the pipeline using `list_workflows`

### How it works

1. Anchor this core interface directly within your native MCP agent framework
2. Safely entrench your `SHORTCUT_API_TOKEN` matrix inside the workspace to lock down security boundaries
3. Engage your agent pragmatically: "Find all bugs reported this week and tell me what Epic they belong to based on their details!"


## Available Tools
- **search_stories**: Useful for tracking specific tasks or features.

Searches for stories in Shortcut
- **get_story_details**: Retrieves details for a specific story
- **list_epics**: Lists all epics in Shortcut
- **list_iterations**: Lists all iterations (sprints)
- **list_projects**: Lists all projects
- **list_workflows**: g., "To Do", "Done") a story can be in.

Lists all workflows and their states
- **list_members**: Lists all workspace members


## Installation & Usage

To install and use the **Shortcut** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shortcut](https://vinkius.com/mcp/shortcut)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
