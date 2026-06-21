# Shortcut MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shortcut)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/shortcut-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/shortcut-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Equip your AI agent to radically manage your Shortcut workspace. Search stories, track epics and iterations, fetch team members, and audit workflows from your IDE.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shortcut** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all stories mentioning 'database timeout' using keyword search."

**🤖 AI Agent:**
> Executing `search_stories` aggressively with query terms `"database timeout"`. Found 3 latent incident logs heavily referencing database connection anomalies tied predominantly to the recent infrastructure rollout. Would you like me to deeply retrieve their nested tasks exploiting `get_story_details` sequentially?

---

**👤 You:**
> "List all ongoing epics and let me evaluate our current roadmap vectors."

**🤖 AI Agent:**
> Triggering the macro-level aggregator `list_epics`. Discovered 8 massive roadmap clusters actively in motion. Noteworthy dense collections prominently included "Q3 Payment Refactor" housing severely delayed workflow statuses and "Client App Redesign" exhibiting strong momentum matrices safely. Should I drill downwards targeting specific iterations next?

---

**👤 You:**
> "List workflows to show me all valid issue states in this organization."

**🤖 AI Agent:**
> Initiating standard extraction accessing `list_workflows` exclusively. Successfully isolated 2 primary organizational workflow state pipelines. 'Engineering Workflow' notably incorporates active transition tags directly translating as 'Unstarted', 'Ready for Dev', 'In Development', securely mapping seamlessly into endpoint resolution state uniquely marked 'Completed'.


## Installation & Usage

To install and use the **Shortcut** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shortcut](https://vinkius.com/mcp/shortcut)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
